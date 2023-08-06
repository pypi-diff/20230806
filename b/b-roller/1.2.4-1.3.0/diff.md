# Comparing `tmp/b_roller-1.2.4.tar.gz` & `tmp/b_roller-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_roller-1.2.4.tar", max compression
+gzip compressed data, was "b_roller-1.3.0.tar", max compression
```

## Comparing `b_roller-1.2.4.tar` & `b_roller-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       22 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/__init__.py
--rw-r--r--   0        0        0     2937 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/__main__.py
--rw-r--r--   0        0        0      530 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/credits.py
--rw-r--r--   0        0        0     1218 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/iconfinder.py
--rw-r--r--   0        0        0     1566 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/pexels.py
--rw-r--r--   0        0        0     3931 2023-05-30 07:53:09.739147 b_roller-1.2.4/b_roller/youtube.py
--rw-r--r--   0        0        0     1291 2023-05-30 07:53:09.739147 b_roller-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      511 2023-05-30 07:53:09.739147 b_roller-1.2.4/readme.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 b_roller-1.2.4/setup.py
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 b_roller-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/__main__.py
+-rw-r--r--   0        0        0      530 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/credits.py
+-rw-r--r--   0        0        0     1218 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/iconfinder.py
+-rw-r--r--   0        0        0     1566 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/pexels.py
+-rw-r--r--   0        0        0       90 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/settings.py
+-rw-r--r--   0        0        0     5020 2023-08-06 07:06:43.226541 b_roller-1.3.0/b_roller/youtube.py
+-rw-r--r--   0        0        0     1291 2023-08-06 07:06:43.226541 b_roller-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      511 2023-08-06 07:06:43.226541 b_roller-1.3.0/readme.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 b_roller-1.3.0/setup.py
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 b_roller-1.3.0/PKG-INFO
```

### Comparing `b_roller-1.2.4/b_roller/__main__.py` & `b_roller-1.3.0/b_roller/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from b_roller.credits import add_credit_url
 from b_roller.iconfinder import download_icon
@@ -82,14 +83,47 @@
         if api_key := secrets.get("ICONFINDER_API_KEY"):
             title, url = download_icon(url, api_key)
             if not no_credits:
                 add_credit_url(url, title)
 
 
 @app.command()
+def clear_cache():
+    """
+    Clear the cache
+    """
+    from b_roller.settings import cache
+
+    if cache.exists():
+        for file in cache.iterdir():
+            file.unlink()
+    else:
+        cache.mkdir()
+
+
+@app.command()
 def init():
     pass
 
 
+@app.callback()
+def callback(verbose: int = typer.Option(0, "--verbose", "-v", count=True, help="Increase verbosity")):
+    log_level = logging.WARNING
+    if verbose > 1:
+        log_level = logging.DEBUG
+    elif verbose > 0:
+        log_level = logging.INFO
+
+    logger = logging.getLogger("b_roller")
+    logger.setLevel(log_level)
+    handler = logging.StreamHandler()
+    logger.addHandler(handler)
+
+    from b_roller.settings import cache
+
+    cache.mkdir(exist_ok=True)
+    logger.debug(f"Cache: {cache}")
+
+
 if __name__ == "__main__":
     print(get_secrets())
     # app()
```

### Comparing `b_roller-1.2.4/b_roller/credits.py` & `b_roller-1.3.0/b_roller/credits.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.4/b_roller/iconfinder.py` & `b_roller-1.3.0/b_roller/iconfinder.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.4/b_roller/pexels.py` & `b_roller-1.3.0/b_roller/pexels.py`

 * *Files identical despite different names*

### Comparing `b_roller-1.2.4/b_roller/youtube.py` & `b_roller-1.3.0/b_roller/youtube.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import logging
+import shutil
 from pathlib import Path
 from typing import Optional, Union
 from urllib.parse import parse_qs, urlparse
 
 import ffmpeg
 from pytube import YouTube
 from pytube.streams import Stream
 from slugify import slugify
 
+from b_roller.settings import cache
+
 VIDEO_ITAGS = [137, 136, 135, 134, 133, 160]
 AUDIO_ITAGS = [140, 139]
 
+logger = logging.getLogger(__name__)
+
 
 def to_hh_mm_ss(time: Union[int, str, None]) -> str:
     """
     Convert any time defined as a string or seconds to the HH:MM:SS format
     """
     if time is None:
         return None
@@ -62,61 +67,95 @@
     sorted_streams = sorted(
         streams, key=lambda stream: 1000 if stream.itag not in VIDEO_ITAGS else VIDEO_ITAGS.index(stream.itag)
     )
     return sorted_streams[0]
 
 
 def download_audio_only(original_name, yt) -> Path:
-    audio_file = f"{original_name}_audio.mp4"
+    audio_file = cache / f"{original_name}_audio.mp4"
+    logger.debug("Downloading audio")
+    if audio_file.exists():
+        logger.info("Using cached audio")
+        return audio_file
     audio = get_audio_stream(yt)
     audio.download(filename=audio_file)
     return Path(audio_file)
 
 
 def download_video_only(original_name, yt) -> Path:
-    video_file = f"{original_name}_video.mp4"
+    video_file = cache / f"{original_name}_video.mp4"
+    logger.debug("Downloading video")
+    if video_file.exists():
+        logger.info("Using cached video")
+        return video_file
     video = get_video_streams(yt)
     video.download(filename=video_file)
     return Path(video_file)
 
 
 def download_video(
-    video_id: str, start_time: Optional[str] = None, end_time: Optional[str] = None, download: str = "both"
+    video_id: str,
+    start_time: Optional[str] = None,
+    end_time: Optional[str] = None,
+    download: str = "both",
+    output_path: Optional[Path] = None,
 ) -> YouTube:
     yt = YouTube(f"https://www.youtube.com/watch?v={video_id}")
     name_slug = slugify(yt.title)
 
     base_name = f"{name_slug}__{video_id}"
     if download == "both":
         video_file = download_video_only(base_name, yt)
         audio_file = download_audio_only(base_name, yt)
         try:
-            ffmpeg_processing(audio_file, video_file, base_name, end_time, start_time)
-            audio_file.unlink()
-            video_file.unlink()
+            logger.info("Merging audio and video")
+            result = ffmpeg_processing(audio_file, video_file, base_name, end_time, start_time)
         except FileNotFoundError:
             logging.warning("No ffmpeg is not available")
     elif download == "audio":
-        audio_file = download_audio_only(base_name, yt)
+        result = download_audio_only(base_name, yt)
     elif download == "video":
-        video_file = download_video_only(base_name, yt)
+        result = download_video_only(base_name, yt)
+
+    output_file = (output_path or Path.cwd()) / f"{base_name}.mp4"
+    logger.debug(f"Downloaded to {output_file}")
+    shutil.copy(result, output_file)
 
     return yt
 
 
 def ffmpeg_processing(
     audio_file: Path,
     video_file: Path,
     original_name: str,
     end_time: Optional[str] = None,
     start_time: Optional[str] = None,
 ) -> None:
+    output_file = cache / f"{original_name}.mp4"
+    if not output_file.exists():
+        logger.info("Using cached result")
+
+        input_video = ffmpeg.input(str(video_file))
+        input_audio = ffmpeg.input(str(audio_file))
+
+        ffmpeg.concat(input_video, input_audio, v=1, a=1).output(
+            str(output_file),
+        ).run(quiet=True, overwrite_output=True)
+
     ffmpeg_arguments = {}
     if start_time:
-        ffmpeg_arguments["ss"] = start_time
+        ffmpeg_arguments["start"] = start_time
     if end_time:
-        ffmpeg_arguments["to"] = end_time
-    input_video = ffmpeg.input(str(video_file), **ffmpeg_arguments)
-    input_audio = ffmpeg.input(str(audio_file), **ffmpeg_arguments)
-    ffmpeg.concat(input_video, input_audio, v=1, a=1).output(
-        f"./{original_name}.mp4",
-    ).run(quiet=True, overwrite_output=True)
+        ffmpeg_arguments["end"] = end_time
+
+    if ffmpeg_arguments:
+        message = f"Trimming video from {start_time or '-'} to {end_time or '-'}"
+        logger.info(message)
+        result = cache / f"{original_name}_trimmed.mp4"
+
+        ffmpeg.input(str(output_file)).trim(**ffmpeg_arguments).setpts("PTS-STARTPTS").output(
+            str(result),
+        ).run(quiet=True, overwrite_output=True)
+
+        output_file = result
+
+    return output_file
```

### Comparing `b_roller-1.2.4/pyproject.toml` & `b_roller-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b-roller"
-version = "1.2.4"
+version = "1.3.0"
 description = "Download resources from several sources across the web"
 readme = "readme.md"
 authors = ["Antonio Feregrino <antonio.feregrino@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "b_roller" },
 ]
```

### Comparing `b_roller-1.2.4/setup.py` & `b_roller-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'urllib3<=2']
 
 entry_points = \
 {'console_scripts': ['broll = b_roller.__main__:app']}
 
 setup_kwargs = {
     'name': 'b-roller',
-    'version': '1.2.4',
+    'version': '1.3.0',
     'description': 'Download resources from several sources across the web',
     'long_description': '# B-Roller\n\nDownload B-roll footage from YouTube **for fair use purposes**.\n\n## Usage\n\n### Download from YouTube\n\n```\nbroll yt [OPTIONS] URL [START] [END]\n\n  Download content from YouTube\n\nArguments:\n  URL      A video id or a YouTube short/long url  [required]\n  [START]  The desired start of the video in seconds or the format 00:00:00\n  [END]    The desired end of the video in seconds or the format 00:00:00\n```\n\nFor example:\n\n```shell\nbroll yt "https://www.youtube.com/watch?v=QFLiIU8g-R0" 00:10 00:17\n```\n',
     'author': 'Antonio Feregrino',
     'author_email': 'antonio.feregrino@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `b_roller-1.2.4/PKG-INFO` & `b_roller-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-roller
-Version: 1.2.4
+Version: 1.3.0
 Summary: Download resources from several sources across the web
 License: MIT
 Author: Antonio Feregrino
 Author-email: antonio.feregrino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

