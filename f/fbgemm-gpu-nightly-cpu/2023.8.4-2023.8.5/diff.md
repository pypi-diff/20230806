# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.8.4-cp39-cp39-manylinux2014_aarch64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.8.5-cp39-cp39-manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,43 @@
-Zip file size: 2426975 bytes, number of entries: 41
--rw-r--r--  2.0 unx      567 b- defN 23-Aug-04 13:01 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-Aug-04 13:01 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Aug-04 13:01 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-Aug-04 13:01 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx  7619920 b- defN 23-Aug-04 13:01 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-Aug-04 13:01 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-Aug-04 13:01 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2737 b- defN 23-Aug-04 13:01 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Aug-04 13:01 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Aug-04 13:01 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5745 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      525 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    19833 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    60371 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    80930 b- defN 23-Aug-04 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39550 b- defN 23-Aug-04 13:01 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-Aug-04 13:01 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1603 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4076 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     3291 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     2775 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+Zip file size: 2426976 bytes, number of entries: 41
+-rw-r--r--  2.0 unx      567 b- defN 23-Aug-05 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-Aug-05 12:59 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Aug-05 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Aug-05 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx  7619920 b- defN 23-Aug-05 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-Aug-05 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Aug-05 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2737 b- defN 23-Aug-05 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Aug-05 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Aug-05 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5745 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     6661 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    19833 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    60371 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    80930 b- defN 23-Aug-05 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39550 b- defN 23-Aug-05 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Aug-05 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4076 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     3291 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     2775 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
 -rw-r--r--  2.0 unx     1906 b- defN 23-Jul-31 12:54 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3291 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3040 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     2316 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4320 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6067 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2768 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4602 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3658 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx      635 b- defN 23-Jun-22 15:52 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6136 b- defN 23-Aug-04 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2933 b- defN 23-Aug-04 13:01 fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 23-Aug-04 13:01 fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Aug-04 13:01 fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4529 b- defN 23-Aug-04 13:01 fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/RECORD
-41 files, 7945566 bytes uncompressed, 2419345 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     3291 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3040 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     2316 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4320 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6067 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2768 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4602 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3658 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Jun-22 18:27 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6136 b- defN 23-Aug-05 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2933 b- defN 23-Aug-05 12:59 fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      106 b- defN 23-Aug-05 12:59 fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-05 12:59 fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4529 b- defN 23-Aug-05 12:59 fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/RECORD
+41 files, 7945566 bytes uncompressed, 2419346 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.8.4
+Version: 2023.8.5
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=ToqlGd9bLtY0OtUZr7JnaujeLgIcI2mAoCcPeaMVn1s,4320
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=PVePhoU52wiFE_1gdZezHBiqsjiwJjzn2JBLEW3X2uk,6067
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=lUEZjp4C3HxSizRXKr47gAV1hgBtGqENVSFqNo5NtA0,2768
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=2U09t7mznAY-6HosMRX5kqplVO-HETHt4gKI26jjQXs,4602
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=wv_Sdrifrrcw2hsgRwNCGsma6roIU5hXiEzpct4bmrc,3658
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=I6xnQ0vv6PZCxMsR87fWvb1Qtkp7ehx1b-9-La1vW2U,635
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=soARoBsdOnNNZdCIkVmryPHtKyhbcFLqHOTveG-hk6s,6136
-fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/METADATA,sha256=grY2g8IfnUSDsgt1gi3NZ4oO_FYhkctZwDSA5O4k0Vw,2933
-fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/WHEEL,sha256=QS_R-QQSWSRw5liIm8i7XTjFgUJNmR921C3Rhvwyw_M,106
-fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.8.4.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/METADATA,sha256=NW8TkB0enKph-3WNw-GXkgLzcBMwGjg_aupQ_8jWvA4,2933
+fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/WHEEL,sha256=ICZqLeDlvTRZ7H_XkkAxWGWfUQl8ghTdIaSNvR3KLhk,106
+fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.8.5.dist-info/RECORD,,
```

