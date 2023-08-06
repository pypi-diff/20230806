# Comparing `tmp/configration-2.0.5.tar.gz` & `tmp/configration-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.5.tar", last modified: Thu Jun 29 10:59:40 2023, max compression
+gzip compressed data, was "configration-2.0.6.tar", last modified: Thu Jun 29 13:37:45 2023, max compression
```

## Comparing `configration-2.0.5.tar` & `configration-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.5/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1162 2023-06-29 10:59:40.925925 configration-2.0.5/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.5/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.5/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 10:57:45.000000 configration-2.0.5/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.5/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2631 2023-06-29 10:57:45.000000 configration-2.0.5/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.5/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.5/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-18 11:40:32.000000 configration-2.0.5/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.5/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2909 2023-06-29 10:57:45.000000 configration-2.0.5/configration/tests/test_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      229 2023-06-18 11:34:14.000000 configration-2.0.5/configration/xxx.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1162 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      469 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 10:59:40.925925 configration-2.0.5/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.5/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:37:45.798720 configration-2.0.6/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.6/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1216 2023-06-29 13:37:45.798720 configration-2.0.6/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.6/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:37:45.795386 configration-2.0.6/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.6/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 13:36:13.000000 configration-2.0.6/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:37:45.798720 configration-2.0.6/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:36:13.000000 configration-2.0.6/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2631 2023-06-29 13:36:13.000000 configration-2.0.6/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      397 2023-06-29 13:36:13.000000 configration-2.0.6/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-29 13:36:13.000000 configration-2.0.6/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-29 13:36:13.000000 configration-2.0.6/configration/src/toml_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      229 2023-06-18 11:34:14.000000 configration-2.0.6/configration/src/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:37:45.798720 configration-2.0.6/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:36:13.000000 configration-2.0.6/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2909 2023-06-29 13:36:13.000000 configration-2.0.6/configration/tests/test_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1762 2023-06-29 13:36:13.000000 configration-2.0.6/configration/tests/test_json.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1712 2023-06-29 13:36:13.000000 configration-2.0.6/configration/tests/test_toml.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:37:45.795386 configration-2.0.6/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1216 2023-06-29 13:37:45.000000 configration-2.0.6/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      537 2023-06-29 13:37:45.000000 configration-2.0.6/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 13:37:45.000000 configration-2.0.6/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-29 13:37:45.000000 configration-2.0.6/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 13:37:45.798720 configration-2.0.6/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.6/setup.py
```

### Comparing `configration-2.0.5/LICENSE.txt` & `configration-2.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.5/PKG-INFO` & `configration-2.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.5
+Version: 2.0.6
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.6 29 Jun 2023
+
+1. Copt all tests
+
+------
+
 Version 2.0.5 29 Jun 2023
 
 1. Tests on json and Toml
 ------
 
 Version 2.0.4 18 June 2023
```

### Comparing `configration-2.0.5/configration/src/config.py` & `configration-2.0.6/configration/src/config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.5/configration/src/json_config.py` & `configration-2.0.6/configration/src/json_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.5/configration/src/toml_config.py` & `configration-2.0.6/configration/src/toml_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.5/configration/tests/test_config.py` & `configration-2.0.6/configration/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.5/configration.egg-info/PKG-INFO` & `configration-2.0.6/configration.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.5
+Version: 2.0.6
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.6 29 Jun 2023
+
+1. Copt all tests
+
+------
+
 Version 2.0.5 29 Jun 2023
 
 1. Tests on json and Toml
 ------
 
 Version 2.0.4 18 June 2023
```

### Comparing `configration-2.0.5/setup.py` & `configration-2.0.6/setup.py`

 * *Files identical despite different names*

