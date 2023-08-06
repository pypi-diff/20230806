# Comparing `tmp/Swagger2Tests-1.0.8.tar.gz` & `tmp/Swagger2Tests-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Swagger2Tests-1.0.8.tar", last modified: Fri Aug  4 10:46:33 2023, max compression
+gzip compressed data, was "Swagger2Tests-1.0.9.tar", last modified: Fri Aug  4 11:39:45 2023, max compression
```

## Comparing `Swagger2Tests-1.0.8.tar` & `Swagger2Tests-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:46:33.002633 Swagger2Tests-1.0.8/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:46:33.002161 Swagger2Tests-1.0.8/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:46:32.992718 Swagger2Tests-1.0.8/Swagger2Tests/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     6618 2023-08-04 10:46:16.000000 Swagger2Tests-1.0.8/Swagger2Tests/Swagger2Tests.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-08-04 09:27:37.000000 Swagger2Tests-1.0.8/Swagger2Tests/__init__.py
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:46:33.000843 Swagger2Tests-1.0.8/Swagger2Tests/constants/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.8/Swagger2Tests/constants/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      193 2023-08-04 10:44:39.000000 Swagger2Tests-1.0.8/Swagger2Tests/constants/base_constants.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3247 2023-08-04 10:39:54.000000 Swagger2Tests-1.0.8/Swagger2Tests/loadswagger.py
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 10:46:32.999294 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      396 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       66 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       14 2023-08-04 10:46:32.000000 Swagger2Tests-1.0.8/Swagger2Tests.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 10:46:33.002840 Swagger2Tests-1.0.8/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      905 2023-08-04 10:46:28.000000 Swagger2Tests-1.0.8/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 11:39:45.137675 Swagger2Tests-1.0.9/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 11:39:45.137195 Swagger2Tests-1.0.9/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 11:39:45.130591 Swagger2Tests-1.0.9/Swagger2Tests/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     6617 2023-08-04 11:38:56.000000 Swagger2Tests-1.0.9/Swagger2Tests/Swagger2Tests.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 11:39:45.136161 Swagger2Tests-1.0.9/Swagger2Tests/constants/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-24 06:47:35.000000 Swagger2Tests-1.0.9/Swagger2Tests/constants/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      191 2023-08-04 11:39:04.000000 Swagger2Tests-1.0.9/Swagger2Tests/constants/base_constants.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3246 2023-08-04 11:38:33.000000 Swagger2Tests-1.0.9/Swagger2Tests/loadswagger.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-04 11:39:45.134703 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     1784 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      370 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       66 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       50 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-04 11:39:45.000000 Swagger2Tests-1.0.9/Swagger2Tests.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-04 11:39:45.137923 Swagger2Tests-1.0.9/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      905 2023-08-04 11:39:41.000000 Swagger2Tests-1.0.9/setup.py
```

### Comparing `Swagger2Tests-1.0.8/PKG-INFO` & `Swagger2Tests-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.8
+Version: 1.0.9
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.8/Swagger2Tests/Swagger2Tests.py` & `Swagger2Tests-1.0.9/Swagger2Tests/Swagger2Tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from jinja2 import Environment, FileSystemLoader, Template
 import json
 from enum import Enum
 from pathlib import Path
-from .constants.base_constants import *
+from constants.base_constants import *
 import requests
 
 
 class BaseEnum(Enum):
 
     @classmethod
     def get_enum_by_value(cls, value):
```

### Comparing `Swagger2Tests-1.0.8/Swagger2Tests/loadswagger.py` & `Swagger2Tests-1.0.9/Swagger2Tests/loadswagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import coloredlogs
 import logging
 from pathlib import Path
-from .Swagger2Tests import *
+from Swagger2Tests import *
 import argparse
 import os
 import shutil
 
 coloredlogs.install()
```

### Comparing `Swagger2Tests-1.0.8/Swagger2Tests.egg-info/PKG-INFO` & `Swagger2Tests-1.0.9/Swagger2Tests.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Swagger2Tests
-Version: 1.0.8
+Version: 1.0.9
 Summary: swagger
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Swagger2Tests-1.0.8/setup.py` & `Swagger2Tests-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 readmepath = 'README.md'
 setup(
     name='Swagger2Tests',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'Swagger2Tests = Swagger2Tests.loadswagger:main'
         ]
     },
     install_requires=[
```

