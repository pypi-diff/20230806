# Comparing `tmp/dcentrapi-0.3.4.tar.gz` & `tmp/dcentrapi-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.3.4.tar", last modified: Sun Aug  6 06:07:07 2023, max compression
+gzip compressed data, was "dcentrapi-0.3.5.tar", last modified: Sun Aug  6 06:12:06 2023, max compression
```

## Comparing `dcentrapi-0.3.4.tar` & `dcentrapi-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.599927 dcentrapi-0.3.4/
--rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.4/LICENSE.rst
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:07:07.599789 dcentrapi-0.3.4/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.4/README.md
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.598866 dcentrapi-0.3.4/dcentrapi/
--rw-r--r--   0 oded       (502) staff       (20)      902 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/dcentrapi/Base.py
--rw-r--r--   0 oded       (502) staff       (20)      482 2023-08-03 11:37:36.000000 dcentrapi-0.3.4/dcentrapi/__init__.py
--rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/eventPolling.py
--rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.4/dcentrapi/gasMonitor.py
--rw-r--r--   0 oded       (502) staff       (20)     1900 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/dcentrapi/hackMitigation.py
--rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.4/dcentrapi/merkleTree.py
--rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/requests_dappi.py
--rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/rpcAggregation.py
--rw-r--r--   0 oded       (502) staff       (20)     1484 2023-08-03 12:37:42.000000 dcentrapi-0.3.4/dcentrapi/test.py
--rw-r--r--   0 oded       (502) staff       (20)     1758 2023-08-03 11:37:36.000000 dcentrapi-0.3.4/dcentrapi/txSimulation.py
--rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.4/dcentrapi/web3Index.py
-drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:07:07.599570 dcentrapi-0.3.4/dcentrapi.egg-info/
--rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 oded       (502) staff       (20)      459 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 oded       (502) staff       (20)        1 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 oded       (502) staff       (20)        9 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 oded       (502) staff       (20)       10 2023-08-06 06:07:07.000000 dcentrapi-0.3.4/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 oded       (502) staff       (20)       38 2023-08-06 06:07:07.599973 dcentrapi-0.3.4/setup.cfg
--rw-r--r--   0 oded       (502) staff       (20)     1109 2023-08-06 06:06:36.000000 dcentrapi-0.3.4/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:12:06.817701 dcentrapi-0.3.5/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.5/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:12:06.817573 dcentrapi-0.3.5/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.5/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:12:06.816708 dcentrapi-0.3.5/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      902 2023-08-06 06:11:59.000000 dcentrapi-0.3.5/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      482 2023-08-03 11:37:36.000000 dcentrapi-0.3.5/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.5/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.5/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)     1900 2023-08-06 06:06:36.000000 dcentrapi-0.3.5/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.5/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.5/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.5/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)        0 2023-08-06 06:11:59.000000 dcentrapi-0.3.5/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)     1758 2023-08-03 11:37:36.000000 dcentrapi-0.3.5/dcentrapi/txSimulation.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.5/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-08-06 06:12:06.817384 dcentrapi-0.3.5/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-08-06 06:12:06.000000 dcentrapi-0.3.5/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      459 2023-08-06 06:12:06.000000 dcentrapi-0.3.5/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-08-06 06:12:06.000000 dcentrapi-0.3.5/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-08-06 06:12:06.000000 dcentrapi-0.3.5/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-08-06 06:12:06.000000 dcentrapi-0.3.5/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-08-06 06:12:06.817737 dcentrapi-0.3.5/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1109 2023-08-06 06:11:59.000000 dcentrapi-0.3.5/setup.py
```

### Comparing `dcentrapi-0.3.4/LICENSE.rst` & `dcentrapi-0.3.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/PKG-INFO` & `dcentrapi-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.4
+Version: 0.3.5
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.4/README.md` & `dcentrapi-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/Base.py` & `dcentrapi-0.3.5/dcentrapi/Base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.3.4"
+        self.__version__ = "0.3.5"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
```

### Comparing `dcentrapi-0.3.4/dcentrapi/eventPolling.py` & `dcentrapi-0.3.5/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/gasMonitor.py` & `dcentrapi-0.3.5/dcentrapi/gasMonitor.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/hackMitigation.py` & `dcentrapi-0.3.5/dcentrapi/hackMitigation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/merkleTree.py` & `dcentrapi-0.3.5/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/rpcAggregation.py` & `dcentrapi-0.3.5/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/txSimulation.py` & `dcentrapi-0.3.5/dcentrapi/txSimulation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi/web3Index.py` & `dcentrapi-0.3.5/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.3.4/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.3.5/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.3.4
+Version: 0.3.5
 Summary: Dcentralab Pypi packages
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `dcentrapi-0.3.4/setup.py` & `dcentrapi-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.3.4"
+VERSION = "0.3.5"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

