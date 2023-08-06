# Comparing `tmp/monai-weekly-1.3.dev2331.tar.gz` & `tmp/monai-weekly-1.3.dev2332.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.3.dev2331.tar", last modified: Sun Jul 30 02:18:15 2023, max compression
+gzip compressed data, was "monai-weekly-1.3.dev2332.tar", last modified: Sun Aug  6 02:12:36 2023, max compression
```

## Comparing `monai-weekly-1.3.dev2331.tar` & `monai-weekly-1.3.dev2332.tar`

### file list

```diff
@@ -1,1152 +1,1160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.674950 monai-weekly-1.3.dev2331/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-30 02:16:21.000000 monai-weekly-1.3.dev2331/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 02:18:15.674950 monai-weekly-1.3.dev2331/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.326950 monai-weekly-1.3.dev2331/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.330950 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    41979 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.334950 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.338950 monai-weekly-1.3.dev2331/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.338950 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.342950 monai-weekly-1.3.dev2331/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.342950 monai-weekly-1.3.dev2331/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.346950 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.350950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.354950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.358950 monai-weekly-1.3.dev2331/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.362950 monai-weekly-1.3.dev2331/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.366950 monai-weekly-1.3.dev2331/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.374950 monai-weekly-1.3.dev2331/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    78913 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/ultrasound_confidence_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.378950 monai-weekly-1.3.dev2331/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.382950 monai-weekly-1.3.dev2331/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.394950 monai-weekly-1.3.dev2331/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.394950 monai-weekly-1.3.dev2331/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.398950 monai-weekly-1.3.dev2331/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/cldice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46558 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.406950 monai-weekly-1.3.dev2331/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    42239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.406950 monai-weekly-1.3.dev2331/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.418950 monai-weekly-1.3.dev2331/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.422950 monai-weekly-1.3.dev2331/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.434950 monai-weekly-1.3.dev2331/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.434950 monai-weekly-1.3.dev2331/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.442950 monai-weekly-1.3.dev2331/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.442950 monai-weekly-1.3.dev2331/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75075 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    61070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    82785 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.446950 monai-weekly-1.3.dev2331/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.450950 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.454950 monai-weekly-1.3.dev2331/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179715 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   127506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.454950 monai-weekly-1.3.dev2331/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    81426 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.458950 monai-weekly-1.3.dev2331/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.462950 monai-weekly-1.3.dev2331/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.462950 monai-weekly-1.3.dev2331/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34514 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 02:18:15.000000 monai-weekly-1.3.dev2331/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 02:18:15.670950 monai-weekly-1.3.dev2331/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cldice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gdsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_ultrasound_confidence_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-07-30 02:16:18.000000 monai-weekly-1.3.dev2331/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.704421 monai-weekly-1.3.dev2332/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-08-06 02:12:36.704421 monai-weekly-1.3.dev2332/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.708421 monai-weekly-1.3.dev2332/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-06 02:10:46.000000 monai-weekly-1.3.dev2332/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.272413 monai-weekly-1.3.dev2332/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.272413 monai-weekly-1.3.dev2332/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-06 02:12:36.708421 monai-weekly-1.3.dev2332/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.276413 monai-weekly-1.3.dev2332/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.280413 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37154 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27506 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.280413 monai-weekly-1.3.dev2332/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.280413 monai-weekly-1.3.dev2332/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41979 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.280413 monai-weekly-1.3.dev2332/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.284413 monai-weekly-1.3.dev2332/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.284413 monai-weekly-1.3.dev2332/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53640 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.284413 monai-weekly-1.3.dev2332/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69282 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.288413 monai-weekly-1.3.dev2332/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.288413 monai-weekly-1.3.dev2332/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.292413 monai-weekly-1.3.dev2332/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48577 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.292413 monai-weekly-1.3.dev2332/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.292413 monai-weekly-1.3.dev2332/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.292413 monai-weekly-1.3.dev2332/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.292413 monai-weekly-1.3.dev2332/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.296413 monai-weekly-1.3.dev2332/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.296413 monai-weekly-1.3.dev2332/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.296413 monai-weekly-1.3.dev2332/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.296413 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.296413 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.300413 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.300413 monai-weekly-1.3.dev2332/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.300413 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.300413 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.304413 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.304413 monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.304413 monai-weekly-1.3.dev2332/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.308414 monai-weekly-1.3.dev2332/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.312414 monai-weekly-1.3.dev2332/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64632 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.312414 monai-weekly-1.3.dev2332/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.324414 monai-weekly-1.3.dev2332/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78883 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/ultrasound_confidence_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65554 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49494 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.324414 monai-weekly-1.3.dev2332/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.324414 monai-weekly-1.3.dev2332/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.328414 monai-weekly-1.3.dev2332/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33232 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.328414 monai-weekly-1.3.dev2332/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.340414 monai-weekly-1.3.dev2332/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22501 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.340414 monai-weekly-1.3.dev2332/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.348414 monai-weekly-1.3.dev2332/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/cldice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46558 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.356414 monai-weekly-1.3.dev2332/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42239 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.356414 monai-weekly-1.3.dev2332/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.364415 monai-weekly-1.3.dev2332/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.368415 monai-weekly-1.3.dev2332/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.384415 monai-weekly-1.3.dev2332/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40667 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47132 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.388415 monai-weekly-1.3.dev2332/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.392415 monai-weekly-1.3.dev2332/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37090 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.396415 monai-weekly-1.3.dev2332/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75075 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61070 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.396415 monai-weekly-1.3.dev2332/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112239 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82785 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.396415 monai-weekly-1.3.dev2332/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25374 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.400415 monai-weekly-1.3.dev2332/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.400415 monai-weekly-1.3.dev2332/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.400415 monai-weekly-1.3.dev2332/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40802 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.404415 monai-weekly-1.3.dev2332/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.404415 monai-weekly-1.3.dev2332/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.404415 monai-weekly-1.3.dev2332/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   183594 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131629 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.408415 monai-weekly-1.3.dev2332/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70963 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76167 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81426 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.412415 monai-weekly-1.3.dev2332/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29761 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.416416 monai-weekly-1.3.dev2332/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.416416 monai-weekly-1.3.dev2332/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34780 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 02:12:36.000000 monai-weekly-1.3.dev2332/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-08-06 02:12:36.708421 monai-weekly-1.3.dev2332/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:12:36.704421 monai-weekly-1.3.dev2332/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cldice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25175 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gdsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23754 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_perceptual_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_simulate_low_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_simulate_low_resolutiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23814 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_ultrasound_confidence_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26104 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-08-06 02:10:43.000000 monai-weekly-1.3.dev2332/versioneer.py
```

### Comparing `monai-weekly-1.3.dev2331/LICENSE` & `monai-weekly-1.3.dev2332/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/PKG-INFO` & `monai-weekly-1.3.dev2332/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2331
+Version: 1.3.dev2332
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -58,14 +58,15 @@
 Provides-Extra: pynrrd
 Provides-Extra: pydicom
 Provides-Extra: h5py
 Provides-Extra: nni
 Provides-Extra: optuna
 Provides-Extra: onnx
 Provides-Extra: zarr
+Provides-Extra: lpips
 License-File: LICENSE
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/MONAI-logo-color.png" width="50%" alt='project-monai'>
 </p>
 
 **M**edical **O**pen **N**etwork for **AI**
```

### Comparing `monai-weekly-1.3.dev2331/README.md` & `monai-weekly-1.3.dev2332/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/__init__.py` & `monai-weekly-1.3.dev2332/monai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "5feb353030e0bb204e21e1de338cd81b5972bb8a"
+__commit_id__ = "65cf5fe1234d0d01cc52c9ab48395a3efbad6f45"
```

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/__init__.py` & `monai-weekly-1.3.dev2332/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.3.dev2332/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/_extensions/loader.py` & `monai-weekly-1.3.dev2332/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/auto_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/bundle_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/ensemble_builder.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/datasets.py` & `monai-weekly-1.3.dev2332/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepedit/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepedit/interaction.py` & `monai-weekly-1.3.dev2332/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepedit/transforms.py` & `monai-weekly-1.3.dev2332/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.3.dev2332/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.3.dev2332/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.3.dev2332/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/array.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.3.dev2332/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/mmars/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/mmars/mmars.py` & `monai-weekly-1.3.dev2332/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/mmars/model_desc.py` & `monai-weekly-1.3.dev2332/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nnunet/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nnunet/__main__.py` & `monai-weekly-1.3.dev2332/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.3.dev2332/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nnunet/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nuclick/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/nuclick/transforms.py` & `monai-weekly-1.3.dev2332/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/pathology/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.3.dev2332/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/tcia/__init__.py` & `monai-weekly-1.3.dev2332/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/tcia/label_desc.py` & `monai-weekly-1.3.dev2332/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/tcia/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/apps/utils.py` & `monai-weekly-1.3.dev2332/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/__init__.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/analyzer.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/operations.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/auto3dseg/utils.py` & `monai-weekly-1.3.dev2332/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/__init__.py` & `monai-weekly-1.3.dev2332/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/__main__.py` & `monai-weekly-1.3.dev2332/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/config_item.py` & `monai-weekly-1.3.dev2332/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/config_parser.py` & `monai-weekly-1.3.dev2332/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/properties.py` & `monai-weekly-1.3.dev2332/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/reference_resolver.py` & `monai-weekly-1.3.dev2332/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/scripts.py` & `monai-weekly-1.3.dev2332/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/utils.py` & `monai-weekly-1.3.dev2332/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/bundle/workflows.py` & `monai-weekly-1.3.dev2332/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/config/__init__.py` & `monai-weekly-1.3.dev2332/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/config/deviceconfig.py` & `monai-weekly-1.3.dev2332/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/config/type_definitions.py` & `monai-weekly-1.3.dev2332/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/__init__.py` & `monai-weekly-1.3.dev2332/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/box_utils.py` & `monai-weekly-1.3.dev2332/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/csv_saver.py` & `monai-weekly-1.3.dev2332/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/dataloader.py` & `monai-weekly-1.3.dev2332/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/dataset.py` & `monai-weekly-1.3.dev2332/monai/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1596,15 +1596,15 @@
             data_item_md5 = self.hash_func(item_transformed).decode("utf-8")
             data_item_md5 += self.transform_hash
             hashfile = self.cache_dir / f"{data_item_md5}.pt"
 
         if hashfile is not None and hashfile.is_file():  # cache hit
             with cp.cuda.Device(self.device):
                 if isinstance(item_transformed, dict):
-                    item: dict[Any, Any] = {}  # type:ignore
+                    item: dict[Any, Any] = {}
                     for k in item_transformed:
                         meta_k = self._load_meta_cache(meta_hash_file_name=f"{hashfile.name}-{k}-meta")
                         item[k] = kvikio_numpy.fromfile(f"{hashfile}-{k}", dtype=meta_k["dtype"], like=cp.empty(()))
                         item[k] = convert_to_tensor(item[k].reshape(meta_k["shape"]), device=f"cuda:{self.device}")
                         item[f"{k}_meta_dict"] = meta_k
                     return item
                 elif isinstance(item_transformed, (np.ndarray, torch.Tensor)):
@@ -1684,8 +1684,8 @@
         except PermissionError:  # project-monai/monai issue #3613
             pass
 
     def _load_meta_cache(self, meta_hash_file_name):
         if meta_hash_file_name in self._meta_cache:
             return self._meta_cache[meta_hash_file_name]
         else:
-            return torch.load(self.cache_dir / meta_hash_file_name)  # type:ignore
+            return torch.load(self.cache_dir / meta_hash_file_name)
```

### Comparing `monai-weekly-1.3.dev2331/monai/data/dataset_summary.py` & `monai-weekly-1.3.dev2332/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/decathlon_datalist.py` & `monai-weekly-1.3.dev2332/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/fft_utils.py` & `monai-weekly-1.3.dev2332/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/folder_layout.py` & `monai-weekly-1.3.dev2332/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/grid_dataset.py` & `monai-weekly-1.3.dev2332/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/image_dataset.py` & `monai-weekly-1.3.dev2332/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/image_reader.py` & `monai-weekly-1.3.dev2332/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/image_writer.py` & `monai-weekly-1.3.dev2332/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/iterable_dataset.py` & `monai-weekly-1.3.dev2332/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/itk_torch_bridge.py` & `monai-weekly-1.3.dev2332/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/meta_obj.py` & `monai-weekly-1.3.dev2332/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/meta_tensor.py` & `monai-weekly-1.3.dev2332/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/samplers.py` & `monai-weekly-1.3.dev2332/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/synthetic.py` & `monai-weekly-1.3.dev2332/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/test_time_augmentation.py` & `monai-weekly-1.3.dev2332/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/thread_buffer.py` & `monai-weekly-1.3.dev2332/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/torchscript_utils.py` & `monai-weekly-1.3.dev2332/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/ultrasound_confidence_map.py` & `monai-weekly-1.3.dev2332/monai/data/ultrasound_confidence_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/utils.py` & `monai-weekly-1.3.dev2332/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/video_dataset.py` & `monai-weekly-1.3.dev2332/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/wsi_datasets.py` & `monai-weekly-1.3.dev2332/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/data/wsi_reader.py` & `monai-weekly-1.3.dev2332/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/__init__.py` & `monai-weekly-1.3.dev2332/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/evaluator.py` & `monai-weekly-1.3.dev2332/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.3.dev2332/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/trainer.py` & `monai-weekly-1.3.dev2332/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/utils.py` & `monai-weekly-1.3.dev2332/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/engines/workflow.py` & `monai-weekly-1.3.dev2332/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/__init__.py` & `monai-weekly-1.3.dev2332/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/client/__init__.py` & `monai-weekly-1.3.dev2332/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/client/client_algo.py` & `monai-weekly-1.3.dev2332/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/client/monai_algo.py` & `monai-weekly-1.3.dev2332/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/utils/__init__.py` & `monai-weekly-1.3.dev2332/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/utils/constants.py` & `monai-weekly-1.3.dev2332/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/utils/exchange_object.py` & `monai-weekly-1.3.dev2332/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/fl/utils/filters.py` & `monai-weekly-1.3.dev2332/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/__init__.py` & `monai-weekly-1.3.dev2332/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.3.dev2332/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.3.dev2332/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/classification_saver.py` & `monai-weekly-1.3.dev2332/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/clearml_handlers.py` & `monai-weekly-1.3.dev2332/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/confusion_matrix.py` & `monai-weekly-1.3.dev2332/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/decollate_batch.py` & `monai-weekly-1.3.dev2332/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/earlystop_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/garbage_collector.py` & `monai-weekly-1.3.dev2332/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.3.dev2332/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/ignite_metric.py` & `monai-weekly-1.3.dev2332/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/logfile_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/mean_dice.py` & `monai-weekly-1.3.dev2332/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/mean_iou.py` & `monai-weekly-1.3.dev2332/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/metric_logger.py` & `monai-weekly-1.3.dev2332/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/metrics_saver.py` & `monai-weekly-1.3.dev2332/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/mlflow_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.3.dev2332/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/panoptic_quality.py` & `monai-weekly-1.3.dev2332/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.3.dev2332/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/postprocessing.py` & `monai-weekly-1.3.dev2332/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/probability_maps.py` & `monai-weekly-1.3.dev2332/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/regression_metrics.py` & `monai-weekly-1.3.dev2332/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/roc_auc.py` & `monai-weekly-1.3.dev2332/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/smartcache_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/stats_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/surface_distance.py` & `monai-weekly-1.3.dev2332/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.3.dev2332/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/utils.py` & `monai-weekly-1.3.dev2332/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/handlers/validation_handler.py` & `monai-weekly-1.3.dev2332/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/inferers/__init__.py` & `monai-weekly-1.3.dev2332/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/inferers/inferer.py` & `monai-weekly-1.3.dev2332/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/inferers/merger.py` & `monai-weekly-1.3.dev2332/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/inferers/splitter.py` & `monai-weekly-1.3.dev2332/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/inferers/utils.py` & `monai-weekly-1.3.dev2332/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/__init__.py` & `monai-weekly-1.3.dev2332/monai/losses/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from .adversarial_loss import PatchAdversarialLoss
 from .cldice import SoftclDiceLoss, SoftDiceclDiceLoss
 from .contrastive import ContrastiveLoss
 from .deform import BendingEnergyLoss
 from .dice import (
     Dice,
     DiceCELoss,
     DiceFocalLoss,
@@ -30,11 +31,13 @@
     generalized_wasserstein_dice,
 )
 from .ds_loss import DeepSupervisionLoss
 from .focal_loss import FocalLoss
 from .giou_loss import BoxGIoULoss, giou
 from .image_dissimilarity import GlobalMutualInformationLoss, LocalNormalizedCrossCorrelationLoss
 from .multi_scale import MultiScaleLoss
+from .perceptual import PerceptualLoss
 from .spatial_mask import MaskedLoss
+from .spectral_loss import JukeboxLoss
 from .ssim_loss import SSIMLoss
 from .tversky import TverskyLoss
 from .unified_focal_loss import AsymmetricUnifiedFocalLoss
```

### Comparing `monai-weekly-1.3.dev2331/monai/losses/cldice.py` & `monai-weekly-1.3.dev2332/monai/losses/cldice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/contrastive.py` & `monai-weekly-1.3.dev2332/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/deform.py` & `monai-weekly-1.3.dev2332/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/dice.py` & `monai-weekly-1.3.dev2332/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/ds_loss.py` & `monai-weekly-1.3.dev2332/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/focal_loss.py` & `monai-weekly-1.3.dev2332/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/giou_loss.py` & `monai-weekly-1.3.dev2332/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/image_dissimilarity.py` & `monai-weekly-1.3.dev2332/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/multi_scale.py` & `monai-weekly-1.3.dev2332/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/spatial_mask.py` & `monai-weekly-1.3.dev2332/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/ssim_loss.py` & `monai-weekly-1.3.dev2332/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/tversky.py` & `monai-weekly-1.3.dev2332/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/losses/unified_focal_loss.py` & `monai-weekly-1.3.dev2332/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/__init__.py` & `monai-weekly-1.3.dev2332/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.3.dev2332/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/confusion_matrix.py` & `monai-weekly-1.3.dev2332/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/cumulative_average.py` & `monai-weekly-1.3.dev2332/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/f_beta_score.py` & `monai-weekly-1.3.dev2332/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/froc.py` & `monai-weekly-1.3.dev2332/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/generalized_dice.py` & `monai-weekly-1.3.dev2332/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.3.dev2332/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/loss_metric.py` & `monai-weekly-1.3.dev2332/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/meandice.py` & `monai-weekly-1.3.dev2332/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/meaniou.py` & `monai-weekly-1.3.dev2332/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/metric.py` & `monai-weekly-1.3.dev2332/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/panoptic_quality.py` & `monai-weekly-1.3.dev2332/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/regression.py` & `monai-weekly-1.3.dev2332/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/rocauc.py` & `monai-weekly-1.3.dev2332/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/surface_dice.py` & `monai-weekly-1.3.dev2332/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/surface_distance.py` & `monai-weekly-1.3.dev2332/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/utils.py` & `monai-weekly-1.3.dev2332/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/metrics/wrapper.py` & `monai-weekly-1.3.dev2332/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/__init__.py` & `monai-weekly-1.3.dev2332/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/__init__.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/activation.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/aspp.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/convolutions.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/crf.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/denseblock.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/dints_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/downsample.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/encoder.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/fcn.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/mlp.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/selfattention.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/text_embedding.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/upsample.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/blocks/warp.py` & `monai-weekly-1.3.dev2332/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/__init__.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/convutils.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/drop_path.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/factories.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/filtering.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/gmm.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/simplelayers.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/utils.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/layers/weight_init.py` & `monai-weekly-1.3.dev2332/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/__init__.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/ahnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/attentionunet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/autoencoder.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/basic_unet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/classifier.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/daf3d.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/densenet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/dints.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/dynunet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/efficientnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/generator.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/highresnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/hovernet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/milmodel.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/netadapter.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/quicknat.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/regressor.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/regunet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/resnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/segresnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/senet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/transchex.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/unet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/unetr.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/vit.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/vitautoenc.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/nets/vnet.py` & `monai-weekly-1.3.dev2332/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/networks/utils.py` & `monai-weekly-1.3.dev2332/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/optimizers/__init__.py` & `monai-weekly-1.3.dev2332/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/optimizers/lr_finder.py` & `monai-weekly-1.3.dev2332/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.3.dev2332/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/optimizers/novograd.py` & `monai-weekly-1.3.dev2332/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/optimizers/utils.py` & `monai-weekly-1.3.dev2332/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,14 +377,15 @@
     RandAxisFlip,
     RandDeformGrid,
     RandFlip,
     RandGridDistortion,
     RandGridPatch,
     RandRotate,
     RandRotate90,
+    RandSimulateLowResolution,
     RandZoom,
     Resample,
     ResampleToMatch,
     Resize,
     Rotate,
     Rotate90,
     Spacing,
@@ -433,14 +434,17 @@
     RandGridPatchDict,
     RandRotate90d,
     RandRotate90D,
     RandRotate90Dict,
     RandRotated,
     RandRotateD,
     RandRotateDict,
+    RandSimulateLowResolutiond,
+    RandSimulateLowResolutionD,
+    RandSimulateLowResolutionDict,
     RandZoomd,
     RandZoomD,
     RandZoomDict,
     ResampleToMatchd,
     ResampleToMatchD,
     ResampleToMatchDict,
     Resized,
```

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/adaptors.py` & `monai-weekly-1.3.dev2332/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/compose.py` & `monai-weekly-1.3.dev2332/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/croppad/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/croppad/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/croppad/batch.py` & `monai-weekly-1.3.dev2332/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/croppad/functional.py` & `monai-weekly-1.3.dev2332/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/intensity/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/intensity/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/inverse.py` & `monai-weekly-1.3.dev2332/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.3.dev2332/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/io/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/io/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/io/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/lazy/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/lazy/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/lazy/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/lazy/functional.py` & `monai-weekly-1.3.dev2332/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/lazy/utils.py` & `monai-weekly-1.3.dev2332/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/nvtx.py` & `monai-weekly-1.3.dev2332/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/post/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/post/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/post/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/signal/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/signal/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/spatial/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/spatial/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/spatial/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Any, Optional, Sequence, Tuple, Union, cast
 
 import numpy as np
 import torch
 
 from monai.config import USE_COMPILED, DtypeLike
 from monai.config.type_definitions import NdarrayOrTensor
-from monai.data.meta_obj import get_track_meta
+from monai.data.meta_obj import get_track_meta, set_track_meta
 from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import AFFINE_TOL, affine_to_spacing, compute_shape_offset, iter_patch, to_affine_nd, zoom_affine
 from monai.networks.layers import AffineTransform, GaussianFilter, grid_pull
 from monai.networks.utils import meshgrid_ij
 from monai.transforms.croppad.array import CenterSpatialCrop, ResizeWithPadOrCrop
 from monai.transforms.inverse import InvertibleTransform
 from monai.transforms.spatial.functional import (
@@ -107,14 +107,15 @@
     "RandAffineGrid",
     "RandDeformGrid",
     "Resample",
     "Affine",
     "RandAffine",
     "Rand2DElastic",
     "Rand3DElastic",
+    "RandSimulateLowResolution",
 ]
 
 RandRange = Optional[Union[Sequence[Union[Tuple[float, float], float]], float]]
 
 
 class SpatialResample(InvertibleTransform, LazyTransform):
     """
@@ -3452,7 +3453,99 @@
             raise ValueError(f'`sort_fn` should be either "min", "max", "random" or None! {self.sort_fn} provided!')
         return super().filter_count(image_np, locations)
 
     def __call__(self, array: NdarrayOrTensor, randomize: bool = True):
         if randomize:
             self.randomize(array)
         return super().__call__(array)
+
+
+class RandSimulateLowResolution(RandomizableTransform):
+    """
+    Random simulation of low resolution corresponding to nnU-Net's SimulateLowResolutionTransform
+    (https://github.com/MIC-DKFZ/batchgenerators/blob/7651ece69faf55263dd582a9f5cbd149ed9c3ad0/batchgenerators/transforms/resample_transforms.py#L23)
+    First, the array/tensor is resampled at lower resolution as determined by the zoom_factor which is uniformly sampled
+    from the `zoom_range`. Then, the array/tensor is resampled at the original resolution.
+    """
+
+    backend = Affine.backend
+
+    def __init__(
+        self,
+        prob: float = 0.1,
+        downsample_mode: InterpolateMode | str = InterpolateMode.NEAREST,
+        upsample_mode: InterpolateMode | str = InterpolateMode.TRILINEAR,
+        zoom_range: Sequence[float] = (0.5, 1.0),
+        align_corners=False,
+        device: torch.device | None = None,
+    ) -> None:
+        """
+        Args:
+            prob: probability of performing this augmentation
+            downsample_mode: interpolation mode for downsampling operation
+            upsample_mode: interpolation mode for upsampling operation
+            zoom_range: range from which the random zoom factor for the downsampling and upsampling operation is
+            sampled. It determines the shape of the downsampled tensor.
+            align_corners: This only has an effect when downsample_mode or upsample_mode  is 'linear', 'bilinear',
+                'bicubic' or 'trilinear'. Default: False
+                See also: https://pytorch.org/docs/stable/generated/torch.nn.functional.interpolate.html
+            device: device on which the tensor will be allocated.
+
+        """
+        RandomizableTransform.__init__(self, prob)
+
+        self.downsample_mode = downsample_mode
+        self.upsample_mode = upsample_mode
+        self.zoom_range = zoom_range
+        self.align_corners = align_corners
+        self.device = device
+        self.zoom_factor = 1.0
+
+    def randomize(self, data: Any | None = None) -> None:
+        super().randomize(None)
+        self.zoom_factor = self.R.uniform(self.zoom_range[0], self.zoom_range[1])
+        if not self._do_transform:
+            return None
+
+    def __call__(self, img: torch.Tensor, randomize: bool = True) -> torch.Tensor:
+        """
+        Args:
+            img: shape must be (num_channels, H, W[, D]),
+            randomize: whether to execute `randomize()` function first, defaults to True.
+        """
+        if randomize:
+            self.randomize()
+
+        if self._do_transform:
+            input_shape = img.shape[1:]
+            target_shape = np.round(np.array(input_shape) * self.zoom_factor).astype(np.int_)
+
+            resize_tfm_downsample = Resize(
+                spatial_size=target_shape, size_mode="all", mode=self.downsample_mode, anti_aliasing=False
+            )
+
+            resize_tfm_upsample = Resize(
+                spatial_size=input_shape,
+                size_mode="all",
+                mode=self.upsample_mode,
+                anti_aliasing=False,
+                align_corners=self.align_corners,
+            )
+            # temporarily disable metadata tracking, since we do not want to invert the two Resize functions during
+            # post-processing
+            original_tack_meta_value = get_track_meta()
+            set_track_meta(False)
+
+            img_downsampled = resize_tfm_downsample(img)
+            img_upsampled = resize_tfm_upsample(img_downsampled)
+
+            # reset metadata tracking to original value
+            set_track_meta(original_tack_meta_value)
+
+            # copy metadata from original image to down-and-upsampled image
+            img_upsampled = MetaTensor(img_upsampled)
+            img_upsampled.copy_meta_from(img)
+
+            return img_upsampled
+
+        else:
+            return img
```

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/spatial/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     Rand2DElastic,
     Rand3DElastic,
     RandAffine,
     RandAxisFlip,
     RandGridDistortion,
     RandGridPatch,
     RandRotate,
+    RandSimulateLowResolution,
     RandZoom,
     ResampleToMatch,
     Resize,
     Rotate,
     Rotate90,
     Spacing,
     SpatialResample,
@@ -136,14 +137,17 @@
     "GridSplitDict",
     "GridPatchd",
     "GridPatchD",
     "GridPatchDict",
     "RandGridPatchd",
     "RandGridPatchD",
     "RandGridPatchDict",
+    "RandSimulateLowResolutiond",
+    "RandSimulateLowResolutionD",
+    "RandSimulateLowResolutionDict",
 ]
 
 
 class SpatialResampled(MapTransform, InvertibleTransform, LazyTransform):
     """
     Dictionary-based wrapper of :py:class:`monai.transforms.SpatialResample`.
 
@@ -2514,14 +2518,102 @@
             self.patcher.randomize(d[key])
             break
         for key in self.key_iterator(d):
             d[key] = self.patcher(d[key], randomize=False)
         return d
 
 
+class RandSimulateLowResolutiond(RandomizableTransform, MapTransform):
+    """
+    Dictionary-based wrapper of :py:class:`monai.transforms.RandSimulateLowResolution`.
+    Random simulation of low resolution corresponding to nnU-Net's SimulateLowResolutionTransform
+    (https://github.com/MIC-DKFZ/batchgenerators/blob/7651ece69faf55263dd582a9f5cbd149ed9c3ad0/batchgenerators/transforms/resample_transforms.py#L23)
+    First, the array/tensor is resampled at lower resolution as determined by the zoom_factor which is uniformly sampled
+    from the `zoom_range`. Then, the array/tensor is resampled at the original resolution.
+    """
+
+    backend = RandAffine.backend
+
+    def __init__(
+        self,
+        keys: KeysCollection,
+        prob: float = 0.1,
+        downsample_mode: InterpolateMode | str = InterpolateMode.NEAREST,
+        upsample_mode: InterpolateMode | str = InterpolateMode.TRILINEAR,
+        zoom_range=(0.5, 1.0),
+        align_corners=False,
+        allow_missing_keys: bool = False,
+        device: torch.device | None = None,
+    ) -> None:
+        """
+        Args:
+            keys: keys of the corresponding items to be transformed.
+            prob: probability of performing this augmentation
+            downsample_mode: interpolation mode for downsampling operation
+            upsample_mode: interpolation mode for upsampling operation
+            zoom_range: range from which the random zoom factor for the downsampling and upsampling operation is
+            sampled. It determines the shape of the downsampled tensor.
+            align_corners: This only has an effect when downsample_mode or upsample_mode  is 'linear', 'bilinear',
+                'bicubic' or 'trilinear'. Default: False
+                See also: https://pytorch.org/docs/stable/generated/torch.nn.functional.interpolate.html
+            allow_missing_keys: don't raise exception if key is missing.
+            device: device on which the tensor will be allocated.
+
+        See also:
+            - :py:class:`monai.transforms.compose.MapTransform`
+
+        """
+        MapTransform.__init__(self, keys, allow_missing_keys)
+        RandomizableTransform.__init__(self, prob)
+
+        self.downsample_mode = downsample_mode
+        self.upsample_mode = upsample_mode
+        self.zoom_range = zoom_range
+        self.align_corners = align_corners
+        self.device = device
+
+        self.sim_lowres_tfm = RandSimulateLowResolution(
+            prob=1.0,  # probability is handled by dictionary class
+            downsample_mode=self.downsample_mode,
+            upsample_mode=self.upsample_mode,
+            zoom_range=self.zoom_range,
+            align_corners=self.align_corners,
+            device=self.device,
+        )
+
+    def set_random_state(
+        self, seed: int | None = None, state: np.random.RandomState | None = None
+    ) -> RandSimulateLowResolutiond:
+        super().set_random_state(seed, state)
+        return self
+
+    def __call__(self, data: Mapping[Hashable, NdarrayOrTensor]) -> dict[Hashable, NdarrayOrTensor]:
+        """
+        Args:
+            data: a dictionary containing the tensor-like data to be transformed. The ``keys`` specified
+                in this dictionary must be tensor like arrays that are channel first and have at most
+                three spatial dimensions
+        """
+        d = dict(data)
+        first_key: Hashable = self.first_key(d)
+        if first_key == ():
+            out: dict[Hashable, NdarrayOrTensor] = convert_to_tensor(d, track_meta=get_track_meta())
+            return out
+
+        self.randomize(None)
+
+        for key in self.key_iterator(d):
+            # do the transform
+            if self._do_transform:
+                d[key] = self.sim_lowres_tfm(d[key])  # type: ignore
+            else:
+                d[key] = convert_to_tensor(d[key], track_meta=get_track_meta(), dtype=torch.float32)
+        return d
+
+
 SpatialResampleD = SpatialResampleDict = SpatialResampled
 ResampleToMatchD = ResampleToMatchDict = ResampleToMatchd
 SpacingD = SpacingDict = Spacingd
 OrientationD = OrientationDict = Orientationd
 Rotate90D = Rotate90Dict = Rotate90d
 RandRotate90D = RandRotate90Dict = RandRotate90d
 ResizeD = ResizeDict = Resized
@@ -2537,7 +2629,8 @@
 RotateD = RotateDict = Rotated
 RandRotateD = RandRotateDict = RandRotated
 ZoomD = ZoomDict = Zoomd
 RandZoomD = RandZoomDict = RandZoomd
 GridSplitD = GridSplitDict = GridSplitd
 GridPatchD = GridPatchDict = GridPatchd
 RandGridPatchD = RandGridPatchDict = RandGridPatchd
+RandSimulateLowResolutionD = RandSimulateLowResolutionDict = RandSimulateLowResolutiond
```

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/spatial/functional.py` & `monai-weekly-1.3.dev2332/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/traits.py` & `monai-weekly-1.3.dev2332/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/transform.py` & `monai-weekly-1.3.dev2332/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utility/__init__.py` & `monai-weekly-1.3.dev2332/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utility/array.py` & `monai-weekly-1.3.dev2332/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utility/dictionary.py` & `monai-weekly-1.3.dev2332/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utils.py` & `monai-weekly-1.3.dev2332/monai/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.3.dev2332/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2332/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/__init__.py` & `monai-weekly-1.3.dev2332/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/aliases.py` & `monai-weekly-1.3.dev2332/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/decorators.py` & `monai-weekly-1.3.dev2332/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/deprecate_utils.py` & `monai-weekly-1.3.dev2332/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/dist.py` & `monai-weekly-1.3.dev2332/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/enums.py` & `monai-weekly-1.3.dev2332/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/jupyter_utils.py` & `monai-weekly-1.3.dev2332/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/misc.py` & `monai-weekly-1.3.dev2332/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/module.py` & `monai-weekly-1.3.dev2332/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/nvtx.py` & `monai-weekly-1.3.dev2332/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/profiling.py` & `monai-weekly-1.3.dev2332/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/state_cacher.py` & `monai-weekly-1.3.dev2332/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/utils/type_conversion.py` & `monai-weekly-1.3.dev2332/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/__init__.py` & `monai-weekly-1.3.dev2332/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/class_activation_maps.py` & `monai-weekly-1.3.dev2332/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/gradient_based.py` & `monai-weekly-1.3.dev2332/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/img2tensorboard.py` & `monai-weekly-1.3.dev2332/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.3.dev2332/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/utils.py` & `monai-weekly-1.3.dev2332/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai/visualize/visualizer.py` & `monai-weekly-1.3.dev2332/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.3.dev2332/monai_weekly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.3.dev2331
+Version: 1.3.dev2332
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -58,14 +58,15 @@
 Provides-Extra: pynrrd
 Provides-Extra: pydicom
 Provides-Extra: h5py
 Provides-Extra: nni
 Provides-Extra: optuna
 Provides-Extra: onnx
 Provides-Extra: zarr
+Provides-Extra: lpips
 License-File: LICENSE
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/Project-MONAI/MONAI/dev/docs/images/MONAI-logo-color.png" width="50%" alt='project-monai'>
 </p>
 
 **M**edical **O**pen **N**etwork for **AI**
```

### Comparing `monai-weekly-1.3.dev2331/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.3.dev2332/monai_weekly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -192,24 +192,27 @@
 monai/handlers/validation_handler.py
 monai/inferers/__init__.py
 monai/inferers/inferer.py
 monai/inferers/merger.py
 monai/inferers/splitter.py
 monai/inferers/utils.py
 monai/losses/__init__.py
+monai/losses/adversarial_loss.py
 monai/losses/cldice.py
 monai/losses/contrastive.py
 monai/losses/deform.py
 monai/losses/dice.py
 monai/losses/ds_loss.py
 monai/losses/focal_loss.py
 monai/losses/giou_loss.py
 monai/losses/image_dissimilarity.py
 monai/losses/multi_scale.py
+monai/losses/perceptual.py
 monai/losses/spatial_mask.py
+monai/losses/spectral_loss.py
 monai/losses/ssim_loss.py
 monai/losses/tversky.py
 monai/losses/unified_focal_loss.py
 monai/metrics/__init__.py
 monai/metrics/active_learning_metrics.py
 monai/metrics/confusion_matrix.py
 monai/metrics/cumulative_average.py
@@ -385,14 +388,15 @@
 tests/test_add_coordinate_channels.py
 tests/test_add_coordinate_channelsd.py
 tests/test_add_extreme_points_channel.py
 tests/test_add_extreme_points_channeld.py
 tests/test_adjust_contrast.py
 tests/test_adjust_contrastd.py
 tests/test_adn.py
+tests/test_adversarial_loss.py
 tests/test_affine.py
 tests/test_affine_grid.py
 tests/test_affine_transform.py
 tests/test_affined.py
 tests/test_ahnet.py
 tests/test_alias.py
 tests/test_anchor_box.py
@@ -801,14 +805,15 @@
 tests/test_patch_dataset.py
 tests/test_patch_inferer.py
 tests/test_patch_wsi_dataset.py
 tests/test_patchembedding.py
 tests/test_pathology_he_stain.py
 tests/test_pathology_he_stain_dict.py
 tests/test_pathology_prob_nms.py
+tests/test_perceptual_loss.py
 tests/test_persistentdataset.py
 tests/test_persistentdataset_dist.py
 tests/test_phl_cpu.py
 tests/test_phl_cuda.py
 tests/test_pil_reader.py
 tests/test_plot_2d_or_3d_image.py
 tests/test_png_rw.py
@@ -880,14 +885,16 @@
 tests/test_rand_scale_cropd.py
 tests/test_rand_scale_intensity.py
 tests/test_rand_scale_intensity_fixed_mean.py
 tests/test_rand_scale_intensity_fixed_meand.py
 tests/test_rand_scale_intensityd.py
 tests/test_rand_shift_intensity.py
 tests/test_rand_shift_intensityd.py
+tests/test_rand_simulate_low_resolution.py
+tests/test_rand_simulate_low_resolutiond.py
 tests/test_rand_spatial_crop.py
 tests/test_rand_spatial_crop_samples.py
 tests/test_rand_spatial_crop_samplesd.py
 tests/test_rand_spatial_cropd.py
 tests/test_rand_std_shift_intensity.py
 tests/test_rand_std_shift_intensityd.py
 tests/test_rand_weighted_crop.py
@@ -996,14 +1003,15 @@
 tests/test_spatial_combine_transforms.py
 tests/test_spatial_crop.py
 tests/test_spatial_cropd.py
 tests/test_spatial_pad.py
 tests/test_spatial_padd.py
 tests/test_spatial_resample.py
 tests/test_spatial_resampled.py
+tests/test_spectral_loss.py
 tests/test_split_channel.py
 tests/test_split_channeld.py
 tests/test_splitdim.py
 tests/test_splitdimd.py
 tests/test_squeezedim.py
 tests/test_squeezedimd.py
 tests/test_ssim_loss.py
```

### Comparing `monai-weekly-1.3.dev2331/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.3.dev2332/monai_weekly.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 pynrrd
 pydicom
 h5py
 nni
 optuna
 onnx>=1.13.0
 zarr
+lpips==0.1.4
 
 [all:python_version <= "3.10"]
 onnxruntime
 
 [cucim]
 cucim>=23.2.0
 
@@ -66,14 +67,17 @@
 
 [jsonschema]
 jsonschema
 
 [lmdb]
 lmdb
 
+[lpips]
+lpips==0.1.4
+
 [matplotlib]
 matplotlib
 
 [mlflow]
 mlflow
 
 [nibabel]
```

### Comparing `monai-weekly-1.3.dev2331/pyproject.toml` & `monai-weekly-1.3.dev2332/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/setup.cfg` & `monai-weekly-1.3.dev2332/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 	pydicom
 	h5py
 	nni
 	optuna
 	onnx>=1.13.0
 	onnxruntime; python_version <= '3.10'
 	zarr
+	lpips==0.1.4
 nibabel = 
 	nibabel
 ninja = 
 	ninja
 skimage = 
 	scikit-image>=0.14.2
 scipy = 
@@ -141,14 +142,16 @@
 optuna = 
 	optuna
 onnx = 
 	onnx>=1.13.0
 	onnxruntime; python_version <= '3.10'
 zarr = 
 	zarr
+lpips = 
+	lpips==0.1.4
 
 [flake8]
 select = B,C,E,F,N,P,T4,W,B9
 max_line_length = 120
 ignore = 
 	E203
 	E501
```

### Comparing `monai-weekly-1.3.dev2331/setup.py` & `monai-weekly-1.3.dev2332/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_acn_block.py` & `monai-weekly-1.3.dev2332/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_activations.py` & `monai-weekly-1.3.dev2332/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_activationsd.py` & `monai-weekly-1.3.dev2332/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_adaptors.py` & `monai-weekly-1.3.dev2332/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_add_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_add_coordinate_channels.py` & `monai-weekly-1.3.dev2332/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.3.dev2332/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.3.dev2332/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_adjust_contrast.py` & `monai-weekly-1.3.dev2332/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_adjust_contrastd.py` & `monai-weekly-1.3.dev2332/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_adn.py` & `monai-weekly-1.3.dev2332/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_affine.py` & `monai-weekly-1.3.dev2332/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_affine_grid.py` & `monai-weekly-1.3.dev2332/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_affine_transform.py` & `monai-weekly-1.3.dev2332/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_affined.py` & `monai-weekly-1.3.dev2332/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ahnet.py` & `monai-weekly-1.3.dev2332/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_alias.py` & `monai-weekly-1.3.dev2332/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_anchor_box.py` & `monai-weekly-1.3.dev2332/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_apply.py` & `monai-weekly-1.3.dev2332/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_apply_filter.py` & `monai-weekly-1.3.dev2332/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_arraydataset.py` & `monai-weekly-1.3.dev2332/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_channel_first.py` & `monai-weekly-1.3.dev2332/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_channel_firstd.py` & `monai-weekly-1.3.dev2332/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_channel_last.py` & `monai-weekly-1.3.dev2332/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_channel_lastd.py` & `monai-weekly-1.3.dev2332/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_discrete.py` & `monai-weekly-1.3.dev2332/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_as_discreted.py` & `monai-weekly-1.3.dev2332/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_atss_box_matcher.py` & `monai-weekly-1.3.dev2332/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_attentionunet.py` & `monai-weekly-1.3.dev2332/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_auto3dseg.py` & `monai-weekly-1.3.dev2332/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_auto3dseg_bundlegen.py` & `monai-weekly-1.3.dev2332/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.3.dev2332/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_auto3dseg_hpo.py` & `monai-weekly-1.3.dev2332/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_autoencoder.py` & `monai-weekly-1.3.dev2332/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_avg_merger.py` & `monai-weekly-1.3.dev2332/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_basic_unet.py` & `monai-weekly-1.3.dev2332/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_basic_unetplusplus.py` & `monai-weekly-1.3.dev2332/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bending_energy.py` & `monai-weekly-1.3.dev2332/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.3.dev2332/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.3.dev2332/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bilateral_precise.py` & `monai-weekly-1.3.dev2332/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_blend_images.py` & `monai-weekly-1.3.dev2332/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_border_pad.py` & `monai-weekly-1.3.dev2332/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_border_padd.py` & `monai-weekly-1.3.dev2332/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bounding_rect.py` & `monai-weekly-1.3.dev2332/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bounding_rectd.py` & `monai-weekly-1.3.dev2332/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_box_coder.py` & `monai-weekly-1.3.dev2332/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_box_transform.py` & `monai-weekly-1.3.dev2332/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_box_utils.py` & `monai-weekly-1.3.dev2332/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_download.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_get_data.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_init_bundle.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_onnx_export.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_trt_export.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_utils.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_verify_net.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_bundle_workflow.py` & `monai-weekly-1.3.dev2332/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cachedataset.py` & `monai-weekly-1.3.dev2332/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cachedataset_parallel.py` & `monai-weekly-1.3.dev2332/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.3.dev2332/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cachentransdataset.py` & `monai-weekly-1.3.dev2332/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_call_dist.py` & `monai-weekly-1.3.dev2332/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cast_to_type.py` & `monai-weekly-1.3.dev2332/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cast_to_typed.py` & `monai-weekly-1.3.dev2332/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_center_scale_crop.py` & `monai-weekly-1.3.dev2332/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_center_scale_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_center_spatial_crop.py` & `monai-weekly-1.3.dev2332/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_center_spatial_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_channel_pad.py` & `monai-weekly-1.3.dev2332/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_check_hash.py` & `monai-weekly-1.3.dev2332/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_check_missing_files.py` & `monai-weekly-1.3.dev2332/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_classes_to_indices.py` & `monai-weekly-1.3.dev2332/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_classes_to_indicesd.py` & `monai-weekly-1.3.dev2332/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cldice_loss.py` & `monai-weekly-1.3.dev2332/tests/test_cldice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_complex_utils.py` & `monai-weekly-1.3.dev2332/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_component_locator.py` & `monai-weekly-1.3.dev2332/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compose.py` & `monai-weekly-1.3.dev2332/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.3.dev2332/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.3.dev2332/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_f_beta.py` & `monai-weekly-1.3.dev2332/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_froc.py` & `monai-weekly-1.3.dev2332/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_generalized_dice.py` & `monai-weekly-1.3.dev2332/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.3.dev2332/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.3.dev2332/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_meandice.py` & `monai-weekly-1.3.dev2332/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_meaniou.py` & `monai-weekly-1.3.dev2332/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.3.dev2332/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_regression_metrics.py` & `monai-weekly-1.3.dev2332/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_roc_auc.py` & `monai-weekly-1.3.dev2332/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_compute_variance.py` & `monai-weekly-1.3.dev2332/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_concat_itemsd.py` & `monai-weekly-1.3.dev2332/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_config_item.py` & `monai-weekly-1.3.dev2332/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_config_parser.py` & `monai-weekly-1.3.dev2332/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_contrastive_loss.py` & `monai-weekly-1.3.dev2332/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_data_type.py` & `monai-weekly-1.3.dev2332/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.3.dev2332/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_to_onnx.py` & `monai-weekly-1.3.dev2332/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_to_torchscript.py` & `monai-weekly-1.3.dev2332/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convert_to_trt.py` & `monai-weekly-1.3.dev2332/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_convolutions.py` & `monai-weekly-1.3.dev2332/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_copy_itemsd.py` & `monai-weekly-1.3.dev2332/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_copy_model_state.py` & `monai-weekly-1.3.dev2332/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_correct_crop_centers.py` & `monai-weekly-1.3.dev2332/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.3.dev2332/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_create_grid_and_affine.py` & `monai-weekly-1.3.dev2332/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_crf_cpu.py` & `monai-weekly-1.3.dev2332/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_crf_cuda.py` & `monai-weekly-1.3.dev2332/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_crop_foreground.py` & `monai-weekly-1.3.dev2332/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_crop_foregroundd.py` & `monai-weekly-1.3.dev2332/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cross_validation.py` & `monai-weekly-1.3.dev2332/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_csv_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_csv_saver.py` & `monai-weekly-1.3.dev2332/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cucim_dict_transform.py` & `monai-weekly-1.3.dev2332/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cucim_transform.py` & `monai-weekly-1.3.dev2332/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cumulative.py` & `monai-weekly-1.3.dev2332/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cumulative_average.py` & `monai-weekly-1.3.dev2332/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cumulative_average_dist.py` & `monai-weekly-1.3.dev2332/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_cv2_dist.py` & `monai-weekly-1.3.dev2332/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_daf3d.py` & `monai-weekly-1.3.dev2332/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_data_stats.py` & `monai-weekly-1.3.dev2332/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_data_statsd.py` & `monai-weekly-1.3.dev2332/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dataloader.py` & `monai-weekly-1.3.dev2332/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dataset_func.py` & `monai-weekly-1.3.dev2332/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dataset_summary.py` & `monai-weekly-1.3.dev2332/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_decathlondataset.py` & `monai-weekly-1.3.dev2332/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_decollate.py` & `monai-weekly-1.3.dev2332/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deepedit_interaction.py` & `monai-weekly-1.3.dev2332/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deepedit_transforms.py` & `monai-weekly-1.3.dev2332/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deepgrow_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deepgrow_interaction.py` & `monai-weekly-1.3.dev2332/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deepgrow_transforms.py` & `monai-weekly-1.3.dev2332/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_delete_itemsd.py` & `monai-weekly-1.3.dev2332/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_denseblock.py` & `monai-weekly-1.3.dev2332/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_densenet.py` & `monai-weekly-1.3.dev2332/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_deprecated.py` & `monai-weekly-1.3.dev2332/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_detect_envelope.py` & `monai-weekly-1.3.dev2332/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_detection_coco_metrics.py` & `monai-weekly-1.3.dev2332/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_detector_boxselector.py` & `monai-weekly-1.3.dev2332/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_detector_utils.py` & `monai-weekly-1.3.dev2332/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dev_collate.py` & `monai-weekly-1.3.dev2332/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dice_ce_loss.py` & `monai-weekly-1.3.dev2332/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dice_focal_loss.py` & `monai-weekly-1.3.dev2332/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dice_loss.py` & `monai-weekly-1.3.dev2332/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dints_cell.py` & `monai-weekly-1.3.dev2332/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dints_mixop.py` & `monai-weekly-1.3.dev2332/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dints_network.py` & `monai-weekly-1.3.dev2332/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_discriminator.py` & `monai-weekly-1.3.dev2332/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_divisible_pad.py` & `monai-weekly-1.3.dev2332/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_divisible_padd.py` & `monai-weekly-1.3.dev2332/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_download_and_extract.py` & `monai-weekly-1.3.dev2332/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_download_url_yandex.py` & `monai-weekly-1.3.dev2332/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_downsample_block.py` & `monai-weekly-1.3.dev2332/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_drop_path.py` & `monai-weekly-1.3.dev2332/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ds_loss.py` & `monai-weekly-1.3.dev2332/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dvf2ddf.py` & `monai-weekly-1.3.dev2332/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dynunet.py` & `monai-weekly-1.3.dev2332/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_dynunet_block.py` & `monai-weekly-1.3.dev2332/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_efficientnet.py` & `monai-weekly-1.3.dev2332/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensemble_evaluator.py` & `monai-weekly-1.3.dev2332/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensure_channel_first.py` & `monai-weekly-1.3.dev2332/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.3.dev2332/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensure_tuple.py` & `monai-weekly-1.3.dev2332/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensure_type.py` & `monai-weekly-1.3.dev2332/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ensure_typed.py` & `monai-weekly-1.3.dev2332/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_enum_bound_interp.py` & `monai-weekly-1.3.dev2332/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_eval_mode.py` & `monai-weekly-1.3.dev2332/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.3.dev2332/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_factorized_increase.py` & `monai-weekly-1.3.dev2332/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_factorized_reduce.py` & `monai-weekly-1.3.dev2332/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fastmri_reader.py` & `monai-weekly-1.3.dev2332/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fft_utils.py` & `monai-weekly-1.3.dev2332/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.3.dev2332/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.3.dev2332/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_file_basename.py` & `monai-weekly-1.3.dev2332/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fill_holes.py` & `monai-weekly-1.3.dev2332/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fill_holesd.py` & `monai-weekly-1.3.dev2332/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fl_exchange_object.py` & `monai-weekly-1.3.dev2332/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo.py` & `monai-weekly-1.3.dev2332/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.3.dev2332/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.3.dev2332/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.3.dev2332/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_flexible_unet.py` & `monai-weekly-1.3.dev2332/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_flip.py` & `monai-weekly-1.3.dev2332/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_flipd.py` & `monai-weekly-1.3.dev2332/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_focal_loss.py` & `monai-weekly-1.3.dev2332/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_folder_layout.py` & `monai-weekly-1.3.dev2332/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_foreground_mask.py` & `monai-weekly-1.3.dev2332/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_foreground_maskd.py` & `monai-weekly-1.3.dev2332/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fourier.py` & `monai-weekly-1.3.dev2332/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fpn_block.py` & `monai-weekly-1.3.dev2332/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_from_engine_hovernet.py` & `monai-weekly-1.3.dev2332/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_fullyconnectednet.py` & `monai-weekly-1.3.dev2332/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian_filter.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian_sharpen.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian_sharpend.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian_smooth.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gaussian_smoothd.py` & `monai-weekly-1.3.dev2332/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gdsdataset.py` & `monai-weekly-1.3.dev2332/tests/test_gdsdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.3.dev2332/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generalized_dice_loss.py` & `monai-weekly-1.3.dev2332/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.3.dev2332/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_distance_map.py` & `monai-weekly-1.3.dev2332/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_distance_mapd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_border.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_borderd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_centroid.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_contour.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_contourd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_type.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_instance_typed.py` & `monai-weekly-1.3.dev2332/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.3.dev2332/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_param_groups.py` & `monai-weekly-1.3.dev2332/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.3.dev2332/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.3.dev2332/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_succinct_contour.py` & `monai-weekly-1.3.dev2332/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_watershed_markers.py` & `monai-weekly-1.3.dev2332/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_watershed_mask.py` & `monai-weekly-1.3.dev2332/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.3.dev2332/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_generator.py` & `monai-weekly-1.3.dev2332/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.3.dev2332/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_get_extreme_points.py` & `monai-weekly-1.3.dev2332/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_get_layers.py` & `monai-weekly-1.3.dev2332/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_get_package_version.py` & `monai-weekly-1.3.dev2332/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_get_unique_labels.py` & `monai-weekly-1.3.dev2332/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gibbs_noise.py` & `monai-weekly-1.3.dev2332/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gibbs_noised.py` & `monai-weekly-1.3.dev2332/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_giou_loss.py` & `monai-weekly-1.3.dev2332/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.3.dev2332/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_globalnet.py` & `monai-weekly-1.3.dev2332/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_gmm.py` & `monai-weekly-1.3.dev2332/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_distortion.py` & `monai-weekly-1.3.dev2332/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_distortiond.py` & `monai-weekly-1.3.dev2332/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_patch.py` & `monai-weekly-1.3.dev2332/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_patchd.py` & `monai-weekly-1.3.dev2332/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_pull.py` & `monai-weekly-1.3.dev2332/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_split.py` & `monai-weekly-1.3.dev2332/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_grid_splitd.py` & `monai-weekly-1.3.dev2332/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.3.dev2332/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.3.dev2332/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_classification_saver.py` & `monai-weekly-1.3.dev2332/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.3.dev2332/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_clearml_image.py` & `monai-weekly-1.3.dev2332/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_clearml_stats.py` & `monai-weekly-1.3.dev2332/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.3.dev2332/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.3.dev2332/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_decollate_batch.py` & `monai-weekly-1.3.dev2332/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_early_stop.py` & `monai-weekly-1.3.dev2332/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_garbage_collector.py` & `monai-weekly-1.3.dev2332/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.3.dev2332/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_ignite_metric.py` & `monai-weekly-1.3.dev2332/tests/test_handler_ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_logfile.py` & `monai-weekly-1.3.dev2332/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.3.dev2332/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_mean_dice.py` & `monai-weekly-1.3.dev2332/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_mean_iou.py` & `monai-weekly-1.3.dev2332/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_metric_logger.py` & `monai-weekly-1.3.dev2332/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.3.dev2332/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver.py` & `monai-weekly-1.3.dev2332/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.3.dev2332/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_mlflow.py` & `monai-weekly-1.3.dev2332/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_nvtx.py` & `monai-weekly-1.3.dev2332/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.3.dev2332/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.3.dev2332/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_post_processing.py` & `monai-weekly-1.3.dev2332/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.3.dev2332/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics.py` & `monai-weekly-1.3.dev2332/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.3.dev2332/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_rocauc.py` & `monai-weekly-1.3.dev2332/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.3.dev2332/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_smartcache.py` & `monai-weekly-1.3.dev2332/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_stats.py` & `monai-weekly-1.3.dev2332/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_surface_distance.py` & `monai-weekly-1.3.dev2332/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_tb_image.py` & `monai-weekly-1.3.dev2332/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_tb_stats.py` & `monai-weekly-1.3.dev2332/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_handler_validation.py` & `monai-weekly-1.3.dev2332/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hardnegsampler.py` & `monai-weekly-1.3.dev2332/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hashing.py` & `monai-weekly-1.3.dev2332/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hausdorff_distance.py` & `monai-weekly-1.3.dev2332/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_header_correct.py` & `monai-weekly-1.3.dev2332/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_highresnet.py` & `monai-weekly-1.3.dev2332/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hilbert_transform.py` & `monai-weekly-1.3.dev2332/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_histogram_normalize.py` & `monai-weekly-1.3.dev2332/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_histogram_normalized.py` & `monai-weekly-1.3.dev2332/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet_loss.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.3.dev2332/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_identity.py` & `monai-weekly-1.3.dev2332/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_identityd.py` & `monai-weekly-1.3.dev2332/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_image_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_image_filter.py` & `monai-weekly-1.3.dev2332/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_image_rw.py` & `monai-weekly-1.3.dev2332/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_img2tensorboard.py` & `monai-weekly-1.3.dev2332/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_init_reader.py` & `monai-weekly-1.3.dev2332/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_autorunner.py` & `monai-weekly-1.3.dev2332/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_bundle_run.py` & `monai-weekly-1.3.dev2332/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_classification_2d.py` & `monai-weekly-1.3.dev2332/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_determinism.py` & `monai-weekly-1.3.dev2332/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_fast_train.py` & `monai-weekly-1.3.dev2332/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_gpu_customization.py` & `monai-weekly-1.3.dev2332/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_lazy_samples.py` & `monai-weekly-1.3.dev2332/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.3.dev2332/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.3.dev2332/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_sliding_window.py` & `monai-weekly-1.3.dev2332/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_stn.py` & `monai-weekly-1.3.dev2332/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_unet_2d.py` & `monai-weekly-1.3.dev2332/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_workers.py` & `monai-weekly-1.3.dev2332/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_workflows.py` & `monai-weekly-1.3.dev2332/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_integration_workflows_gan.py` & `monai-weekly-1.3.dev2332/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_intensity_stats.py` & `monai-weekly-1.3.dev2332/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_intensity_statsd.py` & `monai-weekly-1.3.dev2332/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_inverse.py` & `monai-weekly-1.3.dev2332/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_inverse_array.py` & `monai-weekly-1.3.dev2332/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_inverse_collation.py` & `monai-weekly-1.3.dev2332/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_invert.py` & `monai-weekly-1.3.dev2332/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_invertd.py` & `monai-weekly-1.3.dev2332/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_is_supported_format.py` & `monai-weekly-1.3.dev2332/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_iterable_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_itk_torch_bridge.py` & `monai-weekly-1.3.dev2332/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_itk_writer.py` & `monai-weekly-1.3.dev2332/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_k_space_spike_noise.py` & `monai-weekly-1.3.dev2332/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_k_space_spike_noised.py` & `monai-weekly-1.3.dev2332/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.3.dev2332/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.3.dev2332/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_kspace_mask.py` & `monai-weekly-1.3.dev2332/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_filter.py` & `monai-weekly-1.3.dev2332/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_filterd.py` & `monai-weekly-1.3.dev2332/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_quality_score.py` & `monai-weekly-1.3.dev2332/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_to_contour.py` & `monai-weekly-1.3.dev2332/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_to_contourd.py` & `monai-weekly-1.3.dev2332/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_to_mask.py` & `monai-weekly-1.3.dev2332/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_label_to_maskd.py` & `monai-weekly-1.3.dev2332/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lambda.py` & `monai-weekly-1.3.dev2332/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lambdad.py` & `monai-weekly-1.3.dev2332/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lesion_froc.py` & `monai-weekly-1.3.dev2332/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_list_data_collate.py` & `monai-weekly-1.3.dev2332/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_list_to_dict.py` & `monai-weekly-1.3.dev2332/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lltm.py` & `monai-weekly-1.3.dev2332/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lmdbdataset.py` & `monai-weekly-1.3.dev2332/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.3.dev2332/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.3.dev2332/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_load_image.py` & `monai-weekly-1.3.dev2332/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_load_imaged.py` & `monai-weekly-1.3.dev2332/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_load_spacing_orientation.py` & `monai-weekly-1.3.dev2332/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_loader_semaphore.py` & `monai-weekly-1.3.dev2332/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.3.dev2332/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_localnet.py` & `monai-weekly-1.3.dev2332/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_localnet_block.py` & `monai-weekly-1.3.dev2332/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_look_up_option.py` & `monai-weekly-1.3.dev2332/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_loss_metric.py` & `monai-weekly-1.3.dev2332/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lr_finder.py` & `monai-weekly-1.3.dev2332/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_lr_scheduler.py` & `monai-weekly-1.3.dev2332/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_make_nifti.py` & `monai-weekly-1.3.dev2332/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_map_binary_to_indices.py` & `monai-weekly-1.3.dev2332/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_map_classes_to_indices.py` & `monai-weekly-1.3.dev2332/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_map_label_value.py` & `monai-weekly-1.3.dev2332/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_map_label_valued.py` & `monai-weekly-1.3.dev2332/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_map_transform.py` & `monai-weekly-1.3.dev2332/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mask_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mask_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_masked_dice_loss.py` & `monai-weekly-1.3.dev2332/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_masked_loss.py` & `monai-weekly-1.3.dev2332/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_matshow3d.py` & `monai-weekly-1.3.dev2332/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mean_ensemble.py` & `monai-weekly-1.3.dev2332/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mean_ensembled.py` & `monai-weekly-1.3.dev2332/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_median_filter.py` & `monai-weekly-1.3.dev2332/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_median_smooth.py` & `monai-weekly-1.3.dev2332/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_median_smoothd.py` & `monai-weekly-1.3.dev2332/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mednistdataset.py` & `monai-weekly-1.3.dev2332/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_meta_affine.py` & `monai-weekly-1.3.dev2332/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_meta_tensor.py` & `monai-weekly-1.3.dev2332/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_metatensor_integration.py` & `monai-weekly-1.3.dev2332/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_metrics_reloaded.py` & `monai-weekly-1.3.dev2332/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_milmodel.py` & `monai-weekly-1.3.dev2332/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mlp.py` & `monai-weekly-1.3.dev2332/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mmar_download.py` & `monai-weekly-1.3.dev2332/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_module_list.py` & `monai-weekly-1.3.dev2332/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_monai_env_vars.py` & `monai-weekly-1.3.dev2332/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_monai_utils_misc.py` & `monai-weekly-1.3.dev2332/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_mri_utils.py` & `monai-weekly-1.3.dev2332/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_multi_scale.py` & `monai-weekly-1.3.dev2332/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_net_adapter.py` & `monai-weekly-1.3.dev2332/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_network_consistency.py` & `monai-weekly-1.3.dev2332/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nifti_endianness.py` & `monai-weekly-1.3.dev2332/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nifti_header_revise.py` & `monai-weekly-1.3.dev2332/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nifti_rw.py` & `monai-weekly-1.3.dev2332/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_normalize_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_normalize_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_npzdictitemdataset.py` & `monai-weekly-1.3.dev2332/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nrrd_reader.py` & `monai-weekly-1.3.dev2332/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nuclick_transforms.py` & `monai-weekly-1.3.dev2332/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_numpy_reader.py` & `monai-weekly-1.3.dev2332/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nvtx_decorator.py` & `monai-weekly-1.3.dev2332/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_nvtx_transform.py` & `monai-weekly-1.3.dev2332/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.3.dev2332/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_one_of.py` & `monai-weekly-1.3.dev2332/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_optim_novograd.py` & `monai-weekly-1.3.dev2332/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_optional_import.py` & `monai-weekly-1.3.dev2332/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ori_ras_lps.py` & `monai-weekly-1.3.dev2332/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_orientation.py` & `monai-weekly-1.3.dev2332/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_orientationd.py` & `monai-weekly-1.3.dev2332/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_p3d_block.py` & `monai-weekly-1.3.dev2332/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pad_collation.py` & `monai-weekly-1.3.dev2332/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pad_mode.py` & `monai-weekly-1.3.dev2332/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_parallel_execution.py` & `monai-weekly-1.3.dev2332/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_parallel_execution_dist.py` & `monai-weekly-1.3.dev2332/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_partition_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_partition_dataset_classes.py` & `monai-weekly-1.3.dev2332/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_patch_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_patch_inferer.py` & `monai-weekly-1.3.dev2332/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_patchembedding.py` & `monai-weekly-1.3.dev2332/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pathology_he_stain.py` & `monai-weekly-1.3.dev2332/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.3.dev2332/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pathology_prob_nms.py` & `monai-weekly-1.3.dev2332/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_persistentdataset.py` & `monai-weekly-1.3.dev2332/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_persistentdataset_dist.py` & `monai-weekly-1.3.dev2332/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_phl_cpu.py` & `monai-weekly-1.3.dev2332/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_phl_cuda.py` & `monai-weekly-1.3.dev2332/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pil_reader.py` & `monai-weekly-1.3.dev2332/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.3.dev2332/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_png_rw.py` & `monai-weekly-1.3.dev2332/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_polyval.py` & `monai-weekly-1.3.dev2332/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_prepare_batch_default.py` & `monai-weekly-1.3.dev2332/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.3.dev2332/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.3.dev2332/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.3.dev2332/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_preset_filters.py` & `monai-weekly-1.3.dev2332/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_print_info.py` & `monai-weekly-1.3.dev2332/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_print_transform_backends.py` & `monai-weekly-1.3.dev2332/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_probnms.py` & `monai-weekly-1.3.dev2332/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_probnmsd.py` & `monai-weekly-1.3.dev2332/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_profiling.py` & `monai-weekly-1.3.dev2332/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_pytorch_version_after.py` & `monai-weekly-1.3.dev2332/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_query_memory.py` & `monai-weekly-1.3.dev2332/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_quicknat.py` & `monai-weekly-1.3.dev2332/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.3.dev2332/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_affine.py` & `monai-weekly-1.3.dev2332/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_affine_grid.py` & `monai-weekly-1.3.dev2332/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_affined.py` & `monai-weekly-1.3.dev2332/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_axis_flip.py` & `monai-weekly-1.3.dev2332/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_axis_flipd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_bias_field.py` & `monai-weekly-1.3.dev2332/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.3.dev2332/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.3.dev2332/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.3.dev2332/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.3.dev2332/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.3.dev2332/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.3.dev2332/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.3.dev2332/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_cucim_transform.py` & `monai-weekly-1.3.dev2332/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_deform_grid.py` & `monai-weekly-1.3.dev2332/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_elastic_2d.py` & `monai-weekly-1.3.dev2332/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_elastic_3d.py` & `monai-weekly-1.3.dev2332/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.3.dev2332/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.3.dev2332/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_flip.py` & `monai-weekly-1.3.dev2332/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_flipd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.3.dev2332/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_grid_distortion.py` & `monai-weekly-1.3.dev2332/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.3.dev2332/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_grid_patch.py` & `monai-weekly-1.3.dev2332/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_grid_patchd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_histogram_shift.py` & `monai-weekly-1.3.dev2332/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.3.dev2332/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.3.dev2332/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_lambda.py` & `monai-weekly-1.3.dev2332/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_lambdad.py` & `monai-weekly-1.3.dev2332/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rician_noise.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rician_noised.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rotate.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rotate90.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rotate90d.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_rotated.py` & `monai-weekly-1.3.dev2332/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_crop.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensity_fixed_meand.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_shift_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop.py` & `monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_weighted_crop.py` & `monai-weekly-1.3.dev2332/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_zoom.py` & `monai-weekly-1.3.dev2332/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rand_zoomd.py` & `monai-weekly-1.3.dev2332/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_randidentity.py` & `monai-weekly-1.3.dev2332/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_random_order.py` & `monai-weekly-1.3.dev2332/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_randomizable.py` & `monai-weekly-1.3.dev2332/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_randomizable_transform_type.py` & `monai-weekly-1.3.dev2332/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_randtorchvisiond.py` & `monai-weekly-1.3.dev2332/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rankfilter_dist.py` & `monai-weekly-1.3.dev2332/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_recon_net_utils.py` & `monai-weekly-1.3.dev2332/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_reference_resolver.py` & `monai-weekly-1.3.dev2332/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_reg_loss_integration.py` & `monai-weekly-1.3.dev2332/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_regunet.py` & `monai-weekly-1.3.dev2332/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_regunet_block.py` & `monai-weekly-1.3.dev2332/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_remove_repeated_channel.py` & `monai-weekly-1.3.dev2332/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_remove_small_objects.py` & `monai-weekly-1.3.dev2332/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_repeat_channel.py` & `monai-weekly-1.3.dev2332/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_repeat_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_replace_module.py` & `monai-weekly-1.3.dev2332/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_require_pkg.py` & `monai-weekly-1.3.dev2332/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resample.py` & `monai-weekly-1.3.dev2332/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resample_backends.py` & `monai-weekly-1.3.dev2332/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resample_datalist.py` & `monai-weekly-1.3.dev2332/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resample_to_match.py` & `monai-weekly-1.3.dev2332/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resample_to_matchd.py` & `monai-weekly-1.3.dev2332/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resampler.py` & `monai-weekly-1.3.dev2332/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resize.py` & `monai-weekly-1.3.dev2332/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.3.dev2332/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resized.py` & `monai-weekly-1.3.dev2332/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_resnet.py` & `monai-weekly-1.3.dev2332/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_retinanet.py` & `monai-weekly-1.3.dev2332/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_retinanet_detector.py` & `monai-weekly-1.3.dev2332/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.3.dev2332/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rotate.py` & `monai-weekly-1.3.dev2332/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rotate90.py` & `monai-weekly-1.3.dev2332/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rotate90d.py` & `monai-weekly-1.3.dev2332/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_rotated.py` & `monai-weekly-1.3.dev2332/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_safe_dtype_range.py` & `monai-weekly-1.3.dev2332/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_saliency_inferer.py` & `monai-weekly-1.3.dev2332/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sample_slices.py` & `monai-weekly-1.3.dev2332/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sampler_dist.py` & `monai-weekly-1.3.dev2332/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_save_classificationd.py` & `monai-weekly-1.3.dev2332/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_save_image.py` & `monai-weekly-1.3.dev2332/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_save_imaged.py` & `monai-weekly-1.3.dev2332/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_save_state.py` & `monai-weekly-1.3.dev2332/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.3.dev2332/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.3.dev2332/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.3.dev2332/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity_fixed_mean.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_scale_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_se_block.py` & `monai-weekly-1.3.dev2332/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_se_blocks.py` & `monai-weekly-1.3.dev2332/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_seg_loss_integration.py` & `monai-weekly-1.3.dev2332/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_segresnet.py` & `monai-weekly-1.3.dev2332/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_segresnet_block.py` & `monai-weekly-1.3.dev2332/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_segresnet_ds.py` & `monai-weekly-1.3.dev2332/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.3.dev2332/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_select_itemsd.py` & `monai-weekly-1.3.dev2332/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_selfattention.py` & `monai-weekly-1.3.dev2332/tests/test_selfattention.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         num_heads = 2
         dropout_rate = 0
         input_shape = (2, 256, hidden_size)
 
         # be  not able to access the matrix
         no_matrix_acess_blk = SABlock(hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate)
         no_matrix_acess_blk(torch.randn(input_shape))
-        assert type(no_matrix_acess_blk.att_mat) == torch.Tensor
+        assert isinstance(no_matrix_acess_blk.att_mat, torch.Tensor)
         # no of elements is zero
         assert no_matrix_acess_blk.att_mat.nelement() == 0
 
         # be able to acess the attention matrix
         matrix_acess_blk = SABlock(
             hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate, save_attn=True
         )
```

### Comparing `monai-weekly-1.3.dev2331/tests/test_senet.py` & `monai-weekly-1.3.dev2332/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_separable_filter.py` & `monai-weekly-1.3.dev2332/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_set_determinism.py` & `monai-weekly-1.3.dev2332/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_set_visible_devices.py` & `monai-weekly-1.3.dev2332/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_shift_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_shift_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_shuffle_buffer.py` & `monai-weekly-1.3.dev2332/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.3.dev2332/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_fillempty.py` & `monai-weekly-1.3.dev2332/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_drop.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_scale.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_rand_shift.py` & `monai-weekly-1.3.dev2332/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_signal_remove_frequency.py` & `monai-weekly-1.3.dev2332/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_simple_aspp.py` & `monai-weekly-1.3.dev2332/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_simulatedelay.py` & `monai-weekly-1.3.dev2332/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_simulatedelayd.py` & `monai-weekly-1.3.dev2332/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_skip_connection.py` & `monai-weekly-1.3.dev2332/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_slice_inferer.py` & `monai-weekly-1.3.dev2332/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.3.dev2332/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.3.dev2332/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sliding_window_inference.py` & `monai-weekly-1.3.dev2332/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sliding_window_splitter.py` & `monai-weekly-1.3.dev2332/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_smartcachedataset.py` & `monai-weekly-1.3.dev2332/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_smooth_field.py` & `monai-weekly-1.3.dev2332/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sobel_gradient.py` & `monai-weekly-1.3.dev2332/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_sobel_gradientd.py` & `monai-weekly-1.3.dev2332/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_some_of.py` & `monai-weekly-1.3.dev2332/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spacing.py` & `monai-weekly-1.3.dev2332/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spacingd.py` & `monai-weekly-1.3.dev2332/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_crop.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_cropd.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_pad.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_padd.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_resample.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_spatial_resampled.py` & `monai-weekly-1.3.dev2332/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_split_channel.py` & `monai-weekly-1.3.dev2332/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_split_channeld.py` & `monai-weekly-1.3.dev2332/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_splitdim.py` & `monai-weekly-1.3.dev2332/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_splitdimd.py` & `monai-weekly-1.3.dev2332/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_squeezedim.py` & `monai-weekly-1.3.dev2332/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_squeezedimd.py` & `monai-weekly-1.3.dev2332/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ssim_loss.py` & `monai-weekly-1.3.dev2332/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ssim_metric.py` & `monai-weekly-1.3.dev2332/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_state_cacher.py` & `monai-weekly-1.3.dev2332/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_std_shift_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_std_shift_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_str2bool.py` & `monai-weekly-1.3.dev2332/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_str2list.py` & `monai-weekly-1.3.dev2332/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_subpixel_upsample.py` & `monai-weekly-1.3.dev2332/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_surface_dice.py` & `monai-weekly-1.3.dev2332/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_surface_distance.py` & `monai-weekly-1.3.dev2332/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_swin_unetr.py` & `monai-weekly-1.3.dev2332/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_synthetic.py` & `monai-weekly-1.3.dev2332/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_tciadataset.py` & `monai-weekly-1.3.dev2332/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_testtimeaugmentation.py` & `monai-weekly-1.3.dev2332/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_text_encoding.py` & `monai-weekly-1.3.dev2332/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_thread_buffer.py` & `monai-weekly-1.3.dev2332/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_threadcontainer.py` & `monai-weekly-1.3.dev2332/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_threshold_intensity.py` & `monai-weekly-1.3.dev2332/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_threshold_intensityd.py` & `monai-weekly-1.3.dev2332/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_timedcall_dist.py` & `monai-weekly-1.3.dev2332/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_contiguous.py` & `monai-weekly-1.3.dev2332/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_cupy.py` & `monai-weekly-1.3.dev2332/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_cupyd.py` & `monai-weekly-1.3.dev2332/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_device.py` & `monai-weekly-1.3.dev2332/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_deviced.py` & `monai-weekly-1.3.dev2332/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.3.dev2332/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_numpy.py` & `monai-weekly-1.3.dev2332/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_numpyd.py` & `monai-weekly-1.3.dev2332/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_onehot.py` & `monai-weekly-1.3.dev2332/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_pil.py` & `monai-weekly-1.3.dev2332/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_pild.py` & `monai-weekly-1.3.dev2332/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_tensor.py` & `monai-weekly-1.3.dev2332/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_to_tensord.py` & `monai-weekly-1.3.dev2332/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_torchscript_utils.py` & `monai-weekly-1.3.dev2332/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_torchvision.py` & `monai-weekly-1.3.dev2332/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_torchvision_fc_model.py` & `monai-weekly-1.3.dev2332/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_torchvisiond.py` & `monai-weekly-1.3.dev2332/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_traceable_transform.py` & `monai-weekly-1.3.dev2332/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_train_mode.py` & `monai-weekly-1.3.dev2332/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_trainable_bilateral.py` & `monai-weekly-1.3.dev2332/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.3.dev2332/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_transchex.py` & `monai-weekly-1.3.dev2332/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_transform.py` & `monai-weekly-1.3.dev2332/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_transformerblock.py` & `monai-weekly-1.3.dev2332/tests/test_transformerblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         input_shape = (2, 256, hidden_size)
 
         # returns an empty attention matrix
         no_matrix_acess_blk = TransformerBlock(
             hidden_size=hidden_size, mlp_dim=mlp_dim, num_heads=num_heads, dropout_rate=dropout_rate
         )
         no_matrix_acess_blk(torch.randn(input_shape))
-        assert type(no_matrix_acess_blk.attn.att_mat) == torch.Tensor
+        assert isinstance(no_matrix_acess_blk.attn.att_mat, torch.Tensor)
         # no of elements is zero
         assert no_matrix_acess_blk.attn.att_mat.nelement() == 0
 
         # be able to acess the attention matrix
         matrix_acess_blk = TransformerBlock(
             hidden_size=hidden_size, mlp_dim=mlp_dim, num_heads=num_heads, dropout_rate=dropout_rate, save_attn=True
         )
```

### Comparing `monai-weekly-1.3.dev2331/tests/test_transpose.py` & `monai-weekly-1.3.dev2332/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_transposed.py` & `monai-weekly-1.3.dev2332/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_tversky_loss.py` & `monai-weekly-1.3.dev2332/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_ultrasound_confidence_map_transform.py` & `monai-weekly-1.3.dev2332/tests/test_ultrasound_confidence_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_unet.py` & `monai-weekly-1.3.dev2332/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_unetr.py` & `monai-weekly-1.3.dev2332/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_unetr_block.py` & `monai-weekly-1.3.dev2332/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_unified_focal_loss.py` & `monai-weekly-1.3.dev2332/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_upsample_block.py` & `monai-weekly-1.3.dev2332/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.3.dev2332/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_varautoencoder.py` & `monai-weekly-1.3.dev2332/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_varnet.py` & `monai-weekly-1.3.dev2332/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_version_leq.py` & `monai-weekly-1.3.dev2332/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_video_datasets.py` & `monai-weekly-1.3.dev2332/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vis_cam.py` & `monai-weekly-1.3.dev2332/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vis_gradbased.py` & `monai-weekly-1.3.dev2332/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vis_gradcam.py` & `monai-weekly-1.3.dev2332/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vit.py` & `monai-weekly-1.3.dev2332/tests/test_vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         img_size = (96, 96, 96)
         patch_size = (16, 16, 16)
         in_shape = (1, in_channels, img_size[0], img_size[1], img_size[2])
 
         # no data in the matrix
         no_matrix_acess_blk = ViT(in_channels=in_channels, img_size=img_size, patch_size=patch_size)
         no_matrix_acess_blk(torch.randn(in_shape))
-        assert type(no_matrix_acess_blk.blocks[0].attn.att_mat) == torch.Tensor
+        assert isinstance(no_matrix_acess_blk.blocks[0].attn.att_mat, torch.Tensor)
         # no of elements is zero
         assert no_matrix_acess_blk.blocks[0].attn.att_mat.nelement() == 0
 
         # be able to acess the attention matrix
         matrix_acess_blk = ViT(in_channels=in_channels, img_size=img_size, patch_size=patch_size, save_attn=True)
         matrix_acess_blk(torch.randn(in_shape))
         assert matrix_acess_blk.blocks[0].attn.att_mat.shape == (in_shape[0], 12, 216, 216)
```

### Comparing `monai-weekly-1.3.dev2331/tests/test_vitautoenc.py` & `monai-weekly-1.3.dev2332/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vnet.py` & `monai-weekly-1.3.dev2332/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vote_ensemble.py` & `monai-weekly-1.3.dev2332/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_vote_ensembled.py` & `monai-weekly-1.3.dev2332/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_warp.py` & `monai-weekly-1.3.dev2332/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_watershed.py` & `monai-weekly-1.3.dev2332/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_watershedd.py` & `monai-weekly-1.3.dev2332/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_weight_init.py` & `monai-weekly-1.3.dev2332/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.3.dev2332/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.3.dev2332/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_write_metrics_reports.py` & `monai-weekly-1.3.dev2332/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_wsi_sliding_window_splitter.py` & `monai-weekly-1.3.dev2332/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_wsireader.py` & `monai-weekly-1.3.dev2332/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_zarr_avg_merger.py` & `monai-weekly-1.3.dev2332/tests/test_zarr_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_zipdataset.py` & `monai-weekly-1.3.dev2332/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_zoom.py` & `monai-weekly-1.3.dev2332/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_zoom_affine.py` & `monai-weekly-1.3.dev2332/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/tests/test_zoomd.py` & `monai-weekly-1.3.dev2332/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.3.dev2331/versioneer.py` & `monai-weekly-1.3.dev2332/versioneer.py`

 * *Files identical despite different names*

