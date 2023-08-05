# Comparing `tmp/karaoke_generator-0.4.3.tar.gz` & `tmp/karaoke_generator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karaoke_generator-0.4.3.tar", max compression
+gzip compressed data, was "karaoke_generator-0.5.1.tar", max compression
```

## Comparing `karaoke_generator-0.4.3.tar` & `karaoke_generator-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2360 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/README.md
--rw-r--r--   0        0        0       40 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/__init__.py
--rw-r--r--   0        0        0    15081 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/generator.py
--rw-r--r--   0        0        0        0 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/utils/__init__.py
--rwxr-xr-x   0        0        0     3471 2023-07-09 20:12:18.911453 karaoke_generator-0.4.3/karaoke_generator/utils/cli.py
--rw-r--r--   0        0        0     1528 2023-07-09 20:12:18.915454 karaoke_generator-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 karaoke_generator-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2360 2023-08-05 23:06:22.442347 karaoke_generator-0.5.1/README.md
+-rw-r--r--   0        0        0       40 2023-08-05 23:06:22.442347 karaoke_generator-0.5.1/karaoke_generator/__init__.py
+-rw-r--r--   0        0        0    15758 2023-08-05 23:06:22.442347 karaoke_generator-0.5.1/karaoke_generator/generator.py
+-rw-r--r--   0        0        0        0 2023-08-05 23:06:22.442347 karaoke_generator-0.5.1/karaoke_generator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3471 2023-08-05 23:06:22.442347 karaoke_generator-0.5.1/karaoke_generator/utils/cli.py
+-rw-r--r--   0        0        0     1528 2023-08-05 23:06:22.446347 karaoke_generator-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 karaoke_generator-0.5.1/PKG-INFO
```

### Comparing `karaoke_generator-0.4.3/README.md` & `karaoke_generator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `karaoke_generator-0.4.3/karaoke_generator/generator.py` & `karaoke_generator-0.5.1/karaoke_generator/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,24 @@
         elif os.path.exists(self.input_path):
             self.audio_file = self.input_path
             self.input_source_slug = slugify.slugify(os.path.basename(self.audio_file), lowercase=False)
             self.logger.debug(f"Input path was valid file path, set audio_file and input_source_slug: {self.input_source_slug}")
         else:
             raise Exception("Input path must be either a valid file path or URL")
 
-        self.input_source_slug = "-".join(filter(None, [slugify.slugify(self.artist), slugify.slugify(self.title), self.input_source_slug]))
+        self.input_source_slug = "-".join(
+            filter(
+                None,
+                [
+                    slugify.slugify(self.artist) if self.artist else None,
+                    slugify.slugify(self.title) if self.title else None,
+                    self.input_source_slug,
+                ],
+            )
+        )
 
     def generate(self):
         self.logger.info("KaraokeGenerator beginning generation")
 
         if self.audio_file is None and self.source_url is not None:
             self.logger.debug(f"audio_file is none and source_url is {self.source_url}, fetching video from youtube")
             self.download_youtube_video()
@@ -232,23 +241,33 @@
                 ydl.download([self.source_url])
                 shutil.move(temp_download_filepath, youtube_info["download_filepath"])
                 self.youtube_video_file = youtube_info["download_filepath"]
                 self.logger.debug(f"successfully downloaded youtube video to path: {self.youtube_video_file}")
 
         if self.title is None:
             self.logger.debug(f"Song title not specified, attempting to split from YouTube title: {youtube_info['title']}")
-            # Define the hyphen variations pattern
-            hyphen_pattern = regex.compile(r" [^[:ascii:]-_\p{Dash}] ")
-            # Split the string using the hyphen variations pattern
-            title_parts = hyphen_pattern.split(youtube_info["title"])
 
-            self.artist = title_parts[0]
-            self.title = title_parts[1]
+            # Define the pattern using regular expressions for possible hyphen-like characters
+            hyphen_pattern = regex.compile(r" [-\u2010-\u2015] ")
+
+            # Split the string using the hyphen pattern
+            title_parts = hyphen_pattern.split(youtube_info["title"], maxsplit=1)
+
+            if len(title_parts) < 2:
+                self.artist = None
+                self.title = None
+                self.logger.warning("Failed to extract artist and title from YouTube title.")
+            else:
+                self.artist = title_parts[0].strip()
+                self.title = title_parts[1].strip()
+
+                # Optional: further split to remove additional info, such as "(Painkiller Sessions 1990) [Audio]"
+                self.title = self.title.split(" (", 1)[0].strip()
 
-            print(f"Guessed metadata from title: Artist: {self.artist}, Title: {self.title}")
+                self.logger.debug(f"Guessed metadata from title: Artist: {self.artist}, Title: {self.title}")
 
         # Extract audio to WAV file using ffmpeg
         self.audio_file = os.path.join(self.cache_dir, self.output_filename_slug + ".wav")
         if os.path.isfile(self.audio_file):
             self.logger.debug(f"Existing file found at self.audio_file, skipping extraction: {self.audio_file}")
         else:
             self.logger.debug(f"Extracting audio from {self.youtube_video_file} to {self.audio_file}")
```

### Comparing `karaoke_generator-0.4.3/karaoke_generator/utils/cli.py` & `karaoke_generator-0.5.1/karaoke_generator/utils/cli.py`

 * *Files identical despite different names*

### Comparing `karaoke_generator-0.4.3/pyproject.toml` & `karaoke_generator-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "karaoke-generator"
-version = "0.4.3"
+version = "0.5.1"
 description = "Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "karaoke_generator" }]
 homepage = "https://github.com/karaokenerds/karaoke-generator"
 repository = "https://github.com/karaokenerds/karaoke-generator"
 documentation = "https://github.com/karaokenerds/karaoke-generator/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 yt-dlp = "^2023.6.22"
 pydub = "^0.25.1"
-audio-separator = "^0.3"
+audio-separator = "^0.6"
 lyrics-transcriber = "^0.6.3"
 python-slugify = "^8.0.1"
 regex = "^2023.6.3"
 tldextract = "^3.4"
 # Note: after adding lyrics-transcriber with poetry lock, I then removed all traces of triton
 # from poetry.lock before running poetry install, as triton doesn't support macOS but isn't actually needed for whisper.
 # This was the only way I was able to get a working cross-platform build published to PyPI.
```

### Comparing `karaoke_generator-0.4.3/PKG-INFO` & `karaoke_generator-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: karaoke-generator
-Version: 0.4.3
+Version: 0.5.1
 Summary: Fully automated creation of _acceptable_ karaoke music videos from any music on YouTube, using open source tools and AI (e.g. Whisper and MDX-Net)
 Home-page: https://github.com/karaokenerds/karaoke-generator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: audio-separator (>=0.3,<0.4)
+Requires-Dist: audio-separator (>=0.6,<0.7)
 Requires-Dist: lyrics-transcriber (>=0.6.3,<0.7.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: python-slugify (>=8.0.1,<9.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: tldextract (>=3.4,<4.0)
 Requires-Dist: yt-dlp (>=2023.6.22,<2024.0.0)
 Project-URL: Documentation, https://github.com/karaokenerds/karaoke-generator/blob/main/README.md
```

