# Comparing `tmp/voicebox-pytorch-0.0.8.tar.gz` & `tmp/voicebox-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.8.tar", last modified: Sun Aug  6 03:48:56 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.9.tar", last modified: Sun Aug  6 03:50:08 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.8.tar` & `voicebox-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:48:56.891018 voicebox-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:48:56.891018 voicebox-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:48:56.891018 voicebox-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:48:56.891018 voicebox-pytorch-0.0.8/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-08-06 03:48:42.000000 voicebox-pytorch-0.0.8/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:48:56.891018 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:48:56.000000 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-06 03:48:56.000000 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:48:56.000000 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 03:48:56.000000 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 03:48:56.000000 voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:50:08.469484 voicebox-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:50:08.469484 voicebox-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:50:08.469484 voicebox-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:50:08.469484 voicebox-pytorch-0.0.9/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-08-06 03:49:59.000000 voicebox-pytorch-0.0.9/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:50:08.469484 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-06 03:50:08.000000 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-06 03:50:08.000000 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:50:08.000000 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 03:50:08.000000 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 03:50:08.000000 voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.8/LICENSE` & `voicebox-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.8/PKG-INFO` & `voicebox-pytorch-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.8/README.md` & `voicebox-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.8/setup.py` & `voicebox-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
```

### Comparing `voicebox-pytorch-0.0.8/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.9/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.8/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.9/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,15 +514,17 @@
         cond_drop_prob = 0.,
         prob_seq_drop = 0.3  # not entirely sure
     ):
         super().__init__()
         self.sigma = sigma
 
         self.voicebox = voicebox
+
         self.cond_drop_prob = cond_drop_prob
+        self.prob_seq_drop = prob_seq_drop
 
         self.odeint_kwargs = dict(
             atol = ode_atol,
             rtol = ode_rtol,
             method= ode_method
         )
```

### Comparing `voicebox-pytorch-0.0.8/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.9/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

