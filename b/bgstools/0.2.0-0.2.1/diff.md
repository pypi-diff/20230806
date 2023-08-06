# Comparing `tmp/bgstools-0.2.0.tar.gz` & `tmp/bgstools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.2.0.tar", max compression
+gzip compressed data, was "bgstools-0.2.1.tar", max compression
```

## Comparing `bgstools-0.2.0.tar` & `bgstools-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       72 2023-06-11 05:11:36.804060 bgstools-0.2.0/README.md
--rw-r--r--   0        0        0       32 2023-07-17 19:28:40.744164 bgstools-0.2.0/bgstools/__init__.py
--rw-r--r--   0        0        0      132 2023-07-29 11:29:50.466544 bgstools-0.2.0/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0    10597 2023-07-29 11:23:03.266953 bgstools-0.2.0/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0       32 2023-07-02 08:13:04.227813 bgstools-0.2.0/bgstools/experimental/__init__.py
--rw-r--r--   0        0        0      144 2023-07-02 08:10:15.065987 bgstools-0.2.0/bgstools/experimental/lambdas.py
--rw-r--r--   0        0        0      796 2023-07-29 14:11:52.668928 bgstools-0.2.0/bgstools/io/__init__.py
--rw-r--r--   0        0        0    21504 2023-08-05 09:37:05.538002 bgstools-0.2.0/bgstools/io/io.py
--rw-r--r--   0        0        0    16003 2023-08-06 11:43:46.333721 bgstools-0.2.0/bgstools/io/media.py
--rw-r--r--   0        0        0      418 2023-07-18 13:46:07.987038 bgstools-0.2.0/bgstools/requirements.txt
--rw-r--r--   0        0        0      122 2023-06-11 05:11:36.804060 bgstools-0.2.0/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-06-11 05:11:36.804060 bgstools-0.2.0/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0      119 2023-07-07 07:04:39.928611 bgstools-0.2.0/bgstools/stt/__init__.py
--rw-r--r--   0        0        0    10001 2023-08-01 08:28:42.691148 bgstools-0.2.0/bgstools/stt/stt.py
--rw-r--r--   0        0        0      229 2023-07-29 13:06:41.824761 bgstools-0.2.0/bgstools/utils/__init__.py
--rw-r--r--   0        0        0     8833 2023-07-29 13:14:54.351335 bgstools-0.2.0/bgstools/utils/utils.py
--rw-r--r--   0        0        0       20 2023-08-06 11:45:56.533962 bgstools-0.2.0/bgstools/version.py
--rw-r--r--   0        0        0      541 2023-08-06 11:46:19.683743 bgstools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 bgstools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-06-11 05:11:36.804060 bgstools-0.2.1/README.md
+-rw-r--r--   0        0        0       32 2023-07-17 19:28:40.744164 bgstools-0.2.1/bgstools/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-29 11:29:50.466544 bgstools-0.2.1/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0    10597 2023-07-29 11:23:03.266953 bgstools-0.2.1/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0       32 2023-07-02 08:13:04.227813 bgstools-0.2.1/bgstools/experimental/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-02 08:10:15.065987 bgstools-0.2.1/bgstools/experimental/lambdas.py
+-rw-r--r--   0        0        0      796 2023-07-29 14:11:52.668928 bgstools-0.2.1/bgstools/io/__init__.py
+-rw-r--r--   0        0        0    21504 2023-08-05 09:37:05.538002 bgstools-0.2.1/bgstools/io/io.py
+-rw-r--r--   0        0        0    16003 2023-08-06 11:43:46.333721 bgstools-0.2.1/bgstools/io/media.py
+-rw-r--r--   0        0        0      418 2023-07-18 13:46:07.987038 bgstools-0.2.1/bgstools/requirements.txt
+-rw-r--r--   0        0        0      122 2023-06-11 05:11:36.804060 bgstools-0.2.1/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-06-11 05:11:36.804060 bgstools-0.2.1/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0      119 2023-07-07 07:04:39.928611 bgstools-0.2.1/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0    10001 2023-08-01 08:28:42.691148 bgstools-0.2.1/bgstools/stt/stt.py
+-rw-r--r--   0        0        0      229 2023-07-29 13:06:41.824761 bgstools-0.2.1/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     8843 2023-08-06 16:53:13.746360 bgstools-0.2.1/bgstools/utils/utils.py
+-rw-r--r--   0        0        0       20 2023-08-06 16:53:30.696501 bgstools-0.2.1/bgstools/version.py
+-rw-r--r--   0        0        0      541 2023-08-06 16:54:01.646921 bgstools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 bgstools-0.2.1/PKG-INFO
```

### Comparing `bgstools-0.2.0/bgstools/datastorage/datastorage.py` & `bgstools-0.2.1/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/io/__init__.py` & `bgstools-0.2.1/bgstools/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/io/io.py` & `bgstools-0.2.1/bgstools/io/io.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/io/media.py` & `bgstools-0.2.1/bgstools/io/media.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/spatial/spatial.py` & `bgstools-0.2.1/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/stt/stt.py` & `bgstools-0.2.1/bgstools/stt/stt.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.2.0/bgstools/utils/utils.py` & `bgstools-0.2.1/bgstools/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             Defaults to None.
 
     Returns:
         The value at the nested key if it exists, otherwise the default value.
     """
     try:
         for key in keys_list:
-            data_dict = data_dict[key]
+            data_dict = data_dict.get(key, None)
         return data_dict
     except KeyError:
         return default
 
 
 
 def str_as_dtype(datatype: str, callback: callable = None):
```

### Comparing `bgstools-0.2.0/pyproject.toml` & `bgstools-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # poetry export --without-hashes --format=requirements.txt > requirements.txt && twine upload -r pypi dist/*
 [tool.poetry]
 name = "bgstools"
-version = "0.2.0"
+version = "0.2.1"
 description = "BeGeoSpatial Development Tools"
 authors = ["José Beltrán <102664984+jose-begeospatial@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 PyYAML = "^6.0"
```

### Comparing `bgstools-0.2.0/PKG-INFO` & `bgstools-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgstools
-Version: 0.2.0
+Version: 0.2.1
 Summary: BeGeoSpatial Development Tools
 Author: José Beltrán
 Author-email: 102664984+jose-begeospatial@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
```

