# Comparing `tmp/tf_nightly_cpu-2.15.0.dev20230805-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly_cpu-2.15.0.dev20230806-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2263 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     3362 b- defN 23-Aug-05 07:50 tf_nightly_cpu-2.15.0.dev20230805.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 23-Aug-05 07:50 tf_nightly_cpu-2.15.0.dev20230805.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Aug-05 07:50 tf_nightly_cpu-2.15.0.dev20230805.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      377 b- defN 23-Aug-05 07:50 tf_nightly_cpu-2.15.0.dev20230805.dist-info/RECORD
-4 files, 3839 bytes uncompressed, 1521 bytes compressed:  60.4%
+Zip file size: 2262 bytes, number of entries: 4
+-rw-rw-r--  2.0 unx     3362 b- defN 23-Aug-06 07:50 tf_nightly_cpu-2.15.0.dev20230806.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 23-Aug-06 07:50 tf_nightly_cpu-2.15.0.dev20230806.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-06 07:50 tf_nightly_cpu-2.15.0.dev20230806.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      377 b- defN 23-Aug-06 07:50 tf_nightly_cpu-2.15.0.dev20230806.dist-info/RECORD
+4 files, 3839 bytes uncompressed, 1520 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly_cpu-2.15.0.dev20230805.dist-info/METADATA
+Filename: tf_nightly_cpu-2.15.0.dev20230806.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly_cpu-2.15.0.dev20230805.dist-info/WHEEL
+Filename: tf_nightly_cpu-2.15.0.dev20230806.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly_cpu-2.15.0.dev20230805.dist-info/top_level.txt
+Filename: tf_nightly_cpu-2.15.0.dev20230806.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly_cpu-2.15.0.dev20230805.dist-info/RECORD
+Filename: tf_nightly_cpu-2.15.0.dev20230806.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly_cpu-2.15.0.dev20230805.dist-info/METADATA` & `tf_nightly_cpu-2.15.0.dev20230806.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly-cpu
-Version: 2.15.0.dev20230805
+Version: 2.15.0.dev20230806
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -24,17 +24,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-macos (==2.15.0-dev20230805) ; platform_system == "Darwin" and platform_machine == "arm64"
-Requires-Dist: tf-nightly-cpu-aws (==2.15.0-dev20230805) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
-Requires-Dist: tf-nightly-intel (==2.15.0-dev20230805) ; platform_system == "Windows"
+Requires-Dist: tf-nightly-macos (==2.15.0-dev20230806) ; platform_system == "Darwin" and platform_machine == "arm64"
+Requires-Dist: tf-nightly-cpu-aws (==2.15.0-dev20230806) ; platform_system == "Linux" and (platform_machine == "arm64" or platform_machine == "aarch64")
+Requires-Dist: tf-nightly-intel (==2.15.0-dev20230806) ; platform_system == "Windows"
 Provides-Extra: and-cuda
 Requires-Dist: nvidia-cublas-cu11 (==11.11.3.6) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-cupti-cu11 (==11.8.87) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvcc-cu11 (==11.8.89) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-runtime-cu11 (==11.8.89) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cudnn-cu11 (==8.7.0.84) ; extra == 'and-cuda'
 Requires-Dist: nvidia-cufft-cu11 (==10.9.0.58) ; extra == 'and-cuda'
```

