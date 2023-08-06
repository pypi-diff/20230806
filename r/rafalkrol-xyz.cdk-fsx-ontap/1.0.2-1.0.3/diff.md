# Comparing `tmp/rafalkrol-xyz.cdk-fsx-ontap-1.0.2.tar.gz` & `tmp/rafalkrol-xyz.cdk-fsx-ontap-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rafalkrol-xyz.cdk-fsx-ontap-1.0.2.tar", last modified: Wed Aug  2 09:51:28 2023, max compression
+gzip compressed data, was "rafalkrol-xyz.cdk-fsx-ontap-1.0.3.tar", last modified: Sun Aug  6 19:12:44 2023, max compression
```

## Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2.tar` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.443618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.443618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1218237 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:51:15.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:28.447618 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 09:51:28.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 09:51:28.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:51:28.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 09:51:28.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 09:51:28.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.340111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:12:44.340111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1218235 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:12:33.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:12:44.336111 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-06 19:12:44.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-06 19:12:44.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:12:44.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-06 19:12:44.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 19:12:44.000000 rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/top_level.txt
```

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/LICENSE` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/PKG-INFO` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafalkrol-xyz.cdk-fsx-ontap
-Version: 1.0.2
+Version: 1.0.3
 Summary: CDK construct for Amazon FSx for Netapp ONTAP
 Home-page: https://rafalkrol.xyz
 Author: Rafal Krol<ameotoko1+github@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rafalkrol-xyz/cdk-fsx-ontap
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/README.md` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/setup.py` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "rafalkrol-xyz.cdk-fsx-ontap",
-    "version": "1.0.2",
+    "version": "1.0.3",
     "description": "CDK construct for Amazon FSx for Netapp ONTAP",
     "license": "MIT",
     "url": "https://rafalkrol.xyz",
     "long_description_content_type": "text/markdown",
     "author": "Rafal Krol<ameotoko1+github@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "rafalkrol-xyz.cdk_fsx_ontap",
         "rafalkrol-xyz.cdk_fsx_ontap._jsii"
     ],
     "package_data": {
         "rafalkrol-xyz.cdk_fsx_ontap._jsii": [
-            "cdk-fsx-ontap@1.0.2.jsii.tgz"
+            "cdk-fsx-ontap@1.0.3.jsii.tgz"
         ],
         "rafalkrol-xyz.cdk_fsx_ontap": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.85.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.86.0, <2.0.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol-xyz/cdk_fsx_ontap/__init__.py` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol-xyz/cdk_fsx_ontap/__init__.py`

 * *Files identical despite different names*

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/PKG-INFO` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rafalkrol-xyz.cdk-fsx-ontap
-Version: 1.0.2
+Version: 1.0.3
 Summary: CDK construct for Amazon FSx for Netapp ONTAP
 Home-page: https://rafalkrol.xyz
 Author: Rafal Krol<ameotoko1+github@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/rafalkrol-xyz/cdk-fsx-ontap
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rafalkrol-xyz.cdk-fsx-ontap-1.0.2/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/SOURCES.txt` & `rafalkrol-xyz.cdk-fsx-ontap-1.0.3/src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/rafalkrol-xyz/cdk_fsx_ontap/__init__.py
 src/rafalkrol-xyz/cdk_fsx_ontap/py.typed
 src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/__init__.py
-src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.2.jsii.tgz
+src/rafalkrol-xyz/cdk_fsx_ontap/_jsii/cdk-fsx-ontap@1.0.3.jsii.tgz
 src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/PKG-INFO
 src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/SOURCES.txt
 src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/dependency_links.txt
 src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/requires.txt
 src/rafalkrol_xyz.cdk_fsx_ontap.egg-info/top_level.txt
```

