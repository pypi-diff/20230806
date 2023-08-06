# Comparing `tmp/zhijian-0.0.1.tar.gz` & `tmp/zhijian-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhijian-0.0.1.tar", last modified: Wed Jul 19 02:17:22 2023, max compression
+gzip compressed data, was "zhijian-0.0.2.tar", last modified: Sun Aug  6 11:28:57 2023, max compression
```

## Comparing `zhijian-0.0.1.tar` & `zhijian-0.0.2.tar`

### file list

```diff
@@ -1,121 +1,127 @@
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.596327 zhijian-0.0.1/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      379 2023-07-19 02:17:22.596327 zhijian-0.0.1/PKG-INFO
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    48133 2023-07-18 12:32:53.000000 zhijian-0.0.1/README.md
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)       38 2023-07-19 02:17:22.596327 zhijian-0.0.1/setup.cfg
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      659 2023-07-19 02:15:27.000000 zhijian-0.0.1/setup.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.588328 zhijian-0.0.1/zhijian/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      122 2023-07-16 13:35:46.000000 zhijian-0.0.1/zhijian/__init__.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.588328 zhijian-0.0.1/zhijian/data/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      514 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/aid.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4032 2023-07-16 09:47:49.000000 zhijian-0.0.1/zhijian/data/aircraft.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    33368 2023-07-17 07:53:30.000000 zhijian-0.0.1/zhijian/data/base.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1125 2023-07-16 08:40:06.000000 zhijian-0.0.1/zhijian/data/caltech101.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2424 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/cars.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4550 2023-07-16 08:41:46.000000 zhijian-0.0.1/zhijian/data/config.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3422 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/cub2011.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4242 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/dogs.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     6642 2023-07-16 08:38:27.000000 zhijian-0.0.1/zhijian/data/domain.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2126 2023-07-16 09:34:50.000000 zhijian-0.0.1/zhijian/data/domainnet.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1607 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/dtd.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      903 2023-07-16 08:40:22.000000 zhijian-0.0.1/zhijian/data/eurosat.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2279 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/flowers.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4003 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/nabirds.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1938 2023-07-16 08:40:31.000000 zhijian-0.0.1/zhijian/data/officehome.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4802 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/oxford_iiit_pet.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2966 2023-07-16 08:38:19.000000 zhijian-0.0.1/zhijian/data/pacs.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4674 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/pcam.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1085 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/resisc45.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13513 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/smallnorb.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      904 2023-07-16 08:40:51.000000 zhijian-0.0.1/zhijian/data/sun397.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5574 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/data/template.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.588328 zhijian-0.0.1/zhijian/models/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 13:35:39.000000 zhijian-0.0.1/zhijian/models/__init__.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.588328 zhijian-0.0.1/zhijian/models/addin/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      103 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13431 2023-07-17 13:16:03.000000 zhijian-0.0.1/zhijian/models/addin/base.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/addin/module/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-17 14:13:45.000000 zhijian-0.0.1/zhijian/models/addin/module/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1543 2023-07-17 06:52:42.000000 zhijian-0.0.1/zhijian/models/addin/module/adapter.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2875 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/adaptformer.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      689 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/base.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2859 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/convpass.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3342 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/fact_tk.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4009 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/fact_tt.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1092 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/lora.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)       61 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/partial_k.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1963 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/ssf.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3103 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/addin/module/vpt.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5228 2023-07-17 06:59:04.000000 zhijian-0.0.1/zhijian/models/addin/module/vqt.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/backbone/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    17692 2023-07-17 14:49:25.000000 zhijian-0.0.1/zhijian/models/backbone/base.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/backbone/clip/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/clip/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1246 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/clip/utils.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      594 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/customized.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/backbone/timm/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/timm/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    20247 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/timm/arguments.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2118 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/backbone/timm/hooks.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1006 2023-07-17 07:53:17.000000 zhijian-0.0.1/zhijian/models/backbone/wrapper.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/configs/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/configs/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3738 2023-07-16 09:18:04.000000 zhijian-0.0.1/zhijian/models/configs/base.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/kd/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1966 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/base.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/kd/loss/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      742 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/ab.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1880 2023-07-16 09:42:21.000000 zhijian-0.0.1/zhijian/models/kd/loss/afd.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      899 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/at.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2624 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/bss.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1230 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/cc.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5078 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/crd.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      397 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/customized.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      620 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/dml.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      450 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/fitnet.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      970 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/fsp.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      727 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/ft.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3724 2023-07-16 09:42:30.000000 zhijian-0.0.1/zhijian/models/kd/loss/irg.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      377 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/logits.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1817 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/lwm.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1727 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/nst.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1726 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/ofd.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1715 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/pkt.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     6705 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/refilled.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2181 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/rkd.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1389 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/sobolev.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      730 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/sp.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      641 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/st.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2115 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/kd/loss/vid.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/regularization/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      761 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/base.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/regularization/loss/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      103 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/loss/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      461 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/loss/bss.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      316 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/loss/customized.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      874 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/loss/delta.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      917 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/regularization/loss/l2sp.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.592327 zhijian-0.0.1/zhijian/models/soup/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      103 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/soup/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/models/soup/base.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    19269 2023-07-18 01:30:35.000000 zhijian-0.0.1/zhijian/models/utils.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.596327 zhijian-0.0.1/zhijian/trainers/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/trainers/__init__.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     9024 2023-07-18 07:11:05.000000 zhijian-0.0.1/zhijian/trainers/base.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     7260 2023-07-18 07:06:26.000000 zhijian-0.0.1/zhijian/trainers/finetune.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    10713 2023-07-16 12:41:41.000000 zhijian-0.0.1/zhijian/trainers/knowledge_distillation.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13111 2023-07-16 03:14:28.000000 zhijian-0.0.1/zhijian/trainers/llm_config.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2580 2023-07-16 09:45:53.000000 zhijian-0.0.1/zhijian/trainers/llm_sft.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1010 2023-07-16 13:14:24.000000 zhijian-0.0.1/zhijian/trainers/model_soup.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4871 2023-07-17 07:49:40.000000 zhijian-0.0.1/zhijian/trainers/nearest_class_mean.py
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4918 2023-07-16 09:57:41.000000 zhijian-0.0.1/zhijian/trainers/regularization.py
-drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-07-19 02:17:22.588328 zhijian-0.0.1/zhijian.egg-info/
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      379 2023-07-19 02:17:22.000000 zhijian-0.0.1/zhijian.egg-info/PKG-INFO
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3170 2023-07-19 02:17:22.000000 zhijian-0.0.1/zhijian.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        1 2023-07-19 02:17:22.000000 zhijian-0.0.1/zhijian.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      100 2023-07-19 02:17:22.000000 zhijian-0.0.1/zhijian.egg-info/requires.txt
--rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        8 2023-07-19 02:17:22.000000 zhijian-0.0.1/zhijian.egg-info/top_level.txt
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      379 2023-08-06 11:28:57.792013 zhijian-0.0.2/PKG-INFO
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    29581 2023-08-06 11:15:56.000000 zhijian-0.0.2/README.md
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)       38 2023-08-06 11:28:57.792013 zhijian-0.0.2/setup.cfg
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      660 2023-08-06 11:28:46.000000 zhijian-0.0.2/setup.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      122 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/__init__.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/data/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      514 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/data/aid.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4032 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/data/aircraft.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    33938 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/data/base.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1125 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/data/caltech101.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2424 2023-08-06 11:15:56.000000 zhijian-0.0.2/zhijian/data/cars.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4570 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/config.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3422 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/cub2011.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4242 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/dogs.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     6642 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/domain.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2126 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/domainnet.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1607 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/dtd.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      903 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/eurosat.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2279 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/flowers.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4003 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/nabirds.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1938 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/officehome.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4802 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/oxford_iiit_pet.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2966 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/pacs.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4674 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/pcam.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1085 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/resisc45.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13513 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/smallnorb.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      904 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/sun397.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5574 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/data/template.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/models/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/models/__init__.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/models/addin/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/addin/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13431 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/addin/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/models/addin/module/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1543 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/adapter.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2875 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/adaptformer.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      689 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/base.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2859 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/convpass.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3342 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/fact_tk.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4009 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/fact_tt.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1092 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/lora.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)       61 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/partial_k.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1963 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/ssf.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3103 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/vpt.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5228 2023-08-06 11:16:01.000000 zhijian-0.0.2/zhijian/models/addin/module/vqt.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/models/backbone/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/backbone/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    17857 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/backbone/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian/models/backbone/clip/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:02.000000 zhijian-0.0.2/zhijian/models/backbone/clip/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1246 2023-08-06 11:16:02.000000 zhijian-0.0.2/zhijian/models/backbone/clip/utils.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     8016 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/backbone/customized.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/backbone/timm/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:02.000000 zhijian-0.0.2/zhijian/models/backbone/timm/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    20246 2023-08-06 11:16:02.000000 zhijian-0.0.2/zhijian/models/backbone/timm/arguments.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2118 2023-08-06 11:16:02.000000 zhijian-0.0.2/zhijian/models/backbone/timm/hooks.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1006 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/backbone/wrapper.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/configs/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/configs/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3850 2023-08-06 11:15:59.000000 zhijian-0.0.2/zhijian/models/configs/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/kd/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/kd/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1966 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/kd/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/kd/loss/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      742 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/ab.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1880 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/afd.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      899 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/at.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2624 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/bss.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1230 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/cc.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     5078 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/crd.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      397 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/customized.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      620 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/dml.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      450 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/fitnet.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      970 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/fsp.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      727 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/ft.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3724 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/irg.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      377 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/logits.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1817 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/lwm.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1727 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/nst.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1726 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/ofd.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1715 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/pkt.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     6705 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/refilled.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2181 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/rkd.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     1389 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/sobolev.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      730 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/sp.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      641 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/st.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2115 2023-08-06 11:16:03.000000 zhijian-0.0.2/zhijian/models/kd/loss/vid.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/model_merging/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/model_merging/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      460 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/model_merging/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/model_merging/method/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/model_merging/method/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    11869 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/model_merging/method/gamf.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    75672 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/model_merging/method/ot.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    14618 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/model_merging/method/repair.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      138 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/model_merging/method/soup.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/regularization/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/regularization/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      761 2023-08-06 11:16:00.000000 zhijian-0.0.2/zhijian/models/regularization/base.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/models/regularization/loss/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/regularization/loss/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      461 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/regularization/loss/bss.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      316 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/regularization/loss/customized.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      874 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/regularization/loss/delta.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      917 2023-08-06 11:16:04.000000 zhijian-0.0.2/zhijian/models/regularization/loss/l2sp.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    20173 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/models/utils.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.792013 zhijian-0.0.2/zhijian/trainers/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/__init__.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     9024 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/base.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     7460 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/finetune.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    10625 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/knowledge_distillation.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)    13111 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/llm_config.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     2250 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/llm_sft.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     9090 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/model_merging.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4880 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/nearest_class_mean.py
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     4918 2023-08-06 11:15:57.000000 zhijian-0.0.2/zhijian/trainers/regularization.py
+drwxr-xr-x   0 zhangyk   (1008) lamda3   (10000)        0 2023-08-06 11:28:57.788012 zhijian-0.0.2/zhijian.egg-info/
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      379 2023-08-06 11:28:57.000000 zhijian-0.0.2/zhijian.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)     3415 2023-08-06 11:28:57.000000 zhijian-0.0.2/zhijian.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        1 2023-08-06 11:28:57.000000 zhijian-0.0.2/zhijian.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)      100 2023-08-06 11:28:57.000000 zhijian-0.0.2/zhijian.egg-info/requires.txt
+-rw-r--r--   0 zhangyk   (1008) lamda3   (10000)        8 2023-08-06 11:28:57.000000 zhijian-0.0.2/zhijian.egg-info/top_level.txt
```

### Comparing `zhijian-0.0.1/setup.py` & `zhijian-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zhijian',
-    version='0.0.1',
+    version='0.0.2',
     description='ZhiJian: A Unifying and Rapidly Deployable Toolbox for Pre-trained Model Reuse',
     author='ZhiJian Contributors',
     author_email='yumzhangyk@gmail.com',
     packages=find_packages(),
     keywords='pytorch pretrained model reuse',
     url='https://github.com/zhangyikaii/LAMDA-ZhiJian',
     install_requires=[
@@ -17,8 +17,8 @@
         'tensorboardX',
         'torch>=1.7',
         'torchvision',
         'tqdm',
         'transformers',
     ],
     python_requires='>=3.7',
-)
+)
```

### Comparing `zhijian-0.0.1/zhijian/data/aid.py` & `zhijian-0.0.2/zhijian/data/aid.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/aircraft.py` & `zhijian-0.0.2/zhijian/data/aircraft.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/base.py` & `zhijian-0.0.2/zhijian/data/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 from zhijian.models.utils import load_pickle, save_pickle, MyImageFolderDataset
+from zhijian.models.configs.base import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from zhijian.data.config import DATA_PATH_SUB_DIR, DATASET2NUM_CLASSES, IGNORE_INDEX
+from zhijian.data.template import Template
 
 import torch
 from torch.utils.data.sampler import Sampler
 import random
 
 from tqdm import tqdm
 
@@ -22,25 +24,23 @@
 
 
 from itertools import chain
 import hashlib
 
 from datasets import Dataset, concatenate_datasets, load_dataset
 
-from zhijian.data.template import Template
 
 
 class TestAugTransform:
     def __init__(self, transform, aug_times):
         self.transform = transform
         self.aug_times = aug_times
     def __call__(self, x):
         return [self.transform(x) for _ in range(self.aug_times)]
 
-
 def get_in_train_transform(dataset, crop_size, mean, std):
     if dataset in ['CLEVR-Distance', 'CLEVR-Count', 'smallNORB-Azimuth', 'smallNORB-Elevation', 'dSprites-Orientation', 'dSprites-Location', 'KITTI']:
          return transforms.Compose([
             transforms.Resize((224, 224), interpolation=3),
             transforms.ToTensor(),
             transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])])
     else:
@@ -54,16 +54,21 @@
         ])
 
 def get_in_test_transform(dataset, resize_size, crop_size, mean, std):
     if dataset in ['CLEVR-Distance', 'CLEVR-Count', 'smallNORB-Azimuth', 'smallNORB-Elevation', 'dSprites-Orientation', 'dSprites-Location', 'KITTI']:
         return transforms.Compose([
             transforms.Resize((224, 224), interpolation=3),
             transforms.ToTensor(),
-            transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])])
+            transforms.Normalize(mean=IMAGENET_DEFAULT_MEAN, std=IMAGENET_DEFAULT_STD)])
     else:
+        if resize_size is None and crop_size is None:
+            return transforms.Compose([
+                torchvision.transforms.ToTensor(),
+                torchvision.transforms.Normalize(mean=mean, std=std),
+            ])
         return transforms.Compose([
             transforms.Resize(resize_size),
             transforms.CenterCrop(crop_size),
             transforms.ToTensor(),
             transforms.Normalize(
                 mean=mean, std=std
             )
@@ -74,16 +79,15 @@
     raw_dataset = re.sub(remove_pattern, '', args.dataset)
 
     if hasattr(model_args, 'preprocess'):
         train_transform = model_args.preprocess
         val_transform = model_args.preprocess
     else:
         train_transform = get_in_train_transform(raw_dataset, model_args.input_size[1], model_args.mean, model_args.std)
-        val_transform = get_in_test_transform(raw_dataset, 256, model_args.input_size[1], model_args.mean, model_args.std)
-
+        val_transform = get_in_test_transform(raw_dataset, model_args.resize_size, model_args.input_size[1], model_args.mean, model_args.std)
 
     train_dataset, val_dataset, num_classes = get_dataset(args.dataset, os.path.join(args.dataset_dir, DATA_PATH_SUB_DIR[args.dataset]), train_transform, val_transform, logger)
 
     train_loader = torch.utils.data.DataLoader(
         train_dataset,
         batch_size=args.batch_size,
         num_workers=args.num_workers,
@@ -101,14 +105,22 @@
 
 
     return train_loader, val_loader, num_classes
 
 
 class general_vtab_dataset(ImageFolder):
     def __init__(self, name, root, train=True, transform=None, **kwargs):
+        """write the description of the function here, like this is the ...
+
+        write the description of the function here
+
+        :param a1: write parameter a1 description here
+
+        :return: write return thing here
+        """
         self.dataset_root = root
         self.loader = default_loader
         self.target_transform = None
         self.transform = transform
 
         if 'VTAB-1k' in name:
             train_list_path = os.path.join(self.dataset_root, 'train800val200.txt')
@@ -161,19 +173,19 @@
         train_dataset = None
         val_dataset = general_imageneta_dataset(data_path, transform=val_transform)
         num_classes = 200
     elif name == 'ImageNet-R':
         train_dataset = None
         val_dataset = general_imageneta_dataset(data_path, transform=val_transform)
         num_classes = 200
-    elif name == 'CIFAR10':
+    elif name == 'CIFAR-10':
         train_dataset = torchvision.datasets.CIFAR10(root=data_path, train=True, download=False, transform=train_transform)
         val_dataset = torchvision.datasets.CIFAR10(root=data_path, train=False, download=False, transform=val_transform)
         num_classes = 10
-    elif name == 'CIFAR100':
+    elif name == 'CIFAR-100':
         train_dataset = torchvision.datasets.CIFAR100(root=data_path, train=True, download=False, transform=train_transform)
         val_dataset = torchvision.datasets.CIFAR100(root=data_path, train=False, download=False, transform=val_transform)
         num_classes = 100
     elif name == 'Aircraft':
         from zhijian.data.aircraft import Aircraft
         train_dataset = Aircraft(data_path, transform=train_transform, train=True, download=False)
         val_dataset = Aircraft(data_path, transform=val_transform, train=False, download=False)
```

### Comparing `zhijian-0.0.1/zhijian/data/caltech101.py` & `zhijian-0.0.2/zhijian/data/caltech101.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/cars.py` & `zhijian-0.0.2/zhijian/data/cars.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/config.py` & `zhijian-0.0.2/zhijian/data/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         889, 895, 907, 928, 931, 932, 933, 934, 936, 937, 943, 945, 947, 948, 949, 951, 953, 954, 957, 963, 965,
         967, 980, 981,
         983, 988]
 }
 
 
 DATASET2NUM_CLASSES = {
+    'CIFAR-10': 10,
     'CIFAR-100': 100,
     'CLEVR-Count': 8,
     'CLEVR-Distance': 6,
     'Caltech101': 102,
     'DTD': 47,
     'Diabetic-Retinopathy': 5,
     'Dmlab': 6,
```

### Comparing `zhijian-0.0.1/zhijian/data/cub2011.py` & `zhijian-0.0.2/zhijian/data/cub2011.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/dogs.py` & `zhijian-0.0.2/zhijian/data/dogs.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/domain.py` & `zhijian-0.0.2/zhijian/data/domain.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/domainnet.py` & `zhijian-0.0.2/zhijian/data/domainnet.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/dtd.py` & `zhijian-0.0.2/zhijian/data/dtd.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/eurosat.py` & `zhijian-0.0.2/zhijian/data/eurosat.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/flowers.py` & `zhijian-0.0.2/zhijian/data/flowers.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/nabirds.py` & `zhijian-0.0.2/zhijian/data/nabirds.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/officehome.py` & `zhijian-0.0.2/zhijian/data/officehome.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/oxford_iiit_pet.py` & `zhijian-0.0.2/zhijian/data/oxford_iiit_pet.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/pacs.py` & `zhijian-0.0.2/zhijian/data/pacs.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/pcam.py` & `zhijian-0.0.2/zhijian/data/pcam.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/resisc45.py` & `zhijian-0.0.2/zhijian/data/resisc45.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/smallnorb.py` & `zhijian-0.0.2/zhijian/data/smallnorb.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/sun397.py` & `zhijian-0.0.2/zhijian/data/sun397.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/data/template.py` & `zhijian-0.0.2/zhijian/data/template.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/base.py` & `zhijian-0.0.2/zhijian/models/addin/base.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/adapter.py` & `zhijian-0.0.2/zhijian/models/addin/module/adapter.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/adaptformer.py` & `zhijian-0.0.2/zhijian/models/addin/module/adaptformer.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/base.py` & `zhijian-0.0.2/zhijian/models/addin/module/base.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/convpass.py` & `zhijian-0.0.2/zhijian/models/addin/module/convpass.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/fact_tk.py` & `zhijian-0.0.2/zhijian/models/addin/module/fact_tk.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/fact_tt.py` & `zhijian-0.0.2/zhijian/models/addin/module/fact_tt.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/lora.py` & `zhijian-0.0.2/zhijian/models/addin/module/lora.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/ssf.py` & `zhijian-0.0.2/zhijian/models/addin/module/ssf.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/vpt.py` & `zhijian-0.0.2/zhijian/models/addin/module/vpt.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/addin/module/vqt.py` & `zhijian-0.0.2/zhijian/models/addin/module/vqt.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/backbone/base.py` & `zhijian-0.0.2/zhijian/models/backbone/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 import torch.nn as nn
 
-from zhijian.models.utils import dict2args, get_class_from_module
+from zhijian.models.utils import dict2args, get_class_from_module, safe_update
 from zhijian.models.configs.base import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from zhijian.models.backbone.wrapper import ModelWrapper
 
 from zhijian.data.config import DATASET2NUM_CLASSES
 
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
 
 from copy import deepcopy
 
 import os
 from zhijian.trainers.llm_config import FinetuningArguments
 from transformers import AutoTokenizer, AutoConfig, BitsAndBytesConfig, AutoModelForCausalLM
 from typing import Literal, Optional, Tuple
@@ -108,47 +108,43 @@
                 add_layer.register_forward_pre_hook(cur_hook)
             elif i_hook[1] == 'post':
                 add_layer.register_forward_hook(cur_hook)
             else:
                 raise NotImplementedError
 
 
-def prepare_pretrained(model, pretrained_urls, soup_mode=None, logger=None):
+def prepare_pretrained(model, pretrained_urls, logger=None):
     updated_keys = defaultdict(set)
     model_dict = model.state_dict()
     num_pretrained = len(pretrained_urls)
     if num_pretrained == 0:
         return
     for idx, cur_pretrained_url in enumerate(pretrained_urls):
         pretrained_dict = torch.load(cur_pretrained_url, map_location='cpu')
         if isinstance(pretrained_dict, dict):
-            keys_to_check = ['model', 'state_dict']
+            keys_to_check = ['model', 'state_dict', 'model_state_dict']
             matching_key = next((key for key in keys_to_check if key in pretrained_dict), None)
             if matching_key is not None:
                 pretrained_dict = pretrained_dict[matching_key]
+        
         pretrained_dict = {k: v.to(next(model.parameters()).device) for k, v in pretrained_dict.items()}
 
-        def _fine_tune_params_dict(cur_d, cur_soup_mode):
+        def _fine_tune_params_dict(cur_d):
             ret_d = deepcopy(model_dict)
             for k_idx, k in enumerate(model_dict.keys()):
                 if k in cur_d.keys() and cur_d[k].shape == model_dict[k].shape:
-                    if cur_soup_mode == 'differential' and not torch.equal(cur_d[k], model_dict[k]):
+                    if not torch.equal(cur_d[k], model_dict[k]):
                         if idx != 0 and k in updated_keys[idx - 1]:
                             logger.warning(f'{k} is overwritten in the {idx} iteration')
                         ret_d[k] = cur_d[k]
                         updated_keys[idx].add(k)
 
-                    elif cur_soup_mode == 'uniform_soup':
-                        if k_idx == 0:
-                            ret_d[k] = cur_d[k] * (1./num_pretrained)
-                        else:
-                            ret_d[k] = cur_d[k] * (1./num_pretrained) + ret_d[k]
             return ret_d
 
-        model_dict = _fine_tune_params_dict(pretrained_dict, soup_mode)
+        model_dict = _fine_tune_params_dict(pretrained_dict)
 
     model.load_state_dict(model_dict)
     for i in updated_keys.keys():
         logger.info(f"Loaded parameters (file {i}): [{', '.join(updated_keys[i])}]")
 
 
 
@@ -252,48 +248,65 @@
                 nn.init.zeros_(model.heads.head.weight)
                 nn.init.zeros_(model.heads.head.bias)
 
         model_args.update({
             'input_size': (model.image_size, model.image_size)
         })
 
+
     elif args.model.startswith('clip.'):
         import clip
         from zhijian.models.backbone.clip.utils import CLIPModelWrapper
         model, preprocess = clip.load(args.model.replace('clip.', ''))
 
         model = CLIPModelWrapper(model)
         if args.model == 'clip.ViT-B/32':
             model_args.update({
                 # 'dtype': model.dtype,
                 # 'ln_final_weight': model.ln_final_weight,
                 # 'visual_input_size': model.visual_input_size,
                 'preprocess': preprocess,
             })
-
+ 
     elif args.model.startswith('customized.'):
-        from zhijian.models.backbone.customized import MyModels
-        model = MyModels[args.model.replace('customized.', '')](args, num_classes=DATASET2NUM_CLASSES[cur_dataset])
+        from zhijian.models.backbone.customized import MyModels 
+        model = MyModels[args.model.replace('customized.', '')](
+            args,
+            num_classes=DATASET2NUM_CLASSES[cur_dataset],
+            **{k: v for k, v in kwargs.items() if k not in ['model_args']}
+        )
+
+        if hasattr(model, "image_size"):
+            model_args.update({
+                'input_size': (model.image_size, model.image_size)
+            })
 
-        model_args.update({
-            'input_size': (model.image_size, model.image_size)
-        })
     else:
         assert False, f'Unkown model type {args.model}'
 
-
     if not args.model.startswith('clip.'):
         model = ModelWrapper(model)
 
+    if 'model_args' in kwargs.keys():
+        model_args.update(kwargs['model_args'])
+
+    if 'mean' not in model_args.keys() and 'std' not in model_args.keys():
+        model_args.update({
+            
+        })
+    safe_update(
+        model_args,
+        {'mean': IMAGENET_DEFAULT_MEAN, 'std': IMAGENET_DEFAULT_STD, 'resize_size': 224}
+    )
+
     model_args = dict2args(model_args)
 
     return model, model_args
 
 
-# load_pretrained
 def prepare_llm(
     model_args,
     finetuning_args,
     is_trainable: Optional[bool] = False,
     stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft",
     logger=None
 ) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
@@ -347,15 +360,14 @@
             config_kwargs["load_in_4bit"] = True
             config_kwargs["quantization_config"] = BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_compute_dtype=model_args.compute_dtype,
                 bnb_4bit_use_double_quant=model_args.double_quantization,
                 bnb_4bit_quant_type=model_args.quantization_type
             )
-        is_mergeable = False
         config_kwargs["device_map"] = {"": int(os.environ.get("LOCAL_RANK", "0"))}
         if logger is not None:
             logger.info("Quantizing model to {} bit.".format(model_args.quantization_bit))
 
     if not is_trainable: # `device_map=auto` should be used for inference only
         config_kwargs["device_map"] = "auto"
```

### Comparing `zhijian-0.0.1/zhijian/models/backbone/clip/utils.py` & `zhijian-0.0.2/zhijian/models/backbone/clip/utils.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/backbone/timm/arguments.py` & `zhijian-0.0.2/zhijian/models/backbone/timm/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,8 +272,7 @@
     group.add_argument("--local_rank", default=0, type=int)
     group.add_argument('--use-multi-epochs-loader', action='store_true', default=False,
                     help='use the multi-epochs-loader to save time at the beginning of every epoch')
     group.add_argument('--log-wandb', action='store_true', default=False,
                     help='log training and validation metrics to wandb')
 
     return parser
-
```

### Comparing `zhijian-0.0.1/zhijian/models/backbone/timm/hooks.py` & `zhijian-0.0.2/zhijian/models/backbone/timm/hooks.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/backbone/wrapper.py` & `zhijian-0.0.2/zhijian/models/backbone/wrapper.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/configs/base.py` & `zhijian-0.0.2/zhijian/models/configs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-IN1K_CLASSES = 1000
+customize_pre_trained_modelIN1K_CLASSES = 1000
 
 TQDM_BAR_FORMAT = '{l_bar}{bar:10}{r_bar}'  # tqdm bar format
 
 DATA_PATH_PREFIX = '/data/zhangyk/data'
 DATA_PATHS = {
     'ImageNet': f'{DATA_PATH_PREFIX}/imagenet',
-    'CIFAR10': f'{DATA_PATH_PREFIX}/cifar10',
-    'CIFAR100': f'{DATA_PATH_PREFIX}/cifar100',
+    'CIFAR-10': f'{DATA_PATH_PREFIX}/cifar10',
+    'CIFAR-100': f'{DATA_PATH_PREFIX}/cifar100',
     'Aircraft': f'{DATA_PATH_PREFIX}/aircraft',
     'Caltech101': f'{DATA_PATH_PREFIX}/caltech101/caltech-101',
     'Cars': f'{DATA_PATH_PREFIX}/cars',
     'CUB2011': f'{DATA_PATH_PREFIX}/cub2011',
     'Dogs': f'{DATA_PATH_PREFIX}/dogs',
     'DomainNet': f'{DATA_PATH_PREFIX}/domainnet',
     'DTD': f'{DATA_PATH_PREFIX}/dtd',
@@ -44,14 +44,16 @@
 IMAGENET_DEFAULT_STD = (0.229, 0.224, 0.225)
 IMAGENET_INCEPTION_MEAN = (0.5, 0.5, 0.5)
 IMAGENET_INCEPTION_STD = (0.5, 0.5, 0.5)
 IMAGENET_DPN_MEAN = (124 / 255, 117 / 255, 104 / 255)
 IMAGENET_DPN_STD = tuple([1 / (.0167 * 255)] * 3)
 OPENAI_CLIP_MEAN = (0.48145466, 0.4578275, 0.40821073)
 OPENAI_CLIP_STD = (0.26862954, 0.26130258, 0.27577711)
+FB_RESNET_MEAN = (0.4914, 0.4822, 0.4465)
+FB_RESNET_STD = (0.2023, 0.1994, 0.2010)
 
 try:
     from torchvision.transforms.functional import InterpolationMode
     has_interpolation_mode = True
 except ImportError:
     has_interpolation_mode = False
```

### Comparing `zhijian-0.0.1/zhijian/models/kd/base.py` & `zhijian-0.0.2/zhijian/models/kd/base.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/ab.py` & `zhijian-0.0.2/zhijian/models/kd/loss/ab.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/afd.py` & `zhijian-0.0.2/zhijian/models/kd/loss/afd.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/at.py` & `zhijian-0.0.2/zhijian/models/kd/loss/at.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/bss.py` & `zhijian-0.0.2/zhijian/models/kd/loss/bss.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/cc.py` & `zhijian-0.0.2/zhijian/models/kd/loss/cc.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/crd.py` & `zhijian-0.0.2/zhijian/models/kd/loss/crd.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/dml.py` & `zhijian-0.0.2/zhijian/models/kd/loss/dml.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/fsp.py` & `zhijian-0.0.2/zhijian/models/kd/loss/fsp.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/ft.py` & `zhijian-0.0.2/zhijian/models/kd/loss/ft.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/irg.py` & `zhijian-0.0.2/zhijian/models/kd/loss/irg.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/lwm.py` & `zhijian-0.0.2/zhijian/models/kd/loss/lwm.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/nst.py` & `zhijian-0.0.2/zhijian/models/kd/loss/nst.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/ofd.py` & `zhijian-0.0.2/zhijian/models/kd/loss/ofd.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/pkt.py` & `zhijian-0.0.2/zhijian/models/kd/loss/pkt.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/refilled.py` & `zhijian-0.0.2/zhijian/models/kd/loss/refilled.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/rkd.py` & `zhijian-0.0.2/zhijian/models/kd/loss/rkd.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/sobolev.py` & `zhijian-0.0.2/zhijian/models/kd/loss/sobolev.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/sp.py` & `zhijian-0.0.2/zhijian/models/kd/loss/sp.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/st.py` & `zhijian-0.0.2/zhijian/models/kd/loss/st.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/kd/loss/vid.py` & `zhijian-0.0.2/zhijian/models/kd/loss/vid.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/regularization/base.py` & `zhijian-0.0.2/zhijian/models/regularization/base.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/regularization/loss/delta.py` & `zhijian-0.0.2/zhijian/models/regularization/loss/delta.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/regularization/loss/l2sp.py` & `zhijian-0.0.2/zhijian/models/regularization/loss/l2sp.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/models/utils.py` & `zhijian-0.0.2/zhijian/models/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -536,14 +536,15 @@
     def warning(self, message):
         logging.warning(message)
 
     def info(self, message):
         logging.info(message)
 
 
+
 class LogHandle(object):
     def __init__(self, args):
         self.args = args
         self.save_path = Path(os.path.join(args.log_url, args.time_str))
         self.save_path.mkdir(parents=True, exist_ok=True)
         self.logger = Logger(args, self.save_path, 'INFO')
 
@@ -604,13 +605,36 @@
         return self.data.get(k, None)
 
 def dict2args(d):
     cur_args = argparse.Namespace()
     cur_args.__dict__.update(d)
     return cur_args
 
+def safe_update(d, d_prime):
+    for k, v in d_prime.items():
+        if k not in d.keys():
+            d.update({k: v})
+
 def get_class_from_module(module_name, class_name):
     try:
         module = importlib.import_module(module_name)
         return getattr(module, class_name)
     except ModuleNotFoundError:
         return None
+
+def select_from_input(prompt_for_select, valid_selections):
+    selections2print = '\n\t'.join([f'[{idx + 1}] {i}' for idx, i in enumerate(valid_selections)])
+    while True:
+        selected = input(f"Please input a {prompt_for_select}, type 'help' to show the options: ")
+
+        if selected == 'help':
+            print(f"Available {prompt_for_select}(s):\n\t{selections2print}")
+        elif selected.isdigit() and int(selected) >= 1 and int(selected) <= len(valid_selections):
+            selected = valid_selections[int(selected) - 1]
+            break
+        elif selected in valid_selections:
+            break
+        else:
+            print("Sorry, input not support.")
+            print(f"Available {prompt_for_select}(s):\n\t{selections2print}")
+
+    return selected
```

### Comparing `zhijian-0.0.1/zhijian/trainers/base.py` & `zhijian-0.0.2/zhijian/trainers/base.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/trainers/finetune.py` & `zhijian-0.0.2/zhijian/trainers/finetune.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,47 +31,54 @@
         model_args=None,
         train_loader=None,
         val_loader=None,
         num_classes=None,
         optimizer=None,
         lr_scheduler=None,
         criterion=None,
-        device=None
+        device=None,
+        **kwargs
         ):
         set_seed(args.seed)
         self.logger = LogHandle(args)
 
+        pretrained_loaded_flag = False
         if None in [model, model_args, device]:
             self.model, self.model_args = prepare_model(args, self.logger)
             self.addins, self.fixed_params = prepare_addins(args, self.model_args)
+            if 'preloaded' in kwargs.keys():
+                kwargs['preloaded'](self.model, self.addins, args.pretrained_url)
+                pretrained_loaded_flag = True
             prepare_hook(args.addins, self.addins, self.model, 'addin')
             prepare_gradient(args.reuse_keys, self.model, self.logger)
             self.device = prepare_cuda(self.model)
             self.logger.info(f'Training with a single process on 1 device ({self.device})')
         else:
             self.model, self.model_args, self.device = model, model_args, device
 
         if None in [train_loader, val_loader, num_classes]:
             self.train_loader, self.val_loader, self.num_classes = prepare_vision_dataloader(args, self.model_args, self.logger)
         else:
             self.train_loader, self.val_loader, self.num_classes = train_loader, val_loader, num_classes
 
+        if not pretrained_loaded_flag:
+            prepare_pretrained(self.model, args.pretrained_url, self.logger)
+
         if None in [optimizer, lr_scheduler]:
             prepare_optim_handle = PrepareFunc(args)
             self.optimizer, self.lr_scheduler = prepare_optim_handle.prepare_optimizer(self.model)
         else:
             self.optimizer, self.lr_scheduler = optimizer, lr_scheduler
 
         if criterion is None:
             prepare_optim_handle = PrepareFunc(args)
             self.criterion = prepare_optim_handle.prepare_criterion()
         else:
             self.criterion = criterion
 
-        prepare_pretrained(self.model, args.pretrained_url, 'differential' if args.training_mode != 'model_soup' else args.soup_mode, self.logger)
 
         self.lr, self.batch_size = args.lr, args.batch_size
         self.verbose, self.max_epoch, self.only_do_test = args.verbose, args.max_epoch, args.only_do_test
         self.dataset = args.dataset
 
         self.args = args
```

### Comparing `zhijian-0.0.1/zhijian/trainers/knowledge_distillation.py` & `zhijian-0.0.2/zhijian/trainers/knowledge_distillation.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         ):
         super().__init__(args, model, model_args, train_loader, val_loader, num_classes, optimizer, lr_scheduler, criterion, device)
 
         args.t_args = prepare_args(args.t_args, update_default=True)
         self.t_model, t_model_args = prepare_model(args.t_args, self.logger)
         self.t_addins, self.t_fixed_params = prepare_addins(args.t_args, t_model_args)
         prepare_hook(args.t_args.addins, self.t_addins, self.t_model, 'addin')
-        prepare_pretrained(self.t_model, args.t_args.pretrained_url, 'differential' if args.t_args.training_mode != 'model_soup' else args.t_args.soup_mode, self.logger)
+        prepare_pretrained(self.t_model, args.t_args.pretrained_url, self.logger)
 
 
 class Trainer(TwinPTMTrainer):
     def __init__(
         self, args,
         model=None,
         model_args=None,
```

### Comparing `zhijian-0.0.1/zhijian/trainers/llm_config.py` & `zhijian-0.0.2/zhijian/trainers/llm_config.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian/trainers/llm_sft.py` & `zhijian-0.0.2/zhijian/trainers/llm_sft.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-from zhijian.models.backbone.base import prepare_llm, prepare_hook, prepare_gradient, prepare_cuda, prepare_pretrained
-from zhijian.models.addin.base import prepare_addins
+from zhijian.models.backbone.base import prepare_llm
 from zhijian.data.base import prepare_llm_dataset, preprocess_llm_dataset, DynamicDataCollatorWithPadding
-from zhijian.models.configs.base import TQDM_BAR_FORMAT
-from zhijian.models.utils import AverageMeter, accuracy, PrepareFunc, LogHandle, set_seed
-
-import time
-import torch
-from contextlib import suppress
-import os
-from copy import deepcopy
-
-from tqdm import tqdm
+from zhijian.models.utils import LogHandle, set_seed
 
 def prepare_specific_trainer_parser(parser):
-
     return parser
 
 
 class Trainer(object):
     def __init__(
         self, args,
         model=None,
```

### Comparing `zhijian-0.0.1/zhijian/trainers/nearest_class_mean.py` & `zhijian-0.0.2/zhijian/trainers/nearest_class_mean.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         criterion=None,
         device=None
         ):
         super().__init__(args, model, model_args, train_loader, val_loader, num_classes, optimizer, lr_scheduler, criterion, device)
         cur_ncm_hook = HOOKS[args.model.replace('timm.', '')]()
         prepare_hook(cur_ncm_hook.get_feature_hook_info(), [cur_ncm_hook], self.model, 'hook')
 
+        
         self.shot_transform = self.args.shot_transform
         self.metric = self.args.metric
         self.temperature = self.args.temperature
 
     def fit(self):
         self.prototypes = compute_prototypes(self.model, self.train_loader, self.num_classes, self.device, self.verbose, self.logger)
```

### Comparing `zhijian-0.0.1/zhijian/trainers/regularization.py` & `zhijian-0.0.2/zhijian/trainers/regularization.py`

 * *Files identical despite different names*

### Comparing `zhijian-0.0.1/zhijian.egg-info/SOURCES.txt` & `zhijian-0.0.2/zhijian.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -78,25 +78,30 @@
 zhijian/models/kd/loss/pkt.py
 zhijian/models/kd/loss/refilled.py
 zhijian/models/kd/loss/rkd.py
 zhijian/models/kd/loss/sobolev.py
 zhijian/models/kd/loss/sp.py
 zhijian/models/kd/loss/st.py
 zhijian/models/kd/loss/vid.py
+zhijian/models/model_merging/__init__.py
+zhijian/models/model_merging/base.py
+zhijian/models/model_merging/method/__init__.py
+zhijian/models/model_merging/method/gamf.py
+zhijian/models/model_merging/method/ot.py
+zhijian/models/model_merging/method/repair.py
+zhijian/models/model_merging/method/soup.py
 zhijian/models/regularization/__init__.py
 zhijian/models/regularization/base.py
 zhijian/models/regularization/loss/__init__.py
 zhijian/models/regularization/loss/bss.py
 zhijian/models/regularization/loss/customized.py
 zhijian/models/regularization/loss/delta.py
 zhijian/models/regularization/loss/l2sp.py
-zhijian/models/soup/__init__.py
-zhijian/models/soup/base.py
 zhijian/trainers/__init__.py
 zhijian/trainers/base.py
 zhijian/trainers/finetune.py
 zhijian/trainers/knowledge_distillation.py
 zhijian/trainers/llm_config.py
 zhijian/trainers/llm_sft.py
-zhijian/trainers/model_soup.py
+zhijian/trainers/model_merging.py
 zhijian/trainers/nearest_class_mean.py
 zhijian/trainers/regularization.py
```

