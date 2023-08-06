# Comparing `tmp/manim_voiceover-0.3.3.post0.tar.gz` & `tmp/manim_voiceover-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_voiceover-0.3.3.post0.tar", max compression
+gzip compressed data, was "manim_voiceover-0.3.4.tar", max compression
```

## Comparing `manim_voiceover-0.3.3.post0.tar` & `manim_voiceover-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1088 2023-05-27 13:25:03.684307 manim_voiceover-0.3.3.post0/LICENSE
--rw-r--r--   0        0        0     2832 2023-05-27 13:25:03.684307 manim_voiceover-0.3.3.post0/README.md
--rw-r--r--   0        0        0      203 2023-05-27 13:25:03.688307 manim_voiceover-0.3.3.post0/manim_voiceover/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-27 13:25:03.688307 manim_voiceover-0.3.3.post0/manim_voiceover/defaults.py
--rw-r--r--   0        0        0     6048 2023-05-27 13:25:03.688307 manim_voiceover-0.3.3.post0/manim_voiceover/helper.py
--rw-r--r--   0        0        0      658 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/modify_audio.py
--rw-r--r--   0        0        0      343 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/__init__.py
--rw-r--r--   0        0        0     8972 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/azure.py
--rw-r--r--   0        0        0     7794 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/base.py
--rw-r--r--   0        0        0     2759 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/coqui.py
--rw-r--r--   0        0        0     2799 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/gtts.py
--rw-r--r--   0        0        0     1546 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/pyttsx3.py
--rw-r--r--   0        0        0     3992 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/recorder/__init__.py
--rw-r--r--   0        0        0     7901 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/recorder/utility.py
--rw-r--r--   0        0        0     6047 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/services/stitcher.py
--rw-r--r--   0        0        0     5053 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/tracker.py
--rw-r--r--   0        0        0      584 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/translate/__init__.py
--rw-r--r--   0        0        0     6395 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/translate/gettext_utils.py
--rw-r--r--   0        0        0     3814 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/translate/render.py
--rw-r--r--   0        0        0     2510 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/translate/translate.py
--rw-r--r--   0        0        0     7104 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/manim_voiceover/voiceover_scene.py
--rw-r--r--   0        0        0     3432 2023-05-27 13:25:03.692307 manim_voiceover-0.3.3.post0/pyproject.toml
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 manim_voiceover-0.3.3.post0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-08-06 09:47:20.211854 manim_voiceover-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2832 2023-08-06 09:47:20.211854 manim_voiceover-0.3.4/README.md
+-rw-r--r--   0        0        0      203 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/__init__.py
+-rw-r--r--   0        0        0     1779 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/defaults.py
+-rw-r--r--   0        0        0     6048 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/helper.py
+-rw-r--r--   0        0        0      658 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/modify_audio.py
+-rw-r--r--   0        0        0      343 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/__init__.py
+-rw-r--r--   0        0        0     8972 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/azure.py
+-rw-r--r--   0        0        0     7794 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/base.py
+-rw-r--r--   0        0        0     2759 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/coqui.py
+-rw-r--r--   0        0        0     2799 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/gtts.py
+-rw-r--r--   0        0        0     1546 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/pyttsx3.py
+-rw-r--r--   0        0        0     3992 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/recorder/__init__.py
+-rw-r--r--   0        0        0     8549 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/recorder/utility.py
+-rw-r--r--   0        0        0     6047 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/services/stitcher.py
+-rw-r--r--   0        0        0     5053 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/tracker.py
+-rw-r--r--   0        0        0      584 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/translate/__init__.py
+-rw-r--r--   0        0        0     6395 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/translate/gettext_utils.py
+-rw-r--r--   0        0        0     3814 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/translate/render.py
+-rw-r--r--   0        0        0     2510 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/translate/translate.py
+-rw-r--r--   0        0        0     7104 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/manim_voiceover/voiceover_scene.py
+-rw-r--r--   0        0        0     3427 2023-08-06 09:47:20.219854 manim_voiceover-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5372 1970-01-01 00:00:00.000000 manim_voiceover-0.3.4/PKG-INFO
```

### Comparing `manim_voiceover-0.3.3.post0/LICENSE` & `manim_voiceover-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/README.md` & `manim_voiceover-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/defaults.py` & `manim_voiceover-0.3.4/manim_voiceover/defaults.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/helper.py` & `manim_voiceover-0.3.4/manim_voiceover/helper.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/modify_audio.py` & `manim_voiceover-0.3.4/manim_voiceover/modify_audio.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/azure.py` & `manim_voiceover-0.3.4/manim_voiceover/services/azure.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/base.py` & `manim_voiceover-0.3.4/manim_voiceover/services/base.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/coqui.py` & `manim_voiceover-0.3.4/manim_voiceover/services/coqui.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/gtts.py` & `manim_voiceover-0.3.4/manim_voiceover/services/gtts.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/pyttsx3.py` & `manim_voiceover-0.3.4/manim_voiceover/services/pyttsx3.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/recorder/__init__.py` & `manim_voiceover-0.3.4/manim_voiceover/services/recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/recorder/utility.py` & `manim_voiceover-0.3.4/manim_voiceover/services/recorder/utility.py`

 * *Files 21% similar despite different names*

```diff
@@ -137,38 +137,53 @@
 
         try:
             self.device_index = int(input())
             device_name = self.audio.get_device_info_by_host_api_device_index(
                 0, self.device_index
             ).get("name")
             self._set_channels_from_device_index(self.device_index)
+            self._set_rate_from_device_index(self.device_index)
             print("Selected device:", device_name)
         except KeyboardInterrupt:
             print("KeyboardInterrupt")
             exit()
         except:
             print("Invalid device index. Please try again.")
             self._set_device()
 
         return
 
     def _set_channels_from_device_index(self, device_index):
-        self.channels = self.audio.get_device_info_by_host_api_device_index(
+        channels_from_device = self.audio.get_device_info_by_host_api_device_index(
             0, device_index
         ).get("maxInputChannels")
+        if self.channels is None:
+            self.channels = channels_from_device
+        else:
+            self.channels = min(self.channels, channels_from_device)
+
+    def _set_rate_from_device_index(self, device_index):
+        rate_from_device = self.audio.get_device_info_by_host_api_device_index(
+            0, device_index
+        ).get("defaultSampleRate")
+        if self.rate is None:
+            self.rate = int(rate_from_device)
+        else:
+            self.rate = int(min(self.rate, rate_from_device))
 
     def _record_task(self, path):
         if self.listener.key_pressed and not self.started:
             # Start the recording
             try:
                 self.stream = self.audio.open(
                     format=self.format,
                     channels=self.channels,
                     rate=self.rate,
                     input=True,
+                    input_device_index=self.device_index,
                     frames_per_buffer=self.chunk,
                     stream_callback=self.callback,
                 )
                 print("Stream active:", self.stream.is_active())
                 self.started = True
                 print("start Stream")
             except:
```

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/services/stitcher.py` & `manim_voiceover-0.3.4/manim_voiceover/services/stitcher.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/tracker.py` & `manim_voiceover-0.3.4/manim_voiceover/tracker.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/translate/__init__.py` & `manim_voiceover-0.3.4/manim_voiceover/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/translate/gettext_utils.py` & `manim_voiceover-0.3.4/manim_voiceover/translate/gettext_utils.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/translate/render.py` & `manim_voiceover-0.3.4/manim_voiceover/translate/render.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/translate/translate.py` & `manim_voiceover-0.3.4/manim_voiceover/translate/translate.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/manim_voiceover/voiceover_scene.py` & `manim_voiceover-0.3.4/manim_voiceover/voiceover_scene.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.3.post0/pyproject.toml` & `manim_voiceover-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-voiceover"
-version = "0.3.3.post"
+version = "0.3.4"
 description = "Manim plugin for all things voiceover"
 authors = ["The Manim Community Developers <contact@manim.community>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "manim_voiceover" }]
 repository = "https://github.com/ManimCommunity/manim-voiceover"
 homepage = "https://voiceover.manim.community"
```

### Comparing `manim_voiceover-0.3.3.post0/PKG-INFO` & `manim_voiceover-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-voiceover
-Version: 0.3.3.post0
+Version: 0.3.4
 Summary: Manim plugin for all things voiceover
 Home-page: https://voiceover.manim.community
 License: MIT
 Keywords: text-to-speech,tts,voiceover,manim,recording,speech synthesis,math animations
 Author: The Manim Community Developers
 Author-email: contact@manim.community
 Requires-Python: >=3.8,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.3.post0 Summary: Manim
+Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.4 Summary: Manim
 plugin for all things voiceover Home-page: https://voiceover.manim.community
 License: MIT Keywords: text-to-speech,tts,voiceover,manim,recording,speech
 synthesis,math animations Author: The Manim Community Developers Author-email:
 contact@manim.community Requires-Python: >=3.8,<4 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

