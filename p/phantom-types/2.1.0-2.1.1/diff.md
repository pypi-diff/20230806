# Comparing `tmp/phantom-types-2.1.0.tar.gz` & `tmp/phantom-types-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phantom-types-2.1.0.tar", last modified: Sun Jun 11 19:42:27 2023, max compression
+gzip compressed data, was "phantom-types-2.1.1.tar", last modified: Sun Aug  6 12:47:55 2023, max compression
```

## Comparing `phantom-types-2.1.0.tar` & `phantom-types-2.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-11 19:42:06.000000 phantom-types-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-11 19:42:06.000000 phantom-types-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-11 19:42:27.411161 phantom-types-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-11 19:42:06.000000 phantom-types-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-11 19:42:06.000000 phantom-types-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-11 19:42:27.411161 phantom-types-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 19:42:06.000000 phantom-types-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.407161 phantom-types-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_hypothesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/_utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/ext/phonenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/iso3166.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/negated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom/predicates/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/predicates/re.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-11 19:42:06.000000 phantom-types-2.1.0/src/phantom/sized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:42:27.411161 phantom-types-2.1.0/src/phantom_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:42:27.000000 phantom-types-2.1.0/src/phantom_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 12:47:46.000000 phantom-types-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-06 12:47:46.000000 phantom-types-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-08-06 12:47:55.869621 phantom-types-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-08-06 12:47:46.000000 phantom-types-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-06 12:47:46.000000 phantom-types-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-06 12:47:55.869621 phantom-types-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:47:46.000000 phantom-types-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.865621 phantom-types-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/src/phantom/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/_hypothesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/src/phantom/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/_utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/src/phantom/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/ext/phonenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/iso3166.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/negated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/src/phantom/predicates/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/predicates/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-08-06 12:47:46.000000 phantom-types-2.1.1/src/phantom/sized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:47:55.869621 phantom-types-2.1.1/src/phantom_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-08-06 12:47:55.000000 phantom-types-2.1.1/src/phantom_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-06 12:47:55.000000 phantom-types-2.1.1/src/phantom_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:47:55.000000 phantom-types-2.1.1/src/phantom_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-06 12:47:55.000000 phantom-types-2.1.1/src/phantom_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 12:47:55.000000 phantom-types-2.1.1/src/phantom_types.egg-info/top_level.txt
```

### Comparing `phantom-types-2.1.0/LICENSE` & `phantom-types-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/PKG-INFO` & `phantom-types-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 2.1.0
+Version: 2.1.1
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
```

### Comparing `phantom-types-2.1.0/README.md` & `phantom-types-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/pyproject.toml` & `phantom-types-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/setup.cfg` & `phantom-types-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [options.package_data]
 phantom = py.typed
 
 [options.extras_require]
 phonenumbers = 
 	phonenumbers>=8.12.41
 pydantic = 
-	pydantic>=1.9.0
+	pydantic>=1.9.0,<2
 dateutil = 
 	python-dateutil>=2.8.2
 hypothesis = 
 	hypothesis[zoneinfo]>=6.68.0
 all = 
 	phantom-types[phonenumbers]
 	phantom-types[pydantic]
```

### Comparing `phantom-types-2.1.0/src/phantom/__init__.py` & `phantom-types-2.1.1/src/phantom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ._base import Phantom
 from ._base import PhantomBase
 from ._base import PhantomMeta
 from .bounds import get_bound_parser
 from .errors import BoundError
 from .predicates import Predicate
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __all__ = (
     "BoundError",
     "Phantom",
     "PhantomBase",
     "PhantomMeta",
     "get_bound_parser",
     "Predicate",
```

### Comparing `phantom-types-2.1.0/src/phantom/_base.py` & `phantom-types-2.1.1/src/phantom/_base.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/_hypothesis.py` & `phantom-types-2.1.1/src/phantom/_hypothesis.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/_utils/misc.py` & `phantom-types-2.1.1/src/phantom/_utils/misc.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/_utils/types.py` & `phantom-types-2.1.1/src/phantom/_utils/types.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/boolean.py` & `phantom-types-2.1.1/src/phantom/boolean.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/bounds.py` & `phantom-types-2.1.1/src/phantom/bounds.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/datetime.py` & `phantom-types-2.1.1/src/phantom/datetime.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/ext/phonenumbers.py` & `phantom-types-2.1.1/src/phantom/ext/phonenumbers.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/fn.py` & `phantom-types-2.1.1/src/phantom/fn.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/interval.py` & `phantom-types-2.1.1/src/phantom/interval.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/iso3166.py` & `phantom-types-2.1.1/src/phantom/iso3166.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/negated.py` & `phantom-types-2.1.1/src/phantom/negated.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/_utils.py` & `phantom-types-2.1.1/src/phantom/predicates/_utils.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/boolean.py` & `phantom-types-2.1.1/src/phantom/predicates/boolean.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/collection.py` & `phantom-types-2.1.1/src/phantom/predicates/collection.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/generic.py` & `phantom-types-2.1.1/src/phantom/predicates/generic.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/interval.py` & `phantom-types-2.1.1/src/phantom/predicates/interval.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/numeric.py` & `phantom-types-2.1.1/src/phantom/predicates/numeric.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/predicates/re.py` & `phantom-types-2.1.1/src/phantom/predicates/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/re.py` & `phantom-types-2.1.1/src/phantom/re.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom/schema.py` & `phantom-types-2.1.1/src/phantom/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing_extensions import TypedDict
 from typing_extensions import final
 
 
 class Schema(TypedDict, total=False):
     title: str
     description: str
-    type: Literal["array", "string", "float", "number"]  # noqa: A003
-    format: str  # noqa: A003
+    type: Literal["array", "string", "float", "number"]
+    format: str
     examples: Sequence[object]
     minimum: Optional[float]
     maximum: Optional[float]
     exclusiveMinimum: Optional[float]
     exclusiveMaximum: Optional[float]
     minItems: Optional[int]
     maxItems: Optional[int]
```

### Comparing `phantom-types-2.1.0/src/phantom/sized.py` & `phantom-types-2.1.1/src/phantom/sized.py`

 * *Files identical despite different names*

### Comparing `phantom-types-2.1.0/src/phantom_types.egg-info/PKG-INFO` & `phantom-types-2.1.1/src/phantom_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phantom-types
-Version: 2.1.0
+Version: 2.1.1
 Summary: Phantom types for Python
 Home-page: https://github.com/antonagestam/phantom-types/
 Author: Anton Agestam
 Author-email: git@antonagestam.se
 License: BSD 3-Clause License
 Project-URL: Source Repository, https://github.com/antonagestam/phantom-types/
 Project-URL: Documentation, https://phantom-types.readthedocs.io/en/stable/
```

### Comparing `phantom-types-2.1.0/src/phantom_types.egg-info/SOURCES.txt` & `phantom-types-2.1.1/src/phantom_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

