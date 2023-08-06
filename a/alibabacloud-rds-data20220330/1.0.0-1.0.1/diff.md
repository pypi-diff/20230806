# Comparing `tmp/alibabacloud_rds-data20220330-1.0.0.tar.gz` & `tmp/alibabacloud_rds-data20220330-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds-data20220330-1.0.0.tar", last modified: Fri Aug  4 15:04:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds-data20220330-1.0.1.tar", last modified: Sat Aug  5 15:04:11 2023, max compression
```

## Comparing `alibabacloud_rds-data20220330-1.0.0.tar` & `alibabacloud_rds-data20220330-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42584 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/client.py
--rw-r--r--   0 root         (0) root         (0)    86832 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      447 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2638 2023-08-04 15:04:18.000000 alibabacloud_rds-data20220330-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42584 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/client.py
+-rw-r--r--   0 root         (0) root         (0)    86832 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-08-05 15:04:11.000000 alibabacloud_rds-data20220330-1.0.1/setup.py
```

### Comparing `alibabacloud_rds-data20220330-1.0.0/LICENSE` & `alibabacloud_rds-data20220330-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330-1.0.0/PKG-INFO` & `alibabacloud_rds-data20220330-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds-data20220330
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud rds-data (20220330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds-data20220330-1.0.0/README-CN.md` & `alibabacloud_rds-data20220330-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330-1.0.0/README.md` & `alibabacloud_rds-data20220330-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/client.py` & `alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330/models.py` & `alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330-1.0.0/alibabacloud_rds_data20220330.egg-info/PKG-INFO` & `alibabacloud_rds-data20220330-1.0.1/alibabacloud_rds_data20220330.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds-data20220330
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud rds-data (20220330) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds-data20220330-1.0.0/setup.py` & `alibabacloud_rds-data20220330-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds-data20220330.
 
-Created on 04/08/2023
+Created on 05/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds_data20220330"
 NAME = "alibabacloud_rds-data20220330" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds-data (20220330) SDK Library for Python"
```

