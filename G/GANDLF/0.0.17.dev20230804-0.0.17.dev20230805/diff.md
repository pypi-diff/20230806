# Comparing `tmp/GANDLF-0.0.17.dev20230804.tar.gz` & `tmp/GANDLF-0.0.17.dev20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230804.tar", last modified: Fri Aug  4 03:13:04 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230805.tar", last modified: Sat Aug  5 03:13:14 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230804.tar` & `GANDLF-0.0.17.dev20230805.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.937793 GANDLF-0.0.17.dev20230804/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.885790 GANDLF-0.0.17.dev20230804/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.889790 GANDLF-0.0.17.dev20230804/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.893790 GANDLF-0.0.17.dev20230804/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.897791 GANDLF-0.0.17.dev20230804/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.897791 GANDLF-0.0.17.dev20230804/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.901791 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/hed_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.901791 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.901791 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.901791 GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.905791 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.909791 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.909791 GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.913792 GANDLF-0.0.17.dev20230804/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.913792 GANDLF-0.0.17.dev20230804/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.925792 GANDLF-0.0.17.dev20230804/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.929793 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.933793 GANDLF-0.0.17.dev20230804/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.933793 GANDLF-0.0.17.dev20230804/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.937793 GANDLF-0.0.17.dev20230804/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 03:12:57.000000 GANDLF-0.0.17.dev20230804/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:13:04.885790 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-04 03:13:04.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-04 03:13:04.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 03:13:04.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 03:10:38.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-04 03:13:04.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 03:13:04.000000 GANDLF-0.0.17.dev20230804/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-04 03:13:04.937793 GANDLF-0.0.17.dev20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 03:13:04.937793 GANDLF-0.0.17.dev20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-04 03:10:12.000000 GANDLF-0.0.17.dev20230804/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.426281 GANDLF-0.0.17.dev20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.358280 GANDLF-0.0.17.dev20230805/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.362280 GANDLF-0.0.17.dev20230805/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.366280 GANDLF-0.0.17.dev20230805/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.370280 GANDLF-0.0.17.dev20230805/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.374280 GANDLF-0.0.17.dev20230805/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.374280 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/hed_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.374280 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.378280 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.378280 GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.382280 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.386280 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.390281 GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.390281 GANDLF-0.0.17.dev20230805/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.394281 GANDLF-0.0.17.dev20230805/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.406281 GANDLF-0.0.17.dev20230805/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.418281 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.418281 GANDLF-0.0.17.dev20230805/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.418281 GANDLF-0.0.17.dev20230805/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.426281 GANDLF-0.0.17.dev20230805/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-05 03:13:06.000000 GANDLF-0.0.17.dev20230805/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:13:14.362280 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-05 03:13:14.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-08-05 03:13:14.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:13:14.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:10:42.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-05 03:13:14.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 03:13:14.000000 GANDLF-0.0.17.dev20230805/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-08-05 03:13:14.426281 GANDLF-0.0.17.dev20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 03:13:14.426281 GANDLF-0.0.17.dev20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-08-05 03:10:13.000000 GANDLF-0.0.17.dev20230805/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230804/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230805/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230805/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230805/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230805/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230805/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230805/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/generate_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,21 +279,39 @@
                 gt_image_infill, output_infill
             ).item()
 
             overall_stats_dict[current_subject_id]["mae"] = mean_absolute_error(
                 gt_image_infill, output_infill
             ).item()
 
-            #TODO: use data_range=1.0 as parameter for PSNR when the Pull request is accepted that introduces the data_range parameter!
-            # PSNR - similar to pytorch PeakSignalNoiseRatio until 4 digits after decimal point
+            # torchmetrics PSNR using "max"
             overall_stats_dict[current_subject_id]["psnr"] = peak_signal_noise_ratio(
                 gt_image_infill, output_infill
             ).item()
 
-            overall_stats_dict[current_subject_id]["psnr_eps"] = peak_signal_noise_ratio(
+            # same as above but with epsilon for robustness
+            overall_stats_dict[current_subject_id][
+                "psnr_eps"
+            ] = peak_signal_noise_ratio(
                 gt_image_infill, output_infill, epsilon=sys.float_info.epsilon
             ).item()
 
+            # only use fix data range to [0;1] if the data was normalized before
+            if normalize:
+                # torchmetrics PSNR but with fixed data range of 0 to 1
+                overall_stats_dict[current_subject_id][
+                    "psnr_01"
+                ] = peak_signal_noise_ratio(
+                    gt_image_infill, output_infill, data_range=1.0
+                ).item()
+
+                # same as above but with epsilon for robustness
+                overall_stats_dict[current_subject_id][
+                    "psnr_01_eps"
+                ] = peak_signal_noise_ratio(
+                    gt_image_infill, output_infill, epsilon=sys.float_info.epsilon
+                ).item()
+
     pprint(overall_stats_dict)
     if outputfile is not None:
         with open(outputfile, "w") as outfile:
             yaml.dump(overall_stats_dict, outfile)
```

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230805/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/loss_and_metric.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230805/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/hed_augs.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/hed_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230805/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230805/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230805/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230805/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230805/GANDLF/losses/hybrid.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230805/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230805/GANDLF/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230805/GANDLF/metrics/synthesis.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230805/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230805/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230805/GANDLF/parseConfig.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230805/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230805/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230805/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230805/GANDLF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230804
+Version: 0.0.17.dev20230805
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230804 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230805 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230804/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230805/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/LICENSE` & `GANDLF-0.0.17.dev20230805/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/PKG-INFO` & `GANDLF-0.0.17.dev20230805/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230804
+Version: 0.0.17.dev20230805
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230804 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230805 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230804/README.md` & `GANDLF-0.0.17.dev20230805/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/SECURITY.md` & `GANDLF-0.0.17.dev20230805/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230805/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_collectStats` & `GANDLF-0.0.17.dev20230805/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230805/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230805/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_deploy` & `GANDLF-0.0.17.dev20230805/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230805/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230805/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230805/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_preprocess` & `GANDLF-0.0.17.dev20230805/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230805/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_run` & `GANDLF-0.0.17.dev20230805/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230805/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230804/setup.py` & `GANDLF-0.0.17.dev20230805/setup.py`

 * *Files identical despite different names*

