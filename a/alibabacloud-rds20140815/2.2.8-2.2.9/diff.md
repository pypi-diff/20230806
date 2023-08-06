# Comparing `tmp/alibabacloud_rds20140815-2.2.8.tar.gz` & `tmp/alibabacloud_rds20140815-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.8.tar", last modified: Sat Jul  8 15:10:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.9.tar", last modified: Sun Jul  9 15:08:57 2023, max compression
```

## Comparing `alibabacloud_rds20140815-2.2.8.tar` & `alibabacloud_rds20140815-2.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:48.000000 alibabacloud_rds20140815-2.2.8/
--rw-r--r--   0 root         (0) root         (0)     1990 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-08 15:10:48.000000 alibabacloud_rds20140815-2.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:48.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1662691 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2540490 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 15:10:48.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-08 15:10:48.000000 alibabacloud_rds20140815-2.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-07-08 15:10:47.000000 alibabacloud_rds20140815-2.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1662691 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2540490 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-09 15:08:57.000000 alibabacloud_rds20140815-2.2.9/setup.py
```

### Comparing `alibabacloud_rds20140815-2.2.8/ChangeLog.md` & `alibabacloud_rds20140815-2.2.9/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-08 Version: 2.2.8
+- Add AutoUseCoupon field.
+- Api Offline.
+
 2023-07-07 Version: 2.2.7
 - Add AutoUseCoupon field.
 - Api Offline.
 
 2023-07-06 Version: 2.2.6
 - Add AutoUseCoupon field.
 - Api Offline.
```

### Comparing `alibabacloud_rds20140815-2.2.8/LICENSE` & `alibabacloud_rds20140815-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.8/PKG-INFO` & `alibabacloud_rds20140815-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.8/README-CN.md` & `alibabacloud_rds20140815-2.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.8/README.md` & `alibabacloud_rds20140815-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.8/alibabacloud_rds20140815.egg-info/PKG-INFO` & `alibabacloud_rds20140815-2.2.9/alibabacloud_rds20140815.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.8/setup.py` & `alibabacloud_rds20140815-2.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815.
 
-Created on 08/07/2023
+Created on 09/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python"
```

