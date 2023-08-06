# Comparing `tmp/eniris-0.7.2.tar.gz` & `tmp/eniris-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.7.2.tar", last modified: Sun Aug  6 16:14:35 2023, max compression
+gzip compressed data, was "eniris-0.7.3.tar", last modified: Sun Aug  6 17:14:39 2023, max compression
```

## Comparing `eniris-0.7.2.tar` & `eniris-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.084597 eniris-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 16:14:20.000000 eniris-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 16:14:35.084597 eniris-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 16:14:20.000000 eniris-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.080597 eniris-0.7.2/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 16:14:20.000000 eniris-0.7.2/eniris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-08-06 16:14:20.000000 eniris-0.7.2/eniris/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.084597 eniris-0.7.2/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 16:14:35.084597 eniris-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 16:14:20.000000 eniris-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:14:27.000000 eniris-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:14:39.453792 eniris-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 17:14:27.000000 eniris-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 17:14:27.000000 eniris-0.7.3/eniris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 17:14:27.000000 eniris-0.7.3/eniris/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:14:39.453792 eniris-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:14:27.000000 eniris-0.7.3/setup.py
```

### Comparing `eniris-0.7.2/LICENSE` & `eniris-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.7.2/PKG-INFO` & `eniris-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.2
+Version: 0.7.3
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
 Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
```

### Comparing `eniris-0.7.2/README.md` & `eniris-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.7.2/eniris/driver.py` & `eniris-0.7.3/eniris/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from threading import RLock
 from http import HTTPStatus
 
 class AuthenticationFailure(Exception):
     "Raised when failing to authentiate to the Insights API"
     pass
 
-def retryRequest(requestsFunction:Callable, path:str, authorizationHeaderFunction: Callable|None = None,
+def retryRequest(requestsFunction:Callable, path:str, authorizationHeaderFunction: 'Callable|None' = None,
             maximumRetries:int = 4, initialRetryDelayS:int=1, maximumRetryDelayS:int=60, retryStatusCodes:set[int]=set([HTTPStatus.TOO_MANY_REQUESTS,HTTPStatus.INTERNAL_SERVER_ERROR,HTTPStatus.SERVICE_UNAVAILABLE]), retryNr:int = 0,
             **req_function_kwargs) -> requests.Response:
   """Execute the given requests_function with the provided req_function_kwargs keyword arguments. If the function fails, it will try again until the amount of retries has exceeded.
 
   Args:
       requestsFunction (Callable): Requests function to use. Can be self.session.get, self.session.post, self.session.put or self.session.delete
       path (str): Url to use with the requests function
```

### Comparing `eniris-0.7.2/eniris.egg-info/PKG-INFO` & `eniris-0.7.3/eniris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.2
+Version: 0.7.3
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
 Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
```

### Comparing `eniris-0.7.2/setup.py` & `eniris-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.7.2',
+  version = '0.7.3',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
```

