# Comparing `tmp/lyrics_transcriber-0.6.4.tar.gz` & `tmp/lyrics_transcriber-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.6.4.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.6.5.tar", max compression
```

## Comparing `lyrics_transcriber-0.6.4.tar` & `lyrics_transcriber-0.6.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/LICENSE
--rw-r--r--   0        0        0     3626 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/README.md
--rw-r--r--   0        0        0       94 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0    13166 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     4176 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0     1668 2023-07-09 20:13:23.590120 lyrics_transcriber-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3626 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/README.md
+-rw-r--r--   0        0        0       94 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0    13166 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     4176 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0     1668 2023-08-05 22:08:36.461130 lyrics_transcriber-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     4931 1970-01-01 00:00:00.000000 lyrics_transcriber-0.6.5/PKG-INFO
```

### Comparing `lyrics_transcriber-0.6.4/LICENSE` & `lyrics_transcriber-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.4/README.md` & `lyrics_transcriber-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.4/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.6.5/lyrics_transcriber/transcriber.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.4/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.6.5/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.6.4/pyproject.toml` & `lyrics_transcriber-0.6.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.6.4"
+version = "0.6.5"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "lyrics_transcriber" }]
 homepage = "https://github.com/karaokenerds/python-lyrics-transcriber"
 repository = "https://github.com/karaokenerds/python-lyrics-transcriber"
@@ -16,15 +16,15 @@
 Cython = "^0"
 dtw-python = "^1"
 llvmlite = "^0"
 numba = "^0.57"
 numpy = "^1"
 onnx = "^1"
 onnxruntime = "^1"
-torch = "^1"
+torch = ">1"
 tqdm = "^4"
 lyricsgenius = "^3"
 python-slugify = "^8"
 syrics = "^0"
 openai-whisper = "20230314"
 whisper-timestamped = "^1"
 # Note: after adding openai-whisper and whisper-timestamped with poetry lock, I then removed all traces of triton
```

### Comparing `lyrics_transcriber-0.6.4/PKG-INFO` & `lyrics_transcriber-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrics-transcriber
-Version: 0.6.4
+Version: 0.6.5
 Summary: Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify
 Home-page: https://github.com/karaokenerds/python-lyrics-transcriber
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: onnx (>=1,<2)
 Requires-Dist: onnxruntime (>=1,<2)
 Requires-Dist: openai-whisper (==20230314)
 Requires-Dist: python-slugify (>=8,<9)
 Requires-Dist: syrics (>=0,<1)
-Requires-Dist: torch (>=1,<2)
+Requires-Dist: torch (>1)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: whisper-timestamped (>=1,<2)
 Project-URL: Documentation, https://github.com/karaokenerds/python-lyrics-transcriber/blob/main/README.md
 Project-URL: Repository, https://github.com/karaokenerds/python-lyrics-transcriber
 Description-Content-Type: text/markdown
 
 # Lyrics Transcriber 🎶
```

