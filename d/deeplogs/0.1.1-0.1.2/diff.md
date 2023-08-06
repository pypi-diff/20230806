# Comparing `tmp/deeplogs-0.1.1.tar.gz` & `tmp/deeplogs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplogs-0.1.1.tar", last modified: Tue Aug  1 00:59:30 2023, max compression
+gzip compressed data, was "deeplogs-0.1.2.tar", last modified: Tue Aug  1 01:02:10 2023, max compression
```

## Comparing `deeplogs-0.1.1.tar` & `deeplogs-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 00:59:30.040023 deeplogs-0.1.1/
--rw-rw-r--   0 guy       (1000) guy       (1000)     1273 2023-08-01 00:59:30.040023 deeplogs-0.1.1/PKG-INFO
--rw-rw-r--   0 guy       (1000) guy       (1000)     8013 2023-08-01 00:22:04.000000 deeplogs-0.1.1/README.rst
-drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 00:59:30.040023 deeplogs-0.1.1/deeplogs/
--rw-rw-r--   0 guy       (1000) guy       (1000)      114 2023-08-01 00:57:17.000000 deeplogs-0.1.1/deeplogs/__init__.py
--rw-rw-r--   0 guy       (1000) guy       (1000)     1393 2023-07-27 11:59:49.000000 deeplogs-0.1.1/deeplogs/_colors.py
--rw-rw-r--   0 guy       (1000) guy       (1000)       21 2023-08-01 00:55:19.000000 deeplogs-0.1.1/deeplogs/_version.py
--rw-rw-r--   0 guy       (1000) guy       (1000)     3985 2023-07-30 22:38:57.000000 deeplogs-0.1.1/deeplogs/bar.py
--rw-rw-r--   0 guy       (1000) guy       (1000)     7157 2023-07-31 01:42:45.000000 deeplogs-0.1.1/deeplogs/logger.py
--rw-rw-r--   0 guy       (1000) guy       (1000)     6038 2023-07-30 23:18:27.000000 deeplogs-0.1.1/deeplogs/reader.py
-drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 00:59:30.040023 deeplogs-0.1.1/deeplogs.egg-info/
--rw-rw-r--   0 guy       (1000) guy       (1000)     1273 2023-08-01 00:59:30.000000 deeplogs-0.1.1/deeplogs.egg-info/PKG-INFO
--rw-rw-r--   0 guy       (1000) guy       (1000)      294 2023-08-01 00:59:30.000000 deeplogs-0.1.1/deeplogs.egg-info/SOURCES.txt
--rw-rw-r--   0 guy       (1000) guy       (1000)        1 2023-08-01 00:59:30.000000 deeplogs-0.1.1/deeplogs.egg-info/dependency_links.txt
--rw-rw-r--   0 guy       (1000) guy       (1000)       47 2023-08-01 00:59:30.000000 deeplogs-0.1.1/deeplogs.egg-info/requires.txt
--rw-rw-r--   0 guy       (1000) guy       (1000)        9 2023-08-01 00:59:30.000000 deeplogs-0.1.1/deeplogs.egg-info/top_level.txt
--rw-rw-r--   0 guy       (1000) guy       (1000)       38 2023-08-01 00:59:30.040023 deeplogs-0.1.1/setup.cfg
--rw-rw-r--   0 guy       (1000) guy       (1000)     1536 2023-08-01 00:54:19.000000 deeplogs-0.1.1/setup.py
+drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 01:02:10.115217 deeplogs-0.1.2/
+-rw-rw-r--   0 guy       (1000) guy       (1000)     1273 2023-08-01 01:02:10.115217 deeplogs-0.1.2/PKG-INFO
+-rw-rw-r--   0 guy       (1000) guy       (1000)     8013 2023-08-01 00:22:04.000000 deeplogs-0.1.2/README.rst
+drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 01:02:10.115217 deeplogs-0.1.2/deeplogs/
+-rw-rw-r--   0 guy       (1000) guy       (1000)      114 2023-08-01 00:57:17.000000 deeplogs-0.1.2/deeplogs/__init__.py
+-rw-rw-r--   0 guy       (1000) guy       (1000)     1393 2023-07-27 11:59:49.000000 deeplogs-0.1.2/deeplogs/_colors.py
+-rw-rw-r--   0 guy       (1000) guy       (1000)       21 2023-08-01 01:01:21.000000 deeplogs-0.1.2/deeplogs/_version.py
+-rw-rw-r--   0 guy       (1000) guy       (1000)     3985 2023-07-30 22:38:57.000000 deeplogs-0.1.2/deeplogs/bar.py
+-rw-rw-r--   0 guy       (1000) guy       (1000)     7157 2023-07-31 01:42:45.000000 deeplogs-0.1.2/deeplogs/logger.py
+-rw-rw-r--   0 guy       (1000) guy       (1000)     6038 2023-07-30 23:18:27.000000 deeplogs-0.1.2/deeplogs/reader.py
+drwxrwxr-x   0 guy       (1000) guy       (1000)        0 2023-08-01 01:02:10.115217 deeplogs-0.1.2/deeplogs.egg-info/
+-rw-rw-r--   0 guy       (1000) guy       (1000)     1273 2023-08-01 01:02:10.000000 deeplogs-0.1.2/deeplogs.egg-info/PKG-INFO
+-rw-rw-r--   0 guy       (1000) guy       (1000)      294 2023-08-01 01:02:10.000000 deeplogs-0.1.2/deeplogs.egg-info/SOURCES.txt
+-rw-rw-r--   0 guy       (1000) guy       (1000)        1 2023-08-01 01:02:10.000000 deeplogs-0.1.2/deeplogs.egg-info/dependency_links.txt
+-rw-rw-r--   0 guy       (1000) guy       (1000)       47 2023-08-01 01:02:10.000000 deeplogs-0.1.2/deeplogs.egg-info/requires.txt
+-rw-rw-r--   0 guy       (1000) guy       (1000)        9 2023-08-01 01:02:10.000000 deeplogs-0.1.2/deeplogs.egg-info/top_level.txt
+-rw-rw-r--   0 guy       (1000) guy       (1000)       38 2023-08-01 01:02:10.115217 deeplogs-0.1.2/setup.cfg
+-rw-rw-r--   0 guy       (1000) guy       (1000)     1509 2023-08-01 01:00:36.000000 deeplogs-0.1.2/setup.py
```

### Comparing `deeplogs-0.1.1/PKG-INFO` & `deeplogs-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplogs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simplified Python Logging and Progress Tracking
 Home-page: https://github.com/guychahine/deeplogs
 Author: Guy Chahine
 Author-email: guychahine@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deeplogs-0.1.1/README.rst` & `deeplogs-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `deeplogs-0.1.1/deeplogs/_colors.py` & `deeplogs-0.1.2/deeplogs/_colors.py`

 * *Files identical despite different names*

### Comparing `deeplogs-0.1.1/deeplogs/bar.py` & `deeplogs-0.1.2/deeplogs/bar.py`

 * *Files identical despite different names*

### Comparing `deeplogs-0.1.1/deeplogs/logger.py` & `deeplogs-0.1.2/deeplogs/logger.py`

 * *Files identical despite different names*

### Comparing `deeplogs-0.1.1/deeplogs/reader.py` & `deeplogs-0.1.2/deeplogs/reader.py`

 * *Files identical despite different names*

### Comparing `deeplogs-0.1.1/deeplogs.egg-info/PKG-INFO` & `deeplogs-0.1.2/deeplogs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplogs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simplified Python Logging and Progress Tracking
 Home-page: https://github.com/guychahine/deeplogs
 Author: Guy Chahine
 Author-email: guychahine@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `deeplogs-0.1.1/setup.py` & `deeplogs-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "matplotlib==3.7.2",
     "pandas==2.0.3",
     "plotly==5.15.0",
 ]
 
 setup(
     name="deeplogs",
-    version=open("./deeplogs/VERSION", "r").read(),
+    version=__version__,
     url="https://github.com/guychahine/deeplogs",
     description="Simplified Python Logging and Progress Tracking",
     author="Guy Chahine",
     author_email="guychahine@gmail.com",
     packages=["deeplogs"],
     install_requires=install_requires,
     license="BSD",
```

