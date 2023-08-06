# Comparing `tmp/nobuco-0.6.3.tar.gz` & `tmp/nobuco-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.6.3.tar", last modified: Wed Jul 26 22:37:10 2023, max compression
+gzip compressed data, was "nobuco-0.6.4.tar", last modified: Sun Aug  6 13:11:58 2023, max compression
```

## Comparing `nobuco-0.6.3.tar` & `nobuco-0.6.4.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.151925 nobuco-0.6.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-26 22:37:10.151925 nobuco-0.6.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.143925 nobuco-0.6.3/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      581 2023-07-25 20:58:16.000000 nobuco-0.6.3/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13988 2023-07-20 10:12:52.000000 nobuco-0.6.3/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.147925 nobuco-0.6.3/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-25 20:57:18.000000 nobuco-0.6.3/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.6.3/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-07-24 13:27:30.000000 nobuco-0.6.3/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4274 2023-07-24 13:14:20.000000 nobuco-0.6.3/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.147925 nobuco-0.6.3/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.147925 nobuco-0.6.3/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-07-24 13:29:19.000000 nobuco-0.6.3/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.3/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.147925 nobuco-0.6.3/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.151925 nobuco-0.6.3/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1192 2023-07-26 14:20:16.000000 nobuco-0.6.3/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    11813 2023-07-25 20:54:47.000000 nobuco-0.6.3/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1309 2023-07-26 14:39:38.000000 nobuco-0.6.3/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16532 2023-07-24 13:27:30.000000 nobuco-0.6.3/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2734 2023-07-26 14:33:48.000000 nobuco-0.6.3/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6506 2023-07-26 22:17:54.000000 nobuco-0.6.3/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.3/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4029 2023-07-23 08:12:26.000000 nobuco-0.6.3/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6726 2023-07-23 08:18:17.000000 nobuco-0.6.3/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11648 2023-07-26 14:22:14.000000 nobuco-0.6.3/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.151925 nobuco-0.6.3/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.3/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-23 20:33:27.000000 nobuco-0.6.3/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.151925 nobuco-0.6.3/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.3/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-26 22:37:10.147925 nobuco-0.6.3/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-07-26 22:37:10.000000 nobuco-0.6.3/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-07-26 22:37:10.000000 nobuco-0.6.3/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-26 22:37:10.000000 nobuco-0.6.3/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-07-26 22:37:10.000000 nobuco-0.6.3/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-07-26 22:37:10.000000 nobuco-0.6.3/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-07-26 14:20:52.000000 nobuco-0.6.3/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-26 22:37:10.151925 nobuco-0.6.3/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.659987 nobuco-0.6.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.6.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-08-06 13:11:58.659987 nobuco-0.6.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24311 2023-07-01 11:16:21.000000 nobuco-0.6.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.651987 nobuco-0.6.4/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      705 2023-07-31 09:28:25.000000 nobuco-0.6.4/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    14011 2023-08-06 11:12:53.000000 nobuco-0.6.4/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.651987 nobuco-0.6.4/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-07-25 20:57:18.000000 nobuco-0.6.4/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-08-06 12:41:35.000000 nobuco-0.6.4/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-07-24 13:27:30.000000 nobuco-0.6.4/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4298 2023-08-06 11:47:43.000000 nobuco-0.6.4/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.651987 nobuco-0.6.4/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.655987 nobuco-0.6.4/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-07-24 13:29:19.000000 nobuco-0.6.4/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      630 2023-08-06 11:12:41.000000 nobuco-0.6.4/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-07-20 18:19:12.000000 nobuco-0.6.4/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.655987 nobuco-0.6.4/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.659987 nobuco-0.6.4/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-08-06 10:51:45.000000 nobuco-0.6.4/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1192 2023-07-26 14:20:16.000000 nobuco-0.6.4/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    11813 2023-07-25 20:54:47.000000 nobuco-0.6.4/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1309 2023-07-26 14:39:38.000000 nobuco-0.6.4/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10177 2023-08-06 12:56:55.000000 nobuco-0.6.4/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2734 2023-07-26 14:33:48.000000 nobuco-0.6.4/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6506 2023-07-27 00:08:34.000000 nobuco-0.6.4/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8632 2023-08-06 13:10:36.000000 nobuco-0.6.4/nobuco/node_converters/reduce.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-07-11 12:35:48.000000 nobuco-0.6.4/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4029 2023-07-23 08:12:26.000000 nobuco-0.6.4/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6726 2023-07-23 08:18:17.000000 nobuco-0.6.4/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11648 2023-07-26 14:22:14.000000 nobuco-0.6.4/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.659987 nobuco-0.6.4/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-07-01 10:07:17.000000 nobuco-0.6.4/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10069 2023-07-23 20:33:27.000000 nobuco-0.6.4/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.659987 nobuco-0.6.4/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.6.4/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-08-06 13:11:58.651987 nobuco-0.6.4/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24897 2023-08-06 13:11:58.000000 nobuco-0.6.4/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1735 2023-08-06 13:11:58.000000 nobuco-0.6.4/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-08-06 13:11:58.000000 nobuco-0.6.4/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-08-06 13:11:58.000000 nobuco-0.6.4/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-08-06 13:11:58.000000 nobuco-0.6.4/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-08-06 13:10:58.000000 nobuco-0.6.4/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-08-06 13:11:58.659987 nobuco-0.6.4/setup.cfg
```

### Comparing `nobuco-0.6.3/LICENSE` & `nobuco-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/PKG-INFO` & `nobuco-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.3/README.md` & `nobuco-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/__init__.py` & `nobuco-0.6.4/nobuco/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from nobuco.converters.channel_ordering import t_pytorch2keras, t_keras2pytorch
+
 from nobuco.funcs import force_tensorflow_order, force_pytorch_order, shape
 from nobuco.locate.locate import locate_converter
 from nobuco.trace.trace import traceable
 
 from nobuco.converters.node_converter import converter, unregister_converter
 from nobuco.convert import pytorch_to_keras
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
@@ -13,10 +15,12 @@
     unregister_converter,
     traceable,
     ChannelOrder,
     ChannelOrderingStrategy,
     force_tensorflow_order,
     force_pytorch_order,
     shape,
-    locate_converter
+    locate_converter,
+    t_pytorch2keras,
+    t_keras2pytorch,
 ]
```

### Comparing `nobuco-0.6.3/nobuco/commons.py` & `nobuco-0.6.4/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/convert.py` & `nobuco-0.6.4/nobuco/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tensorflow import keras
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TF_TENSOR_CLASSES, TraceLevel
 from nobuco.converters.channel_ordering import t_pytorch2keras, set_channel_order, t_keras2pytorch
 from nobuco.converters.validation import validate, ValidationResult, ConversionResult
 from nobuco.layers.channel_order import ChangeOrderingLayer
 from nobuco.layers.container import TransientContainer
-from nobuco.layers.stub import UnimplementedOpStub
+from nobuco.layers.stub import UnimplementedOpStub, FailedConversionStub
 from nobuco.util import get_torch_tensor_identifier, collect_recursively, replace_recursively_func, \
     clone_torch_tensors_recursively
 from nobuco.entity.keras import KerasConvertedNode
 from nobuco.entity.pytorch import PytorchNode, PytorchNodeHierarchy
 from nobuco.trace.trace import Tracer
 from nobuco.converters.node_converter import CONVERTER_DICT, Pytorch2KerasNodeConverter
 from nobuco.vis.html_stylizer import HtmlStylizer
@@ -142,15 +142,15 @@
             node_converter: Pytorch2KerasNodeConverter = converter_dict.get(node.get_type(), None)
             try:
                 keras_op = convert_node(node, node_converter)
                 node_is_reusable = node_converter.reusable
             except Exception as e:
                 warnings.warn(f"Conversion exception on node '{node.get_type().__name__}': {e}")
                 traceback.print_exc()
-                keras_op = UnimplementedOpStub(node.get_op())
+                keras_op = FailedConversionStub(node.get_op())
             conversion_result = ConversionResult(converted_manually=True, converter=converter)
         elif len(children) > 0:
             children_converted_nodes = [convert(child, converted_op_dict, reuse_layers, full_validation, depth + 1) for child in children]
             keras_op = convert_container(node, children, children_converted_nodes, input_names, output_names, node.output_tensors, constants_to_variables=constants_to_variables)
 
             connectivity_status = keras_op.get_connectivity_status()
             if not connectivity_status.is_connected():
```

### Comparing `nobuco-0.6.3/nobuco/converters/channel_ordering.py` & `nobuco-0.6.4/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/converters/node_converter.py` & `nobuco-0.6.4/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/converters/tensor.py` & `nobuco-0.6.4/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/converters/type_cast.py` & `nobuco-0.6.4/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/converters/validation.py` & `nobuco-0.6.4/nobuco/converters/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,33 +80,33 @@
     # with torch.no_grad():
     #     outputs_pt = pytorch_op(*args_pt, **kwargs_pt)
     #     outputs_pt = collect_recursively(outputs_pt, torch.Tensor)
 
     if len(outputs_tf_converted) != len(outputs_pt):
         raise Exception(f"Number of outputs do not match: (Pytorch) {len(outputs_pt)} vs {len(outputs_tf_converted)} (Tensorflow)")
 
-    for t_tf, t_pt in zip(outputs_tf_converted, outputs_pt):
+    for i, (t_tf, t_pt) in enumerate(zip(outputs_tf_converted, outputs_pt)):
         if t_tf.shape != t_pt.shape:
-            raise Exception(f"Tensor shapes don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
+            raise Exception(f"Tensor shapes of output #{i} don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
 
         # if t_tf.dtype != t_pt.dtype:
         #     raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
 
     def calc_diff(t1, t2):
         def calc_diff_numerical(t1, t2):
             nan_mask = torch.isnan(t1) & torch.isnan(t2)
             diff = t1[~nan_mask] - t2[~nan_mask]
             if diff.numel() == 0:
                 return 0
             else:
-                return diff.abs().max().detach().cpu().numpy()
+                return diff.abs().max().numpy()
 
         def calc_diff_boolean(t1, t2):
             diff = t1 ^ t2
-            return diff.to(torch.float32).max()
+            return diff.to(torch.float32).max().numpy()
 
         if t1.numel() == t2.numel() == 0:
             return 0
 
         if t1.dtype == t2.dtype == torch.bool:
             return calc_diff_boolean(t1, t2)
         else:
```

### Comparing `nobuco-0.6.3/nobuco/entity/keras.py` & `nobuco-0.6.4/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/entity/pytorch.py` & `nobuco-0.6.4/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/funcs.py` & `nobuco-0.6.4/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/layers/channel_order.py` & `nobuco-0.6.4/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/layers/container.py` & `nobuco-0.6.4/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/layers/weight.py` & `nobuco-0.6.4/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/locate/link.py` & `nobuco-0.6.4/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/locate/locate.py` & `nobuco-0.6.4/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/activation.py` & `nobuco-0.6.4/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/attention.py` & `nobuco-0.6.4/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/boolean.py` & `nobuco-0.6.4/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/boolean_mask.py` & `nobuco-0.6.4/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/comparison.py` & `nobuco-0.6.4/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/convolution.py` & `nobuco-0.6.4/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/dropout.py` & `nobuco-0.6.4/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/interpolation.py` & `nobuco-0.6.4/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/linear.py` & `nobuco-0.6.4/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/misc.py` & `nobuco-0.6.4/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/normalization.py` & `nobuco-0.6.4/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/padding.py` & `nobuco-0.6.4/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/pooling.py` & `nobuco-0.6.4/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/recurrent.py` & `nobuco-0.6.4/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/slice.py` & `nobuco-0.6.4/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/tensor_cast.py` & `nobuco-0.6.4/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/tensor_creation.py` & `nobuco-0.6.4/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.6.4/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/trace/tensor_storage.py` & `nobuco-0.6.4/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/trace/trace.py` & `nobuco-0.6.4/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/util.py` & `nobuco-0.6.4/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/vis/console_stylizer.py` & `nobuco-0.6.4/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco/vis/html_stylizer.py` & `nobuco-0.6.4/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.6.3/nobuco.egg-info/PKG-INFO` & `nobuco-0.6.4/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.6.3
+Version: 0.6.4
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.6.3/nobuco.egg-info/SOURCES.txt` & `nobuco-0.6.4/nobuco.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 nobuco/node_converters/linear.py
 nobuco/node_converters/math.py
 nobuco/node_converters/misc.py
 nobuco/node_converters/normalization.py
 nobuco/node_converters/padding.py
 nobuco/node_converters/pooling.py
 nobuco/node_converters/recurrent.py
+nobuco/node_converters/reduce.py
 nobuco/node_converters/slice.py
 nobuco/node_converters/tensor_cast.py
 nobuco/node_converters/tensor_creation.py
 nobuco/node_converters/tensor_manipulation.py
 nobuco/node_converters/tensor_shape.py
 nobuco/node_converters/torchvision.py
 nobuco/trace/__init__.py
```

### Comparing `nobuco-0.6.3/pyproject.toml` & `nobuco-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.6.3"
+version = "0.6.4"
 description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

