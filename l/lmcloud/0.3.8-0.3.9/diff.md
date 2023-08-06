# Comparing `tmp/lmcloud-0.3.8.tar.gz` & `tmp/lmcloud-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcloud-0.3.8.tar", last modified: Sun Jul  9 13:50:23 2023, max compression
+gzip compressed data, was "lmcloud-0.3.9.tar", last modified: Sun Jul  9 14:12:03 2023, max compression
```

## Comparing `lmcloud-0.3.8.tar` & `lmcloud-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 13:50:10.000000 lmcloud-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 13:50:23.701481 lmcloud-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-09 13:50:10.000000 lmcloud-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/lmcloud/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmbluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-09 13:50:10.000000 lmcloud-0.3.8/lmcloud/lmlocalapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:50:23.701481 lmcloud-0.3.8/lmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:50:23.000000 lmcloud-0.3.8/lmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:50:23.701481 lmcloud-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 13:50:10.000000 lmcloud-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:12:03.434445 lmcloud-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-09 14:11:45.000000 lmcloud-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 14:12:03.434445 lmcloud-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-09 14:11:45.000000 lmcloud-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:12:03.434445 lmcloud-0.3.9/lmcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/lmbluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23367 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/lmcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-09 14:11:45.000000 lmcloud-0.3.9/lmcloud/lmlocalapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:12:03.434445 lmcloud-0.3.9/lmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-07-09 14:12:03.000000 lmcloud-0.3.9/lmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 14:12:03.000000 lmcloud-0.3.9/lmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:12:03.000000 lmcloud-0.3.9/lmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-09 14:12:03.000000 lmcloud-0.3.9/lmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 14:12:03.000000 lmcloud-0.3.9/lmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:12:03.434445 lmcloud-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-09 14:11:45.000000 lmcloud-0.3.9/setup.py
```

### Comparing `lmcloud-0.3.8/LICENSE` & `lmcloud-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/PKG-INFO` & `lmcloud-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.8/README.md` & `lmcloud-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/lmcloud/const.py` & `lmcloud-0.3.9/lmcloud/const.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/lmcloud/helpers.py` & `lmcloud-0.3.9/lmcloud/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def parse_preinfusion_settings(config) -> dict:
     parsed = {}
     i = 1
     preinfusion_settings = config["preinfusionSettings"]
     for group in preinfusion_settings["Group1"]:
         parsed[f"prebrewing_ton_k{i}"] = group["preWetTime"]
         parsed[f"prebrewing_toff_k{i}"] = group["preWetHoldTime"]
-        parsed[f"preinfusion_ton_k{i}"] = group["preWetTime"]
+        parsed[f"preinfusion_k{i}"] = group["preWetTime"]
         i += 1
     return parsed
 
 def parse_doses(config):
     parsed = {}
     i = 1
     groupCapabilities = config["groupCapabilities"]
```

### Comparing `lmcloud-0.3.8/lmcloud/lmbluetooth.py` & `lmcloud-0.3.9/lmcloud/lmbluetooth.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/lmcloud/lmcloud.py` & `lmcloud-0.3.9/lmcloud/lmcloud.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/lmcloud/lmlocalapi.py` & `lmcloud-0.3.9/lmcloud/lmlocalapi.py`

 * *Files identical despite different names*

### Comparing `lmcloud-0.3.8/lmcloud.egg-info/PKG-INFO` & `lmcloud-0.3.9/lmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmcloud
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python implementation of the new La Marzocco API
 Home-page: https://github.com/zweckj/lmcloud
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `lmcloud-0.3.8/setup.py` & `lmcloud-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="lmcloud",
-    version="0.3.8",
+    version="0.3.9",
     description="A Python implementation of the new La Marzocco API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/lmcloud",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

