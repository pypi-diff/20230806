# Comparing `tmp/tai_aws_account_bootstrap-0.0.0.tar.gz` & `tmp/tai_aws_account_bootstrap-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tai_aws_account_bootstrap-0.0.0.tar", max compression
+gzip compressed data, was "tai_aws_account_bootstrap-0.0.1.tar", max compression
```

## Comparing `tai_aws_account_bootstrap-0.0.0.tar` & `tai_aws_account_bootstrap-0.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      150 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/README.md
--rw-r--r--   0        0        0        0 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/accountbootstrap/__init__.py
--rw-r--r--   0        0        0      866 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/accountbootstrap/base_stack.py
--rw-r--r--   0        0        0     2589 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/accountbootstrap/bootstrap_stack.py
--rw-r--r--   0        0        0     7396 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/accountbootstrap/stack_config_models.py
--rw-r--r--   0        0        0     2278 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.0/accountbootstrap/stack_helpers.py
--rw-r--r--   0        0        0      841 2023-08-06 12:39:42.361341 tai_aws_account_bootstrap-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 tai_aws_account_bootstrap-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      150 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.1/README.md
+-rw-r--r--   0        0        0      850 2023-08-06 13:14:42.120957 tai_aws_account_bootstrap-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/__init__.py
+-rw-r--r--   0        0        0      875 2023-08-06 13:13:16.716897 tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/base_stack.py
+-rw-r--r--   0        0        0     2607 2023-08-06 13:13:23.053198 tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/bootstrap_stack.py
+-rw-r--r--   0        0        0     7396 2023-08-06 03:26:04.307705 tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/stack_config_models.py
+-rw-r--r--   0        0        0     2287 2023-08-06 13:13:27.733421 tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/stack_helpers.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 tai_aws_account_bootstrap-0.0.1/PKG-INFO
```

### Comparing `tai_aws_account_bootstrap-0.0.0/accountbootstrap/base_stack.py` & `tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/base_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Define a base stack that provides some nice usability features."""
 from constructs import Construct
 from aws_cdk import (
     Stack,
 )
-from accountbootstrap.stack_config_models import (
+from tai_aws_account_bootstrap.stack_config_models import (
     StackConfigBaseModel,
 )
 
 class BaseStack(Stack):
     """Define the stack for the TAI API service."""
 
     def __init__(
```

### Comparing `tai_aws_account_bootstrap-0.0.0/accountbootstrap/bootstrap_stack.py` & `tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/bootstrap_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define a bootstrap stack to bootstrap an AWS account."""
 from constructs import Construct
 from aws_cdk import (
     aws_ec2 as ec2,
 )
-from accountbootstrap.base_stack import BaseStack
-from accountbootstrap.stack_config_models import (
+from tai_aws_account_bootstrap.base_stack import BaseStack
+from tai_aws_account_bootstrap.stack_config_models import (
     StackConfigBaseModel,
 )
 
 
 class BootstrapStack(BaseStack):
     """Define the stack for bootstrapping an AWS account."""
```

### Comparing `tai_aws_account_bootstrap-0.0.0/accountbootstrap/stack_config_models.py` & `tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/stack_config_models.py`

 * *Files identical despite different names*

### Comparing `tai_aws_account_bootstrap-0.0.0/accountbootstrap/stack_helpers.py` & `tai_aws_account_bootstrap-0.0.1/tai_aws_account_bootstrap/stack_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define helpers for CDK stacks."""
 from aws_cdk import (
     Tags,
 )
 import boto3
 from constructs import Construct
-from accountbootstrap.stack_config_models import (
+from tai_aws_account_bootstrap.stack_config_models import (
     AWSDeploymentSettings,
 )
 
 
 def add_tags(scope: Construct, tags: dict):
     """Add tags to a CDK stack.
```

### Comparing `tai_aws_account_bootstrap-0.0.0/pyproject.toml` & `tai_aws_account_bootstrap-0.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 authors = [ "Jacob Petterle" ]
 description = "Bootstraps a new AWS account with a baseline set of resources"
 homepage = "https://github.com/tai-team-ai/tai-aws-account-bootstrap"
 license = "MIT"
 name = "tai-aws-account-bootstrap"
 readme = "README.md"
 repository = "https://github.com/tai-team-ai/tai-aws-account-bootstrap"
-version = "0.0.0"
+version = "0.0.1"
 
   [[tool.poetry.packages]]
-  include = "accountbootstrap"
+  include = "tai_aws_account_bootstrap"
 
   [tool.poetry.dependencies]
   pygit2 = "*"
   boto3 = "*"
   poetry = "*"
 
     [tool.poetry.dependencies.pydantic]
```

### Comparing `tai_aws_account_bootstrap-0.0.0/PKG-INFO` & `tai_aws_account_bootstrap-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tai-aws-account-bootstrap
-Version: 0.0.0
+Version: 0.0.1
 Summary: Bootstraps a new AWS account with a baseline set of resources
 Home-page: https://github.com/tai-team-ai/tai-aws-account-bootstrap
 License: MIT
 Author: Jacob Petterle
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

