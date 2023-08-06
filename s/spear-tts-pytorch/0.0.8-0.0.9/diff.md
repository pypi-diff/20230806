# Comparing `tmp/spear-tts-pytorch-0.0.8.tar.gz` & `tmp/spear-tts-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.8.tar", last modified: Fri Jun 30 17:13:52 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.9.tar", last modified: Sat Jul 15 04:16:31 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.8.tar` & `spear-tts-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.911023 spear-tts-pytorch-0.0.8/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:16:31.642715 spear-tts-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 04:16:21.000000 spear-tts-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-15 04:16:31.642715 spear-tts-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-15 04:16:21.000000 spear-tts-pytorch-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:16:31.642715 spear-tts-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-15 04:16:21.000000 spear-tts-pytorch-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:16:31.642715 spear-tts-pytorch-0.0.9/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-15 04:16:21.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19107 2023-07-15 04:16:21.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:16:31.642715 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-15 04:16:31.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-15 04:16:31.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:16:31.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-15 04:16:31.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 04:16:31.000000 spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.8/LICENSE` & `spear-tts-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.8/PKG-INFO` & `spear-tts-pytorch-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.8/README.md` & `spear-tts-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.8/setup.py` & `spear-tts-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
```

### Comparing `spear-tts-pytorch-0.0.8/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.9/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         # projection to logits
 
         to_semantic_logit = nn.Linear(dim, num_semantic_token_ids, bias = False)
         to_text_logit = nn.Linear(dim, num_text_token_ids, bias = False)
 
         to_semantic_logit.weight = semantic_token_emb.weight
-        to_text_logit.weight = to_text_logit.weight
+        to_text_logit.weight = text_token_emb.weight
 
         self.to_logits = nn.ModuleDict(dict(
             speech = to_semantic_logit,
             text = to_text_logit
         ))
 
         # source and target attention layers
```

### Comparing `spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.9/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

