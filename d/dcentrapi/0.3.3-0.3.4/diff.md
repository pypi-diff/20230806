# Comparing `tmp/dcentrapi-0.3.3.tar.gz` & `tmp/dcentrapi-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.3.3.tar", last modified: Thu Aug  3 12:41:59 2023, max compression
+gzip compressed data, was "dcentrapi-0.3.4.tar", last modified: Sun Aug  6 06:07:07 2023, max compression
```

## Comparing `dcentrapi-0.3.3.tar` & `dcentrapi-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.035478 dcentrapi-0.3.3/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.3/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-03 12:41:59.035343 dcentrapi-0.3.3/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.3/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.034450 dcentrapi-0.3.3/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      902 2023-08-03 12:41:57.000000 dcentrapi-0.3.3/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      482 2023-08-03 11:37:36.000000 dcentrapi-0.3.3/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.3/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)     1548 2023-08-03 12:36:23.000000 dcentrapi-0.3.3/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.3/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/requests_dappi.py
--rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)     1484 2023-08-03 12:37:42.000000 dcentrapi-0.3.3/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)     1758 2023-08-03 11:37:36.000000 dcentrapi-0.3.3/dcentrapi/txSimulation.py
--rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.3/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-03 12:41:59.035149 dcentrapi-0.3.3/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      459 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-08-03 12:41:59.000000 dcentrapi-0.3.3/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-08-03 12:41:59.035524 dcentrapi-0.3.3/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1109 2023-08-03 12:41:57.000000 dcentrapi-0.3.3/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.599927 dcentrapi-0.3.4/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.4/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:07:07.599789 dcentrapi-0.3.4/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.4/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.598866 dcentrapi-0.3.4/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      902 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      482 2023-08-03 11:37:36.000000 dcentrapi-0.3.4/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.4/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)     1900 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.4/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)     1484 2023-08-03 12:37:42.000000 dcentrapi-0.3.4/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)     1758 2023-08-03 11:37:36.000000 dcentrapi-0.3.4/dcentrapi/txSimulation.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.599570 dcentrapi-0.3.4/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      459 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-08-06 06:07:07.599973 dcentrapi-0.3.4/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1109 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/setup.py
```

### Comparing `dcentrapi-0.3.3/LICENSE.rst` & `dcentrapi-0.3.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/PKG-INFO` & `dcentrapi-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.3
+Version: 0.3.4
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.3/README.md` & `dcentrapi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/Base.py` & `dcentrapi-0.3.4/dcentrapi/Base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.3.3"
+        self.__version__ = "0.3.4"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.3.3/dcentrapi/eventPolling.py` & `dcentrapi-0.3.4/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/gasMonitor.py` & `dcentrapi-0.3.4/dcentrapi/gasMonitor.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/hackMitigation.py` & `dcentrapi-0.3.4/dcentrapi/hackMitigation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import logging
 import traceback
+from time import sleep
 from dcentrapi.Base import Base, DapiError
 from dcentrapi.requests_dappi import requests_get
 
 logger = logging.getLogger()
 logger.setLevel("INFO")
 
 
@@ -23,18 +24,26 @@
             logger.info(f"before request: {before}")
             try:
                 response = requests_get(url, params=data, headers=self.headers)
 
                 after = datetime.datetime.now()
                 logger.info(f"after request: {after}")
                 logger.info(f"time elapsed: {after-before}")
+
                 if response.status_code == 200:
                     # Parse the JSON data using the json() method
-                    data = response.json()
-                    logger.info(f"data={data}")  # This will logger.info the parsed JSON data as a Python dictionary
-                    return data
+                    response_data = response.json()
+                    logger.info(f"data={response_data}")  # This will print the parsed JSON data as a Python dictionary
+                    return response_data
                 else:
-                    logger.error(f"Request failed with status code: {response.status_code} and error message: {response.error_message}")
+                    msg = f"Request failed with status code: {response.status_code}"
+                    if hasattr(response, "error_message"):
+                        msg += f" and error message: {response.error_message}"
+                    logger.error(msg)
                     tries -= 1
+                    logger.info(f"sleeping for 1.75 secs")
+                    sleep(1.75)
 
             except Exception as e:
                 return DapiError(response=response.__dict__, exception=f"e: {e}, traceback: {traceback.format_exc()}")
+
+        return DapiError(response=response.__dict__, exception="Stop retry after 7 tries")
```

### Comparing `dcentrapi-0.3.3/dcentrapi/merkleTree.py` & `dcentrapi-0.3.4/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/rpcAggregation.py` & `dcentrapi-0.3.4/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/test.py` & `dcentrapi-0.3.4/dcentrapi/test.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/txSimulation.py` & `dcentrapi-0.3.4/dcentrapi/txSimulation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi/web3Index.py` & `dcentrapi-0.3.4/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.3/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.3.4/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.3
+Version: 0.3.4
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.3/setup.py` & `dcentrapi-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.3.3"
+VERSION = "0.3.4"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

