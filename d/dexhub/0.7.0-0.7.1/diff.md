# Comparing `tmp/dexhub-0.7.0.tar.gz` & `tmp/dexhub-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.7.0.tar", last modified: Sun Aug  6 14:54:35 2023, max compression
+gzip compressed data, was "dexhub-0.7.1.tar", last modified: Sun Aug  6 14:59:45 2023, max compression
```

## Comparing `dexhub-0.7.0.tar` & `dexhub-0.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.164568 dexhub-0.7.0/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:54:35.164410 dexhub-0.7.0/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.0/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.160066 dexhub-0.7.0/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1249 2023-08-06 14:33:56.000000 dexhub-0.7.0/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.162360 dexhub-0.7.0/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      261 2023-08-06 10:36:45.000000 dexhub-0.7.0/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.0/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.0/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.0/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.0/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.7.0/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.163500 dexhub-0.7.0/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      499 2023-08-06 14:33:28.000000 dexhub-0.7.0/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.0/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.0/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.0/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.0/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.7.0/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.0/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      886 2023-08-06 14:26:53.000000 dexhub-0.7.0/dexhub/bridge.py
--rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.0/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.163791 dexhub-0.7.0/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.0/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.0/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.164203 dexhub-0.7.0/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.0/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.0/dexhub/util/helper.py
--rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.0/dexhub/util/joe_v2.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:54:35.161050 dexhub-0.7.0/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:54:34.000000 dexhub-0.7.0/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 14:54:35.000000 dexhub-0.7.0/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 14:54:34.000000 dexhub-0.7.0/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 14:54:35.000000 dexhub-0.7.0/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 14:54:35.000000 dexhub-0.7.0/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 14:54:35.164620 dexhub-0.7.0/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 14:54:26.000000 dexhub-0.7.0/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.354229 dexhub-0.7.1/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:59:45.354097 dexhub-0.7.1/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.7.1/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.350906 dexhub-0.7.1/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1291 2023-08-06 14:59:24.000000 dexhub-0.7.1/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.352462 dexhub-0.7.1/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      261 2023-08-06 10:36:45.000000 dexhub-0.7.1/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.7.1/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.7.1/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    28418 2023-08-06 10:36:23.000000 dexhub-0.7.1/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.7.1/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.7.1/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353282 dexhub-0.7.1/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      499 2023-08-06 14:33:28.000000 dexhub-0.7.1/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.7.1/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.7.1/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4654 2023-08-06 14:33:24.000000 dexhub-0.7.1/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.7.1/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.7.1/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.7.1/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      886 2023-08-06 14:26:53.000000 dexhub-0.7.1/dexhub/bridge.py
+-rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.7.1/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353510 dexhub-0.7.1/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.7.1/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.7.1/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.353923 dexhub-0.7.1/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.7.1/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.7.1/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.7.1/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-08-06 14:59:45.351577 dexhub-0.7.1/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      696 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-08-06 14:59:45.000000 dexhub-0.7.1/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-08-06 14:59:45.354273 dexhub-0.7.1/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-08-06 14:59:38.000000 dexhub-0.7.1/setup.py
```

### Comparing `dexhub-0.7.0/PKG-INFO` & `dexhub-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.7.0
+Version: 0.7.1
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.7.0/dexhub/__init__.py` & `dexhub-0.7.1/dexhub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 name = "dex"
 
+from dexhub.bridge import(
+    Synapse
+)
+
 from dexhub.dex import(
     Erc20,
     UniswapV2,UniswapV2Pair,
     UniswapV3,UniswapV3Quoter,UniswapV3Factory,UniswapV3Router,
     JoeV2Factory,JoeV2Pair,JoeV2Route,JoeV2Quote,JoeV2Erc20
 )
```

### Comparing `dexhub-0.7.0/dexhub/abi/arbitrum_abi.py` & `dexhub-0.7.1/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/abi/avax_abi.py` & `dexhub-0.7.1/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/abi/dfk_abi.py` & `dexhub-0.7.1/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/abi/eth_abi.py` & `dexhub-0.7.1/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/abi/klay_abi.py` & `dexhub-0.7.1/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/arbitrum_address.py` & `dexhub-0.7.1/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/avax_address.py` & `dexhub-0.7.1/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/dfk_address.py` & `dexhub-0.7.1/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/eth_address.py` & `dexhub-0.7.1/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/klay_address.py` & `dexhub-0.7.1/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/address/polygon_address.py` & `dexhub-0.7.1/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/bridge.py` & `dexhub-0.7.1/dexhub/bridge.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/dex.py` & `dexhub-0.7.1/dexhub/dex.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/interface/joe.py` & `dexhub-0.7.1/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub/util/helper.py` & `dexhub-0.7.1/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/dexhub.egg-info/PKG-INFO` & `dexhub-0.7.1/dexhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.7.0
+Version: 0.7.1
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.7.0/dexhub.egg-info/SOURCES.txt` & `dexhub-0.7.1/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.7.0/setup.py` & `dexhub-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.7.0",
+    version="0.7.1",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

