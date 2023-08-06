# Comparing `tmp/janus_client-0.4.0.tar.gz` & `tmp/janus_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_client-0.4.0.tar", max compression
+gzip compressed data, was "janus_client-0.4.1.tar", max compression
```

## Comparing `janus_client-0.4.0.tar` & `janus_client-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      451 2023-08-06 06:54:43.649064 janus_client-0.4.0/janus_client/__init__.py
--rw-r--r--   0        0        0    11283 2023-08-05 06:20:05.227375 janus_client-0.4.0/janus_client/core.py
--rw-r--r--   0        0        0     7592 2023-07-29 16:26:44.628495 janus_client-0.4.0/janus_client/media.py
--rw-r--r--   0        0        0     2816 2023-08-05 13:01:11.384945 janus_client-0.4.0/janus_client/plugin_base.py
--rw-r--r--   0        0        0     1238 2023-08-05 12:51:20.448331 janus_client-0.4.0/janus_client/plugin_video_call.py
--rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.4.0/janus_client/plugin_video_room.py
--rw-r--r--   0        0        0     7975 2023-08-05 13:30:07.030590 janus_client-0.4.0/janus_client/plugin_video_room_ffmpeg.py
--rw-r--r--   0        0        0     4022 2023-08-06 06:16:17.063277 janus_client-0.4.0/janus_client/session.py
--rw-r--r--   0        0        0     8072 2023-08-06 08:59:28.189276 janus_client-0.4.0/janus_client/transport.py
--rw-r--r--   0        0        0     4330 2023-08-06 08:57:53.281310 janus_client-0.4.0/janus_client/transport_http.py
--rw-r--r--   0        0        0     2660 2023-08-06 06:12:27.825554 janus_client-0.4.0/janus_client/transport_websocket.py
--rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.4.0/LICENSE
--rw-r--r--   0        0        0      949 2023-08-06 09:09:28.545057 janus_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4662 2023-08-06 09:05:43.870792 janus_client-0.4.0/README.md
--rw-r--r--   0        0        0     5716 1970-01-01 00:00:00.000000 janus_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-08-06 06:54:43.649064 janus_client-0.4.1/janus_client/__init__.py
+-rw-r--r--   0        0        0    11283 2023-08-05 06:20:05.227375 janus_client-0.4.1/janus_client/core.py
+-rw-r--r--   0        0        0     7592 2023-07-29 16:26:44.628495 janus_client-0.4.1/janus_client/media.py
+-rw-r--r--   0        0        0     2816 2023-08-05 13:01:11.384945 janus_client-0.4.1/janus_client/plugin_base.py
+-rw-r--r--   0        0        0     1238 2023-08-05 12:51:20.448331 janus_client-0.4.1/janus_client/plugin_video_call.py
+-rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.4.1/janus_client/plugin_video_room.py
+-rw-r--r--   0        0        0     7975 2023-08-05 13:30:07.030590 janus_client-0.4.1/janus_client/plugin_video_room_ffmpeg.py
+-rw-r--r--   0        0        0     4022 2023-08-06 06:16:17.063277 janus_client-0.4.1/janus_client/session.py
+-rw-r--r--   0        0        0     8072 2023-08-06 08:59:28.189276 janus_client-0.4.1/janus_client/transport.py
+-rw-r--r--   0        0        0     4330 2023-08-06 08:57:53.281310 janus_client-0.4.1/janus_client/transport_http.py
+-rw-r--r--   0        0        0     2660 2023-08-06 06:12:27.825554 janus_client-0.4.1/janus_client/transport_websocket.py
+-rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0      941 2023-08-06 09:13:12.529772 janus_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4662 2023-08-06 09:05:43.870792 janus_client-0.4.1/README.md
+-rw-r--r--   0        0        0     5708 1970-01-01 00:00:00.000000 janus_client-0.4.1/PKG-INFO
```

### Comparing `janus_client-0.4.0/janus_client/core.py` & `janus_client-0.4.1/janus_client/core.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/media.py` & `janus_client-0.4.1/janus_client/media.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/plugin_base.py` & `janus_client-0.4.1/janus_client/plugin_base.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/plugin_video_call.py` & `janus_client-0.4.1/janus_client/plugin_video_call.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/plugin_video_room.py` & `janus_client-0.4.1/janus_client/plugin_video_room.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/plugin_video_room_ffmpeg.py` & `janus_client-0.4.1/janus_client/plugin_video_room_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/session.py` & `janus_client-0.4.1/janus_client/session.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/transport.py` & `janus_client-0.4.1/janus_client/transport.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/transport_http.py` & `janus_client-0.4.1/janus_client/transport_http.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/janus_client/transport_websocket.py` & `janus_client-0.4.1/janus_client/transport_websocket.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/LICENSE` & `janus_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/pyproject.toml` & `janus_client-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "janus-client"
-version = "0.4.0"
-description = "Janus gatewau webrtc async client in Python."
+version = "0.4.1"
+description = "Janus WebRTC async client in Python."
 authors = ["Joseph Lim <josephlim_94@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "janus_client"}]
 repository = "https://github.com/josephlim94/janus_gst_client_py"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `janus_client-0.4.0/README.md` & `janus_client-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `janus_client-0.4.0/PKG-INFO` & `janus_client-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: janus-client
-Version: 0.4.0
-Summary: Janus gatewau webrtc async client in Python.
+Version: 0.4.1
+Summary: Janus WebRTC async client in Python.
 Home-page: https://github.com/josephlim94/janus_gst_client_py
 License: MIT
 Author: Joseph Lim
 Author-email: josephlim_94@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

