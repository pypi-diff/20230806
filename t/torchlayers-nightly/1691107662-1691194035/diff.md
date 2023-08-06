# Comparing `tmp/torchlayers-nightly-1691107662.tar.gz` & `tmp/torchlayers-nightly-1691194035.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchlayers-nightly-1691107662.tar", last modified: Fri Aug  4 00:07:51 2023, max compression
+gzip compressed data, was "dist/torchlayers-nightly-1691194035.tar", last modified: Sat Aug  5 00:07:20 2023, max compression
```

## Comparing `torchlayers-nightly-1691107662.tar` & `torchlayers-nightly-1691194035.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/convolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/general_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/jit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/linear_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/padding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/pickle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/recurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/tests/torchlayers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers/
--rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers/_dev_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/_dev_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/_dev_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/_dev_utils/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-04 00:07:42.000000 torchlayers-nightly-1691107662/torchlayers/upsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 00:07:51.000000 torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/convolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/general_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/jit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/linear_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/padding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/pickle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/recurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/tests/torchlayers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers/
+-rw-r--r--   0 runner    (1001) docker     (123)    24781 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers/_dev_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/_dev_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/_dev_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/_dev_utils/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36698 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-08-05 00:07:15.000000 torchlayers-nightly-1691194035/torchlayers/upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17559 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 00:07:20.000000 torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/top_level.txt
```

### Comparing `torchlayers-nightly-1691107662/PKG-INFO` & `torchlayers-nightly-1691194035/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1691107662
+Version: 1691194035
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1691107662/README.md` & `torchlayers-nightly-1691194035/README.md`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/setup.py` & `torchlayers-nightly-1691194035/setup.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/convolution_test.py` & `torchlayers-nightly-1691194035/tests/convolution_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/general_test.py` & `torchlayers-nightly-1691194035/tests/general_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/jit_test.py` & `torchlayers-nightly-1691194035/tests/jit_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/pickle_test.py` & `torchlayers-nightly-1691194035/tests/pickle_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/preprocessing_test.py` & `torchlayers-nightly-1691194035/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/regularization_test.py` & `torchlayers-nightly-1691194035/tests/regularization_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/tests/torchlayers_test.py` & `torchlayers-nightly-1691194035/tests/torchlayers_test.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/__init__.py` & `torchlayers-nightly-1691194035/torchlayers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/_dev_utils/helpers.py` & `torchlayers-nightly-1691194035/torchlayers/_dev_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/_dev_utils/infer.py` & `torchlayers-nightly-1691194035/torchlayers/_dev_utils/infer.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/activations.py` & `torchlayers-nightly-1691194035/torchlayers/activations.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/convolution.py` & `torchlayers-nightly-1691194035/torchlayers/convolution.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/module.py` & `torchlayers-nightly-1691194035/torchlayers/module.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/normalization.py` & `torchlayers-nightly-1691194035/torchlayers/normalization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/pooling.py` & `torchlayers-nightly-1691194035/torchlayers/pooling.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/preprocessing.py` & `torchlayers-nightly-1691194035/torchlayers/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/regularization.py` & `torchlayers-nightly-1691194035/torchlayers/regularization.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers/upsample.py` & `torchlayers-nightly-1691194035/torchlayers/upsample.py`

 * *Files identical despite different names*

### Comparing `torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/PKG-INFO` & `torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlayers-nightly
-Version: 1691107662
+Version: 1691194035
 Summary: Input shape inference and SOTA custom layers for PyTorch.
 Home-page: https://github.com/pypa/torchlayers
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchlayers
 Project-URL: Documentation, https://szymonmaszke.github.io/torchlayers/#torchlayers
```

### Comparing `torchlayers-nightly-1691107662/torchlayers_nightly.egg-info/SOURCES.txt` & `torchlayers-nightly-1691194035/torchlayers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

