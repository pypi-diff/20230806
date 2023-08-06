# Comparing `tmp/lc-checkpoint-0.5.1.tar.gz` & `tmp/lc-checkpoint-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.5.1.tar", last modified: Mon Jul 31 11:53:22 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.5.2.tar", last modified: Sun Aug  6 10:51:32 2023, max compression
```

## Comparing `lc-checkpoint-0.5.1.tar` & `lc-checkpoint-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5698 2023-07-31 11:31:00.000000 lc-checkpoint-0.5.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/lc_checkpoint/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2023-07-31 11:10:39.000000 lc-checkpoint-0.5.1/src/lc_checkpoint/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/top_level.txt
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-08-06 10:51:32.932426 lc-checkpoint-0.5.2/
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     1041 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.2/LICENSE
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)     6212 2023-08-06 10:51:32.932539 lc-checkpoint-0.5.2/PKG-INFO
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     5869 2023-08-06 10:50:25.000000 lc-checkpoint-0.5.2/README.md
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      104 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.2/pyproject.toml
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      608 2023-08-06 10:51:32.933000 lc-checkpoint-0.5.2/setup.cfg
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-08-06 10:51:32.930020 lc-checkpoint-0.5.2/src/
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-08-06 10:51:32.931359 lc-checkpoint-0.5.2/src/lc_checkpoint/
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        0 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.2/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     8180 2023-08-06 10:32:12.000000 lc-checkpoint-0.5.2/src/lc_checkpoint/main.py
+drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-08-06 10:51:32.932245 lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)     6212 2023-08-06 10:51:32.000000 lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)      262 2023-08-06 10:51:32.000000 lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)        1 2023-08-06 10:51:32.000000 lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 yeoshuheng   (501) staff       (20)       14 2023-08-06 10:51:32.000000 lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.5.1/LICENSE` & `lc-checkpoint-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.5.1/PKG-INFO` & `lc-checkpoint-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -141,14 +141,17 @@
 ### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
 ### `lc.restore_model(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name)`
 Loads the compressed data into a pytorch model.
 
+### `lc.restore_model_async(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name, n_cores)`
+Loads the compressed data into a pytorch model asynchronously.
+
 ### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `lc-checkpoint-0.5.1/README.md` & `lc-checkpoint-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,17 @@
 ### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
 ### `lc.restore_model(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name)`
 Loads the compressed data into a pytorch model.
 
+### `lc.restore_model_async(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name, n_cores)`
+Loads the compressed data into a pytorch model asynchronously.
+
 ### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `lc-checkpoint-0.5.1/setup.cfg` & `lc-checkpoint-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lc-checkpoint
-version = 0.5.1
+version = 0.5.2
 author = Dedy Van Hauten
 author_email = dedy.van@ui.ac.id
 description = A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pypi.org/project/lc-checkpoint/
 classifiers =
```

### Comparing `lc-checkpoint-0.5.1/src/lc_checkpoint/main.py` & `lc-checkpoint-0.5.2/src/lc_checkpoint/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import pickle
 import math
 import numpy as np
-import torch.optim as optim
-import torch.nn as nn
+import pathos.multiprocessing as pmp
 import dahuffman
 import torch
 
-__all__ = ['initialize', 'compress_data', 'decode_data', 'restore_model',
+__all__ = ['initialize', 'compress_data', 'decode_data', 'restore_model', 'restore_model_async',
            'save_checkpoint', 'load_checkpoint', 'calculate_compression_rate']
 
 net = None
 optimizer = None
 criterion = None
 checkpoint_dir = None
 num_buckets = None
@@ -127,38 +126,96 @@
     compression_rate = num_elements * math.log(num_buckets, 2) + num_buckets * num_bits
     return compression_rate
 
 def restore_model(init_model, last_epoch, last_iter, max_iter, init_filename, cpt_name = "lc_checkpoint"):
     # Get initial model
     init_model.load_state_dict(torch.load(init_filename))
     deltas = np.concatenate([tensor.numpy().flatten() for tensor in init_model.state_dict().values()])
-
+  
     # Get deltas for last epoch.
     for j in range(last_iter + 1):
+        if last_epoch == 0 and j == 0:
+            continue
         ckpt = cpt_name + "_epoch{}_iter{}.pt".format(last_epoch, j)
         cp, _ = load_checkpoint(ckpt)
         deltas = np.add(deltas,cp)
 
     # Get deltas for previous epochs
-    for e in range(last_epoch - 1):
+    for e in range(max(last_epoch - 1, 0)):
         for j in range(max_iter):
             if e == 0 and j == 0:
                 continue
             ckpt = cpt_name + "_epoch{}_iter{}.pt".format(e, j)
             cp, _ = load_checkpoint(ckpt)
             deltas = np.add(deltas,cp)
 
     # Reshape based on model's state dictionary.
     fin_dict = init_model.state_dict()
     last_idx = 0
+    
     for layer_name, init_tensor in fin_dict.items():
         # Extract appropriate elements
         dim = init_tensor.numpy().shape
+        if dim == ():
+            continue
         t_elements = np.prod(dim)
         needed_ele = deltas[last_idx : last_idx + t_elements]
         last_idx = t_elements # Reset the last index
 
         # Reshape delta and reinsert into the dictionary.
         fin_dict[layer_name] = torch.from_numpy(np.reshape(needed_ele, dim))
-        
+    
+    init_model.load_state_dict(fin_dict)
+    return init_model
+
+def restore_model_async(init_model, last_epoch, last_iter, max_iter, 
+                        init_filename, cpt_name = "lc_checkpoint", 
+                        n_cores = pmp.cpu_count() // 2):
+    
+    # Get initial model
+    init_model.load_state_dict(torch.load(init_filename))
+    deltas = np.concatenate([tensor.numpy().flatten() for tensor in init_model.state_dict().values()])
+    print("Decompression process with {} cores".format(n_cores))
+
+    pool = pmp.ProcessingPool(nodes = n_cores)
+    filenames = []
+
+    # Get deltas for last epoch.
+    for j in range(last_iter + 1):
+        if last_epoch == 0 and j == 0:
+            continue
+        ckpt = cpt_name + "_epoch{}_iter{}.pt".format(last_epoch, j)
+        filenames.append(ckpt)
+
+    # Get deltas for previous epochs
+    for e in range(max(last_epoch - 1, 0)):
+        for j in range(max_iter):
+            if e == 0 and j == 0:
+                continue
+            ckpt = cpt_name + "_epoch{}_iter{}.pt".format(e, j)
+            filenames.append(ckpt)
+    
+    # Async checkpoint decompression
+    with pool:
+        results = pool.amap(lambda x : load_checkpoint(x), 
+                             filenames)
+        for res in results.get():
+            d, _ = res
+            deltas = np.add(deltas, d)
+
+    # Reshape based on model's state dictionary.
+    fin_dict = init_model.state_dict()
+    last_idx = 0
+    for layer_name, init_tensor in fin_dict.items():
+        # Extract appropriate elements
+        dim = init_tensor.numpy().shape
+        if dim == ():
+            continue
+        t_elements = np.prod(dim)
+        needed_ele = deltas[last_idx : last_idx + t_elements]
+        last_idx = t_elements # Reset the last index
+
+        # Reshape delta and reinsert into the dictionary.
+        fin_dict[layer_name] = torch.from_numpy(np.reshape(needed_ele, dim))
+    
     init_model.load_state_dict(fin_dict)
     return init_model
```

### Comparing `lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.5.2/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.5.1
+Version: 0.5.2
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -141,14 +141,17 @@
 ### `lc.load_checkpoint(filename)`
 
 Loads the compressed data from a file with the given filename.
 
 ### `lc.restore_model(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name)`
 Loads the compressed data into a pytorch model.
 
+### `lc.restore_model_async(model, last_epoch, last_iter, max_iter, init_filename, ckpt_name, n_cores)`
+Loads the compressed data into a pytorch model asynchronously.
+
 ### `lc.calculate_compression_rate(prev_state_dict, num_bits=num_bits, num_buckets=num_buckets)`
 
 Calculates the compression rate of the LC-Checkpoint method based on the previous state dictionary and the current number of bits and buckets.
 
 ## License
 
 LC-Checkpoint is licensed under the MIT License. See the LICENSE file for more information.
```

