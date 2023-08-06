# Comparing `tmp/rwkv-beta-0.8.0.tar.gz` & `tmp/rwkv-beta-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-beta-0.8.0.tar", last modified: Sat Jul 29 13:07:14 2023, max compression
+gzip compressed data, was "rwkv-beta-0.8.1.tar", last modified: Sun Aug  6 10:47:25 2023, max compression
```

## Comparing `rwkv-beta-0.8.0.tar` & `rwkv-beta-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/
--rw-r--r--   0 dev       (1017) dev       (1017)    11357 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/LICENSE
--rw-r--r--   0 dev       (1017) dev       (1017)       47 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/MANIFEST.in
--rw-r--r--   0 dev       (1017) dev       (1017)     4847 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/PKG-INFO
--rw-r--r--   0 dev       (1017) dev       (1017)     4372 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/README.md
--rw-r--r--   0 dev       (1017) dev       (1017)      504 2023-07-29 13:06:55.000000 rwkv-beta-0.8.0/pyproject.toml
--rw-r--r--   0 dev       (1017) dev       (1017)       38 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/setup.cfg
-drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-07-29 13:07:14.759629 rwkv-beta-0.8.0/src/
-drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/src/rwkv/
--rw-r--r--   0 dev       (1017) dev       (1017)        0 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/src/rwkv/__init__.py
-drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/src/rwkv/cuda/
--rw-r--r--   0 dev       (1017) dev       (1017)     3734 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/att_one.cu
--rw-r--r--   0 dev       (1017) dev       (1017)     6591 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/att_seq.cu
--rw-r--r--   0 dev       (1017) dev       (1017)      645 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/element_wise.h
--rw-r--r--   0 dev       (1017) dev       (1017)     5679 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/ffn.cu
--rw-r--r--   0 dev       (1017) dev       (1017)     3358 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/gemm_fp16_cublas.cpp
--rw-r--r--   0 dev       (1017) dev       (1017)     8677 2023-07-20 11:25:40.000000 rwkv-beta-0.8.0/src/rwkv/cuda/operators.cu
--rw-r--r--   0 dev       (1017) dev       (1017)      240 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/util.h
--rw-r--r--   0 dev       (1017) dev       (1017)     6482 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 dev       (1017) dev       (1017)    38451 2023-07-29 13:02:44.000000 rwkv-beta-0.8.0/src/rwkv/model.py
--rw-r--r--   0 dev       (1017) dev       (1017)     3201 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 dev       (1017) dev       (1017)  1093733 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 dev       (1017) dev       (1017)     5356 2023-07-15 14:33:06.000000 rwkv-beta-0.8.0/src/rwkv/utils.py
-drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-07-29 13:07:14.763630 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/
--rw-r--r--   0 dev       (1017) dev       (1017)     4847 2023-07-29 13:07:14.000000 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1017) dev       (1017)      555 2023-07-29 13:07:14.000000 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1017) dev       (1017)        1 2023-07-29 13:07:14.000000 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1017) dev       (1017)       19 2023-07-29 13:07:14.000000 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/requires.txt
--rw-r--r--   0 dev       (1017) dev       (1017)        5 2023-07-29 13:07:14.000000 rwkv-beta-0.8.0/src/rwkv_beta.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/
+-rw-r--r--   0 dev       (1017) dev       (1017)    11357 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/LICENSE
+-rw-r--r--   0 dev       (1017) dev       (1017)       47 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/MANIFEST.in
+-rw-r--r--   0 dev       (1017) dev       (1017)     4847 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/PKG-INFO
+-rw-r--r--   0 dev       (1017) dev       (1017)     4372 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/README.md
+-rw-r--r--   0 dev       (1017) dev       (1017)      504 2023-08-06 10:47:15.000000 rwkv-beta-0.8.1/pyproject.toml
+-rw-r--r--   0 dev       (1017) dev       (1017)       38 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/setup.cfg
+drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-08-06 10:47:25.070351 rwkv-beta-0.8.1/src/
+drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/src/rwkv/
+-rw-r--r--   0 dev       (1017) dev       (1017)        0 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/src/rwkv/__init__.py
+drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/src/rwkv/cuda/
+-rw-r--r--   0 dev       (1017) dev       (1017)     3734 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/att_one.cu
+-rw-r--r--   0 dev       (1017) dev       (1017)     6591 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/att_seq.cu
+-rw-r--r--   0 dev       (1017) dev       (1017)      645 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/element_wise.h
+-rw-r--r--   0 dev       (1017) dev       (1017)     5679 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/ffn.cu
+-rw-r--r--   0 dev       (1017) dev       (1017)     3364 2023-08-06 10:44:59.000000 rwkv-beta-0.8.1/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 dev       (1017) dev       (1017)     8677 2023-07-20 11:25:40.000000 rwkv-beta-0.8.1/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 dev       (1017) dev       (1017)      240 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/util.h
+-rw-r--r--   0 dev       (1017) dev       (1017)     6482 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 dev       (1017) dev       (1017)    38451 2023-08-06 10:44:13.000000 rwkv-beta-0.8.1/src/rwkv/model.py
+-rw-r--r--   0 dev       (1017) dev       (1017)     3201 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 dev       (1017) dev       (1017)  1093733 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 dev       (1017) dev       (1017)     5356 2023-07-15 14:33:06.000000 rwkv-beta-0.8.1/src/rwkv/utils.py
+drwxr-xr-x   0 dev       (1017) dev       (1017)        0 2023-08-06 10:47:25.074352 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/
+-rw-r--r--   0 dev       (1017) dev       (1017)     4847 2023-08-06 10:47:25.000000 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1017) dev       (1017)      555 2023-08-06 10:47:25.000000 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1017) dev       (1017)        1 2023-08-06 10:47:25.000000 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1017) dev       (1017)       19 2023-08-06 10:47:25.000000 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/requires.txt
+-rw-r--r--   0 dev       (1017) dev       (1017)        5 2023-08-06 10:47:25.000000 rwkv-beta-0.8.1/src/rwkv_beta.egg-info/top_level.txt
```

### Comparing `rwkv-beta-0.8.0/LICENSE` & `rwkv-beta-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/PKG-INFO` & `rwkv-beta-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv-beta
-Version: 0.8.0
+Version: 0.8.1
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-beta-0.8.0/README.md` & `rwkv-beta-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/att_one.cu` & `rwkv-beta-0.8.1/src/rwkv/cuda/att_one.cu`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/att_seq.cu` & `rwkv-beta-0.8.1/src/rwkv/cuda/att_seq.cu`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/element_wise.h` & `rwkv-beta-0.8.1/src/rwkv/cuda/element_wise.h`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/ffn.cu` & `rwkv-beta-0.8.1/src/rwkv/cuda/ffn.cu`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/gemm_fp16_cublas.cpp` & `rwkv-beta-0.8.1/src/rwkv/cuda/gemm_fp16_cublas.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   // use CUBLAS_OP_N. see the notes above
   const cublasOperation_t cublas_trans_a = CUBLAS_OP_N;
   const cublasOperation_t cublas_trans_b = CUBLAS_OP_N;
   // m = (B^T).size(0) = B.size(1) = n;
   const int cublas_m = ori_n;
   const int cublas_k = ori_k;
   // comptiable with rwkv one mode, where 1-D tensor * 2-D tensor
-  // const int n = a.dense_dim() == 1 ? 1 : a.size(0);
+  // const int n = a.sizes().size() == 1 ? 1 : a.size(0);
   const int cublas_n = ori_m;
   const int cublas_lda = cublas_m;
   const int cublas_ldb = cublas_k;
   const int cublas_ldc = cublas_m;
   cublasHandle_t cublas_handle = get_cublas_handle();
 
 #if CUDA_VERSION >= 11000
@@ -68,13 +68,13 @@
       cublas_k, &sp_alpha, b, cuda_data_type, cublas_lda,
       a, cuda_data_type, cublas_ldb, &sp_beta, c,
       cuda_c_data_type, cublas_ldc, compute_type, algo));
 }
 
 void gemm_fp16_cublas(torch::Tensor a, torch::Tensor b, torch::Tensor c) {
   // comptiable with rwkv one mode, 1-D tensor * 2-D tensor
-  const int m = a.dense_dim() == 1 ? 1 : a.size(0);
+  const int m = a.sizes().size() == 1 ? 1 : a.size(0);
   const int n = b.size(1);
   const int k = b.size(0);
   gemm_fp16_cublas(a.data_ptr(), b.data_ptr(), c.data_ptr(), m, n, k,
                    c.dtype() == torch::kFloat32);
 }
```

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/operators.cu` & `rwkv-beta-0.8.1/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/cuda/wrapper.cpp` & `rwkv-beta-0.8.1/src/rwkv/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/model.py` & `rwkv-beta-0.8.1/src/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/rwkv_tokenizer.py` & `rwkv-beta-0.8.1/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-beta-0.8.1/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv/utils.py` & `rwkv-beta-0.8.1/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-beta-0.8.0/src/rwkv_beta.egg-info/PKG-INFO` & `rwkv-beta-0.8.1/src/rwkv_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv-beta
-Version: 0.8.0
+Version: 0.8.1
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-beta-0.8.0/src/rwkv_beta.egg-info/SOURCES.txt` & `rwkv-beta-0.8.1/src/rwkv_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

