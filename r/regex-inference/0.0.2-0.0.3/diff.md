# Comparing `tmp/regex-inference-0.0.2.tar.gz` & `tmp/regex-inference-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-inference-0.0.2.tar", last modified: Sun Aug  6 01:12:02 2023, max compression
+gzip compressed data, was "regex-inference-0.0.3.tar", last modified: Sun Aug  6 01:15:02 2023, max compression
```

## Comparing `regex-inference-0.0.2.tar` & `regex-inference-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 01:11:42.000000 regex-inference-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:12:02.180233 regex-inference-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 01:11:42.000000 regex-inference-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/cmd/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/inference/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/inference/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/inference/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/schema/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/inference/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference/schema/objs/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/objs/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/objs/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/schema/objs/records.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 01:11:42.000000 regex-inference-0.0.2/regex_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:12:02.180233 regex-inference-0.0.2/regex_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 01:12:02.000000 regex-inference-0.0.2/regex_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 01:12:02.180233 regex-inference-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-06 01:11:42.000000 regex-inference-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 01:14:43.000000 regex-inference-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:15:02.462707 regex-inference-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 01:14:43.000000 regex-inference-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/cmd/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/objs/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 01:15:02.462707 regex-inference-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-06 01:14:44.000000 regex-inference-0.0.3/setup.py
```

### Comparing `regex-inference-0.0.2/LICENSE` & `regex-inference-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/PKG-INFO` & `regex-inference-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.2
+Version: 0.0.3
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.2/regex_inference/cmd/inference.py` & `regex-inference-0.0.3/regex_inference/cmd/inference.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/config.py` & `regex-inference-0.0.3/regex_inference/config.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/inference/api.py` & `regex-inference-0.0.3/regex_inference/inference/api.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/inference/jsonl.py` & `regex-inference-0.0.3/regex_inference/inference/jsonl.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/inference/remote.py` & `regex-inference-0.0.3/regex_inference/inference/remote.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/schema/fitter.py` & `regex-inference-0.0.3/regex_inference/schema/fitter.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/schema/inference/base.py` & `regex-inference-0.0.3/regex_inference/schema/inference/base.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/schema/objs/array.py` & `regex-inference-0.0.3/regex_inference/schema/objs/array.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/schema/objs/basic.py` & `regex-inference-0.0.3/regex_inference/schema/objs/basic.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference/schema/objs/records.py` & `regex-inference-0.0.3/regex_inference/schema/objs/records.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/regex_inference.egg-info/PKG-INFO` & `regex-inference-0.0.3/regex_inference.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.2
+Version: 0.0.3
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.2/regex_inference.egg-info/SOURCES.txt` & `regex-inference-0.0.3/regex_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.2/setup.py` & `regex-inference-0.0.3/setup.py`

 * *Files identical despite different names*

