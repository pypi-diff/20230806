# Comparing `tmp/rgpvApi-1.0.0.tar.gz` & `tmp/rgpvApi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgpvApi-1.0.0.tar", last modified: Mon Jul 31 14:15:00 2023, max compression
+gzip compressed data, was "rgpvApi-1.0.1.tar", last modified: Sun Aug  6 10:17:27 2023, max compression
```

## Comparing `rgpvApi-1.0.0.tar` & `rgpvApi-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-07-31 14:15:00.814052 rgpvApi-1.0.0/
--rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 rgpvApi-1.0.0/LICENSE.txt
--rw-r--r--   0 cro        (501) staff       (20)      957 2023-07-31 14:15:00.813937 rgpvApi-1.0.0/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      402 2023-07-31 13:39:31.000000 rgpvApi-1.0.0/README.md
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-07-31 14:15:00.812984 rgpvApi-1.0.0/rgpvApi/
--rw-r--r--   0 cro        (501) staff       (20)        0 2023-07-26 07:48:08.000000 rgpvApi-1.0.0/rgpvApi/__init__.py
--rw-r--r--   0 cro        (501) staff       (20)    21615 2023-07-31 12:43:39.000000 rgpvApi-1.0.0/rgpvApi/info_api.py
--rw-r--r--   0 cro        (501) staff       (20)    14892 2023-07-31 13:36:59.000000 rgpvApi-1.0.0/rgpvApi/result_api.py
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-07-31 14:15:00.813779 rgpvApi-1.0.0/rgpvApi.egg-info/
--rw-r--r--   0 cro        (501) staff       (20)      957 2023-07-31 14:15:00.000000 rgpvApi-1.0.0/rgpvApi.egg-info/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      246 2023-07-31 14:15:00.000000 rgpvApi-1.0.0/rgpvApi.egg-info/SOURCES.txt
--rw-r--r--   0 cro        (501) staff       (20)        1 2023-07-31 14:15:00.000000 rgpvApi-1.0.0/rgpvApi.egg-info/dependency_links.txt
--rw-r--r--   0 cro        (501) staff       (20)       49 2023-07-31 14:15:00.000000 rgpvApi-1.0.0/rgpvApi.egg-info/requires.txt
--rw-r--r--   0 cro        (501) staff       (20)        8 2023-07-31 14:15:00.000000 rgpvApi-1.0.0/rgpvApi.egg-info/top_level.txt
--rw-r--r--   0 cro        (501) staff       (20)       38 2023-07-31 14:15:00.814092 rgpvApi-1.0.0/setup.cfg
--rw-r--r--   0 cro        (501) staff       (20)      883 2023-07-31 14:11:00.000000 rgpvApi-1.0.0/setup.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.176677 rgpvApi-1.0.1/
+-rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 rgpvApi-1.0.1/LICENSE.txt
+-rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-06 10:17:27.176565 rgpvApi-1.0.1/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      412 2023-08-06 10:12:57.000000 rgpvApi-1.0.1/README.md
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.175551 rgpvApi-1.0.1/rgpvApi/
+-rw-r--r--   0 cro        (501) staff       (20)       57 2023-08-06 10:08:49.000000 rgpvApi-1.0.1/rgpvApi/__init__.py
+-rw-r--r--   0 cro        (501) staff       (20)    21615 2023-07-31 12:43:39.000000 rgpvApi-1.0.1/rgpvApi/info_api.py
+-rw-r--r--   0 cro        (501) staff       (20)    14892 2023-07-31 13:36:59.000000 rgpvApi-1.0.1/rgpvApi/result_api.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2023-08-06 10:17:27.176388 rgpvApi-1.0.1/rgpvApi.egg-info/
+-rw-r--r--   0 cro        (501) staff       (20)      967 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      246 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/SOURCES.txt
+-rw-r--r--   0 cro        (501) staff       (20)        1 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/dependency_links.txt
+-rw-r--r--   0 cro        (501) staff       (20)       49 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/requires.txt
+-rw-r--r--   0 cro        (501) staff       (20)        8 2023-08-06 10:17:27.000000 rgpvApi-1.0.1/rgpvApi.egg-info/top_level.txt
+-rw-r--r--   0 cro        (501) staff       (20)       38 2023-08-06 10:17:27.176710 rgpvApi-1.0.1/setup.cfg
+-rw-r--r--   0 cro        (501) staff       (20)      883 2023-08-06 10:16:44.000000 rgpvApi-1.0.1/setup.py
```

### Comparing `rgpvApi-1.0.0/LICENSE.txt` & `rgpvApi-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rgpvApi-1.0.0/PKG-INFO` & `rgpvApi-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgpvApi
-Version: 1.0.0
+Version: 1.0.1
 Summary: RGPV API wrapper, written in Python.
 Home-page: https://github.com/cro2003/rgpvApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/rgpvApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,22 +23,22 @@
 ```bash
 pip install rgpvApi
 ```
 
 ## Usage
 Example code to get Main Result:
 ```python
-from rgpvApi import result
+import rgpvApi
 
 enrollId = ENROLLMENT_NUMBER
 courseId = COURSE_ID
 sem = SEMESTER
 
-Res = result(enrollId, courseId)
+stu_result = rgpvApi.result(enrollId, courseId)
 
-print(Res.getMain(sem))
+print(stu_result.getMain(sem))
 ```
 
 ## Contact 
 Chirag
 <br>[cro@chirag.software](mailto:cro@chirag.software)
```

### Comparing `rgpvApi-1.0.0/rgpvApi/info_api.py` & `rgpvApi-1.0.1/rgpvApi/info_api.py`

 * *Files identical despite different names*

### Comparing `rgpvApi-1.0.0/rgpvApi/result_api.py` & `rgpvApi-1.0.1/rgpvApi/result_api.py`

 * *Files identical despite different names*

### Comparing `rgpvApi-1.0.0/rgpvApi.egg-info/PKG-INFO` & `rgpvApi-1.0.1/rgpvApi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgpvApi
-Version: 1.0.0
+Version: 1.0.1
 Summary: RGPV API wrapper, written in Python.
 Home-page: https://github.com/cro2003/rgpvApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documnetation, https://cro2003.github.io/rgpvApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,22 +23,22 @@
 ```bash
 pip install rgpvApi
 ```
 
 ## Usage
 Example code to get Main Result:
 ```python
-from rgpvApi import result
+import rgpvApi
 
 enrollId = ENROLLMENT_NUMBER
 courseId = COURSE_ID
 sem = SEMESTER
 
-Res = result(enrollId, courseId)
+stu_result = rgpvApi.result(enrollId, courseId)
 
-print(Res.getMain(sem))
+print(stu_result.getMain(sem))
 ```
 
 ## Contact 
 Chirag
 <br>[cro@chirag.software](mailto:cro@chirag.software)
```

### Comparing `rgpvApi-1.0.0/setup.py` & `rgpvApi-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="rgpvApi",
-    version="1.0.0",
+    version="1.0.1",
     description="RGPV API wrapper, written in Python.",
     packages=['rgpvApi'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cro2003/rgpvApi",
     project_urls = {
     'Documnetation': 'https://cro2003.github.io/rgpvApi/',
```

