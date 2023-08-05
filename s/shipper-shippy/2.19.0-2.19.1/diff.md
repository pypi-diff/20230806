# Comparing `tmp/shipper-shippy-2.19.0.tar.gz` & `tmp/shipper-shippy-2.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.19.0.tar", last modified: Wed Aug  2 04:59:27 2023, max compression
+gzip compressed data, was "shipper-shippy-2.19.1.tar", last modified: Sat Aug  5 23:14:14 2023, max compression
```

## Comparing `shipper-shippy-2.19.0.tar` & `shipper-shippy-2.19.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 04:59:27.000000 shipper-shippy-2.19.0/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:27.570995 shipper-shippy-2.19.0/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 04:59:16.000000 shipper-shippy-2.19.0/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:14:14.896396 shipper-shippy-2.19.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-05 23:14:14.896396 shipper-shippy-2.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 23:14:14.896396 shipper-shippy-2.19.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:14:14.896396 shipper-shippy-2.19.1/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 23:14:14.000000 shipper-shippy-2.19.1/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:14:14.896396 shipper-shippy-2.19.1/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 23:14:03.000000 shipper-shippy-2.19.1/shippy/version.py
```

### Comparing `shipper-shippy-2.19.0/PKG-INFO` & `shipper-shippy-2.19.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.19.0
+Version: 2.19.1
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.19.0/README.md` & `shipper-shippy-2.19.1/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/setup.py` & `shipper-shippy-2.19.1/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.19.1/shipper_shippy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.19.0
+Version: 2.19.1
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.19.0/shippy/__main__.py` & `shipper-shippy-2.19.1/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/shippy/client.py` & `shipper-shippy-2.19.1/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/shippy/config.py` & `shipper-shippy-2.19.1/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/shippy/constants.py` & `shipper-shippy-2.19.1/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.19.0/shippy/helper.py` & `shipper-shippy-2.19.1/shippy/helper.py`

 * *Files identical despite different names*

