# Comparing `tmp/alibabacloud_rds-data20220330_py2-1.0.1.tar.gz` & `tmp/alibabacloud_rds-data20220330_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds-data20220330_py2-1.0.1.tar", last modified: Sat Aug  5 15:03:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds-data20220330_py2-1.0.2.tar", last modified: Sun Aug  6 15:02:56 2023, max compression
```

## Comparing `alibabacloud_rds-data20220330_py2-1.0.1.tar` & `alibabacloud_rds-data20220330_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       72 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18957 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/client.py
--rw-r--r--   0 root         (0) root         (0)    86852 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2930 2023-08-05 15:03:23.000000 alibabacloud_rds-data20220330_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      144 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18957 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/client.py
+-rw-r--r--   0 root         (0) root         (0)    86852 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-08-06 15:02:56.000000 alibabacloud_rds-data20220330_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/LICENSE` & `alibabacloud_rds-data20220330_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/PKG-INFO` & `alibabacloud_rds-data20220330_py2-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds-data20220330_py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud rds-data (20220330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/README-CN.md` & `alibabacloud_rds-data20220330_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/README.md` & `alibabacloud_rds-data20220330_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/client.py` & `alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330/models.py` & `alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/alibabacloud_rds_data20220330_py2.egg-info/PKG-INFO` & `alibabacloud_rds-data20220330_py2-1.0.2/alibabacloud_rds_data20220330_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds-data20220330-py2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud rds-data (20220330) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds-data20220330_py2-1.0.1/setup.py` & `alibabacloud_rds-data20220330_py2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds-data20220330_py2.
 
-Created on 05/08/2023
+Created on 06/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds_data20220330"
 NAME = "alibabacloud_rds-data20220330_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds-data (20220330) SDK Library for Python2"
```

