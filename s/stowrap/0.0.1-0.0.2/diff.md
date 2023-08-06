# Comparing `tmp/stowrap-0.0.1.tar.gz` & `tmp/stowrap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stowrap-0.0.1.tar", last modified: Sun Aug  6 12:49:38 2023, max compression
+gzip compressed data, was "stowrap-0.0.2.tar", last modified: Sun Aug  6 12:57:49 2023, max compression
```

## Comparing `stowrap-0.0.1.tar` & `stowrap-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 12:49:38.058904 stowrap-0.0.1/
--rw-r--r--   0 kreuz45    (501) staff       (20)     1062 2023-08-05 09:15:52.000000 stowrap-0.0.1/LICENSE
--rw-r--r--   0 kreuz45    (501) staff       (20)      551 2023-08-06 12:49:38.058594 stowrap-0.0.1/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)       41 2023-08-05 09:15:52.000000 stowrap-0.0.1/README.md
--rw-r--r--   0 kreuz45    (501) staff       (20)       38 2023-08-06 12:49:38.058943 stowrap-0.0.1/setup.cfg
--rw-r--r--   0 kreuz45    (501) staff       (20)     1224 2023-08-06 12:24:22.000000 stowrap-0.0.1/setup.py
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 12:49:38.055491 stowrap-0.0.1/src/
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 12:49:38.057745 stowrap-0.0.1/src/stowrap/
--rw-r--r--   0 kreuz45    (501) staff       (20)       27 2023-08-06 10:23:40.000000 stowrap-0.0.1/src/stowrap/__init__.py
--rw-r--r--   0 kreuz45    (501) staff       (20)     1114 2023-08-06 12:31:36.000000 stowrap-0.0.1/src/stowrap/client.py
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 12:49:38.058417 stowrap-0.0.1/src/stowrap.egg-info/
--rw-r--r--   0 kreuz45    (501) staff       (20)      551 2023-08-06 12:49:38.000000 stowrap-0.0.1/src/stowrap.egg-info/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)      246 2023-08-06 12:49:38.000000 stowrap-0.0.1/src/stowrap.egg-info/SOURCES.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        1 2023-08-06 12:49:38.000000 stowrap-0.0.1/src/stowrap.egg-info/dependency_links.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)       13 2023-08-06 12:49:38.000000 stowrap-0.0.1/src/stowrap.egg-info/requires.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        8 2023-08-06 12:49:38.000000 stowrap-0.0.1/src/stowrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 12:57:40.000000 stowrap-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 12:57:49.083281 stowrap-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-06 12:57:40.000000 stowrap-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:57:49.083281 stowrap-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-06 12:57:40.000000 stowrap-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.079281 stowrap-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.079281 stowrap-0.0.2/src/stowrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 12:57:40.000000 stowrap-0.0.2/src/stowrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-06 12:57:40.000000 stowrap-0.0.2/src/stowrap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/src/stowrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-06 12:57:40.000000 stowrap-0.0.2/tests/test_upload.py
```

### Comparing `stowrap-0.0.1/LICENSE` & `stowrap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stowrap-0.0.1/setup.py` & `stowrap-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "stowrap: Python Storage Service Wrapper."
 NAME = "stowrap"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/stowrap"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.9"
 INSTALL_REQUIRES = [
     "gcshus",
     "boto3",
 ]
 PACKAGES = ["stowrap"]
 PACKAGE_DIR = {"": "src"}
```

### Comparing `stowrap-0.0.1/src/stowrap/client.py` & `stowrap-0.0.2/src/stowrap/client.py`

 * *Files identical despite different names*

