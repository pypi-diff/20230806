# Comparing `tmp/elevenlabs-0.2.8.tar.gz` & `tmp/elevenlabs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.8.tar", last modified: Mon May  1 15:14:18 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.9.tar", last modified: Wed May  3 09:57:45 2023, max compression
```

## Comparing `elevenlabs-0.2.8.tar` & `elevenlabs-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.886002 elevenlabs-0.2.8/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:18.886002 elevenlabs-0.2.8/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 15:14:18.000000 elevenlabs-0.2.8/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:14:18.890002 elevenlabs-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 15:14:04.000000 elevenlabs-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:57:45.533472 elevenlabs-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 09:57:45.533472 elevenlabs-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:57:45.529472 elevenlabs-0.2.9/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:57:45.533472 elevenlabs-0.2.9/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:57:45.529472 elevenlabs-0.2.9/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 09:57:45.000000 elevenlabs-0.2.9/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-03 09:57:45.000000 elevenlabs-0.2.9/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:57:45.000000 elevenlabs-0.2.9/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 09:57:45.000000 elevenlabs-0.2.9/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 09:57:45.000000 elevenlabs-0.2.9/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:57:45.533472 elevenlabs-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-03 09:57:34.000000 elevenlabs-0.2.9/setup.py
```

### Comparing `elevenlabs-0.2.8/PKG-INFO` & `elevenlabs-0.2.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.8
+Version: 0.2.9
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.8/README.md` & `elevenlabs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/base.py` & `elevenlabs-0.2.9/elevenlabs/api/base.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/error.py` & `elevenlabs-0.2.9/elevenlabs/api/error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/history.py` & `elevenlabs-0.2.9/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/model.py` & `elevenlabs-0.2.9/elevenlabs/api/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/tts.py` & `elevenlabs-0.2.9/elevenlabs/api/tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/api/voice.py` & `elevenlabs-0.2.9/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/simple.py` & `elevenlabs-0.2.9/elevenlabs/simple.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs/utils.py` & `elevenlabs-0.2.9/elevenlabs/utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.8/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.9/elevenlabs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.8
+Version: 0.2.9
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.8/setup.py` & `elevenlabs-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.8",
+    version="0.2.9",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
     install_requires=[
         "pydantic>=1.10",
```

