# Comparing `tmp/datclass-0.2.3.tar.gz` & `tmp/datclass-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datclass-0.2.3.tar", last modified: Fri Aug  4 11:38:20 2023, max compression
+gzip compressed data, was "datclass-0.2.4.tar", last modified: Sun Aug  6 03:58:36 2023, max compression
```

## Comparing `datclass-0.2.3.tar` & `datclass-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.801518 datclass-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 11:38:10.000000 datclass-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 11:38:10.000000 datclass-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-04 11:38:20.797517 datclass-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-04 11:38:10.000000 datclass-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 11:38:10.000000 datclass-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:38:10.000000 datclass-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:38:20.801518 datclass-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/datclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-04 11:38:19.000000 datclass-0.2.3/src/datclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/datclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:58:36.576074 datclass-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-06 03:58:29.000000 datclass-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 03:58:29.000000 datclass-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-06 03:58:36.572074 datclass-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-06 03:58:29.000000 datclass-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-06 03:58:29.000000 datclass-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:58:29.000000 datclass-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:58:36.576074 datclass-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:58:36.572074 datclass-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:58:36.572074 datclass-0.2.4/src/datclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-08-06 03:58:35.000000 datclass-0.2.4/src/datclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 03:58:29.000000 datclass-0.2.4/src/datclass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-08-06 03:58:29.000000 datclass-0.2.4/src/datclass/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-06 03:58:29.000000 datclass-0.2.4/src/datclass/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:58:36.572074 datclass-0.2.4/src/datclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 03:58:36.000000 datclass-0.2.4/src/datclass.egg-info/top_level.txt
```

### Comparing `datclass-0.2.3/LICENSE` & `datclass-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datclass-0.2.3/PKG-INFO` & `datclass-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.2.3
+Version: 0.2.4
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

### Comparing `datclass-0.2.3/README.md` & `datclass-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `datclass-0.2.3/pyproject.toml` & `datclass-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datclass-0.2.3/src/datclass/__init__.py` & `datclass-0.2.4/src/datclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = 'datclass'
 __author__ = 'foyoux'
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 __all__ = [
     'main',
     'DatGen',
     'DatClass',
     'get_datclass',
 ]
@@ -67,15 +67,16 @@
                 origin = get_origin(attr_type)
                 if origin is None and is_dataclass(attr_type):
                     attr = getattr(self, attr_name)
                     setattr(self, attr_name, attr_type(**attr) if attr else None)
                     continue
                 for item_type in get_args(attr_type):
                     if is_dataclass(item_type):
-                        setattr(self, attr_name, [item_type(**i) for i in getattr(self, attr_name) or []])
+                        setattr(self, attr_name,
+                                [i if is_dataclass(i) else item_type(**i) for i in getattr(self, attr_name) or []])
 
     return __datclass__
 
 
 DatClass = get_datclass()
```

### Comparing `datclass-0.2.3/src/datclass/gens.py` & `datclass-0.2.4/src/datclass/gens.py`

 * *Files identical despite different names*

### Comparing `datclass-0.2.3/src/datclass/utils.py` & `datclass-0.2.4/src/datclass/utils.py`

 * *Files identical despite different names*

### Comparing `datclass-0.2.3/src/datclass.egg-info/PKG-INFO` & `datclass-0.2.4/src/datclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.2.3
+Version: 0.2.4
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

