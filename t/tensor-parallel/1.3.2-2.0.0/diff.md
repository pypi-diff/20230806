# Comparing `tmp/tensor_parallel-1.3.2.tar.gz` & `tmp/tensor_parallel-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.3.2.tar", last modified: Thu Jul 27 12:02:28 2023, max compression
+gzip compressed data, was "tensor_parallel-2.0.0.tar", last modified: Sun Aug  6 14:21:37 2023, max compression
```

## Comparing `tensor_parallel-1.3.2.tar` & `tensor_parallel-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:28.986104 tensor_parallel-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-27 12:02:28.000000 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-27 12:02:28.000000 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:02:28.000000 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-27 12:02:28.000000 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 12:02:28.000000 tensor_parallel-1.3.2/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:28.990104 tensor_parallel-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-27 12:02:19.000000 tensor_parallel-1.3.2/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:21:37.531163 tensor_parallel-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-08-06 14:21:37.531163 tensor_parallel-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-06 14:21:37.531163 tensor_parallel-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:21:37.527162 tensor_parallel-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:21:37.527162 tensor_parallel-2.0.0/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22130 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:21:37.527162 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-08-06 14:21:37.000000 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-06 14:21:37.000000 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:21:37.000000 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-06 14:21:37.000000 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 14:21:37.000000 tensor_parallel-2.0.0/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:21:37.531163 tensor_parallel-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-08-06 14:21:24.000000 tensor_parallel-2.0.0/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.3.2/LICENCE` & `tensor_parallel-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/PKG-INFO` & `tensor_parallel-2.0.0/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tensor_parallel
-Version: 1.3.2
+Name: tensor-parallel
+Version: 2.0.0
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.3.2 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 2.0.0 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.3.2/README.md` & `tensor_parallel-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/setup.cfg` & `tensor_parallel-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.3.2
+version = 2.0.0
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/__init__.py` & `tensor_parallel-2.0.0/src/tensor_parallel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,11 +2,12 @@
 A prototype TensorParallel wrapper that works without torch.distributed.
 Splits linear, conv and some other layers between GPUs
 """
 
 from tensor_parallel.config import Config
 from tensor_parallel.dispatch import convert_state_dict, infer_sharded_device_map, save_tensor_parallel
 from tensor_parallel.factory import tensor_parallel
+from tensor_parallel.legacy import Sharded
 from tensor_parallel.pretrained_model import TensorParallelPreTrainedModel
-from tensor_parallel.sharding import Sharded
+from tensor_parallel.shard import make_distributed_shard
 from tensor_parallel.state_actions import StateAction
 from tensor_parallel.tensor_parallel import TensorParallel
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/autoconfig.py` & `tensor_parallel-2.0.0/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/aux_actions.py` & `tensor_parallel-2.0.0/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/communications.py` & `tensor_parallel-2.0.0/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/config.py` & `tensor_parallel-2.0.0/src/tensor_parallel/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 import logging
 import os
 import re
 from functools import partial
-from typing import Any, Callable, Dict, Sequence, Union
+from itertools import chain
+from typing import Any, Callable, Dict, Iterable, Mapping, Sequence, Union
 
 import torch
 from torch import nn
 
 import tensor_parallel.cross_device_ops as cross_device_ops
 from tensor_parallel.communications import (
     AllGather,
@@ -147,7 +148,44 @@
                             f"Can't apply action {action} since it uses LoRA. The only actions with LoRA support are Split and it's variations."
                         )
 
     config.state_rules.update(lora_state_rules)
     config.input_rules.update(lora_input_rules)
     config.output_rules.update(lora_output_rules)
     return config
+
+
+def get_parameter_name_mapping(names: Iterable[str], tensor_parallel_config: Config) -> Mapping[str, str]:
+    """Maps original model's parameter names to tensor_parallel parameter names.
+
+    Args:
+        names (Iterable[str]): Parameter names
+        tensor_parallel_config (Config): Config
+
+    Returns:
+        Iterable[str]: tensor_parallel parameter names
+    """
+    patterns = tuple(
+        regex.pattern
+        for regex in chain(tensor_parallel_config.input_rules.keys(), tensor_parallel_config.output_rules.keys())
+    )
+    patterns = [pattern[:-1] if pattern.endswith("$") else pattern for pattern in patterns]
+    patterns = set(pattern if pattern.endswith(".") else pattern + r"\." for pattern in patterns)
+    patterns = [re.compile(pattern) for pattern in patterns]
+
+    insertions = {name: [] for name in names}
+    for pattern in patterns:
+        for name in names:
+            match = pattern.search(name)
+            if match is not None:
+                end_pos = match.span()[1]
+                insertions[name].append(end_pos)
+    insertions = {name: sorted(pos) for name, pos in insertions.items()}
+
+    name_replacements = {}
+    for name in names:
+        new_name = name
+        for pos in insertions[name][::-1]:
+            new_name = new_name[:pos] + r"tp_wrapped_module." + new_name[pos:]
+        name_replacements[name] = new_name
+
+    return name_replacements
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-2.0.0/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/dispatch.py` & `tensor_parallel-2.0.0/src/tensor_parallel/dispatch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import re
 from contextlib import contextmanager
-from itertools import chain
 from typing import Union
 
 import torch
 
+from tensor_parallel.config import get_parameter_name_mapping
 from tensor_parallel.pretrained_model import TensorParallelPreTrainedModel
-from tensor_parallel.sharding import Sharded
 from tensor_parallel.tensor_parallel import Config, TensorParallel
 from tensor_parallel.utils import find_tied_weight_aliases
 
 
 @contextmanager
-def save_tensor_parallel(model: Union[TensorParallel, TensorParallelPreTrainedModel, Sharded]):
+def save_tensor_parallel(model: Union[TensorParallel, TensorParallelPreTrainedModel]):
     """Enables state_dict reconstruction for tensor_parallel models.
     With it '.state_dict()' produces a state dict that can be loaded into an underlying model.
     Example:
     ```python
     model = <some model>
     model_tp = tensor_parallel(model)
     with save_tensor_parallel(model_tp):
         model.load_state_dict(model_tp.state_dict()) # state dicts match
     ```
 
     Args:
-        model (Union[TensorParallel, TensorParallelPreTrainedModel, Sharded]): tensor_parallel model
+        model (Union[TensorParallel, TensorParallelPreTrainedModel]): tensor_parallel model
     """
-    model.preserve_shards_when_saving = False
+    model.set_preserve_shards_when_saving(False)
     try:
         yield
     finally:
-        model.preserve_shards_when_saving = True
+        model.set_preserve_shards_when_saving(True)
 
 
 def infer_sharded_data_device_id(name: str):
     if name.find("_sanity_check_params.") != -1:
         shard_id_start = name.find("_sanity_check_params.") + len("_sanity_check_params.")
     elif name.find("module_shards.") != -1:
         shard_id_start = name.find("module_shards.") + len("module_shards.")
@@ -108,29 +107,15 @@
                 output_state_dict[name] = action(state, rank=rank)
                 break
         else:
             output_state_dict[name] = input_state_dict[name]  # copy source parameter as is
 
 
 def convert_names(state_dict, tensor_parallel_config: Config):
-    patterns = tuple(
-        regex.pattern
-        for regex in chain(tensor_parallel_config.input_rules.keys(), tensor_parallel_config.output_rules.keys())
-    )
-    patterns = set(pattern[:-1] + "\." if pattern.endswith("$") else pattern for pattern in patterns)
-    patterns = [re.compile(pattern) for pattern in patterns]
-
-    name_replacements = {name: name for name in state_dict.keys()}
-    for pattern in patterns:
-        for initial_name, old_name in name_replacements.items():
-            match = pattern.search(old_name)
-            if match is not None:
-                end_pos = match.span()[1]
-                new_name = old_name[:end_pos] + "tp_wrapped_module." + old_name[end_pos:]
-                name_replacements[initial_name] = new_name
+    name_replacements = get_parameter_name_mapping(state_dict.keys(), tensor_parallel_config)
 
     for initial_name, final_name in name_replacements.items():
         state_dict[final_name] = state_dict.pop(initial_name)
 
 
 def prefix_names_with_shard_id(state_dict, rank: int):
     name_replacements = {name: f"module_shards.{rank}." + name for name in state_dict.keys()}
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-2.0.0/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-2.0.0/src/tensor_parallel/pretrained_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import torch
 from torch import nn
 from transformers import PretrainedConfig, PreTrainedModel
 
 from tensor_parallel.config import TENSOR_PARALLEL_USE_NATIVE, Config
 from tensor_parallel.per_device_tensors import PerDeviceTensors
-from tensor_parallel.sharding import Sharded
 from tensor_parallel.slicing_configs import PREDEFINED_CONFIGS
 from tensor_parallel.tensor_parallel import TensorParallel, check_device_ids, parallel_apply, parallel_apply_simple
 from tensor_parallel.utils import nested_map
 
 logger = logging.getLogger(__file__)
 
 
@@ -39,45 +38,43 @@
     def __init__(
         self,
         module: PreTrainedModel,
         device_ids: Optional[Sequence[torch.device]] = None,
         output_device: Optional[torch.device] = None,
         output_device_index: Optional[int] = None,
         tensor_parallel_config: Optional[Config] = None,
-        distributed: bool = True,
+        **kwargs,
     ):
         super().__init__(module.config)  # Temporary empty config. Gets replaced in from_pretrained
 
         if hasattr(module, "_hf_hook"):
             from accelerate.hooks import remove_hook_from_module
 
             remove_hook_from_module(module, recurse=True)
 
         if tensor_parallel_config is None:
             tensor_parallel_config = find_predefined_tensor_parallel_config(module.config, device_ids)
 
         self.wrapped_model = TensorParallel(
-            module, device_ids, output_device, output_device_index, tensor_parallel_config, distributed=distributed
+            module, device_ids, output_device, output_device_index, tensor_parallel_config, **kwargs
         )
 
     @property
     def devices(self):
         return self.wrapped_model.devices
 
     @property
     def tensor_parallel_config(self):
         return self.wrapped_model.tensor_parallel_config
 
-    @property
-    def preserve_shards_when_saving(self):
-        return self.wrapped_model.preserve_shards_when_saving
+    def set_preserve_shards_when_saving(self, value: bool):
+        self.wrapped_model.set_preserve_shards_when_saving(value)
 
-    @preserve_shards_when_saving.setter
-    def preserve_shards_when_saving(self, value):
-        self.wrapped_model.preserve_shards_when_saving = value
+    def apply_sharding(self, *args, **kwargs):
+        self.wrapped_model.apply_sharding(*args, **kwargs)
 
     def forward(self, *args, **kwargs):
         return self.wrapped_model(*args, **kwargs)
 
     def state_dict(self, *args, **kwargs):
         state_dict = super().state_dict(*args, **kwargs)
         if self.wrapped_model.preserve_shards_when_saving:
@@ -119,74 +116,47 @@
         if len(self.wrapped_model.module_shards) == 1:
             return self.wrapped_model.module_shards[0].get_encoder()
 
         encoder_shards = [
             encoder_decoder_shard.get_encoder() for encoder_decoder_shard in self.wrapped_model.module_shards
         ]
 
-        encoder_wrapper_class = None
-        if isinstance(self.wrapped_model, TensorParallel):
+        class _EncoderWrapper(torch.nn.Module):
+            def __init__(self, wrapped_pretrained_model: TensorParallelPreTrainedModel) -> None:
+                super().__init__()
+                self.wrapped_pretrained_model = wrapped_pretrained_model
+
+            def forward(self, *args, **kwargs):
+                if self.wrapped_pretrained_model.wrapped_model.need_delayed_init:
+                    for shard, device in zip(
+                        self.wrapped_pretrained_model.wrapped_model.module_shards,
+                        self.wrapped_pretrained_model.wrapped_model.devices,
+                    ):
+                        shard.to(device)
+                    self.wrapped_pretrained_model.wrapped_model.need_delayed_init = False
 
-            class _EncoderWrapper(torch.nn.Module):
-                def __init__(self, wrapped_pretrained_model: TensorParallelPreTrainedModel) -> None:
-                    super().__init__()
-                    self.wrapped_pretrained_model = wrapped_pretrained_model
+                # Synchronize sharded parameters
+                if self.wrapped_pretrained_model.wrapped_model.sharding_manager is not None:
+                    self.wrapped_pretrained_model.wrapped_model.sharding_manager.synchronize_weights(
+                        self.wrapped_pretrained_model.wrapped_model.all_cuda
+                    )
 
-                def forward(self, *args, **kwargs):
-                    (
+                (
+                    inputs,
+                    kwargs_tup,
+                ) = self.wrapped_pretrained_model.wrapped_model.prepare_args_kwargs_for_forward(*args, **kwargs)
+                if self.wrapped_pretrained_model.wrapped_model.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
+                    return parallel_apply(
+                        encoder_shards,
                         inputs,
                         kwargs_tup,
-                    ) = self.wrapped_pretrained_model.wrapped_model.prepare_args_kwargs_for_forward(*args, **kwargs)
-                    if self.wrapped_pretrained_model.wrapped_model.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
-                        return parallel_apply(
-                            encoder_shards,
-                            inputs,
-                            kwargs_tup,
-                            self.wrapped_pretrained_model.wrapped_model.devices,
-                        )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
-                    else:
-                        return parallel_apply_simple(
-                            encoder_shards,
-                            inputs,
-                            kwargs_tup,
-                            self.wrapped_pretrained_model.wrapped_model.devices,
-                        )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
-
-            encoder_wrapper_class = _EncoderWrapper
-
-        elif isinstance(self.wrapped_model, Sharded):
-
-            class _EncoderWrapper(torch.nn.Module):
-                def __init__(self, wrapped_pretrained_model: TensorParallelPreTrainedModel) -> None:
-                    super().__init__()
-                    self.wrapped_pretrained_model = wrapped_pretrained_model
-
-                def forward(self, *args, **kwargs):
-                    if (
-                        len(self.wrapped_pretrained_model.wrapped_model.module.module_shards) > 1
-                        and len(self.wrapped_pretrained_model.wrapped_model.sharded_param_names) > 0
-                    ):
-                        self.wrapped_pretrained_model.wrapped_model._maybe_fill_sharded_params()
-                    (
+                        self.wrapped_pretrained_model.wrapped_model.devices,
+                    )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
+                else:
+                    return parallel_apply_simple(
+                        encoder_shards,
                         inputs,
                         kwargs_tup,
-                    ) = self.wrapped_pretrained_model.wrapped_model.module.prepare_args_kwargs_for_forward(
-                        *args, **kwargs
-                    )
-                    if self.wrapped_pretrained_model.wrapped_model.module.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
-                        return parallel_apply(
-                            encoder_shards,
-                            inputs,
-                            kwargs_tup,
-                            self.wrapped_pretrained_model.wrapped_model.module.devices,
-                        )[self.wrapped_pretrained_model.wrapped_model.module.output_device_index]
-                    else:
-                        return parallel_apply_simple(
-                            encoder_shards,
-                            inputs,
-                            kwargs_tup,
-                            self.wrapped_pretrained_model.wrapped_model.module.devices,
-                        )[self.wrapped_pretrained_model.wrapped_model.module.output_device_index]
-
-            encoder_wrapper_class = _EncoderWrapper
+                        self.wrapped_pretrained_model.wrapped_model.devices,
+                    )[self.wrapped_pretrained_model.wrapped_model.output_device_index]
 
-        return encoder_wrapper_class(self)
+        return _EncoderWrapper(self)
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/shard.py` & `tensor_parallel-2.0.0/src/tensor_parallel/shard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 import logging
 from copy import deepcopy
 from itertools import chain
-from typing import Dict, Optional
+from typing import Collection, Dict, Optional, Tuple
 
 import torch
 from torch import nn
 
 from tensor_parallel.autoconfig import get_default_config
-from tensor_parallel.config import Config, MappedActions, ModuleRules
+from tensor_parallel.config import Config, MappedActions, ModuleRules, get_parameter_name_mapping
 from tensor_parallel.wrapper import TensorParallelWrapper
 
 logger = logging.getLogger(__file__)
 
 
-def make_shard(module: nn.Module, device: torch.device, config: Config, *, rank: int, world_size: int) -> nn.Module:
-    """Apply a tensor-parallel config to a high-level module, return module shard for a given rank and device"""
+def make_shard(
+    module: nn.Module, device: torch.device, config: Config, *, rank: int, world_size: int
+) -> Tuple[nn.Module, Collection[str]]:
+    """Apply a tensor-parallel config to a high-level module, return module shard for a given rank and device
+
+    Args:
+        module (nn.Module): Module to make a shard of
+        device (torch.device): Device, on which to put shard
+        config (Config): Config to create shard by
+        rank (int): Rank of the shard
+        world_size (int): Total number of shards
+
+    Returns:
+        Tuple[nn.Module, Collection[str]]: Shard and a set of modified parameter names after modification
+    """
     assert (
         len(list(module.children())) != 0
     ), "Please ensure module is a container (e.g. Sequential), not a single layer"
     source_tensors = dict(chain(module.named_parameters(), module.named_buffers()))
     substitutes = {
         id(x): nn.Parameter(
             torch.empty(
@@ -36,15 +49,15 @@
         for x in source_tensors.values()
     }
     shard = deepcopy(module, memo=substitutes)
     # ^-- note: the memo=... above will replace all parameters and buffers with empty tensors
     del module, substitutes
 
     # convert parameters and buffers
-    process_state_(shard, source_tensors, config, rank=rank, world_size=world_size)
+    modified_parameter_names = process_state_(shard, source_tensors, config, rank=rank, world_size=world_size)
     del source_tensors
 
     # convert or wrap intermediate modules
     unique_wrappers = {}
     with torch.no_grad():
         for name, submodule in shard.named_modules():
             if submodule in unique_wrappers:
@@ -57,16 +70,19 @@
         for child_name, child in list(parent.named_children()):
             if child in unique_wrappers:
                 setattr(parent, child_name, unique_wrappers[child])
 
     # automatically fixes certain submodule attributes such that
     # it's not necessary to specify in a config
     fix_general_attributes(shard)
+    shard = unique_wrappers.get(shard, shard)  # wrap the root module if needed
 
-    return unique_wrappers.get(shard, shard)  # wrap the root module if needed
+    modified_parameter_names = set(get_parameter_name_mapping(modified_parameter_names, config).values())
+
+    return shard, modified_parameter_names
 
 
 def make_distributed_shard(module: nn.Module, device: torch.device, config: Optional[Config] = None):
     if config is None:
         config = get_default_config(module, device_ids=range(torch.distributed.get_world_size()))
         logger.info("Using automatic config: sharding individual linear/conv/emb layers")
 
@@ -112,36 +128,47 @@
                 found_actions[key] = action
     return found_actions
 
 
 @torch.no_grad()
 def process_state_(
     sharded_module: nn.Module, source_tensors: Dict[str, torch.Tensor], config: Config, *, rank: int, world_size: int
-):
-    """
-    Initialize sharded_module's parameters and buffers by applying prescribed rules to source_module's buffers
-    :param sharded_module: target module that will be modified in-place
-    :param source_tensors: original parameters and buffers on a source device
+) -> Collection[str]:
+    """Initialize sharded_module's parameters and buffers by applying prescribed rules to source_module's buffers
+
+    Args:
+        sharded_module (nn.Module): target module that will be modified in-place
+        source_tensors (Dict[str, torch.Tensor]): original parameters and buffers on a source device
+        config (Config): config to split by
+        rank (int): shard rank
+        world_size (int): number of shards
+
+    Returns:
+        Collection[str]: set of parameter/buffer names modified
     """
+    modified_parameter_names = set()
     unused_patterns = set(config.state_rules.keys())
     for name, state in chain(sharded_module.named_parameters(), sharded_module.named_buffers()):
         for pattern, action in config.state_rules.items():
             if pattern.search(name) is not None:
                 new_data = action(source_tensors[name], rank=rank)
+                modified_parameter_names.add(name)
                 unused_patterns.discard(pattern)
                 break
         else:
             new_data = source_tensors[name]  # copy source parameter as is
 
         state.data = new_data.clone().detach().to(state.device).requires_grad_(state.requires_grad)
         # note: .clone is required so that the resulting parameter owns its storage
 
     if unused_patterns:
         logger.warning(f"The following patterns in state_rules were unused: {[str(p) for p in unused_patterns]}")
 
+    return modified_parameter_names
+
 
 def process_attrs_(module: nn.Module, actions: MappedActions, rank: int, world_size: int):
     """Modify module properties in-place"""
     assert not getattr(module, "__tensor_parallel_process_attrs", False), "process_attrs was called more than once"
     for attr, action in actions.items():
         setattr(module, attr, action(getattr(module, attr), rank=rank))
     module.__tensor_parallel_process_attrs = True
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-2.0.0/src/tensor_parallel/slicing_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         input_rules={
             r".*[0-9]\.attn$": {"layer_past": select_kv_for_rank},
             r".*lm_head$": {0: "split -1"},  # note: we need to split lm_head inputs because
             # ... lm_head's weights (tied embeddings) are already split across input dimension
         },
         output_rules={
             r".*[0-9]\.attn$": {0: "sum", 1: gather_kv_across_ranks},
-            r".*mlp$$": {0: "sum"},
+            r".*mlp$": {0: "sum"},
             r".*wte$": {0: "gather -1"},
             r".*wpe$": {0: "gather -1"},
             r".*lm_head$": {0: "sum"},
         },
         attr_rules={
             r".*attn\.c_attn$": {
                 "nf": partial(split_inner_dim, num_heads=num_heads, world_size=world_size),
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/state_actions.py` & `tensor_parallel-2.0.0/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-2.0.0/src/tensor_parallel/tensor_parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 The main TensorParallel module wrapper
 """
 import logging
 import threading
 from contextlib import nullcontext
-from typing import Any, Optional, Sequence, Union
+from operator import attrgetter
+from typing import Any, Collection, Optional, Sequence, Union
 
 import torch
 from torch import nn
 from torch._utils import ExceptionWrapper, _get_all_device_indices, _get_device_index
 from torch.cuda.amp import autocast
 from torch.nn.parallel import parallel_apply
 
 from tensor_parallel.autoconfig import get_default_config
 from tensor_parallel.config import TENSOR_PARALLEL_USE_NATIVE, Config, add_lora_rules
 from tensor_parallel.cross_device_ops import broadcast_coalesced
 from tensor_parallel.shard import make_shard
+from tensor_parallel.sharding import Sharded
 from tensor_parallel.utils import nested_flatten, nested_pack
 
 logger = logging.getLogger(__file__)
 
 
 class TensorParallel(nn.Module):
     def __init__(
@@ -27,14 +29,16 @@
         module: nn.Module,
         device_ids: Optional[Sequence[torch.device]] = None,
         output_device: Optional[torch.device] = None,
         output_device_index: Optional[int] = None,
         tensor_parallel_config: Optional[Config] = None,
         delay_init: bool = False,
         distributed: bool = True,
+        sharded: bool = True,
+        sharded_param_names: Optional[Collection[str]] = None,
     ):
         super().__init__()
         original_params = sum(p.numel() for p in module.parameters())
         assert output_device is None or output_device_index is None, "please specify either device or index, not both"
         device_ids = check_device_ids(device_ids)
 
         if output_device is not None:
@@ -49,14 +53,15 @@
 
         self.devices = device_ids
         self.output_device_index = output_device_index
         self.all_cuda = all(device.type == "cuda" for device in self.devices)
         self.device_ids = [_get_device_index(x, optional=True, allow_cpu=True) for x in device_ids]
         self.need_delayed_init = delay_init
         world_size = len(self.devices)
+        self.sharding_manager = None
 
         if len(device_ids) <= 1:
             self.module_shards.append(module)
             if len(device_ids) == 1 and not delay_init:
                 self.module_shards[0].to(device_ids[0])
             return
 
@@ -66,18 +71,23 @@
 
         tensor_parallel_config = add_lora_rules(module, tensor_parallel_config)
         self.tensor_parallel_config = tensor_parallel_config
 
         config_with_ops = tensor_parallel_config.create_collective_ops(self.devices, distributed)
         # ^-- creates a copy of comfig with collective op instances, such as AllReduce and AllGather
 
+        self.modified_parameters_names = set()
         for rank, device in enumerate(self.devices):
             if delay_init:
                 device = torch.device("cpu")
-            self.module_shards.append(make_shard(module, device, config_with_ops, rank=rank, world_size=world_size))
+            shard, modified_parameters_names = make_shard(
+                module, device, config_with_ops, rank=rank, world_size=world_size
+            )
+            self.module_shards.append(shard)
+            self.modified_parameters_names.update(modified_parameters_names)
 
         # self-diagnostics: check if the model was sharded properly
 
         params_per_shard = [sum(p.numel() for p in shard.parameters()) for shard in self.module_shards]
         assert sum(params_per_shard) >= original_params, "Internal assert failed: lost some parameters during sharding"
         self.param_fractions = tuple(params_i / original_params for params_i in params_per_shard)
         inefficiency_rate = (sum(self.param_fractions) - 1) / len(device_ids)  # extra params rate per GPU
@@ -90,14 +100,28 @@
 
         # more self-diagnostics: make sure that the model was not cast .to one device
         self._sanity_check_params = nn.ParameterList(
             [nn.Parameter(torch.empty(0, device=device), requires_grad=False) for device in self.devices]
         )
         self.preserve_shards_when_saving: bool = True
 
+        if sharded:
+            self.apply_sharding(sharded_param_names)
+
+    def apply_sharding(
+        self,
+        replicated_param_names: Optional[Collection[str]] = None,
+    ):
+        if self.sharding_manager is not None:
+            raise Exception(
+                "Trying to apply sharding for the second time. If you wish NOT to apply sharding during model initialization, pass `sharded=False`."
+            )
+        else:
+            self.sharding_manager = Sharded(self, len(self.devices), replicated_param_names)
+
     def prepare_args_kwargs_for_forward(self, *args, **kwargs):
         args_and_kwargs = (args, kwargs)
         flat_tensors = [obj for obj in nested_flatten(args_and_kwargs) if isinstance(obj, torch.Tensor)]
         flat_tensors_replicated = broadcast_coalesced(flat_tensors, self.devices, all_cuda=self.all_cuda)
         next_tensor_index = 0
         args_and_kwargs_replicated = [list() for _ in self.device_ids]
         for obj in nested_flatten(args_and_kwargs):
@@ -114,48 +138,60 @@
 
     def forward(self, *args, **kwargs):
         if self.need_delayed_init:
             for shard, device in zip(self.module_shards, self.devices):
                 shard.to(device)
             self.need_delayed_init = False
 
+        # Synchronize replicated parameters
+        if self.sharding_manager is not None:
+            self.sharding_manager.synchronize_weights(self.all_cuda)
+
         if len(self.module_shards) <= 1:
             return [self.module_shards[0](*args, **kwargs)][self.output_device_index]
 
         if not all(p.device == d for p, d in zip(self._sanity_check_params, self.devices)):
             raise ValueError(
                 "Model parameters were moved to incorrect devices, did call on model.cuda() or "
                 "model.to(device)? If so, please avoid doing that"
             )
         inputs, kwargs_tup = self.prepare_args_kwargs_for_forward(*args, **kwargs)
         if self.all_cuda and not TENSOR_PARALLEL_USE_NATIVE:
             return parallel_apply(self.module_shards, inputs, kwargs_tup, self.devices)[self.output_device_index]
         else:
             return parallel_apply_simple(self.module_shards, inputs, kwargs_tup, self.devices)[self.output_device_index]
 
+    def set_preserve_shards_when_saving(self, value: bool):
+        self.preserve_shards_when_saving = value
+        if self.sharding_manager is not None:
+            self.sharding_manager.preserve_shards_when_saving = value
+
     def state_dict(self, *args, **kwargs):
         state_dict = super().state_dict(*args, **kwargs)
+
         if self.preserve_shards_when_saving:
             return state_dict
 
         for i in range(len(self.module_shards)):
             sanity_check_param_name = next(
                 name for name, _ in state_dict.items() if name.endswith(f"_sanity_check_params.{i}")
             )
             del state_dict[sanity_check_param_name]
 
-        # fix names for zero-3'ed params that were inside _TensorParallelWrapper
+        # fix names for sharded params that were inside _TensorParallelWrapper
         names_inside_tp_wrapper = [name for name in state_dict.keys() if "tp_wrapped_module." in name]
         for name in names_inside_tp_wrapper:
             state_dict[name.replace("tp_wrapped_module.", "")] = state_dict.pop(name)
 
         try:
             shards_prefix = next(name for name, _ in state_dict.items() if "module_shards." in name)
         except StopIteration:
-            return state_dict  # no parameters are actually tensor parallel
+            return self.process_sharded_state_dict(
+                state_dict, kwargs.get("prefix", "")
+            )  # no parameters are actually tensor parallel
         shards_prefix = shards_prefix[: shards_prefix.find("module_shards.") + len("module_shards.")]
         module_prefix = shards_prefix[: -len("module_shards.")]
 
         # get names for desired tensors and where to find them (shards of zero-3)
         is_name_prefixed = {}
         for name, tensor in state_dict.items():
             if name.startswith(shards_prefix + "0."):  # dict entry is from shards
@@ -177,15 +213,29 @@
                     tensor for name, tensor in state_dict.items() if name.endswith(unsharded_name)
                 )
             if is_prefixed:
                 # delete sharded tensor entries
                 for i in range(len(self.module_shards)):
                     del state_dict[f"{shards_prefix}{i}.{unsharded_name}"]
 
-        return state_dict
+        # processing Sharded
+        return self.process_sharded_state_dict(state_dict, kwargs.get("prefix", ""))
+
+    def process_sharded_state_dict(self, destination, prefix):
+        if self.sharding_manager is not None:
+            self.sharding_manager.synchronize_weights(self.all_cuda)
+            for name in self.sharding_manager.sharded_param_names:
+                for shard in self.module_shards:
+                    try:
+                        destination[prefix + name] = attrgetter(name)(shard)
+                        break
+                    except KeyError:
+                        pass
+
+        return destination
 
 
 def parallel_apply_simple(
     modules: Sequence[nn.Module],
     inputs: Sequence[Sequence[torch.Tensor]],
     kwargs_tup: Optional[Any],
     devices: Sequence[torch.device],
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/utils.py` & `tensor_parallel-2.0.0/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel/wrapper.py` & `tensor_parallel-2.0.0/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tensor-parallel
-Version: 1.3.2
+Name: tensor_parallel
+Version: 2.0.0
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.3.2 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 2.0.0 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.3.2/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-2.0.0/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/tensor_parallel/aux_actions.py
 src/tensor_parallel/communications.py
 src/tensor_parallel/config.py
 src/tensor_parallel/cross_device_ops.py
 src/tensor_parallel/dispatch.py
 src/tensor_parallel/factory.py
 src/tensor_parallel/imports.py
+src/tensor_parallel/legacy.py
 src/tensor_parallel/per_device_tensors.py
 src/tensor_parallel/pretrained_model.py
 src/tensor_parallel/shard.py
 src/tensor_parallel/sharding.py
 src/tensor_parallel/slicing_configs.py
 src/tensor_parallel/state_actions.py
 src/tensor_parallel/tensor_parallel.py
```

### Comparing `tensor_parallel-1.3.2/tests/test_basic.py` & `tensor_parallel-2.0.0/tests/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,41 @@
 
 import pytest
 import torch
 import torch.nn as nn
 from torch.nn.modules.conv import _ConvTransposeNd
 
 import tensor_parallel
-from tensor_parallel import Config, Sharded, TensorParallel
+from tensor_parallel import Config, TensorParallel
 
 
 @pytest.mark.parametrize("emb_cls", [nn.Embedding, nn.EmbeddingBag])
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu", "cpu"), ("cpu", "cpu", "cpu")])
 def test_basic_attributes(emb_cls, devices):
     model_tp = TensorParallel(
         nn.Sequential(
             emb_cls(num_embeddings=1337, embedding_dim=64),
             nn.LayerNorm(64),
             nn.Linear(64, 128),
             nn.ReLU(),
             nn.Linear(128, 10),
         ),
         device_ids=devices,
+        sharded=False,
     )
 
     for name, module in model_tp.named_modules():
         if isinstance(module, nn.Linear):
             assert module.weight.shape == (module.out_features, module.in_features), f"For module {name}"
 
 
 @pytest.mark.parametrize("emb_cls", [nn.Embedding, nn.EmbeddingBag])
+@pytest.mark.parametrize("sharded", [False, True])
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu", "cpu"), ("cpu", "cpu", "cpu")])
-def test_embeds_and_linear(emb_cls, devices):
+def test_embeds_and_linear(emb_cls, sharded, devices):
     torch.manual_seed(0)
 
     model = nn.Sequential(
         emb_cls(num_embeddings=1337, embedding_dim=64),
         nn.LayerNorm(64),
         nn.Linear(64, 128),
         nn.ReLU(),
@@ -42,25 +44,26 @@
     )
 
     inputs = torch.randint(1, 1000, size=(1, 10))
     ref_out = model(inputs)
     ref_out.norm().backward()
 
     model_tp = deepcopy(model)  # deepcopy to avoid accidental grad spillage and false positives
-    model_tp = TensorParallel(model_tp, device_ids=devices)
+    model_tp = TensorParallel(model_tp, device_ids=devices, sharded=sharded)
     out_ours = model_tp(inputs)
     out_ours.norm().backward()
     torch.testing.assert_close(ref_out, out_ours, atol=1e-6, rtol=1e-05)
     our_grad = torch.cat([next(shard[0].parameters()).grad for shard in model_tp.module_shards], dim=1)
     torch.testing.assert_close(model[0].weight.grad, our_grad, atol=1e-6, rtol=1e-05)
 
 
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu",) * 2, ("cpu",) * 3, ("cpu",) * 4])
+@pytest.mark.parametrize("sharded", [False, True])
 @pytest.mark.parametrize("extra_options", [{}, {"padding": "same"}, {"stride": 2}, {"dilation": 2}, {"groups": 2}])
-def test_convs(devices, extra_options):
+def test_convs(devices, sharded, extra_options):
     torch.manual_seed(0)
 
     batchnorm_cls = (None, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d)
     # ^-- note: batchnorms test that tensor_parallel handles buffers (non-parameter state tensors) correctly
     for Conv, nd in (
         (nn.Conv1d, 1),
         (nn.Conv2d, 2),
@@ -79,15 +82,15 @@
         )
         inputs1 = torch.randn(3, 32, *[10 for _ in range(nd)], requires_grad=True)
         inputs2 = inputs1.detach().clone().requires_grad_(True)
         ref_out = model(inputs1)
         ref_out.norm().backward()
 
         model_tp = deepcopy(model)  # deepcopy to avoid accidental grad spillage and false positives
-        model_tp = TensorParallel(model_tp, device_ids=devices)
+        model_tp = TensorParallel(model_tp, device_ids=devices, sharded=sharded)
         out_ours = model_tp(inputs2)
         out_ours.norm().backward()
         torch.testing.assert_close(
             ref_out,
             out_ours,
             atol=1e-6,
             rtol=1e-3,
@@ -100,15 +103,15 @@
             rtol=1e-05,
             msg=lambda msg: f"{msg}\n where Conv is {Conv} with extra_options {extra_options}",
         )
 
 
 @pytest.mark.parametrize("emb_cls", [nn.Embedding, nn.EmbeddingBag])
 @pytest.mark.parametrize("devices", [None, ("cpu",), ("cpu", "cpu"), ("cpu", "cpu", "cpu")])
-def test_sharding(emb_cls, devices):
+def test_sharded_num_params(emb_cls, devices):
     torch.manual_seed(0)
 
     model = nn.Sequential(
         emb_cls(num_embeddings=1337, embedding_dim=64),
         nn.LayerNorm(64),
         nn.Linear(64, 128),
         nn.ReLU(),
@@ -117,30 +120,24 @@
     num_params_original = sum(p.numel() for p in model.parameters())
 
     inputs = torch.randint(1, 1000, size=(1, 10))
     ref_out = model(inputs)
     ref_out.norm().backward()
 
     model_tp = deepcopy(model)  # deepcopy to avoid accidental grad spillage and false positives
-    model_tp = TensorParallel(model_tp, device_ids=devices)
+    model_tp = TensorParallel(model_tp, device_ids=devices, sharded=False)
     world_size = len(model_tp.module_shards)
     num_params_tp = sum(p.numel() for p in model_tp.parameters())
-    model_tp = Sharded(model_tp)
+    model_tp.apply_sharding()
     num_params_sharded = sum(p.numel() for p in model_tp.parameters())
     assert num_params_sharded < num_params_tp or world_size == 1
 
     padding_params = 0 if world_size < 3 else 4
     assert num_params_sharded == num_params_original + padding_params
 
-    out_ours = model_tp(inputs)
-    out_ours.norm().backward()
-    torch.testing.assert_close(ref_out, out_ours, atol=1e-6, rtol=1e-05)
-    our_grad = torch.cat([next(shard[0].parameters()).grad for shard in model_tp.module.module_shards], dim=1)
-    torch.testing.assert_close(model[0].weight.grad, our_grad, atol=1e-6, rtol=1e-05)
-
 
 @pytest.mark.parametrize("devices", [("cpu", "cpu"), ("cpu", "cpu", "cpu")])
 def test_config_backward_compatibility(devices):
     class Module(nn.Module):
         def __init__(self):
             super().__init__()
             self.linear = nn.Linear(10, 10, bias=False)
```

### Comparing `tensor_parallel-1.3.2/tests/test_factory.py` & `tensor_parallel-2.0.0/tests/test_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         nn.Linear(64, 128),
         nn.ReLU(),
         nn.Linear(128, 10),
     )
 
     assert isinstance(model, nn.Module)
     model = tensor_parallel(model, device_ids=["cpu", "cpu"], sharded=sharded)
-    assert isinstance(model, TensorParallel) if not sharded else isinstance(model.module, TensorParallel)
+    assert isinstance(model, TensorParallel)
+    assert (model.sharding_manager is None) != sharded
 
 
 def test_factory_pretrainedmodel():
     devices = ["cpu", "cpu"]
     model_name = "bigscience/bloom-560m"
     model = transformers.AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
```

### Comparing `tensor_parallel-1.3.2/tests/test_integration.py` & `tensor_parallel-2.0.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.2/tests/test_saving.py` & `tensor_parallel-2.0.0/tests/test_saving.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import pytest
 import torch
 from accelerate import init_empty_weights, load_checkpoint_in_model
+from accelerate.utils import set_module_tensor_to_device
 from transformers import AutoConfig, AutoModel
 
 from tensor_parallel import (
     Config,
-    Sharded,
     TensorParallel,
     TensorParallelPreTrainedModel,
     convert_state_dict,
     infer_sharded_device_map,
     save_tensor_parallel,
-    tensor_parallel,
 )
-from tensor_parallel.pretrained_model import find_predefined_tensor_parallel_config
 
 PATH_TO_SAVE = "/tmp/"
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_no_parallelism_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
+    model = AutoModel.from_pretrained(model_name).to(devices[0])
     model_state_dict = model.state_dict()
-    model_tp = Sharded(
-        TensorParallel(model, devices, tensor_parallel_config=Config({}, {}, {}, {}))
+    model_tp = TensorParallel(
+        model, devices, tensor_parallel_config=Config({}, {}, {}, {}), sharded=True
     )  # zero-3 sharding only
     del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
     del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
@@ -41,17 +39,17 @@
 
         torch.testing.assert_close(data, data_tp)
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased", "gpt2", "hf-internal-testing/tiny-random-t5"])
 def test_parallelism_no_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
+    model = AutoModel.from_pretrained(model_name).to(devices[0])
     model_state_dict = model.state_dict()
-    model_tp = TensorParallelPreTrainedModel(model, devices)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=False)
     del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
     del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
 
@@ -63,17 +61,17 @@
 
         torch.testing.assert_close(data, data_tp)
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
 def test_parallelism_zero_3(devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
+    model = AutoModel.from_pretrained(model_name).to(devices[0])
     model_state_dict = model.state_dict()
-    model_tp = tensor_parallel(model, devices, sharded=True)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=True)
     del model
     with save_tensor_parallel(model_tp):
         model_tp_state_dict = model_tp.state_dict()
     del model_tp
 
     assert sorted(list(model_state_dict.keys())) == sorted(list(model_tp_state_dict.keys()))
 
@@ -84,101 +82,88 @@
         assert data.shape == data_tp.shape, name
 
         torch.testing.assert_close(data, data_tp, msg=lambda msg: f"{name}:\n{msg}")
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize(
-    "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-bloom"]
+    "model_name",
+    ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-BloomModel"],
 )
 @pytest.mark.parametrize("shard_as_pretrained", [True, False])
 def test_save_keep_shards(devices, model_name, shard_as_pretrained):
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
+    model = AutoModel.from_pretrained(model_name).to(devices[0])
     if shard_as_pretrained:
         model_tp = TensorParallelPreTrainedModel(model, devices)
     else:
         model_tp = TensorParallel(model, devices)
 
     model_tp.load_state_dict(model_tp.state_dict())
 
 
-def get_tensor_parallel(model: torch.nn.Module, devices, pretrained: bool, zero3: bool):
+def get_tensor_parallel(model: torch.nn.Module, devices, pretrained: bool, sharded: bool):
     if pretrained:
-        model_tp = TensorParallelPreTrainedModel(model, devices)
-        if zero3:
-            model_tp.wrapped_model = Sharded(model_tp.wrapped_model)
+        return TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     else:
-        model_tp = TensorParallel(model, devices)
-        if zero3:
-            model_tp = Sharded(model_tp)
-    return model_tp
+        return TensorParallel(model, devices, sharded=sharded)
 
 
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
-@pytest.mark.parametrize(
-    "model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-t5", "hf-internal-testing/tiny-random-bloom"]
-)
+@pytest.mark.parametrize("model_name", ["bert-base-uncased", "hf-internal-testing/tiny-random-BloomModel"])
 @pytest.mark.parametrize("pretrained", [True, False])
-@pytest.mark.parametrize("zero3", [True, False])
-@pytest.mark.parametrize("meta", [True, False])
-def test_save_shards_load_shards(devices, model_name, pretrained, zero3, meta):
+@pytest.mark.parametrize("sharded", [True, False])
+def test_save_shards_load_shards(devices, model_name, pretrained, sharded):
     devices = [torch.device(device) for device in devices]
 
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
-    model_tp = get_tensor_parallel(model, devices, pretrained, zero3)
+    model = AutoModel.from_pretrained(model_name).to(devices[0])
+    model_tp = get_tensor_parallel(model, devices, pretrained, sharded=sharded)
 
     if pretrained:
-        half_the_model = f"{sum([p.numel() for p in model_tp.parameters()]) // 1_000_000 // 2}MB"
+        half_the_model = f"{sum([p.numel() for p in model_tp.parameters()]) * 8 // 1_000_000 // 2}MB"
         model_tp.save_pretrained(PATH_TO_SAVE, max_shard_size=half_the_model)
     else:
         torch.save(model_tp.state_dict(), PATH_TO_SAVE + "test_save_shards_load_shards.bin")
     del model_tp
 
-    if meta:
-        if zero3:
-            pytest.skip("Can't use zero3 with meta")
-        with init_empty_weights():
-            model_tp = get_tensor_parallel(
-                AutoModel.from_config(AutoConfig.from_pretrained(model_name)).half(), devices, pretrained, zero3
-            )
-    else:
-        model_tp = get_tensor_parallel(AutoModel.from_pretrained(model_name).half(), devices, pretrained, zero3)
+    new_model_tp = get_tensor_parallel(AutoModel.from_pretrained(model_name), devices, pretrained, sharded=sharded)
 
     checkpoint = PATH_TO_SAVE + ("pytorch_model.bin.index.json" if pretrained else "test_save_shards_load_shards.bin")
     load_checkpoint_in_model(
-        model_tp,
+        new_model_tp,
         checkpoint=checkpoint,
-        device_map=infer_sharded_device_map(model_tp),
+        device_map=infer_sharded_device_map(new_model_tp),
     )
-    assert not "meta" in [p.device.type for p in model_tp.parameters()]
+    assert not "meta" in [p.device.type for p in new_model_tp.parameters()]
+    new_model_tp(torch.zeros(1, 8, dtype=int))
 
 
 @pytest.mark.parametrize("use_pretrained", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
-def test_convert_state_dict(use_pretrained, devices, model_name):
-    model = AutoModel.from_pretrained(model_name).to(devices[0]).half()
+@pytest.mark.parametrize("sharded", [True, False])
+def test_convert_state_dict(use_pretrained, devices, model_name, sharded):
+    model = AutoModel.from_pretrained(model_name)
     torch.save(model.state_dict(), PATH_TO_SAVE + "test_convert_state_dict.bin")
-
-    if use_pretrained:
-        model_tp = TensorParallelPreTrainedModel(model, devices)
-    else:
-        model_tp = TensorParallel(model, devices)
     del model
 
-    model_tp_state_dict = model_tp.state_dict()
+    with init_empty_weights():
+        meta_model = AutoModel.from_pretrained(model_name)
+        if use_pretrained:
+            model_tp = TensorParallelPreTrainedModel(meta_model, devices, sharded=False)
+        else:
+            model_tp = TensorParallel(meta_model, devices, sharded=False)
+
     converted_state_dict = convert_state_dict(
         torch.load(PATH_TO_SAVE + "test_convert_state_dict.bin"),
         model_tp.tensor_parallel_config,
         world_size=len(devices),
         for_pretrained=use_pretrained,
     )
 
-    assert sorted(list(model_tp_state_dict.keys())) == sorted(list(converted_state_dict.keys()))
-
-    for name in model_tp_state_dict.keys():
-        data_tp = model_tp_state_dict[name]
-        data_converted = converted_state_dict[name]
+    for param_name, param in converted_state_dict.items():
+        set_module_tensor_to_device(model_tp, param_name, "cpu", value=param)
 
-        assert data_tp.shape == data_converted.shape
+    # When using meta device ZeRO-3 should only be applied after dispatch
+    if sharded:
+        model_tp.apply_sharding()
 
-        torch.testing.assert_close(data_tp, data_converted)
+    model_tp(torch.zeros(1, 8, dtype=int))
```

### Comparing `tensor_parallel-1.3.2/tests/test_transformers.py` & `tensor_parallel-2.0.0/tests/test_transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pytest
 import torch
 import transformers
 from peft import LoraConfig, get_peft_model
 from transformers import AutoModelForCausalLM, AutoTokenizer, BertModel, T5ForConditionalGeneration
 
-from tensor_parallel import TensorParallel, TensorParallelPreTrainedModel, tensor_parallel
+from tensor_parallel import TensorParallelPreTrainedModel
 from tensor_parallel.pretrained_model import find_predefined_tensor_parallel_config
 
 
 def add_lora(model: torch.nn.Module, model_name: str) -> torch.nn.Module:
     try:
         lora_config = LoraConfig(base_model_name_or_path=model_name, lora_alpha=32, lora_dropout=0.05)
         model = get_peft_model(model, lora_config)
@@ -75,92 +75,86 @@
 def prepare_model(model_name, use_lora):
     if model_name == "BlackSamorez/falcon-40b-tiny-testing" and torch.__version__ < "2.0":
         pytest.skip(f"Not testing {model_name} with torch=={torch.__version__}")
     if model_name == "BlackSamorez/llama-2-tiny-testing" and transformers.__version__ < "4.31":
         pytest.skip(f"Not testing {model_name} with transformers=={transformers.__version__}")
 
     try:
-        model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True, trust_remote_code=True).float()
+        model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True, trust_remote_code=True)
     except KeyError as err:
         pytest.skip(f"Could not create model {model_name} with error {err}")
     if use_lora:
         if model_name == "gpt2":
             pytest.skip("Not testing LoRA for gpt2")
         model = add_lora(model, model_name)
     return model
 
 
 @pytest.mark.parametrize("use_lora", [False, True])
-@pytest.mark.parametrize("use_config", [False, True])
+@pytest.mark.parametrize("sharded", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize(
     "model_name",
     [
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Salesforce/codegen-350M-mono",
         "Bingsu/llama-190m-arch",
         "BlackSamorez/llama-2-tiny-testing",
         "BlackSamorez/falcon-40b-tiny-testing",
     ],
 )
-def test_forward_gpt2_like(use_lora, use_config, devices, model_name):
+def test_forward_gpt2_like(use_lora, sharded, devices, model_name):
     torch.manual_seed(0)
 
-    model = prepare_model(model_name, use_lora)
+    model = prepare_model(model_name, use_lora).to(devices[0])
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, use_cache=True, output_hidden_states=True)
     out2_ref = model(inp2, use_cache=True, past_key_values=out1_ref.past_key_values)
     out3_ref = model(inp3, use_cache=True, past_key_values=out2_ref.past_key_values)
 
-    tp_config = None
-    if use_config:
-        tp_config = find_predefined_tensor_parallel_config(model.config, devices)
-    model_tp = TensorParallel(model, devices, tensor_parallel_config=tp_config)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     del model
 
     out1 = model_tp(inp1, use_cache=True, output_hidden_states=True)
     out2 = model_tp(inp2, use_cache=True, past_key_values=out1.past_key_values)
     out3 = model_tp(inp3, use_cache=True, past_key_values=out2.past_key_values)
 
     torch.testing.assert_close(out1_ref.hidden_states[-1], out1.hidden_states[-1], atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out1_ref.logits, out1.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out2_ref.logits, out2.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
 @pytest.mark.parametrize("use_lora", [False, True])
-@pytest.mark.parametrize("use_config", [False, True])
+@pytest.mark.parametrize("sharded", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["t5-small"])
-def test_forward_t5_like(use_lora, use_config, devices, model_name):
+def test_forward_t5_like(use_lora, sharded, devices, model_name):
     torch.manual_seed(0)
 
-    model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+    model = T5ForConditionalGeneration.from_pretrained(model_name).to(devices[0])
     if use_lora:
         model = add_lora(model, model_name)
 
     enc = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     dec2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     dec3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(enc, decoder_input_ids=dec1, use_cache=True, output_hidden_states=True)
     out2_ref = model(enc, decoder_input_ids=dec2, use_cache=True, past_key_values=out1_ref.past_key_values)
     out3_ref = model(enc, decoder_input_ids=dec3, use_cache=True, past_key_values=out2_ref.past_key_values)
 
-    tp_config = None
-    if use_config:
-        tp_config = find_predefined_tensor_parallel_config(model.config, devices)
-    model_tp = TensorParallel(model, devices, tensor_parallel_config=tp_config)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     del model
 
     out1 = model_tp(enc, decoder_input_ids=dec1, use_cache=True, output_hidden_states=True)
     out2 = model_tp(enc, decoder_input_ids=dec2, use_cache=True, past_key_values=out1_ref.past_key_values)
     out3 = model_tp(enc, decoder_input_ids=dec3, use_cache=True, past_key_values=out2_ref.past_key_values)
 
     torch.testing.assert_close(
@@ -168,36 +162,33 @@
     )
     torch.testing.assert_close(out1_ref.logits, out1.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out2_ref.logits, out2.logits, atol=3e-3, rtol=1e-05)
     torch.testing.assert_close(out3_ref.logits, out3.logits, atol=3e-3, rtol=1e-05)
 
 
 @pytest.mark.parametrize("use_lora", [False, True])
-@pytest.mark.parametrize("use_config", [False, True])
+@pytest.mark.parametrize("sharded", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize("model_name", ["bert-base-uncased"])
-def test_forward_bert_like(use_lora, use_config, devices, model_name):
+def test_forward_bert_like(use_lora, sharded, devices, model_name):
     torch.manual_seed(0)
 
     model = BertModel.from_pretrained(model_name).to(devices[0])
     if use_lora:
         model = add_lora(model, model_name)
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, output_hidden_states=True)
     out2_ref = model(inp2, output_hidden_states=True)
     out3_ref = model(inp3, output_hidden_states=True)
 
-    tp_config = None
-    if use_config:
-        tp_config = find_predefined_tensor_parallel_config(model.config, devices)
-    model_tp = TensorParallel(model, devices, tensor_parallel_config=tp_config)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     del model
 
     out1 = model_tp(inp1, output_hidden_states=True)
     out2 = model_tp(inp2, output_hidden_states=True)
     out3 = model_tp(inp3, output_hidden_states=True)
 
     torch.testing.assert_close(out1_ref.hidden_states[-1], out1.hidden_states[-1], atol=3e-3, rtol=1e-05)
@@ -226,16 +217,17 @@
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Bingsu/llama-190m-arch",
         "BlackSamorez/falcon-40b-tiny-testing",
     ],
 )
+@pytest.mark.parametrize("sharded", [True, False])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
-def test_generate(generate_kwargs, model_name, devices):
+def test_generate(generate_kwargs, model_name, sharded, devices):
     torch.manual_seed(0)
 
     if model_name == "BlackSamorez/falcon-40b-tiny-testing" and torch.__version__ < "2.0":
         pytest.skip(f"Not testing {model_name} with torch=={torch.__version__}")
 
     def _generate_scores(model, input_ids, generate_kwargs):
         scores_tuple = model.generate(
@@ -245,33 +237,29 @@
             output_scores=True,
             **generate_kwargs,
         ).scores
         return torch.stack([scores[0] for scores in scores_tuple], dim=0)
 
     try:
         if model_name == "t5-small":
-            model = (
-                T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
-            )
+            model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).to(devices[0])
         else:
             model = (
                 transformers.AutoModelForCausalLM.from_pretrained(
                     model_name, low_cpu_mem_usage=True, trust_remote_code=True
                 )
-                .float()
-                .to(devices[0])
-            )
+            ).to(devices[0])
     except KeyError as err:
         pytest.skip(f"Could not create model {model_name} with error {err}")
 
     input_ids = torch.randint(1, 1000, size=(2, 10), device=devices[0])
 
     scores_ref = _generate_scores(model, input_ids, generate_kwargs)
 
-    model_tp = tensor_parallel(model, devices)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     del model
 
     scores = _generate_scores(model_tp, input_ids, generate_kwargs)
 
     _assert_scores_allclose_long_enough(scores_ref, scores)
 
 
@@ -306,40 +294,37 @@
             .to(devices[0])
         )
 
     inputs_embeds = torch.rand(1, 3, model.config.hidden_size, device=devices[0])
 
     scores_ref = _generate_scores(model, inputs_embeds)
 
-    model_tp = tensor_parallel(model, devices)
+    model_tp = TensorParallelPreTrainedModel(model, devices)
     del model
 
     scores = _generate_scores(model_tp, inputs_embeds)
 
     _assert_scores_allclose_long_enough(scores_ref, scores)
 
 
-@pytest.mark.parametrize("use_predefined_config", [False, True])
 @pytest.mark.parametrize("model_name", ["t5-small"])
 @pytest.mark.parametrize("sharded", [False, True])
-def test_encoder(use_predefined_config, model_name, sharded):
+@pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
+def test_encoder(model_name, sharded, devices):
     torch.manual_seed(0)
 
-    devices = ["cpu"] * 2
-    model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True).float().to(devices[0])
+    model = T5ForConditionalGeneration.from_pretrained(model_name, low_cpu_mem_usage=True)
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
 
     out1_ref = model.get_encoder()(inp1)
     out2_ref = model.get_encoder()(inp2)
 
-    if not use_predefined_config:
-        model.config.architectures = ["Pretend we don't know this architecture"]
-    model_tp = tensor_parallel(model, devices, sharded=sharded)
+    model_tp = TensorParallelPreTrainedModel(model, devices, sharded=sharded)
     assert isinstance(model_tp, TensorParallelPreTrainedModel)
     del model
 
     out1 = model_tp.get_encoder()(inp1)
     out2 = model_tp.get_encoder()(inp2)
 
     torch.testing.assert_close(out1_ref, out1, atol=3e-3, rtol=1e-05)
```

