# Comparing `tmp/SQLAlchemyExample-0.1.4.tar.gz` & `tmp/SQLAlchemyExample-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLAlchemyExample-0.1.4.tar", last modified: Fri Aug  4 01:05:47 2023, max compression
+gzip compressed data, was "SQLAlchemyExample-0.1.5.tar", last modified: Sat Aug  5 23:02:22 2023, max compression
```

## Comparing `SQLAlchemyExample-0.1.4.tar` & `SQLAlchemyExample-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-04 01:05:47.000000 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-04 01:05:47.000000 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:05:47.000000 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 01:05:47.000000 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:05:47.000000 SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:05:47.524157 SQLAlchemyExample-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/tests/test_otm_bi_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/tests/test_otm_uni_single_table_inherit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-04 01:05:38.000000 SQLAlchemyExample-0.1.4/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:02:22.000000 SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:02:22.034472 SQLAlchemyExample-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex01_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex02_otm_bi_single_table_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-05 23:02:12.000000 SQLAlchemyExample-0.1.5/tests/test_ex03_otm_uni_single_table_inherit.py
```

### Comparing `SQLAlchemyExample-0.1.4/LICENSE` & `SQLAlchemyExample-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.4/PKG-INFO` & `SQLAlchemyExample-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.4
+Version: 0.1.5
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
```

### Comparing `SQLAlchemyExample-0.1.4/README.rst` & `SQLAlchemyExample-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.4/pyproject.toml` & `SQLAlchemyExample-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.4/requirements.txt` & `SQLAlchemyExample-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `SQLAlchemyExample-0.1.4/setup.cfg` & `SQLAlchemyExample-0.1.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SQLAlchemyExample
-version = 0.1.4
+version = 0.1.5
 author = Hendrik du Toit
 author_email = hendrik@brightedge.co.za
 description = Exploring SQLAlchemy
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `SQLAlchemyExample-0.1.4/src/SQLAlchemyExample.egg-info/PKG-INFO` & `SQLAlchemyExample-0.1.5/src/SQLAlchemyExample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLAlchemyExample
-Version: 0.1.4
+Version: 0.1.5
 Summary: Exploring SQLAlchemy
 Author: Hendrik du Toit
 Author-email: hendrik@brightedge.co.za
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
```

