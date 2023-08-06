# Comparing `tmp/seagoat-0.9.2.tar.gz` & `tmp/seagoat-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.9.2.tar", max compression
+gzip compressed data, was "seagoat-0.9.3.tar", max compression
```

## Comparing `seagoat-0.9.2.tar` & `seagoat-0.9.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-08-04 13:19:17.527065 seagoat-0.9.2/LICENSE
--rw-r--r--   0        0        0     1877 2023-08-04 13:19:17.527065 seagoat-0.9.2/README.md
--rw-r--r--   0        0        0     3120 2023-08-04 13:19:18.639093 seagoat-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-08-04 13:19:18.639093 seagoat-0.9.2/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/cache.py
--rw-r--r--   0        0        0     3209 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/engine.py
--rw-r--r--   0        0        0     3482 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/server.py
--rw-r--r--   0        0        0     1678 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 seagoat-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 18:30:58.654841 seagoat-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1877 2023-08-06 18:30:58.654841 seagoat-0.9.3/README.md
+-rw-r--r--   0        0        0     3120 2023-08-06 18:30:59.802918 seagoat-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-06 18:30:59.806918 seagoat-0.9.3/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/cache.py
+-rw-r--r--   0        0        0     3209 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/engine.py
+-rw-r--r--   0        0        0     3482 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/server.py
+-rw-r--r--   0        0        0     1678 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-08-06 18:30:58.670842 seagoat-0.9.3/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 seagoat-0.9.3/PKG-INFO
```

### Comparing `seagoat-0.9.2/LICENSE` & `seagoat-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/README.md` & `seagoat-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/pyproject.toml` & `seagoat-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.9.2"
+version = "0.9.3"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
```

### Comparing `seagoat-0.9.2/seagoat/cache.py` & `seagoat-0.9.3/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/cli.py` & `seagoat-0.9.3/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/engine.py` & `seagoat-0.9.3/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/file.py` & `seagoat-0.9.3/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/repository.py` & `seagoat-0.9.3/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/result.py` & `seagoat-0.9.3/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/server.py` & `seagoat-0.9.3/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/sources/chroma.py` & `seagoat-0.9.3/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/seagoat/sources/ripgrep.py` & `seagoat-0.9.3/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.2/PKG-INFO` & `seagoat-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.9.2
+Version: 0.9.3
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

