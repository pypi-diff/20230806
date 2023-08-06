# Comparing `tmp/torch_rim-0.2.8.tar.gz` & `tmp/torch_rim-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_rim-0.2.8.tar", last modified: Sun Aug  6 00:45:35 2023, max compression
+gzip compressed data, was "torch_rim-0.2.9.tar", last modified: Sun Aug  6 00:52:20 2023, max compression
```

## Comparing `torch_rim-0.2.8.tar` & `torch_rim-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.771949 torch_rim-0.2.8/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-08-05 23:02:16.000000 torch_rim-0.2.8/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    10410 2023-08-06 00:45:35.767949 torch_rim-0.2.8/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9515 2023-08-05 23:53:31.000000 torch_rim-0.2.8/README.md
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.767949 torch_rim-0.2.8/rim/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.8/rim/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.767949 torch_rim-0.2.8/rim/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.8/rim/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.8/rim/architectures/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5859 2023-08-05 23:39:49.000000 torch_rim-0.2.8/rim/architectures/hourglass.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.8/rim/architectures/unet.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.8/rim/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.767949 torch_rim-0.2.8/rim/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.8/rim/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.8/rim/layers/gru.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.8/rim/layers/gru_component.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23019 2023-08-06 00:42:22.000000 torch_rim-0.2.8/rim/rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.8/rim/utils.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-06 00:45:35.771949 torch_rim-0.2.8/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      883 2023-08-06 00:45:24.000000 torch_rim-0.2.8/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.767949 torch_rim-0.2.8/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.8/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.8/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4255 2023-08-06 00:45:02.000000 torch_rim-0.2.8/tests/test_rim.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.8/tests/test_training.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:45:35.767949 torch_rim-0.2.8/torch_rim.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    10410 2023-08-06 00:45:35.000000 torch_rim-0.2.8/torch_rim.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      525 2023-08-06 00:45:35.000000 torch_rim-0.2.8/torch_rim.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-06 00:45:35.000000 torch_rim-0.2.8/torch_rim.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       58 2023-08-06 00:45:35.000000 torch_rim-0.2.8/torch_rim.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-06 00:45:35.000000 torch_rim-0.2.8/torch_rim.egg-info/top_level.txt
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-08-05 23:02:16.000000 torch_rim-0.2.9/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    10404 2023-08-06 00:52:20.051948 torch_rim-0.2.9/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     9509 2023-08-06 00:51:02.000000 torch_rim-0.2.9/README.md
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/rim/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       72 2023-07-30 05:03:49.000000 torch_rim-0.2.9/rim/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/rim/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       33 2023-07-30 04:16:22.000000 torch_rim-0.2.9/rim/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      364 2023-07-30 04:46:56.000000 torch_rim-0.2.9/rim/architectures/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5859 2023-08-05 23:39:49.000000 torch_rim-0.2.9/rim/architectures/hourglass.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        7 2023-07-30 05:34:37.000000 torch_rim-0.2.9/rim/architectures/unet.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      108 2023-07-29 23:08:17.000000 torch_rim-0.2.9/rim/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/rim/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      358 2023-07-31 23:40:45.000000 torch_rim-0.2.9/rim/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2269 2023-08-01 00:03:41.000000 torch_rim-0.2.9/rim/layers/gru.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1921 2023-07-30 00:22:46.000000 torch_rim-0.2.9/rim/layers/gru_component.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    23019 2023-08-06 00:42:22.000000 torch_rim-0.2.9/rim/rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2926 2023-07-31 19:31:56.000000 torch_rim-0.2.9/rim/utils.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-06 00:52:20.051948 torch_rim-0.2.9/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      883 2023-08-06 00:52:07.000000 torch_rim-0.2.9/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2137 2023-08-01 00:00:12.000000 torch_rim-0.2.9/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2693 2023-08-01 00:04:18.000000 torch_rim-0.2.9/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4255 2023-08-06 00:45:02.000000 torch_rim-0.2.9/tests/test_rim.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3938 2023-08-05 21:32:32.000000 torch_rim-0.2.9/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-06 00:52:20.051948 torch_rim-0.2.9/torch_rim.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    10404 2023-08-06 00:52:19.000000 torch_rim-0.2.9/torch_rim.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      525 2023-08-06 00:52:20.000000 torch_rim-0.2.9/torch_rim.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-06 00:52:19.000000 torch_rim-0.2.9/torch_rim.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       58 2023-08-06 00:52:19.000000 torch_rim-0.2.9/torch_rim.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        4 2023-08-06 00:52:19.000000 torch_rim-0.2.9/torch_rim.egg-info/top_level.txt
```

### Comparing `torch_rim-0.2.8/LICENSE.txt` & `torch_rim-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/PKG-INFO` & `torch_rim-0.2.9/torch_rim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch_rim
-Version: 0.2.8
+Name: torch-rim
+Version: 0.2.9
 Summary: A torch implementation of the Recurrent Inference Machine
 Home-page: https://github.com/AlexandreAdam/torch_rim
 Author: Alexandre Adam
 Author-email: alexande.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
     pip install torch-rim
 
 Usage
 -----
 
 .. code-block:: python
 
-    from torch_rim import RIM, Hourglass, Unet
+    from rim import RIM, Hourglass, Unet
     from torch.func import vmap
 
     # B is the batch size
     # C is the input channels
     # dimensions are the spatial dimensions (e.g. [28, 28] for MNIST)
 
     # Create a score_fn, e.g. a Gaussian likelihood score function
```

### Comparing `torch_rim-0.2.8/README.md` & `torch_rim-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 To install the package, you can use pip:
 ```bash
 pip install torch-rim
 ```
 
 # Usage
 ```python
-from torch_rim import RIM, Hourglass, Unet
+from rim import RIM, Hourglass, Unet
 from torch.func import vmap
 
 # B is the batch size
 # C is the input channels
 # dimensions are the spatial dimensions (e.g. [28, 28] for MNIST)
 
 # Create a score_fn, e.g. a Gaussian likelihood score function
```

### Comparing `torch_rim-0.2.8/rim/architectures/hourglass.py` & `torch_rim-0.2.9/rim/architectures/hourglass.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/rim/layers/gru.py` & `torch_rim-0.2.9/rim/layers/gru.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/rim/layers/gru_component.py` & `torch_rim-0.2.9/rim/layers/gru_component.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/rim/rim.py` & `torch_rim-0.2.9/rim/rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/rim/utils.py` & `torch_rim-0.2.9/rim/utils.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/setup.py` & `torch_rim-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch_rim',
-    version='0.2.8',
+    version='0.2.9',
     author='Alexandre Adam',
     author_email='alexande.adam@umontreal.ca',
     description='A torch implementation of the Recurrent Inference Machine',
     long_description=long_description,
     url="https://github.com/AlexandreAdam/torch_rim",
     packages=find_packages(),
     install_requires=[
```

### Comparing `torch_rim-0.2.8/tests/test_architectures.py` & `torch_rim-0.2.9/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/tests/test_layers.py` & `torch_rim-0.2.9/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/tests/test_rim.py` & `torch_rim-0.2.9/tests/test_rim.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/tests/test_training.py` & `torch_rim-0.2.9/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `torch_rim-0.2.8/torch_rim.egg-info/PKG-INFO` & `torch_rim-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-rim
-Version: 0.2.8
+Name: torch_rim
+Version: 0.2.9
 Summary: A torch implementation of the Recurrent Inference Machine
 Home-page: https://github.com/AlexandreAdam/torch_rim
 Author: Alexandre Adam
 Author-email: alexande.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
     pip install torch-rim
 
 Usage
 -----
 
 .. code-block:: python
 
-    from torch_rim import RIM, Hourglass, Unet
+    from rim import RIM, Hourglass, Unet
     from torch.func import vmap
 
     # B is the batch size
     # C is the input channels
     # dimensions are the spatial dimensions (e.g. [28, 28] for MNIST)
 
     # Create a score_fn, e.g. a Gaussian likelihood score function
```

### Comparing `torch_rim-0.2.8/torch_rim.egg-info/SOURCES.txt` & `torch_rim-0.2.9/torch_rim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

