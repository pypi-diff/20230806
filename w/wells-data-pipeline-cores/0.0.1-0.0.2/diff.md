# Comparing `tmp/wells-data-pipeline-cores-0.0.1.tar.gz` & `tmp/wells-data-pipeline-cores-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wells-data-pipeline-cores-0.0.1.tar", last modified: Sun Aug  6 01:51:28 2023, max compression
+gzip compressed data, was "wells-data-pipeline-cores-0.0.2.tar", last modified: Sun Aug  6 03:37:23 2023, max compression
```

## Comparing `wells-data-pipeline-cores-0.0.1.tar` & `wells-data-pipeline-cores-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.440504 wells-data-pipeline-cores-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/test/test_env_vars_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.440504 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/dev_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/env_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/key_vaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.444504 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_adx_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_storage_account_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/send_email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/snow_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-08-06 01:51:17.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/wells_etl_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:51:28.440504 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 01:51:28.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-06 01:51:28.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:51:28.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 01:51:28.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-06 01:51:28.000000 wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.924891 wells-data-pipeline-cores-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/test/test_env_vars_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.924891 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/dev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19055 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/env_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/key_vaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_adx_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_storage_account_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/send_email_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/snow_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-08-06 03:37:10.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/wells_etl_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:37:23.928891 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 03:37:23.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-06 03:37:23.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:37:23.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 03:37:23.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-06 03:37:23.000000 wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/top_level.txt
```

### Comparing `wells-data-pipeline-cores-0.0.1/README.md` & `wells-data-pipeline-cores-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/setup.py` & `wells-data-pipeline-cores-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Wells Data Pipeline Cores
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wells-data-pipeline-cores"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/common.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/common.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/env_variables.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/env_variables.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/key_vaults.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/key_vaults.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/commons/utils.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/commons/utils.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/__init__.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/__init__.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_ad_authz_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_adx_data_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_adx_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_cosmos_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/az_storage_account_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/az_storage_account_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/send_email_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/send_email_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/snow_data_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/snow_data_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores/services/cores/wells_etl_service.py` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores/services/cores/wells_etl_service.py`

 * *Files identical despite different names*

### Comparing `wells-data-pipeline-cores-0.0.1/wells_data_pipeline_cores.egg-info/SOURCES.txt` & `wells-data-pipeline-cores-0.0.2/wells_data_pipeline_cores.egg-info/SOURCES.txt`

 * *Files identical despite different names*

