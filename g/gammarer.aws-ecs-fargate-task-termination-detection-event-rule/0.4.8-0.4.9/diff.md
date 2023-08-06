# Comparing `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8.tar.gz` & `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8.tar", last modified: Fri Jul 28 18:22:50 2023, max compression
+gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9.tar", last modified: Sat Jul 29 18:22:52 2023, max compression
```

## Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8.tar` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.270611 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.270611 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:22:36.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:50.274612 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-28 18:22:50.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-28 18:22:50.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:22:50.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 18:22:50.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:22:50.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.748139 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.748139 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:22:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:22:52.752140 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-29 18:22:52.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-29 18:22:52.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:22:52.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-29 18:22:52.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 18:22:52.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/LICENSE` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.8
+Version: 0.4.9
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/README.md` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/setup.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ecs-fargate-task-termination-detection-event-rule",
-    "version": "0.4.8",
+    "version": "0.4.9",
     "description": "This an AWS ECS Fargate task termination detection Event Rule.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule",
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii"
     ],
     "package_data": {
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii": [
-            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.8.jsii.tgz"
+            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.9.jsii.tgz"
         ],
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.8
+Version: 0.4.9
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.8/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.9/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
-src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.8.jsii.tgz
+src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.9.jsii.tgz
```

