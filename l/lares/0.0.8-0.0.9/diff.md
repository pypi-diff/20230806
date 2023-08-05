# Comparing `tmp/lares-0.0.8.tar.gz` & `tmp/lares-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lares-0.0.8.tar", last modified: Thu Aug  3 06:05:47 2023, max compression
+gzip compressed data, was "lares-0.0.9.tar", last modified: Thu Aug  3 06:07:16 2023, max compression
```

## Comparing `lares-0.0.8.tar` & `lares-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:05:47.164340 lares-0.0.8/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.8/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.8/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:05:47.164340 lares-0.0.8/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.8/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:05:47.164340 lares-0.0.8/lares/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:52:38.000000 lares-0.0.8/lares/__init__.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1700 2023-08-03 06:05:01.000000 lares-0.0.8/lares/evaluate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     3066 2023-08-03 06:05:11.000000 lares-0.0.8/lares/generate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2017 2023-08-03 06:04:38.000000 lares-0.0.8/lares/validate.py
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:05:47.164340 lares-0.0.8/lares.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:05:47.000000 lares-0.0.8/lares.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 06:05:47.000000 lares-0.0.8/lares.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 06:05:47.000000 lares-0.0.8/lares.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 06:05:47.000000 lares-0.0.8/lares.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 06:05:47.000000 lares-0.0.8/lares.egg-info/top_level.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 06:05:47.164340 lares-0.0.8/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 06:05:44.000000 lares-0.0.8/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:07:16.492343 lares-0.0.9/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.9/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.9/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:07:16.492343 lares-0.0.9/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.9/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:07:16.492343 lares-0.0.9/lares/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       72 2023-08-03 06:07:07.000000 lares-0.0.9/lares/__init__.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1700 2023-08-03 06:05:01.000000 lares-0.0.9/lares/evaluate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     3066 2023-08-03 06:05:11.000000 lares-0.0.9/lares/generate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2017 2023-08-03 06:04:38.000000 lares-0.0.9/lares/validate.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:07:16.492343 lares-0.0.9/lares.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:07:16.000000 lares-0.0.9/lares.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 06:07:16.000000 lares-0.0.9/lares.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 06:07:16.000000 lares-0.0.9/lares.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 06:07:16.000000 lares-0.0.9/lares.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 06:07:16.000000 lares-0.0.9/lares.egg-info/top_level.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 06:07:16.492343 lares-0.0.9/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 06:07:14.000000 lares-0.0.9/setup.py
```

### Comparing `lares-0.0.8/LICENSE` & `lares-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lares-0.0.8/PKG-INFO` & `lares-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.8
+Version: 0.0.9
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.8/lares/evaluate.py` & `lares-0.0.9/lares/evaluate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.8/lares/generate.py` & `lares-0.0.9/lares/generate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.8/lares/validate.py` & `lares-0.0.9/lares/validate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.8/lares.egg-info/PKG-INFO` & `lares-0.0.9/lares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.8
+Version: 0.0.9
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.8/setup.py` & `lares-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lares",
-    version="0.0.8",
+    version="0.0.9",
     author="Karime Maamari",
     author_email="maamari@usc.edu",
     description="LARES: vaLidation, evAluation and REliability Solutions",
     license="MIT",
     keywords="evaluation, validation",
     url="http://packages.python.org/lares",
     packages=setuptools.find_packages(),
```

