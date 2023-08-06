# Comparing `tmp/tvdcn-0.4.0.tar.gz` & `tmp/tvdcn-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.4.0.tar", last modified: Sat Aug  5 19:15:44 2023, max compression
+gzip compressed data, was "tvdcn-0.4.1.tar", last modified: Sun Aug  6 20:35:48 2023, max compression
```

## Comparing `tvdcn-0.4.0.tar` & `tvdcn-0.4.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-05 19:13:49.000000 tvdcn-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-05 19:13:49.000000 tvdcn-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-05 19:15:44.160912 tvdcn-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-05 19:13:49.000000 tvdcn-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-05 19:13:49.000000 tvdcn-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 19:13:49.000000 tvdcn-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-05 19:15:44.160912 tvdcn-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-05 19:13:49.000000 tvdcn-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.148911 tvdcn-0.4.0/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.148911 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.152912 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.156911 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28031 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32013 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28023 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/csrc/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/utils/tensor_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.465257 tvdcn-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 20:33:41.000000 tvdcn-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-06 20:33:41.000000 tvdcn-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-06 20:35:48.465257 tvdcn-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-06 20:33:41.000000 tvdcn-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-06 20:33:41.000000 tvdcn-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 20:33:41.000000 tvdcn-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-06 20:35:48.465257 tvdcn-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-06 20:33:41.000000 tvdcn-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.429256 tvdcn-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.437256 tvdcn-0.4.1/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.441256 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.445256 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.453256 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28031 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32013 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.457256 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28023 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.461257 tvdcn-0.4.1/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.461257 tvdcn-0.4.1/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.465257 tvdcn-0.4.1/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.4.0/LICENSE.txt` & `tvdcn-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/PKG-INFO` & `tvdcn-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.4.0
+Version: 0.4.1
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
-Keywords: deform_conv; deformable convolution
+Keywords: deform_conv,deform_conv_transposed,deformable_convolution,transposed_deformable_convolution
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tvdcn-0.4.0/README.md` & `tvdcn-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/pyproject.toml` & `tvdcn-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/setup.cfg` & `tvdcn-0.4.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering :: Artificial Intelligence
-keywords = deform_conv; deformable convolution
+keywords = deform_conv,deform_conv_transposed,deformable_convolution,transposed_deformable_convolution
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 python_requires = >=3.6
 setup_requires = torch
```

### Comparing `tvdcn-0.4.0/setup.py` & `tvdcn-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.4.1/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tests/test_grad.py` & `tvdcn-0.4.1/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/csrc/ops/utils/tensor_utils.cpp` & `tvdcn-0.4.1/tvdcn/csrc/ops/utils/tensor_utils.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include <ATen/TensorUtils.h>
 
 namespace at {
-    static inline IntArrayRef definedPositions(ArrayRef<TensorArg> tensors) {
+    static inline std::vector<int64_t> definedPositions(ArrayRef<TensorArg> tensors) {
         std::vector<int64_t> res;
         res.reserve(tensors.size());
         for (const auto i: c10::irange(tensors.size())) {
             if (tensors[i]->defined())
                 res.emplace_back(i);
         }
         return res;
@@ -20,15 +20,15 @@
                 t.pos,
                 " '",
                 t.name,
                 "' to have ",
                 device_type,
                 " DeviceType, but got tensor with ",
                 t->device().type(),
-                " DeviceType (while checking arguments for ", c, ")");
+                " DeviceType (while checking arguments for ", c, ")")
     }
 
     void checkDeviceType(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors,
             DeviceType device_type) {
         for (const auto i: c10::irange(tensors.size())) {
@@ -37,16 +37,16 @@
     }
 
     void checkDeviceTypeExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors,
             DeviceType device_type) {
         auto defined_pos = definedPositions(tensors);
-        for (const auto i: c10::irange(defined_pos.size())) {
-            checkDeviceType(c, tensors[defined_pos[i]], device_type);
+        for (const auto i: defined_pos) {
+            checkDeviceType(c, tensors[i], device_type);
         }
     }
 
     void checkSameDeviceType(
             CheckedFrom c,
             const TensorArg &t1,
             const TensorArg &t2) {
@@ -80,16 +80,17 @@
 
     void checkAllSameDeviceTypeExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (const auto i: c10::irange(1, defined_pos.size())) {
-            checkSameDeviceType(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
+        auto t0 = tensors[defined_pos[0]];
+        for (auto iter = std::next(defined_pos.begin()); iter != defined_pos.end(); iter++) {
+            checkSameDeviceType(c, t0, tensors[*iter]);
         }
     }
 
     void checkSameDevice(
             CheckedFrom c,
             const TensorArg &t1,
             const TensorArg &t2) {
@@ -123,32 +124,35 @@
 
     void checkAllSameDeviceExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (const auto i: c10::irange(1, defined_pos.size())) {
-            checkSameDevice(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
+        auto t0 = tensors[defined_pos[0]];
+        for (auto iter = std::next(defined_pos.begin()); iter != defined_pos.end(); iter++) {
+            checkSameDevice(c, t0, tensors[*iter]);
         }
     }
 
     void checkAllSameGPUExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (const auto i: c10::irange(1, defined_pos.size())) {
-            checkSameGPU(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
+        auto t0 = tensors[defined_pos[0]];
+        for (auto iter = std::next(defined_pos.begin()); iter != defined_pos.end(); iter++) {
+            checkSameGPU(c, t0, tensors[*iter]);
         }
     }
 
     void checkAllSameTypeExceptUndefined(CheckedFrom c, ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (const auto i: c10::irange(1, defined_pos.size())) {
-            checkSameType(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
+        auto t0 = tensors[defined_pos[0]];
+        for (auto iter = std::next(defined_pos.begin()); iter != defined_pos.end(); iter++) {
+            checkSameType(c, t0, tensors[*iter]);
         }
     }
 }
```

### Comparing `tvdcn-0.4.0/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.4.1/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/extension.py` & `tvdcn-0.4.1/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.4.1/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.4.1/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/ops/deform_conv.py` & `tvdcn-0.4.1/tvdcn/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.4.1/tvdcn/ops/deform_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn/utils.py` & `tvdcn-0.4.1/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.0/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.4.1/tvdcn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.4.0
+Version: 0.4.1
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
-Keywords: deform_conv; deformable convolution
+Keywords: deform_conv,deform_conv_transposed,deformable_convolution,transposed_deformable_convolution
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tvdcn-0.4.0/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.4.1/tvdcn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

