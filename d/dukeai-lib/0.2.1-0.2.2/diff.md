# Comparing `tmp/dukeai_lib-0.2.1.tar.gz` & `tmp/dukeai_lib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.2.1.tar", last modified: Sun Aug  6 03:57:00 2023, max compression
+gzip compressed data, was "dukeai_lib-0.2.2.tar", last modified: Sun Aug  6 03:59:55 2023, max compression
```

## Comparing `dukeai_lib-0.2.1.tar` & `dukeai_lib-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.558985 dukeai_lib-0.2.1/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.2.1/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:57:00.558985 dukeai_lib-0.2.1/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.2.1/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.537985 dukeai_lib-0.2.1/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      244 2023-08-06 03:56:46.000000 dukeai_lib-0.2.1/dukeai_lib/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.2.1/dukeai_lib/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      116 2023-08-05 19:11:34.000000 dukeai_lib-0.2.1/dukeai_lib/globals.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.543985 dukeai_lib-0.2.1/dukeai_lib/load_transmission/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      108 2023-08-05 19:14:11.000000 dukeai_lib-0.2.1/dukeai_lib/load_transmission/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     6619 2023-08-06 03:45:42.000000 dukeai_lib-0.2.1/dukeai_lib/load_transmission/functions.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.553985 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/accessorial.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/bill_of_lading.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/classification.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/classification_exceptions.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/invoice.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/noa_lor.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/rate_confirmation.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/rsi_translator.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/schema_utilities.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      601 2023-08-06 03:45:42.000000 dukeai_lib-0.2.1/dukeai_lib/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    18350 2023-08-06 03:54:32.000000 dukeai_lib-0.2.1/dukeai_lib/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.541985 dukeai_lib-0.2.1/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:57:00.000000 dukeai_lib-0.2.1/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      967 2023-08-06 03:57:00.000000 dukeai_lib-0.2.1/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-08-06 03:57:00.000000 dukeai_lib-0.2.1/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-08-06 03:57:00.000000 dukeai_lib-0.2.1/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-08-06 03:57:00.000000 dukeai_lib-0.2.1/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      711 2023-08-06 03:56:46.000000 dukeai_lib-0.2.1/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-08-06 03:57:00.558985 dukeai_lib-0.2.1/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      924 2023-08-06 03:56:46.000000 dukeai_lib-0.2.1/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:57:00.557985 dukeai_lib-0.2.1/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.2.1/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.2.1/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.1/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.2.1/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.835908 dukeai_lib-0.2.2/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.2.2/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:59:55.834908 dukeai_lib-0.2.2/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.2.2/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.814923 dukeai_lib-0.2.2/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      244 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/dukeai_lib/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.2.2/dukeai_lib/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      116 2023-08-05 19:11:34.000000 dukeai_lib-0.2.2/dukeai_lib/globals.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.820908 dukeai_lib-0.2.2/dukeai_lib/load_transmission/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       59 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/dukeai_lib/load_transmission/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     6619 2023-08-06 03:45:42.000000 dukeai_lib-0.2.2/dukeai_lib/load_transmission/functions.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.830907 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/accessorial.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/bill_of_lading.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification_exceptions.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/invoice.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/noa_lor.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rate_confirmation.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rsi_translator.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/schema_utilities.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      601 2023-08-06 03:45:42.000000 dukeai_lib-0.2.2/dukeai_lib/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    18350 2023-08-06 03:54:32.000000 dukeai_lib-0.2.2/dukeai_lib/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.818907 dukeai_lib-0.2.2/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      967 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-08-06 03:59:55.000000 dukeai_lib-0.2.2/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      711 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-08-06 03:59:55.835908 dukeai_lib-0.2.2/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      924 2023-08-06 03:59:47.000000 dukeai_lib-0.2.2/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-06 03:59:55.834908 dukeai_lib-0.2.2/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.2.2/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.2.2/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.2/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.2.2/src/utilities.py
```

### Comparing `dukeai_lib-0.2.1/LICENSE` & `dukeai_lib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/PKG-INFO` & `dukeai_lib-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.2.1/README.md` & `dukeai_lib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/application.py` & `dukeai_lib-0.2.2/dukeai_lib/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/load_transmission/functions.py` & `dukeai_lib-0.2.2/dukeai_lib/load_transmission/functions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/accessorial.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/accessorial.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/bill_of_lading.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/bill_of_lading.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/classification.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/classification_exceptions.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/classification_exceptions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/invoice.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/invoice.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/noa_lor.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/noa_lor.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/parse_classification_page_range.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/parse_classification_page_range.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/rate_confirmation.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rate_confirmation.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/rsi_translator.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/rsi_translator.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/schema_kung_fu/schema_utilities.py` & `dukeai_lib-0.2.2/dukeai_lib/schema_kung_fu/schema_utilities.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/tools.py` & `dukeai_lib-0.2.2/dukeai_lib/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib/utilities.py` & `dukeai_lib-0.2.2/dukeai_lib/utilities.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.2.2/dukeai_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.2.1/dukeai_lib.egg-info/SOURCES.txt` & `dukeai_lib-0.2.2/dukeai_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/pyproject.toml` & `dukeai_lib-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.2.1/setup.py` & `dukeai_lib-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.2.1",
+    version="0.2.2",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
```

### Comparing `dukeai_lib-0.2.1/src/application.py` & `dukeai_lib-0.2.2/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.2.1/src/tools.py` & `dukeai_lib-0.2.2/src/tools.py`

 * *Files identical despite different names*

