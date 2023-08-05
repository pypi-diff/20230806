# Comparing `tmp/gmpg-0.1.8.tar.gz` & `tmp/gmpg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmpg-0.1.8.tar", max compression
+gzip compressed data, was "gmpg-0.1.9.tar", max compression
```

## Comparing `gmpg-0.1.8.tar` & `gmpg-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      407 2023-01-27 00:43:43.216118 gmpg-0.1.8/gmpg/__init__.py
--rw-r--r--   0        0        0    10896 2023-01-27 00:43:43.216118 gmpg-0.1.8/gmpg/__main__.py
--rw-r--r--   0        0        0        0 2023-01-27 00:43:43.208118 gmpg-0.1.8/gmpg/_pkg/__init__.py
--rw-r--r--   0        0        0     2356 2023-01-27 00:43:43.204118 gmpg-0.1.8/gmpg/_pkg/install.py
--rw-r--r--   0        0        0     4554 2023-01-27 00:43:43.204118 gmpg-0.1.8/gmpg/_pkg/licensing/__init__.py
--rw-r--r--   0        0        0     1876 2023-01-27 00:43:43.204118 gmpg-0.1.8/gmpg/_pkg/licensing/licenses.json
--rw-r--r--   0        0        0     5185 2023-01-27 00:43:43.208118 gmpg-0.1.8/gmpg/_pkg/listing.py
--rwxr-xr-x   0        0        0       80 2023-01-27 00:43:43.208118 gmpg-0.1.8/gmpg/_pkg/runinenv
--rw-r--r--   0        0        0      497 2023-01-27 00:43:43.212118 gmpg-0.1.8/gmpg/_pkg/system.py
--rw-r--r--   0        0        0    12067 2023-05-18 22:43:58.957203 gmpg-0.1.8/gmpg/analysis.py
--rw-r--r--   0        0        0    12058 2023-07-30 01:48:26.118378 gmpg-0.1.8/gmpg/git.py
--rw-r--r--   0        0        0     6329 2023-01-27 00:43:43.216118 gmpg-0.1.8/gmpg/ide.py
--rw-r--r--   0        0        0     7161 2023-05-18 23:42:42.179473 gmpg-0.1.8/gmpg/pkg.py
--rw-r--r--   0        0        0     1011 2023-07-30 01:52:24.342155 gmpg-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 gmpg-0.1.8/setup.py
--rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 gmpg-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      407 2023-01-27 00:43:43.216118 gmpg-0.1.9/gmpg/__init__.py
+-rw-r--r--   0        0        0    10896 2023-01-27 00:43:43.216118 gmpg-0.1.9/gmpg/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-27 00:43:43.208118 gmpg-0.1.9/gmpg/_pkg/__init__.py
+-rw-r--r--   0        0        0     2356 2023-01-27 00:43:43.204118 gmpg-0.1.9/gmpg/_pkg/install.py
+-rw-r--r--   0        0        0     4554 2023-01-27 00:43:43.204118 gmpg-0.1.9/gmpg/_pkg/licensing/__init__.py
+-rw-r--r--   0        0        0     1876 2023-01-27 00:43:43.204118 gmpg-0.1.9/gmpg/_pkg/licensing/licenses.json
+-rw-r--r--   0        0        0     5185 2023-01-27 00:43:43.208118 gmpg-0.1.9/gmpg/_pkg/listing.py
+-rwxr-xr-x   0        0        0       80 2023-01-27 00:43:43.208118 gmpg-0.1.9/gmpg/_pkg/runinenv
+-rw-r--r--   0        0        0      497 2023-01-27 00:43:43.212118 gmpg-0.1.9/gmpg/_pkg/system.py
+-rw-r--r--   0        0        0    12067 2023-05-18 22:43:58.957203 gmpg-0.1.9/gmpg/analysis.py
+-rw-r--r--   0        0        0    12058 2023-07-30 01:48:26.118378 gmpg-0.1.9/gmpg/git.py
+-rw-r--r--   0        0        0     6329 2023-01-27 00:43:43.216118 gmpg-0.1.9/gmpg/ide.py
+-rw-r--r--   0        0        0     7161 2023-05-18 23:42:42.179473 gmpg-0.1.9/gmpg/pkg.py
+-rw-r--r--   0        0        0     1011 2023-07-30 01:53:12.746919 gmpg-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 gmpg-0.1.9/setup.py
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 gmpg-0.1.9/PKG-INFO
```

### Comparing `gmpg-0.1.8/gmpg/__main__.py` & `gmpg-0.1.9/gmpg/__main__.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/_pkg/install.py` & `gmpg-0.1.9/gmpg/_pkg/install.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/_pkg/licensing/__init__.py` & `gmpg-0.1.9/gmpg/_pkg/licensing/__init__.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/_pkg/licensing/licenses.json` & `gmpg-0.1.9/gmpg/_pkg/licensing/licenses.json`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/_pkg/listing.py` & `gmpg-0.1.9/gmpg/_pkg/listing.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/analysis.py` & `gmpg-0.1.9/gmpg/analysis.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/git.py` & `gmpg-0.1.9/gmpg/git.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/ide.py` & `gmpg-0.1.9/gmpg/ide.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/gmpg/pkg.py` & `gmpg-0.1.9/gmpg/pkg.py`

 * *Files identical despite different names*

### Comparing `gmpg-0.1.8/pyproject.toml` & `gmpg-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmpg"
-version = "0.1.8"
+version = "0.1.9"
 description = "tools for metamodern software development"
 keywords = ["Git", "Poetry"]
 homepage = "https://ragt.ag/code/projects/gmpg"
 repository = "https://ragt.ag/code/projects/gmpg.git"
 documentation = "https://ragt.ag/code/projects/gmpg/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `gmpg-0.1.8/setup.py` & `gmpg-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'txtint>=0.0.0']
 
 entry_points = \
 {'console_scripts': ['gmpg = gmpg.__main__:main']}
 
 setup_kwargs = {
     'name': 'gmpg',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'tools for metamodern software development',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/gmpg',
```

### Comparing `gmpg-0.1.8/PKG-INFO` & `gmpg-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmpg
-Version: 0.1.8
+Version: 0.1.9
 Summary: tools for metamodern software development
 Home-page: https://ragt.ag/code/projects/gmpg
 License: BSD-2-Clause
 Keywords: Git,Poetry
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.8,<3.11
```

