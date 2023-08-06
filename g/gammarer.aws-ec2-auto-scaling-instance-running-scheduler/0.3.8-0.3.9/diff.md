# Comparing `tmp/gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8.tar.gz` & `tmp/gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8.tar", last modified: Tue Jul 25 19:15:49 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9.tar", last modified: Wed Jul 26 19:16:10 2023, max compression
```

## Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8.tar` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.342606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:15:49.342606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.3.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:15:33.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:15:49.338606 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-25 19:15:49.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 19:15:49.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:15:49.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 19:15:49.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:15:49.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.937981 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-26 19:16:10.937981 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:16:10.937981 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.933982 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.933982 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.933982 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.937981 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20738 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.3.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:15:57.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:16:10.933982 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-26 19:16:10.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 19:16:10.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:16:10.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 19:16:10.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 19:16:10.000000 gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/LICENSE` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/PKG-INFO` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-auto-scaling-instance-running-scheduler
-Version: 0.3.8
+Version: 0.3.9
 Summary: AWS EC2 AutoScaling Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/README.md` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/setup.py` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-auto-scaling-instance-running-scheduler",
-    "version": "0.3.8",
+    "version": "0.3.9",
     "description": "AWS EC2 AutoScaling Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_auto_scaling_instance_running_scheduler",
         "gammarer.aws_ec2_auto_scaling_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_auto_scaling_instance_running_scheduler._jsii": [
-            "aws-ec2-auto-scaling-instance-running-scheduler@0.3.8.jsii.tgz"
+            "aws-ec2-auto-scaling-instance-running-scheduler@0.3.9.jsii.tgz"
         ],
         "gammarer.aws_ec2_auto_scaling_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-auto-scaling-instance-running-scheduler
-Version: 0.3.8
+Version: 0.3.9
 Summary: AWS EC2 AutoScaling Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-auto-scaling-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.8/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-ec2-auto-scaling-instance-running-scheduler-0.3.9/src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_ec2_auto_scaling_instance_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/__init__.py
 src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/py.typed
 src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.3.8.jsii.tgz
+src/gammarer/aws_ec2_auto_scaling_instance_running_scheduler/_jsii/aws-ec2-auto-scaling-instance-running-scheduler@0.3.9.jsii.tgz
```

