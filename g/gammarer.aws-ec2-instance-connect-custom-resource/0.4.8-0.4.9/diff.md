# Comparing `tmp/gammarer.aws-ec2-instance-connect-custom-resource-0.4.8.tar.gz` & `tmp/gammarer.aws-ec2-instance-connect-custom-resource-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-0.4.8.tar", last modified: Tue Jul 25 17:13:50 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-connect-custom-resource-0.4.9.tar", last modified: Wed Jul 26 17:11:55 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8.tar` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.526291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 17:13:50.526291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:13:50.526291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.522291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.522291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.522291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.526291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16979 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:13:32.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:13:50.522291 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 17:13:50.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 17:13:50.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:13:50.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 17:13:50.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 17:13:50.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:11:43.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:11:55.205553 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-26 17:11:55.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-26 17:11:55.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:11:55.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 17:11:55.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 17:11:55.000000 gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/LICENSE` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 0.4.8
+Version: 0.4.9
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/README.md` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/setup.py` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-connect-custom-resource",
-    "version": "0.4.8",
+    "version": "0.4.9",
     "description": "AWS EC2 instance connect custom resource",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_connect_custom_resource",
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_connect_custom_resource._jsii": [
-            "aws-ec2-instance-connect-custom-resource@0.4.8.jsii.tgz"
+            "aws-ec2-instance-connect-custom-resource@0.4.9.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_connect_custom_resource": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-connect-custom-resource
-Version: 0.4.8
+Version: 0.4.9
 Summary: AWS EC2 instance connect custom resource
 Home-page: https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-connect-custom-resource.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-connect-custom-resource-0.4.8/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-connect-custom-resource-0.4.9/src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_connect_custom_resource.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_connect_custom_resource/__init__.py
 src/gammarer/aws_ec2_instance_connect_custom_resource/py.typed
 src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.8.jsii.tgz
+src/gammarer/aws_ec2_instance_connect_custom_resource/_jsii/aws-ec2-instance-connect-custom-resource@0.4.9.jsii.tgz
```

