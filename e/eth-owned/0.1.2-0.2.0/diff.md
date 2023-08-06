# Comparing `tmp/eth-owned-0.1.2.tar.gz` & `tmp/eth-owned-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eth-owned-0.1.2.tar", last modified: Fri Jun  9 09:34:28 2023, max compression
+gzip compressed data, was "eth-owned-0.2.0.tar", last modified: Sun Aug  6 15:18:09 2023, max compression
```

## Comparing `eth-owned-0.1.2.tar` & `eth-owned-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/
--rw-r--r--   0 lash      (1000) lash      (1000)     3216 2021-04-17 09:25:30.000000 eth-owned-0.1.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       43 2021-08-24 19:44:28.000000 eth-owned-0.1.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-06-09 09:34:28.246656 eth-owned-0.1.2/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.239989 eth-owned-0.1.2/eth_owned/
--rw-r--r--   0 lash      (1000) lash      (1000)       62 2023-03-25 13:46:48.000000 eth-owned-0.1.2/eth_owned/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     3138 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/Owned.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     1020 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/Owned.json
--rw-r--r--   0 lash      (1000) lash      (1000)     1502 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/OwnedSimple.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/OwnedSimple.json
--rw-r--r--   0 lash      (1000) lash      (1000)     4116 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/VoidOwner.bin
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-28 20:25:47.000000 eth-owned-0.1.2/eth_owned/data/VoidOwner.json
--rw-r--r--   0 lash      (1000) lash      (1000)       85 2021-04-17 05:52:58.000000 eth-owned-0.1.2/eth_owned/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1620 2023-03-25 13:46:21.000000 eth-owned-0.1.2/eth_owned/owned.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2101 2021-10-24 14:08:49.000000 eth-owned-0.1.2/eth_owned/runnable/owner.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4216 2021-10-24 14:07:02.000000 eth-owned-0.1.2/eth_owned/runnable/void.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4015 2021-10-24 14:05:55.000000 eth-owned-0.1.2/eth_owned/runnable/void_deploy.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/eth_owned/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)      128 2023-06-09 09:27:31.000000 eth-owned-0.1.2/eth_owned/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1348 2023-03-25 13:47:19.000000 eth-owned-0.1.2/eth_owned/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5018 2023-06-09 09:27:28.000000 eth-owned-0.1.2/eth_owned/unittest/interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1406 2021-08-24 19:44:28.000000 eth-owned-0.1.2/eth_owned/void.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.243322 eth-owned-0.1.2/eth_owned.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      735 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      114 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       10 2023-06-09 09:34:28.000000 eth-owned-0.1.2/eth_owned.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-05-15 14:07:11.000000 eth-owned-0.1.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1019 2023-06-09 09:34:28.246656 eth-owned-0.1.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      642 2021-04-17 09:25:26.000000 eth-owned-0.1.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-17 06:02:27.000000 eth-owned-0.1.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-09 09:34:28.246656 eth-owned-0.1.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      262 2023-02-28 20:33:12.000000 eth-owned-0.1.2/tests/test_owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.052306 eth-owned-0.2.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3216 2021-04-17 09:25:30.000000 eth-owned-0.2.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       43 2021-08-24 19:44:28.000000 eth-owned-0.2.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-06 15:18:09.052306 eth-owned-0.2.0/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.048972 eth-owned-0.2.0/eth_owned/
+-rw-r--r--   0 lash      (1000) lash      (1000)       62 2023-03-25 13:46:48.000000 eth-owned-0.2.0/eth_owned/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.052306 eth-owned-0.2.0/eth_owned/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3138 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/Owned.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     1020 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/Owned.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     1502 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/OwnedSimple.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      655 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/OwnedSimple.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     4116 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/VoidOwner.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2023-02-28 20:25:47.000000 eth-owned-0.2.0/eth_owned/data/VoidOwner.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       85 2021-04-17 05:52:58.000000 eth-owned-0.2.0/eth_owned/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1620 2023-03-25 13:46:21.000000 eth-owned-0.2.0/eth_owned/owned.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.052306 eth-owned-0.2.0/eth_owned/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2101 2021-10-24 14:08:49.000000 eth-owned-0.2.0/eth_owned/runnable/owner.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4216 2021-10-24 14:07:02.000000 eth-owned-0.2.0/eth_owned/runnable/void.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4015 2021-10-24 14:05:55.000000 eth-owned-0.2.0/eth_owned/runnable/void_deploy.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.052306 eth-owned-0.2.0/eth_owned/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)      128 2023-06-09 09:27:31.000000 eth-owned-0.2.0/eth_owned/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1348 2023-03-25 13:47:19.000000 eth-owned-0.2.0/eth_owned/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5018 2023-06-09 09:27:28.000000 eth-owned-0.2.0/eth_owned/unittest/interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1406 2021-08-24 19:44:28.000000 eth-owned-0.2.0/eth_owned/void.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.048972 eth-owned-0.2.0/eth_owned.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      715 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      735 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       60 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      114 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       10 2023-08-06 15:18:09.000000 eth-owned-0.2.0/eth_owned.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-08-06 15:17:08.000000 eth-owned-0.2.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1019 2023-08-06 15:18:09.052306 eth-owned-0.2.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      642 2021-04-17 09:25:26.000000 eth-owned-0.2.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       37 2021-04-17 06:02:27.000000 eth-owned-0.2.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 15:18:09.052306 eth-owned-0.2.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      262 2023-02-28 20:33:12.000000 eth-owned-0.2.0/tests/test_owned.py
```

### Comparing `eth-owned-0.1.2/LICENSE` & `eth-owned-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/PKG-INFO` & `eth-owned-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-owned
-Version: 0.1.2
+Version: 0.2.0
 Summary: EIP 173 interface and tools
 Home-page: https://holbrook.no/src/eth-owned/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-owned-0.1.2/eth_owned/data/Owned.bin` & `eth-owned-0.2.0/eth_owned/data/Owned.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/data/Owned.json` & `eth-owned-0.2.0/eth_owned/data/Owned.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/data/OwnedSimple.bin` & `eth-owned-0.2.0/eth_owned/data/OwnedSimple.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/data/OwnedSimple.json` & `eth-owned-0.2.0/eth_owned/data/OwnedSimple.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/data/VoidOwner.bin` & `eth-owned-0.2.0/eth_owned/data/VoidOwner.bin`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/data/VoidOwner.json` & `eth-owned-0.2.0/eth_owned/data/VoidOwner.json`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/owned.py` & `eth-owned-0.2.0/eth_owned/owned.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/runnable/owner.py` & `eth-owned-0.2.0/eth_owned/runnable/owner.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/runnable/void.py` & `eth-owned-0.2.0/eth_owned/runnable/void.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/runnable/void_deploy.py` & `eth-owned-0.2.0/eth_owned/runnable/void_deploy.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/unittest/base.py` & `eth-owned-0.2.0/eth_owned/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/unittest/interface.py` & `eth-owned-0.2.0/eth_owned/unittest/interface.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned/void.py` & `eth-owned-0.2.0/eth_owned/void.py`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/eth_owned.egg-info/PKG-INFO` & `eth-owned-0.2.0/eth_owned.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-owned
-Version: 0.1.2
+Version: 0.2.0
 Summary: EIP 173 interface and tools
 Home-page: https://holbrook.no/src/eth-owned/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-owned-0.1.2/eth_owned.egg-info/SOURCES.txt` & `eth-owned-0.2.0/eth_owned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-owned-0.1.2/setup.cfg` & `eth-owned-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-owned
-version = 0.1.2
+version = 0.2.0
 description = EIP 173 interface and tools
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/eth-owned/log.html
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-owned-0.1.2/setup.py` & `eth-owned-0.2.0/setup.py`

 * *Files identical despite different names*

