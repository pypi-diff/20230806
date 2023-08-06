# Comparing `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.7.tar.gz` & `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.7.tar", last modified: Sun Jul 23 19:18:57 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.9.tar", last modified: Tue Jul 25 19:18:34 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7.tar` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.475307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.475307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20664 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:18:40.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:57.479307 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-23 19:18:57.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-23 19:18:57.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:18:57.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 19:18:57.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 19:18:57.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.794659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.794659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20662 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:18:23.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:34.798659 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-25 19:18:34.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-25 19:18:34.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:18:34.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 19:18:34.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:18:34.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/LICENSE` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.7
+Version: 0.4.9
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/README.md` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/setup.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-running-scheduler",
-    "version": "0.4.7",
+    "version": "0.4.9",
     "description": "AWS EC2 Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_running_scheduler",
         "gammarer.aws_ec2_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_running_scheduler._jsii": [
-            "aws-ec2-instance-running-scheduler@0.4.7.jsii.tgz"
+            "aws-ec2-instance-running-scheduler@0.4.9.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.7
+Version: 0.4.9
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.7/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-running-scheduler-0.4.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
 src/gammarer/aws_ec2_instance_running_scheduler/py.typed
 src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.7.jsii.tgz
+src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.9.jsii.tgz
```

