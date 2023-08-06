# Comparing `tmp/autogluon.features-0.8.3b20230804.tar.gz` & `tmp/autogluon.features-0.8.3b20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.features-0.8.3b20230804.tar", last modified: Fri Aug  4 09:04:10 2023, max compression
+gzip compressed data, was "autogluon.features-0.8.3b20230805.tar", last modified: Sat Aug  5 09:03:58 2023, max compression
```

## Comparing `autogluon.features-0.8.3b20230804.tar` & `autogluon.features-0.8.3b20230805.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.322238 autogluon.features-0.8.3b20230804/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-04 09:04:10.322238 autogluon.features-0.8.3b20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:04:10.322238 autogluon.features-0.8.3b20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.318238 autogluon.features-0.8.3b20230804/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.318238 autogluon.features-0.8.3b20230804/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.318238 autogluon.features-0.8.3b20230804/src/autogluon/features/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.322238 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44204 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/auto_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/drop_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/drop_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/fillna.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/isnan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/memory_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/text_ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/generators/text_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-04 09:03:48.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon/features/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:10.318238 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:10.000000 autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.392007 autogluon.features-0.8.3b20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-08-05 09:03:58.392007 autogluon.features-0.8.3b20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:03:58.392007 autogluon.features-0.8.3b20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.380007 autogluon.features-0.8.3b20230805/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.380007 autogluon.features-0.8.3b20230805/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.384007 autogluon.features-0.8.3b20230805/src/autogluon/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.392007 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44204 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/auto_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/drop_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/drop_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/fillna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/isnan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/memory_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/text_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/generators/text_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-05 09:03:35.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon/features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:58.384007 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:03:58.000000 autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/zip-safe
```

### Comparing `autogluon.features-0.8.3b20230804/PKG-INFO` & `autogluon.features-0.8.3b20230805/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.3b20230804
+Version: 0.8.3b20230805
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -17,14 +17,15 @@
         </div>
         
         ## AutoML for Image, Text, Time Series, and Tabular Data
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
+        [![Broken Link Checker](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml/badge.svg)](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
```

### Comparing `autogluon.features-0.8.3b20230804/setup.py` & `autogluon.features-0.8.3b20230805/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/binning.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/binning.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/__init__.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/abstract.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/astype.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/astype.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/auto_ml_pipeline.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/auto_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/binned.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/binned.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/bulk.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/bulk.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/category.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/category.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/datetime.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/drop_duplicates.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/drop_duplicates.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/drop_unique.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/drop_unique.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/dummy.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/dummy.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/fillna.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/identity.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/identity.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/isnan.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/isnan.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/label_encoder.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/memory_minimize.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/memory_minimize.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/one_hot_encoder.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/pipeline.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/rename.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/rename.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/text_ngram.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/text_ngram.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/generators/text_special.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/generators/text_special.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/utils.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon/features/vectorizers.py` & `autogluon.features-0.8.3b20230805/src/autogluon/features/vectorizers.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/PKG-INFO` & `autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.8.3b20230804
+Version: 0.8.3b20230805
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -17,14 +17,15 @@
         </div>
         
         ## AutoML for Image, Text, Time Series, and Tabular Data
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
+        [![Broken Link Checker](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml/badge.svg)](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
```

### Comparing `autogluon.features-0.8.3b20230804/src/autogluon.features.egg-info/SOURCES.txt` & `autogluon.features-0.8.3b20230805/src/autogluon.features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

