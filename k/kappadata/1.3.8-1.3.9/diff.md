# Comparing `tmp/kappadata-1.3.8.tar.gz` & `tmp/kappadata-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.3.8.tar", last modified: Wed Jul 26 15:12:57 2023, max compression
+gzip compressed data, was "kappadata-1.3.9.tar", last modified: Wed Jul 26 17:45:31 2023, max compression
```

## Comparing `kappadata-1.3.8.tar` & `kappadata-1.3.9.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.956762 kappadata-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 15:10:18.000000 kappadata-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-26 15:12:57.956762 kappadata-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-26 15:10:18.000000 kappadata-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-26 15:12:41.000000 kappadata-1.3.8/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/kd_dino_mask_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/kd_ijepa_mask_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/norm/kd_ade20k_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.932761 kappadata-1.3.8/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/copying/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.936761 kappadata-1.3.8/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.936761 kappadata-1.3.8/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.936761 kappadata-1.3.8/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/interleaved_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/semi_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/samplers/sequential_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.940762 kappadata-1.3.8/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.944762 kappadata-1.3.8/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_columnwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_minsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_additive_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_random_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_simple_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_three_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/kd_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.944762 kappadata-1.3.8/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/norm/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/save_state_to_context_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.944762 kappadata-1.3.8/kappadata/transforms/semseg/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_random_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.948762 kappadata-1.3.8/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/getall_class_as_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.952762 kappadata-1.3.8/kappadata/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_dataset_imgsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_mae_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_masked_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/visualization/visualize_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.952762 kappadata-1.3.8/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.952762 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.956762 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.956762 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-26 15:10:18.000000 kappadata-1.3.8/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.928761 kappadata-1.3.8/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-26 15:12:57.000000 kappadata-1.3.8/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-26 15:12:57.000000 kappadata-1.3.8/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:12:57.000000 kappadata-1.3.8/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 15:12:57.000000 kappadata-1.3.8/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 15:12:57.000000 kappadata-1.3.8/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 15:10:18.000000 kappadata-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 15:12:57.956762 kappadata-1.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.956762 kappadata-1.3.8/test_unit_long/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:10:18.000000 kappadata-1.3.8/test_unit_long/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-26 15:10:18.000000 kappadata-1.3.8/test_unit_long/test_stochastic_transform_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:12:57.956762 kappadata-1.3.8/tests_external_sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:10:18.000000 kappadata-1.3.8/tests_external_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-26 15:10:18.000000 kappadata-1.3.8/tests_external_sources/dinov2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-26 15:10:18.000000 kappadata-1.3.8/tests_external_sources/ijepa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.390210 kappadata-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 17:42:39.000000 kappadata-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-26 17:45:31.390210 kappadata-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-26 17:42:39.000000 kappadata-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.358208 kappadata-1.3.9/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-26 17:45:11.000000 kappadata-1.3.9/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/kd_dino_mask_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/kd_ijepa_mask_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/norm/kd_ade20k_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/copying/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.366209 kappadata-1.3.9/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.370209 kappadata-1.3.9/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13355 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/interleaved_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/semi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/samplers/sequential_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.374209 kappadata-1.3.9/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.378209 kappadata-1.3.9/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_columnwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_minsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_random_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_simple_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_three_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.378209 kappadata-1.3.9/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/norm/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/save_state_to_context_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.378209 kappadata-1.3.9/kappadata/transforms/semseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.382210 kappadata-1.3.9/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/getall_class_as_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.386210 kappadata-1.3.9/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_dataset_imgsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_mae_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.386210 kappadata-1.3.9/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.386210 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.390210 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.390210 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-26 17:42:39.000000 kappadata-1.3.9/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.362208 kappadata-1.3.9/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-26 17:45:31.000000 kappadata-1.3.9/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-26 17:45:31.000000 kappadata-1.3.9/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:45:31.000000 kappadata-1.3.9/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 17:45:31.000000 kappadata-1.3.9/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 17:45:31.000000 kappadata-1.3.9/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 17:42:39.000000 kappadata-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 17:45:31.390210 kappadata-1.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.390210 kappadata-1.3.9/test_unit_long/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:39.000000 kappadata-1.3.9/test_unit_long/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-26 17:42:39.000000 kappadata-1.3.9/test_unit_long/test_stochastic_transform_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:45:31.390210 kappadata-1.3.9/tests_external_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:42:39.000000 kappadata-1.3.9/tests_external_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-26 17:42:39.000000 kappadata-1.3.9/tests_external_sources/dinov2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-26 17:42:39.000000 kappadata-1.3.9/tests_external_sources/ijepa.py
```

### Comparing `kappadata-1.3.8/LICENSE` & `kappadata-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/PKG-INFO` & `kappadata-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.8
+Version: 1.3.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.8/README.md` & `kappadata-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/__init__.py` & `kappadata-1.3.9/kappadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 import kappadata.caching
 import kappadata.collators
 import kappadata.common
 import kappadata.copying
 import kappadata.datasets
 import kappadata.loading
```

### Comparing `kappadata-1.3.8/kappadata/caching/cached_dataset.py` & `kappadata-1.3.9/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.3.9/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.3.9/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.3.9/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.3.9/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/kd_dino_mask_collator.py` & `kappadata-1.3.9/kappadata/collators/kd_dino_mask_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/kd_ijepa_mask_collator.py` & `kappadata-1.3.9/kappadata/collators/kd_ijepa_mask_collator.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         masks_predictor = [[mask[:min_keep_pred] for mask in masks] for masks in masks_predictor]
         masks_predictor = torch.utils.data.default_collate(masks_predictor)
         masks_encoder = [[mask[:min_keep_enc] for mask in masks] for masks in masks_encoder]
         masks_encoder = torch.utils.data.default_collate(masks_encoder)
 
         ctx["masks_encoder"] = masks_encoder
         ctx["masks_predictor"] = masks_predictor
-        return batch, masks_encoder, masks_predictor
+        return batch
 
     def step(self):
         i = self._itr_counter
         with i.get_lock():
             i.value += 1
             v = i.value
         return v
```

### Comparing `kappadata-1.3.8/kappadata/collators/kd_mix_collator.py` & `kappadata-1.3.9/kappadata/collators/kd_mix_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.3.9/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.3.9/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.3.9/kappadata/common/transforms/byol_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.3.9/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.3.9/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.3.9/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.3.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/copying/folder.py` & `kappadata-1.3.9/kappadata/copying/folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/copying/image_folder.py` & `kappadata-1.3.9/kappadata/copying/image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.3.9/kappadata/datasets/kd_concat_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/datasets/kd_dataset.py` & `kappadata-1.3.9/kappadata/datasets/kd_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/datasets/kd_subset.py` & `kappadata-1.3.9/kappadata/datasets/kd_subset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/datasets/kd_wrapper.py` & `kappadata-1.3.9/kappadata/datasets/kd_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/factory.py` & `kappadata-1.3.9/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/samplers/distributed_sampler.py` & `kappadata-1.3.9/kappadata/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.3.9/kappadata/samplers/infinite_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.3.9/kappadata/samplers/interleaved_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/samplers/random_sampler.py` & `kappadata-1.3.9/kappadata/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/samplers/semi_sampler.py` & `kappadata-1.3.9/kappadata/samplers/semi_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/__init__.py` & `kappadata-1.3.9/kappadata/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.3.9/kappadata/transforms/base/kd_compose_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.3.9/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.3.9/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/base/kd_stochastic_transform.py` & `kappadata-1.3.9/kappadata/transforms/base/kd_stochastic_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/base/kd_transform.py` & `kappadata-1.3.9/kappadata/transforms/base/kd_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.3.9/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.3.9/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_additive_gaussian_noise.py` & `kappadata-1.3.9/kappadata/transforms/kd_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_bucketize.py` & `kappadata-1.3.9/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.3.9/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_columnwise_norm.py` & `kappadata-1.3.9/kappadata/transforms/kd_columnwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.3.9/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.3.9/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_minsize.py` & `kappadata-1.3.9/kappadata/transforms/kd_minsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.3.9/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_additive_gaussian_noise.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_additive_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_apply.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_apply.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_crop.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_grayscale.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_random_threshold.py` & `kappadata-1.3.9/kappadata/transforms/kd_random_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_resize.py` & `kappadata-1.3.9/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_simple_random_crop.py` & `kappadata-1.3.9/kappadata/transforms/kd_simple_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_solarize.py` & `kappadata-1.3.9/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_three_augment.py` & `kappadata-1.3.9/kappadata/transforms/kd_three_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_threshold.py` & `kappadata-1.3.9/kappadata/transforms/kd_threshold.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/kd_two_random_crop.py` & `kappadata-1.3.9/kappadata/transforms/kd_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.3.9/kappadata/transforms/norm/kd_image_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.3.9/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/norm/kd_norm_base.py` & `kappadata-1.3.9/kappadata/transforms/norm/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/patchify_image.py` & `kappadata-1.3.9/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/patchwise_norm.py` & `kappadata-1.3.9/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.3.9/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_pad.py` & `kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_pad.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_random_crop.py` & `kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_random_resize.py` & `kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_random_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/transforms/semseg/kd_semseg_resize.py` & `kappadata-1.3.9/kappadata/transforms/semseg/kd_semseg_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/bounding_box_utils.py` & `kappadata-1.3.9/kappadata/utils/bounding_box_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/class_counts.py` & `kappadata-1.3.9/kappadata/utils/class_counts.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/color_histogram.py` & `kappadata-1.3.9/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/hash_utils.py` & `kappadata-1.3.9/kappadata/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/magnitude_sampler.py` & `kappadata-1.3.9/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/multi_crop_utils.py` & `kappadata-1.3.9/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/pos_embed.py` & `kappadata-1.3.9/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/random.py` & `kappadata-1.3.9/kappadata/utils/random.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/save_image.py` & `kappadata-1.3.9/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/utils/transform_utils.py` & `kappadata-1.3.9/kappadata/utils/transform_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_dataset_imgsize.py` & `kappadata-1.3.9/kappadata/visualization/visualize_dataset_imgsize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_interpolation.py` & `kappadata-1.3.9/kappadata/visualization/visualize_interpolation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_jigsaw.py` & `kappadata-1.3.9/kappadata/visualization/visualize_jigsaw.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_mae_schematic.py` & `kappadata-1.3.9/kappadata/visualization/visualize_mae_schematic.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_masked_image.py` & `kappadata-1.3.9/kappadata/visualization/visualize_masked_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_transform.py` & `kappadata-1.3.9/kappadata/visualization/visualize_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/visualization/visualize_two_random_crop.py` & `kappadata-1.3.9/kappadata/visualization/visualize_two_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/mode_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/mode_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.3.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.3.9/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/kappadata.egg-info/PKG-INFO` & `kappadata-1.3.9/kappadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.3.8
+Version: 1.3.9
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappadata-1.3.8/kappadata.egg-info/SOURCES.txt` & `kappadata-1.3.9/kappadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/setup.cfg` & `kappadata-1.3.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.3.8
+version = 1.3.9
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

### Comparing `kappadata-1.3.8/test_unit_long/test_stochastic_transform_seed.py` & `kappadata-1.3.9/test_unit_long/test_stochastic_transform_seed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/tests_external_sources/dinov2.py` & `kappadata-1.3.9/tests_external_sources/dinov2.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.3.8/tests_external_sources/ijepa.py` & `kappadata-1.3.9/tests_external_sources/ijepa.py`

 * *Files identical despite different names*

