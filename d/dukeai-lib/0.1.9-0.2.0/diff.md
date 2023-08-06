# Comparing `tmp/dukeai_lib-0.1.9.tar.gz` & `tmp/dukeai_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.9.tar", last modified: Tue Jul 25 20:19:30 2023, max compression
+gzip compressed data, was "dukeai_lib-0.2.0.tar", last modified: Sat Aug  5 19:35:40 2023, max compression
```

## Comparing `dukeai_lib-0.1.9.tar` & `dukeai_lib-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.9/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.1.9/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.766007 dukeai_lib-0.1.9/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      216 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/dukeai_lib/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.9/dukeai_lib/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.781007 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/accessorial.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/bill_of_lading.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification_exceptions.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/invoice.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/noa_lor.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rate_confirmation.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rsi_translator.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/schema_utilities.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.9/dukeai_lib/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.9/dukeai_lib/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.770006 dukeai_lib-0.1.9/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2161 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      862 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 20:19:30.000000 dukeai_lib-0.1.9/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 20:19:30.785006 dukeai_lib-0.1.9/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 20:19:22.000000 dukeai_lib-0.1.9/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 20:19:30.784007 dukeai_lib-0.1.9/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.1.9/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.1.9/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.9/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.9/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.590645 dukeai_lib-0.2.0/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.2.0/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-05 19:35:40.590645 dukeai_lib-0.2.0/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1546 2023-07-25 20:07:46.000000 dukeai_lib-0.2.0/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.568644 dukeai_lib-0.2.0/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      244 2023-08-05 19:14:11.000000 dukeai_lib-0.2.0/dukeai_lib/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.2.0/dukeai_lib/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      116 2023-08-05 19:11:34.000000 dukeai_lib-0.2.0/dukeai_lib/globals.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.574645 dukeai_lib-0.2.0/dukeai_lib/load_transmission/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      108 2023-08-05 19:14:11.000000 dukeai_lib-0.2.0/dukeai_lib/load_transmission/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     4741 2023-08-05 19:35:18.000000 dukeai_lib-0.2.0/dukeai_lib/load_transmission/functions.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.585645 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      227 2023-07-25 20:09:28.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8318 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/accessorial.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    17455 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/bill_of_lading.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    14694 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/classification.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1294 2023-07-25 19:53:30.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/classification_exceptions.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    13798 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/invoice.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8933 2023-07-25 19:35:31.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/noa_lor.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8825 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/parse_classification_page_range.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    64258 2023-07-25 20:18:53.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/rate_confirmation.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     9397 2023-07-25 19:48:24.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/rsi_translator.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     8445 2023-07-25 19:48:24.000000 dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/schema_utilities.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.0/dukeai_lib/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2727 2023-08-05 19:35:18.000000 dukeai_lib-0.2.0/dukeai_lib/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.573645 dukeai_lib-0.2.0/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     2114 2023-08-05 19:35:40.000000 dukeai_lib-0.2.0/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      967 2023-08-05 19:35:40.000000 dukeai_lib-0.2.0/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-08-05 19:35:40.000000 dukeai_lib-0.2.0/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-08-05 19:35:40.000000 dukeai_lib-0.2.0/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-08-05 19:35:40.000000 dukeai_lib-0.2.0/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      711 2023-08-05 19:29:35.000000 dukeai_lib-0.2.0/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-08-05 19:35:40.590645 dukeai_lib-0.2.0/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      924 2023-08-05 19:29:35.000000 dukeai_lib-0.2.0/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-08-05 19:35:40.589645 dukeai_lib-0.2.0/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      204 2023-07-25 18:46:18.000000 dukeai_lib-0.2.0/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3601 2023-07-25 18:56:49.000000 dukeai_lib-0.2.0/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.2.0/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.2.0/src/utilities.py
```

### Comparing `dukeai_lib-0.1.9/LICENSE` & `dukeai_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/PKG-INFO` & `dukeai_lib-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Duke.ai Lib (*dukeai_lib*)
```

### Comparing `dukeai_lib-0.1.9/README.md` & `dukeai_lib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/application.py` & `dukeai_lib-0.2.0/dukeai_lib/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/accessorial.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/accessorial.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/bill_of_lading.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/bill_of_lading.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/classification.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/classification_exceptions.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/classification_exceptions.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/invoice.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/invoice.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/noa_lor.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/noa_lor.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/parse_classification_page_range.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/parse_classification_page_range.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rate_confirmation.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/rate_confirmation.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/rsi_translator.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/rsi_translator.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/schema_kung_fu/schema_utilities.py` & `dukeai_lib-0.2.0/dukeai_lib/schema_kung_fu/schema_utilities.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib/tools.py` & `dukeai_lib-0.2.0/dukeai_lib/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.2.0/dukeai_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Duke.ai Lib (*dukeai_lib*)
```

### Comparing `dukeai_lib-0.1.9/dukeai_lib.egg-info/SOURCES.txt` & `dukeai_lib-0.2.0/dukeai_lib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 dukeai_lib/__init__.py
 dukeai_lib/application.py
+dukeai_lib/globals.py
 dukeai_lib/tools.py
 dukeai_lib/utilities.py
 dukeai_lib.egg-info/PKG-INFO
 dukeai_lib.egg-info/SOURCES.txt
 dukeai_lib.egg-info/dependency_links.txt
 dukeai_lib.egg-info/requires.txt
 dukeai_lib.egg-info/top_level.txt
+dukeai_lib/load_transmission/__init__.py
+dukeai_lib/load_transmission/functions.py
 dukeai_lib/schema_kung_fu/__init__.py
 dukeai_lib/schema_kung_fu/accessorial.py
 dukeai_lib/schema_kung_fu/bill_of_lading.py
 dukeai_lib/schema_kung_fu/classification.py
 dukeai_lib/schema_kung_fu/classification_exceptions.py
 dukeai_lib/schema_kung_fu/invoice.py
 dukeai_lib/schema_kung_fu/noa_lor.py
```

### Comparing `dukeai_lib-0.1.9/pyproject.toml` & `dukeai_lib-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
     "Topic :: Utilities"
 ]
 dependencies = [
     'chalice~=1.27.1',
     'requests~=2.27.1',
     'base58==2.1.1',
     'urllib3==1.26.9'
```

### Comparing `dukeai_lib-0.1.9/setup.py` & `dukeai_lib-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.1.9",
+    version="0.2.0",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
@@ -17,11 +17,14 @@
         'urllib3==1.26.9'
     ],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: OS Independent",
         "Topic :: Utilities"
     ],
 )
+
+# python3 -m build
+# python3 -m twine upload --repository duke-pypi dist/dukeai_lib-0.1.9*
+
```

### Comparing `dukeai_lib-0.1.9/src/application.py` & `dukeai_lib-0.2.0/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.9/src/tools.py` & `dukeai_lib-0.2.0/src/tools.py`

 * *Files identical despite different names*

