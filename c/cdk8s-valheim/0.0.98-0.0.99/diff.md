# Comparing `tmp/cdk8s-valheim-0.0.98.tar.gz` & `tmp/cdk8s-valheim-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-valheim-0.0.98.tar", last modified: Tue Jun 27 00:21:31 2023, max compression
+gzip compressed data, was "cdk8s-valheim-0.0.99.tar", last modified: Wed Jun 28 00:21:24 2023, max compression
```

## Comparing `cdk8s-valheim-0.0.98.tar` & `cdk8s-valheim-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:21:31.028225 cdk8s-valheim-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-27 00:21:31.024225 cdk8s-valheim-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 00:21:31.028225 cdk8s-valheim-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:21:31.024225 cdk8s-valheim-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:21:31.024225 cdk8s-valheim-0.0.98/src/cdk8s_valheim/
--rw-r--r--   0 runner    (1001) docker     (123)    74269 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:21:31.024225 cdk8s-valheim-0.0.98/src/cdk8s_valheim/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35321 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim/_jsii/cdk8s-valheim@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:21:19.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:21:31.024225 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-27 00:21:30.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 00:21:31.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:21:30.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-27 00:21:30.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 00:21:30.000000 cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/src/cdk8s_valheim/
+-rw-r--r--   0 runner    (1001) docker     (123)    74269 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/src/cdk8s_valheim/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35323 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim/_jsii/cdk8s-valheim@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 00:21:10.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 00:21:24.826461 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-28 00:21:24.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-28 00:21:24.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 00:21:24.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-28 00:21:24.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 00:21:24.000000 cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/top_level.txt
```

### Comparing `cdk8s-valheim-0.0.98/LICENSE` & `cdk8s-valheim-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.98/PKG-INFO` & `cdk8s-valheim-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-valheim
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends a Valheim server chart.
 Home-page: https://github.com/awlsring/cdk8s-valheim.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk8s-valheim.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-valheim-0.0.98/README.md` & `cdk8s-valheim-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.98/setup.py` & `cdk8s-valheim-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-valheim",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "A package that vends a Valheim server chart.",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdk8s-valheim.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_valheim",
         "cdk8s_valheim._jsii"
     ],
     "package_data": {
         "cdk8s_valheim._jsii": [
-            "cdk8s-valheim@0.0.98.jsii.tgz"
+            "cdk8s-valheim@0.0.99.jsii.tgz"
         ],
         "cdk8s_valheim": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-valheim-0.0.98/src/cdk8s_valheim/__init__.py` & `cdk8s-valheim-0.0.99/src/cdk8s_valheim/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-valheim-0.0.98/src/cdk8s_valheim.egg-info/PKG-INFO` & `cdk8s-valheim-0.0.99/src/cdk8s_valheim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-valheim
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends a Valheim server chart.
 Home-page: https://github.com/awlsring/cdk8s-valheim.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk8s-valheim.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

