# Comparing `tmp/gcshus-0.0.1.tar.gz` & `tmp/gcshus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcshus-0.0.1.tar", last modified: Sun Aug  6 02:29:14 2023, max compression
+gzip compressed data, was "gcshus-0.0.2.tar", last modified: Sun Aug  6 02:55:21 2023, max compression
```

## Comparing `gcshus-0.0.1.tar` & `gcshus-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 02:29:14.925110 gcshus-0.0.1/
--rw-r--r--   0 kreuz45    (501) staff       (20)     1062 2023-02-20 11:48:46.000000 gcshus-0.0.1/LICENSE
--rw-r--r--   0 kreuz45    (501) staff       (20)      944 2023-08-06 02:29:14.924907 gcshus-0.0.1/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)      455 2023-08-06 02:25:41.000000 gcshus-0.0.1/README.md
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 02:29:14.923492 gcshus-0.0.1/gcshus/
--rw-r--r--   0 kreuz45    (501) staff       (20)      174 2023-08-05 12:04:04.000000 gcshus-0.0.1/gcshus/__init__.py
--rw-r--r--   0 kreuz45    (501) staff       (20)     1377 2023-08-05 12:09:42.000000 gcshus-0.0.1/gcshus/signed_url.py
--rw-r--r--   0 kreuz45    (501) staff       (20)      304 2023-03-18 08:14:43.000000 gcshus-0.0.1/gcshus/upload.py
-drwxr-xr-x   0 kreuz45    (501) staff       (20)        0 2023-08-06 02:29:14.924711 gcshus-0.0.1/gcshus.egg-info/
--rw-r--r--   0 kreuz45    (501) staff       (20)      944 2023-08-06 02:29:14.000000 gcshus-0.0.1/gcshus.egg-info/PKG-INFO
--rw-r--r--   0 kreuz45    (501) staff       (20)      232 2023-08-06 02:29:14.000000 gcshus-0.0.1/gcshus.egg-info/SOURCES.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        1 2023-08-06 02:29:14.000000 gcshus-0.0.1/gcshus.egg-info/dependency_links.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)       28 2023-08-06 02:29:14.000000 gcshus-0.0.1/gcshus.egg-info/requires.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)        7 2023-08-06 02:29:14.000000 gcshus-0.0.1/gcshus.egg-info/top_level.txt
--rw-r--r--   0 kreuz45    (501) staff       (20)       38 2023-08-06 02:29:14.925141 gcshus-0.0.1/setup.cfg
--rw-r--r--   0 kreuz45    (501) staff       (20)     1162 2023-02-20 11:50:02.000000 gcshus-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:55:21.202113 gcshus-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 02:55:11.000000 gcshus-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-06 02:55:21.202113 gcshus-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-06 02:55:11.000000 gcshus-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:55:21.198113 gcshus-0.0.2/gcshus/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-06 02:55:11.000000 gcshus-0.0.2/gcshus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-06 02:55:11.000000 gcshus-0.0.2/gcshus/signed_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-06 02:55:11.000000 gcshus-0.0.2/gcshus/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:55:21.198113 gcshus-0.0.2/gcshus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-06 02:55:21.000000 gcshus-0.0.2/gcshus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-06 02:55:21.000000 gcshus-0.0.2/gcshus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:55:21.000000 gcshus-0.0.2/gcshus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 02:55:21.000000 gcshus-0.0.2/gcshus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 02:55:21.000000 gcshus-0.0.2/gcshus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 02:55:21.202113 gcshus-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-06 02:55:11.000000 gcshus-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:55:21.202113 gcshus-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-06 02:55:11.000000 gcshus-0.0.2/tests/test_signed_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 02:55:11.000000 gcshus-0.0.2/tests/test_upload.py
```

### Comparing `gcshus-0.0.1/LICENSE` & `gcshus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gcshus-0.0.1/PKG-INFO` & `gcshus-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gcshus
-Version: 0.0.1
+Version: 0.0.2
 Summary: gcshus: GCS helper utils.
 Home-page: https://github.com/yokoe/gcshus
+Download-URL: https://github.com/yokoe/gcshus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
 License: MIT
-Download-URL: https://github.com/yokoe/gcshus
 Keywords: gcs
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gcshus
 GCS Helper Utils for Python
@@ -40,9 +39,7 @@
 )
 ```
 
 ## Run test
 ```
 docker compose up
 ```
-
-
```

### Comparing `gcshus-0.0.1/gcshus/signed_url.py` & `gcshus-0.0.2/gcshus/signed_url.py`

 * *Files identical despite different names*

### Comparing `gcshus-0.0.1/gcshus.egg-info/PKG-INFO` & `gcshus-0.0.2/gcshus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gcshus
-Version: 0.0.1
+Version: 0.0.2
 Summary: gcshus: GCS helper utils.
 Home-page: https://github.com/yokoe/gcshus
+Download-URL: https://github.com/yokoe/gcshus
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
 License: MIT
-Download-URL: https://github.com/yokoe/gcshus
 Keywords: gcs
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gcshus
 GCS Helper Utils for Python
@@ -40,9 +39,7 @@
 )
 ```
 
 ## Run test
 ```
 docker compose up
 ```
-
-
```

### Comparing `gcshus-0.0.1/setup.py` & `gcshus-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "gcshus: GCS helper utils."
 NAME = "gcshus"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/gcshus"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.6"
 INSTALL_REQUIRES = open("requirements.txt").read().splitlines()
 PACKAGES = ["gcshus"]
 KEYWORDS = "gcs"
 CLASSIFIERS = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.6",
```

