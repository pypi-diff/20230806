# Comparing `tmp/usermgr-0.2.0.tar.gz` & `tmp/usermgr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usermgr-0.2.0.tar", max compression
+gzip compressed data, was "usermgr-0.2.1.tar", max compression
```

## Comparing `usermgr-0.2.0.tar` & `usermgr-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.2.0/LICENSE
--rw-r--r--   0        0        0      407 2023-07-31 06:05:17.779124 usermgr-0.2.0/README.md
--rw-r--r--   0        0        0      607 2023-08-04 03:57:13.879824 usermgr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      335 2023-08-02 17:01:51.661912 usermgr-0.2.0/usermgr/Factory.py
--rw-r--r--   0        0        0       22 2023-08-04 03:56:14.259827 usermgr-0.2.0/usermgr/__init__.py
--rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.2.0/usermgr/base.py
--rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.2.0/usermgr/providers/__init__.py
--rw-r--r--   0        0        0     3656 2023-07-31 05:54:04.809152 usermgr-0.2.0/usermgr/providers/cognito.py
--rw-r--r--   0        0        0     2125 2023-08-04 03:49:19.409848 usermgr-0.2.0/usermgr/providers/lambda.py
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 usermgr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.2.1/LICENSE
+-rw-r--r--   0        0        0      407 2023-07-31 06:05:17.779124 usermgr-0.2.1/README.md
+-rw-r--r--   0        0        0      625 2023-08-05 07:38:10.752752 usermgr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-08-05 07:34:57.291085 usermgr-0.2.1/usermgr/Factory.py
+-rw-r--r--   0        0        0       22 2023-08-05 07:38:17.176918 usermgr-0.2.1/usermgr/__init__.py
+-rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.2.1/usermgr/base.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.2.1/usermgr/providers/__init__.py
+-rw-r--r--   0        0        0     3652 2023-08-05 07:35:21.644418 usermgr-0.2.1/usermgr/providers/cognito.py
+-rw-r--r--   0        0        0     2111 2023-08-05 07:32:26.426097 usermgr-0.2.1/usermgr/providers/lambda.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 usermgr-0.2.1/PKG-INFO
```

### Comparing `usermgr-0.2.0/LICENSE` & `usermgr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `usermgr-0.2.0/pyproject.toml` & `usermgr-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usermgr"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["tamuto <tamuto@infodb.jp>"]
 readme = "README.md"
 homepage = "https://github.com/tamuto/usermgr"
 repository = "https://github.com/tamuto/usermgr"
 
 packages = [
@@ -17,11 +17,12 @@
 
 [tool.poetry.extras]
 cognito = ["boto3"]
 lambda = ["boto3"]
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = {extras = ["cli"], version = "^0.21.1"}
+flake8 = "^6.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `usermgr-0.2.0/usermgr/base.py` & `usermgr-0.2.1/usermgr/base.py`

 * *Files identical despite different names*

### Comparing `usermgr-0.2.0/usermgr/providers/cognito.py` & `usermgr-0.2.1/usermgr/providers/cognito.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             digestmod=hashlib.sha256).digest()).decode()
 
     def add_user(self, username, password, attrs):
         response = self.idp.admin_create_user(
             UserPoolId=self.user_pool_id,
             Username=username,
             TemporaryPassword=password,
-            UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
+            UserAttributes=[{"Name": k, "Value": v} for k, v in attrs.items()],
             MessageAction="SUPPRESS"
         )
         sub_id = [d['Value'] for d in response['User']['Attributes'] if d['Name'] == 'sub'][0]
 
         response = self.idp.admin_initiate_auth(
             UserPoolId=self.user_pool_id,
             ClientId=self.client_id,
@@ -65,15 +65,15 @@
         )
         return sub_id
 
     def update_user(self, username, attrs):
         self.idp.admin_update_user_attributes(
             UserPoolId=self.user_pool_id,
             Username=username,
-            UserAttributes=[{ "Name": k, "Value": v } for k, v in attrs.items()],
+            UserAttributes=[{"Name": k, "Value": v} for k, v in attrs.items()],
         )
 
     def set_password(self, username, password, permanent=False):
         self.idp.admin_set_user_password(
             UserPoolId=self.user_pool_id,
             Username=username,
             Password=password,
```

### Comparing `usermgr-0.2.0/usermgr/providers/lambda.py` & `usermgr-0.2.1/usermgr/providers/lambda.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import boto3
 import json
-import base64
 
 from ..base import UserManager
 
 
 def new_instance(**kwargs):
     return LambdaUserMgr(**kwargs)
```

### Comparing `usermgr-0.2.0/PKG-INFO` & `usermgr-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usermgr
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Home-page: https://github.com/tamuto/usermgr
 Author: tamuto
 Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

