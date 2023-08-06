# Comparing `tmp/kufar-0.1.2.tar.gz` & `tmp/kufar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kufar-0.1.2.tar", max compression
+gzip compressed data, was "kufar-0.1.3.tar", max compression
```

## Comparing `kufar-0.1.2.tar` & `kufar-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1488 2023-08-06 19:07:08.660012 kufar-0.1.2/README.md
--rw-r--r--   0        0        0       68 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/__init__.py
--rw-r--r--   0        0        0     2250 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/_instance.py
--rw-r--r--   0        0        0       33 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/__init__.py
--rw-r--r--   0        0        0      311 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/consts.py
--rw-r--r--   0        0        0     1167 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/service.py
--rw-r--r--   0        0        0      206 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/__init__.py
--rw-r--r--   0        0        0       59 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/__init__.py
--rw-r--r--   0        0        0       49 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/consts.py
--rw-r--r--   0        0        0      347 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/instance.py
--rw-r--r--   0        0        0     1065 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/schemas.py
--rw-r--r--   0        0        0       56 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/__init__.py
--rw-r--r--   0        0        0      911 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/consts.py
--rw-r--r--   0        0        0     1680 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/instance.py
--rw-r--r--   0        0        0     1766 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/schemas.py
--rw-r--r--   0        0        0       57 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/__init__.py
--rw-r--r--   0        0        0      626 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/consts.py
--rw-r--r--   0        0        0     3017 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/instance.py
--rw-r--r--   0        0        0     1522 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/schemas.py
--rw-r--r--   0        0        0       61 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/__init__.py
--rw-r--r--   0        0        0       51 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/consts.py
--rw-r--r--   0        0        0      259 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/instance.py
--rw-r--r--   0        0        0      450 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/schemas.py
--rw-r--r--   0        0        0        0 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/favorites/__init__.py
--rw-r--r--   0        0        0      454 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/favorites/consts.py
--rw-r--r--   0        0        0       36 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/__init__.py
--rw-r--r--   0        0        0      315 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/consts.py
--rw-r--r--   0        0        0      783 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/instance.py
--rw-r--r--   0        0        0     1407 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/schemas.py
--rw-r--r--   0        0        0       61 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/__init__.py
--rw-r--r--   0        0        0       46 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/consts.py
--rw-r--r--   0        0        0      342 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/instance.py
--rw-r--r--   0        0        0      136 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/schemas.py
--rw-r--r--   0        0        0       58 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/__init__.py
--rw-r--r--   0        0        0      303 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/consts.py
--rw-r--r--   0        0        0     1041 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/instance.py
--rw-r--r--   0        0        0      522 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/schemas.py
--rw-r--r--   0        0        0       60 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/__init__.py
--rw-r--r--   0        0        0      269 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/consts.py
--rw-r--r--   0        0        0     1301 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/instance.py
--rw-r--r--   0        0        0     2429 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/schemas.py
--rw-r--r--   0        0        0      317 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/schemas.py
--rw-r--r--   0        0        0       58 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/__init__.py
--rw-r--r--   0        0        0      652 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/auth.py
--rw-r--r--   0        0        0     4665 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/requester.py
--rw-r--r--   0        0        0      327 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/signature_decoder.py
--rw-r--r--   0        0        0      942 2023-08-06 19:07:08.664013 kufar-0.1.2/kufar/utils/state.py
--rw-r--r--   0        0        0     1123 2023-08-06 19:07:08.664013 kufar-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 kufar-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:11:22.021892 kufar-0.1.3/README.md
+-rw-r--r--   0        0        0       68 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/__init__.py
+-rw-r--r--   0        0        0     2250 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/_instance.py
+-rw-r--r--   0        0        0       33 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/base/__init__.py
+-rw-r--r--   0        0        0      311 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/base/consts.py
+-rw-r--r--   0        0        0     1167 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/base/service.py
+-rw-r--r--   0        0        0      206 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/__init__.py
+-rw-r--r--   0        0        0       59 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/account/__init__.py
+-rw-r--r--   0        0        0       49 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/account/consts.py
+-rw-r--r--   0        0        0      347 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/account/instance.py
+-rw-r--r--   0        0        0     1065 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/account/schemas.py
+-rw-r--r--   0        0        0       56 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/ads/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/ads/consts.py
+-rw-r--r--   0        0        0     1680 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/ads/instance.py
+-rw-r--r--   0        0        0     1766 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/ads/schemas.py
+-rw-r--r--   0        0        0       57 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/auth/__init__.py
+-rw-r--r--   0        0        0      626 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/auth/consts.py
+-rw-r--r--   0        0        0     3017 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/auth/instance.py
+-rw-r--r--   0        0        0     1522 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/auth/schemas.py
+-rw-r--r--   0        0        0       61 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/categories/__init__.py
+-rw-r--r--   0        0        0       51 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/categories/consts.py
+-rw-r--r--   0        0        0      259 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/categories/instance.py
+-rw-r--r--   0        0        0      450 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/categories/schemas.py
+-rw-r--r--   0        0        0        0 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/favorites/__init__.py
+-rw-r--r--   0        0        0      454 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/favorites/consts.py
+-rw-r--r--   0        0        0       36 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/filters/__init__.py
+-rw-r--r--   0        0        0      315 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/filters/consts.py
+-rw-r--r--   0        0        0      783 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/filters/instance.py
+-rw-r--r--   0        0        0     1407 2023-08-06 19:11:22.021892 kufar-0.1.3/kufar/packages/filters/schemas.py
+-rw-r--r--   0        0        0       61 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/messaging/__init__.py
+-rw-r--r--   0        0        0       46 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/messaging/consts.py
+-rw-r--r--   0        0        0      342 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/messaging/instance.py
+-rw-r--r--   0        0        0      136 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/messaging/schemas.py
+-rw-r--r--   0        0        0       58 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/saved/__init__.py
+-rw-r--r--   0        0        0      303 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/saved/consts.py
+-rw-r--r--   0        0        0     1041 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/saved/instance.py
+-rw-r--r--   0        0        0      522 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/saved/schemas.py
+-rw-r--r--   0        0        0       60 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/user_ads/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/user_ads/consts.py
+-rw-r--r--   0        0        0     1301 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/user_ads/instance.py
+-rw-r--r--   0        0        0     2429 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/packages/user_ads/schemas.py
+-rw-r--r--   0        0        0      317 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/schemas.py
+-rw-r--r--   0        0        0       58 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/utils/__init__.py
+-rw-r--r--   0        0        0      652 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/utils/auth.py
+-rw-r--r--   0        0        0     4665 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/utils/requester.py
+-rw-r--r--   0        0        0      327 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/utils/signature_decoder.py
+-rw-r--r--   0        0        0      942 2023-08-06 19:11:22.025892 kufar-0.1.3/kufar/utils/state.py
+-rw-r--r--   0        0        0     1123 2023-08-06 19:11:22.025892 kufar-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 kufar-0.1.3/PKG-INFO
```

### Comparing `kufar-0.1.2/README.md` & `kufar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/_instance.py` & `kufar-0.1.3/kufar/_instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/base/service.py` & `kufar-0.1.3/kufar/base/service.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/account/schemas.py` & `kufar-0.1.3/kufar/packages/account/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/ads/consts.py` & `kufar-0.1.3/kufar/packages/ads/consts.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/ads/instance.py` & `kufar-0.1.3/kufar/packages/ads/instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/ads/schemas.py` & `kufar-0.1.3/kufar/packages/ads/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/auth/consts.py` & `kufar-0.1.3/kufar/packages/auth/consts.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/auth/instance.py` & `kufar-0.1.3/kufar/packages/auth/instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/auth/schemas.py` & `kufar-0.1.3/kufar/packages/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/filters/instance.py` & `kufar-0.1.3/kufar/packages/filters/instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/filters/schemas.py` & `kufar-0.1.3/kufar/packages/filters/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/saved/instance.py` & `kufar-0.1.3/kufar/packages/saved/instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/saved/schemas.py` & `kufar-0.1.3/kufar/packages/saved/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/user_ads/instance.py` & `kufar-0.1.3/kufar/packages/user_ads/instance.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/packages/user_ads/schemas.py` & `kufar-0.1.3/kufar/packages/user_ads/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/utils/auth.py` & `kufar-0.1.3/kufar/utils/auth.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/utils/requester.py` & `kufar-0.1.3/kufar/utils/requester.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/kufar/utils/state.py` & `kufar-0.1.3/kufar/utils/state.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.2/pyproject.toml` & `kufar-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kufar"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Kiel Ed <kieledssh@gmail.com>"]
 readme = "README.md"
 keywords = ["kufar", "kufar-api", "kufar_api"]
 packages = [
   { include = "kufar" }
 ]
```

### Comparing `kufar-0.1.2/PKG-INFO` & `kufar-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kufar
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Keywords: kufar,kufar-api,kufar_api
 Author: Kiel Ed
 Author-email: kieledssh@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

