# Comparing `tmp/gammarer.aws-rds-database-running-scheduler-0.3.8.tar.gz` & `tmp/gammarer.aws-rds-database-running-scheduler-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-rds-database-running-scheduler-0.3.8.tar", last modified: Wed Jul 19 19:15:59 2023, max compression
+gzip compressed data, was "gammarer.aws-rds-database-running-scheduler-0.3.9.tar", last modified: Thu Jul 20 19:15:20 2023, max compression
```

## Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8.tar` & `gammarer.aws-rds-database-running-scheduler-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.335280 gammarer.aws-rds-database-running-scheduler-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-19 19:15:59.335280 gammarer.aws-rds-database-running-scheduler-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 19:15:59.335280 gammarer.aws-rds-database-running-scheduler-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.331280 gammarer.aws-rds-database-running-scheduler-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.331280 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.331280 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.331280 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22265 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 19:15:47.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 19:15:59.331280 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-19 19:15:59.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-19 19:15:59.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 19:15:59.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-19 19:15:59.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 19:15:59.000000 gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.195902 gammarer.aws-rds-database-running-scheduler-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.195902 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22262 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:15:07.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:15:20.199902 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-20 19:15:20.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-20 19:15:20.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:15:20.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 19:15:20.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 19:15:20.000000 gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/LICENSE` & `gammarer.aws-rds-database-running-scheduler-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/PKG-INFO` & `gammarer.aws-rds-database-running-scheduler-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-rds-database-running-scheduler
-Version: 0.3.8
+Version: 0.3.9
 Summary: AWS RDS Database Running Scheduler
 Home-page: https://github.com/yicr/aws-rds-database-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-rds-database-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/README.md` & `gammarer.aws-rds-database-running-scheduler-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/setup.py` & `gammarer.aws-rds-database-running-scheduler-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-rds-database-running-scheduler",
-    "version": "0.3.8",
+    "version": "0.3.9",
     "description": "AWS RDS Database Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-rds-database-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_rds_database_running_scheduler",
         "gammarer.aws_rds_database_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_rds_database_running_scheduler._jsii": [
-            "aws-rds-database-running-scheduler@0.3.8.jsii.tgz"
+            "aws-rds-database-running-scheduler@0.3.9.jsii.tgz"
         ],
         "gammarer.aws_rds_database_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer/aws_rds_database_running_scheduler/__init__.py` & `gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer/aws_rds_database_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-rds-database-running-scheduler
-Version: 0.3.8
+Version: 0.3.9
 Summary: AWS RDS Database Running Scheduler
 Home-page: https://github.com/yicr/aws-rds-database-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-rds-database-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-rds-database-running-scheduler-0.3.8/src/gammarer.aws_rds_database_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-rds-database-running-scheduler-0.3.9/src/gammarer.aws_rds_database_running_scheduler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_rds_database_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_rds_database_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_rds_database_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_rds_database_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_rds_database_running_scheduler/__init__.py
 src/gammarer/aws_rds_database_running_scheduler/py.typed
 src/gammarer/aws_rds_database_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.8.jsii.tgz
+src/gammarer/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.9.jsii.tgz
```

