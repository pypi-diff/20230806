# Comparing `tmp/alacorder-81.1.8.tar.gz` & `tmp/alacorder-81.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-81.1.8.tar", max compression
+gzip compressed data, was "alacorder-81.1.9.tar", max compression
```

## Comparing `alacorder-81.1.8.tar` & `alacorder-81.1.9.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.8/LICENSE
--rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.8/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 02:07:06.233018 alacorder-81.1.8/alacorder/.DS_Store
--rw-r--r--   0        0        0       72 2023-08-04 20:41:53.084285 alacorder-81.1.8/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0   338687 2023-08-05 21:03:17.371559 alacorder-81.1.8/alacorder/Untitled.ipynb
--rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.8/alacorder/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.8/alacorder/__main__.py
--rw-r--r--   0        0        0   278452 2023-08-05 21:05:57.207182 alacorder-81.1.8/alacorder/alac.py
--rw-r--r--   0        0        0      557 2023-08-05 21:06:10.198178 alacorder-81.1.8/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-18 14:01:34.633926 alacorder-81.1.9/LICENSE
+-rw-r--r--   0        0        0     4865 2023-07-25 18:33:12.479611 alacorder-81.1.9/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 21:07:02.301721 alacorder-81.1.9/alacorder/.DS_Store
+-rw-r--r--   0        0        0       72 2023-08-04 20:41:53.084285 alacorder-81.1.9/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       19 2023-07-25 19:20:19.054678 alacorder-81.1.9/alacorder/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-25 19:23:49.408885 alacorder-81.1.9/alacorder/__main__.py
+-rw-r--r--   0        0        0   278452 2023-08-05 21:07:53.085512 alacorder-81.1.9/alacorder/alac.py
+-rw-r--r--   0        0        0      557 2023-08-05 21:07:58.277203 alacorder-81.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 alacorder-81.1.9/PKG-INFO
```

### Comparing `alacorder-81.1.8/LICENSE` & `alacorder-81.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.8/README.md` & `alacorder-81.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.8/alacorder/.DS_Store` & `alacorder-81.1.9/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-81.1.8/alacorder/alac.py` & `alacorder-81.1.9/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ┣┫┃ ┣┫┃ ┃┃┣┫┃┃┣ ┣┫
 ┛┗┗┛┛┗┗┛┗┛┛┗┻┛┗┛┛┗
 (c) 2023 Sam Robson
 
 Dependencies: Python 3.9+, Google Chrome, brotli 1.0.9+, polars 0.18.1+, pymupdf 1.21.1+, rich 13.3.3+, selenium 4.8.3+, typer 0.9.0+, xlsx2csv 0.8.1+, xlsxwriter 3.0.9+
 """
 
-__version__ = "81.1.8"
+__version__ = "81.1.9"
 
 import os
 import re
 import glob
 import time
 from datetime import datetime
 from pathlib import Path
```

### Comparing `alacorder-81.1.8/pyproject.toml` & `alacorder-81.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "81.1.8"
+version = "81.1.9"
 description = "Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `alacorder-81.1.8/PKG-INFO` & `alacorder-81.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 81.1.8
+Version: 81.1.9
 Summary: Alacorder retrieves case detail PDFs from Alacourt.com and processes them into data tables suitable for research purposes.
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

