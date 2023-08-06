# Comparing `tmp/pytrafikverket-0.3.3.tar.gz` & `tmp/pytrafikverket-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrafikverket-0.3.3.tar", last modified: Sun May  7 18:27:15 2023, max compression
+gzip compressed data, was "pytrafikverket-0.3.4.tar", last modified: Sun Aug  6 16:58:29 2023, max compression
```

## Comparing `pytrafikverket-0.3.3.tar` & `pytrafikverket-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:27:15.143665 pytrafikverket-0.3.3/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.3/LICENSE
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-07 18:27:15.143665 pytrafikverket-0.3.3/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.3/README.md
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:27:15.133665 pytrafikverket-0.3.3/pytrafikverket/
--rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.3/pytrafikverket/__init__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-06 08:48:37.000000 pytrafikverket-0.3.3/pytrafikverket/__main__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.3/pytrafikverket/exceptions.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.3/pytrafikverket/py.typed
--rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-06 08:48:37.000000 pytrafikverket-0.3.3/pytrafikverket/trafikverket.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.3/pytrafikverket/trafikverket_camera.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.3/pytrafikverket/trafikverket_ferry.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)    12067 2023-05-07 18:26:59.000000 pytrafikverket-0.3.3/pytrafikverket/trafikverket_train.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     7309 2023-05-04 16:19:35.000000 pytrafikverket-0.3.3/pytrafikverket/trafikverket_weather.py
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:27:15.143665 pytrafikverket-0.3.3/pytrafikverket.egg-info/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-07 18:27:15.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-07 18:27:15.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/SOURCES.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-07 18:27:15.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/dependency_links.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-07 18:27:15.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/requires.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-07 18:27:15.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/top_level.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.3/pytrafikverket.egg-info/zip-safe
--rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-07 18:27:15.143665 pytrafikverket-0.3.3/setup.cfg
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-07 18:26:59.000000 pytrafikverket-0.3.3/setup.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-08-06 16:58:29.369166 pytrafikverket-0.3.4/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.4/LICENSE
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-08-06 16:58:29.369166 pytrafikverket-0.3.4/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-08-06 16:57:02.000000 pytrafikverket-0.3.4/README.md
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-08-06 16:58:29.369166 pytrafikverket-0.3.4/pytrafikverket/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.4/pytrafikverket/__init__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-08-06 16:55:20.000000 pytrafikverket-0.3.4/pytrafikverket/__main__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.4/pytrafikverket/exceptions.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.4/pytrafikverket/py.typed
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-06 08:48:37.000000 pytrafikverket-0.3.4/pytrafikverket/trafikverket.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.4/pytrafikverket/trafikverket_camera.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.4/pytrafikverket/trafikverket_ferry.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)    12067 2023-08-06 16:56:32.000000 pytrafikverket-0.3.4/pytrafikverket/trafikverket_train.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     7309 2023-05-04 16:19:35.000000 pytrafikverket-0.3.4/pytrafikverket/trafikverket_weather.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-08-06 16:58:29.369166 pytrafikverket-0.3.4/pytrafikverket.egg-info/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-08-06 16:58:29.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-08-06 16:58:29.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/SOURCES.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-08-06 16:58:29.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/dependency_links.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-08-06 16:58:29.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/requires.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-08-06 16:58:29.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/top_level.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.4/pytrafikverket.egg-info/zip-safe
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-08-06 16:58:29.369166 pytrafikverket-0.3.4/setup.cfg
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-08-06 16:56:45.000000 pytrafikverket-0.3.4/setup.py
```

### Comparing `pytrafikverket-0.3.3/LICENSE` & `pytrafikverket-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/PKG-INFO` & `pytrafikverket-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.3
+Version: 0.3.4
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytrafikverket
 python module for communicating with the swedish trafikverket api
 
-Development and testing done with 3.10
+Development and testing done with 3.11
 
 ## Code example
 ```python
 from pytrafikverket import TrafikverketTrain, StationInfo
 import aiohttp
 import asyncio
 import async_timeout
```

### Comparing `pytrafikverket-0.3.3/README.md` & `pytrafikverket-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pytrafikverket
 python module for communicating with the swedish trafikverket api
 
-Development and testing done with 3.10
+Development and testing done with 3.11
 
 ## Code example
 ```python
 from pytrafikverket import TrafikverketTrain, StationInfo
 import aiohttp
 import asyncio
 import async_timeout
```

### Comparing `pytrafikverket-0.3.3/pytrafikverket/__init__.py` & `pytrafikverket-0.3.4/pytrafikverket/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/__main__.py` & `pytrafikverket-0.3.4/pytrafikverket/__main__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/exceptions.py` & `pytrafikverket-0.3.4/pytrafikverket/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/trafikverket.py` & `pytrafikverket-0.3.4/pytrafikverket/trafikverket.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/trafikverket_camera.py` & `pytrafikverket-0.3.4/pytrafikverket/trafikverket_camera.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/trafikverket_ferry.py` & `pytrafikverket-0.3.4/pytrafikverket/trafikverket_ferry.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/trafikverket_train.py` & `pytrafikverket-0.3.4/pytrafikverket/trafikverket_train.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket/trafikverket_weather.py` & `pytrafikverket-0.3.4/pytrafikverket/trafikverket_weather.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/pytrafikverket.egg-info/PKG-INFO` & `pytrafikverket-0.3.4/pytrafikverket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.3
+Version: 0.3.4
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytrafikverket
 python module for communicating with the swedish trafikverket api
 
-Development and testing done with 3.10
+Development and testing done with 3.11
 
 ## Code example
 ```python
 from pytrafikverket import TrafikverketTrain, StationInfo
 import aiohttp
 import asyncio
 import async_timeout
```

### Comparing `pytrafikverket-0.3.3/pytrafikverket.egg-info/SOURCES.txt` & `pytrafikverket-0.3.4/pytrafikverket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.3/setup.py` & `pytrafikverket-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pytrafikverket",
-    version="0.3.3",
+    version="0.3.4",
     description="Retreive values from public API at the Swedish Transport Administration (Trafikverket).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/endor-force/pytrafikverket",
     author="Peter Andersson, Jonas Karlsson",
     license="MIT",
     classifiers=[
```

