# Comparing `tmp/aiohuesyncbox-0.0.23.tar.gz` & `tmp/aiohuesyncbox-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohuesyncbox-0.0.23.tar", last modified: Thu Aug  3 18:57:43 2023, max compression
+gzip compressed data, was "aiohuesyncbox-0.0.24.tar", last modified: Sun Aug  6 13:17:16 2023, max compression
```

## Comparing `aiohuesyncbox-0.0.23.tar` & `aiohuesyncbox-0.0.24.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:57:43.079273 aiohuesyncbox-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-03 18:57:43.079273 aiohuesyncbox-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:57:43.079273 aiohuesyncbox-0.0.23/aiohuesyncbox/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/hdmi.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/hsb_cacert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/hue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/huesyncbox.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/aiohuesyncbox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:57:43.079273 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-03 18:57:43.000000 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-03 18:57:43.000000 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:57:43.000000 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 18:57:43.000000 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 18:57:43.000000 aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 18:57:43.079273 aiohuesyncbox-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-03 18:57:31.000000 aiohuesyncbox-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:16.053260 aiohuesyncbox-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-06 13:17:16.053260 aiohuesyncbox-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:16.053260 aiohuesyncbox-0.0.24/aiohuesyncbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/hdmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/hsb_cacert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/hue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/huesyncbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/aiohuesyncbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:17:16.053260 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-06 13:17:16.000000 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-06 13:17:16.000000 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:17:16.000000 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 13:17:16.000000 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 13:17:16.000000 aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-06 13:17:16.053260 aiohuesyncbox-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-06 13:17:07.000000 aiohuesyncbox-0.0.24/setup.py
```

### Comparing `aiohuesyncbox-0.0.23/LICENSE` & `aiohuesyncbox-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/PKG-INFO` & `aiohuesyncbox-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.23
+Version: 0.0.24
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiohuesyncbox-0.0.23/README.rst` & `aiohuesyncbox-0.0.24/README.rst`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/behavior.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/behavior.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/device.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/device.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/errors.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/errors.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/execution.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/execution.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/hdmi.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/hdmi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List
 from .helpers import generate_attribute_string
 
+INPUTS = ["input1", "input2", "input3", "input4"]
 
 class Input:
-    def __init__(self, id: str, raw: Dict) -> None:
-        self.id = id
+    def __init__(self, raw: Dict) -> None:
         self._raw = raw
 
     @property
     def name(self) -> str:
         """Friendly name of the input."""
         return self._raw["name"]
 
@@ -52,20 +52,19 @@
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Hdmi):
             return NotImplemented
         return self._raw == other._raw
 
     def _update_inputs_and_output(self) -> None:
-        inputs = []
-        for key, value in self._raw.items():
-            if key.startswith("input"):
-                inputs.append(Input(key, value))
-        self._inputs = inputs
-        self._output = Output("output", self._raw["output"])
+        for input_id in INPUTS:
+            if input_id in self._raw:
+                input = Input(self._raw[input_id])
+                setattr(self, f"_{input_id}", input)
+        self._output = Output(self._raw["output"])
 
     @property
     def content_specs(self) -> str:
         """Content specs of current input of huesyncbox."""
         return self._raw["contentSpecs"]
 
     @property
@@ -75,17 +74,32 @@
 
     @property
     def audio_sync_supported(self) -> bool:
         """Indicates if syncing is supported on audio content."""
         return self._raw["audioSyncSupported"]
 
     @property
-    def inputs(self) -> List[Input]:
-        """HDMI inputs of the huesyncbox."""
-        return self._inputs
+    def input1(self) -> Input:
+        """HDMI input 1 of the huesyncbox."""
+        return getattr(self, "_input1")
+
+    @property
+    def input2(self) -> Input:
+        """HDMI input 2 of the huesyncbox."""
+        return getattr(self, "_input2")
+
+    @property
+    def input3(self) -> Input:
+        """HDMI input 3 of the huesyncbox."""
+        return getattr(self, "_input3")
+
+    @property
+    def input4(self) -> Input:
+        """HDMI input 4 of the huesyncbox."""
+        return getattr(self, "_input4")
 
     @property
     def output(self) -> Output:
         """HDMI output of the huesyncbox."""
         return self._output
 
     async def update(self) -> None:
```

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/hsb_cacert.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/hsb_cacert.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/hue.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/hue.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox/huesyncbox.py` & `aiohuesyncbox-0.0.24/aiohuesyncbox/huesyncbox.py`

 * *Files identical despite different names*

### Comparing `aiohuesyncbox-0.0.23/aiohuesyncbox.egg-info/PKG-INFO` & `aiohuesyncbox-0.0.24/aiohuesyncbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohuesyncbox
-Version: 0.0.23
+Version: 0.0.24
 Summary: Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.
 Home-page: https://github.com/mvdwetering/aiohuesyncbox
 Author: Michel van de Wetering
 Author-email: michel.van.de.wetering@gmail.com
 License: Apache License 2.0
 Keywords: automation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiohuesyncbox-0.0.23/setup.py` & `aiohuesyncbox-0.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     long_description = f.read()
 
 setup(
     name="aiohuesyncbox",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.0.23",
+    version="0.0.24",
     description="Asyncio package to communicate with a Philips Hue Play HDMI Sync Box.",
     long_description=long_description,
     # The project's main homepage.
     url="https://github.com/mvdwetering/aiohuesyncbox",
     # Author details
     author="Michel van de Wetering",
     author_email="michel.van.de.wetering@gmail.com",
```

