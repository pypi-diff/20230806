# Comparing `tmp/EasyDeL-0.0.8.tar.gz` & `tmp/EasyDeL-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyDeL-0.0.8.tar", last modified: Thu Jul  6 04:44:31 2023, max compression
+gzip compressed data, was "EasyDeL-0.0.9.tar", last modified: Thu Jul  6 07:50:58 2023, max compression
```

## Comparing `EasyDeL-0.0.8.tar` & `EasyDeL-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.848134 EasyDeL-0.0.8/EasyDeL.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1512 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-06 04:44:31.000000 EasyDeL-0.0.8/EasyDeL.egg-info/top_level.txt
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1892 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/configs/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       91 2023-07-06 04:35:58.000000 EasyDeL-0.0.8/EasyDel/configs/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9145 2023-07-06 04:35:58.000000 EasyDeL-0.0.8/EasyDel/configs/configs.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1428 2023-07-06 04:25:19.000000 EasyDeL-0.0.8/EasyDel/modules/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/falcon/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.8/EasyDel/modules/falcon/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-29 05:59:18.000000 EasyDeL-0.0.8/EasyDel/modules/falcon/modelling_falcon_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/gpt_j/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_j/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.852134 EasyDeL-0.0.8/EasyDel/modules/llama/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.8/EasyDel/modules/llama/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 16:24:48.000000 EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_flax.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_pytorch.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-29 05:59:18.000000 EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.856134 EasyDeL-0.0.8/EasyDel/modules/opt/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-07-06 04:25:19.000000 EasyDeL-0.0.8/EasyDel/modules/opt/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    29993 2023-07-06 04:19:00.000000 EasyDeL-0.0.8/EasyDel/modules/opt/modelling_opt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/modules/palm/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-30 08:01:08.000000 EasyDeL-0.0.8/EasyDel/modules/palm/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16353 2023-06-30 07:08:03.000000 EasyDeL-0.0.8/EasyDel/modules/palm/modelling_palm_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/modules/t5/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       85 2023-07-06 04:19:25.000000 EasyDeL-0.0.8/EasyDel/modules/t5/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    59589 2023-06-30 07:56:15.000000 EasyDeL-0.0.8/EasyDel/modules/t5/modelling_t5_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/serve/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/serve/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/serve/serve_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/trainer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      219 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/trainer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8944 2023-06-29 08:35:15.000000 EasyDeL-0.0.8/EasyDel/trainer/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    22483 2023-07-06 04:19:25.000000 EasyDeL-0.0.8/EasyDel/trainer/fsdp_train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9443 2023-07-06 04:43:45.000000 EasyDeL-0.0.8/EasyDel/trainer/training_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.860134 EasyDeL-0.0.8/EasyDel/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/EasyDel/utils/checker.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.8/EasyDel/utils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/EasyDel/weight_convertor/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/falcon.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/llama.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/mpt.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.8/EasyDel/weight_convertor/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.8/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5471 2023-06-30 07:58:59.000000 EasyDeL-0.0.8/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.8/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-06 04:44:31.864133 EasyDeL-0.0.8/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-07-06 04:43:54.000000 EasyDeL-0.0.8/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.077553 EasyDeL-0.0.9/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.049553 EasyDeL-0.0.9/EasyDeL.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 07:50:57.000000 EasyDeL-0.0.9/EasyDeL.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1512 2023-07-06 07:50:57.000000 EasyDeL-0.0.9/EasyDeL.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-06 07:50:57.000000 EasyDeL-0.0.9/EasyDeL.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-06 07:50:57.000000 EasyDeL-0.0.9/EasyDeL.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-07-06 07:50:57.000000 EasyDeL-0.0.9/EasyDeL.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.049553 EasyDeL-0.0.9/EasyDel/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1892 2023-07-06 04:43:45.000000 EasyDeL-0.0.9/EasyDel/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.053553 EasyDeL-0.0.9/EasyDel/configs/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       91 2023-07-06 04:35:58.000000 EasyDeL-0.0.9/EasyDel/configs/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9047 2023-07-06 07:50:47.000000 EasyDeL-0.0.9/EasyDel/configs/configs.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.053553 EasyDeL-0.0.9/EasyDel/modules/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1428 2023-07-06 04:25:19.000000 EasyDeL-0.0.9/EasyDel/modules/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.053553 EasyDeL-0.0.9/EasyDel/modules/falcon/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.9/EasyDel/modules/falcon/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19533 2023-06-29 05:59:18.000000 EasyDeL-0.0.9/EasyDel/modules/falcon/modelling_falcon_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.057553 EasyDeL-0.0.9/EasyDel/modules/gpt_j/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/EasyDel/modules/gpt_j/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.057553 EasyDeL-0.0.9/EasyDel/modules/gpt_neo_x/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.9/EasyDel/modules/gpt_neo_x/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.9/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.057553 EasyDeL-0.0.9/EasyDel/modules/llama/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.9/EasyDel/modules/llama/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    34041 2023-06-27 16:24:48.000000 EasyDeL-0.0.9/EasyDel/modules/llama/modelling_llama_flax.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.9/EasyDel/modules/llama/modelling_llama_pytorch.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.061553 EasyDeL-0.0.9/EasyDel/modules/lucid_transformer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/EasyDel/modules/lucid_transformer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13472 2023-06-29 05:59:18.000000 EasyDeL-0.0.9/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.061553 EasyDeL-0.0.9/EasyDel/modules/mosaic_mpt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.9/EasyDel/modules/mosaic_mpt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.9/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.061553 EasyDeL-0.0.9/EasyDel/modules/opt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-07-06 04:25:19.000000 EasyDeL-0.0.9/EasyDel/modules/opt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    29993 2023-07-06 04:19:00.000000 EasyDeL-0.0.9/EasyDel/modules/opt/modelling_opt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.065553 EasyDeL-0.0.9/EasyDel/modules/palm/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-30 08:01:08.000000 EasyDeL-0.0.9/EasyDel/modules/palm/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16353 2023-06-30 07:08:03.000000 EasyDeL-0.0.9/EasyDel/modules/palm/modelling_palm_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.065553 EasyDeL-0.0.9/EasyDel/modules/t5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       85 2023-07-06 04:19:25.000000 EasyDeL-0.0.9/EasyDel/modules/t5/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    59589 2023-06-30 07:56:15.000000 EasyDeL-0.0.9/EasyDel/modules/t5/modelling_t5_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.065553 EasyDeL-0.0.9/EasyDel/serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.9/EasyDel/serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.9/EasyDel/serve/serve_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.069553 EasyDeL-0.0.9/EasyDel/trainer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      219 2023-07-06 04:43:45.000000 EasyDeL-0.0.9/EasyDel/trainer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8944 2023-06-29 08:35:15.000000 EasyDeL-0.0.9/EasyDel/trainer/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    22483 2023-07-06 04:19:25.000000 EasyDeL-0.0.9/EasyDel/trainer/fsdp_train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9443 2023-07-06 04:43:45.000000 EasyDeL-0.0.9/EasyDel/trainer/training_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.073553 EasyDeL-0.0.9/EasyDel/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/EasyDel/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/EasyDel/utils/checker.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.9/EasyDel/utils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-06 07:50:58.077553 EasyDeL-0.0.9/EasyDel/weight_convertor/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.9/EasyDel/weight_convertor/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.9/EasyDel/weight_convertor/falcon.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.9/EasyDel/weight_convertor/llama.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.9/EasyDel/weight_convertor/mpt.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.9/EasyDel/weight_convertor/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.9/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6365 2023-07-06 07:50:58.077553 EasyDeL-0.0.9/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5471 2023-06-30 07:58:59.000000 EasyDeL-0.0.9/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.9/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-06 07:50:58.077553 EasyDeL-0.0.9/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-07-06 07:50:54.000000 EasyDeL-0.0.9/setup.py
```

### Comparing `EasyDeL-0.0.8/EasyDeL.egg-info/PKG-INFO` & `EasyDeL-0.0.9/EasyDeL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `EasyDeL-0.0.8/EasyDeL.egg-info/SOURCES.txt` & `EasyDeL-0.0.9/EasyDeL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/__init__.py` & `EasyDeL-0.0.9/EasyDel/__init__.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/configs/configs.py` & `EasyDeL-0.0.9/EasyDel/configs/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,36 +206,36 @@
         "use_cache": True,
         "vocab_size": 65024
     }
 }
 
 opt_configs = {
     '1.3b': {
-        {
-            "activation_dropout": 0.0,
-            "activation_function": "relu",
-            "attention_dropout": 0.0,
-            "bos_token_id": 2,
-            "do_layer_norm_before": True,
-            "dropout": 0.1,
-            "eos_token_id": 2,
-            "ffn_dim": 8192,
-            "hidden_size": 2048,
-            "init_std": 0.02,
-            "layerdrop": 0.0,
-            "max_position_embeddings": 2048,
-            "model_type": "opt",
-            "num_attention_heads": 32,
-            "num_hidden_layers": 24,
-            "pad_token_id": 1,
-            "prefix": "</s>",
-            "use_cache": True,
-            "vocab_size": 50272,
-            "word_embed_proj_dim": 2048
-        }
+
+        "activation_dropout": 0.0,
+        "activation_function": "relu",
+        "attention_dropout": 0.0,
+        "bos_token_id": 2,
+        "do_layer_norm_before": True,
+        "dropout": 0.1,
+        "eos_token_id": 2,
+        "ffn_dim": 8192,
+        "hidden_size": 2048,
+        "init_std": 0.02,
+        "layerdrop": 0.0,
+        "max_position_embeddings": 2048,
+        "model_type": "opt",
+        "num_attention_heads": 32,
+        "num_hidden_layers": 24,
+        "pad_token_id": 1,
+        "prefix": "</s>",
+        "use_cache": True,
+        "vocab_size": 50272,
+        "word_embed_proj_dim": 2048
+
     },
     '6.7b': {
         "_remove_final_layer_norm": False,
         "activation_dropout": 0.0,
         "activation_function": "relu",
         "attention_dropout": 0.0,
         "bos_token_id": 2,
```

### Comparing `EasyDeL-0.0.8/EasyDel/modules/__init__.py` & `EasyDeL-0.0.9/EasyDel/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/falcon/modelling_falcon_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/falcon/modelling_falcon_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/llama/modelling_llama_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/llama/modelling_llama_pytorch.py` & `EasyDeL-0.0.9/EasyDel/modules/llama/modelling_llama_pytorch.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/lucid_transformer/modelling_lt_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/lucid_transformer/modelling_lt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/opt/modelling_opt_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/opt/modelling_opt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/palm/modelling_palm_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/palm/modelling_palm_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/modules/t5/modelling_t5_flax.py` & `EasyDeL-0.0.9/EasyDel/modules/t5/modelling_t5_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/serve/serve_utils.py` & `EasyDeL-0.0.9/EasyDel/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/trainer/config.py` & `EasyDeL-0.0.9/EasyDel/trainer/config.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/trainer/fsdp_train.py` & `EasyDeL-0.0.9/EasyDel/trainer/fsdp_train.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/trainer/training_utils.py` & `EasyDeL-0.0.9/EasyDel/trainer/training_utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/utils/utils.py` & `EasyDeL-0.0.9/EasyDel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/weight_convertor/falcon.py` & `EasyDeL-0.0.9/EasyDel/weight_convertor/falcon.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/weight_convertor/llama.py` & `EasyDeL-0.0.9/EasyDel/weight_convertor/llama.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/weight_convertor/mpt.py` & `EasyDeL-0.0.9/EasyDel/weight_convertor/mpt.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/EasyDel/weight_convertor/utils.py` & `EasyDeL-0.0.9/EasyDel/weight_convertor/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/LICENSE` & `EasyDeL-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/PKG-INFO` & `EasyDeL-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyDeL
-Version: 0.0.8
+Version: 0.0.9
 Summary: An open-source library to make training faster and more optimized in Jax/Flax
 Home-page: https://github.com/erfanzar/EasyDeL
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `EasyDeL-0.0.8/README.md` & `EasyDeL-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/pyproject.toml` & `EasyDeL-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.8/setup.py` & `EasyDeL-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyDeL',
-    version='0.0.8',
+    version='0.0.9',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description='An open-source library to make training faster and more optimized in Jax/Flax',
     url='https://github.com/erfanzar/EasyDeL',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

