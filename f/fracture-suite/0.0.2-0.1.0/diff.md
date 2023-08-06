# Comparing `tmp/fracture-suite-0.0.2.tar.gz` & `tmp/fracture-suite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fracture-suite-0.0.2.tar", last modified: Sun Aug  6 20:15:22 2023, max compression
+gzip compressed data, was "fracture-suite-0.1.0.tar", last modified: Sun Aug  6 21:21:14 2023, max compression
```

## Comparing `fracture-suite-0.0.2.tar` & `fracture-suite-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:15:22.136391 fracture-suite-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-06 20:15:22.136391 fracture-suite-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:15:22.132391 fracture-suite-0.0.2/fracture_suite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/fracture_suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/fracture_suite/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/fracture_suite/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/fracture_suite/splinter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:15:22.136391 fracture-suite-0.0.2/fracture_suite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-06 20:15:22.000000 fracture-suite-0.0.2/fracture_suite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-06 20:15:22.000000 fracture-suite-0.0.2/fracture_suite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:15:22.000000 fracture-suite-0.0.2/fracture_suite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 20:15:22.000000 fracture-suite-0.0.2/fracture_suite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 20:15:22.000000 fracture-suite-0.0.2/fracture_suite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-06 20:15:10.000000 fracture-suite-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:15:22.136391 fracture-suite-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:21:14.138588 fracture-suite-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-06 21:21:14.138588 fracture-suite-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-06 21:21:04.000000 fracture-suite-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:21:14.138588 fracture-suite-0.1.0/fracture_suite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:21:04.000000 fracture-suite-0.1.0/fracture_suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-08-06 21:21:04.000000 fracture-suite-0.1.0/fracture_suite/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-08-06 21:21:04.000000 fracture-suite-0.1.0/fracture_suite/splinter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:21:14.138588 fracture-suite-0.1.0/fracture_suite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-06 21:21:14.000000 fracture-suite-0.1.0/fracture_suite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 21:21:14.000000 fracture-suite-0.1.0/fracture_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:21:14.000000 fracture-suite-0.1.0/fracture_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 21:21:14.000000 fracture-suite-0.1.0/fracture_suite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 21:21:14.000000 fracture-suite-0.1.0/fracture_suite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-06 21:21:04.000000 fracture-suite-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:21:14.138588 fracture-suite-0.1.0/setup.cfg
```

### Comparing `fracture-suite-0.0.2/PKG-INFO` & `fracture-suite-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fracture-suite
-Version: 0.0.2
+Version: 0.1.0
 Summary: Package to help analyze fracture patterns on broken glass plys.
 Author-email: Leon Bohmann <mail@leonbohmann.de>
 Project-URL: Homepage, https://github.com/leonbohmann/fracture-suite
 Project-URL: Bug Tracker, https://github.com/leonbohmann/fracture-suite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fracture-suite-0.0.2/fracture_suite/splinter.py` & `fracture-suite-0.1.0/fracture_suite/splinter.py`

 * *Files identical despite different names*

### Comparing `fracture-suite-0.0.2/fracture_suite.egg-info/PKG-INFO` & `fracture-suite-0.1.0/fracture_suite.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fracture-suite
-Version: 0.0.2
+Version: 0.1.0
 Summary: Package to help analyze fracture patterns on broken glass plys.
 Author-email: Leon Bohmann <mail@leonbohmann.de>
 Project-URL: Homepage, https://github.com/leonbohmann/fracture-suite
 Project-URL: Bug Tracker, https://github.com/leonbohmann/fracture-suite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fracture-suite-0.0.2/pyproject.toml` & `fracture-suite-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["matplotlib", "opencv-python", "numpy", "tqdm", "scikit-image"]
 name = "fracture-suite"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Leon Bohmann", email="mail@leonbohmann.de" },
 ]
 description = "Package to help analyze fracture patterns on broken glass plys."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

