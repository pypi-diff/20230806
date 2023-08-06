# Comparing `tmp/cdk-remote-stack-2.0.8.tar.gz` & `tmp/cdk-remote-stack-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-remote-stack/cdk-remote-stack/dist/python/cdk-remote-stack-2.0.8.tar", last modified: Mon Dec 13 00:19:39 2021, max compression
+gzip compressed data, was "cdk-remote-stack-2.0.9.tar", last modified: Fri Jul  8 22:50:33 2022, max compression
```

## Comparing `cdk-remote-stack-2.0.8.tar` & `cdk-remote-stack-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)    10806 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     9854 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      106 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1756 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17592 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      365 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    44517 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/_jsii/cdk-remote-stack@2.0.8.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-12-13 00:19:35.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    10806 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      433 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       92 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       17 2021-12-13 00:19:39.000000 cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10402 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9449 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 22:50:33.502758 cdk-remote-stack-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/src/cdk_remote_stack/
+-rw-r--r--   0 runner    (1001) docker     (121)    17187 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/src/cdk_remote_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44656 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack/_jsii/cdk-remote-stack@2.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 22:50:20.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 22:50:33.506759 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10402 2022-07-08 22:50:32.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-07-08 22:50:33.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 22:50:32.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-08 22:50:33.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-08 22:50:33.000000 cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdk-remote-stack-2.0.8/LICENSE` & `cdk-remote-stack-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-remote-stack-2.0.8/PKG-INFO` & `cdk-remote-stack-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk-remote-stack
-Version: 2.0.8
+Version: 2.0.9
 Summary: Get outputs and AWS SSM parameters from cross-region AWS CloudFormation stacks
 Home-page: https://github.com/pahud/cdk-remote-stack.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-remote-stack.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![npm version](https://badge.fury.io/js/cdk-remote-stack.svg)](https://badge.fury.io/js/cdk-remote-stack)
 [![PyPI version](https://badge.fury.io/py/cdk-remote-stack.svg)](https://badge.fury.io/py/cdk-remote-stack)
 [![release](https://github.com/pahud/cdk-remote-stack/actions/workflows/release.yml/badge.svg)](https://github.com/pahud/cdk-remote-stack/actions/workflows/release.yml)
 
@@ -61,15 +61,14 @@
 
 Let's say we have two cross-regional stacks in the same AWS CDK application:
 
 1. **stackJP** - stack in Japan (`JP`) to create a SNS topic
 2. **stackUS** - stack in United States (`US`) to get the outputs from `stackJP` and print out the SNS `TopicName` from `stackJP` outputs.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import { RemoteOutputs } from 'cdk-remote-stack';
 import * as cdk from 'aws-cdk-lib';
 
 const app = new cdk.App();
 
 const envJP = {
   region: 'ap-northeast-1',
@@ -106,15 +105,14 @@
 ## Always get the latest stack output
 
 By default, the `RemoteOutputs` construct will always try to get the latest output from the source stack. You may opt out by setting `alwaysUpdate` to `false` to turn this feature off.
 
 For example:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 const outputs = new RemoteOutputs(stackUS, 'Outputs', {
   stack: stackJP,
   alwaysUpdate: false,
 })
 ```
 
 # RemoteParameters
@@ -124,15 +122,14 @@
 ## Stacks from single account and different regions
 
 In this sample, we create two stacks from JP (`ap-northeast-1`) and US (`us-west-2`). The JP stack will produce and update parameters in its parameter store, while the US stack will consume the parameters across differnt regions with the `RemoteParameters` construct.
 
 ![](images/remote-param-1.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '111111111111' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
     const parameterPath = `/${envJP.account}/${envJP.region}/${producerStackName}`
@@ -174,15 +171,14 @@
 ## Stacks from differnt accounts and different regions
 
 Similar to the use case above, but now we deploy stacks in separate accounts and regions.  We will need to pass an AWS Identity and Access Management (AWS IAM) `role` to the `RemoteParameters` construct to get all the parameters from the remote environment.
 
 ![](images/remote-param-2.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '222222222222' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
@@ -238,15 +234,14 @@
 This scenario is pretty much like #2. The difference is that there's a dedicated account for centralized configuration store being shared with all other accounts.
 
 ![](images/remote-param-3.svg)
 
 You will need create `RemoteParameters` for all the consuming stacks like:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 // for StackUS
 new RemoteParameters(stackUS, 'Parameters', {
   path: parameterPath,
   region: 'eu-central-1'
   // assume this role for cross-account parameters
   role: iam.Role.fromRoleArn(stackUS, 'readOnlyRole', sharedReadOnlyRoleArn),
 })
```

### Comparing `cdk-remote-stack-2.0.8/README.md` & `cdk-remote-stack-2.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 Let's say we have two cross-regional stacks in the same AWS CDK application:
 
 1. **stackJP** - stack in Japan (`JP`) to create a SNS topic
 2. **stackUS** - stack in United States (`US`) to get the outputs from `stackJP` and print out the SNS `TopicName` from `stackJP` outputs.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import { RemoteOutputs } from 'cdk-remote-stack';
 import * as cdk from 'aws-cdk-lib';
 
 const app = new cdk.App();
 
 const envJP = {
   region: 'ap-northeast-1',
@@ -82,15 +81,14 @@
 ## Always get the latest stack output
 
 By default, the `RemoteOutputs` construct will always try to get the latest output from the source stack. You may opt out by setting `alwaysUpdate` to `false` to turn this feature off.
 
 For example:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 const outputs = new RemoteOutputs(stackUS, 'Outputs', {
   stack: stackJP,
   alwaysUpdate: false,
 })
 ```
 
 # RemoteParameters
@@ -100,15 +98,14 @@
 ## Stacks from single account and different regions
 
 In this sample, we create two stacks from JP (`ap-northeast-1`) and US (`us-west-2`). The JP stack will produce and update parameters in its parameter store, while the US stack will consume the parameters across differnt regions with the `RemoteParameters` construct.
 
 ![](images/remote-param-1.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '111111111111' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
     const parameterPath = `/${envJP.account}/${envJP.region}/${producerStackName}`
@@ -150,15 +147,14 @@
 ## Stacks from differnt accounts and different regions
 
 Similar to the use case above, but now we deploy stacks in separate accounts and regions.  We will need to pass an AWS Identity and Access Management (AWS IAM) `role` to the `RemoteParameters` construct to get all the parameters from the remote environment.
 
 ![](images/remote-param-2.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '222222222222' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
@@ -214,15 +210,14 @@
 This scenario is pretty much like #2. The difference is that there's a dedicated account for centralized configuration store being shared with all other accounts.
 
 ![](images/remote-param-3.svg)
 
 You will need create `RemoteParameters` for all the consuming stacks like:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 // for StackUS
 new RemoteParameters(stackUS, 'Parameters', {
   path: parameterPath,
   region: 'eu-central-1'
   // assume this role for cross-account parameters
   role: iam.Role.fromRoleArn(stackUS, 'readOnlyRole', sharedReadOnlyRoleArn),
 })
```

### Comparing `cdk-remote-stack-2.0.8/setup.py` & `cdk-remote-stack-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-remote-stack",
-    "version": "2.0.8",
+    "version": "2.0.9",
     "description": "Get outputs and AWS SSM parameters from cross-region AWS CloudFormation stacks",
     "license": "Apache-2.0",
     "url": "https://github.com/pahud/cdk-remote-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "Pahud Hsieh<pahudnet@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,36 +22,36 @@
     },
     "packages": [
         "cdk_remote_stack",
         "cdk_remote_stack._jsii"
     ],
     "package_data": {
         "cdk_remote_stack._jsii": [
-            "cdk-remote-stack@2.0.8.jsii.tgz"
+            "cdk-remote-stack@2.0.9.jsii.tgz"
         ],
         "cdk_remote_stack": [
             "py.typed"
         ]
     },
-    "python_requires": ">=3.6",
+    "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.0.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.47.0, <2.0.0",
+        "jsii>=1.61.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-remote-stack-2.0.8/src/cdk_remote_stack/__init__.py` & `cdk-remote-stack-2.0.9/src/cdk_remote_stack/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 
 Let's say we have two cross-regional stacks in the same AWS CDK application:
 
 1. **stackJP** - stack in Japan (`JP`) to create a SNS topic
 2. **stackUS** - stack in United States (`US`) to get the outputs from `stackJP` and print out the SNS `TopicName` from `stackJP` outputs.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import { RemoteOutputs } from 'cdk-remote-stack';
 import * as cdk from 'aws-cdk-lib';
 
 const app = new cdk.App();
 
 const envJP = {
   region: 'ap-northeast-1',
@@ -83,15 +82,14 @@
 ## Always get the latest stack output
 
 By default, the `RemoteOutputs` construct will always try to get the latest output from the source stack. You may opt out by setting `alwaysUpdate` to `false` to turn this feature off.
 
 For example:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 const outputs = new RemoteOutputs(stackUS, 'Outputs', {
   stack: stackJP,
   alwaysUpdate: false,
 })
 ```
 
 # RemoteParameters
@@ -101,15 +99,14 @@
 ## Stacks from single account and different regions
 
 In this sample, we create two stacks from JP (`ap-northeast-1`) and US (`us-west-2`). The JP stack will produce and update parameters in its parameter store, while the US stack will consume the parameters across differnt regions with the `RemoteParameters` construct.
 
 ![](images/remote-param-1.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '111111111111' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
     const parameterPath = `/${envJP.account}/${envJP.region}/${producerStackName}`
@@ -151,15 +148,14 @@
 ## Stacks from differnt accounts and different regions
 
 Similar to the use case above, but now we deploy stacks in separate accounts and regions.  We will need to pass an AWS Identity and Access Management (AWS IAM) `role` to the `RemoteParameters` construct to get all the parameters from the remote environment.
 
 ![](images/remote-param-2.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '222222222222' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
@@ -215,15 +211,14 @@
 This scenario is pretty much like #2. The difference is that there's a dedicated account for centralized configuration store being shared with all other accounts.
 
 ![](images/remote-param-3.svg)
 
 You will need create `RemoteParameters` for all the consuming stacks like:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 // for StackUS
 new RemoteParameters(stackUS, 'Parameters', {
   path: parameterPath,
   region: 'eu-central-1'
   // assume this role for cross-account parameters
   role: iam.Role.fromRoleArn(stackUS, 'readOnlyRole', sharedReadOnlyRoleArn),
 })
```

### Comparing `cdk-remote-stack-2.0.8/src/cdk_remote_stack.egg-info/PKG-INFO` & `cdk-remote-stack-2.0.9/src/cdk_remote_stack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk-remote-stack
-Version: 2.0.8
+Version: 2.0.9
 Summary: Get outputs and AWS SSM parameters from cross-region AWS CloudFormation stacks
 Home-page: https://github.com/pahud/cdk-remote-stack.git
 Author: Pahud Hsieh<pahudnet@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/pahud/cdk-remote-stack.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![npm version](https://badge.fury.io/js/cdk-remote-stack.svg)](https://badge.fury.io/js/cdk-remote-stack)
 [![PyPI version](https://badge.fury.io/py/cdk-remote-stack.svg)](https://badge.fury.io/py/cdk-remote-stack)
 [![release](https://github.com/pahud/cdk-remote-stack/actions/workflows/release.yml/badge.svg)](https://github.com/pahud/cdk-remote-stack/actions/workflows/release.yml)
 
@@ -61,15 +61,14 @@
 
 Let's say we have two cross-regional stacks in the same AWS CDK application:
 
 1. **stackJP** - stack in Japan (`JP`) to create a SNS topic
 2. **stackUS** - stack in United States (`US`) to get the outputs from `stackJP` and print out the SNS `TopicName` from `stackJP` outputs.
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 import { RemoteOutputs } from 'cdk-remote-stack';
 import * as cdk from 'aws-cdk-lib';
 
 const app = new cdk.App();
 
 const envJP = {
   region: 'ap-northeast-1',
@@ -106,15 +105,14 @@
 ## Always get the latest stack output
 
 By default, the `RemoteOutputs` construct will always try to get the latest output from the source stack. You may opt out by setting `alwaysUpdate` to `false` to turn this feature off.
 
 For example:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 const outputs = new RemoteOutputs(stackUS, 'Outputs', {
   stack: stackJP,
   alwaysUpdate: false,
 })
 ```
 
 # RemoteParameters
@@ -124,15 +122,14 @@
 ## Stacks from single account and different regions
 
 In this sample, we create two stacks from JP (`ap-northeast-1`) and US (`us-west-2`). The JP stack will produce and update parameters in its parameter store, while the US stack will consume the parameters across differnt regions with the `RemoteParameters` construct.
 
 ![](images/remote-param-1.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '111111111111' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
     const parameterPath = `/${envJP.account}/${envJP.region}/${producerStackName}`
@@ -174,15 +171,14 @@
 ## Stacks from differnt accounts and different regions
 
 Similar to the use case above, but now we deploy stacks in separate accounts and regions.  We will need to pass an AWS Identity and Access Management (AWS IAM) `role` to the `RemoteParameters` construct to get all the parameters from the remote environment.
 
 ![](images/remote-param-2.svg)
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 
     const envJP = { region: 'ap-northeast-1', account: '111111111111' };
     const envUS = { region: 'us-west-2', account: '222222222222' };
 
     // first stack in JP
     const producerStackName = 'demo-stack-jp';
     const stackJP = new cdk.Stack(app, producerStackName, { env: envJP });
@@ -238,15 +234,14 @@
 This scenario is pretty much like #2. The difference is that there's a dedicated account for centralized configuration store being shared with all other accounts.
 
 ![](images/remote-param-3.svg)
 
 You will need create `RemoteParameters` for all the consuming stacks like:
 
 ```python
-# Example automatically generated from non-compiling source. May contain errors.
 // for StackUS
 new RemoteParameters(stackUS, 'Parameters', {
   path: parameterPath,
   region: 'eu-central-1'
   // assume this role for cross-account parameters
   role: iam.Role.fromRoleArn(stackUS, 'readOnlyRole', sharedReadOnlyRoleArn),
 })
```

