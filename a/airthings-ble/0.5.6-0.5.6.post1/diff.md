# Comparing `tmp/airthings_ble-0.5.6.tar.gz` & `tmp/airthings_ble-0.5.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings_ble-0.5.6.tar", max compression
+gzip compressed data, was "airthings_ble-0.5.6.post1.tar", max compression
```

## Comparing `airthings_ble-0.5.6.tar` & `airthings_ble-0.5.6.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/LICENSE
--rw-r--r--   0        0        0      113 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/README.md
--rw-r--r--   0        0        0      235 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/__init__.py
--rw-r--r--   0        0        0     2109 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/const.py
--rw-r--r--   0        0        0    20993 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/parser.py
--rw-r--r--   0        0        0        0 2023-08-06 13:20:23.024188 airthings_ble-0.5.6/airthings_ble/py.typed
--rw-r--r--   0        0        0     2159 2023-08-06 13:20:24.792241 airthings_ble-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1249 1970-01-01 00:00:00.000000 airthings_ble-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/LICENSE
+-rw-r--r--   0        0        0      113 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/README.md
+-rw-r--r--   0        0        0      235 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/airthings_ble/__init__.py
+-rw-r--r--   0        0        0     2109 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/airthings_ble/const.py
+-rw-r--r--   0        0        0    20993 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/airthings_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:24:17.067602 airthings_ble-0.5.6.post1/airthings_ble/py.typed
+-rw-r--r--   0        0        0     2161 2023-08-06 13:24:18.691579 airthings_ble-0.5.6.post1/pyproject.toml
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 airthings_ble-0.5.6.post1/PKG-INFO
```

### Comparing `airthings_ble-0.5.6/LICENSE` & `airthings_ble-0.5.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6/airthings_ble/const.py` & `airthings_ble-0.5.6.post1/airthings_ble/const.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6/airthings_ble/parser.py` & `airthings_ble-0.5.6.post1/airthings_ble/parser.py`

 * *Files identical despite different names*

### Comparing `airthings_ble-0.5.6/pyproject.toml` & `airthings_ble-0.5.6.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airthings-ble"
-version = "v0.5.6"
+version = "v0.5.6-1"
 description = "Manage Airthings BLE devices"
 authors = ["Vincent Giorgi"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/vincegio/airthings-ble"
 documentation = "https://airthings-ble.readthedocs.io"
 classifiers = [
```

### Comparing `airthings_ble-0.5.6/PKG-INFO` & `airthings_ble-0.5.6.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airthings-ble
-Version: 0.5.6
+Version: 0.5.6.post1
 Summary: Manage Airthings BLE devices
 Home-page: https://github.com/vincegio/airthings-ble
 License: Apache Software License 2.0
 Author: Vincent Giorgi
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

