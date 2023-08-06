# Comparing `tmp/durkinza.cdk-networkfirewall-l2-0.0.4.tar.gz` & `tmp/durkinza.cdk-networkfirewall-l2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.4.tar", last modified: Sun Jul 30 18:41:55 2023, max compression
+gzip compressed data, was "durkinza.cdk-networkfirewall-l2-0.0.5.tar", last modified: Sun Aug  6 21:17:30 2023, max compression
```

## Comparing `durkinza.cdk-networkfirewall-l2-0.0.4.tar` & `durkinza.cdk-networkfirewall-l2-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/
--rw-r--r--   0 runner    (1001) docker     (123)   217751 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102134 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:41:43.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 18:41:55.243554 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-30 18:41:55.000000 durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.818765 durkinza.cdk-networkfirewall-l2-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:17:30.818765 durkinza.cdk-networkfirewall-l2-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/
+-rw-r--r--   0 runner    (1001) docker     (123)   217751 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102125 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:17:17.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:17:30.814765 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-08-06 21:17:30.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-06 21:17:30.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:17:30.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-06 21:17:30.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 21:17:30.000000 durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/LICENSE` & `durkinza.cdk-networkfirewall-l2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/README.md` & `durkinza.cdk-networkfirewall-l2-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/setup.py` & `durkinza.cdk-networkfirewall-l2-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "durkinza.cdk-networkfirewall-l2",
-    "version": "0.0.4",
+    "version": "0.0.5",
     "description": "Experimental L2 constructs for the aws-networkfirewall",
     "license": "Apache-2.0",
     "url": "https://github.com/durkinza/cdk-networkfirewall-l2#readme",
     "long_description_content_type": "text/markdown",
     "author": "durkinza<8985088+durkinza@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "durkinza.cdk_networkfirewall_l2",
         "durkinza.cdk_networkfirewall_l2._jsii"
     ],
     "package_data": {
         "durkinza.cdk_networkfirewall_l2._jsii": [
-            "cdk-networkfirewall-l2@0.0.4.jsii.tgz"
+            "cdk-networkfirewall-l2@0.0.5.jsii.tgz"
         ],
         "durkinza.cdk_networkfirewall_l2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.79.0, <3.0.0",
+        "aws-cdk-lib>=2.90.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.85.0, <2.0.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza/cdk_networkfirewall_l2/__init__.py` & `durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza/cdk_networkfirewall_l2/__init__.py`

 * *Files identical despite different names*

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO` & `durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkinza.cdk-networkfirewall-l2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Experimental L2 constructs for the aws-networkfirewall
 Home-page: https://github.com/durkinza/cdk-networkfirewall-l2#readme
 Author: durkinza<8985088+durkinza@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/durkinza/cdk-networkfirewall-l2.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `durkinza.cdk-networkfirewall-l2-0.0.4/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt` & `durkinza.cdk-networkfirewall-l2-0.0.5/src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/durkinza.cdk_networkfirewall_l2.egg-info/SOURCES.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/dependency_links.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/requires.txt
 src/durkinza.cdk_networkfirewall_l2.egg-info/top_level.txt
 src/durkinza/cdk_networkfirewall_l2/__init__.py
 src/durkinza/cdk_networkfirewall_l2/py.typed
 src/durkinza/cdk_networkfirewall_l2/_jsii/__init__.py
-src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.4.jsii.tgz
+src/durkinza/cdk_networkfirewall_l2/_jsii/cdk-networkfirewall-l2@0.0.5.jsii.tgz
```

