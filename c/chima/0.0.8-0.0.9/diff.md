# Comparing `tmp/chima-0.0.8.tar.gz` & `tmp/chima-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chima-0.0.8.tar", max compression
+gzip compressed data, was "chima-0.0.9.tar", max compression
```

## Comparing `chima-0.0.8.tar` & `chima-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2253 2023-06-12 03:33:44.967216 chima-0.0.8/README.md
--rw-r--r--   0        0        0      365 2023-06-12 03:33:44.967216 chima-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      275 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/__init__.py
--rw-r--r--   0        0        0    11927 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/client.py
--rw-r--r--   0        0        0      348 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      159 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/environment.py
--rw-r--r--   0        0        0        0 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/py.typed
--rw-r--r--   0        0        0      288 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/__init__.py
--rw-r--r--   0        0        0      754 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/converse_response.py
--rw-r--r--   0        0        0      757 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/generate_text_response.py
--rw-r--r--   0        0        0      920 2023-06-12 03:33:44.971216 chima-0.0.8/src/chima/types/search_response.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-06-12 18:42:33.033012 chima-0.0.9/README.md
+-rw-r--r--   0        0        0      365 2023-06-12 18:42:33.033012 chima-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      275 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/__init__.py
+-rw-r--r--   0        0        0    11927 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/client.py
+-rw-r--r--   0        0        0      348 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      159 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/environment.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/py.typed
+-rw-r--r--   0        0        0      288 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/types/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/types/converse_response.py
+-rw-r--r--   0        0        0      757 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/types/generate_text_response.py
+-rw-r--r--   0        0        0      920 2023-06-12 18:42:33.033012 chima-0.0.9/src/chima/types/search_response.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.9/PKG-INFO
```

### Comparing `chima-0.0.8/README.md` & `chima-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/client.py` & `chima-0.0.9/src/chima/client.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/core/datetime_utils.py` & `chima-0.0.9/src/chima/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/core/jsonable_encoder.py` & `chima-0.0.9/src/chima/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/types/converse_response.py` & `chima-0.0.9/src/chima/types/converse_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/types/generate_text_response.py` & `chima-0.0.9/src/chima/types/generate_text_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/src/chima/types/search_response.py` & `chima-0.0.9/src/chima/types/search_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.8/PKG-INFO` & `chima-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chima
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

