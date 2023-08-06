# Comparing `tmp/epochraft-0.1.0.dev20230804.tar.gz` & `tmp/epochraft-0.1.0.dev20230806.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochraft-0.1.0.dev20230804.tar", last modified: Thu Aug  3 15:09:56 2023, max compression
+gzip compressed data, was "epochraft-0.1.0.dev20230806.tar", last modified: Sun Aug  6 13:16:26 2023, max compression
```

## Comparing `epochraft-0.1.0.dev20230804.tar` & `epochraft-0.1.0.dev20230806.tar`

### file list

```diff
@@ -1,33 +1,42 @@
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1069 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/LICENSE
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3642 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/PKG-INFO
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1180 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/README.md
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      463 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     7615 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/base.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/combinations/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      135 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     2202 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/concat.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3280 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/combinations/interleave.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/sources/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      325 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1904 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/iterable.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     2930 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/mosaicml.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1951 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/sources/sequence.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3481 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/testing.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft/transforms/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      589 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/__init__.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1266 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/batch.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3435 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/concat_chunk.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     1724 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/count.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      955 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/filter_map.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     7242 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/epochraft/transforms/parallel_filter_map.py
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       33 2023-08-03 15:09:53.000000 epochraft-0.1.0.dev20230804/epochraft/version.py
-drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/epochraft.egg-info/
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     3642 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/PKG-INFO
--rw-rw-r--   0 takiba    (1000) takiba    (1000)      712 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/SOURCES.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)        1 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/dependency_links.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       99 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/requires.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       10 2023-08-03 15:09:56.000000 epochraft-0.1.0.dev20230804/epochraft.egg-info/top_level.txt
--rw-rw-r--   0 takiba    (1000) takiba    (1000)     2086 2023-08-03 15:09:49.000000 epochraft-0.1.0.dev20230804/pyproject.toml
--rw-rw-r--   0 takiba    (1000) takiba    (1000)       38 2023-08-03 15:09:56.289235 epochraft-0.1.0.dev20230804/setup.cfg
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1069 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/LICENSE
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     8565 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/PKG-INFO
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     6103 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/README.md
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      463 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     9232 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/base.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/combinations/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      135 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/combinations/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2202 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/combinations/concat.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3301 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/combinations/interleave.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/sources/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      325 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/sources/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1904 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/sources/iterable.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2930 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/sources/mosaicml.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1951 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/sources/sequence.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3481 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/testing.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/transforms/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      841 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/__init__.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      451 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1267 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/batch.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1725 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/count.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      956 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/filter_map.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     7243 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/basic/parallel_filter_map.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      542 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/__init__.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     4155 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/bos_eos.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2232 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/chunk.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1897 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/concat_chunk.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     3441 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/pack_chunk.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1246 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/padding.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     4029 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/tokenizer_utils.py
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       33 2023-08-06 13:16:23.000000 epochraft-0.1.0.dev20230806/epochraft/version.py
+drwxrwxr-x   0 takiba    (1000) takiba    (1000)        0 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/epochraft.egg-info/
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     8565 2023-08-06 13:16:26.000000 epochraft-0.1.0.dev20230806/epochraft.egg-info/PKG-INFO
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     1103 2023-08-06 13:16:26.000000 epochraft-0.1.0.dev20230806/epochraft.egg-info/SOURCES.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)        1 2023-08-06 13:16:26.000000 epochraft-0.1.0.dev20230806/epochraft.egg-info/dependency_links.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)      113 2023-08-06 13:16:26.000000 epochraft-0.1.0.dev20230806/epochraft.egg-info/requires.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       10 2023-08-06 13:16:26.000000 epochraft-0.1.0.dev20230806/epochraft.egg-info/top_level.txt
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)     2107 2023-08-06 13:16:18.000000 epochraft-0.1.0.dev20230806/pyproject.toml
+-rw-rw-r--   0 takiba    (1000) takiba    (1000)       38 2023-08-06 13:16:26.230281 epochraft-0.1.0.dev20230806/setup.cfg
```

### Comparing `epochraft-0.1.0.dev20230804/LICENSE` & `epochraft-0.1.0.dev20230806/LICENSE`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/base.py` & `epochraft-0.1.0.dev20230806/epochraft/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
+    Mapping,
     Optional,
     Sequence,
     Union,
 )
 
 import numpy as np
 import torch
@@ -196,45 +197,29 @@
     ) -> CheckpointableDataset:
         from .transforms import BatchDataset
 
         return BatchDataset(
             self, batch_size=batch_size, collate_fn=collate_fn, drop_last=drop_last
         )
 
-    def concat_chunk(
-        self,
-        chunk_length: int,
-        column: str = "input_ids",
-        bos_tokens: Optional[TokenArray] = None,
-        eos_tokens: Optional[TokenArray] = None,
-    ) -> CheckpointableDataset:
-        from .transforms import ConcatChunkDataset
-
-        return ConcatChunkDataset(
-            self,
-            chunk_length=chunk_length,
-            column=column,
-            bos_tokens=bos_tokens,
-            eos_tokens=eos_tokens,
-        )
-
     def tokenize(
         self,
         tokenizer: Tokenizer,
         tokenizer_kwargs: Optional[Dict[str, Any]] = None,
         target_column: str = "text",
         parallel: bool = True,
         max_workers: Optional[int] = None,
         prefetch_factor: int = 10,
         ordered: bool = True,
         executor_type: ParallelExecutorType = "process",
     ) -> CheckpointableDataset:
         tokenizer_kwargs = tokenizer_kwargs or {}
 
         def _fn(sample: Sample) -> Sample:
+            sample = sample.copy()
             sample.update(tokenizer(sample[target_column], **tokenizer_kwargs))
             return sample
 
         if parallel:
             # TODO: show some warning on this
             os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
@@ -244,13 +229,84 @@
                 prefetch_factor=prefetch_factor,
                 ordered=ordered,
                 executor_type=executor_type,
             )
         else:
             return self.map(_fn)
 
+    def add_bos_eos(
+        self,
+        bos_token_id: Optional[int],
+        eos_token_id: Optional[int],
+        target_column: str = "input_ids",
+    ) -> CheckpointableDataset:
+        from .transforms import add_bos_eos
+
+        return add_bos_eos(
+            self, bos_token_id=bos_token_id, eos_token_id=eos_token_id, target_column=target_column
+        )
+
+    def ensure_bos_eos(
+        self, tokenizer: Tokenizer, target_column: str = "input_ids"
+    ) -> CheckpointableDataset:
+        from .transforms import ensure_bos_eos
+
+        return ensure_bos_eos(self, tokenizer=tokenizer, target_column=target_column)
+
+    def pad(
+        self,
+        pad_values: Mapping[str, int],
+        chunk_length: int,
+    ) -> CheckpointableDataset:
+        from .transforms import pad
+
+        return pad(self, pad_values=pad_values, chunk_length=chunk_length)
+
+    def chunk(
+        self,
+        chunk_length: int,
+        target_columns: Sequence[str] = ("input_ids",),
+        drop_remainder: bool = True,
+    ) -> CheckpointableDataset:
+        from .transforms import ChunkDataset
+
+        return ChunkDataset(
+            self,
+            chunk_length=chunk_length,
+            target_columns=target_columns,
+            drop_remainder=drop_remainder,
+        )
+
+    def concat_chunk(
+        self,
+        chunk_length: int,
+        target_columns: Sequence[str] = ("input_ids",),
+    ) -> CheckpointableDataset:
+        from .transforms import ConcatChunkDataset
+
+        return ConcatChunkDataset(
+            self,
+            chunk_length=chunk_length,
+            target_columns=target_columns,
+        )
+
+    def pack_chunk(
+        self,
+        chunk_length: int,
+        target_columns: Sequence[str],
+        discard_long_samples: bool = False,
+    ) -> CheckpointableDataset:
+        from .transforms import PackChunkDataset
+
+        return PackChunkDataset(
+            self,
+            chunk_length=chunk_length,
+            target_columns=target_columns,
+            discard_long_samples=discard_long_samples,
+        )
+
     # `__add__` is implemented in PyTorch's `IterableDataset`,
     # so we need to override it here for prevent unexpected behavior
     def __add__(self, other: CheckpointableDataset) -> CheckpointableDataset:  # type: ignore
         from .combinations import concat_datasets
 
         return concat_datasets([self, other])
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/combinations/concat.py` & `epochraft-0.1.0.dev20230806/epochraft/combinations/concat.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/combinations/interleave.py` & `epochraft-0.1.0.dev20230806/epochraft/combinations/interleave.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         order.append(source_id)
 
     return order
 
 
 class InterleaveIterator(CheckpointableIterator):
     def __init__(
-        self, dataset: Interleave, sources: list[CheckpointableIterator], start_index: int
+        self, dataset: InterleaveDataset, sources: list[CheckpointableIterator], start_index: int
     ) -> None:
         self.dataset = dataset
         self.sources = sources
         self.index = start_index
         self.source_ids = generate_stratified_sampling_order(
             self.dataset.weights, self.dataset.chunk_size
         )
@@ -46,15 +46,15 @@
             f"source{source_id}": source.state_dict()
             for source_id, source in enumerate(self.sources)
         }
         state_dict["index"] = self.index
         return state_dict
 
 
-class Interleave(CheckpointableDataset):
+class InterleaveDataset(CheckpointableDataset):
     def __init__(
         self,
         sources: list[CheckpointableDataset],
         weights: Optional[list[float]],
         chunk_size: int = 1024,
     ):
         if weights is not None:
@@ -90,8 +90,8 @@
 
 
 def interleave_datasets(
     sources: list[CheckpointableDataset],
     weights: Optional[list[float]] = None,
     chunk_size: int = 1024,
 ) -> CheckpointableDataset:
-    return Interleave(sources, weights, chunk_size=chunk_size)
+    return InterleaveDataset(sources, weights, chunk_size=chunk_size)
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/sources/iterable.py` & `epochraft-0.1.0.dev20230806/epochraft/sources/iterable.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/sources/mosaicml.py` & `epochraft-0.1.0.dev20230806/epochraft/sources/mosaicml.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/sources/sequence.py` & `epochraft-0.1.0.dev20230806/epochraft/sources/sequence.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/testing.py` & `epochraft-0.1.0.dev20230806/epochraft/testing.py`

 * *Files identical despite different names*

### Comparing `epochraft-0.1.0.dev20230804/epochraft/transforms/batch.py` & `epochraft-0.1.0.dev20230806/epochraft/transforms/basic/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from ..base import CheckpointableDataset, CheckpointableIterator, CollateFn, Sample, StateDict
+from ...base import CheckpointableDataset, CheckpointableIterator, CollateFn, Sample, StateDict
 
 
 class BatchIterator(CheckpointableIterator):
     def __init__(self, dataset: BatchDataset, source: CheckpointableIterator) -> None:
         self.dataset = dataset
         self.source = source
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/transforms/concat_chunk.py` & `epochraft-0.1.0.dev20230806/epochraft/transforms/language_modeling/pack_chunk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,95 @@
 from __future__ import annotations
 
-from typing import Any, Optional, Union
+import copy
+from typing import Any, Optional, Sequence
 
-import numpy as np
 import torch
 
-from ..base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict, TokenArray
+from ...base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict
+from .tokenizer_utils import TokensQueue
 
 
-def tensor_from_token_array(data: Optional[Union[int, TokenArray]]) -> torch.Tensor:
-    if data is None:
-        data = []
-    if isinstance(data, int):
-        data = [data]
-
-    if isinstance(data, torch.Tensor):
-        tensor = data
-    elif isinstance(data, np.ndarray):
-        if np.issubdtype(data.dtype, np.integer):
-            tensor = torch.from_numpy(data).long()
-        else:
-            raise ValueError(f"Expected integer ndarray, got ndarray of {data.dtype}")
-    else:
-        tensor = torch.tensor(data, dtype=torch.long)
-
-    if tensor.dtype != torch.long:
-        raise ValueError(f"Expected long tensor, got {tensor.dtype}")
-
-    if tensor.dim() == 2:
-        if tensor.shape[0] != 1:
-            raise ValueError(
-                "input_ids must be 1-dimensional tensor or 2-dimensional tensor with batch size 1"
-            )
-        tensor = tensor[0]
-    elif tensor.dim() != 1:
-        raise ValueError("input_ids must be 1-dimensional tensor")
-    return tensor
-
-
-class ConcatChunkIterator(CheckpointableIterator):
+class PackChunkIterator(CheckpointableIterator):
     def __init__(
         self,
-        dataset: ConcatChunkDataset,
+        dataset: PackChunkDataset,
         source: CheckpointableIterator,
-        buffer: Optional[torch.LongTensor],
+        buffers: Optional[dict[str, torch.Tensor]],
     ) -> None:
         self.dataset = dataset
+        self.queue = TokensQueue(columns=self.dataset.target_columns, buffers=buffers)
         self.source = source
-        self.buffer = torch.empty((0,), dtype=torch.long) if buffer is None else buffer
 
     def __next__(self) -> Sample:
-        while len(self.buffer) < self.dataset.chunk_length:
-            source_sample = next(self.source)
-            tokens = tensor_from_token_array(source_sample[self.dataset.column])
-            self.buffer = torch.cat(
-                [
-                    self.buffer,
-                    self.dataset.bos_tokens,
-                    tokens,
-                    self.dataset.eos_tokens,
-                ]
-            )
-            print(tokens.shape, self.buffer.shape)
-
-        y = self.buffer[: self.dataset.chunk_length]
-        self.buffer = self.buffer[self.dataset.chunk_length :]
-        return {self.dataset.column: y}
+        # Add samples until the buffer exceeds the chunk length
+        while True:
+            try:
+                input_sample = next(self.source)
+            except StopIteration:
+                input_tensor_dict = None
+                break
+            input_tensor_dict = self.queue.tensor_dict_from_sample(input_sample)
+            input_length = len(input_tensor_dict[self.dataset.target_columns[0]])
+
+            # Discard too long samples
+            if self.dataset.discard_long_samples and input_length > self.dataset.chunk_length:
+                continue
+
+            buffer_length = self.queue.length()
+
+            if input_length + buffer_length > self.dataset.chunk_length:
+                break
+            else:
+                self.queue.push_from_tensor_dict(input_tensor_dict)
+
+        # Take the sample from the buffer, then add the remaining sample
+        output_sample = self.queue.pop_all()
+        if input_tensor_dict is None:
+            output_length = len(output_sample[self.dataset.target_columns[0]])
+            # If the source is exhausted and the buffer is empty, then we are done
+            if output_length == 0:
+                raise StopIteration()
+        else:
+            self.queue.push_from_tensor_dict(input_tensor_dict)
+
+        # Truncate the output sample
+        for column in self.dataset.target_columns:
+            if len(output_sample[column]) > self.dataset.chunk_length:
+                # Truncate
+                assert not self.dataset.discard_long_samples  # This should have been discarded
+                output_sample[column] = output_sample[column][: self.dataset.chunk_length]
+
+        return output_sample
 
     def state_dict(self) -> StateDict:
         return {
             "source": self.source.state_dict(),
-            "buffer": self.buffer,
+            "buffers": self.queue.buffers.copy(),
         }
 
 
-class ConcatChunkDataset(CheckpointableDataset):
+class PackChunkDataset(CheckpointableDataset):
     def __init__(
         self,
         source: CheckpointableDataset,
         chunk_length: int,
-        column: str,
-        bos_tokens: Optional[Union[int, TokenArray]],
-        eos_tokens: Optional[Union[int, TokenArray]],
+        target_columns: Sequence[str],
+        discard_long_samples: bool = False,
     ) -> None:
         self.source = source
-        self.column = column
+        self.target_columns = target_columns
         self.chunk_length = chunk_length
-        self.bos_tokens = tensor_from_token_array(bos_tokens)
-        self.eos_tokens = tensor_from_token_array(eos_tokens)
+        self.discard_long_samples = discard_long_samples
 
     def iter(self, state_dict: Optional[dict[str, Any]] = None) -> CheckpointableIterator:
         if state_dict:
             source_state_dict = state_dict.pop("source")
-            buffer = state_dict.pop("buffer")
+            buffers = copy.copy(state_dict.pop("buffers"))
             if state_dict:
                 raise ValueError(f"Unexpected keys in state_dict: {state_dict.keys()}")
         else:
             source_state_dict = None
-            buffer = None
+            buffers = None
 
         source = self.source.iter(state_dict=source_state_dict)
-        return ConcatChunkIterator(self, source, buffer)
+        return PackChunkIterator(self, source, buffers)
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/transforms/count.py` & `epochraft-0.1.0.dev20230806/epochraft/transforms/basic/count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from ..base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict
+from ...base import CheckpointableDataset, CheckpointableIterator, Sample, StateDict
 
 
 class CountIterator(CheckpointableIterator):
     def __init__(
         self, dataset: CountDataset, source: CheckpointableIterator, start_count: int
     ) -> None:
         self.count = start_count
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/transforms/filter_map.py` & `epochraft-0.1.0.dev20230806/epochraft/transforms/basic/filter_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
-from ..base import CheckpointableDataset, CheckpointableIterator, FilterMapFn, Sample, StateDict
+from ...base import CheckpointableDataset, CheckpointableIterator, FilterMapFn, Sample, StateDict
 
 
 class FilterMapIterator(CheckpointableIterator):
     def __init__(self, source: CheckpointableIterator, fn: FilterMapFn):
         self.source = source
         self.fn = fn
```

### Comparing `epochraft-0.1.0.dev20230804/epochraft/transforms/parallel_filter_map.py` & `epochraft-0.1.0.dev20230806/epochraft/transforms/basic/parallel_filter_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import uuid
 from collections import deque
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from contextlib import contextmanager
 from typing import Any, Callable, Generator, Iterator, Optional, Type, Union
 
-from ..base import (
+from ...base import (
     CheckpointableDataset,
     CheckpointableIterator,
     FilterMapFn,
     ParallelExecutorType,
     Sample,
     StateDict,
 )
```

### Comparing `epochraft-0.1.0.dev20230804/pyproject.toml` & `epochraft-0.1.0.dev20230806/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "blackdoc",
     "flake8",
     "isort",
     "mypy",
     "pytest",
     "mosaicml-streaming",
     "transformers",
+    "sentencepiece",
 ]
 
 [project.urls]
 repository = "https://github.com/iwiwi/epochraft"
 
 [tool.setuptools.packages.find]
 include = ["epochraft*"]
```

