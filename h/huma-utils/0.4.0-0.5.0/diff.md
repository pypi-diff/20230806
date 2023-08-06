# Comparing `tmp/huma_utils-0.4.0.tar.gz` & `tmp/huma_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_utils-0.4.0.tar", max compression
+gzip compressed data, was "huma_utils-0.5.0.tar", max compression
```

## Comparing `huma_utils-0.4.0.tar` & `huma_utils-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-07-15 00:26:44.760374 huma_utils-0.4.0/LICENSE
--rw-r--r--   0        0        0       35 2023-07-15 00:26:44.760374 huma_utils-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/__init__.py
--rw-r--r--   0        0        0      270 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/async_utils.py
--rw-r--r--   0        0        0      291 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/chain_utils.py
--rw-r--r--   0        0        0      330 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/datetime_utils.py
--rw-r--r--   0        0        0        0 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/py.typed
--rw-r--r--   0        0        0      428 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/pydantic_utils.py
--rw-r--r--   0        0        0      702 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/request_utils.py
--rw-r--r--   0        0        0     1113 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/string_utils.py
--rw-r--r--   0        0        0      543 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/address_helpers.py
--rw-r--r--   0        0        0      809 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/api_test_helpers.py
--rw-r--r--   0        0        0     2042 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/vcr_helpers.py
--rw-r--r--   0        0        0     1129 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/web3_utils.py
--rw-r--r--   0        0        0     2269 2023-07-15 00:26:44.764374 huma_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 huma_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-06 01:43:51.771354 huma_utils-0.5.0/LICENSE
+-rw-r--r--   0        0        0       35 2023-08-06 01:43:51.771354 huma_utils-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/__init__.py
+-rw-r--r--   0        0        0      270 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/async_utils.py
+-rw-r--r--   0        0        0      291 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/chain_utils.py
+-rw-r--r--   0        0        0      330 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/datetime_utils.py
+-rw-r--r--   0        0        0        0 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/py.typed
+-rw-r--r--   0        0        0      428 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/pydantic_utils.py
+-rw-r--r--   0        0        0      702 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/request_utils.py
+-rw-r--r--   0        0        0     1113 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/string_utils.py
+-rw-r--r--   0        0        0      543 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/test_helpers/address_helpers.py
+-rw-r--r--   0        0        0      809 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/test_helpers/api_test_helpers.py
+-rw-r--r--   0        0        0     2042 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/test_helpers/vcr_helpers.py
+-rw-r--r--   0        0        0     1129 2023-08-06 01:43:51.775354 huma_utils-0.5.0/huma_utils/web3_utils.py
+-rw-r--r--   0        0        0     2297 2023-08-06 01:43:51.775354 huma_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 huma_utils-0.5.0/PKG-INFO
```

### Comparing `huma_utils-0.4.0/LICENSE` & `huma_utils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/request_utils.py` & `huma_utils-0.5.0/huma_utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/string_utils.py` & `huma_utils-0.5.0/huma_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/test_helpers/address_helpers.py` & `huma_utils-0.5.0/huma_utils/test_helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/test_helpers/api_test_helpers.py` & `huma_utils-0.5.0/huma_utils/test_helpers/api_test_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/test_helpers/vcr_helpers.py` & `huma_utils-0.5.0/huma_utils/test_helpers/vcr_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/huma_utils/web3_utils.py` & `huma_utils-0.5.0/huma_utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.4.0/pyproject.toml` & `huma_utils-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "huma-utils"
-version = "0.4.0"
-description = ""
+version = "0.5.0"
+description = "Huma Python utilities library"
 authors = ["Flora Huang <flora@huma.finance>", "Jiatu Liu <jiatu@huma.finance>"]
 readme = "README.md"
 packages = [{include = "huma_utils"}]
 
 [tool.poetry.dependencies]
-python = "~3.10"
+python = "~3.11"
 httpx = "^0.24.1"
 orjson = "^3.9.1"
 pydantic = "^1.10.9"
 web3 = "^6.4.0"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-describe = "^2.1.0"
 pytest-asyncio = "^0.21.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

