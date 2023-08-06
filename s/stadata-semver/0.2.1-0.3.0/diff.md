# Comparing `tmp/stadata_semver-0.2.1.tar.gz` & `tmp/stadata_semver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadata_semver-0.2.1.tar", max compression
+gzip compressed data, was "stadata_semver-0.3.0.tar", max compression
```

## Comparing `stadata_semver-0.2.1.tar` & `stadata_semver-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1279 2023-08-06 08:25:46.242654 stadata_semver-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-08-06 08:25:05.410337 stadata_semver-0.2.1/stadata/.DS_Store
--rw-r--r--   0        0        0       24 2023-08-06 08:25:05.410337 stadata_semver-0.2.1/stadata/__init__.py
--rw-r--r--   0        0        0    26028 2023-08-06 08:25:05.410337 stadata_semver-0.2.1/stadata/main.py
--rw-r--r--   0        0        0      454 2023-08-06 08:25:05.410337 stadata_semver-0.2.1/stadata/material.py
--rw-r--r--   0        0        0       37 2023-08-06 08:25:05.410337 stadata_semver-0.2.1/stadata/semver_demo.py
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 stadata_semver-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1279 2023-08-06 08:27:37.715158 stadata_semver-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-08-06 08:26:59.362094 stadata_semver-0.3.0/stadata/.DS_Store
+-rw-r--r--   0        0        0       24 2023-08-06 08:26:59.362094 stadata_semver-0.3.0/stadata/__init__.py
+-rw-r--r--   0        0        0    26028 2023-08-06 08:26:59.366094 stadata_semver-0.3.0/stadata/main.py
+-rw-r--r--   0        0        0      454 2023-08-06 08:26:59.366094 stadata_semver-0.3.0/stadata/material.py
+-rw-r--r--   0        0        0       56 2023-08-06 08:26:59.366094 stadata_semver-0.3.0/stadata/semver_demo.py
+-rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 stadata_semver-0.3.0/PKG-INFO
```

### Comparing `stadata_semver-0.2.1/pyproject.toml` & `stadata_semver-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stadata-semver"
-version = "0.2.1"
+version = "0.3.0"
 description = "API for get all statistics data from BPS"
 authors = ["Muhammad Luqman <im.imperativa@gmail.com>"]
 urls = {homepage = "https://github.com/bps-statistics/stadata"}
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `stadata_semver-0.2.1/stadata/.DS_Store` & `stadata_semver-0.3.0/stadata/.DS_Store`

 * *Files identical despite different names*

### Comparing `stadata_semver-0.2.1/stadata/main.py` & `stadata_semver-0.3.0/stadata/main.py`

 * *Files identical despite different names*

### Comparing `stadata_semver-0.2.1/PKG-INFO` & `stadata_semver-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadata-semver
-Version: 0.2.1
+Version: 0.3.0
 Summary: API for get all statistics data from BPS
 License: MIT
 Keywords: bps dataset utility indonesia
 Author: Muhammad Luqman
 Author-email: im.imperativa@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

