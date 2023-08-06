# Comparing `tmp/cdk-aws-discord-notifiers-0.0.98.tar.gz` & `tmp/cdk-aws-discord-notifiers-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-aws-discord-notifiers-0.0.98.tar", last modified: Sun Jun 18 00:09:45 2023, max compression
+gzip compressed data, was "cdk-aws-discord-notifiers-0.0.99.tar", last modified: Mon Jun 19 00:10:13 2023, max compression
```

## Comparing `cdk-aws-discord-notifiers-0.0.98.tar` & `cdk-aws-discord-notifiers-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 00:09:45.088244 cdk-aws-discord-notifiers-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-18 00:09:45.088244 cdk-aws-discord-notifiers-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 00:09:45.088244 cdk-aws-discord-notifiers-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 00:09:45.084244 cdk-aws-discord-notifiers-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 00:09:45.084244 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 00:09:45.084244 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2509688 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 00:09:22.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 00:09:45.088244 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-18 00:09:45.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-18 00:09:45.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 00:09:45.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-18 00:09:45.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 00:09:45.000000 cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:10:13.565571 cdk-aws-discord-notifiers-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-19 00:10:13.565571 cdk-aws-discord-notifiers-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 00:10:13.565571 cdk-aws-discord-notifiers-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:10:13.561571 cdk-aws-discord-notifiers-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:10:13.561571 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:10:13.561571 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2509680 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:09:54.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:10:13.565571 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-19 00:10:13.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-19 00:10:13.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:10:13.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 00:10:13.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 00:10:13.000000 cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

### Comparing `cdk-aws-discord-notifiers-0.0.98/LICENSE` & `cdk-aws-discord-notifiers-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.98/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.98/README.md` & `cdk-aws-discord-notifiers-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.98/setup.py` & `cdk-aws-discord-notifiers-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-aws-discord-notifiers",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "A package that vends constructs to notify about AWS resources via discord",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdk-aws-discord-notifiers.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_aws-discord-notifiers",
         "cdk_aws-discord-notifiers._jsii"
     ],
     "package_data": {
         "cdk_aws-discord-notifiers._jsii": [
-            "cdk-aws-discord-notifiers@0.0.98.jsii.tgz"
+            "cdk-aws-discord-notifiers@0.0.99.jsii.tgz"
         ],
         "cdk_aws-discord-notifiers": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-aws-discord-notifiers-0.0.98/src/cdk_aws-discord-notifiers/__init__.py` & `cdk-aws-discord-notifiers-0.0.99/src/cdk_aws-discord-notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.98
+Version: 0.0.99
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.98/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt` & `cdk-aws-discord-notifiers-0.0.99/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/cdk_aws-discord-notifiers/__init__.py
 src/cdk_aws-discord-notifiers/py.typed
 src/cdk_aws-discord-notifiers/_jsii/__init__.py
-src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.98.jsii.tgz
+src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.99.jsii.tgz
 src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
 src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
 src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
 src/cdk_aws_discord_notifiers.egg-info/requires.txt
 src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

