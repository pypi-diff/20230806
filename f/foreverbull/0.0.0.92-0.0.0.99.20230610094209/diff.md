# Comparing `tmp/foreverbull-0.0.0.92.tar.gz` & `tmp/foreverbull-0.0.0.99.20230610094209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foreverbull-0.0.0.92.tar", max compression
+gzip compressed data, was "foreverbull-0.0.0.99.20230610094209.tar", max compression
```

## Comparing `foreverbull-0.0.0.92.tar` & `foreverbull-0.0.0.99.20230610094209.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2023-04-16 16:04:59.423524 foreverbull-0.0.0.92/LICENSE
--rw-r--r--   0        0        0     1475 2023-06-10 08:13:14.682889 foreverbull-0.0.0.92/pyproject.toml
--rw-r--r--   0        0        0      205 2023-06-10 07:37:57.196448 foreverbull-0.0.0.92/src/foreverbull/__init__.py
--rw-r--r--   0        0        0     7271 2023-06-08 19:45:32.542228 foreverbull-0.0.0.92/src/foreverbull/__main__.py
--rw-r--r--   0        0        0      140 2023-04-16 16:04:59.437807 foreverbull-0.0.0.92/src/foreverbull/data/__init__.py
--rw-r--r--   0        0        0     2332 2023-06-08 19:45:32.565868 foreverbull-0.0.0.92/src/foreverbull/data/data.py
--rw-r--r--   0        0        0     1344 2023-04-16 16:04:59.439186 foreverbull-0.0.0.92/src/foreverbull/data/stock_data.py
--rw-r--r--   0        0        0     3811 2023-05-13 12:14:40.064905 foreverbull-0.0.0.92/src/foreverbull/foreverbull.py
--rw-r--r--   0        0        0     1298 2023-06-08 19:45:32.535440 foreverbull-0.0.0.92/src/foreverbull/models.py
--rw-r--r--   0        0        0       71 2023-04-16 16:04:59.441329 foreverbull-0.0.0.92/src/foreverbull/worker/__init__.py
--rw-r--r--   0        0        0       43 2023-04-16 16:04:59.442340 foreverbull-0.0.0.92/src/foreverbull/worker/exceptions.py
--rw-r--r--   0        0        0     8787 2023-06-08 19:45:32.551672 foreverbull-0.0.0.92/src/foreverbull/worker/worker.py
--rw-r--r--   0        0        0       79 2023-04-16 16:04:59.456109 foreverbull-0.0.0.92/src/foreverbull_core/__init__.py
--rw-r--r--   0        0        0      641 2023-05-18 11:20:15.252868 foreverbull-0.0.0.92/src/foreverbull_core/broker.py
--rw-r--r--   0        0        0      104 2023-04-16 16:04:59.457071 foreverbull-0.0.0.92/src/foreverbull_core/http/__init__.py
--rw-r--r--   0        0        0     1405 2023-06-08 19:45:32.620309 foreverbull-0.0.0.92/src/foreverbull_core/http/backtest.py
--rw-r--r--   0        0        0       92 2023-04-16 16:04:59.458259 foreverbull-0.0.0.92/src/foreverbull_core/http/exceptions.py
--rw-r--r--   0        0        0     2205 2023-04-26 09:27:45.941293 foreverbull-0.0.0.92/src/foreverbull_core/http/finance.py
--rw-r--r--   0        0        0      510 2023-04-26 09:27:45.941523 foreverbull-0.0.0.92/src/foreverbull_core/http/http.py
--rw-r--r--   0        0        0     2779 2023-06-08 19:45:32.609229 foreverbull-0.0.0.92/src/foreverbull_core/http/service.py
--rw-r--r--   0        0        0     1103 2023-04-26 09:27:45.941972 foreverbull-0.0.0.92/src/foreverbull_core/http/strategy.py
--rw-r--r--   0        0        0      742 2023-04-16 16:04:59.460828 foreverbull-0.0.0.92/src/foreverbull_core/logger.py
--rw-r--r--   0        0        0        0 2023-04-16 16:04:59.460908 foreverbull-0.0.0.92/src/foreverbull_core/models/__init__.py
--rw-r--r--   0        0        0     4823 2023-06-08 19:45:32.596054 foreverbull-0.0.0.92/src/foreverbull_core/models/backtest.py
--rw-r--r--   0        0        0     1180 2023-04-16 16:04:59.462971 foreverbull-0.0.0.92/src/foreverbull_core/models/base.py
--rw-r--r--   0        0        0     1214 2023-04-16 16:04:59.463786 foreverbull-0.0.0.92/src/foreverbull_core/models/finance.py
--rw-r--r--   0        0        0     1529 2023-06-08 19:45:32.586672 foreverbull-0.0.0.92/src/foreverbull_core/models/service.py
--rw-r--r--   0        0        0     1952 2023-06-09 12:55:50.591033 foreverbull-0.0.0.92/src/foreverbull_core/models/socket.py
--rw-r--r--   0        0        0     1000 2023-04-16 16:04:59.466308 foreverbull-0.0.0.92/src/foreverbull_core/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-16 16:04:59.466389 foreverbull-0.0.0.92/src/foreverbull_core/socket/__init__.py
--rw-r--r--   0        0        0     2916 2023-04-16 16:04:59.467501 foreverbull-0.0.0.92/src/foreverbull_core/socket/client.py
--rw-r--r--   0        0        0       83 2023-04-16 16:04:59.468288 foreverbull-0.0.0.92/src/foreverbull_core/socket/exceptions.py
--rw-r--r--   0        0        0     4194 2023-06-08 19:45:32.625693 foreverbull-0.0.0.92/src/foreverbull_core/socket/nanomsg.py
--rw-r--r--   0        0        0     2192 2023-06-08 19:45:32.636301 foreverbull-0.0.0.92/src/foreverbull_core/socket/router.py
--rw-r--r--   0        0        0        0 2023-06-03 10:49:47.186831 foreverbull-0.0.0.92/src/foreverbull_core/storage/__init__.py
--rw-r--r--   0        0        0      579 2023-06-03 10:49:47.188162 foreverbull-0.0.0.92/src/foreverbull_core/storage/backtest.py
--rw-r--r--   0        0        0      371 2023-06-03 10:49:47.188571 foreverbull-0.0.0.92/src/foreverbull_core/storage/storage.py
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 foreverbull-0.0.0.92/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 16:04:59.423524 foreverbull-0.0.0.99.20230610094209/LICENSE
+-rw-r--r--   0        0        0     1510 2023-06-10 09:46:21.990797 foreverbull-0.0.0.99.20230610094209/pyproject.toml
+-rw-r--r--   0        0        0      205 2023-06-10 09:30:47.427306 foreverbull-0.0.0.99.20230610094209/src/foreverbull/__init__.py
+-rw-r--r--   0        0        0     7271 2023-06-10 09:30:47.427893 foreverbull-0.0.0.99.20230610094209/src/foreverbull/__main__.py
+-rw-r--r--   0        0        0      140 2023-06-10 09:30:47.428372 foreverbull-0.0.0.99.20230610094209/src/foreverbull/data/__init__.py
+-rw-r--r--   0        0        0     2332 2023-06-10 09:30:47.428763 foreverbull-0.0.0.99.20230610094209/src/foreverbull/data/data.py
+-rw-r--r--   0        0        0     1344 2023-06-10 09:30:47.429151 foreverbull-0.0.0.99.20230610094209/src/foreverbull/data/stock_data.py
+-rw-r--r--   0        0        0     3811 2023-06-10 09:30:47.429562 foreverbull-0.0.0.99.20230610094209/src/foreverbull/foreverbull.py
+-rw-r--r--   0        0        0     1298 2023-06-10 09:30:47.430050 foreverbull-0.0.0.99.20230610094209/src/foreverbull/models.py
+-rw-r--r--   0        0        0       71 2023-06-10 09:30:47.430567 foreverbull-0.0.0.99.20230610094209/src/foreverbull/worker/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-10 09:30:47.437221 foreverbull-0.0.0.99.20230610094209/src/foreverbull/worker/exceptions.py
+-rw-r--r--   0        0        0     8787 2023-06-10 09:30:47.443006 foreverbull-0.0.0.99.20230610094209/src/foreverbull/worker/worker.py
+-rw-r--r--   0        0        0       79 2023-06-10 09:30:47.443481 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/__init__.py
+-rw-r--r--   0        0        0      641 2023-06-10 09:30:47.445180 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/broker.py
+-rw-r--r--   0        0        0      104 2023-06-10 09:30:47.445508 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/__init__.py
+-rw-r--r--   0        0        0     1405 2023-06-10 09:30:47.445952 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/backtest.py
+-rw-r--r--   0        0        0       92 2023-06-10 09:30:47.446384 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/exceptions.py
+-rw-r--r--   0        0        0     2205 2023-06-10 09:30:47.446874 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/finance.py
+-rw-r--r--   0        0        0      510 2023-06-10 09:30:47.447286 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/http.py
+-rw-r--r--   0        0        0     2779 2023-06-10 09:30:47.447735 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/service.py
+-rw-r--r--   0        0        0     1103 2023-06-10 09:30:47.448072 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/strategy.py
+-rw-r--r--   0        0        0      742 2023-06-10 09:30:47.448379 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:30:47.448419 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/__init__.py
+-rw-r--r--   0        0        0     4823 2023-06-10 09:30:47.449342 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/backtest.py
+-rw-r--r--   0        0        0     1180 2023-06-10 09:30:47.449693 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/base.py
+-rw-r--r--   0        0        0     1214 2023-06-10 09:30:47.450003 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/finance.py
+-rw-r--r--   0        0        0     1529 2023-06-10 09:30:47.450428 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/service.py
+-rw-r--r--   0        0        0     1952 2023-06-10 09:30:47.450737 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/socket.py
+-rw-r--r--   0        0        0     1000 2023-06-10 09:30:47.451100 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/worker.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:30:47.451141 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/__init__.py
+-rw-r--r--   0        0        0     2916 2023-06-10 09:30:47.451979 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/client.py
+-rw-r--r--   0        0        0       83 2023-06-10 09:30:47.452393 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/exceptions.py
+-rw-r--r--   0        0        0     4194 2023-06-10 09:30:47.452695 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/nanomsg.py
+-rw-r--r--   0        0        0     2192 2023-06-10 09:30:47.453191 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 09:30:47.453271 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/storage/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-10 09:30:47.453926 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/storage/backtest.py
+-rw-r--r--   0        0        0      371 2023-06-10 09:30:47.454338 foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/storage/storage.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 foreverbull-0.0.0.99.20230610094209/PKG-INFO
```

### Comparing `foreverbull-0.0.0.92/LICENSE` & `foreverbull-0.0.0.99.20230610094209/LICENSE`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/pyproject.toml` & `foreverbull-0.0.0.99.20230610094209/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-[build-system]
-requires = [
-  "setuptools>=45.0",
-  "wheel",
-  "setuptools_scm"
-]
-build-backend = "setuptools.build_meta"
-
 [tool.ruff]
 fix = true
 target-version = "py38"
 line-length = 120
 
 [tool.ruff.isort]
 force-single-line = true
@@ -25,25 +17,29 @@
 [tool.isort]
 profile = "black"
 src_paths = ["src"]
 line_length = 120
 
 [tool.poetry]
 name = "foreverbull"
-version="0.0.0.92"
+version="0.0.0.99.20230610094209"
 description="foreverbull"
 authors = [ "Henrik Nilsson <henrik@lhjnilsson.com>" ]
 packages = [
     { include = "foreverbull", from = "src" },
     { include = "foreverbull_core", from = "src" }
 ]
 
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
 [tool.poetry-dynamic-versioning]
 enable = false
-format = "{base}.{distance}"
+format = "{base}.{distance}.{timestamp}"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 pydantic = ">=1.8.2,<2.0.0"
 pynng = ">=0.7.1,<1.0.0"
 minio = ">=7.1.14,<8.0.0"
```

### Comparing `foreverbull-0.0.0.92/src/foreverbull/__main__.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/__main__.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull/data/data.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/data/data.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull/data/stock_data.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/data/stock_data.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull/foreverbull.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/foreverbull.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull/models.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/models.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull/worker/worker.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull/worker/worker.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/broker.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/broker.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/http/backtest.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/http/finance.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/finance.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/http/service.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/service.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/http/strategy.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/http/strategy.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/logger.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/logger.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/backtest.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/base.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/base.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/finance.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/finance.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/service.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/service.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/socket.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/socket.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/models/worker.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/models/worker.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/socket/client.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/client.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/socket/nanomsg.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/nanomsg.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/socket/router.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/socket/router.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/src/foreverbull_core/storage/backtest.py` & `foreverbull-0.0.0.99.20230610094209/src/foreverbull_core/storage/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.0.92/PKG-INFO` & `foreverbull-0.0.0.99.20230610094209/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foreverbull
-Version: 0.0.0.92
+Version: 0.0.0.99.20230610094209
 Summary: foreverbull
 Author: Henrik Nilsson
 Author-email: henrik@lhjnilsson.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

