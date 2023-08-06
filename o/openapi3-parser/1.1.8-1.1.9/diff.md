# Comparing `tmp/openapi3-parser-1.1.8.tar.gz` & `tmp/openapi3-parser-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi3-parser-1.1.8.tar", last modified: Fri Apr 21 19:45:13 2023, max compression
+gzip compressed data, was "openapi3-parser-1.1.9.tar", last modified: Thu Jun  1 20:35:29 2023, max compression
```

## Comparing `openapi3-parser-1.1.8.tar` & `openapi3-parser-1.1.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.307370 openapi3-parser-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-21 19:45:13.307370 openapi3-parser-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 19:45:13.307370 openapi3-parser-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.303370 openapi3-parser-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.303370 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-21 19:45:13.000000 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-21 19:45:13.000000 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:45:13.000000 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 19:45:13.000000 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 19:45:13.000000 openapi3-parser-1.1.8/src/openapi3_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.303370 openapi3-parser-1.1.8/src/openapi_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.303370 openapi3-parser-1.1.8/src/openapi_parser/builders/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/external_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/oauth_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/builders/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/loose_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/src/openapi_parser/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:45:13.307370 openapi3-parser-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/tests/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/tests/test_parser_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-21 19:44:50.000000 openapi3-parser-1.1.8/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.084006 openapi3-parser-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-01 20:35:29.084006 openapi3-parser-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-01 20:35:29.084006 openapi3-parser-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.072006 openapi3-parser-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.076006 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-01 20:35:29.000000 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 20:35:29.000000 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:35:29.000000 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 20:35:29.000000 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 20:35:29.000000 openapi3-parser-1.1.9/src/openapi3_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.076006 openapi3-parser-1.1.9/src/openapi_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.080006 openapi3-parser-1.1.9/src/openapi_parser/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/external_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/oauth_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/builders/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/loose_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/src/openapi_parser/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:35:29.084006 openapi3-parser-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/tests/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/tests/test_parser_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 20:34:56.000000 openapi3-parser-1.1.9/tests/test_runner.py
```

### Comparing `openapi3-parser-1.1.8/PKG-INFO` & `openapi3-parser-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3-parser
-Version: 1.1.8
+Version: 1.1.9
 Summary: OpenAPI v3 parser
 Home-page: https://github.com/manchenkoff/openapi3-parser
 Author: Artem Manchenkov
 Author-email: artem@manchenkoff.me
 License: MIT
 Project-URL: Source, https://github.com/manchenkoff/openapi3-parser
 Keywords: swagger,python,swagger-parser,openapi3-parser,parser,openapi3,swagger-api
```

### Comparing `openapi3-parser-1.1.8/license.txt` & `openapi3-parser-1.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/setup.cfg` & `openapi3-parser-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/setup.py` & `openapi3-parser-1.1.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     url="https://github.com/manchenkoff/openapi3-parser",
     project_urls={
         "Source": "https://github.com/manchenkoff/openapi3-parser",
     },
     version=openapi_parser.__version__,
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
+    package_data={"openapi_parser": ["py.typed"]},
     license="MIT",
     description=openapi_parser.__description__,
     long_description=open(description_file).read(),
     long_description_content_type="text/markdown",
     keywords="swagger, python, swagger-parser, openapi3-parser, parser, openapi3, swagger-api",
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `openapi3-parser-1.1.8/src/openapi3_parser.egg-info/PKG-INFO` & `openapi3-parser-1.1.9/src/openapi3_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3-parser
-Version: 1.1.8
+Version: 1.1.9
 Summary: OpenAPI v3 parser
 Home-page: https://github.com/manchenkoff/openapi3-parser
 Author: Artem Manchenkov
 Author-email: artem@manchenkoff.me
 License: MIT
 Project-URL: Source, https://github.com/manchenkoff/openapi3-parser
 Keywords: swagger,python,swagger-parser,openapi3-parser,parser,openapi3,swagger-api
```

### Comparing `openapi3-parser-1.1.8/src/openapi3_parser.egg-info/SOURCES.txt` & `openapi3-parser-1.1.9/src/openapi3_parser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/openapi3_parser.egg-info/requires.txt
 src/openapi3_parser.egg-info/top_level.txt
 src/openapi_parser/__init__.py
 src/openapi_parser/enumeration.py
 src/openapi_parser/errors.py
 src/openapi_parser/loose_types.py
 src/openapi_parser/parser.py
+src/openapi_parser/py.typed
 src/openapi_parser/resolver.py
 src/openapi_parser/specification.py
 src/openapi_parser/builders/__init__.py
 src/openapi_parser/builders/common.py
 src/openapi_parser/builders/content.py
 src/openapi_parser/builders/external_doc.py
 src/openapi_parser/builders/header.py
```

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/__init__.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/common.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/common.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/content.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/content.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/header.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/header.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/info.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/info.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/oauth_flow.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/operation.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/operation.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/parameter.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/path.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/path.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/request.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/request.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/response.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/response.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/schema.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/schema.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/schemas.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/schemas.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/security.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/security.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/server.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/server.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/builders/tag.py` & `openapi3-parser-1.1.9/src/openapi_parser/builders/tag.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/enumeration.py` & `openapi3-parser-1.1.9/src/openapi_parser/enumeration.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/parser.py` & `openapi3-parser-1.1.9/src/openapi_parser/parser.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/resolver.py` & `openapi3-parser-1.1.9/src/openapi_parser/resolver.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/src/openapi_parser/specification.py` & `openapi3-parser-1.1.9/src/openapi_parser/specification.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/tests/test_enumeration.py` & `openapi3-parser-1.1.9/tests/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/tests/test_parser.py` & `openapi3-parser-1.1.9/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `openapi3-parser-1.1.8/tests/test_parser_options.py` & `openapi3-parser-1.1.9/tests/test_parser_options.py`

 * *Files identical despite different names*

