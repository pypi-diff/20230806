# Comparing `tmp/snap-helpers-0.4.0.tar.gz` & `tmp/snap-helpers-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap-helpers-0.4.0.tar", last modified: Sun Jul 16 17:10:42 2023, max compression
+gzip compressed data, was "snap-helpers-0.4.1.tar", last modified: Sun Aug  6 08:06:30 2023, max compression
```

## Comparing `snap-helpers-0.4.0.tar` & `snap-helpers-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/
--rw-rw-r--   0 ack       (1000) ack       (1000)     7652 2019-03-06 14:04:03.000000 snap-helpers-0.4.0/LICENSE.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)     8758 2023-04-06 22:14:25.000000 snap-helpers-0.4.0/README.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)     2301 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/pyproject.toml
--rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/setup.cfg
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snap_helpers.egg-info/
--rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)      596 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       73 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/entry_points.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       84 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/requires.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       12 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/top_level.txt
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snaphelpers/
--rw-rw-r--   0 ack       (1000) ack       (1000)      670 2023-07-16 16:46:21.000000 snap-helpers-0.4.0/snaphelpers/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3798 2023-03-15 07:35:35.000000 snap-helpers-0.4.0/snaphelpers/_conf.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     9301 2023-04-22 08:36:28.000000 snap-helpers-0.4.0/snaphelpers/_ctl.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1590 2023-03-15 07:43:44.000000 snap-helpers-0.4.0/snaphelpers/_env.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1862 2023-03-05 09:31:10.000000 snap-helpers-0.4.0/snaphelpers/_health.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1768 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/snaphelpers/_hook.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      366 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/snaphelpers/_importlib.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2244 2023-03-11 23:44:03.000000 snap-helpers-0.4.0/snaphelpers/_meta.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      964 2023-03-11 23:44:03.000000 snap-helpers-0.4.0/snaphelpers/_path.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2585 2023-03-05 09:31:10.000000 snap-helpers-0.4.0/snaphelpers/_service.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1949 2023-03-15 07:42:04.000000 snap-helpers-0.4.0/snaphelpers/_snap.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snaphelpers/scripts/
--rw-rw-r--   0 ack       (1000) ack       (1000)        0 2023-02-27 23:36:00.000000 snap-helpers-0.4.0/snaphelpers/scripts/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1434 2023-03-14 16:12:46.000000 snap-helpers-0.4.0/snaphelpers/scripts/_script.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     4666 2023-03-14 19:36:28.000000 snap-helpers-0.4.0/snaphelpers/scripts/snap_helpers.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-08-06 08:06:30.341610 snap-helpers-0.4.1/
+-rw-rw-r--   0 ack       (1000) ack       (1000)     7652 2019-03-06 14:04:03.000000 snap-helpers-0.4.1/LICENSE.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-08-06 08:06:30.341610 snap-helpers-0.4.1/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)     8758 2023-04-06 22:14:25.000000 snap-helpers-0.4.1/README.rst
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2360 2023-08-06 08:04:00.000000 snap-helpers-0.4.1/pyproject.toml
+-rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-08-06 08:06:30.341610 snap-helpers-0.4.1/setup.cfg
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-08-06 08:06:30.337610 snap-helpers-0.4.1/snap_helpers.egg-info/
+-rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)      617 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       73 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/entry_points.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       84 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/requires.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       12 2023-08-06 08:06:30.000000 snap-helpers-0.4.1/snap_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-08-06 08:06:30.341610 snap-helpers-0.4.1/snaphelpers/
+-rw-rw-r--   0 ack       (1000) ack       (1000)      670 2023-08-06 08:05:36.000000 snap-helpers-0.4.1/snaphelpers/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     3798 2023-03-15 07:35:35.000000 snap-helpers-0.4.1/snaphelpers/_conf.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     9301 2023-04-22 08:36:28.000000 snap-helpers-0.4.1/snaphelpers/_ctl.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1590 2023-03-15 07:43:44.000000 snap-helpers-0.4.1/snaphelpers/_env.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1862 2023-03-05 09:31:10.000000 snap-helpers-0.4.1/snaphelpers/_health.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1768 2023-07-16 16:35:24.000000 snap-helpers-0.4.1/snaphelpers/_hook.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      366 2023-07-16 16:35:24.000000 snap-helpers-0.4.1/snaphelpers/_importlib.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2244 2023-03-11 23:44:03.000000 snap-helpers-0.4.1/snaphelpers/_meta.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      964 2023-03-11 23:44:03.000000 snap-helpers-0.4.1/snaphelpers/_path.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2585 2023-03-05 09:31:10.000000 snap-helpers-0.4.1/snaphelpers/_service.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1949 2023-03-15 07:42:04.000000 snap-helpers-0.4.1/snaphelpers/_snap.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)        0 2023-04-06 22:09:39.000000 snap-helpers-0.4.1/snaphelpers/py.typed
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-08-06 08:06:30.341610 snap-helpers-0.4.1/snaphelpers/scripts/
+-rw-rw-r--   0 ack       (1000) ack       (1000)        0 2023-02-27 23:36:00.000000 snap-helpers-0.4.1/snaphelpers/scripts/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1434 2023-03-14 16:12:46.000000 snap-helpers-0.4.1/snaphelpers/scripts/_script.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4666 2023-03-14 19:36:28.000000 snap-helpers-0.4.1/snaphelpers/scripts/snap_helpers.py
```

### Comparing `snap-helpers-0.4.0/LICENSE.txt` & `snap-helpers-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/PKG-INFO` & `snap-helpers-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-helpers
-Version: 0.4.0
+Version: 0.4.1
 Summary: Helpers for interacting with the Snap system within a Snap
 Author-email: Alberto Donato <alberto.donato@gmail.com>
 Maintainer-email: Alberto Donato <alberto.donato@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `snap-helpers-0.4.0/README.rst` & `snap-helpers-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/pyproject.toml` & `snap-helpers-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 repository = "https://github.com/albertodonato/snap-helpers"
 [project.scripts]
 snap-helpers = "snaphelpers.scripts.snap_helpers:script"
 
 [tool.setuptools.packages.find]
 include = ["snaphelpers*"]
 
+[tool.setuptools.package-data]
+snaphelpers = ["py.typed"]
+
 [tool.setuptools.dynamic]
 version = {attr = "snaphelpers.__version__"}
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
```

### Comparing `snap-helpers-0.4.0/snap_helpers.egg-info/PKG-INFO` & `snap-helpers-0.4.1/snap_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-helpers
-Version: 0.4.0
+Version: 0.4.1
 Summary: Helpers for interacting with the Snap system within a Snap
 Author-email: Alberto Donato <alberto.donato@gmail.com>
 Maintainer-email: Alberto Donato <alberto.donato@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `snap-helpers-0.4.0/snap_helpers.egg-info/SOURCES.txt` & `snap-helpers-0.4.1/snap_helpers.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 snaphelpers/_health.py
 snaphelpers/_hook.py
 snaphelpers/_importlib.py
 snaphelpers/_meta.py
 snaphelpers/_path.py
 snaphelpers/_service.py
 snaphelpers/_snap.py
+snaphelpers/py.typed
 snaphelpers/scripts/__init__.py
 snaphelpers/scripts/_script.py
 snaphelpers/scripts/snap_helpers.py
```

### Comparing `snap-helpers-0.4.0/snaphelpers/__init__.py` & `snap-helpers-0.4.1/snaphelpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     "SnapHealth",
     "SnapPaths",
     "SnapServices",
     "UnknownConfigKey",
     "__version__",
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `snap-helpers-0.4.0/snaphelpers/_conf.py` & `snap-helpers-0.4.1/snaphelpers/_conf.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_ctl.py` & `snap-helpers-0.4.1/snaphelpers/_ctl.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_env.py` & `snap-helpers-0.4.1/snaphelpers/_env.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_health.py` & `snap-helpers-0.4.1/snaphelpers/_health.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_hook.py` & `snap-helpers-0.4.1/snaphelpers/_hook.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_meta.py` & `snap-helpers-0.4.1/snaphelpers/_meta.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_path.py` & `snap-helpers-0.4.1/snaphelpers/_path.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_service.py` & `snap-helpers-0.4.1/snaphelpers/_service.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/_snap.py` & `snap-helpers-0.4.1/snaphelpers/_snap.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/scripts/_script.py` & `snap-helpers-0.4.1/snaphelpers/scripts/_script.py`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.4.0/snaphelpers/scripts/snap_helpers.py` & `snap-helpers-0.4.1/snaphelpers/scripts/snap_helpers.py`

 * *Files identical despite different names*

