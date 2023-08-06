# Comparing `tmp/django-authorization-1.0.2.tar.gz` & `tmp/django-authorization-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-authorization-1.0.2.tar", last modified: Sat Jul  8 14:35:51 2023, max compression
+gzip compressed data, was "django-authorization-1.0.3.tar", last modified: Sun Aug  6 14:12:47 2023, max compression
```

## Comparing `django-authorization-1.0.2.tar` & `django-authorization-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 14:35:14.000000 django-authorization-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-08 14:35:51.782308 django-authorization-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-08 14:35:14.000000 django-authorization-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/_enforcer_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/decorators/_request_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/role.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/management/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.778308 django-authorization-1.0.2/dauthz/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/enforcer_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/middlewares/request_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/dauthz/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-08 14:35:14.000000 django-authorization-1.0.2/dauthz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/django_authorization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-08 14:35:51.000000 django-authorization-1.0.2/django_authorization.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 14:35:14.000000 django-authorization-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 14:35:51.790308 django-authorization-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-08 14:35:14.000000 django-authorization-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:35:51.782308 django-authorization-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-08 14:35:14.000000 django-authorization-1.0.2/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.389695 django-authorization-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 14:12:07.000000 django-authorization-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-06 14:12:47.389695 django-authorization-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-06 14:12:07.000000 django-authorization-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.385695 django-authorization-1.0.3/dauthz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.385695 django-authorization-1.0.3/dauthz/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.385695 django-authorization-1.0.3/dauthz/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/decorators/_enforcer_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/decorators/_request_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.385695 django-authorization-1.0.3/dauthz/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.385695 django-authorization-1.0.3/dauthz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/commands/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/commands/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/management/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.389695 django-authorization-1.0.3/dauthz/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/middlewares/enforcer_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/middlewares/request_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.389695 django-authorization-1.0.3/dauthz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-06 14:12:07.000000 django-authorization-1.0.3/dauthz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.389695 django-authorization-1.0.3/django_authorization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-08-06 14:12:47.000000 django-authorization-1.0.3/django_authorization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-06 14:12:47.000000 django-authorization-1.0.3/django_authorization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:12:47.000000 django-authorization-1.0.3/django_authorization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 14:12:47.000000 django-authorization-1.0.3/django_authorization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 14:12:47.000000 django-authorization-1.0.3/django_authorization.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-06 14:12:07.000000 django-authorization-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-06 14:12:47.389695 django-authorization-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-06 14:12:07.000000 django-authorization-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:12:47.389695 django-authorization-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-06 14:12:07.000000 django-authorization-1.0.3/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-06 14:12:07.000000 django-authorization-1.0.3/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-06 14:12:07.000000 django-authorization-1.0.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-06 14:12:07.000000 django-authorization-1.0.3/tests/test_middleware.py
```

### Comparing `django-authorization-1.0.2/LICENSE` & `django-authorization-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/PKG-INFO` & `django-authorization-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.0.2
+Version: 1.0.3
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Home-page: https://github.com/pycasbin/django-authorization
 Author: JonLee
 Author-email: leeqvip@gmail.com
 License: Apache 2.0
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
@@ -92,15 +92,15 @@
 
 to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
 
 ## Usage
 
 ### Some Important Concepts:
 
-such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
+such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.org/)
 
 ### Middleware Usage
 
 ```python
 # Install middleware for django-authorization as required
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
```

### Comparing `django-authorization-1.0.2/README.md` & `django-authorization-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
 
 ## Usage
 
 ### Some Important Concepts:
 
-such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
+such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.org/)
 
 ### Middleware Usage
 
 ```python
 # Install middleware for django-authorization as required
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
```

### Comparing `django-authorization-1.0.2/dauthz/core.py` & `django-authorization-1.0.3/dauthz/core.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/management/commands/group.py` & `django-authorization-1.0.3/dauthz/management/commands/group.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/management/commands/policy.py` & `django-authorization-1.0.3/dauthz/management/commands/policy.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/management/commands/role.py` & `django-authorization-1.0.3/dauthz/management/commands/role.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/middlewares/enforcer_middleware.py` & `django-authorization-1.0.3/dauthz/middlewares/enforcer_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/middlewares/request_middleware.py` & `django-authorization-1.0.3/dauthz/middlewares/request_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/dauthz/settings.py` & `django-authorization-1.0.3/dauthz/settings.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/django_authorization.egg-info/PKG-INFO` & `django-authorization-1.0.3/django_authorization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.0.2
+Version: 1.0.3
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Home-page: https://github.com/pycasbin/django-authorization
 Author: JonLee
 Author-email: leeqvip@gmail.com
 License: Apache 2.0
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
@@ -92,15 +92,15 @@
 
 to better prompt the configure method of django-authorization, we made a django-app based on django-authorization, you can see it in [django-authorization-example](https://github.com/pycasbin/django-authorization-example)
 
 ## Usage
 
 ### Some Important Concepts:
 
-such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.io/)
+such as .conf file, policy, sub, obj, act, please refer to the [casbin website](https://casbin.org/)
 
 ### Middleware Usage
 
 ```python
 # Install middleware for django-authorization as required
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
```

### Comparing `django-authorization-1.0.2/django_authorization.egg-info/SOURCES.txt` & `django-authorization-1.0.3/django_authorization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/setup.py` & `django-authorization-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/tests/test_basic.py` & `django-authorization-1.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/tests/test_command.py` & `django-authorization-1.0.3/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/tests/test_decorator.py` & `django-authorization-1.0.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.0.2/tests/test_middleware.py` & `django-authorization-1.0.3/tests/test_middleware.py`

 * *Files identical despite different names*

