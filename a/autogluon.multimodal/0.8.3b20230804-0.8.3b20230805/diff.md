# Comparing `tmp/autogluon.multimodal-0.8.3b20230804.tar.gz` & `tmp/autogluon.multimodal-0.8.3b20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.8.3b20230804.tar", last modified: Fri Aug  4 09:04:19 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.8.3b20230805.tar", last modified: Sat Aug  5 09:04:07 2023, max compression
```

## Comparing `autogluon.multimodal-0.8.3b20230804.tar` & `autogluon.multimodal-0.8.3b20230805.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.810466 autogluon.multimodal-0.8.3b20230804/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-04 09:04:19.806466 autogluon.multimodal-0.8.3b20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:04:19.810466 autogluon.multimodal-0.8.3b20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86709 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    27987 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   120595 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.806466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22866 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.927969 autogluon.multimodal-0.8.3b20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-08-05 09:04:07.927969 autogluon.multimodal-0.8.3b20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:04:07.927969 autogluon.multimodal-0.8.3b20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.919969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86709 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.923969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.923969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27987 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.923969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120595 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.927969 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22866 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-05 09:03:35.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:07.915969 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:04:07.000000 autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.8.3b20230804/PKG-INFO` & `autogluon.multimodal-0.8.3b20230805/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230804
+Version: 0.8.3b20230805
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -17,14 +17,15 @@
         </div>
         
         ## AutoML for Image, Text, Time Series, and Tabular Data
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
+        [![Broken Link Checker](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml/badge.svg)](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
```

### Comparing `autogluon.multimodal-0.8.3b20230804/setup.py` & `autogluon.multimodal-0.8.3b20230805/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.8.3b20230805/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230804
+Version: 0.8.3b20230805
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -17,14 +17,15 @@
         </div>
         
         ## AutoML for Image, Text, Time Series, and Tabular Data
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Continuous Integration](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon/actions/workflows/continuous_integration.yml)
         [![Platform Tests](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml/badge.svg?event=schedule)](https://github.com/autogluon/autogluon/actions/workflows/platform_tests-command.yml)
+        [![Broken Link Checker](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml/badge.svg)](https://github.com/autogluon/autogluon-brokenlinks/actions/workflows/broken_link_checker.yml)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/autogluon/)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
         [![Twitter](https://img.shields.io/twitter/follow/autogluon?style=social)](https://twitter.com/autogluon)
         
         [Install Instructions](https://auto.gluon.ai/stable/install.html) | Documentation ([Stable](https://auto.gluon.ai/stable/index.html) | [Latest](https://auto.gluon.ai/dev/index.html))
```

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.8.3b20230805/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 torchvision<0.16.0,>=0.14.0
 scikit-image<0.20.0,>=0.19.1
 text-unidecode<1.4,>=1.3
 torchmetrics<1.1.0,>=1.0.0
 transformers[sentencepiece]<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
-autogluon.core[raytune]==0.8.3b20230804
-autogluon.features==0.8.3b20230804
-autogluon.common==0.8.3b20230804
+autogluon.core[raytune]==0.8.3b20230805
+autogluon.features==0.8.3b20230805
+autogluon.common==0.8.3b20230805
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

