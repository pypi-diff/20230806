# Comparing `tmp/open-metric-learning-0.4.3.tar.gz` & `tmp/open-metric-learning-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-0.4.3.tar", last modified: Sun Jul  2 15:09:24 2023, max compression
+gzip compressed data, was "dist/open-metric-learning-0.4.4.tar", last modified: Sun Aug  6 17:14:21 2023, max compression
```

## Comparing `open-metric-learning-0.4.3.tar` & `open-metric-learning-0.4.4.tar`

### file list

```diff
@@ -1,220 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    29205 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/extractor/vit_unicom.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.960665 open-metric-learning-0.4.3/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.964665 open-metric-learning-0.4.3/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.968665 open-metric-learning-0.4.3/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.968665 open-metric-learning-0.4.3/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/configs/transforms/unicom_transforms.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/ddp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.972665 open-metric-learning-0.4.3/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (122)     7566 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.976665 open-metric-learning-0.4.3/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    15994 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/meta/siamese.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/resnet/pooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.980665 open-metric-learning-0.4.3/oml/models/vit_clip/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_clip/external/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/external/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_clip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_dino/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_dino/external/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/external/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_dino/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_unicom/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/models/vit_unicom/external/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    11680 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/external/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/models/vit_unicom/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.984665 open-metric-learning-0.4.3/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.988665 open-metric-learning-0.4.3/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    30629 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-07-02 15:09:24.000000 open-metric-learning-0.4.3/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-02 15:09:24.992665 open-metric-learning-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-07-02 15:09:00.000000 open-metric-learning-0.4.3/tests/test_outdated_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    32246 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    30822 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/extractor/vit_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/extractor/vit_unicom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/logger/neptune.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/logger/tensorboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/logger/wandb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.622305 open-metric-learning-0.4.4/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.626305 open-metric-learning-0.4.4/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.626305 open-metric-learning-0.4.4/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.626305 open-metric-learning-0.4.4/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.626305 open-metric-learning-0.4.4/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.626305 open-metric-learning-0.4.4/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/configs/transforms/unicom_transforms.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12302 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/ddp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25034 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2354 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3106 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.630305 open-metric-learning-0.4.4/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9246 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6617 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2956 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7566 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8578 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15994 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6162 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6530 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2620 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.634305 open-metric-learning-0.4.4/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5280 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/meta/siamese.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7770 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/resnet/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/resnet/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_clip/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_clip/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_clip/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_clip/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_clip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_dino/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_dino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_dino/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_dino/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5710 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_dino/external/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_dino/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_dino/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_unicom/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_unicom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/models/vit_unicom/external/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_unicom/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_unicom/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11680 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_unicom/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/models/vit_unicom/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.638305 open-metric-learning-0.4.4/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3818 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6600 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5640 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16347 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    32246 2023-08-06 17:14:21.000000 open-metric-learning-0.4.4/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5826 2023-08-06 17:14:21.000000 open-metric-learning-0.4.4/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-06 17:14:21.000000 open-metric-learning-0.4.4/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-08-06 17:14:21.000000 open-metric-learning-0.4.4/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-08-06 17:14:21.000000 open-metric-learning-0.4.4/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-08-06 17:14:21.646305 open-metric-learning-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-06 17:14:21.642305 open-metric-learning-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-08-06 17:14:02.000000 open-metric-learning-0.4.4/tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-0.4.3/LICENSE` & `open-metric-learning-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/PKG-INFO` & `open-metric-learning-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
 00000020: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00000030: 0a56 6572 7369 6f6e 3a20 302e 342e 330a  .Version: 0.4.3.
+00000030: 0a56 6572 7369 6f6e 3a20 302e 342e 340a  .Version: 0.4.4.
 00000040: 5375 6d6d 6172 793a 204f 4d4c 2069 7320  Summary: OML is 
 00000050: 6120 5079 546f 7263 682d 6261 7365 6420  a PyTorch-based 
 00000060: 6672 616d 6577 6f72 6b20 746f 2074 7261  framework to tra
 00000070: 696e 2061 6e64 2076 616c 6964 6174 6520  in and validate 
 00000080: 7468 6520 6d6f 6465 6c73 2070 726f 6475  the models produ
 00000090: 6369 6e67 2068 6967 682d 7175 616c 6974  cing high-qualit
 000000a0: 7920 656d 6265 6464 696e 6773 2e0a 486f  y embeddings..Ho
@@ -179,1737 +179,1838 @@
 00000b20: 332e 3130 2d70 6173 7369 6e67 2d73 7563  3.10-passing-suc
 00000b30: 6365 7373 295d 2868 7474 7073 3a2f 2f67  cess)](https://g
 00000b40: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
 00000b50: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
 00000b60: 6561 726e 696e 672f 6163 7469 6f6e 732f  earning/actions/
 00000b70: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
 00000b80: 2d76 6572 7369 6f6e 732e 7961 6d6c 2f62  -versions.yaml/b
-00000b90: 6164 6765 2e73 7667 3f29 0a0a 3c64 6976  adge.svg?)..<div
-00000ba0: 2061 6c69 676e 3d22 6c65 6674 223e 0a0a   align="left">..
-00000bb0: 4f4d 4c20 6973 2061 2050 7954 6f72 6368  OML is a PyTorch
-00000bc0: 2d62 6173 6564 2066 7261 6d65 776f 726b  -based framework
-00000bd0: 2074 6f20 7472 6169 6e20 616e 6420 7661   to train and va
-00000be0: 6c69 6461 7465 2074 6865 206d 6f64 656c  lidate the model
-00000bf0: 7320 7072 6f64 7563 696e 6720 6869 6768  s producing high
-00000c00: 2d71 7561 6c69 7479 2065 6d62 6564 6469  -quality embeddi
-00000c10: 6e67 732e 0a0a 2323 205b 4641 515d 2868  ngs...## [FAQ](h
-00000c20: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
-00000c30: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
-00000c40: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000c50: 7465 7374 2f6f 6d6c 2f66 6171 2e68 746d  test/oml/faq.htm
-00000c60: 6c29 0a0a 3c64 6574 6169 6c73 3e0a 3c73  l)..<details>.<s
-00000c70: 756d 6d61 7279 3e57 6879 2064 6f20 4920  ummary>Why do I 
-00000c80: 6e65 6564 204f 4d4c 3f3c 2f73 756d 6d61  need OML?</summa
-00000c90: 7279 3e0a 3c70 3e0a 0a59 6f75 206d 6179  ry>.<p>..You may
-00000ca0: 2074 6869 6e6b 202a 2249 6620 4920 6e65   think *"If I ne
-00000cb0: 6564 2069 6d61 6765 2065 6d62 6564 6469  ed image embeddi
-00000cc0: 6e67 7320 4920 6361 6e20 7369 6d70 6c79  ngs I can simply
-00000cd0: 2074 7261 696e 2061 2076 616e 696c 6c61   train a vanilla
-00000ce0: 2063 6c61 7373 6966 6965 7220 616e 6420   classifier and 
-00000cf0: 7461 6b65 2069 7473 2070 656e 756c 7469  take its penulti
-00000d00: 6d61 7465 206c 6179 6572 222a 2e0a 5765  mate layer"*..We
-00000d10: 6c6c 2c20 6974 206d 616b 6573 2073 656e  ll, it makes sen
-00000d20: 7365 2061 7320 6120 7374 6172 7469 6e67  se as a starting
-00000d30: 2070 6f69 6e74 2e20 4275 7420 7468 6572   point. But ther
-00000d40: 6520 6172 6520 7365 7665 7261 6c20 706f  e are several po
-00000d50: 7373 6962 6c65 2064 7261 7762 6163 6b73  ssible drawbacks
-00000d60: 3a0a 0a2a 2049 6620 796f 7520 7761 6e74  :..* If you want
-00000d70: 2074 6f20 7573 6520 656d 6265 6464 696e   to use embeddin
-00000d80: 6773 2074 6f20 7065 7266 6f72 6d20 7365  gs to perform se
-00000d90: 6172 6368 696e 6720 796f 7520 6e65 6564  arching you need
-00000da0: 2074 6f20 6361 6c63 756c 6174 6520 736f   to calculate so
-00000db0: 6d65 2064 6973 7461 6e63 6520 616d 6f6e  me distance amon
-00000dc0: 6720 7468 656d 2028 666f 7220 6578 616d  g them (for exam
-00000dd0: 706c 652c 2063 6f73 696e 6520 6f72 204c  ple, cosine or L
-00000de0: 3229 2e0a 2020 5573 7561 6c6c 792c 202a  2)..  Usually, *
-00000df0: 2a79 6f75 2064 6f6e 2774 2064 6972 6563  *you don't direc
-00000e00: 746c 7920 6f70 7469 6d69 7a65 2074 6865  tly optimize the
-00000e10: 7365 2064 6973 7461 6e63 6573 2064 7572  se distances dur
-00000e20: 696e 6720 7468 6520 7472 6169 6e69 6e67  ing the training
-00000e30: 2a2a 2069 6e20 7468 6520 636c 6173 7369  ** in the classi
-00000e40: 6669 6361 7469 6f6e 2073 6574 7570 2e20  fication setup. 
-00000e50: 536f 2c20 796f 7520 6361 6e20 6f6e 6c79  So, you can only
-00000e60: 2068 6f70 6520 7468 6174 0a20 2066 696e   hope that.  fin
-00000e70: 616c 2065 6d62 6564 6469 6e67 7320 7769  al embeddings wi
-00000e80: 6c6c 2068 6176 6520 7468 6520 6465 7369  ll have the desi
-00000e90: 7265 6420 7072 6f70 6572 7469 6573 2e0a  red properties..
-00000ea0: 0a2a 202a 2a54 6865 2073 6563 6f6e 6420  .* **The second 
-00000eb0: 7072 6f62 6c65 6d20 6973 2074 6865 2076  problem is the v
-00000ec0: 616c 6964 6174 696f 6e20 7072 6f63 6573  alidation proces
-00000ed0: 732a 2a2e 0a20 2049 6e20 7468 6520 7365  s**..  In the se
-00000ee0: 6172 6368 696e 6720 7365 7475 702c 2079  arching setup, y
-00000ef0: 6f75 2075 7375 616c 6c79 2063 6172 6520  ou usually care 
-00000f00: 686f 7720 7265 6c61 7465 6420 796f 7572  how related your
-00000f10: 2074 6f70 2d4e 206f 7574 7075 7473 2061   top-N outputs a
-00000f20: 7265 2074 6f20 7468 6520 7175 6572 792e  re to the query.
-00000f30: 0a20 2054 6865 206e 6174 7572 616c 2077  .  The natural w
-00000f40: 6179 2074 6f20 6576 616c 7561 7465 2074  ay to evaluate t
-00000f50: 6865 206d 6f64 656c 2069 7320 746f 2073  he model is to s
-00000f60: 696d 756c 6174 6520 7365 6172 6368 696e  imulate searchin
-00000f70: 6720 7265 7175 6573 7473 2074 6f20 7468  g requests to th
-00000f80: 6520 7265 6665 7265 6e63 6520 7365 740a  e reference set.
-00000f90: 2020 616e 6420 6170 706c 7920 6f6e 6520    and apply one 
-00000fa0: 6f66 2074 6865 2072 6574 7269 6576 616c  of the retrieval
-00000fb0: 206d 6574 7269 6373 2e0a 2020 536f 2c20   metrics..  So, 
-00000fc0: 7468 6572 6520 6973 206e 6f20 6775 6172  there is no guar
-00000fd0: 616e 7465 6520 7468 6174 2063 6c61 7373  antee that class
-00000fe0: 6966 6963 6174 696f 6e20 6163 6375 7261  ification accura
-00000ff0: 6379 2077 696c 6c20 636f 7272 656c 6174  cy will correlat
-00001000: 6520 7769 7468 2074 6865 7365 206d 6574  e with these met
-00001010: 7269 6373 2e0a 0a2a 2046 696e 616c 6c79  rics...* Finally
-00001020: 2c20 796f 7520 6d61 7920 7761 6e74 2074  , you may want t
-00001030: 6f20 696d 706c 656d 656e 7420 6120 6d65  o implement a me
-00001040: 7472 6963 206c 6561 726e 696e 6720 7069  tric learning pi
-00001050: 7065 6c69 6e65 2062 7920 796f 7572 7365  peline by yourse
-00001060: 6c66 2e0a 2020 2a2a 5468 6572 6520 6973  lf..  **There is
-00001070: 2061 206c 6f74 206f 6620 776f 726b 2a2a   a lot of work**
-00001080: 3a20 746f 2075 7365 2074 7269 706c 6574  : to use triplet
-00001090: 206c 6f73 7320 796f 7520 6e65 6564 2074   loss you need t
-000010a0: 6f20 666f 726d 2062 6174 6368 6573 2069  o form batches i
-000010b0: 6e20 6120 7370 6563 6966 6963 2077 6179  n a specific way
-000010c0: 2c0a 2020 696d 706c 656d 656e 7420 6469  ,.  implement di
-000010d0: 6666 6572 656e 7420 6b69 6e64 7320 6f66  fferent kinds of
-000010e0: 2074 7269 706c 6574 7320 6d69 6e69 6e67   triplets mining
-000010f0: 2c20 7472 6163 6b69 6e67 2064 6973 7461  , tracking dista
-00001100: 6e63 6573 2c20 6574 632e 2046 6f72 2074  nces, etc. For t
-00001110: 6865 2076 616c 6964 6174 696f 6e2c 2079  he validation, y
-00001120: 6f75 2061 6c73 6f20 6e65 6564 2074 6f0a  ou also need to.
-00001130: 2020 696d 706c 656d 656e 7420 7265 7472    implement retr
-00001140: 6965 7661 6c20 6d65 7472 6963 732c 0a20  ieval metrics,. 
-00001150: 2077 6869 6368 2069 6e63 6c75 6465 2065   which include e
-00001160: 6666 6563 7469 7665 2065 6d62 6564 6469  ffective embeddi
-00001170: 6e67 7320 6163 6375 6d75 6c61 7469 6f6e  ngs accumulation
-00001180: 2064 7572 696e 6720 7468 6520 6570 6f63   during the epoc
-00001190: 682c 2063 6f76 6572 696e 6720 636f 726e  h, covering corn
-000011a0: 6572 2063 6173 6573 2c20 6574 632e 0a20  er cases, etc.. 
-000011b0: 2049 7427 7320 6576 656e 2068 6172 6465   It's even harde
-000011c0: 7220 6966 2079 6f75 2068 6176 6520 7365  r if you have se
-000011d0: 7665 7261 6c20 6770 7573 2061 6e64 2075  veral gpus and u
-000011e0: 7365 2044 4450 2e0a 2020 596f 7520 6d61  se DDP..  You ma
-000011f0: 7920 616c 736f 2077 616e 7420 746f 2076  y also want to v
-00001200: 6973 7561 6c69 7a65 2079 6f75 7220 7365  isualize your se
-00001210: 6172 6368 2072 6571 7565 7374 7320 6279  arch requests by
-00001220: 2068 6967 686c 6967 6874 696e 6720 676f   highlighting go
-00001230: 6f64 2061 6e64 2062 6164 2073 6561 7263  od and bad searc
-00001240: 6820 7265 7375 6c74 732e 0a20 2049 6e73  h results..  Ins
-00001250: 7465 6164 206f 6620 646f 696e 6720 6974  tead of doing it
-00001260: 2062 7920 796f 7572 7365 6c66 2c20 796f   by yourself, yo
-00001270: 7520 6361 6e20 7369 6d70 6c79 2075 7365  u can simply use
-00001280: 204f 4d4c 2066 6f72 2079 6f75 7220 7075   OML for your pu
-00001290: 7270 6f73 6573 2e0a 0a3c 2f70 3e0a 3c2f  rposes...</p>.</
-000012a0: 6465 7461 696c 733e 0a0a 0a3c 6465 7461  details>...<deta
-000012b0: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-000012c0: 6174 2069 7320 7468 6520 6469 6666 6572  at is the differ
-000012d0: 656e 6365 2062 6574 7765 656e 204f 7065  ence between Ope
-000012e0: 6e20 4d65 7472 6963 204c 6561 726e 696e  n Metric Learnin
-000012f0: 6720 616e 6420 5079 546f 7263 6820 4d65  g and PyTorch Me
-00001300: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
-00001310: 7375 6d6d 6172 793e 0a3c 703e 0a0a 5b50  summary>.<p>..[P
-00001320: 4d4c 5d28 6874 7470 733a 2f2f 6769 7468  ML](https://gith
-00001330: 7562 2e63 6f6d 2f4b 6576 696e 4d75 7367  ub.com/KevinMusg
-00001340: 7261 7665 2f70 7974 6f72 6368 2d6d 6574  rave/pytorch-met
-00001350: 7269 632d 6c65 6172 6e69 6e67 2920 6973  ric-learning) is
-00001360: 2074 6865 2070 6f70 756c 6172 206c 6962   the popular lib
-00001370: 7261 7279 2066 6f72 204d 6574 7269 6320  rary for Metric 
-00001380: 4c65 6172 6e69 6e67 2c0a 616e 6420 6974  Learning,.and it
-00001390: 2069 6e63 6c75 6465 7320 6120 7269 6368   includes a rich
-000013a0: 2063 6f6c 6c65 6374 696f 6e20 6f66 206c   collection of l
-000013b0: 6f73 7365 732c 206d 696e 6572 732c 2064  osses, miners, d
-000013c0: 6973 7461 6e63 6573 2c20 616e 6420 7265  istances, and re
-000013d0: 6475 6365 7273 3b20 7468 6174 2069 7320  ducers; that is 
-000013e0: 7768 7920 7765 2070 726f 7669 6465 2073  why we provide s
-000013f0: 7472 6169 6768 7466 6f72 7761 7264 0a5b  traightforward.[
-00001400: 6578 616d 706c 6573 5d28 6874 7470 733a  examples](https:
-00001410: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00001420: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00001430: 632d 6c65 6172 6e69 6e67 2375 7361 6765  c-learning#usage
-00001440: 2d77 6974 682d 7079 746f 7263 682d 6d65  -with-pytorch-me
-00001450: 7472 6963 2d6c 6561 726e 696e 6729 206f  tric-learning) o
-00001460: 6620 7573 696e 6720 7468 656d 2077 6974  f using them wit
-00001470: 6820 4f4d 4c2e 0a49 6e69 7469 616c 6c79  h OML..Initially
-00001480: 2c20 7765 2074 7269 6564 2074 6f20 7573  , we tried to us
-00001490: 6520 504d 4c2c 2062 7574 2069 6e20 7468  e PML, but in th
-000014a0: 6520 656e 642c 2077 6520 6361 6d65 2075  e end, we came u
-000014b0: 7020 7769 7468 206f 7572 206c 6962 7261  p with our libra
-000014c0: 7279 2c20 7768 6963 6820 6973 206d 6f72  ry, which is mor
-000014d0: 6520 7069 7065 6c69 6e65 202f 2072 6563  e pipeline / rec
-000014e0: 6970 6573 206f 7269 656e 7465 642e 0a54  ipes oriented..T
-000014f0: 6861 7420 6973 2068 6f77 204f 4d4c 2064  hat is how OML d
-00001500: 6966 6665 7273 2066 726f 6d20 504d 4c3a  iffers from PML:
-00001510: 0a0a 2a20 4f4d 4c20 6861 7320 5b50 6970  ..* OML has [Pip
-00001520: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00001530: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-00001540: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00001550: 6c65 6172 6e69 6e67 2f74 7265 652f 6d61  learning/tree/ma
-00001560: 696e 2f70 6970 656c 696e 6573 290a 2020  in/pipelines).  
-00001570: 7768 6963 6820 616c 6c6f 7773 2074 7261  which allows tra
-00001580: 696e 696e 6720 6d6f 6465 6c73 2062 7920  ining models by 
-00001590: 7072 6570 6172 696e 6720 6120 636f 6e66  preparing a conf
-000015a0: 6967 2061 6e64 2079 6f75 7220 6461 7461  ig and your data
-000015b0: 2069 6e20 7468 6520 7265 7175 6972 6564   in the required
-000015c0: 2066 6f72 6d61 740a 2020 2869 7427 7320   format.  (it's 
-000015d0: 6c69 6b65 2063 6f6e 7665 7274 696e 6720  like converting 
-000015e0: 6461 7461 2069 6e74 6f20 434f 434f 2066  data into COCO f
-000015f0: 6f72 6d61 7420 746f 2074 7261 696e 2061  ormat to train a
-00001600: 2064 6574 6563 746f 7220 6672 6f6d 205b   detector from [
-00001610: 6d6d 6465 7465 6374 696f 6e5d 2868 7474  mmdetection](htt
-00001620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001630: 6f70 656e 2d6d 6d6c 6162 2f6d 6d64 6574  open-mmlab/mmdet
-00001640: 6563 7469 6f6e 2929 2e0a 0a2a 204f 4d4c  ection))...* OML
-00001650: 2066 6f63 7573 6573 206f 6e20 656e 642d   focuses on end-
-00001660: 746f 2d65 6e64 2070 6970 656c 696e 6573  to-end pipelines
-00001670: 2061 6e64 2070 7261 6374 6963 616c 2075   and practical u
-00001680: 7365 2063 6173 6573 2e0a 2020 4974 2068  se cases..  It h
-00001690: 6173 2063 6f6e 6669 6720 6261 7365 6420  as config based 
-000016a0: 6578 616d 706c 6573 206f 6e20 706f 7075  examples on popu
-000016b0: 6c61 7220 6265 6e63 686d 6172 6b73 2063  lar benchmarks c
-000016c0: 6c6f 7365 2074 6f20 7265 616c 206c 6966  lose to real lif
-000016d0: 6520 286c 696b 6520 7068 6f74 6f73 206f  e (like photos o
-000016e0: 6620 7072 6f64 7563 7473 206f 6620 7468  f products of th
-000016f0: 6f75 7361 6e64 7320 6964 7329 2e0a 2020  ousands ids)..  
-00001700: 5765 2066 6f75 6e64 2073 6f6d 6520 676f  We found some go
-00001710: 6f64 2063 6f6d 6269 6e61 7469 6f6e 7320  od combinations 
-00001720: 6f66 2068 7970 6572 7061 7261 6d65 7465  of hyperparamete
-00001730: 7273 206f 6e20 7468 6573 6520 6461 7461  rs on these data
-00001740: 7365 7473 2c20 7472 6169 6e65 6420 616e  sets, trained an
-00001750: 6420 7075 626c 6973 6865 6420 6d6f 6465  d published mode
-00001760: 6c73 2061 6e64 2074 6865 6972 2063 6f6e  ls and their con
-00001770: 6669 6773 2e0a 2020 5468 7573 2c20 6974  figs..  Thus, it
-00001780: 206d 616b 6573 204f 4d4c 206d 6f72 6520   makes OML more 
-00001790: 7265 6369 7065 7320 6f72 6965 6e74 6564  recipes oriented
-000017a0: 2074 6861 6e20 504d 4c2c 2061 6e64 2069   than PML, and i
-000017b0: 7473 2061 7574 686f 720a 2020 5b63 6f6e  ts author.  [con
-000017c0: 6669 726d 735d 2868 7474 7073 3a2f 2f67  firms](https://g
-000017d0: 6974 6875 622e 636f 6d2f 4b65 7669 6e4d  ithub.com/KevinM
-000017e0: 7573 6772 6176 652f 7079 746f 7263 682d  usgrave/pytorch-
-000017f0: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
-00001800: 6973 7375 6573 2f31 3639 2369 7373 7565  issues/169#issue
-00001810: 636f 6d6d 656e 742d 3637 3038 3134 3339  comment-67081439
-00001820: 3329 0a20 2074 6869 7320 7361 7969 6e67  3).  this saying
-00001830: 2074 6861 7420 6869 7320 6c69 6272 6172   that his librar
-00001840: 7920 6973 2061 2073 6574 206f 6620 746f  y is a set of to
-00001850: 6f6c 7320 7261 7468 6572 2074 6865 2072  ols rather the r
-00001860: 6563 6970 6573 2c20 6d6f 7265 6f76 6572  ecipes, moreover
-00001870: 2c20 7468 6520 6578 616d 706c 6573 2069  , the examples i
-00001880: 6e20 504d 4c20 6172 6520 6d6f 7374 6c79  n PML are mostly
-00001890: 2066 6f72 2043 4946 4152 2061 6e64 204d   for CIFAR and M
-000018a0: 4e49 5354 2064 6174 6173 6574 732e 0a0a  NIST datasets...
-000018b0: 2a20 4f4d 4c20 6861 7320 7468 6520 5b5a  * OML has the [Z
-000018c0: 6f6f 5d28 6874 7470 733a 2f2f 6769 7468  oo](https://gith
-000018d0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-000018e0: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-000018f0: 6e69 6e67 237a 6f6f 2920 6f66 2070 7265  ning#zoo) of pre
-00001900: 7472 6169 6e65 6420 6d6f 6465 6c73 2074  trained models t
-00001910: 6861 7420 6361 6e20 6265 2065 6173 696c  hat can be easil
-00001920: 7920 6163 6365 7373 6564 2066 726f 6d0a  y accessed from.
-00001930: 2020 7468 6520 636f 6465 2069 6e20 7468    the code in th
-00001940: 6520 7361 6d65 2077 6179 2061 7320 696e  e same way as in
-00001950: 2060 746f 7263 6876 6973 696f 6e60 2028   `torchvision` (
-00001960: 7768 656e 2079 6f75 2074 7970 6520 6072  when you type `r
-00001970: 6573 6e65 7435 3028 7072 6574 7261 696e  esnet50(pretrain
-00001980: 6564 3d54 7275 6529 6029 2e0a 0a2a 204f  ed=True)`)...* O
-00001990: 4d4c 2069 7320 696e 7465 6772 6174 6564  ML is integrated
-000019a0: 2077 6974 6820 5b50 7954 6f72 6368 204c   with [PyTorch L
-000019b0: 6967 6874 6e69 6e67 5d28 6874 7470 733a  ightning](https:
-000019c0: 2f2f 7777 772e 7079 746f 7263 686c 6967  //www.pytorchlig
-000019d0: 6874 6e69 6e67 2e61 692f 292c 2073 6f2c  htning.ai/), so,
-000019e0: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-000019f0: 706f 7765 7220 6f66 2069 7473 0a20 205b  power of its.  [
-00001a00: 5472 6169 6e65 725d 2868 7474 7073 3a2f  Trainer](https:/
-00001a10: 2f70 7974 6f72 6368 2d6c 6967 6874 6e69  /pytorch-lightni
-00001a20: 6e67 2e72 6561 6474 6865 646f 6373 2e69  ng.readthedocs.i
-00001a30: 6f2f 656e 2f73 7461 626c 652f 636f 6d6d  o/en/stable/comm
-00001a40: 6f6e 2f74 7261 696e 6572 2e68 746d 6c29  on/trainer.html)
-00001a50: 2e0a 2020 5468 6973 2069 7320 6573 7065  ..  This is espe
-00001a60: 6369 616c 6c79 2068 656c 7066 756c 2077  cially helpful w
-00001a70: 6865 6e20 7765 2077 6f72 6b20 7769 7468  hen we work with
-00001a80: 2044 4450 2c20 736f 2c20 796f 7520 636f   DDP, so, you co
-00001a90: 6d70 6172 6520 6f75 720a 2020 5b44 4450  mpare our.  [DDP
-00001aa0: 2065 7861 6d70 6c65 5d28 6874 7470 733a   example](https:
-00001ab0: 2f2f 6f70 656e 2d6d 6574 7269 632d 6c65  //open-metric-le
-00001ac0: 6172 6e69 6e67 2e72 6561 6474 6865 646f  arning.readthedo
-00001ad0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001ae0: 6578 616d 706c 6573 2f70 7974 686f 6e2e  examples/python.
-00001af0: 6874 6d6c 290a 2020 616e 6420 7468 650a  html).  and the.
-00001b00: 2020 5b50 4d4c 7320 6f6e 655d 2868 7474    [PMLs one](htt
-00001b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001b20: 4b65 7669 6e4d 7573 6772 6176 652f 7079  KevinMusgrave/py
-00001b30: 746f 7263 682d 6d65 7472 6963 2d6c 6561  torch-metric-lea
-00001b40: 726e 696e 672f 626c 6f62 2f6d 6173 7465  rning/blob/maste
-00001b50: 722f 6578 616d 706c 6573 2f6e 6f74 6562  r/examples/noteb
-00001b60: 6f6f 6b73 2f44 6973 7472 6962 7574 6564  ooks/Distributed
-00001b70: 5472 6970 6c65 744d 6172 6769 6e4c 6f73  TripletMarginLos
-00001b80: 734d 4e49 5354 2e69 7079 6e62 292e 0a20  sMNIST.ipynb).. 
-00001b90: 2042 7920 7468 6520 7761 792c 2050 4d4c   By the way, PML
-00001ba0: 2061 6c73 6f20 6861 7320 5b54 7261 696e   also has [Train
-00001bb0: 6572 735d 2868 7474 7073 3a2f 2f6b 6576  ers](https://kev
-00001bc0: 696e 6d75 7367 7261 7665 2e67 6974 6875  inmusgrave.githu
-00001bd0: 622e 696f 2f70 7974 6f72 6368 2d6d 6574  b.io/pytorch-met
-00001be0: 7269 632d 6c65 6172 6e69 6e67 2f74 7261  ric-learning/tra
-00001bf0: 696e 6572 732f 292c 2062 7574 2069 7427  iners/), but it'
-00001c00: 7320 6e6f 740a 2020 7769 6465 6c79 2075  s not.  widely u
-00001c10: 7365 6420 696e 2074 6865 2065 7861 6d70  sed in the examp
-00001c20: 6c65 7320 616e 6420 6375 7374 6f6d 2060  les and custom `
-00001c30: 7472 6169 6e60 202f 2060 7465 7374 6020  train` / `test` 
-00001c40: 6675 6e63 7469 6f6e 7320 6172 6520 7573  functions are us
-00001c50: 6564 2069 6e73 7465 6164 2e0a 0a57 6520  ed instead...We 
-00001c60: 6265 6c69 6576 6520 7468 6174 2068 6176  believe that hav
-00001c70: 696e 6720 5069 7065 6c69 6e65 732c 206c  ing Pipelines, l
-00001c80: 6163 6f6e 6963 2065 7861 6d70 6c65 732c  aconic examples,
-00001c90: 2061 6e64 205a 6f6f 206f 6620 7072 6574   and Zoo of pret
-00001ca0: 7261 696e 6564 206d 6f64 656c 7320 7365  rained models se
-00001cb0: 7473 2074 6865 2065 6e74 7279 2074 6872  ts the entry thr
-00001cc0: 6573 686f 6c64 2074 6f20 6120 7265 616c  eshold to a real
-00001cd0: 6c79 206c 6f77 2076 616c 7565 2e0a 0a3c  ly low value...<
-00001ce0: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
-00001cf0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
-00001d00: 6172 793e 5768 6174 2069 7320 4d65 7472  ary>What is Metr
-00001d10: 6963 204c 6561 726e 696e 673f 3c2f 7375  ic Learning?</su
-00001d20: 6d6d 6172 793e 0a3c 703e 0a0a 4d65 7472  mmary>.<p>..Metr
-00001d30: 6963 204c 6561 726e 696e 6720 7072 6f62  ic Learning prob
-00001d40: 6c65 6d20 2861 6c73 6f20 6b6e 6f77 6e20  lem (also known 
-00001d50: 6173 202a 6578 7472 656d 6520 636c 6173  as *extreme clas
-00001d60: 7369 6669 6361 7469 6f6e 2a20 7072 6f62  sification* prob
-00001d70: 6c65 6d29 206d 6561 6e73 2061 2073 6974  lem) means a sit
-00001d80: 7561 7469 6f6e 2069 6e20 7768 6963 6820  uation in which 
-00001d90: 7765 0a68 6176 6520 7468 6f75 7361 6e64  we.have thousand
-00001da0: 7320 6f66 2069 6473 206f 6620 736f 6d65  s of ids of some
-00001db0: 2065 6e74 6974 6965 732c 2062 7574 206f   entities, but o
-00001dc0: 6e6c 7920 6120 6665 7720 7361 6d70 6c65  nly a few sample
-00001dd0: 7320 666f 7220 6576 6572 7920 656e 7469  s for every enti
-00001de0: 7479 2e0a 4f66 7465 6e20 7765 2061 7373  ty..Often we ass
-00001df0: 756d 6520 7468 6174 2064 7572 696e 6720  ume that during 
-00001e00: 7468 6520 7465 7374 2073 7461 6765 2028  the test stage (
-00001e10: 6f72 2070 726f 6475 6374 696f 6e29 2077  or production) w
-00001e20: 6520 7769 6c6c 2064 6561 6c20 7769 7468  e will deal with
-00001e30: 2075 6e73 6565 6e20 656e 7469 7469 6573   unseen entities
-00001e40: 0a77 6869 6368 206d 616b 6573 2069 7420  .which makes it 
-00001e50: 696d 706f 7373 6962 6c65 2074 6f20 6170  impossible to ap
-00001e60: 706c 7920 7468 6520 7661 6e69 6c6c 6120  ply the vanilla 
-00001e70: 636c 6173 7369 6669 6361 7469 6f6e 2070  classification p
-00001e80: 6970 656c 696e 6520 6469 7265 6374 6c79  ipeline directly
-00001e90: 2e20 496e 206d 616e 7920 6361 7365 7320  . In many cases 
-00001ea0: 6f62 7461 696e 6564 2065 6d62 6564 6469  obtained embeddi
-00001eb0: 6e67 730a 6172 6520 7573 6564 2074 6f20  ngs.are used to 
-00001ec0: 7065 7266 6f72 6d20 7365 6172 6368 206f  perform search o
-00001ed0: 7220 6d61 7463 6869 6e67 2070 726f 6365  r matching proce
-00001ee0: 6475 7265 7320 6f76 6572 2074 6865 6d2e  dures over them.
-00001ef0: 0a0a 4865 7265 2061 7265 2061 2066 6577  ..Here are a few
-00001f00: 2065 7861 6d70 6c65 7320 6f66 2073 7563   examples of suc
-00001f10: 6820 7461 736b 7320 6672 6f6d 2074 6865  h tasks from the
-00001f20: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-00001f30: 2073 7068 6572 653a 0a2a 2050 6572 736f   sphere:.* Perso
-00001f40: 6e2f 416e 696d 616c 2052 652d 4964 656e  n/Animal Re-Iden
-00001f50: 7469 6669 6361 7469 6f6e 0a2a 2046 6163  tification.* Fac
-00001f60: 6520 5265 636f 676e 6974 696f 6e0a 2a20  e Recognition.* 
-00001f70: 4c61 6e64 6d61 726b 2052 6563 6f67 6e69  Landmark Recogni
-00001f80: 7469 6f6e 0a2a 2053 6561 7263 6869 6e67  tion.* Searching
-00001f90: 2065 6e67 696e 6573 2066 6f72 206f 6e6c   engines for onl
-00001fa0: 696e 6520 7368 6f70 730a 2061 6e64 206d  ine shops. and m
-00001fb0: 616e 7920 6f74 6865 7273 2e0a 3c2f 703e  any others..</p>
-00001fc0: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
-00001fd0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00001fe0: 3e47 6c6f 7373 6172 7920 284e 616d 696e  >Glossary (Namin
-00001ff0: 6720 636f 6e76 656e 7469 6f6e 2920 3c2f  g convention) </
-00002000: 7375 6d6d 6172 793e 0a3c 703e 0a0a 2a20  summary>.<p>..* 
-00002010: 6065 6d62 6564 6469 6e67 6020 2d20 6d6f  `embedding` - mo
-00002020: 6465 6c27 7320 6f75 7470 7574 2028 616c  del's output (al
-00002030: 736f 206b 6e6f 776e 2061 7320 6066 6561  so known as `fea
-00002040: 7475 7265 7320 7665 6374 6f72 6020 6f72  tures vector` or
-00002050: 2060 6465 7363 7269 7074 6f72 6029 2e0a   `descriptor`)..
-00002060: 2a20 6071 7565 7279 6020 2d20 6120 7361  * `query` - a sa
-00002070: 6d70 6c65 2077 6869 6368 2069 7320 7573  mple which is us
-00002080: 6564 2061 7320 6120 7265 7175 6573 7420  ed as a request 
-00002090: 696e 2074 6865 2072 6574 7269 6576 616c  in the retrieval
-000020a0: 2070 726f 6365 6475 7265 2e0a 2a20 6067   procedure..* `g
-000020b0: 616c 6c65 7279 2073 6574 6020 2d20 7468  allery set` - th
-000020c0: 6520 7365 7420 6f66 2065 6e74 6974 6965  e set of entitie
-000020d0: 7320 746f 2073 6561 7263 6820 6974 656d  s to search item
-000020e0: 7320 7369 6d69 6c61 7220 746f 2060 7175  s similar to `qu
-000020f0: 6572 7960 2028 616c 736f 206b 6e6f 776e  ery` (also known
-00002100: 2061 7320 6072 6566 6572 656e 6365 6020   as `reference` 
-00002110: 6f72 2060 696e 6465 7860 292e 0a2a 2060  or `index`)..* `
-00002120: 5361 6d70 6c65 7260 202d 2061 6e20 6172  Sampler` - an ar
-00002130: 6775 6d65 6e74 2066 6f72 2060 4461 7461  gument for `Data
-00002140: 4c6f 6164 6572 6020 7768 6963 6820 6973  Loader` which is
-00002150: 2075 7365 6420 746f 2066 6f72 6d20 6261   used to form ba
-00002160: 7463 6865 730a 2a20 604d 696e 6572 6020  tches.* `Miner` 
-00002170: 2d20 7468 6520 6f62 6a65 6374 2074 6f20  - the object to 
-00002180: 666f 726d 2070 6169 7273 206f 7220 7472  form pairs or tr
-00002190: 6970 6c65 7473 2061 6674 6572 2074 6865  iplets after the
-000021a0: 2062 6174 6368 2077 6173 2066 6f72 6d65   batch was forme
-000021b0: 6420 6279 2060 5361 6d70 6c65 7260 2e20  d by `Sampler`. 
-000021c0: 4974 2773 206e 6f74 206e 6563 6573 7361  It's not necessa
-000021d0: 7279 2074 6f20 666f 726d 0a20 2074 6865  ry to form.  the
-000021e0: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
-000021f0: 2073 616d 706c 6573 206f 6e6c 7920 696e   samples only in
-00002200: 7369 6465 2074 6865 2063 7572 7265 6e74  side the current
-00002210: 2062 6174 6368 2c20 7468 7573 2c20 7468   batch, thus, th
-00002220: 6520 6d65 6d6f 7279 2062 616e 6b20 6d61  e memory bank ma
-00002230: 7920 6265 2061 2070 6172 7420 6f66 2060  y be a part of `
-00002240: 4d69 6e65 7260 2e0a 2a20 6053 616d 706c  Miner`..* `Sampl
-00002250: 6573 602f 604c 6162 656c 7360 2f60 496e  es`/`Labels`/`In
-00002260: 7374 616e 6365 7360 202d 2061 7320 616e  stances` - as an
-00002270: 2065 7861 6d70 6c65 206c 6574 2773 2063   example let's c
-00002280: 6f6e 7369 6465 7220 4465 6570 4661 7368  onsider DeepFash
-00002290: 696f 6e20 6461 7461 7365 742e 2049 7420  ion dataset. It 
-000022a0: 696e 636c 7564 6573 2074 686f 7573 616e  includes thousan
-000022b0: 6473 206f 660a 2020 6661 7368 696f 6e20  ds of.  fashion 
-000022c0: 6974 656d 2069 6473 2028 7765 206e 616d  item ids (we nam
-000022d0: 6520 7468 656d 2060 6c61 6265 6c73 6029  e them `labels`)
-000022e0: 2061 6e64 2073 6576 6572 616c 2070 686f   and several pho
-000022f0: 746f 7320 666f 7220 6561 6368 2069 7465  tos for each ite
-00002300: 6d20 6964 0a20 2028 7765 206e 616d 6520  m id.  (we name 
-00002310: 7468 6520 696e 6469 7669 6475 616c 2070  the individual p
-00002320: 686f 746f 2061 7320 6069 6e73 7461 6e63  hoto as `instanc
-00002330: 6560 206f 7220 6073 616d 706c 6560 292e  e` or `sample`).
-00002340: 2041 6c6c 206f 6620 7468 6520 6661 7368   All of the fash
-00002350: 696f 6e20 6974 656d 2069 6473 2068 6176  ion item ids hav
-00002360: 6520 7468 6569 7220 6772 6f75 7073 206c  e their groups l
-00002370: 696b 650a 2020 2273 6b69 7274 7322 2c20  ike.  "skirts", 
-00002380: 226a 6163 6b65 7473 222c 2022 7368 6f72  "jackets", "shor
-00002390: 7473 2220 616e 6420 736f 206f 6e20 2877  ts" and so on (w
-000023a0: 6520 6e61 6d65 2074 6865 6d20 6063 6174  e name them `cat
-000023b0: 6567 6f72 6965 7360 292e 0a20 204e 6f74  egories`)..  Not
-000023c0: 652c 2077 6520 6176 6f69 6420 7573 696e  e, we avoid usin
-000023d0: 6720 7468 6520 7465 726d 2060 636c 6173  g the term `clas
-000023e0: 7360 2074 6f20 6176 6f69 6420 6d69 7375  s` to avoid misu
-000023f0: 6e64 6572 7374 616e 6469 6e67 2e0a 2a20  nderstanding..* 
-00002400: 6074 7261 696e 696e 6720 6570 6f63 6860  `training epoch`
-00002410: 202d 2062 6174 6368 2073 616d 706c 6572   - batch sampler
-00002420: 7320 7768 6963 6820 7765 2075 7365 2066  s which we use f
-00002430: 6f72 2063 6f6d 6269 6e61 7469 6f6e 2d62  or combination-b
-00002440: 6173 6564 206c 6f73 7365 7320 7573 7561  ased losses usua
-00002450: 6c6c 7920 6861 7665 2061 206c 656e 6774  lly have a lengt
-00002460: 6820 6571 7561 6c20 746f 0a20 2060 5b6e  h equal to.  `[n
-00002470: 756d 6265 7220 6f66 206c 6162 656c 7320  umber of labels 
-00002480: 696e 2074 7261 696e 696e 6720 6461 7461  in training data
-00002490: 7365 745d 202f 205b 6e75 6d62 6572 7320  set] / [numbers 
-000024a0: 6f66 206c 6162 656c 7320 696e 206f 6e65  of labels in one
-000024b0: 2062 6174 6368 5d60 2e20 4974 206d 6561   batch]`. It mea
-000024c0: 6e73 2074 6861 7420 7765 2064 6f6e 2774  ns that we don't
-000024d0: 206f 6273 6572 7665 2061 6c6c 206f 660a   observe all of.
-000024e0: 2020 7468 6520 6176 6169 6c61 626c 6520    the available 
-000024f0: 7472 6169 6e69 6e67 2073 616d 706c 6573  training samples
-00002500: 2069 6e20 6f6e 6520 6570 6f63 6820 2861   in one epoch (a
-00002510: 7320 6f70 706f 7365 6420 746f 2076 616e  s opposed to van
-00002520: 696c 6c61 2063 6c61 7373 6966 6963 6174  illa classificat
-00002530: 696f 6e29 2c0a 2020 696e 7374 6561 642c  ion),.  instead,
-00002540: 2077 6520 6f62 7365 7276 6520 616c 6c20   we observe all 
-00002550: 6f66 2074 6865 2061 7661 696c 6162 6c65  of the available
-00002560: 206c 6162 656c 732e 0a0a 3c2f 703e 0a3c   labels...</p>.<
-00002570: 2f64 6574 6169 6c73 3e0a 0a0a 3c64 6574  /details>...<det
-00002580: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e48  ails>.<summary>H
-00002590: 6f77 2067 6f6f 6420 6d61 7920 6265 2061  ow good may be a
-000025a0: 206d 6f64 656c 2074 7261 696e 6564 2077   model trained w
-000025b0: 6974 6820 4f4d 4c3f 203c 2f73 756d 6d61  ith OML? </summa
-000025c0: 7279 3e0a 3c70 3e0a 0a49 7420 6d61 7920  ry>.<p>..It may 
-000025d0: 6265 2063 6f6d 7061 7261 626c 6520 7769  be comparable wi
-000025e0: 7468 2074 6865 2063 7572 7265 6e74 2028  th the current (
-000025f0: 3230 3232 2079 6561 7229 205b 536f 7441  2022 year) [SotA
-00002600: 5d28 6874 7470 733a 2f2f 7061 7065 7273  ](https://papers
-00002610: 7769 7468 636f 6465 2e63 6f6d 2f74 6173  withcode.com/tas
-00002620: 6b2f 6d65 7472 6963 2d6c 6561 726e 696e  k/metric-learnin
-00002630: 6729 206d 6574 686f 6473 2c0a 666f 7220  g) methods,.for 
-00002640: 6578 616d 706c 652c 205b 4879 702d 5669  example, [Hyp-Vi
-00002650: 545d 2868 7474 7073 3a2f 2f61 7278 6976  T](https://arxiv
-00002660: 2e6f 7267 2f70 6466 2f32 3230 332e 3130  .org/pdf/2203.10
-00002670: 3833 332e 7064 6629 2e0a 2a28 4665 7720  833.pdf)..*(Few 
-00002680: 776f 7264 7320 6162 6f75 7420 7468 6973  words about this
-00002690: 2061 7070 726f 6163 683a 2069 7427 7320   approach: it's 
-000026a0: 6120 5669 5420 6172 6368 6974 6563 7475  a ViT architectu
-000026b0: 7265 2074 7261 696e 6564 2077 6974 6820  re trained with 
-000026c0: 636f 6e74 7261 7374 6976 6520 6c6f 7373  contrastive loss
-000026d0: 2c0a 6275 7420 7468 6520 656d 6265 6464  ,.but the embedd
-000026e0: 696e 6773 2077 6572 6520 7072 6f6a 6563  ings were projec
-000026f0: 7465 6420 696e 746f 2073 6f6d 6520 6879  ted into some hy
-00002700: 7065 7262 6f6c 6963 2073 7061 6365 2e0a  perbolic space..
-00002710: 4173 2074 6865 2061 7574 686f 7273 2063  As the authors c
-00002720: 6c61 696d 6564 2c20 7375 6368 2061 2073  laimed, such a s
-00002730: 7061 6365 2069 7320 6162 6c65 2074 6f20  pace is able to 
-00002740: 6465 7363 7269 6265 2074 6865 206e 6573  describe the nes
-00002750: 7465 6420 7374 7275 6374 7572 6520 6f66  ted structure of
-00002760: 2072 6561 6c2d 776f 726c 6420 6461 7461   real-world data
-00002770: 2e0a 536f 2c20 7468 6520 7061 7065 7220  ..So, the paper 
-00002780: 7265 7175 6972 6573 2073 6f6d 6520 6865  requires some he
-00002790: 6176 7920 6d61 7468 2074 6f20 6164 6170  avy math to adap
-000027a0: 7420 7468 6520 7573 7561 6c20 6f70 6572  t the usual oper
-000027b0: 6174 696f 6e73 2066 6f72 2074 6865 2068  ations for the h
-000027c0: 7970 6572 626f 6c69 6361 6c20 7370 6163  yperbolical spac
-000027d0: 652e 292a 0a0a 5765 2074 7261 696e 6564  e.)*..We trained
-000027e0: 2074 6865 2073 616d 6520 6172 6368 6974   the same archit
-000027f0: 6563 7475 7265 2077 6974 6820 7472 6970  ecture with trip
-00002800: 6c65 7420 6c6f 7373 2c20 6669 7869 6e67  let loss, fixing
-00002810: 2074 6865 2072 6573 7420 6f66 2074 6865   the rest of the
-00002820: 2070 6172 616d 6574 6572 733a 0a74 7261   parameters:.tra
-00002830: 696e 696e 6720 616e 6420 7465 7374 2074  ining and test t
-00002840: 7261 6e73 666f 726d 6174 696f 6e73 2c20  ransformations, 
-00002850: 696d 6167 6520 7369 7a65 2c20 616e 6420  image size, and 
-00002860: 6f70 7469 6d69 7a65 722e 2053 6565 2063  optimizer. See c
-00002870: 6f6e 6669 6773 2069 6e20 5b4d 6f64 656c  onfigs in [Model
-00002880: 7320 5a6f 6f5d 2868 7474 7073 3a2f 2f67  s Zoo](https://g
-00002890: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-000028a0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-000028b0: 6561 726e 696e 6723 7a6f 6f29 2e0a 5468  earning#zoo)..Th
-000028c0: 6520 7472 6963 6b20 7761 7320 696e 2068  e trick was in h
-000028d0: 6575 7269 7374 6963 7320 696e 206f 7572  euristics in our
-000028e0: 206d 696e 6572 2061 6e64 2073 616d 706c   miner and sampl
-000028f0: 6572 3a0a 0a2a 205b 4361 7465 676f 7279  er:..* [Category
-00002900: 2042 616c 616e 6365 2053 616d 706c 6572   Balance Sampler
-00002910: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00002920: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00002930: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00002940: 2f6c 6174 6573 742f 636f 6e74 656e 7473  /latest/contents
-00002950: 2f73 616d 706c 6572 732e 6874 6d6c 2363  /samplers.html#c
-00002960: 6174 6567 6f72 7962 616c 616e 6365 7361  ategorybalancesa
-00002970: 6d70 6c65 7229 0a20 2066 6f72 6d73 2074  mpler).  forms t
-00002980: 6865 2062 6174 6368 6573 206c 696d 6974  he batches limit
-00002990: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
-000029a0: 6620 6361 7465 676f 7269 6573 202a 432a  f categories *C*
-000029b0: 2069 6e20 6974 2e0a 2020 466f 7220 696e   in it..  For in
-000029c0: 7374 616e 6365 2c20 7768 656e 202a 4320  stance, when *C 
-000029d0: 3d20 312a 2069 7420 7075 7473 206f 6e6c  = 1* it puts onl
-000029e0: 7920 6a61 636b 6574 7320 696e 206f 6e65  y jackets in one
-000029f0: 2062 6174 6368 2061 6e64 206f 6e6c 7920   batch and only 
-00002a00: 6a65 616e 7320 696e 746f 2061 6e6f 7468  jeans into anoth
-00002a10: 6572 206f 6e65 2028 6a75 7374 2061 6e20  er one (just an 
-00002a20: 6578 616d 706c 6529 2e0a 2020 4974 2061  example)..  It a
-00002a30: 7574 6f6d 6174 6963 616c 6c79 206d 616b  utomatically mak
-00002a40: 6573 2074 6865 206e 6567 6174 6976 6520  es the negative 
-00002a50: 7061 6972 7320 6861 7264 6572 3a20 6974  pairs harder: it
-00002a60: 2773 206d 6f72 6520 6d65 616e 696e 6766  's more meaningf
-00002a70: 756c 2066 6f72 2061 206d 6f64 656c 2074  ul for a model t
-00002a80: 6f20 7265 616c 6973 6520 7768 7920 7477  o realise why tw
-00002a90: 6f20 6a61 636b 6574 730a 2020 6172 6520  o jackets.  are 
-00002aa0: 6469 6666 6572 656e 7420 7468 616e 2074  different than t
-00002ab0: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00002ac0: 2073 616d 6520 6162 6f75 7420 6120 6a61   same about a ja
-00002ad0: 636b 6574 2061 6e64 2061 2074 2d73 6869  cket and a t-shi
-00002ae0: 7274 2e0a 0a2a 205b 4861 7264 2054 7269  rt...* [Hard Tri
-00002af0: 706c 6574 7320 4d69 6e65 725d 2868 7474  plets Miner](htt
-00002b00: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-00002b10: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-00002b20: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00002b30: 7374 2f63 6f6e 7465 6e74 732f 6d69 6e65  st/contents/mine
-00002b40: 7273 2e68 746d 6c23 6861 7264 7472 6970  rs.html#hardtrip
-00002b50: 6c65 7473 6d69 6e65 7229 0a20 206d 616b  letsminer).  mak
-00002b60: 6573 2074 6865 2074 6173 6b20 6576 656e  es the task even
-00002b70: 2068 6172 6465 7220 6b65 6570 696e 6720   harder keeping 
-00002b80: 6f6e 6c79 2074 6865 2068 6172 6465 7374  only the hardest
-00002b90: 2074 7269 706c 6574 7320 2877 6974 6820   triplets (with 
-00002ba0: 6d61 7869 6d61 6c20 706f 7369 7469 7665  maximal positive
-00002bb0: 2061 6e64 206d 696e 696d 616c 206e 6567   and minimal neg
-00002bc0: 6174 6976 6520 6469 7374 616e 6365 7329  ative distances)
-00002bd0: 2e0a 0a48 6572 6520 6172 6520 2a43 4d43  ...Here are *CMC
-00002be0: 4031 2a20 7363 6f72 6573 2066 6f72 2032  @1* scores for 2
-00002bf0: 2070 6f70 756c 6172 2062 656e 6368 6d61   popular benchma
-00002c00: 726b 732e 0a53 4f50 2064 6174 6173 6574  rks..SOP dataset
-00002c10: 3a20 4879 702d 5669 5420 e280 9420 3835  : Hyp-ViT ... 85
-00002c20: 2e39 2c20 6f75 7273 20e2 8094 2038 362e  .9, ours ... 86.
-00002c30: 362e 2044 6565 7046 6173 6869 6f6e 2064  6. DeepFashion d
-00002c40: 6174 6173 6574 3a20 4879 702d 5669 5420  ataset: Hyp-ViT 
-00002c50: e280 9420 3932 2e35 2c20 6f75 7273 20e2  ... 92.5, ours .
-00002c60: 8094 2039 322e 312e 0a54 6875 732c 2075  .. 92.1..Thus, u
-00002c70: 7469 6c69 7369 6e67 2073 696d 706c 6520  tilising simple 
-00002c80: 6865 7572 6973 7469 6373 2061 6e64 2061  heuristics and a
-00002c90: 766f 6964 696e 6720 6865 6176 7920 6d61  voiding heavy ma
-00002ca0: 7468 2077 6520 6172 6520 6162 6c65 2074  th we are able t
-00002cb0: 6f20 7065 7266 6f72 6d20 6f6e 2053 6f74  o perform on Sot
-00002cc0: 4120 6c65 7665 6c2e 0a0a 3c2f 703e 0a3c  A level...</p>.<
-00002cd0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-00002ce0: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-00002cf0: 6174 2061 626f 7574 2053 656c 662d 5375  at about Self-Su
-00002d00: 7065 7276 6973 6564 204c 6561 726e 696e  pervised Learnin
-00002d10: 673f 3c2f 7375 6d6d 6172 793e 0a3c 703e  g?</summary>.<p>
-00002d20: 0a0a 5265 6365 6e74 2072 6573 6561 7263  ..Recent researc
-00002d30: 6820 696e 2053 534c 2064 6566 696e 6974  h in SSL definit
-00002d40: 656c 7920 6f62 7461 696e 6564 2067 7265  ely obtained gre
-00002d50: 6174 2072 6573 756c 7473 2e20 5468 6520  at results. The 
-00002d60: 7072 6f62 6c65 6d20 6973 2074 6861 7420  problem is that 
-00002d70: 7468 6573 6520 6170 7072 6f61 6368 6573  these approaches
-00002d80: 0a72 6571 7569 7265 6420 616e 2065 6e6f  .required an eno
-00002d90: 726d 6f75 7320 616d 6f75 6e74 206f 6620  rmous amount of 
-00002da0: 636f 6d70 7574 696e 6720 746f 2074 7261  computing to tra
-00002db0: 696e 2074 6865 206d 6f64 656c 2e20 4275  in the model. Bu
-00002dc0: 7420 696e 206f 7572 2066 7261 6d65 776f  t in our framewo
-00002dd0: 726b 2c20 7765 2063 6f6e 7369 6465 7220  rk, we consider 
-00002de0: 7468 6520 6d6f 7374 2063 6f6d 6d6f 6e20  the most common 
-00002df0: 6361 7365 0a77 6865 6e20 7468 6520 6176  case.when the av
-00002e00: 6572 6167 6520 7573 6572 2068 6173 206e  erage user has n
-00002e10: 6f20 6d6f 7265 2074 6861 6e20 6120 6665  o more than a fe
-00002e20: 7720 4750 5573 2e0a 0a41 7420 7468 6520  w GPUs...At the 
-00002e30: 7361 6d65 2074 696d 652c 2069 7420 776f  same time, it wo
-00002e40: 756c 6420 6265 2075 6e77 6973 6520 746f  uld be unwise to
-00002e50: 2069 676e 6f72 6520 7375 6363 6573 7320   ignore success 
-00002e60: 696e 2074 6869 7320 7370 6865 7265 2c20  in this sphere, 
-00002e70: 736f 2077 6520 7374 696c 6c20 6578 706c  so we still expl
-00002e80: 6f69 7420 6974 2069 6e20 7477 6f20 7761  oit it in two wa
-00002e90: 7973 3a0a 2a20 4173 2061 2073 6f75 7263  ys:.* As a sourc
-00002ea0: 6520 6f66 2063 6865 636b 706f 696e 7473  e of checkpoints
-00002eb0: 2074 6861 7420 776f 756c 6420 6265 2067   that would be g
-00002ec0: 7265 6174 2074 6f20 7374 6172 7420 7472  reat to start tr
-00002ed0: 6169 6e69 6e67 2077 6974 682e 2046 726f  aining with. Fro
-00002ee0: 6d20 7075 626c 6963 6174 696f 6e73 2061  m publications a
-00002ef0: 6e64 206f 7572 2065 7870 6572 6965 6e63  nd our experienc
-00002f00: 652c 0a20 2074 6865 7920 6172 6520 6d75  e,.  they are mu
-00002f10: 6368 2062 6574 7465 7220 6173 2069 6e69  ch better as ini
-00002f20: 7469 616c 6973 6174 696f 6e20 7468 616e  tialisation than
-00002f30: 2074 6865 2064 6566 6175 6c74 2073 7570   the default sup
-00002f40: 6572 7669 7365 6420 6d6f 6465 6c20 7472  ervised model tr
-00002f50: 6169 6e65 6420 6f6e 2049 6d61 6765 4e65  ained on ImageNe
-00002f60: 742e 2054 6875 732c 2077 6520 6164 6465  t. Thus, we adde
-00002f70: 6420 7468 6520 706f 7373 6962 696c 6974  d the possibilit
-00002f80: 790a 2020 746f 2069 6e69 7469 616c 6973  y.  to initialis
-00002f90: 6520 796f 7572 206d 6f64 656c 7320 7573  e your models us
-00002fa0: 696e 6720 7468 6573 6520 7072 6574 7261  ing these pretra
-00002fb0: 696e 6564 2063 6865 636b 706f 696e 7473  ined checkpoints
-00002fc0: 206f 6e6c 7920 6279 2070 6173 7369 6e67   only by passing
-00002fd0: 2061 6e20 6172 6775 6d65 6e74 2069 6e20   an argument in 
-00002fe0: 7468 6520 636f 6e66 6967 206f 7220 7468  the config or th
-00002ff0: 6520 636f 6e73 7472 7563 746f 722e 0a2a  e constructor..*
-00003000: 2041 7320 6120 736f 7572 6365 206f 6620   As a source of 
-00003010: 696e 7370 6972 6174 696f 6e2e 2046 6f72  inspiration. For
-00003020: 2065 7861 6d70 6c65 2c20 7765 2061 6461   example, we ada
-00003030: 7074 6564 2074 6865 2069 6465 6120 6f66  pted the idea of
-00003040: 2061 206d 656d 6f72 7920 6261 6e6b 2066   a memory bank f
-00003050: 726f 6d20 2a4d 6f43 6f2a 2066 6f72 2074  rom *MoCo* for t
-00003060: 6865 202a 5472 6970 6c65 744c 6f73 732a  he *TripletLoss*
-00003070: 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461 696c  ...</p>.</detail
-00003080: 733e 0a0a 0a3c 6465 7461 696c 733e 0a3c  s>...<details>.<
-00003090: 7375 6d6d 6172 793e 446f 2049 206e 6565  summary>Do I nee
-000030a0: 6420 746f 206b 6e6f 7720 6f74 6865 7220  d to know other 
-000030b0: 6672 616d 6577 6f72 6b73 2074 6f20 7573  frameworks to us
-000030c0: 6520 4f4d 4c3f 3c2f 7375 6d6d 6172 793e  e OML?</summary>
-000030d0: 0a3c 703e 0a0a 4e6f 2c20 796f 7520 646f  .<p>..No, you do
-000030e0: 6e27 742e 204f 4d4c 2069 7320 6120 6672  n't. OML is a fr
-000030f0: 616d 6577 6f72 6b2d 6167 6e6f 7374 6963  amework-agnostic
-00003100: 2e20 4465 7370 6974 6520 7765 2075 7365  . Despite we use
-00003110: 2050 7954 6f72 6368 204c 6967 6874 6e69   PyTorch Lightni
-00003120: 6e67 2061 7320 6120 6c6f 6f70 0a72 756e  ng as a loop.run
-00003130: 6e65 7220 666f 7220 7468 6520 6578 7065  ner for the expe
-00003140: 7269 6d65 6e74 732c 2077 6520 616c 736f  riments, we also
-00003150: 206b 6565 7020 7468 6520 706f 7373 6962   keep the possib
-00003160: 696c 6974 7920 746f 2072 756e 2065 7665  ility to run eve
-00003170: 7279 7468 696e 6720 6f6e 2070 7572 6520  rything on pure 
-00003180: 5079 546f 7263 682e 0a54 6875 732c 206f  PyTorch..Thus, o
-00003190: 6e6c 7920 7468 6520 7469 6e79 2070 6172  nly the tiny par
-000031a0: 7420 6f66 204f 4d4c 2069 7320 4c69 6768  t of OML is Ligh
-000031b0: 746e 696e 672d 7370 6563 6966 6963 2061  tning-specific a
-000031c0: 6e64 2077 6520 6b65 6570 2074 6869 7320  nd we keep this 
-000031d0: 6c6f 6769 6320 7365 7061 7261 7465 6c79  logic separately
-000031e0: 2066 726f 6d0a 6f74 6865 7220 636f 6465   from.other code
-000031f0: 2028 7365 6520 606f 6d6c 2e6c 6967 6874   (see `oml.light
-00003200: 6e69 6e67 6029 2e20 4576 656e 2077 6865  ning`). Even whe
-00003210: 6e20 796f 7520 7573 6520 4c69 6768 746e  n you use Lightn
-00003220: 696e 672c 2079 6f75 2064 6f6e 2774 206e  ing, you don't n
-00003230: 6565 6420 746f 206b 6e6f 7720 6974 2c20  eed to know it, 
-00003240: 7369 6e63 650a 7765 2070 726f 7669 6465  since.we provide
-00003250: 2072 6561 6479 2074 6f20 7573 6520 5b50   ready to use [P
-00003260: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
-00003270: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00003280: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00003290: 632d 6c65 6172 6e69 6e67 2f62 6c6f 622f  c-learning/blob/
-000032a0: 6d61 696e 2f70 6970 656c 696e 6573 2f29  main/pipelines/)
-000032b0: 2e0a 0a54 6865 2070 6f73 7369 6269 6c69  ...The possibili
-000032c0: 7479 206f 6620 7573 696e 6720 7075 7265  ty of using pure
-000032d0: 2050 7954 6f72 6368 2061 6e64 206d 6f64   PyTorch and mod
-000032e0: 756c 6172 2073 7472 7563 7475 7265 206f  ular structure o
-000032f0: 6620 7468 6520 636f 6465 206c 6561 7665  f the code leave
-00003300: 7320 6120 726f 6f6d 2066 6f72 2075 7469  s a room for uti
-00003310: 6c69 7a69 6e67 0a4f 4d4c 2077 6974 6820  lizing.OML with 
-00003320: 796f 7572 2066 6176 6f75 7269 7465 2066  your favourite f
-00003330: 7261 6d65 776f 726b 2061 6674 6572 2074  ramework after t
-00003340: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
-00003350: 6e20 6f66 2074 6865 206e 6563 6573 7361  n of the necessa
-00003360: 7279 2077 7261 7070 6572 732e 0a0a 3c2f  ry wrappers...</
-00003370: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
-00003380: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
-00003390: 7279 3e43 616e 2049 2075 7365 204f 4d4c  ry>Can I use OML
-000033a0: 2077 6974 686f 7574 2061 6e79 206b 6e6f   without any kno
-000033b0: 776c 6564 6765 2069 6e20 4461 7461 5363  wledge in DataSc
-000033c0: 6965 6e63 653f 3c2f 7375 6d6d 6172 793e  ience?</summary>
-000033d0: 0a3c 703e 0a0a 5965 732e 2054 6f20 7275  .<p>..Yes. To ru
-000033e0: 6e20 7468 6520 6578 7065 7269 6d65 6e74  n the experiment
-000033f0: 2077 6974 6820 5b50 6970 656c 696e 6573   with [Pipelines
-00003400: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003410: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00003420: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00003430: 6e67 2f62 6c6f 622f 6d61 696e 2f70 6970  ng/blob/main/pip
-00003440: 656c 696e 6573 2f29 0a79 6f75 206f 6e6c  elines/).you onl
-00003450: 7920 6e65 6564 2074 6f20 7772 6974 6520  y need to write 
-00003460: 6120 636f 6e76 6572 7465 720a 746f 206f  a converter.to o
-00003470: 7572 2066 6f72 6d61 7420 2869 7420 6d65  ur format (it me
-00003480: 616e 7320 7072 6570 6172 696e 6720 7468  ans preparing th
-00003490: 650a 602e 6373 7660 2074 6162 6c65 2077  e.`.csv` table w
-000034a0: 6974 6820 3520 7072 6564 6566 696e 6564  ith 5 predefined
-000034b0: 2063 6f6c 756d 6e73 292e 0a54 6861 7427   columns)..That'
-000034c0: 7320 6974 210a 0a50 726f 6261 626c 7920  s it!..Probably 
-000034d0: 7765 2061 6c72 6561 6479 2068 6176 6520  we already have 
-000034e0: 6120 7375 6974 6162 6c65 2070 7265 2d74  a suitable pre-t
-000034f0: 7261 696e 6564 206d 6f64 656c 2066 6f72  rained model for
-00003500: 2079 6f75 7220 646f 6d61 696e 0a69 6e20   your domain.in 
-00003510: 6f75 7220 2a4d 6f64 656c 7320 5a6f 6f2a  our *Models Zoo*
-00003520: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
-00003530: 796f 7520 646f 6e27 7420 6576 656e 206e  you don't even n
-00003540: 6565 6420 746f 2074 7261 696e 2069 742e  eed to train it.
-00003550: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-00003560: 0a0a 2323 205b 446f 6375 6d65 6e74 6174  ..## [Documentat
-00003570: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
-00003580: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-00003590: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
-000035a0: 2f65 6e2f 6c61 7465 7374 2f69 6e64 6578  /en/latest/index
-000035b0: 2e68 746d 6c29 0a0a 446f 6375 6d65 6e74  .html)..Document
-000035c0: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-000035d0: 6c65 2076 6961 2074 6865 205b 6c69 6e6b  le via the [link
-000035e0: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-000035f0: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00003600: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00003610: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
-00003620: 6d6c 292e 0a0a 596f 7520 6361 6e20 616c  ml)...You can al
-00003630: 736f 2072 6561 6420 736f 6d65 2065 7874  so read some ext
-00003640: 7261 206d 6174 6572 6961 6c73 2072 656c  ra materials rel
-00003650: 6174 6564 2074 6f20 4f4d 4c3a 0a0a 2a20  ated to OML:..* 
-00003660: 5468 656f 7279 2061 6e64 2070 7261 6374  Theory and pract
-00003670: 6963 6520 6f66 206d 6574 7269 6320 6c65  ice of metric le
-00003680: 6172 6e69 6e67 2077 6974 6820 7468 6520  arning with the 
-00003690: 7573 6167 6520 6f66 204f 4d4c 2e0a 5b50  usage of OML..[P
-000036a0: 6f73 7420 696e 2045 6e67 6c69 7368 206f  ost in English o
-000036b0: 6e20 4d65 6469 756d 5d28 6874 7470 733a  n Medium](https:
-000036c0: 2f2f 6d65 6469 756d 2e63 6f6d 2f40 416c  //medium.com/@Al
-000036d0: 656b 7365 6953 6861 6261 6e6f 762f 7072  ekseiShabanov/pr
-000036e0: 6163 7469 6361 6c2d 6d65 7472 6963 2d6c  actical-metric-l
-000036f0: 6561 726e 696e 672d 6230 3431 3063 6461  earning-b0410cda
-00003700: 3232 3031 2920 7c0a 5b50 6f73 7420 696e  2201) |.[Post in
-00003710: 2052 7573 7369 616e 206f 6e20 4861 6272   Russian on Habr
-00003720: 5d28 6874 7470 733a 2f2f 6861 6272 2e63  ](https://habr.c
-00003730: 6f6d 2f72 752f 636f 6d70 616e 792f 6f64  om/ru/company/od
-00003740: 732f 626c 6f67 2f36 3935 3338 302f 2920  s/blog/695380/) 
-00003750: 7c0a 5b50 6f73 7420 696e 2043 6869 6e65  |.[Post in Chine
-00003760: 7365 206f 6e20 4353 444e 5d28 6874 7470  se on CSDN](http
-00003770: 733a 2f2f 626c 6f67 2e63 7364 6e2e 6e65  s://blog.csdn.ne
-00003780: 742f 6665 726d 696f 6e30 3231 372f 6172  t/fermion0217/ar
-00003790: 7469 636c 652f 6465 7461 696c 732f 3132  ticle/details/12
-000037a0: 3739 3332 3038 3729 2c20 7472 616e 736c  7932087), transl
-000037b0: 6174 6564 2062 7920 4368 6961 2d43 6865  ated by Chia-Che
-000037c0: 6e20 4368 616e 672e 0a0a 2a20 5468 650a  n Chang...* The.
-000037d0: 5b44 454d 4f5d 2868 7474 7073 3a2f 2f64  [DEMO](https://d
-000037e0: 6170 6c61 646f 632d 6f6d 6c2d 706f 7374  apladoc-oml-post
-000037f0: 7072 6f63 6573 7369 6e67 2d64 656d 6f2d  processing-demo-
-00003800: 7372 6361 7070 6d61 696e 2d70 6668 3267  srcappmain-pfh2g
-00003810: 302e 7374 7265 616d 6c69 742e 6170 702f  0.streamlit.app/
-00003820: 290a 666f 7220 6f75 7220 7061 7065 720a  ).for our paper.
-00003830: 5b53 5449 523a 2053 6961 6d65 7365 2054  [STIR: Siamese T
-00003840: 7261 6e73 666f 726d 6572 7320 666f 7220  ransformers for 
-00003850: 496d 6167 6520 5265 7472 6965 7661 6c20  Image Retrieval 
-00003860: 506f 7374 7072 6f63 6573 7369 6e67 5d28  Postprocessing](
-00003870: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00003880: 672f 6162 732f 3233 3034 2e31 3333 3933  g/abs/2304.13393
-00003890: 290a 0a2a 2054 6865 2072 6570 6f72 7420  )..* The report 
-000038a0: 666f 7220 4265 726c 696e 2d62 6173 6564  for Berlin-based
-000038b0: 206d 6565 7475 703a 2022 436f 6d70 7574   meetup: "Comput
-000038c0: 6572 2056 6973 696f 6e20 696e 2070 726f  er Vision in pro
-000038d0: 6475 6374 696f 6e22 2e20 4e6f 7665 6d62  duction". Novemb
-000038e0: 6572 2c20 3230 3232 2e0a 5b4c 696e 6b5d  er, 2022..[Link]
-000038f0: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00003900: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00003910: 666f 6c64 6572 732f 3175 486d 4c55 3876  folders/1uHmLU8v
-00003920: 4d72 4d56 4d46 6f64 7433 3675 3075 5841  MrMVMFodt36u0uXA
-00003930: 6759 6a47 5f33 4433 303f 7573 703d 7368  gYjG_3D30?usp=sh
-00003940: 6172 655f 6c69 6e6b 290a 0a23 2320 5b49  are_link)..## [I
-00003950: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
-00003960: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-00003970: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-00003980: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003990: 7374 2f6f 6d6c 2f69 6e73 7461 6c6c 6174  st/oml/installat
-000039a0: 696f 6e2e 6874 6d6c 290a 0a4f 4d4c 2069  ion.html)..OML i
-000039b0: 7320 6176 6169 6c61 626c 6520 696e 2050  s available in P
-000039c0: 7950 493a 0a0a 6060 6073 6865 6c6c 0a70  yPI:..```shell.p
-000039d0: 6970 2069 6e73 7461 6c6c 202d 5520 6f70  ip install -U op
-000039e0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000039f0: 6e67 0a60 6060 0a0a 596f 7520 6361 6e20  ng.```..You can 
-00003a00: 616c 736f 2070 756c 6c20 7468 6520 7072  also pull the pr
-00003a10: 6570 6172 6564 2069 6d61 6765 2066 726f  epared image fro
-00003a20: 6d20 446f 636b 6572 4875 622e 2e2e 0a0a  m DockerHub.....
-00003a30: 6060 6073 6865 6c6c 0a64 6f63 6b65 7220  ```shell.docker 
-00003a40: 7075 6c6c 206f 6d6c 7465 616d 2f6f 6d6c  pull omlteam/oml
-00003a50: 3a67 7075 0a64 6f63 6b65 7220 7075 6c6c  :gpu.docker pull
-00003a60: 206f 6d6c 7465 616d 2f6f 6d6c 3a63 7075   omlteam/oml:cpu
-00003a70: 0a60 6060 0a0a 2e2e 2e6f 7220 6275 696c  .```.....or buil
-00003a80: 6420 6f6e 6520 6279 2079 6f75 7220 6f77  d one by your ow
-00003a90: 6e0a 0a60 6060 7368 656c 6c0a 6d61 6b65  n..```shell.make
-00003aa0: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
-00003ab0: 4e54 494d 453d 6370 750a 6d61 6b65 2064  NTIME=cpu.make d
-00003ac0: 6f63 6b65 725f 6275 696c 6420 5255 4e54  ocker_build RUNT
-00003ad0: 494d 453d 6770 750a 6060 600a 0a23 2320  IME=gpu.```..## 
-00003ae0: 5b45 7861 6d70 6c65 735d 2868 7474 7073  [Examples](https
-00003af0: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
-00003b00: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
-00003b10: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003b20: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
-00003b30: 696f 6e2f 7079 7468 6f6e 5f65 7861 6d70  ion/python_examp
-00003b40: 6c65 732e 6874 6d6c 2329 0a0a 3c64 6574  les.html#)..<det
-00003b50: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e54  ails>.<summary>T
-00003b60: 7261 696e 696e 673c 2f73 756d 6d61 7279  raining</summary
-00003b70: 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e 745d  >.<p>..[comment]
-00003b80: 3a76 616e 696c 6c61 2d74 7261 696e 2d73  :vanilla-train-s
-00003b90: 7461 7274 0a60 6060 7079 7468 6f6e 0a69  tart.```python.i
-00003ba0: 6d70 6f72 7420 746f 7263 680a 6672 6f6d  mport torch.from
-00003bb0: 2074 7164 6d20 696d 706f 7274 2074 7164   tqdm import tqd
-00003bc0: 6d0a 0a66 726f 6d20 6f6d 6c2e 6461 7461  m..from oml.data
-00003bd0: 7365 7473 2e62 6173 6520 696d 706f 7274  sets.base import
-00003be0: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
-00003bf0: 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ls.from oml.loss
-00003c00: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
-00003c10: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
-00003c20: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
-00003c30: 6d69 6e65 7273 2e69 6e62 6174 6368 5f61  miners.inbatch_a
-00003c40: 6c6c 5f74 7269 2069 6d70 6f72 7420 416c  ll_tri import Al
-00003c50: 6c54 7269 706c 6574 734d 696e 6572 0a66  lTripletsMiner.f
-00003c60: 726f 6d20 6f6d 6c2e 6d6f 6465 6c73 2069  rom oml.models i
-00003c70: 6d70 6f72 7420 5669 5445 7874 7261 6374  mport ViTExtract
-00003c80: 6f72 0a66 726f 6d20 6f6d 6c2e 7361 6d70  or.from oml.samp
-00003c90: 6c65 7273 2e62 616c 616e 6365 2069 6d70  lers.balance imp
-00003ca0: 6f72 7420 4261 6c61 6e63 6553 616d 706c  ort BalanceSampl
-00003cb0: 6572 0a66 726f 6d20 6f6d 6c2e 7574 696c  er.from oml.util
-00003cc0: 732e 646f 776e 6c6f 6164 5f6d 6f63 6b5f  s.download_mock_
-00003cd0: 6461 7461 7365 7420 696d 706f 7274 2064  dataset import d
-00003ce0: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
-00003cf0: 6173 6574 0a0a 6461 7461 7365 745f 726f  aset..dataset_ro
-00003d00: 6f74 203d 2022 6d6f 636b 5f64 6174 6173  ot = "mock_datas
-00003d10: 6574 2f22 0a64 665f 7472 6169 6e2c 205f  et/".df_train, _
-00003d20: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-00003d30: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-00003d40: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-00003d50: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-00003d60: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-00003d70: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-00003d80: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00003d90: 733d 4661 6c73 6529 2e74 7261 696e 2829  s=False).train()
-00003da0: 0a6f 7074 696d 697a 6572 203d 2074 6f72  .optimizer = tor
-00003db0: 6368 2e6f 7074 696d 2e53 4744 2865 7874  ch.optim.SGD(ext
-00003dc0: 7261 6374 6f72 2e70 6172 616d 6574 6572  ractor.parameter
-00003dd0: 7328 292c 206c 723d 3165 2d36 290a 0a74  s(), lr=1e-6)..t
-00003de0: 7261 696e 5f64 6174 6173 6574 203d 2044  rain_dataset = D
-00003df0: 6174 6173 6574 5769 7468 4c61 6265 6c73  atasetWithLabels
-00003e00: 2864 665f 7472 6169 6e2c 2064 6174 6173  (df_train, datas
-00003e10: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00003e20: 726f 6f74 290a 6372 6974 6572 696f 6e20  root).criterion 
-00003e30: 3d20 5472 6970 6c65 744c 6f73 7357 6974  = TripletLossWit
-00003e40: 684d 696e 6572 286d 6172 6769 6e3d 302e  hMiner(margin=0.
-00003e50: 312c 206d 696e 6572 3d41 6c6c 5472 6970  1, miner=AllTrip
-00003e60: 6c65 7473 4d69 6e65 7228 292c 206e 6565  letsMiner(), nee
-00003e70: 645f 6c6f 6773 3d54 7275 6529 0a73 616d  d_logs=True).sam
-00003e80: 706c 6572 203d 2042 616c 616e 6365 5361  pler = BalanceSa
-00003e90: 6d70 6c65 7228 7472 6169 6e5f 6461 7461  mpler(train_data
-00003ea0: 7365 742e 6765 745f 6c61 6265 6c73 2829  set.get_labels()
-00003eb0: 2c20 6e5f 6c61 6265 6c73 3d32 2c20 6e5f  , n_labels=2, n_
-00003ec0: 696e 7374 616e 6365 733d 3229 0a74 7261  instances=2).tra
-00003ed0: 696e 5f6c 6f61 6465 7220 3d20 746f 7263  in_loader = torc
-00003ee0: 682e 7574 696c 732e 6461 7461 2e44 6174  h.utils.data.Dat
-00003ef0: 614c 6f61 6465 7228 7472 6169 6e5f 6461  aLoader(train_da
-00003f00: 7461 7365 742c 2062 6174 6368 5f73 616d  taset, batch_sam
-00003f10: 706c 6572 3d73 616d 706c 6572 290a 0a66  pler=sampler)..f
-00003f20: 6f72 2062 6174 6368 2069 6e20 7471 646d  or batch in tqdm
-00003f30: 2874 7261 696e 5f6c 6f61 6465 7229 3a0a  (train_loader):.
-00003f40: 2020 2020 656d 6265 6464 696e 6773 203d      embeddings =
-00003f50: 2065 7874 7261 6374 6f72 2862 6174 6368   extractor(batch
-00003f60: 5b22 696e 7075 745f 7465 6e73 6f72 7322  ["input_tensors"
-00003f70: 5d29 0a20 2020 206c 6f73 7320 3d20 6372  ]).    loss = cr
-00003f80: 6974 6572 696f 6e28 656d 6265 6464 696e  iterion(embeddin
-00003f90: 6773 2c20 6261 7463 685b 226c 6162 656c  gs, batch["label
-00003fa0: 7322 5d29 0a20 2020 206c 6f73 732e 6261  s"]).    loss.ba
-00003fb0: 636b 7761 7264 2829 0a20 2020 206f 7074  ckward().    opt
-00003fc0: 696d 697a 6572 2e73 7465 7028 290a 2020  imizer.step().  
-00003fd0: 2020 6f70 7469 6d69 7a65 722e 7a65 726f    optimizer.zero
-00003fe0: 5f67 7261 6428 290a 0a20 2020 2023 2069  _grad()..    # i
-00003ff0: 6e66 6f20 666f 7220 6c6f 6767 696e 673a  nfo for logging:
-00004000: 2070 6f73 6974 6976 652f 6e65 6761 7469   positive/negati
-00004010: 7665 2064 6973 7461 6e63 6573 2c20 6e75  ve distances, nu
-00004020: 6d62 6572 206f 6620 6163 7469 7665 2074  mber of active t
-00004030: 7269 706c 6574 730a 2020 2020 7072 696e  riplets.    prin
-00004040: 7428 6372 6974 6572 696f 6e2e 6c61 7374  t(criterion.last
-00004050: 5f6c 6f67 7329 0a0a 6060 600a 5b63 6f6d  _logs)..```.[com
-00004060: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7472  ment]:vanilla-tr
-00004070: 6169 6e2d 656e 640a 3c2f 703e 0a3c 2f64  ain-end.</p>.</d
-00004080: 6574 6169 6c73 3e0a 0a5b 215b 4f70 656e  etails>..[![Open
-00004090: 2049 6e20 436f 6c61 625d 2868 7474 7073   In Colab](https
-000040a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-000040b0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-000040c0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-000040d0: 7376 6729 5d28 6874 7470 733a 2f2f 636f  svg)](https://co
-000040e0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-000040f0: 676c 652e 636f 6d2f 6472 6976 652f 316b  gle.com/drive/1k
-00004100: 6e74 4441 4964 495a 394c 3430 6a63 6e64  ntDAIdIZ9L40jcnd
-00004110: 6775 4c41 622d 5871 6d43 464f 6753 353f  guLAb-XqmCFOgS5?
-00004120: 7573 703d 7368 6172 696e 6729 0a3c 6465  usp=sharing).<de
-00004130: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
-00004140: 5661 6c69 6461 7469 6f6e 3c2f 7375 6d6d  Validation</summ
-00004150: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-00004160: 6e74 5d3a 7661 6e69 6c6c 612d 7661 6c69  nt]:vanilla-vali
-00004170: 6461 7469 6f6e 2d73 7461 7274 0a60 6060  dation-start.```
-00004180: 7079 7468 6f6e 0a69 6d70 6f72 7420 746f  python.import to
-00004190: 7263 680a 6672 6f6d 2074 7164 6d20 696d  rch.from tqdm im
-000041a0: 706f 7274 2074 7164 6d0a 0a66 726f 6d20  port tqdm..from 
-000041b0: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-000041c0: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-000041d0: 5175 6572 7947 616c 6c65 7279 0a66 726f  QueryGallery.fro
-000041e0: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-000041f0: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00004200: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
+00000b90: 6164 6765 2e73 7667 3f29 0a0a 4f4d 4c20  adge.svg?)..OML 
+00000ba0: 6973 2061 2050 7954 6f72 6368 2d62 6173  is a PyTorch-bas
+00000bb0: 6564 2066 7261 6d65 776f 726b 2074 6f20  ed framework to 
+00000bc0: 7472 6169 6e20 616e 6420 7661 6c69 6461  train and valida
+00000bd0: 7465 2074 6865 206d 6f64 656c 7320 7072  te the models pr
+00000be0: 6f64 7563 696e 6720 6869 6768 2d71 7561  oducing high-qua
+00000bf0: 6c69 7479 2065 6d62 6564 6469 6e67 732e  lity embeddings.
+00000c00: 0a0a 2323 2320 5472 7573 7465 6420 6279  ..### Trusted by
+00000c10: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000c20: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000c30: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+00000c40: 7475 6e65 2e61 692f 696e 7465 6772 6174  tune.ai/integrat
+00000c50: 696f 6e73 2f63 6f6d 6d75 6e69 7479 5f64  ions/community_d
+00000c60: 6576 656c 6f70 6564 2f22 2074 6172 6765  eveloped/" targe
+00000c70: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00000c80: 7372 633d 2268 7474 7073 3a2f 2f73 6563  src="https://sec
+00000c90: 7572 6974 792e 6e65 7074 756e 652e 6169  urity.neptune.ai
+00000ca0: 2f61 7069 2f73 6861 7265 2f62 3730 3766  /api/share/b707f
+00000cb0: 3165 382d 6532 3837 2d34 6630 312d 6235  1e8-e287-4f01-b5
+00000cc0: 3930 2d33 3961 3666 6137 6539 6661 612f  90-39a6fa7e9faa/
+00000cd0: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
+00000ce0: 2231 3030 222f 3e3c 2f61 3ee3 85a4 e385  "100"/></a>.....
+00000cf0: a40a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000d00: 3a2f 2f77 7777 2e6e 6577 796f 726b 6572  ://www.newyorker
+00000d10: 2e64 652f 2220 7461 7267 6574 3d22 5f62  .de/" target="_b
+00000d20: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+00000d30: 6874 7470 733a 2f2f 7570 6c6f 6164 2e77  https://upload.w
+00000d40: 696b 696d 6564 6961 2e6f 7267 2f77 696b  ikimedia.org/wik
+00000d50: 6970 6564 6961 2f63 6f6d 6d6f 6e73 2f74  ipedia/commons/t
+00000d60: 6875 6d62 2f64 2f64 382f 4e65 775f 596f  humb/d/d8/New_Yo
+00000d70: 726b 6572 2e73 7667 2f31 3238 3070 782d  rker.svg/1280px-
+00000d80: 4e65 775f 596f 726b 6572 2e73 7667 2e70  New_Yorker.svg.p
+00000d90: 6e67 2220 7769 6474 683d 2231 3030 222f  ng" width="100"/
+00000da0: 3e3c 2f61 3ee3 85a4 e385 a40a 3c61 2068  ></a>.......<a h
+00000db0: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000dc0: 2e65 706f 6368 382e 636f 2f22 2074 6172  .epoch8.co/" tar
+00000dd0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+00000de0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000df0: 2e69 6262 2e63 6f2f 4764 4e56 5479 742f  .ibb.co/GdNVTyt/
+00000e00: 5363 7265 656e 7368 6f74 2d32 3032 332d  Screenshot-2023-
+00000e10: 3037 2d30 342d 6174 2d31 312d 3139 2d32  07-04-at-11-19-2
+00000e20: 342e 706e 6722 2077 6964 7468 3d22 3130  4.png" width="10
+00000e30: 3022 2f3e 3c2f 613e e385 a4e3 85a4 0a3c  0"/></a>.......<
+00000e40: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000e50: 7777 772e 6d65 6974 7561 6e2e 636f 6d22  www.meituan.com"
+00000e60: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000e70: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000e80: 3a2f 2f75 706c 6f61 642e 7769 6b69 6d65  ://upload.wikime
+00000e90: 6469 612e 6f72 672f 7769 6b69 7065 6469  dia.org/wikipedi
+00000ea0: 612f 636f 6d6d 6f6e 732f 362f 3631 2f4d  a/commons/6/61/M
+00000eb0: 6569 7475 616e 5f45 6e67 6c69 7368 5f4c  eituan_English_L
+00000ec0: 6f67 6f2e 706e 6722 2077 6964 7468 3d22  ogo.png" width="
+00000ed0: 3130 3022 2f3e 3c2f 613e 0a0a 3c61 2068  100"/></a>..<a h
+00000ee0: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000ef0: 2e6f 782e 6163 2e75 6b2f 2220 7461 7267  .ox.ac.uk/" targ
+00000f00: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00000f10: 2073 7263 3d22 6874 7470 733a 2f2f 7570   src="https://up
+00000f20: 6c6f 6164 2e77 696b 696d 6564 6961 2e6f  load.wikimedia.o
+00000f30: 7267 2f77 696b 6970 6564 6961 2f65 6e2f  rg/wikipedia/en/
+00000f40: 7468 756d 622f 322f 3266 2f55 6e69 7665  thumb/2/2f/Unive
+00000f50: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+00000f60: 7376 672f 3235 3630 7078 2d55 6e69 7665  svg/2560px-Unive
+00000f70: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+00000f80: 7376 672e 706e 6722 2077 6964 7468 3d22  svg.png" width="
+00000f90: 3132 3022 2f3e 3c2f 613e e385 a4e3 85a4  120"/></a>......
+00000fa0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000fb0: 2f2f 7777 772e 6873 652e 7275 2f65 6e2f  //www.hse.ru/en/
+00000fc0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000fd0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000fe0: 733a 2f2f 7777 772e 6873 652e 7275 2f64  s://www.hse.ru/d
+00000ff0: 6174 612f 3230 3230 2f31 312f 3136 2f31  ata/2020/11/16/1
+00001000: 3336 3732 3734 3034 342f 4853 455f 556e  367274044/HSE_Un
+00001010: 6976 6572 7369 7479 5f62 6c75 652e 6a70  iversity_blue.jp
+00001020: 672e 2832 3330 7838 3678 3132 3329 2e6a  g.(230x86x123).j
+00001030: 7067 2220 7769 6474 683d 2231 3030 222f  pg" width="100"/
+00001040: 3e3c 2f61 3e0a 0a54 6865 7265 2069 7320  ></a>..There is 
+00001050: 6120 6e75 6d62 6572 206f 6620 7065 6f70  a number of peop
+00001060: 6c65 2066 726f 6d0a 5b4f 7866 6f72 645d  le from.[Oxford]
+00001070: 2868 7474 7073 3a2f 2f77 7777 2e6f 782e  (https://www.ox.
+00001080: 6163 2e75 6b2f 2920 616e 640a 5b48 5345  ac.uk/) and.[HSE
+00001090: 5d28 6874 7470 733a 2f2f 7777 772e 6873  ](https://www.hs
+000010a0: 652e 7275 2f65 6e2f 290a 756e 6976 6572  e.ru/en/).univer
+000010b0: 7369 7469 6573 2077 686f 2068 6176 6520  sities who have 
+000010c0: 7573 6564 204f 4d4c 2069 6e20 7468 6569  used OML in thei
+000010d0: 7220 7468 6573 6573 2e0a 5b5b 315d 5d28  r theses..[[1]](
+000010e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000010f0: 6f6d 2f6e 696c 6f6d 722f 6f70 656e 2d6d  om/nilomr/open-m
+00001100: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+00001110: 7265 652f 6772 6561 742d 7469 742f 6772  ree/great-tit/gr
+00001120: 6561 742d 7469 742d 7472 6169 6e29 0a5b  eat-tit-train).[
+00001130: 5b32 5d5d 2868 7474 7073 3a2f 2f67 6974  [2]](https://git
+00001140: 6875 622e 636f 6d2f 6e61 7374 7967 6f72  hub.com/nastygor
+00001150: 6f64 692f 5052 4f4a 4543 542d 4465 6570  odi/PROJECT-Deep
+00001160: 5f4d 6574 7269 635f 4c65 6172 6e69 6e67  _Metric_Learning
+00001170: 290a 5b5b 335d 5d28 6874 7470 733a 2f2f  ).[[3]](https://
+00001180: 6769 7468 7562 2e63 6f6d 2f6e 696b 2d66  github.com/nik-f
+00001190: 6564 6f72 6f76 2f74 6572 6d5f 7061 7065  edorov/term_pape
+000011a0: 725f 6d65 7472 6963 5f6c 6561 726e 696e  r_metric_learnin
+000011b0: 6729 0a0a 3c64 6976 2061 6c69 676e 3d22  g)..<div align="
+000011c0: 6c65 6674 223e 0a0a 2323 205b 4641 515d  left">..## [FAQ]
+000011d0: 2868 7474 7073 3a2f 2f6f 7065 6e2d 6d65  (https://open-me
+000011e0: 7472 6963 2d6c 6561 726e 696e 672e 7265  tric-learning.re
+000011f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001200: 6c61 7465 7374 2f6f 6d6c 2f66 6171 2e68  latest/oml/faq.h
+00001210: 746d 6c29 0a0a 3c64 6574 6169 6c73 3e0a  tml)..<details>.
+00001220: 3c73 756d 6d61 7279 3e57 6879 2064 6f20  <summary>Why do 
+00001230: 4920 6e65 6564 204f 4d4c 3f3c 2f73 756d  I need OML?</sum
+00001240: 6d61 7279 3e0a 3c70 3e0a 0a59 6f75 206d  mary>.<p>..You m
+00001250: 6179 2074 6869 6e6b 202a 2249 6620 4920  ay think *"If I 
+00001260: 6e65 6564 2069 6d61 6765 2065 6d62 6564  need image embed
+00001270: 6469 6e67 7320 4920 6361 6e20 7369 6d70  dings I can simp
+00001280: 6c79 2074 7261 696e 2061 2076 616e 696c  ly train a vanil
+00001290: 6c61 2063 6c61 7373 6966 6965 7220 616e  la classifier an
+000012a0: 6420 7461 6b65 2069 7473 2070 656e 756c  d take its penul
+000012b0: 7469 6d61 7465 206c 6179 6572 222a 2e0a  timate layer"*..
+000012c0: 5765 6c6c 2c20 6974 206d 616b 6573 2073  Well, it makes s
+000012d0: 656e 7365 2061 7320 6120 7374 6172 7469  ense as a starti
+000012e0: 6e67 2070 6f69 6e74 2e20 4275 7420 7468  ng point. But th
+000012f0: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
+00001300: 706f 7373 6962 6c65 2064 7261 7762 6163  possible drawbac
+00001310: 6b73 3a0a 0a2a 2049 6620 796f 7520 7761  ks:..* If you wa
+00001320: 6e74 2074 6f20 7573 6520 656d 6265 6464  nt to use embedd
+00001330: 696e 6773 2074 6f20 7065 7266 6f72 6d20  ings to perform 
+00001340: 7365 6172 6368 696e 6720 796f 7520 6e65  searching you ne
+00001350: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+00001360: 736f 6d65 2064 6973 7461 6e63 6520 616d  some distance am
+00001370: 6f6e 6720 7468 656d 2028 666f 7220 6578  ong them (for ex
+00001380: 616d 706c 652c 2063 6f73 696e 6520 6f72  ample, cosine or
+00001390: 204c 3229 2e0a 2020 5573 7561 6c6c 792c   L2)..  Usually,
+000013a0: 202a 2a79 6f75 2064 6f6e 2774 2064 6972   **you don't dir
+000013b0: 6563 746c 7920 6f70 7469 6d69 7a65 2074  ectly optimize t
+000013c0: 6865 7365 2064 6973 7461 6e63 6573 2064  hese distances d
+000013d0: 7572 696e 6720 7468 6520 7472 6169 6e69  uring the traini
+000013e0: 6e67 2a2a 2069 6e20 7468 6520 636c 6173  ng** in the clas
+000013f0: 7369 6669 6361 7469 6f6e 2073 6574 7570  sification setup
+00001400: 2e20 536f 2c20 796f 7520 6361 6e20 6f6e  . So, you can on
+00001410: 6c79 2068 6f70 6520 7468 6174 0a20 2066  ly hope that.  f
+00001420: 696e 616c 2065 6d62 6564 6469 6e67 7320  inal embeddings 
+00001430: 7769 6c6c 2068 6176 6520 7468 6520 6465  will have the de
+00001440: 7369 7265 6420 7072 6f70 6572 7469 6573  sired properties
+00001450: 2e0a 0a2a 202a 2a54 6865 2073 6563 6f6e  ...* **The secon
+00001460: 6420 7072 6f62 6c65 6d20 6973 2074 6865  d problem is the
+00001470: 2076 616c 6964 6174 696f 6e20 7072 6f63   validation proc
+00001480: 6573 732a 2a2e 0a20 2049 6e20 7468 6520  ess**..  In the 
+00001490: 7365 6172 6368 696e 6720 7365 7475 702c  searching setup,
+000014a0: 2079 6f75 2075 7375 616c 6c79 2063 6172   you usually car
+000014b0: 6520 686f 7720 7265 6c61 7465 6420 796f  e how related yo
+000014c0: 7572 2074 6f70 2d4e 206f 7574 7075 7473  ur top-N outputs
+000014d0: 2061 7265 2074 6f20 7468 6520 7175 6572   are to the quer
+000014e0: 792e 0a20 2054 6865 206e 6174 7572 616c  y..  The natural
+000014f0: 2077 6179 2074 6f20 6576 616c 7561 7465   way to evaluate
+00001500: 2074 6865 206d 6f64 656c 2069 7320 746f   the model is to
+00001510: 2073 696d 756c 6174 6520 7365 6172 6368   simulate search
+00001520: 696e 6720 7265 7175 6573 7473 2074 6f20  ing requests to 
+00001530: 7468 6520 7265 6665 7265 6e63 6520 7365  the reference se
+00001540: 740a 2020 616e 6420 6170 706c 7920 6f6e  t.  and apply on
+00001550: 6520 6f66 2074 6865 2072 6574 7269 6576  e of the retriev
+00001560: 616c 206d 6574 7269 6373 2e0a 2020 536f  al metrics..  So
+00001570: 2c20 7468 6572 6520 6973 206e 6f20 6775  , there is no gu
+00001580: 6172 616e 7465 6520 7468 6174 2063 6c61  arantee that cla
+00001590: 7373 6966 6963 6174 696f 6e20 6163 6375  ssification accu
+000015a0: 7261 6379 2077 696c 6c20 636f 7272 656c  racy will correl
+000015b0: 6174 6520 7769 7468 2074 6865 7365 206d  ate with these m
+000015c0: 6574 7269 6373 2e0a 0a2a 2046 696e 616c  etrics...* Final
+000015d0: 6c79 2c20 796f 7520 6d61 7920 7761 6e74  ly, you may want
+000015e0: 2074 6f20 696d 706c 656d 656e 7420 6120   to implement a 
+000015f0: 6d65 7472 6963 206c 6561 726e 696e 6720  metric learning 
+00001600: 7069 7065 6c69 6e65 2062 7920 796f 7572  pipeline by your
+00001610: 7365 6c66 2e0a 2020 2a2a 5468 6572 6520  self..  **There 
+00001620: 6973 2061 206c 6f74 206f 6620 776f 726b  is a lot of work
+00001630: 2a2a 3a20 746f 2075 7365 2074 7269 706c  **: to use tripl
+00001640: 6574 206c 6f73 7320 796f 7520 6e65 6564  et loss you need
+00001650: 2074 6f20 666f 726d 2062 6174 6368 6573   to form batches
+00001660: 2069 6e20 6120 7370 6563 6966 6963 2077   in a specific w
+00001670: 6179 2c0a 2020 696d 706c 656d 656e 7420  ay,.  implement 
+00001680: 6469 6666 6572 656e 7420 6b69 6e64 7320  different kinds 
+00001690: 6f66 2074 7269 706c 6574 7320 6d69 6e69  of triplets mini
+000016a0: 6e67 2c20 7472 6163 6b69 6e67 2064 6973  ng, tracking dis
+000016b0: 7461 6e63 6573 2c20 6574 632e 2046 6f72  tances, etc. For
+000016c0: 2074 6865 2076 616c 6964 6174 696f 6e2c   the validation,
+000016d0: 2079 6f75 2061 6c73 6f20 6e65 6564 2074   you also need t
+000016e0: 6f0a 2020 696d 706c 656d 656e 7420 7265  o.  implement re
+000016f0: 7472 6965 7661 6c20 6d65 7472 6963 732c  trieval metrics,
+00001700: 0a20 2077 6869 6368 2069 6e63 6c75 6465  .  which include
+00001710: 2065 6666 6563 7469 7665 2065 6d62 6564   effective embed
+00001720: 6469 6e67 7320 6163 6375 6d75 6c61 7469  dings accumulati
+00001730: 6f6e 2064 7572 696e 6720 7468 6520 6570  on during the ep
+00001740: 6f63 682c 2063 6f76 6572 696e 6720 636f  och, covering co
+00001750: 726e 6572 2063 6173 6573 2c20 6574 632e  rner cases, etc.
+00001760: 0a20 2049 7427 7320 6576 656e 2068 6172  .  It's even har
+00001770: 6465 7220 6966 2079 6f75 2068 6176 6520  der if you have 
+00001780: 7365 7665 7261 6c20 6770 7573 2061 6e64  several gpus and
+00001790: 2075 7365 2044 4450 2e0a 2020 596f 7520   use DDP..  You 
+000017a0: 6d61 7920 616c 736f 2077 616e 7420 746f  may also want to
+000017b0: 2076 6973 7561 6c69 7a65 2079 6f75 7220   visualize your 
+000017c0: 7365 6172 6368 2072 6571 7565 7374 7320  search requests 
+000017d0: 6279 2068 6967 686c 6967 6874 696e 6720  by highlighting 
+000017e0: 676f 6f64 2061 6e64 2062 6164 2073 6561  good and bad sea
+000017f0: 7263 6820 7265 7375 6c74 732e 0a20 2049  rch results..  I
+00001800: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
+00001810: 6974 2062 7920 796f 7572 7365 6c66 2c20  it by yourself, 
+00001820: 796f 7520 6361 6e20 7369 6d70 6c79 2075  you can simply u
+00001830: 7365 204f 4d4c 2066 6f72 2079 6f75 7220  se OML for your 
+00001840: 7075 7270 6f73 6573 2e0a 0a3c 2f70 3e0a  purposes...</p>.
+00001850: 3c2f 6465 7461 696c 733e 0a0a 0a3c 6465  </details>...<de
+00001860: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+00001870: 5768 6174 2069 7320 7468 6520 6469 6666  What is the diff
+00001880: 6572 656e 6365 2062 6574 7765 656e 204f  erence between O
+00001890: 7065 6e20 4d65 7472 6963 204c 6561 726e  pen Metric Learn
+000018a0: 696e 6720 616e 6420 5079 546f 7263 6820  ing and PyTorch 
+000018b0: 4d65 7472 6963 204c 6561 726e 696e 673f  Metric Learning?
+000018c0: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+000018d0: 5b50 4d4c 5d28 6874 7470 733a 2f2f 6769  [PML](https://gi
+000018e0: 7468 7562 2e63 6f6d 2f4b 6576 696e 4d75  thub.com/KevinMu
+000018f0: 7367 7261 7665 2f70 7974 6f72 6368 2d6d  sgrave/pytorch-m
+00001900: 6574 7269 632d 6c65 6172 6e69 6e67 2920  etric-learning) 
+00001910: 6973 2074 6865 2070 6f70 756c 6172 206c  is the popular l
+00001920: 6962 7261 7279 2066 6f72 204d 6574 7269  ibrary for Metri
+00001930: 6320 4c65 6172 6e69 6e67 2c0a 616e 6420  c Learning,.and 
+00001940: 6974 2069 6e63 6c75 6465 7320 6120 7269  it includes a ri
+00001950: 6368 2063 6f6c 6c65 6374 696f 6e20 6f66  ch collection of
+00001960: 206c 6f73 7365 732c 206d 696e 6572 732c   losses, miners,
+00001970: 2064 6973 7461 6e63 6573 2c20 616e 6420   distances, and 
+00001980: 7265 6475 6365 7273 3b20 7468 6174 2069  reducers; that i
+00001990: 7320 7768 7920 7765 2070 726f 7669 6465  s why we provide
+000019a0: 2073 7472 6169 6768 7466 6f72 7761 7264   straightforward
+000019b0: 0a5b 6578 616d 706c 6573 5d28 6874 7470  .[examples](http
+000019c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+000019d0: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+000019e0: 7269 632d 6c65 6172 6e69 6e67 2375 7361  ric-learning#usa
+000019f0: 6765 2d77 6974 682d 7079 746f 7263 682d  ge-with-pytorch-
+00001a00: 6d65 7472 6963 2d6c 6561 726e 696e 6729  metric-learning)
+00001a10: 206f 6620 7573 696e 6720 7468 656d 2077   of using them w
+00001a20: 6974 6820 4f4d 4c2e 0a49 6e69 7469 616c  ith OML..Initial
+00001a30: 6c79 2c20 7765 2074 7269 6564 2074 6f20  ly, we tried to 
+00001a40: 7573 6520 504d 4c2c 2062 7574 2069 6e20  use PML, but in 
+00001a50: 7468 6520 656e 642c 2077 6520 6361 6d65  the end, we came
+00001a60: 2075 7020 7769 7468 206f 7572 206c 6962   up with our lib
+00001a70: 7261 7279 2c20 7768 6963 6820 6973 206d  rary, which is m
+00001a80: 6f72 6520 7069 7065 6c69 6e65 202f 2072  ore pipeline / r
+00001a90: 6563 6970 6573 206f 7269 656e 7465 642e  ecipes oriented.
+00001aa0: 0a54 6861 7420 6973 2068 6f77 204f 4d4c  .That is how OML
+00001ab0: 2064 6966 6665 7273 2066 726f 6d20 504d   differs from PM
+00001ac0: 4c3a 0a0a 2a20 4f4d 4c20 6861 7320 5b50  L:..* OML has [P
+00001ad0: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
+00001ae0: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00001af0: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00001b00: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+00001b10: 6d61 696e 2f70 6970 656c 696e 6573 290a  main/pipelines).
+00001b20: 2020 7768 6963 6820 616c 6c6f 7773 2074    which allows t
+00001b30: 7261 696e 696e 6720 6d6f 6465 6c73 2062  raining models b
+00001b40: 7920 7072 6570 6172 696e 6720 6120 636f  y preparing a co
+00001b50: 6e66 6967 2061 6e64 2079 6f75 7220 6461  nfig and your da
+00001b60: 7461 2069 6e20 7468 6520 7265 7175 6972  ta in the requir
+00001b70: 6564 2066 6f72 6d61 740a 2020 2869 7427  ed format.  (it'
+00001b80: 7320 6c69 6b65 2063 6f6e 7665 7274 696e  s like convertin
+00001b90: 6720 6461 7461 2069 6e74 6f20 434f 434f  g data into COCO
+00001ba0: 2066 6f72 6d61 7420 746f 2074 7261 696e   format to train
+00001bb0: 2061 2064 6574 6563 746f 7220 6672 6f6d   a detector from
+00001bc0: 205b 6d6d 6465 7465 6374 696f 6e5d 2868   [mmdetection](h
+00001bd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001be0: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d64  m/open-mmlab/mmd
+00001bf0: 6574 6563 7469 6f6e 2929 2e0a 0a2a 204f  etection))...* O
+00001c00: 4d4c 2066 6f63 7573 6573 206f 6e20 656e  ML focuses on en
+00001c10: 642d 746f 2d65 6e64 2070 6970 656c 696e  d-to-end pipelin
+00001c20: 6573 2061 6e64 2070 7261 6374 6963 616c  es and practical
+00001c30: 2075 7365 2063 6173 6573 2e0a 2020 4974   use cases..  It
+00001c40: 2068 6173 2063 6f6e 6669 6720 6261 7365   has config base
+00001c50: 6420 6578 616d 706c 6573 206f 6e20 706f  d examples on po
+00001c60: 7075 6c61 7220 6265 6e63 686d 6172 6b73  pular benchmarks
+00001c70: 2063 6c6f 7365 2074 6f20 7265 616c 206c   close to real l
+00001c80: 6966 6520 286c 696b 6520 7068 6f74 6f73  ife (like photos
+00001c90: 206f 6620 7072 6f64 7563 7473 206f 6620   of products of 
+00001ca0: 7468 6f75 7361 6e64 7320 6964 7329 2e0a  thousands ids)..
+00001cb0: 2020 5765 2066 6f75 6e64 2073 6f6d 6520    We found some 
+00001cc0: 676f 6f64 2063 6f6d 6269 6e61 7469 6f6e  good combination
+00001cd0: 7320 6f66 2068 7970 6572 7061 7261 6d65  s of hyperparame
+00001ce0: 7465 7273 206f 6e20 7468 6573 6520 6461  ters on these da
+00001cf0: 7461 7365 7473 2c20 7472 6169 6e65 6420  tasets, trained 
+00001d00: 616e 6420 7075 626c 6973 6865 6420 6d6f  and published mo
+00001d10: 6465 6c73 2061 6e64 2074 6865 6972 2063  dels and their c
+00001d20: 6f6e 6669 6773 2e0a 2020 5468 7573 2c20  onfigs..  Thus, 
+00001d30: 6974 206d 616b 6573 204f 4d4c 206d 6f72  it makes OML mor
+00001d40: 6520 7265 6369 7065 7320 6f72 6965 6e74  e recipes orient
+00001d50: 6564 2074 6861 6e20 504d 4c2c 2061 6e64  ed than PML, and
+00001d60: 2069 7473 2061 7574 686f 720a 2020 5b63   its author.  [c
+00001d70: 6f6e 6669 726d 735d 2868 7474 7073 3a2f  onfirms](https:/
+00001d80: 2f67 6974 6875 622e 636f 6d2f 4b65 7669  /github.com/Kevi
+00001d90: 6e4d 7573 6772 6176 652f 7079 746f 7263  nMusgrave/pytorc
+00001da0: 682d 6d65 7472 6963 2d6c 6561 726e 696e  h-metric-learnin
+00001db0: 672f 6973 7375 6573 2f31 3639 2369 7373  g/issues/169#iss
+00001dc0: 7565 636f 6d6d 656e 742d 3637 3038 3134  uecomment-670814
+00001dd0: 3339 3329 0a20 2074 6869 7320 7361 7969  393).  this sayi
+00001de0: 6e67 2074 6861 7420 6869 7320 6c69 6272  ng that his libr
+00001df0: 6172 7920 6973 2061 2073 6574 206f 6620  ary is a set of 
+00001e00: 746f 6f6c 7320 7261 7468 6572 2074 6865  tools rather the
+00001e10: 2072 6563 6970 6573 2c20 6d6f 7265 6f76   recipes, moreov
+00001e20: 6572 2c20 7468 6520 6578 616d 706c 6573  er, the examples
+00001e30: 2069 6e20 504d 4c20 6172 6520 6d6f 7374   in PML are most
+00001e40: 6c79 2066 6f72 2043 4946 4152 2061 6e64  ly for CIFAR and
+00001e50: 204d 4e49 5354 2064 6174 6173 6574 732e   MNIST datasets.
+00001e60: 0a0a 2a20 4f4d 4c20 6861 7320 7468 6520  ..* OML has the 
+00001e70: 5b5a 6f6f 5d28 6874 7470 733a 2f2f 6769  [Zoo](https://gi
+00001e80: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
+00001e90: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
+00001ea0: 6172 6e69 6e67 237a 6f6f 2920 6f66 2070  arning#zoo) of p
+00001eb0: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
+00001ec0: 2074 6861 7420 6361 6e20 6265 2065 6173   that can be eas
+00001ed0: 696c 7920 6163 6365 7373 6564 2066 726f  ily accessed fro
+00001ee0: 6d0a 2020 7468 6520 636f 6465 2069 6e20  m.  the code in 
+00001ef0: 7468 6520 7361 6d65 2077 6179 2061 7320  the same way as 
+00001f00: 696e 2060 746f 7263 6876 6973 696f 6e60  in `torchvision`
+00001f10: 2028 7768 656e 2079 6f75 2074 7970 6520   (when you type 
+00001f20: 6072 6573 6e65 7435 3028 7072 6574 7261  `resnet50(pretra
+00001f30: 696e 6564 3d54 7275 6529 6029 2e0a 0a2a  ined=True)`)...*
+00001f40: 204f 4d4c 2069 7320 696e 7465 6772 6174   OML is integrat
+00001f50: 6564 2077 6974 6820 5b50 7954 6f72 6368  ed with [PyTorch
+00001f60: 204c 6967 6874 6e69 6e67 5d28 6874 7470   Lightning](http
+00001f70: 733a 2f2f 7777 772e 7079 746f 7263 686c  s://www.pytorchl
+00001f80: 6967 6874 6e69 6e67 2e61 692f 292c 2073  ightning.ai/), s
+00001f90: 6f2c 2077 6520 6361 6e20 7573 6520 7468  o, we can use th
+00001fa0: 6520 706f 7765 7220 6f66 2069 7473 0a20  e power of its. 
+00001fb0: 205b 5472 6169 6e65 725d 2868 7474 7073   [Trainer](https
+00001fc0: 3a2f 2f70 7974 6f72 6368 2d6c 6967 6874  ://pytorch-light
+00001fd0: 6e69 6e67 2e72 6561 6474 6865 646f 6373  ning.readthedocs
+00001fe0: 2e69 6f2f 656e 2f73 7461 626c 652f 636f  .io/en/stable/co
+00001ff0: 6d6d 6f6e 2f74 7261 696e 6572 2e68 746d  mmon/trainer.htm
+00002000: 6c29 2e0a 2020 5468 6973 2069 7320 6573  l)..  This is es
+00002010: 7065 6369 616c 6c79 2068 656c 7066 756c  pecially helpful
+00002020: 2077 6865 6e20 7765 2077 6f72 6b20 7769   when we work wi
+00002030: 7468 2044 4450 2c20 736f 2c20 796f 7520  th DDP, so, you 
+00002040: 636f 6d70 6172 6520 6f75 720a 2020 5b44  compare our.  [D
+00002050: 4450 2065 7861 6d70 6c65 5d28 6874 7470  DP example](http
+00002060: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00002070: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00002080: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00002090: 742f 6578 616d 706c 6573 2f70 7974 686f  t/examples/pytho
+000020a0: 6e2e 6874 6d6c 290a 2020 616e 6420 7468  n.html).  and th
+000020b0: 650a 2020 5b50 4d4c 7320 6f6e 655d 2868  e.  [PMLs one](h
+000020c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000020d0: 6d2f 4b65 7669 6e4d 7573 6772 6176 652f  m/KevinMusgrave/
+000020e0: 7079 746f 7263 682d 6d65 7472 6963 2d6c  pytorch-metric-l
+000020f0: 6561 726e 696e 672f 626c 6f62 2f6d 6173  earning/blob/mas
+00002100: 7465 722f 6578 616d 706c 6573 2f6e 6f74  ter/examples/not
+00002110: 6562 6f6f 6b73 2f44 6973 7472 6962 7574  ebooks/Distribut
+00002120: 6564 5472 6970 6c65 744d 6172 6769 6e4c  edTripletMarginL
+00002130: 6f73 734d 4e49 5354 2e69 7079 6e62 292e  ossMNIST.ipynb).
+00002140: 0a20 2042 7920 7468 6520 7761 792c 2050  .  By the way, P
+00002150: 4d4c 2061 6c73 6f20 6861 7320 5b54 7261  ML also has [Tra
+00002160: 696e 6572 735d 2868 7474 7073 3a2f 2f6b  iners](https://k
+00002170: 6576 696e 6d75 7367 7261 7665 2e67 6974  evinmusgrave.git
+00002180: 6875 622e 696f 2f70 7974 6f72 6368 2d6d  hub.io/pytorch-m
+00002190: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+000021a0: 7261 696e 6572 732f 292c 2062 7574 2069  rainers/), but i
+000021b0: 7427 7320 6e6f 740a 2020 7769 6465 6c79  t's not.  widely
+000021c0: 2075 7365 6420 696e 2074 6865 2065 7861   used in the exa
+000021d0: 6d70 6c65 7320 616e 6420 6375 7374 6f6d  mples and custom
+000021e0: 2060 7472 6169 6e60 202f 2060 7465 7374   `train` / `test
+000021f0: 6020 6675 6e63 7469 6f6e 7320 6172 6520  ` functions are 
+00002200: 7573 6564 2069 6e73 7465 6164 2e0a 0a57  used instead...W
+00002210: 6520 6265 6c69 6576 6520 7468 6174 2068  e believe that h
+00002220: 6176 696e 6720 5069 7065 6c69 6e65 732c  aving Pipelines,
+00002230: 206c 6163 6f6e 6963 2065 7861 6d70 6c65   laconic example
+00002240: 732c 2061 6e64 205a 6f6f 206f 6620 7072  s, and Zoo of pr
+00002250: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
+00002260: 7365 7473 2074 6865 2065 6e74 7279 2074  sets the entry t
+00002270: 6872 6573 686f 6c64 2074 6f20 6120 7265  hreshold to a re
+00002280: 616c 6c79 206c 6f77 2076 616c 7565 2e0a  ally low value..
+00002290: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
+000022a0: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
+000022b0: 6d6d 6172 793e 5768 6174 2069 7320 4d65  mmary>What is Me
+000022c0: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
+000022d0: 7375 6d6d 6172 793e 0a3c 703e 0a0a 4d65  summary>.<p>..Me
+000022e0: 7472 6963 204c 6561 726e 696e 6720 7072  tric Learning pr
+000022f0: 6f62 6c65 6d20 2861 6c73 6f20 6b6e 6f77  oblem (also know
+00002300: 6e20 6173 202a 6578 7472 656d 6520 636c  n as *extreme cl
+00002310: 6173 7369 6669 6361 7469 6f6e 2a20 7072  assification* pr
+00002320: 6f62 6c65 6d29 206d 6561 6e73 2061 2073  oblem) means a s
+00002330: 6974 7561 7469 6f6e 2069 6e20 7768 6963  ituation in whic
+00002340: 6820 7765 0a68 6176 6520 7468 6f75 7361  h we.have thousa
+00002350: 6e64 7320 6f66 2069 6473 206f 6620 736f  nds of ids of so
+00002360: 6d65 2065 6e74 6974 6965 732c 2062 7574  me entities, but
+00002370: 206f 6e6c 7920 6120 6665 7720 7361 6d70   only a few samp
+00002380: 6c65 7320 666f 7220 6576 6572 7920 656e  les for every en
+00002390: 7469 7479 2e0a 4f66 7465 6e20 7765 2061  tity..Often we a
+000023a0: 7373 756d 6520 7468 6174 2064 7572 696e  ssume that durin
+000023b0: 6720 7468 6520 7465 7374 2073 7461 6765  g the test stage
+000023c0: 2028 6f72 2070 726f 6475 6374 696f 6e29   (or production)
+000023d0: 2077 6520 7769 6c6c 2064 6561 6c20 7769   we will deal wi
+000023e0: 7468 2075 6e73 6565 6e20 656e 7469 7469  th unseen entiti
+000023f0: 6573 0a77 6869 6368 206d 616b 6573 2069  es.which makes i
+00002400: 7420 696d 706f 7373 6962 6c65 2074 6f20  t impossible to 
+00002410: 6170 706c 7920 7468 6520 7661 6e69 6c6c  apply the vanill
+00002420: 6120 636c 6173 7369 6669 6361 7469 6f6e  a classification
+00002430: 2070 6970 656c 696e 6520 6469 7265 6374   pipeline direct
+00002440: 6c79 2e20 496e 206d 616e 7920 6361 7365  ly. In many case
+00002450: 7320 6f62 7461 696e 6564 2065 6d62 6564  s obtained embed
+00002460: 6469 6e67 730a 6172 6520 7573 6564 2074  dings.are used t
+00002470: 6f20 7065 7266 6f72 6d20 7365 6172 6368  o perform search
+00002480: 206f 7220 6d61 7463 6869 6e67 2070 726f   or matching pro
+00002490: 6365 6475 7265 7320 6f76 6572 2074 6865  cedures over the
+000024a0: 6d2e 0a0a 4865 7265 2061 7265 2061 2066  m...Here are a f
+000024b0: 6577 2065 7861 6d70 6c65 7320 6f66 2073  ew examples of s
+000024c0: 7563 6820 7461 736b 7320 6672 6f6d 2074  uch tasks from t
+000024d0: 6865 2063 6f6d 7075 7465 7220 7669 7369  he computer visi
+000024e0: 6f6e 2073 7068 6572 653a 0a2a 2050 6572  on sphere:.* Per
+000024f0: 736f 6e2f 416e 696d 616c 2052 652d 4964  son/Animal Re-Id
+00002500: 656e 7469 6669 6361 7469 6f6e 0a2a 2046  entification.* F
+00002510: 6163 6520 5265 636f 676e 6974 696f 6e0a  ace Recognition.
+00002520: 2a20 4c61 6e64 6d61 726b 2052 6563 6f67  * Landmark Recog
+00002530: 6e69 7469 6f6e 0a2a 2053 6561 7263 6869  nition.* Searchi
+00002540: 6e67 2065 6e67 696e 6573 2066 6f72 206f  ng engines for o
+00002550: 6e6c 696e 6520 7368 6f70 730a 2061 6e64  nline shops. and
+00002560: 206d 616e 7920 6f74 6865 7273 2e0a 3c2f   many others..</
+00002570: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
+00002580: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+00002590: 7279 3e47 6c6f 7373 6172 7920 284e 616d  ry>Glossary (Nam
+000025a0: 696e 6720 636f 6e76 656e 7469 6f6e 2920  ing convention) 
+000025b0: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+000025c0: 2a20 6065 6d62 6564 6469 6e67 6020 2d20  * `embedding` - 
+000025d0: 6d6f 6465 6c27 7320 6f75 7470 7574 2028  model's output (
+000025e0: 616c 736f 206b 6e6f 776e 2061 7320 6066  also known as `f
+000025f0: 6561 7475 7265 7320 7665 6374 6f72 6020  eatures vector` 
+00002600: 6f72 2060 6465 7363 7269 7074 6f72 6029  or `descriptor`)
+00002610: 2e0a 2a20 6071 7565 7279 6020 2d20 6120  ..* `query` - a 
+00002620: 7361 6d70 6c65 2077 6869 6368 2069 7320  sample which is 
+00002630: 7573 6564 2061 7320 6120 7265 7175 6573  used as a reques
+00002640: 7420 696e 2074 6865 2072 6574 7269 6576  t in the retriev
+00002650: 616c 2070 726f 6365 6475 7265 2e0a 2a20  al procedure..* 
+00002660: 6067 616c 6c65 7279 2073 6574 6020 2d20  `gallery set` - 
+00002670: 7468 6520 7365 7420 6f66 2065 6e74 6974  the set of entit
+00002680: 6965 7320 746f 2073 6561 7263 6820 6974  ies to search it
+00002690: 656d 7320 7369 6d69 6c61 7220 746f 2060  ems similar to `
+000026a0: 7175 6572 7960 2028 616c 736f 206b 6e6f  query` (also kno
+000026b0: 776e 2061 7320 6072 6566 6572 656e 6365  wn as `reference
+000026c0: 6020 6f72 2060 696e 6465 7860 292e 0a2a  ` or `index`)..*
+000026d0: 2060 5361 6d70 6c65 7260 202d 2061 6e20   `Sampler` - an 
+000026e0: 6172 6775 6d65 6e74 2066 6f72 2060 4461  argument for `Da
+000026f0: 7461 4c6f 6164 6572 6020 7768 6963 6820  taLoader` which 
+00002700: 6973 2075 7365 6420 746f 2066 6f72 6d20  is used to form 
+00002710: 6261 7463 6865 730a 2a20 604d 696e 6572  batches.* `Miner
+00002720: 6020 2d20 7468 6520 6f62 6a65 6374 2074  ` - the object t
+00002730: 6f20 666f 726d 2070 6169 7273 206f 7220  o form pairs or 
+00002740: 7472 6970 6c65 7473 2061 6674 6572 2074  triplets after t
+00002750: 6865 2062 6174 6368 2077 6173 2066 6f72  he batch was for
+00002760: 6d65 6420 6279 2060 5361 6d70 6c65 7260  med by `Sampler`
+00002770: 2e20 4974 2773 206e 6f74 206e 6563 6573  . It's not neces
+00002780: 7361 7279 2074 6f20 666f 726d 0a20 2074  sary to form.  t
+00002790: 6865 2063 6f6d 6269 6e61 7469 6f6e 7320  he combinations 
+000027a0: 6f66 2073 616d 706c 6573 206f 6e6c 7920  of samples only 
+000027b0: 696e 7369 6465 2074 6865 2063 7572 7265  inside the curre
+000027c0: 6e74 2062 6174 6368 2c20 7468 7573 2c20  nt batch, thus, 
+000027d0: 7468 6520 6d65 6d6f 7279 2062 616e 6b20  the memory bank 
+000027e0: 6d61 7920 6265 2061 2070 6172 7420 6f66  may be a part of
+000027f0: 2060 4d69 6e65 7260 2e0a 2a20 6053 616d   `Miner`..* `Sam
+00002800: 706c 6573 602f 604c 6162 656c 7360 2f60  ples`/`Labels`/`
+00002810: 496e 7374 616e 6365 7360 202d 2061 7320  Instances` - as 
+00002820: 616e 2065 7861 6d70 6c65 206c 6574 2773  an example let's
+00002830: 2063 6f6e 7369 6465 7220 4465 6570 4661   consider DeepFa
+00002840: 7368 696f 6e20 6461 7461 7365 742e 2049  shion dataset. I
+00002850: 7420 696e 636c 7564 6573 2074 686f 7573  t includes thous
+00002860: 616e 6473 206f 660a 2020 6661 7368 696f  ands of.  fashio
+00002870: 6e20 6974 656d 2069 6473 2028 7765 206e  n item ids (we n
+00002880: 616d 6520 7468 656d 2060 6c61 6265 6c73  ame them `labels
+00002890: 6029 2061 6e64 2073 6576 6572 616c 2070  `) and several p
+000028a0: 686f 746f 7320 666f 7220 6561 6368 2069  hotos for each i
+000028b0: 7465 6d20 6964 0a20 2028 7765 206e 616d  tem id.  (we nam
+000028c0: 6520 7468 6520 696e 6469 7669 6475 616c  e the individual
+000028d0: 2070 686f 746f 2061 7320 6069 6e73 7461   photo as `insta
+000028e0: 6e63 6560 206f 7220 6073 616d 706c 6560  nce` or `sample`
+000028f0: 292e 2041 6c6c 206f 6620 7468 6520 6661  ). All of the fa
+00002900: 7368 696f 6e20 6974 656d 2069 6473 2068  shion item ids h
+00002910: 6176 6520 7468 6569 7220 6772 6f75 7073  ave their groups
+00002920: 206c 696b 650a 2020 2273 6b69 7274 7322   like.  "skirts"
+00002930: 2c20 226a 6163 6b65 7473 222c 2022 7368  , "jackets", "sh
+00002940: 6f72 7473 2220 616e 6420 736f 206f 6e20  orts" and so on 
+00002950: 2877 6520 6e61 6d65 2074 6865 6d20 6063  (we name them `c
+00002960: 6174 6567 6f72 6965 7360 292e 0a20 204e  ategories`)..  N
+00002970: 6f74 652c 2077 6520 6176 6f69 6420 7573  ote, we avoid us
+00002980: 696e 6720 7468 6520 7465 726d 2060 636c  ing the term `cl
+00002990: 6173 7360 2074 6f20 6176 6f69 6420 6d69  ass` to avoid mi
+000029a0: 7375 6e64 6572 7374 616e 6469 6e67 2e0a  sunderstanding..
+000029b0: 2a20 6074 7261 696e 696e 6720 6570 6f63  * `training epoc
+000029c0: 6860 202d 2062 6174 6368 2073 616d 706c  h` - batch sampl
+000029d0: 6572 7320 7768 6963 6820 7765 2075 7365  ers which we use
+000029e0: 2066 6f72 2063 6f6d 6269 6e61 7469 6f6e   for combination
+000029f0: 2d62 6173 6564 206c 6f73 7365 7320 7573  -based losses us
+00002a00: 7561 6c6c 7920 6861 7665 2061 206c 656e  ually have a len
+00002a10: 6774 6820 6571 7561 6c20 746f 0a20 2060  gth equal to.  `
+00002a20: 5b6e 756d 6265 7220 6f66 206c 6162 656c  [number of label
+00002a30: 7320 696e 2074 7261 696e 696e 6720 6461  s in training da
+00002a40: 7461 7365 745d 202f 205b 6e75 6d62 6572  taset] / [number
+00002a50: 7320 6f66 206c 6162 656c 7320 696e 206f  s of labels in o
+00002a60: 6e65 2062 6174 6368 5d60 2e20 4974 206d  ne batch]`. It m
+00002a70: 6561 6e73 2074 6861 7420 7765 2064 6f6e  eans that we don
+00002a80: 2774 206f 6273 6572 7665 2061 6c6c 206f  't observe all o
+00002a90: 660a 2020 7468 6520 6176 6169 6c61 626c  f.  the availabl
+00002aa0: 6520 7472 6169 6e69 6e67 2073 616d 706c  e training sampl
+00002ab0: 6573 2069 6e20 6f6e 6520 6570 6f63 6820  es in one epoch 
+00002ac0: 2861 7320 6f70 706f 7365 6420 746f 2076  (as opposed to v
+00002ad0: 616e 696c 6c61 2063 6c61 7373 6966 6963  anilla classific
+00002ae0: 6174 696f 6e29 2c0a 2020 696e 7374 6561  ation),.  instea
+00002af0: 642c 2077 6520 6f62 7365 7276 6520 616c  d, we observe al
+00002b00: 6c20 6f66 2074 6865 2061 7661 696c 6162  l of the availab
+00002b10: 6c65 206c 6162 656c 732e 0a0a 3c2f 703e  le labels...</p>
+00002b20: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
+00002b30: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00002b40: 3e48 6f77 2067 6f6f 6420 6d61 7920 6265  >How good may be
+00002b50: 2061 206d 6f64 656c 2074 7261 696e 6564   a model trained
+00002b60: 2077 6974 6820 4f4d 4c3f 203c 2f73 756d   with OML? </sum
+00002b70: 6d61 7279 3e0a 3c70 3e0a 0a49 7420 6d61  mary>.<p>..It ma
+00002b80: 7920 6265 2063 6f6d 7061 7261 626c 6520  y be comparable 
+00002b90: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
+00002ba0: 2028 3230 3232 2079 6561 7229 205b 536f   (2022 year) [So
+00002bb0: 7441 5d28 6874 7470 733a 2f2f 7061 7065  tA](https://pape
+00002bc0: 7273 7769 7468 636f 6465 2e63 6f6d 2f74  rswithcode.com/t
+00002bd0: 6173 6b2f 6d65 7472 6963 2d6c 6561 726e  ask/metric-learn
+00002be0: 696e 6729 206d 6574 686f 6473 2c0a 666f  ing) methods,.fo
+00002bf0: 7220 6578 616d 706c 652c 205b 4879 702d  r example, [Hyp-
+00002c00: 5669 545d 2868 7474 7073 3a2f 2f61 7278  ViT](https://arx
+00002c10: 6976 2e6f 7267 2f70 6466 2f32 3230 332e  iv.org/pdf/2203.
+00002c20: 3130 3833 332e 7064 6629 2e0a 2a28 4665  10833.pdf)..*(Fe
+00002c30: 7720 776f 7264 7320 6162 6f75 7420 7468  w words about th
+00002c40: 6973 2061 7070 726f 6163 683a 2069 7427  is approach: it'
+00002c50: 7320 6120 5669 5420 6172 6368 6974 6563  s a ViT architec
+00002c60: 7475 7265 2074 7261 696e 6564 2077 6974  ture trained wit
+00002c70: 6820 636f 6e74 7261 7374 6976 6520 6c6f  h contrastive lo
+00002c80: 7373 2c0a 6275 7420 7468 6520 656d 6265  ss,.but the embe
+00002c90: 6464 696e 6773 2077 6572 6520 7072 6f6a  ddings were proj
+00002ca0: 6563 7465 6420 696e 746f 2073 6f6d 6520  ected into some 
+00002cb0: 6879 7065 7262 6f6c 6963 2073 7061 6365  hyperbolic space
+00002cc0: 2e0a 4173 2074 6865 2061 7574 686f 7273  ..As the authors
+00002cd0: 2063 6c61 696d 6564 2c20 7375 6368 2061   claimed, such a
+00002ce0: 2073 7061 6365 2069 7320 6162 6c65 2074   space is able t
+00002cf0: 6f20 6465 7363 7269 6265 2074 6865 206e  o describe the n
+00002d00: 6573 7465 6420 7374 7275 6374 7572 6520  ested structure 
+00002d10: 6f66 2072 6561 6c2d 776f 726c 6420 6461  of real-world da
+00002d20: 7461 2e0a 536f 2c20 7468 6520 7061 7065  ta..So, the pape
+00002d30: 7220 7265 7175 6972 6573 2073 6f6d 6520  r requires some 
+00002d40: 6865 6176 7920 6d61 7468 2074 6f20 6164  heavy math to ad
+00002d50: 6170 7420 7468 6520 7573 7561 6c20 6f70  apt the usual op
+00002d60: 6572 6174 696f 6e73 2066 6f72 2074 6865  erations for the
+00002d70: 2068 7970 6572 626f 6c69 6361 6c20 7370   hyperbolical sp
+00002d80: 6163 652e 292a 0a0a 5765 2074 7261 696e  ace.)*..We train
+00002d90: 6564 2074 6865 2073 616d 6520 6172 6368  ed the same arch
+00002da0: 6974 6563 7475 7265 2077 6974 6820 7472  itecture with tr
+00002db0: 6970 6c65 7420 6c6f 7373 2c20 6669 7869  iplet loss, fixi
+00002dc0: 6e67 2074 6865 2072 6573 7420 6f66 2074  ng the rest of t
+00002dd0: 6865 2070 6172 616d 6574 6572 733a 0a74  he parameters:.t
+00002de0: 7261 696e 696e 6720 616e 6420 7465 7374  raining and test
+00002df0: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+00002e00: 2c20 696d 6167 6520 7369 7a65 2c20 616e  , image size, an
+00002e10: 6420 6f70 7469 6d69 7a65 722e 2053 6565  d optimizer. See
+00002e20: 2063 6f6e 6669 6773 2069 6e20 5b4d 6f64   configs in [Mod
+00002e30: 656c 7320 5a6f 6f5d 2868 7474 7073 3a2f  els Zoo](https:/
+00002e40: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+00002e50: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+00002e60: 2d6c 6561 726e 696e 6723 7a6f 6f29 2e0a  -learning#zoo)..
+00002e70: 5468 6520 7472 6963 6b20 7761 7320 696e  The trick was in
+00002e80: 2068 6575 7269 7374 6963 7320 696e 206f   heuristics in o
+00002e90: 7572 206d 696e 6572 2061 6e64 2073 616d  ur miner and sam
+00002ea0: 706c 6572 3a0a 0a2a 205b 4361 7465 676f  pler:..* [Catego
+00002eb0: 7279 2042 616c 616e 6365 2053 616d 706c  ry Balance Sampl
+00002ec0: 6572 5d28 6874 7470 733a 2f2f 6f70 656e  er](https://open
+00002ed0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00002ee0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002ef0: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
+00002f00: 7473 2f73 616d 706c 6572 732e 6874 6d6c  ts/samplers.html
+00002f10: 2363 6174 6567 6f72 7962 616c 616e 6365  #categorybalance
+00002f20: 7361 6d70 6c65 7229 0a20 2066 6f72 6d73  sampler).  forms
+00002f30: 2074 6865 2062 6174 6368 6573 206c 696d   the batches lim
+00002f40: 6974 696e 6720 7468 6520 6e75 6d62 6572  iting the number
+00002f50: 206f 6620 6361 7465 676f 7269 6573 202a   of categories *
+00002f60: 432a 2069 6e20 6974 2e0a 2020 466f 7220  C* in it..  For 
+00002f70: 696e 7374 616e 6365 2c20 7768 656e 202a  instance, when *
+00002f80: 4320 3d20 312a 2069 7420 7075 7473 206f  C = 1* it puts o
+00002f90: 6e6c 7920 6a61 636b 6574 7320 696e 206f  nly jackets in o
+00002fa0: 6e65 2062 6174 6368 2061 6e64 206f 6e6c  ne batch and onl
+00002fb0: 7920 6a65 616e 7320 696e 746f 2061 6e6f  y jeans into ano
+00002fc0: 7468 6572 206f 6e65 2028 6a75 7374 2061  ther one (just a
+00002fd0: 6e20 6578 616d 706c 6529 2e0a 2020 4974  n example)..  It
+00002fe0: 2061 7574 6f6d 6174 6963 616c 6c79 206d   automatically m
+00002ff0: 616b 6573 2074 6865 206e 6567 6174 6976  akes the negativ
+00003000: 6520 7061 6972 7320 6861 7264 6572 3a20  e pairs harder: 
+00003010: 6974 2773 206d 6f72 6520 6d65 616e 696e  it's more meanin
+00003020: 6766 756c 2066 6f72 2061 206d 6f64 656c  gful for a model
+00003030: 2074 6f20 7265 616c 6973 6520 7768 7920   to realise why 
+00003040: 7477 6f20 6a61 636b 6574 730a 2020 6172  two jackets.  ar
+00003050: 6520 6469 6666 6572 656e 7420 7468 616e  e different than
+00003060: 2074 6f20 756e 6465 7273 7461 6e64 2074   to understand t
+00003070: 6865 2073 616d 6520 6162 6f75 7420 6120  he same about a 
+00003080: 6a61 636b 6574 2061 6e64 2061 2074 2d73  jacket and a t-s
+00003090: 6869 7274 2e0a 0a2a 205b 4861 7264 2054  hirt...* [Hard T
+000030a0: 7269 706c 6574 7320 4d69 6e65 725d 2868  riplets Miner](h
+000030b0: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+000030c0: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+000030d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000030e0: 7465 7374 2f63 6f6e 7465 6e74 732f 6d69  test/contents/mi
+000030f0: 6e65 7273 2e68 746d 6c23 6861 7264 7472  ners.html#hardtr
+00003100: 6970 6c65 7473 6d69 6e65 7229 0a20 206d  ipletsminer).  m
+00003110: 616b 6573 2074 6865 2074 6173 6b20 6576  akes the task ev
+00003120: 656e 2068 6172 6465 7220 6b65 6570 696e  en harder keepin
+00003130: 6720 6f6e 6c79 2074 6865 2068 6172 6465  g only the harde
+00003140: 7374 2074 7269 706c 6574 7320 2877 6974  st triplets (wit
+00003150: 6820 6d61 7869 6d61 6c20 706f 7369 7469  h maximal positi
+00003160: 7665 2061 6e64 206d 696e 696d 616c 206e  ve and minimal n
+00003170: 6567 6174 6976 6520 6469 7374 616e 6365  egative distance
+00003180: 7329 2e0a 0a48 6572 6520 6172 6520 2a43  s)...Here are *C
+00003190: 4d43 4031 2a20 7363 6f72 6573 2066 6f72  MC@1* scores for
+000031a0: 2032 2070 6f70 756c 6172 2062 656e 6368   2 popular bench
+000031b0: 6d61 726b 732e 0a53 4f50 2064 6174 6173  marks..SOP datas
+000031c0: 6574 3a20 4879 702d 5669 5420 e280 9420  et: Hyp-ViT ... 
+000031d0: 3835 2e39 2c20 6f75 7273 20e2 8094 2038  85.9, ours ... 8
+000031e0: 362e 362e 2044 6565 7046 6173 6869 6f6e  6.6. DeepFashion
+000031f0: 2064 6174 6173 6574 3a20 4879 702d 5669   dataset: Hyp-Vi
+00003200: 5420 e280 9420 3932 2e35 2c20 6f75 7273  T ... 92.5, ours
+00003210: 20e2 8094 2039 322e 312e 0a54 6875 732c   ... 92.1..Thus,
+00003220: 2075 7469 6c69 7369 6e67 2073 696d 706c   utilising simpl
+00003230: 6520 6865 7572 6973 7469 6373 2061 6e64  e heuristics and
+00003240: 2061 766f 6964 696e 6720 6865 6176 7920   avoiding heavy 
+00003250: 6d61 7468 2077 6520 6172 6520 6162 6c65  math we are able
+00003260: 2074 6f20 7065 7266 6f72 6d20 6f6e 2053   to perform on S
+00003270: 6f74 4120 6c65 7665 6c2e 0a0a 3c2f 703e  otA level...</p>
+00003280: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00003290: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+000032a0: 5768 6174 2061 626f 7574 2053 656c 662d  What about Self-
+000032b0: 5375 7065 7276 6973 6564 204c 6561 726e  Supervised Learn
+000032c0: 696e 673f 3c2f 7375 6d6d 6172 793e 0a3c  ing?</summary>.<
+000032d0: 703e 0a0a 5265 6365 6e74 2072 6573 6561  p>..Recent resea
+000032e0: 7263 6820 696e 2053 534c 2064 6566 696e  rch in SSL defin
+000032f0: 6974 656c 7920 6f62 7461 696e 6564 2067  itely obtained g
+00003300: 7265 6174 2072 6573 756c 7473 2e20 5468  reat results. Th
+00003310: 6520 7072 6f62 6c65 6d20 6973 2074 6861  e problem is tha
+00003320: 7420 7468 6573 6520 6170 7072 6f61 6368  t these approach
+00003330: 6573 0a72 6571 7569 7265 6420 616e 2065  es.required an e
+00003340: 6e6f 726d 6f75 7320 616d 6f75 6e74 206f  normous amount o
+00003350: 6620 636f 6d70 7574 696e 6720 746f 2074  f computing to t
+00003360: 7261 696e 2074 6865 206d 6f64 656c 2e20  rain the model. 
+00003370: 4275 7420 696e 206f 7572 2066 7261 6d65  But in our frame
+00003380: 776f 726b 2c20 7765 2063 6f6e 7369 6465  work, we conside
+00003390: 7220 7468 6520 6d6f 7374 2063 6f6d 6d6f  r the most commo
+000033a0: 6e20 6361 7365 0a77 6865 6e20 7468 6520  n case.when the 
+000033b0: 6176 6572 6167 6520 7573 6572 2068 6173  average user has
+000033c0: 206e 6f20 6d6f 7265 2074 6861 6e20 6120   no more than a 
+000033d0: 6665 7720 4750 5573 2e0a 0a41 7420 7468  few GPUs...At th
+000033e0: 6520 7361 6d65 2074 696d 652c 2069 7420  e same time, it 
+000033f0: 776f 756c 6420 6265 2075 6e77 6973 6520  would be unwise 
+00003400: 746f 2069 676e 6f72 6520 7375 6363 6573  to ignore succes
+00003410: 7320 696e 2074 6869 7320 7370 6865 7265  s in this sphere
+00003420: 2c20 736f 2077 6520 7374 696c 6c20 6578  , so we still ex
+00003430: 706c 6f69 7420 6974 2069 6e20 7477 6f20  ploit it in two 
+00003440: 7761 7973 3a0a 2a20 4173 2061 2073 6f75  ways:.* As a sou
+00003450: 7263 6520 6f66 2063 6865 636b 706f 696e  rce of checkpoin
+00003460: 7473 2074 6861 7420 776f 756c 6420 6265  ts that would be
+00003470: 2067 7265 6174 2074 6f20 7374 6172 7420   great to start 
+00003480: 7472 6169 6e69 6e67 2077 6974 682e 2046  training with. F
+00003490: 726f 6d20 7075 626c 6963 6174 696f 6e73  rom publications
+000034a0: 2061 6e64 206f 7572 2065 7870 6572 6965   and our experie
+000034b0: 6e63 652c 0a20 2074 6865 7920 6172 6520  nce,.  they are 
+000034c0: 6d75 6368 2062 6574 7465 7220 6173 2069  much better as i
+000034d0: 6e69 7469 616c 6973 6174 696f 6e20 7468  nitialisation th
+000034e0: 616e 2074 6865 2064 6566 6175 6c74 2073  an the default s
+000034f0: 7570 6572 7669 7365 6420 6d6f 6465 6c20  upervised model 
+00003500: 7472 6169 6e65 6420 6f6e 2049 6d61 6765  trained on Image
+00003510: 4e65 742e 2054 6875 732c 2077 6520 6164  Net. Thus, we ad
+00003520: 6465 6420 7468 6520 706f 7373 6962 696c  ded the possibil
+00003530: 6974 790a 2020 746f 2069 6e69 7469 616c  ity.  to initial
+00003540: 6973 6520 796f 7572 206d 6f64 656c 7320  ise your models 
+00003550: 7573 696e 6720 7468 6573 6520 7072 6574  using these pret
+00003560: 7261 696e 6564 2063 6865 636b 706f 696e  rained checkpoin
+00003570: 7473 206f 6e6c 7920 6279 2070 6173 7369  ts only by passi
+00003580: 6e67 2061 6e20 6172 6775 6d65 6e74 2069  ng an argument i
+00003590: 6e20 7468 6520 636f 6e66 6967 206f 7220  n the config or 
+000035a0: 7468 6520 636f 6e73 7472 7563 746f 722e  the constructor.
+000035b0: 0a2a 2041 7320 6120 736f 7572 6365 206f  .* As a source o
+000035c0: 6620 696e 7370 6972 6174 696f 6e2e 2046  f inspiration. F
+000035d0: 6f72 2065 7861 6d70 6c65 2c20 7765 2061  or example, we a
+000035e0: 6461 7074 6564 2074 6865 2069 6465 6120  dapted the idea 
+000035f0: 6f66 2061 206d 656d 6f72 7920 6261 6e6b  of a memory bank
+00003600: 2066 726f 6d20 2a4d 6f43 6f2a 2066 6f72   from *MoCo* for
+00003610: 2074 6865 202a 5472 6970 6c65 744c 6f73   the *TripletLos
+00003620: 732a 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461  s*...</p>.</deta
+00003630: 696c 733e 0a0a 0a3c 6465 7461 696c 733e  ils>...<details>
+00003640: 0a3c 7375 6d6d 6172 793e 446f 2049 206e  .<summary>Do I n
+00003650: 6565 6420 746f 206b 6e6f 7720 6f74 6865  eed to know othe
+00003660: 7220 6672 616d 6577 6f72 6b73 2074 6f20  r frameworks to 
+00003670: 7573 6520 4f4d 4c3f 3c2f 7375 6d6d 6172  use OML?</summar
+00003680: 793e 0a3c 703e 0a0a 4e6f 2c20 796f 7520  y>.<p>..No, you 
+00003690: 646f 6e27 742e 204f 4d4c 2069 7320 6120  don't. OML is a 
+000036a0: 6672 616d 6577 6f72 6b2d 6167 6e6f 7374  framework-agnost
+000036b0: 6963 2e20 4465 7370 6974 6520 7765 2075  ic. Despite we u
+000036c0: 7365 2050 7954 6f72 6368 204c 6967 6874  se PyTorch Light
+000036d0: 6e69 6e67 2061 7320 6120 6c6f 6f70 0a72  ning as a loop.r
+000036e0: 756e 6e65 7220 666f 7220 7468 6520 6578  unner for the ex
+000036f0: 7065 7269 6d65 6e74 732c 2077 6520 616c  periments, we al
+00003700: 736f 206b 6565 7020 7468 6520 706f 7373  so keep the poss
+00003710: 6962 696c 6974 7920 746f 2072 756e 2065  ibility to run e
+00003720: 7665 7279 7468 696e 6720 6f6e 2070 7572  verything on pur
+00003730: 6520 5079 546f 7263 682e 0a54 6875 732c  e PyTorch..Thus,
+00003740: 206f 6e6c 7920 7468 6520 7469 6e79 2070   only the tiny p
+00003750: 6172 7420 6f66 204f 4d4c 2069 7320 4c69  art of OML is Li
+00003760: 6768 746e 696e 672d 7370 6563 6966 6963  ghtning-specific
+00003770: 2061 6e64 2077 6520 6b65 6570 2074 6869   and we keep thi
+00003780: 7320 6c6f 6769 6320 7365 7061 7261 7465  s logic separate
+00003790: 6c79 2066 726f 6d0a 6f74 6865 7220 636f  ly from.other co
+000037a0: 6465 2028 7365 6520 606f 6d6c 2e6c 6967  de (see `oml.lig
+000037b0: 6874 6e69 6e67 6029 2e20 4576 656e 2077  htning`). Even w
+000037c0: 6865 6e20 796f 7520 7573 6520 4c69 6768  hen you use Ligh
+000037d0: 746e 696e 672c 2079 6f75 2064 6f6e 2774  tning, you don't
+000037e0: 206e 6565 6420 746f 206b 6e6f 7720 6974   need to know it
+000037f0: 2c20 7369 6e63 650a 7765 2070 726f 7669  , since.we provi
+00003800: 6465 2072 6561 6479 2074 6f20 7573 6520  de ready to use 
+00003810: 5b50 6970 656c 696e 6573 5d28 6874 7470  [Pipelines](http
+00003820: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+00003830: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+00003840: 7269 632d 6c65 6172 6e69 6e67 2f62 6c6f  ric-learning/blo
+00003850: 622f 6d61 696e 2f70 6970 656c 696e 6573  b/main/pipelines
+00003860: 2f29 2e0a 0a54 6865 2070 6f73 7369 6269  /)...The possibi
+00003870: 6c69 7479 206f 6620 7573 696e 6720 7075  lity of using pu
+00003880: 7265 2050 7954 6f72 6368 2061 6e64 206d  re PyTorch and m
+00003890: 6f64 756c 6172 2073 7472 7563 7475 7265  odular structure
+000038a0: 206f 6620 7468 6520 636f 6465 206c 6561   of the code lea
+000038b0: 7665 7320 6120 726f 6f6d 2066 6f72 2075  ves a room for u
+000038c0: 7469 6c69 7a69 6e67 0a4f 4d4c 2077 6974  tilizing.OML wit
+000038d0: 6820 796f 7572 2066 6176 6f75 7269 7465  h your favourite
+000038e0: 2066 7261 6d65 776f 726b 2061 6674 6572   framework after
+000038f0: 2074 6865 2069 6d70 6c65 6d65 6e74 6174   the implementat
+00003900: 696f 6e20 6f66 2074 6865 206e 6563 6573  ion of the neces
+00003910: 7361 7279 2077 7261 7070 6572 732e 0a0a  sary wrappers...
+00003920: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
+00003930: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
+00003940: 6d61 7279 3e43 616e 2049 2075 7365 204f  mary>Can I use O
+00003950: 4d4c 2077 6974 686f 7574 2061 6e79 206b  ML without any k
+00003960: 6e6f 776c 6564 6765 2069 6e20 4461 7461  nowledge in Data
+00003970: 5363 6965 6e63 653f 3c2f 7375 6d6d 6172  Science?</summar
+00003980: 793e 0a3c 703e 0a0a 5965 732e 2054 6f20  y>.<p>..Yes. To 
+00003990: 7275 6e20 7468 6520 6578 7065 7269 6d65  run the experime
+000039a0: 6e74 2077 6974 6820 5b50 6970 656c 696e  nt with [Pipelin
+000039b0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+000039c0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
+000039d0: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+000039e0: 6e69 6e67 2f62 6c6f 622f 6d61 696e 2f70  ning/blob/main/p
+000039f0: 6970 656c 696e 6573 2f29 0a79 6f75 206f  ipelines/).you o
+00003a00: 6e6c 7920 6e65 6564 2074 6f20 7772 6974  nly need to writ
+00003a10: 6520 6120 636f 6e76 6572 7465 720a 746f  e a converter.to
+00003a20: 206f 7572 2066 6f72 6d61 7420 2869 7420   our format (it 
+00003a30: 6d65 616e 7320 7072 6570 6172 696e 6720  means preparing 
+00003a40: 7468 650a 602e 6373 7660 2074 6162 6c65  the.`.csv` table
+00003a50: 2077 6974 6820 3520 7072 6564 6566 696e   with 5 predefin
+00003a60: 6564 2063 6f6c 756d 6e73 292e 0a54 6861  ed columns)..Tha
+00003a70: 7427 7320 6974 210a 0a50 726f 6261 626c  t's it!..Probabl
+00003a80: 7920 7765 2061 6c72 6561 6479 2068 6176  y we already hav
+00003a90: 6520 6120 7375 6974 6162 6c65 2070 7265  e a suitable pre
+00003aa0: 2d74 7261 696e 6564 206d 6f64 656c 2066  -trained model f
+00003ab0: 6f72 2079 6f75 7220 646f 6d61 696e 0a69  or your domain.i
+00003ac0: 6e20 6f75 7220 2a4d 6f64 656c 7320 5a6f  n our *Models Zo
+00003ad0: 6f2a 2e20 496e 2074 6869 7320 6361 7365  o*. In this case
+00003ae0: 2c20 796f 7520 646f 6e27 7420 6576 656e  , you don't even
+00003af0: 206e 6565 6420 746f 2074 7261 696e 2069   need to train i
+00003b00: 742e 0a3c 2f70 3e0a 3c2f 6465 7461 696c  t..</p>.</detail
+00003b10: 733e 0a0a 2323 205b 446f 6375 6d65 6e74  s>..## [Document
+00003b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+00003b30: 7065 6e2d 6d65 7472 6963 2d6c 6561 726e  pen-metric-learn
+00003b40: 696e 672e 7265 6164 7468 6564 6f63 732e  ing.readthedocs.
+00003b50: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
+00003b60: 6578 2e68 746d 6c29 0a0a 446f 6375 6d65  ex.html)..Docume
+00003b70: 6e74 6174 696f 6e20 6973 2061 7661 696c  ntation is avail
+00003b80: 6162 6c65 2076 6961 2074 6865 205b 6c69  able via the [li
+00003b90: 6e6b 5d28 6874 7470 733a 2f2f 6f70 656e  nk](https://open
+00003ba0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00003bb0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003bc0: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
+00003bd0: 6874 6d6c 292e 0a0a 596f 7520 6361 6e20  html)...You can 
+00003be0: 616c 736f 2072 6561 6420 736f 6d65 2065  also read some e
+00003bf0: 7874 7261 206d 6174 6572 6961 6c73 2072  xtra materials r
+00003c00: 656c 6174 6564 2074 6f20 4f4d 4c3a 0a0a  elated to OML:..
+00003c10: 2a20 5468 656f 7279 2061 6e64 2070 7261  * Theory and pra
+00003c20: 6374 6963 6520 6f66 206d 6574 7269 6320  ctice of metric 
+00003c30: 6c65 6172 6e69 6e67 2077 6974 6820 7468  learning with th
+00003c40: 6520 7573 6167 6520 6f66 204f 4d4c 2e0a  e usage of OML..
+00003c50: 5b50 6f73 7420 696e 2045 6e67 6c69 7368  [Post in English
+00003c60: 206f 6e20 4d65 6469 756d 5d28 6874 7470   on Medium](http
+00003c70: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f40  s://medium.com/@
+00003c80: 416c 656b 7365 6953 6861 6261 6e6f 762f  AlekseiShabanov/
+00003c90: 7072 6163 7469 6361 6c2d 6d65 7472 6963  practical-metric
+00003ca0: 2d6c 6561 726e 696e 672d 6230 3431 3063  -learning-b0410c
+00003cb0: 6461 3232 3031 2920 7c0a 5b50 6f73 7420  da2201) |.[Post 
+00003cc0: 696e 2052 7573 7369 616e 206f 6e20 4861  in Russian on Ha
+00003cd0: 6272 5d28 6874 7470 733a 2f2f 6861 6272  br](https://habr
+00003ce0: 2e63 6f6d 2f72 752f 636f 6d70 616e 792f  .com/ru/company/
+00003cf0: 6f64 732f 626c 6f67 2f36 3935 3338 302f  ods/blog/695380/
+00003d00: 2920 7c0a 5b50 6f73 7420 696e 2043 6869  ) |.[Post in Chi
+00003d10: 6e65 7365 206f 6e20 4353 444e 5d28 6874  nese on CSDN](ht
+00003d20: 7470 733a 2f2f 626c 6f67 2e63 7364 6e2e  tps://blog.csdn.
+00003d30: 6e65 742f 6665 726d 696f 6e30 3231 372f  net/fermion0217/
+00003d40: 6172 7469 636c 652f 6465 7461 696c 732f  article/details/
+00003d50: 3132 3739 3332 3038 3729 2c20 7472 616e  127932087), tran
+00003d60: 736c 6174 6564 2062 7920 4368 6961 2d43  slated by Chia-C
+00003d70: 6865 6e20 4368 616e 672e 0a0a 2a20 5468  hen Chang...* Th
+00003d80: 650a 5b44 454d 4f5d 2868 7474 7073 3a2f  e.[DEMO](https:/
+00003d90: 2f64 6170 6c61 646f 632d 6f6d 6c2d 706f  /dapladoc-oml-po
+00003da0: 7374 7072 6f63 6573 7369 6e67 2d64 656d  stprocessing-dem
+00003db0: 6f2d 7372 6361 7070 6d61 696e 2d70 6668  o-srcappmain-pfh
+00003dc0: 3267 302e 7374 7265 616d 6c69 742e 6170  2g0.streamlit.ap
+00003dd0: 702f 290a 666f 7220 6f75 7220 7061 7065  p/).for our pape
+00003de0: 720a 5b53 5449 523a 2053 6961 6d65 7365  r.[STIR: Siamese
+00003df0: 2054 7261 6e73 666f 726d 6572 7320 666f   Transformers fo
+00003e00: 7220 496d 6167 6520 5265 7472 6965 7661  r Image Retrieva
+00003e10: 6c20 506f 7374 7072 6f63 6573 7369 6e67  l Postprocessing
+00003e20: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00003e30: 6f72 672f 6162 732f 3233 3034 2e31 3333  org/abs/2304.133
+00003e40: 3933 290a 0a2a 2054 6865 2072 6570 6f72  93)..* The repor
+00003e50: 7420 666f 7220 4265 726c 696e 2d62 6173  t for Berlin-bas
+00003e60: 6564 206d 6565 7475 703a 2022 436f 6d70  ed meetup: "Comp
+00003e70: 7574 6572 2056 6973 696f 6e20 696e 2070  uter Vision in p
+00003e80: 726f 6475 6374 696f 6e22 2e20 4e6f 7665  roduction". Nove
+00003e90: 6d62 6572 2c20 3230 3232 2e0a 5b4c 696e  mber, 2022..[Lin
+00003ea0: 6b5d 2868 7474 7073 3a2f 2f64 7269 7665  k](https://drive
+00003eb0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00003ec0: 652f 666f 6c64 6572 732f 3175 486d 4c55  e/folders/1uHmLU
+00003ed0: 3876 4d72 4d56 4d46 6f64 7433 3675 3075  8vMrMVMFodt36u0u
+00003ee0: 5841 6759 6a47 5f33 4433 303f 7573 703d  XAgYjG_3D30?usp=
+00003ef0: 7368 6172 655f 6c69 6e6b 290a 0a23 2320  share_link)..## 
+00003f00: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2868  [Installation](h
+00003f10: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+00003f20: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+00003f30: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00003f40: 7465 7374 2f6f 6d6c 2f69 6e73 7461 6c6c  test/oml/install
+00003f50: 6174 696f 6e2e 6874 6d6c 290a 0a4f 4d4c  ation.html)..OML
+00003f60: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
+00003f70: 2050 7950 493a 0a0a 6060 6073 6865 6c6c   PyPI:..```shell
+00003f80: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00003f90: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00003fa0: 6e69 6e67 0a60 6060 0a0a 596f 7520 6361  ning.```..You ca
+00003fb0: 6e20 616c 736f 2070 756c 6c20 7468 6520  n also pull the 
+00003fc0: 7072 6570 6172 6564 2069 6d61 6765 2066  prepared image f
+00003fd0: 726f 6d20 446f 636b 6572 4875 622e 2e2e  rom DockerHub...
+00003fe0: 0a0a 6060 6073 6865 6c6c 0a64 6f63 6b65  ..```shell.docke
+00003ff0: 7220 7075 6c6c 206f 6d6c 7465 616d 2f6f  r pull omlteam/o
+00004000: 6d6c 3a67 7075 0a64 6f63 6b65 7220 7075  ml:gpu.docker pu
+00004010: 6c6c 206f 6d6c 7465 616d 2f6f 6d6c 3a63  ll omlteam/oml:c
+00004020: 7075 0a60 6060 0a0a 2e2e 2e6f 7220 6275  pu.```.....or bu
+00004030: 696c 6420 6f6e 6520 6279 2079 6f75 7220  ild one by your 
+00004040: 6f77 6e0a 0a60 6060 7368 656c 6c0a 6d61  own..```shell.ma
+00004050: 6b65 2064 6f63 6b65 725f 6275 696c 6420  ke docker_build 
+00004060: 5255 4e54 494d 453d 6370 750a 6d61 6b65  RUNTIME=cpu.make
+00004070: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
+00004080: 4e54 494d 453d 6770 750a 6060 600a 0a23  NTIME=gpu.```..#
+00004090: 2320 5b45 7861 6d70 6c65 735d 2868 7474  # [Examples](htt
+000040a0: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
+000040b0: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
+000040c0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000040d0: 7374 2f66 6561 7475 7265 5f65 7874 7261  st/feature_extra
+000040e0: 6374 696f 6e2f 7079 7468 6f6e 5f65 7861  ction/python_exa
+000040f0: 6d70 6c65 732e 6874 6d6c 2329 0a0a 3c64  mples.html#)..<d
+00004100: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00004110: 3e54 7261 696e 696e 673c 2f73 756d 6d61  >Training</summa
+00004120: 7279 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e  ry>.<p>..[commen
+00004130: 745d 3a76 616e 696c 6c61 2d74 7261 696e  t]:vanilla-train
+00004140: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
+00004150: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
+00004160: 6f6d 2074 7164 6d20 696d 706f 7274 2074  om tqdm import t
+00004170: 7164 6d0a 0a66 726f 6d20 6f6d 6c2e 6461  qdm..from oml.da
+00004180: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00004190: 7274 2044 6174 6173 6574 5769 7468 4c61  rt DatasetWithLa
+000041a0: 6265 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f  bels.from oml.lo
+000041b0: 7373 6573 2e74 7269 706c 6574 2069 6d70  sses.triplet imp
+000041c0: 6f72 7420 5472 6970 6c65 744c 6f73 7357  ort TripletLossW
+000041d0: 6974 684d 696e 6572 0a66 726f 6d20 6f6d  ithMiner.from om
+000041e0: 6c2e 6d69 6e65 7273 2e69 6e62 6174 6368  l.miners.inbatch
+000041f0: 5f61 6c6c 5f74 7269 2069 6d70 6f72 7420  _all_tri import 
+00004200: 416c 6c54 7269 706c 6574 734d 696e 6572  AllTripletsMiner
 00004210: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
 00004220: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00004230: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7574  ctor.from oml.ut
-00004240: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
-00004250: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
-00004260: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
-00004270: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
-00004280: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
-00004290: 6173 6574 2f22 0a5f 2c20 6466 5f76 616c  aset/"._, df_val
-000042a0: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-000042b0: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-000042c0: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-000042d0: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-000042e0: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-000042f0: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-00004300: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00004310: 733d 4661 6c73 6529 2e65 7661 6c28 290a  s=False).eval().
-00004320: 0a76 616c 5f64 6174 6173 6574 203d 2044  .val_dataset = D
-00004330: 6174 6173 6574 5175 6572 7947 616c 6c65  atasetQueryGalle
-00004340: 7279 2864 665f 7661 6c2c 2064 6174 6173  ry(df_val, datas
-00004350: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00004360: 726f 6f74 290a 0a76 616c 5f6c 6f61 6465  root)..val_loade
-00004370: 7220 3d20 746f 7263 682e 7574 696c 732e  r = torch.utils.
-00004380: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
-00004390: 7661 6c5f 6461 7461 7365 742c 2062 6174  val_dataset, bat
-000043a0: 6368 5f73 697a 653d 3429 0a63 616c 6375  ch_size=4).calcu
-000043b0: 6c61 746f 7220 3d20 456d 6265 6464 696e  lator = Embeddin
-000043c0: 674d 6574 7269 6373 2865 7874 7261 5f6b  gMetrics(extra_k
-000043d0: 6579 733d 2822 7061 7468 7322 2c29 290a  eys=("paths",)).
-000043e0: 6361 6c63 756c 6174 6f72 2e73 6574 7570  calculator.setup
-000043f0: 286e 756d 5f73 616d 706c 6573 3d6c 656e  (num_samples=len
-00004400: 2876 616c 5f64 6174 6173 6574 2929 0a0a  (val_dataset))..
-00004410: 7769 7468 2074 6f72 6368 2e6e 6f5f 6772  with torch.no_gr
-00004420: 6164 2829 3a0a 2020 2020 666f 7220 6261  ad():.    for ba
-00004430: 7463 6820 696e 2074 7164 6d28 7661 6c5f  tch in tqdm(val_
-00004440: 6c6f 6164 6572 293a 0a20 2020 2020 2020  loader):.       
-00004450: 2062 6174 6368 5b22 656d 6265 6464 696e   batch["embeddin
-00004460: 6773 225d 203d 2065 7874 7261 6374 6f72  gs"] = extractor
-00004470: 2862 6174 6368 5b22 696e 7075 745f 7465  (batch["input_te
-00004480: 6e73 6f72 7322 5d29 0a20 2020 2020 2020  nsors"]).       
-00004490: 2063 616c 6375 6c61 746f 722e 7570 6461   calculator.upda
-000044a0: 7465 5f64 6174 6128 6261 7463 6829 0a0a  te_data(batch)..
-000044b0: 6d65 7472 6963 7320 3d20 6361 6c63 756c  metrics = calcul
-000044c0: 6174 6f72 2e63 6f6d 7075 7465 5f6d 6574  ator.compute_met
-000044d0: 7269 6373 2829 0a0a 2320 4c6f 6767 696e  rics()..# Loggin
-000044e0: 670a 7072 696e 7428 6361 6c63 756c 6174  g.print(calculat
-000044f0: 6f72 2e6d 6574 7269 6373 2920 2023 206d  or.metrics)  # m
-00004500: 6574 7269 6373 0a70 7269 6e74 2863 616c  etrics.print(cal
-00004510: 6375 6c61 746f 722e 6d65 7472 6963 735f  culator.metrics_
-00004520: 756e 7265 6475 6365 6429 2020 2320 6d65  unreduced)  # me
-00004530: 7472 6963 7320 7769 7468 6f75 7420 6176  trics without av
-00004540: 6572 6167 696e 6720 6f76 6572 2071 7565  eraging over que
-00004550: 7269 6573 0a0a 2320 5669 7375 616c 6973  ries..# Visualis
-00004560: 6174 696f 6e0a 6361 6c63 756c 6174 6f72  ation.calculator
-00004570: 2e67 6574 5f70 6c6f 745f 666f 725f 7175  .get_plot_for_qu
-00004580: 6572 6965 7328 7175 6572 795f 6964 733d  eries(query_ids=
-00004590: 5b30 2c20 325d 2c20 6e5f 696e 7374 616e  [0, 2], n_instan
-000045a0: 6365 733d 3529 2020 2320 6472 6177 2070  ces=5)  # draw p
-000045b0: 7265 6469 6374 696f 6e73 206f 6e20 7072  redictions on pr
-000045c0: 6564 6566 696e 6564 2071 7565 7269 6573  edefined queries
-000045d0: 0a63 616c 6375 6c61 746f 722e 6765 745f  .calculator.get_
-000045e0: 706c 6f74 5f66 6f72 5f77 6f72 7374 5f71  plot_for_worst_q
-000045f0: 7565 7269 6573 286d 6574 7269 635f 6e61  ueries(metric_na
-00004600: 6d65 3d22 4f56 4552 414c 4c2f 6d61 702f  me="OVERALL/map/
-00004610: 3522 2c20 6e5f 7175 6572 6965 733d 322c  5", n_queries=2,
-00004620: 206e 5f69 6e73 7461 6e63 6573 3d35 2920   n_instances=5) 
-00004630: 2023 2064 7261 7720 6d69 7374 616b 6573   # draw mistakes
-00004640: 0a63 616c 6375 6c61 746f 722e 7669 7375  .calculator.visu
-00004650: 616c 697a 6528 2920 2023 2064 7261 7720  alize()  # draw 
-00004660: 6d69 7374 616b 6573 2066 6f72 2061 6c6c  mistakes for all
-00004670: 2074 6865 2061 7661 696c 6162 6c65 206d   the available m
-00004680: 6574 7269 6373 0a0a 6060 600a 5b63 6f6d  etrics..```.[com
-00004690: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
-000046a0: 6c69 6461 7469 6f6e 2d65 6e64 0a3c 2f70  lidation-end.</p
-000046b0: 3e0a 3c2f 6465 7461 696c 733e 0a0a 5b21  >.</details>..[!
-000046c0: 5b4f 7065 6e20 496e 2043 6f6c 6162 5d28  [Open In Colab](
-000046d0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-000046e0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-000046f0: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
-00004700: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00004710: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00004720: 682e 676f 6f67 6c65 2e63 6f6d 2f64 7269  h.google.com/dri
-00004730: 7665 2f31 4f32 6f33 6b38 4938 6a4e 3568  ve/1O2o3k8I8jN5h
-00004740: 5269 6e33 644b 6e41 5333 5773 6747 3034  Rin3dKnAS3WsgG04
-00004750: 746d 4954 3f75 7370 3d73 6861 7269 6e67  tmIT?usp=sharing
-00004760: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
-00004770: 6d61 7279 3e54 7261 696e 696e 6720 2b20  mary>Training + 
-00004780: 5661 6c69 6461 7469 6f6e 205b 4c69 6768  Validation [Ligh
-00004790: 746e 696e 6720 616e 6420 4e65 7074 756e  tning and Neptun
-000047a0: 6520 6c6f 6767 696e 675d 3c2f 7375 6d6d  e logging]</summ
-000047b0: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-000047c0: 6e74 5d3a 6c69 6768 746e 696e 672d 7374  nt]:lightning-st
-000047d0: 6172 740a 6060 6070 7974 686f 6e0a 696d  art.```python.im
-000047e0: 706f 7274 2070 7974 6f72 6368 5f6c 6967  port pytorch_lig
-000047f0: 6874 6e69 6e67 2061 7320 706c 0a69 6d70  htning as pl.imp
-00004800: 6f72 7420 746f 7263 680a 0a66 726f 6d20  ort torch..from 
-00004810: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-00004820: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-00004830: 5175 6572 7947 616c 6c65 7279 2c20 4461  QueryGallery, Da
-00004840: 7461 7365 7457 6974 684c 6162 656c 730a  tasetWithLabels.
-00004850: 6672 6f6d 206f 6d6c 2e6c 6967 6874 6e69  from oml.lightni
-00004860: 6e67 2e6d 6f64 756c 6573 2e65 7874 7261  ng.modules.extra
-00004870: 6374 6f72 2069 6d70 6f72 7420 4578 7472  ctor import Extr
-00004880: 6163 746f 724d 6f64 756c 650a 6672 6f6d  actorModule.from
-00004890: 206f 6d6c 2e6c 6967 6874 6e69 6e67 2e63   oml.lightning.c
-000048a0: 616c 6c62 6163 6b73 2e6d 6574 7269 6320  allbacks.metric 
-000048b0: 696d 706f 7274 204d 6574 7269 6356 616c  import MetricVal
-000048c0: 4361 6c6c 6261 636b 0a66 726f 6d20 6f6d  Callback.from om
-000048d0: 6c2e 6c6f 7373 6573 2e74 7269 706c 6574  l.losses.triplet
-000048e0: 2069 6d70 6f72 7420 5472 6970 6c65 744c   import TripletL
-000048f0: 6f73 7357 6974 684d 696e 6572 0a66 726f  ossWithMiner.fro
-00004900: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-00004910: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00004920: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
-00004930: 0a66 726f 6d20 6f6d 6c2e 6d69 6e65 7273  .from oml.miners
-00004940: 2e69 6e62 6174 6368 5f61 6c6c 5f74 7269  .inbatch_all_tri
-00004950: 2069 6d70 6f72 7420 416c 6c54 7269 706c   import AllTripl
-00004960: 6574 734d 696e 6572 0a66 726f 6d20 6f6d  etsMiner.from om
-00004970: 6c2e 6d6f 6465 6c73 2069 6d70 6f72 7420  l.models import 
-00004980: 5669 5445 7874 7261 6374 6f72 0a66 726f  ViTExtractor.fro
-00004990: 6d20 6f6d 6c2e 7361 6d70 6c65 7273 2e62  m oml.samplers.b
-000049a0: 616c 616e 6365 2069 6d70 6f72 7420 4261  alance import Ba
-000049b0: 6c61 6e63 6553 616d 706c 6572 0a66 726f  lanceSampler.fro
-000049c0: 6d20 6f6d 6c2e 7574 696c 732e 646f 776e  m oml.utils.down
-000049d0: 6c6f 6164 5f6d 6f63 6b5f 6461 7461 7365  load_mock_datase
-000049e0: 7420 696d 706f 7274 2064 6f77 6e6c 6f61  t import downloa
-000049f0: 645f 6d6f 636b 5f64 6174 6173 6574 0a66  d_mock_dataset.f
-00004a00: 726f 6d20 7079 746f 7263 685f 6c69 6768  rom pytorch_ligh
-00004a10: 746e 696e 672e 6c6f 6767 6572 7320 696d  tning.loggers im
-00004a20: 706f 7274 204e 6570 7475 6e65 4c6f 6767  port NeptuneLogg
-00004a30: 6572 2c20 5465 6e73 6f72 426f 6172 644c  er, TensorBoardL
-00004a40: 6f67 6765 720a 0a64 6174 6173 6574 5f72  ogger..dataset_r
-00004a50: 6f6f 7420 3d20 226d 6f63 6b5f 6461 7461  oot = "mock_data
-00004a60: 7365 742f 220a 6466 5f74 7261 696e 2c20  set/".df_train, 
-00004a70: 6466 5f76 616c 203d 2064 6f77 6e6c 6f61  df_val = downloa
-00004a80: 645f 6d6f 636b 5f64 6174 6173 6574 2864  d_mock_dataset(d
-00004a90: 6174 6173 6574 5f72 6f6f 7429 0a0a 2320  ataset_root)..# 
-00004aa0: 6d6f 6465 6c0a 6578 7472 6163 746f 7220  model.extractor 
-00004ab0: 3d20 5669 5445 7874 7261 6374 6f72 2822  = ViTExtractor("
-00004ac0: 7669 7473 3136 5f64 696e 6f22 2c20 6172  vits16_dino", ar
-00004ad0: 6368 3d22 7669 7473 3136 222c 206e 6f72  ch="vits16", nor
-00004ae0: 6d61 6c69 7365 5f66 6561 7475 7265 733d  malise_features=
-00004af0: 4661 6c73 6529 0a0a 2320 7472 6169 6e0a  False)..# train.
-00004b00: 6f70 7469 6d69 7a65 7220 3d20 746f 7263  optimizer = torc
-00004b10: 682e 6f70 7469 6d2e 5347 4428 6578 7472  h.optim.SGD(extr
-00004b20: 6163 746f 722e 7061 7261 6d65 7465 7273  actor.parameters
-00004b30: 2829 2c20 6c72 3d31 652d 3629 0a74 7261  (), lr=1e-6).tra
-00004b40: 696e 5f64 6174 6173 6574 203d 2044 6174  in_dataset = Dat
-00004b50: 6173 6574 5769 7468 4c61 6265 6c73 2864  asetWithLabels(d
-00004b60: 665f 7472 6169 6e2c 2064 6174 6173 6574  f_train, dataset
-00004b70: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-00004b80: 6f74 290a 6372 6974 6572 696f 6e20 3d20  ot).criterion = 
-00004b90: 5472 6970 6c65 744c 6f73 7357 6974 684d  TripletLossWithM
-00004ba0: 696e 6572 286d 6172 6769 6e3d 302e 312c  iner(margin=0.1,
-00004bb0: 206d 696e 6572 3d41 6c6c 5472 6970 6c65   miner=AllTriple
-00004bc0: 7473 4d69 6e65 7228 2929 0a62 6174 6368  tsMiner()).batch
-00004bd0: 5f73 616d 706c 6572 203d 2042 616c 616e  _sampler = Balan
-00004be0: 6365 5361 6d70 6c65 7228 7472 6169 6e5f  ceSampler(train_
-00004bf0: 6461 7461 7365 742e 6765 745f 6c61 6265  dataset.get_labe
-00004c00: 6c73 2829 2c20 6e5f 6c61 6265 6c73 3d32  ls(), n_labels=2
-00004c10: 2c20 6e5f 696e 7374 616e 6365 733d 3329  , n_instances=3)
-00004c20: 0a74 7261 696e 5f6c 6f61 6465 7220 3d20  .train_loader = 
-00004c30: 746f 7263 682e 7574 696c 732e 6461 7461  torch.utils.data
-00004c40: 2e44 6174 614c 6f61 6465 7228 7472 6169  .DataLoader(trai
-00004c50: 6e5f 6461 7461 7365 742c 2062 6174 6368  n_dataset, batch
-00004c60: 5f73 616d 706c 6572 3d62 6174 6368 5f73  _sampler=batch_s
-00004c70: 616d 706c 6572 290a 0a23 2076 616c 0a76  ampler)..# val.v
-00004c80: 616c 5f64 6174 6173 6574 203d 2044 6174  al_dataset = Dat
-00004c90: 6173 6574 5175 6572 7947 616c 6c65 7279  asetQueryGallery
-00004ca0: 2864 665f 7661 6c2c 2064 6174 6173 6574  (df_val, dataset
-00004cb0: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-00004cc0: 6f74 290a 7661 6c5f 6c6f 6164 6572 203d  ot).val_loader =
-00004cd0: 2074 6f72 6368 2e75 7469 6c73 2e64 6174   torch.utils.dat
-00004ce0: 612e 4461 7461 4c6f 6164 6572 2876 616c  a.DataLoader(val
-00004cf0: 5f64 6174 6173 6574 2c20 6261 7463 685f  _dataset, batch_
-00004d00: 7369 7a65 3d34 290a 6d65 7472 6963 5f63  size=4).metric_c
-00004d10: 616c 6c62 6163 6b20 3d20 4d65 7472 6963  allback = Metric
-00004d20: 5661 6c43 616c 6c62 6163 6b28 6d65 7472  ValCallback(metr
-00004d30: 6963 3d45 6d62 6564 6469 6e67 4d65 7472  ic=EmbeddingMetr
-00004d40: 6963 7328 6578 7472 615f 6b65 7973 3d5b  ics(extra_keys=[
-00004d50: 7472 6169 6e5f 6461 7461 7365 742e 7061  train_dataset.pa
-00004d60: 7468 735f 6b65 792c 5d29 2c20 6c6f 675f  ths_key,]), log_
-00004d70: 696d 6167 6573 3d54 7275 6529 0a0a 2320  images=True)..# 
-00004d80: 6c6f 6767 696e 670a 6c6f 6767 6572 203d  logging.logger =
-00004d90: 2054 656e 736f 7242 6f61 7264 4c6f 6767   TensorBoardLogg
-00004da0: 6572 2822 2e22 2920 2023 2046 6f72 2054  er(".")  # For T
-00004db0: 656e 736f 7242 6f61 7264 0a23 206c 6f67  ensorBoard.# log
-00004dc0: 6765 7220 3d20 4e65 7074 756e 654c 6f67  ger = NeptuneLog
-00004dd0: 6765 7228 6170 695f 6b65 793d 2222 2c20  ger(api_key="", 
-00004de0: 7072 6f6a 6563 743d 2222 2c20 6c6f 675f  project="", log_
-00004df0: 6d6f 6465 6c5f 6368 6563 6b70 6f69 6e74  model_checkpoint
-00004e00: 733d 4661 6c73 6529 2020 2320 466f 7220  s=False)  # For 
-00004e10: 4e65 7074 756e 650a 0a23 2072 756e 0a70  Neptune..# run.p
-00004e20: 6c5f 6d6f 6465 6c20 3d20 4578 7472 6163  l_model = Extrac
-00004e30: 746f 724d 6f64 756c 6528 6578 7472 6163  torModule(extrac
-00004e40: 746f 722c 2063 7269 7465 7269 6f6e 2c20  tor, criterion, 
-00004e50: 6f70 7469 6d69 7a65 7229 0a74 7261 696e  optimizer).train
-00004e60: 6572 203d 2070 6c2e 5472 6169 6e65 7228  er = pl.Trainer(
-00004e70: 6d61 785f 6570 6f63 6873 3d33 2c20 6361  max_epochs=3, ca
-00004e80: 6c6c 6261 636b 733d 5b6d 6574 7269 635f  llbacks=[metric_
-00004e90: 6361 6c6c 6261 636b 5d2c 206e 756d 5f73  callback], num_s
-00004ea0: 616e 6974 795f 7661 6c5f 7374 6570 733d  anity_val_steps=
-00004eb0: 302c 206c 6f67 6765 723d 6c6f 6767 6572  0, logger=logger
-00004ec0: 290a 7472 6169 6e65 722e 6669 7428 706c  ).trainer.fit(pl
-00004ed0: 5f6d 6f64 656c 2c20 7472 6169 6e5f 6461  _model, train_da
-00004ee0: 7461 6c6f 6164 6572 733d 7472 6169 6e5f  taloaders=train_
-00004ef0: 6c6f 6164 6572 2c20 7661 6c5f 6461 7461  loader, val_data
-00004f00: 6c6f 6164 6572 733d 7661 6c5f 6c6f 6164  loaders=val_load
-00004f10: 6572 290a 0a60 6060 0a5b 636f 6d6d 656e  er)..```.[commen
-00004f20: 745d 3a6c 6967 6874 6e69 6e67 2d65 6e64  t]:lightning-end
-00004f30: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-00004f40: 0a0a 5b21 5b4f 7065 6e20 496e 2043 6f6c  ..[![Open In Col
-00004f50: 6162 5d28 6874 7470 733a 2f2f 636f 6c61  ab](https://cola
-00004f60: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00004f70: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
-00004f80: 6162 2d62 6164 6765 2e73 7667 295d 2868  ab-badge.svg)](h
-00004f90: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00004fa0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00004fb0: 2f64 7269 7665 2f31 6256 5567 6442 4757  /drive/1bVUgdBGW
-00004fc0: 7651 6743 6b62 6132 5974 6149 5256 6c55  vQgCkba2YtaIRVlU
-00004fd0: 5155 7a37 5136 305a 3f75 7370 3d73 6861  QUz7Q60Z?usp=sha
-00004fe0: 7265 5f6c 696e 6b29 0a3c 6465 7461 696c  re_link).<detail
-00004ff0: 733e 0a3c 7375 6d6d 6172 793e 5573 696e  s>.<summary>Usin
-00005000: 6720 6120 7472 6169 6e65 6420 6d6f 6465  g a trained mode
-00005010: 6c20 666f 7220 7265 7472 6965 7661 6c3c  l for retrieval<
-00005020: 2f73 756d 6d61 7279 3e0a 3c70 3e0a 0a5b  /summary>.<p>..[
-00005030: 636f 6d6d 656e 745d 3a75 7361 6765 2d72  comment]:usage-r
-00005040: 6574 7269 6576 616c 2d73 7461 7274 0a60  etrieval-start.`
-00005050: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00005060: 746f 7263 680a 0a66 726f 6d20 6f6d 6c2e  torch..from oml.
-00005070: 636f 6e73 7420 696d 706f 7274 204d 4f43  const import MOC
-00005080: 4b5f 4441 5441 5345 545f 5041 5448 0a66  K_DATASET_PATH.f
-00005090: 726f 6d20 6f6d 6c2e 696e 6665 7265 6e63  rom oml.inferenc
-000050a0: 652e 666c 6174 2069 6d70 6f72 7420 696e  e.flat import in
-000050b0: 6665 7265 6e63 655f 6f6e 5f69 6d61 6765  ference_on_image
-000050c0: 730a 6672 6f6d 206f 6d6c 2e6d 6f64 656c  s.from oml.model
-000050d0: 7320 696d 706f 7274 2056 6954 4578 7472  s import ViTExtr
-000050e0: 6163 746f 720a 6672 6f6d 206f 6d6c 2e72  actor.from oml.r
-000050f0: 6567 6973 7472 792e 7472 616e 7366 6f72  egistry.transfor
-00005100: 6d73 2069 6d70 6f72 7420 6765 745f 7472  ms import get_tr
-00005110: 616e 7366 6f72 6d73 5f66 6f72 5f70 7265  ansforms_for_pre
-00005120: 7472 6169 6e65 640a 6672 6f6d 206f 6d6c  trained.from oml
-00005130: 2e75 7469 6c73 2e64 6f77 6e6c 6f61 645f  .utils.download_
-00005140: 6d6f 636b 5f64 6174 6173 6574 2069 6d70  mock_dataset imp
-00005150: 6f72 7420 646f 776e 6c6f 6164 5f6d 6f63  ort download_moc
-00005160: 6b5f 6461 7461 7365 740a 6672 6f6d 206f  k_dataset.from o
-00005170: 6d6c 2e75 7469 6c73 2e6d 6973 635f 746f  ml.utils.misc_to
-00005180: 7263 6820 696d 706f 7274 2070 6169 7277  rch import pairw
-00005190: 6973 655f 6469 7374 0a0a 5f2c 2064 665f  ise_dist.._, df_
-000051a0: 7661 6c20 3d20 646f 776e 6c6f 6164 5f6d  val = download_m
-000051b0: 6f63 6b5f 6461 7461 7365 7428 4d4f 434b  ock_dataset(MOCK
-000051c0: 5f44 4154 4153 4554 5f50 4154 4829 0a64  _DATASET_PATH).d
-000051d0: 665f 7661 6c5b 2270 6174 6822 5d20 3d20  f_val["path"] = 
-000051e0: 6466 5f76 616c 5b22 7061 7468 225d 2e61  df_val["path"].a
-000051f0: 7070 6c79 286c 616d 6264 6120 783a 204d  pply(lambda x: M
-00005200: 4f43 4b5f 4441 5441 5345 545f 5041 5448  OCK_DATASET_PATH
-00005210: 202f 2078 290a 7175 6572 6965 7320 3d20   / x).queries = 
-00005220: 6466 5f76 616c 5b64 665f 7661 6c5b 2269  df_val[df_val["i
-00005230: 735f 7175 6572 7922 5d5d 5b22 7061 7468  s_query"]]["path
-00005240: 225d 2e74 6f6c 6973 7428 290a 6761 6c6c  "].tolist().gall
-00005250: 6572 6965 7320 3d20 6466 5f76 616c 5b64  eries = df_val[d
-00005260: 665f 7661 6c5b 2269 735f 6761 6c6c 6572  f_val["is_galler
-00005270: 7922 5d5d 5b22 7061 7468 225d 2e74 6f6c  y"]]["path"].tol
-00005280: 6973 7428 290a 0a65 7874 7261 6374 6f72  ist()..extractor
-00005290: 203d 2056 6954 4578 7472 6163 746f 722e   = ViTExtractor.
-000052a0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-000052b0: 2276 6974 7331 365f 6469 6e6f 2229 0a74  "vits16_dino").t
-000052c0: 7261 6e73 666f 726d 2c20 5f20 3d20 6765  ransform, _ = ge
-000052d0: 745f 7472 616e 7366 6f72 6d73 5f66 6f72  t_transforms_for
-000052e0: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-000052f0: 7331 365f 6469 6e6f 2229 0a0a 6172 6773  s16_dino")..args
-00005300: 203d 207b 226e 756d 5f77 6f72 6b65 7273   = {"num_workers
-00005310: 223a 2030 2c20 2262 6174 6368 5f73 697a  ": 0, "batch_siz
-00005320: 6522 3a20 387d 0a66 6561 7475 7265 735f  e": 8}.features_
-00005330: 7175 6572 6965 7320 3d20 696e 6665 7265  queries = infere
-00005340: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-00005350: 7472 6163 746f 722c 2070 6174 6873 3d71  tractor, paths=q
-00005360: 7565 7269 6573 2c20 7472 616e 7366 6f72  ueries, transfor
-00005370: 6d3d 7472 616e 7366 6f72 6d2c 202a 2a61  m=transform, **a
-00005380: 7267 7329 0a66 6561 7475 7265 735f 6761  rgs).features_ga
-00005390: 6c6c 6572 6965 7320 3d20 696e 6665 7265  lleries = infere
-000053a0: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-000053b0: 7472 6163 746f 722c 2070 6174 6873 3d67  tractor, paths=g
-000053c0: 616c 6c65 7269 6573 2c20 7472 616e 7366  alleries, transf
-000053d0: 6f72 6d3d 7472 616e 7366 6f72 6d2c 202a  orm=transform, *
-000053e0: 2a61 7267 7329 0a0a 2320 4e6f 7720 7765  *args)..# Now we
-000053f0: 2063 616e 2065 7870 6c69 6369 746c 7920   can explicitly 
-00005400: 6275 696c 6420 7061 6972 7769 7365 206d  build pairwise m
-00005410: 6174 7269 7820 6f66 2064 6973 7461 6e63  atrix of distanc
-00005420: 6573 206f 7220 7361 7665 2079 6f75 2052  es or save you R
-00005430: 414d 2076 6961 2075 7369 6e67 206b 4e4e  AM via using kNN
-00005440: 0a75 7365 5f6b 6e6e 203d 2054 7275 650a  .use_knn = True.
-00005450: 746f 705f 6b20 3d20 330a 0a69 6620 7573  top_k = 3..if us
-00005460: 655f 6b6e 6e3a 0a20 2020 2066 726f 6d20  e_knn:.    from 
-00005470: 736b 6c65 6172 6e2e 6e65 6967 6862 6f72  sklearn.neighbor
-00005480: 7320 696d 706f 7274 204e 6561 7265 7374  s import Nearest
-00005490: 4e65 6967 6862 6f72 730a 2020 2020 6b6e  Neighbors.    kn
-000054a0: 6e20 3d20 4e65 6172 6573 744e 6569 6768  n = NearestNeigh
-000054b0: 626f 7273 2861 6c67 6f72 6974 686d 3d22  bors(algorithm="
-000054c0: 6175 746f 222c 2070 3d32 290a 2020 2020  auto", p=2).    
-000054d0: 6b6e 6e2e 6669 7428 6665 6174 7572 6573  knn.fit(features
-000054e0: 5f67 616c 6c65 7269 6573 290a 2020 2020  _galleries).    
-000054f0: 6469 7374 732c 2069 695f 636c 6f73 6573  dists, ii_closes
-00005500: 7420 3d20 6b6e 6e2e 6b6e 6569 6768 626f  t = knn.kneighbo
-00005510: 7273 2866 6561 7475 7265 735f 7175 6572  rs(features_quer
-00005520: 6965 732c 206e 5f6e 6569 6768 626f 7273  ies, n_neighbors
-00005530: 3d74 6f70 5f6b 2c20 7265 7475 726e 5f64  =top_k, return_d
-00005540: 6973 7461 6e63 653d 5472 7565 290a 0a65  istance=True)..e
-00005550: 6c73 653a 0a20 2020 2064 6973 745f 6d61  lse:.    dist_ma
-00005560: 7420 3d20 7061 6972 7769 7365 5f64 6973  t = pairwise_dis
-00005570: 7428 7831 3d66 6561 7475 7265 735f 7175  t(x1=features_qu
-00005580: 6572 6965 732c 2078 323d 6665 6174 7572  eries, x2=featur
-00005590: 6573 5f67 616c 6c65 7269 6573 290a 2020  es_galleries).  
-000055a0: 2020 6469 7374 732c 2069 695f 636c 6f73    dists, ii_clos
-000055b0: 6573 7420 3d20 746f 7263 682e 746f 706b  est = torch.topk
-000055c0: 2864 6973 745f 6d61 742c 2064 696d 3d31  (dist_mat, dim=1
-000055d0: 2c20 6b3d 746f 705f 6b2c 206c 6172 6765  , k=top_k, large
-000055e0: 7374 3d46 616c 7365 290a 0a70 7269 6e74  st=False)..print
-000055f0: 2866 2254 6f70 207b 746f 705f 6b7d 2069  (f"Top {top_k} i
-00005600: 7465 6d73 2063 6c6f 7365 7374 2074 6f20  tems closest to 
-00005610: 7175 6572 6965 7320 6172 653a 5c6e 207b  queries are:\n {
-00005620: 6969 5f63 6c6f 7365 7374 7d22 290a 6060  ii_closest}").``
-00005630: 600a 5b63 6f6d 6d65 6e74 5d3a 7573 6167  `.[comment]:usag
-00005640: 652d 7265 7472 6965 7661 6c2d 656e 640a  e-retrieval-end.
-00005650: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
-00005660: 0a5b 215b 4f70 656e 2049 6e20 436f 6c61  .[![Open In Cola
-00005670: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
-00005680: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00005690: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
-000056a0: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
-000056b0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-000056c0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-000056d0: 6472 6976 652f 3153 326e 4b36 4b61 5265  drive/1S2nK6KaRe
-000056e0: 446d 2d52 6a6a 646f 6a64 4964 3643 616b  Dm-RjjdojdId6Cak
-000056f0: 6868 5379 7666 413f 7573 703d 7368 6172  hhSyvfA?usp=shar
-00005700: 655f 6c69 6e6b 290a 0a5b 2a2a 5363 6865  e_link)..[**Sche
-00005710: 6d61 732c 2065 7870 6c61 6e61 7469 6f6e  mas, explanation
-00005720: 7320 616e 6420 7469 7073 2a2a 5d28 6874  s and tips**](ht
-00005730: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005740: 2f4f 4d4c 2d54 6561 6d2f 6f70 656e 2d6d  /OML-Team/open-m
-00005750: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
-00005760: 7265 652f 6d61 696e 2f70 6970 656c 696e  ree/main/pipelin
-00005770: 6573 2f66 6561 7475 7265 735f 6578 7472  es/features_extr
-00005780: 6163 7469 6f6e 290a 0a53 6565 205b 6578  action)..See [ex
-00005790: 7472 6120 636f 6465 2073 6e69 7070 6574  tra code snippet
-000057a0: 735d 2868 7474 7073 3a2f 2f6f 7065 6e2d  s](https://open-
-000057b0: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-000057c0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000057d0: 6e2f 6c61 7465 7374 2f66 6561 7475 7265  n/latest/feature
-000057e0: 5f65 7874 7261 6374 696f 6e2f 7079 7468  _extraction/pyth
-000057f0: 6f6e 5f65 7861 6d70 6c65 732e 6874 6d6c  on_examples.html
-00005800: 292c 2069 6e63 6c75 6469 6e67 3a0a 2a20  ), including:.* 
-00005810: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
-00005820: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
-00005830: 6e69 6e67 0a2a 2054 7261 696e 696e 6720  ning.* Training 
-00005840: 2b20 5661 6c69 6461 7469 6f6e 2077 6974  + Validation wit
-00005850: 6820 4c69 6768 746e 696e 6720 696e 2044  h Lightning in D
-00005860: 4450 206d 6f64 650a 2a20 5472 6169 6e69  DP mode.* Traini
-00005870: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-00005880: 726f 6d20 504d 4c0a 2a20 5472 6169 6e69  rom PML.* Traini
-00005890: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-000058a0: 726f 6d20 504d 4c20 6164 7661 6e63 6564  rom PML advanced
-000058b0: 2028 7061 7373 696e 6720 6469 7374 616e   (passing distan
-000058c0: 6365 2c20 7265 6475 6365 722c 206d 696e  ce, reducer, min
-000058d0: 6572 290a 0a23 2320 5b50 6970 656c 696e  er)..## [Pipelin
-000058e0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000058f0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00005900: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00005910: 6e69 6e67 2f74 7265 652f 6d61 696e 2f70  ning/tree/main/p
-00005920: 6970 656c 696e 6573 290a 0a50 6970 656c  ipelines)..Pipel
-00005930: 696e 6573 2070 726f 7669 6465 2061 2077  ines provide a w
-00005940: 6179 2074 6f20 7275 6e20 6d65 7472 6963  ay to run metric
-00005950: 206c 6561 726e 696e 6720 6578 7065 7269   learning experi
-00005960: 6d65 6e74 7320 7669 6120 6368 616e 6769  ments via changi
-00005970: 6e67 206f 6e6c 7920 7468 6520 636f 6e66  ng only the conf
-00005980: 6967 2066 696c 652e 0a41 6c6c 2079 6f75  ig file..All you
-00005990: 206e 6565 6420 6973 2074 6f20 7072 6570   need is to prep
-000059a0: 6172 6520 796f 7572 2064 6174 6173 6574  are your dataset
-000059b0: 2069 6e20 6120 7265 7175 6972 6564 2066   in a required f
-000059c0: 6f72 6d61 742e 0a0a 5365 6520 5b50 6970  ormat...See [Pip
-000059d0: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-000059e0: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-000059f0: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00005a00: 6c65 6172 6e69 6e67 2f62 6c6f 622f 6d61  learning/blob/ma
-00005a10: 696e 2f70 6970 656c 696e 6573 2f29 2066  in/pipelines/) f
-00005a20: 6f6c 6465 7220 666f 7220 6d6f 7265 2064  older for more d
-00005a30: 6574 6169 6c73 3a0a 2a20 4665 6174 7572  etails:.* Featur
-00005a40: 6520 6578 7472 6163 746f 7220 5b70 6970  e extractor [pip
-00005a50: 656c 696e 655d 2868 7474 7073 3a2f 2f67  eline](https://g
-00005a60: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-00005a70: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-00005a80: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
-00005a90: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
-00005aa0: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
-00005ab0: 0a2a 2052 6574 7269 6576 616c 2070 6f73  .* Retrieval pos
-00005ac0: 7470 726f 6365 7373 6f72 205b 7069 7065  tprocessor [pipe
-00005ad0: 6c69 6e65 5d28 6874 7470 733a 2f2f 6769  line](https://gi
-00005ae0: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
-00005af0: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
-00005b00: 6172 6e69 6e67 2f74 7265 652f 6d61 696e  arning/tree/main
-00005b10: 2f70 6970 656c 696e 6573 2f70 6f73 7470  /pipelines/postp
-00005b20: 726f 6365 7373 696e 6729 2028 7265 2d72  rocessing) (re-r
-00005b30: 616e 6b69 6e67 290a 0a23 2320 5b5a 6f6f  anking)..## [Zoo
-00005b40: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00005b50: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00005b60: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00005b70: 2f6c 6174 6573 742f 6665 6174 7572 655f  /latest/feature_
-00005b80: 6578 7472 6163 7469 6f6e 2f7a 6f6f 2e68  extraction/zoo.h
-00005b90: 746d 6c29 0a0a 4265 6c6f 7720 6172 6520  tml)..Below are 
-00005ba0: 7468 6520 6d6f 6465 6c73 2074 7261 696e  the models train
-00005bb0: 6564 2077 6974 6820 4f4d 4c20 6f6e 2034  ed with OML on 4
-00005bc0: 2070 7562 6c69 6320 6461 7461 7365 7473   public datasets
-00005bd0: 2e0a 416c 6c20 6d65 7472 6963 7320 6265  ..All metrics be
-00005be0: 6c6f 7720 7765 7265 206f 6274 6169 6e65  low were obtaine
-00005bf0: 6420 6f6e 2074 6865 2069 6d61 6765 7320  d on the images 
-00005c00: 7769 7468 2074 6865 2073 697a 6573 206f  with the sizes o
-00005c10: 6620 2a2a 3232 3420 7820 3232 342a 2a3a  f **224 x 224**:
-00005c20: 0a0a 7c20 2020 2020 2020 2020 2020 2020  ..|             
-00005c30: 2020 2020 2020 2020 206d 6f64 656c 2020           model  
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 7c20 636d 6331 2020 7c20 2020      | cmc1  |   
-00005c60: 2020 2020 2020 6461 7461 7365 7420 2020        dataset   
-00005c70: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 7765 6967 6874 7320 2020        weights   
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 6578 7065 7269 6d65 6e74 2020 2020 2020  experiment      
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005d50: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
-00005d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d80: 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 3a2d 2d2d  --:|:-----:|:---
-00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005da0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00005db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e00: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
-00005e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
-00005e80: 7c20 6056 6954 4578 7472 6163 746f 722e  | `ViTExtractor.
-00005e90: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005ea0: 2276 6974 7331 365f 696e 7368 6f70 2229  "vits16_inshop")
-00005eb0: 6020 7c20 302e 3932 3120 7c20 2020 2044  ` | 0.921 |    D
-00005ec0: 6565 7046 6173 6869 6f6e 2049 6e73 686f  eepFashion Insho
-00005ed0: 7020 2020 207c 2020 2020 5b6c 696e 6b5d  p    |    [link]
-00005ee0: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00005ef0: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
-00005f00: 2f31 6e69 582d 5443 3863 6a36 6a33 3639  /1niX-TC8cj6j369
-00005f10: 7437 6955 3262 6148 5153 564e 334d 564a  t7iU2baHQSVN3MVJ
-00005f20: 6257 2f76 6965 773f 7573 703d 7368 6172  bW/view?usp=shar
-00005f30: 696e 6729 2020 2020 207c 205b 6c69 6e6b  ing)     | [link
-00005f40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005f50: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00005f60: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00005f70: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-00005f80: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-00005f90: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-00005fa0: 6374 6f72 5f69 6e73 686f 7029 207c 0a7c  ctor_inshop) |.|
-00005fb0: 2020 6056 6954 4578 7472 6163 746f 722e    `ViTExtractor.
-00005fc0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005fd0: 2276 6974 7331 365f 736f 7022 2960 2020  "vits16_sop")`  
-00005fe0: 207c 2030 2e38 3636 207c 2053 7461 6e66   | 0.866 | Stanf
-00005ff0: 6f72 6420 4f6e 6c69 6e65 2050 726f 6475  ord Online Produ
-00006000: 6374 7320 7c20 2020 5b6c 696e 6b5d 2868  cts |   [link](h
-00006010: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-00006020: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
-00006030: 7a75 4752 4876 4632 4b48 6435 3961 7737  zuGRHvF2KHd59aw7
-00006040: 6937 3336 374f 485f 7451 4e4f 477a 3741  i7367OH_tQNOGz7A
-00006050: 2f76 6965 773f 7573 703d 7368 6172 696e  /view?usp=sharin
-00006060: 6729 2020 2020 2020 7c20 205b 6c69 6e6b  g)      |  [link
-00006070: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006080: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00006090: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000060a0: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-000060b0: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-000060c0: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-000060d0: 6374 6f72 5f73 6f70 2920 2020 7c0a 7c20  ctor_sop)   |.| 
-000060e0: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-000060f0: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006100: 6974 7331 365f 6361 7273 2229 6020 2020  its16_cars")`   
-00006110: 7c20 302e 3930 3720 7c20 2020 2020 2020  | 0.907 |       
-00006120: 2020 4341 5253 2031 3936 2020 2020 2020    CARS 196      
-00006130: 2020 207c 2020 205b 6c69 6e6b 5d28 6874     |   [link](ht
-00006140: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00006150: 6c65 2e63 6f6d 2f64 7269 7665 2f66 6f6c  le.com/drive/fol
-00006160: 6465 7273 2f31 3761 345f 6667 3934 646f  ders/17a4_fg94do
-00006170: 7832 7366 6b58 6d77 2d4b 4374 694c 426c  x2sfkXmw-KCtiLBl
-00006180: 782d 7574 2d31 3f75 7370 3d73 6861 7269  x-ut-1?usp=shari
-00006190: 6e67 2920 2020 207c 2020 5b6c 696e 6b5d  ng)    |  [link]
-000061a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000061b0: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
-000061c0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-000061d0: 672f 7472 6565 2f6d 6169 6e2f 7069 7065  g/tree/main/pipe
-000061e0: 6c69 6e65 732f 6665 6174 7572 6573 5f65  lines/features_e
-000061f0: 7874 7261 6374 696f 6e2f 6578 7472 6163  xtraction/extrac
-00006200: 746f 725f 6361 7273 2920 207c 0a7c 2020  tor_cars)  |.|  
-00006210: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00006220: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006230: 6974 7331 365f 6375 6222 2960 2020 207c  its16_cub")`   |
-00006240: 2030 2e38 3337 207c 2020 2020 2020 2043   0.837 |       C
-00006250: 5542 2032 3030 2032 3031 3120 2020 2020  UB 200 2011     
-00006260: 2020 7c20 2020 5b6c 696e 6b5d 2868 7474    |   [link](htt
-00006270: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
-00006280: 652e 636f 6d2f 6472 6976 652f 666f 6c64  e.com/drive/fold
-00006290: 6572 732f 3154 5043 4e2d 655a 464c 716f  ers/1TPCN-eZFLqo
-000062a0: 7134 4a42 676e 4966 6c69 4a6f 454b 3438  q4JBgnIfliJoEK48
-000062b0: 7839 6f7a 623f 7573 703d 7368 6172 696e  x9ozb?usp=sharin
-000062c0: 6729 2020 2020 7c20 205b 6c69 6e6b 5d28  g)    |  [link](
-000062d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000062e0: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
-000062f0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00006300: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
-00006310: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
-00006320: 7472 6163 7469 6f6e 2f65 7874 7261 6374  traction/extract
-00006330: 6f72 5f63 7562 2920 2020 7c0a 0a57 6520  or_cub)   |..We 
-00006340: 616c 736f 2070 726f 7669 6465 2061 6e20  also provide an 
-00006350: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
-00006360: 2074 6865 206d 6f64 656c 7320 7072 6574   the models pret
-00006370: 7261 696e 6564 2062 7920 6f74 6865 7220  rained by other 
-00006380: 7265 7365 6172 6368 6572 732e 0a41 6c6c  researchers..All
-00006390: 206d 6574 7269 6373 2062 656c 6f77 2077   metrics below w
-000063a0: 6572 6520 6f62 7461 696e 6564 206f 6e20  ere obtained on 
-000063b0: 7468 6520 696d 6167 6573 2077 6974 6820  the images with 
-000063c0: 7468 6520 7369 7a65 7320 6f66 202a 2a32  the sizes of **2
-000063d0: 3234 2078 2032 3234 2a2a 3a0a 0a7c 2020  24 x 224**:..|  
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2020 2020 2020 2020 7c20 5374              | St
-00006420: 616e 666f 7264 204f 6e6c 696e 6520 5072  anford Online Pr
-00006430: 6f64 7563 7473 207c 2044 6565 7046 6173  oducts | DeepFas
-00006440: 6869 6f6e 2049 6e53 686f 7020 7c20 4355  hion InShop | CU
-00006450: 4220 3230 3020 3230 3131 207c 2043 4152  B 200 2011 | CAR
-00006460: 5320 3139 3620 7c0a 7c3a 2d2d 2d2d 2d2d  S 196 |.|:------
+00004230: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7361  ctor.from oml.sa
+00004240: 6d70 6c65 7273 2e62 616c 616e 6365 2069  mplers.balance i
+00004250: 6d70 6f72 7420 4261 6c61 6e63 6553 616d  mport BalanceSam
+00004260: 706c 6572 0a66 726f 6d20 6f6d 6c2e 7574  pler.from oml.ut
+00004270: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
+00004280: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
+00004290: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
+000042a0: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
+000042b0: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
+000042c0: 6173 6574 2f22 0a64 665f 7472 6169 6e2c  aset/".df_train,
+000042d0: 205f 203d 2064 6f77 6e6c 6f61 645f 6d6f   _ = download_mo
+000042e0: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+000042f0: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+00004300: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00004310: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+00004320: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+00004330: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+00004340: 7265 733d 4661 6c73 6529 2e74 7261 696e  res=False).train
+00004350: 2829 0a6f 7074 696d 697a 6572 203d 2074  ().optimizer = t
+00004360: 6f72 6368 2e6f 7074 696d 2e53 4744 2865  orch.optim.SGD(e
+00004370: 7874 7261 6374 6f72 2e70 6172 616d 6574  xtractor.paramet
+00004380: 6572 7328 292c 206c 723d 3165 2d36 290a  ers(), lr=1e-6).
+00004390: 0a74 7261 696e 5f64 6174 6173 6574 203d  .train_dataset =
+000043a0: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
+000043b0: 6c73 2864 665f 7472 6169 6e2c 2064 6174  ls(df_train, dat
+000043c0: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+000043d0: 745f 726f 6f74 290a 6372 6974 6572 696f  t_root).criterio
+000043e0: 6e20 3d20 5472 6970 6c65 744c 6f73 7357  n = TripletLossW
+000043f0: 6974 684d 696e 6572 286d 6172 6769 6e3d  ithMiner(margin=
+00004400: 302e 312c 206d 696e 6572 3d41 6c6c 5472  0.1, miner=AllTr
+00004410: 6970 6c65 7473 4d69 6e65 7228 292c 206e  ipletsMiner(), n
+00004420: 6565 645f 6c6f 6773 3d54 7275 6529 0a73  eed_logs=True).s
+00004430: 616d 706c 6572 203d 2042 616c 616e 6365  ampler = Balance
+00004440: 5361 6d70 6c65 7228 7472 6169 6e5f 6461  Sampler(train_da
+00004450: 7461 7365 742e 6765 745f 6c61 6265 6c73  taset.get_labels
+00004460: 2829 2c20 6e5f 6c61 6265 6c73 3d32 2c20  (), n_labels=2, 
+00004470: 6e5f 696e 7374 616e 6365 733d 3229 0a74  n_instances=2).t
+00004480: 7261 696e 5f6c 6f61 6465 7220 3d20 746f  rain_loader = to
+00004490: 7263 682e 7574 696c 732e 6461 7461 2e44  rch.utils.data.D
+000044a0: 6174 614c 6f61 6465 7228 7472 6169 6e5f  ataLoader(train_
+000044b0: 6461 7461 7365 742c 2062 6174 6368 5f73  dataset, batch_s
+000044c0: 616d 706c 6572 3d73 616d 706c 6572 290a  ampler=sampler).
+000044d0: 0a66 6f72 2062 6174 6368 2069 6e20 7471  .for batch in tq
+000044e0: 646d 2874 7261 696e 5f6c 6f61 6465 7229  dm(train_loader)
+000044f0: 3a0a 2020 2020 656d 6265 6464 696e 6773  :.    embeddings
+00004500: 203d 2065 7874 7261 6374 6f72 2862 6174   = extractor(bat
+00004510: 6368 5b22 696e 7075 745f 7465 6e73 6f72  ch["input_tensor
+00004520: 7322 5d29 0a20 2020 206c 6f73 7320 3d20  s"]).    loss = 
+00004530: 6372 6974 6572 696f 6e28 656d 6265 6464  criterion(embedd
+00004540: 696e 6773 2c20 6261 7463 685b 226c 6162  ings, batch["lab
+00004550: 656c 7322 5d29 0a20 2020 206c 6f73 732e  els"]).    loss.
+00004560: 6261 636b 7761 7264 2829 0a20 2020 206f  backward().    o
+00004570: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00004580: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
+00004590: 726f 5f67 7261 6428 290a 0a20 2020 2023  ro_grad()..    #
+000045a0: 2069 6e66 6f20 666f 7220 6c6f 6767 696e   info for loggin
+000045b0: 673a 2070 6f73 6974 6976 652f 6e65 6761  g: positive/nega
+000045c0: 7469 7665 2064 6973 7461 6e63 6573 2c20  tive distances, 
+000045d0: 6e75 6d62 6572 206f 6620 6163 7469 7665  number of active
+000045e0: 2074 7269 706c 6574 730a 2020 2020 7072   triplets.    pr
+000045f0: 696e 7428 6372 6974 6572 696f 6e2e 6c61  int(criterion.la
+00004600: 7374 5f6c 6f67 7329 0a0a 6060 600a 5b63  st_logs)..```.[c
+00004610: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+00004620: 7472 6169 6e2d 656e 640a 3c2f 703e 0a3c  train-end.</p>.<
+00004630: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+00004640: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+00004650: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004660: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+00004670: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+00004680: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00004690: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+000046a0: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+000046b0: 316b 6e74 4441 4964 495a 394c 3430 6a63  1kntDAIdIZ9L40jc
+000046c0: 6e64 6775 4c41 622d 5871 6d43 464f 6753  ndguLAb-XqmCFOgS
+000046d0: 353f 7573 703d 7368 6172 696e 6729 0a3c  5?usp=sharing).<
+000046e0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000046f0: 793e 5661 6c69 6461 7469 6f6e 3c2f 7375  y>Validation</su
+00004700: 6d6d 6172 793e 0a3c 703e 0a0a 5b63 6f6d  mmary>.<p>..[com
+00004710: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
+00004720: 6c69 6461 7469 6f6e 2d73 7461 7274 0a60  lidation-start.`
+00004730: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00004740: 746f 7263 680a 6672 6f6d 2074 7164 6d20  torch.from tqdm 
+00004750: 696d 706f 7274 2074 7164 6d0a 0a66 726f  import tqdm..fro
+00004760: 6d20 6f6d 6c2e 6461 7461 7365 7473 2e62  m oml.datasets.b
+00004770: 6173 6520 696d 706f 7274 2044 6174 6173  ase import Datas
+00004780: 6574 5175 6572 7947 616c 6c65 7279 0a66  etQueryGallery.f
+00004790: 726f 6d20 6f6d 6c2e 6d65 7472 6963 732e  rom oml.metrics.
+000047a0: 656d 6265 6464 696e 6773 2069 6d70 6f72  embeddings impor
+000047b0: 7420 456d 6265 6464 696e 674d 6574 7269  t EmbeddingMetri
+000047c0: 6373 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  cs.from oml.mode
+000047d0: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+000047e0: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+000047f0: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+00004800: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004810: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004820: 5f64 6174 6173 6574 0a0a 6461 7461 7365  _dataset..datase
+00004830: 745f 726f 6f74 203d 2022 6d6f 636b 5f64  t_root = "mock_d
+00004840: 6174 6173 6574 2f22 0a5f 2c20 6466 5f76  ataset/"._, df_v
+00004850: 616c 203d 2064 6f77 6e6c 6f61 645f 6d6f  al = download_mo
+00004860: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+00004870: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+00004880: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00004890: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+000048a0: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+000048b0: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+000048c0: 7265 733d 4661 6c73 6529 2e65 7661 6c28  res=False).eval(
+000048d0: 290a 0a76 616c 5f64 6174 6173 6574 203d  )..val_dataset =
+000048e0: 2044 6174 6173 6574 5175 6572 7947 616c   DatasetQueryGal
+000048f0: 6c65 7279 2864 665f 7661 6c2c 2064 6174  lery(df_val, dat
+00004900: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+00004910: 745f 726f 6f74 290a 0a76 616c 5f6c 6f61  t_root)..val_loa
+00004920: 6465 7220 3d20 746f 7263 682e 7574 696c  der = torch.util
+00004930: 732e 6461 7461 2e44 6174 614c 6f61 6465  s.data.DataLoade
+00004940: 7228 7661 6c5f 6461 7461 7365 742c 2062  r(val_dataset, b
+00004950: 6174 6368 5f73 697a 653d 3429 0a63 616c  atch_size=4).cal
+00004960: 6375 6c61 746f 7220 3d20 456d 6265 6464  culator = Embedd
+00004970: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+00004980: 5f6b 6579 733d 2822 7061 7468 7322 2c29  _keys=("paths",)
+00004990: 290a 6361 6c63 756c 6174 6f72 2e73 6574  ).calculator.set
+000049a0: 7570 286e 756d 5f73 616d 706c 6573 3d6c  up(num_samples=l
+000049b0: 656e 2876 616c 5f64 6174 6173 6574 2929  en(val_dataset))
+000049c0: 0a0a 7769 7468 2074 6f72 6368 2e6e 6f5f  ..with torch.no_
+000049d0: 6772 6164 2829 3a0a 2020 2020 666f 7220  grad():.    for 
+000049e0: 6261 7463 6820 696e 2074 7164 6d28 7661  batch in tqdm(va
+000049f0: 6c5f 6c6f 6164 6572 293a 0a20 2020 2020  l_loader):.     
+00004a00: 2020 2062 6174 6368 5b22 656d 6265 6464     batch["embedd
+00004a10: 696e 6773 225d 203d 2065 7874 7261 6374  ings"] = extract
+00004a20: 6f72 2862 6174 6368 5b22 696e 7075 745f  or(batch["input_
+00004a30: 7465 6e73 6f72 7322 5d29 0a20 2020 2020  tensors"]).     
+00004a40: 2020 2063 616c 6375 6c61 746f 722e 7570     calculator.up
+00004a50: 6461 7465 5f64 6174 6128 6261 7463 6829  date_data(batch)
+00004a60: 0a0a 6d65 7472 6963 7320 3d20 6361 6c63  ..metrics = calc
+00004a70: 756c 6174 6f72 2e63 6f6d 7075 7465 5f6d  ulator.compute_m
+00004a80: 6574 7269 6373 2829 0a0a 2320 4c6f 6767  etrics()..# Logg
+00004a90: 696e 670a 7072 696e 7428 6361 6c63 756c  ing.print(calcul
+00004aa0: 6174 6f72 2e6d 6574 7269 6373 2920 2023  ator.metrics)  #
+00004ab0: 206d 6574 7269 6373 0a70 7269 6e74 2863   metrics.print(c
+00004ac0: 616c 6375 6c61 746f 722e 6d65 7472 6963  alculator.metric
+00004ad0: 735f 756e 7265 6475 6365 6429 2020 2320  s_unreduced)  # 
+00004ae0: 6d65 7472 6963 7320 7769 7468 6f75 7420  metrics without 
+00004af0: 6176 6572 6167 696e 6720 6f76 6572 2071  averaging over q
+00004b00: 7565 7269 6573 0a0a 2320 5669 7375 616c  ueries..# Visual
+00004b10: 6973 6174 696f 6e0a 6361 6c63 756c 6174  isation.calculat
+00004b20: 6f72 2e67 6574 5f70 6c6f 745f 666f 725f  or.get_plot_for_
+00004b30: 7175 6572 6965 7328 7175 6572 795f 6964  queries(query_id
+00004b40: 733d 5b30 2c20 325d 2c20 6e5f 696e 7374  s=[0, 2], n_inst
+00004b50: 616e 6365 733d 3529 2020 2320 6472 6177  ances=5)  # draw
+00004b60: 2070 7265 6469 6374 696f 6e73 206f 6e20   predictions on 
+00004b70: 7072 6564 6566 696e 6564 2071 7565 7269  predefined queri
+00004b80: 6573 0a63 616c 6375 6c61 746f 722e 6765  es.calculator.ge
+00004b90: 745f 706c 6f74 5f66 6f72 5f77 6f72 7374  t_plot_for_worst
+00004ba0: 5f71 7565 7269 6573 286d 6574 7269 635f  _queries(metric_
+00004bb0: 6e61 6d65 3d22 4f56 4552 414c 4c2f 6d61  name="OVERALL/ma
+00004bc0: 702f 3522 2c20 6e5f 7175 6572 6965 733d  p/5", n_queries=
+00004bd0: 322c 206e 5f69 6e73 7461 6e63 6573 3d35  2, n_instances=5
+00004be0: 2920 2023 2064 7261 7720 6d69 7374 616b  )  # draw mistak
+00004bf0: 6573 0a63 616c 6375 6c61 746f 722e 7669  es.calculator.vi
+00004c00: 7375 616c 697a 6528 2920 2023 2064 7261  sualize()  # dra
+00004c10: 7720 6d69 7374 616b 6573 2066 6f72 2061  w mistakes for a
+00004c20: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+00004c30: 206d 6574 7269 6373 0a0a 6060 600a 5b63   metrics..```.[c
+00004c40: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+00004c50: 7661 6c69 6461 7469 6f6e 2d65 6e64 0a3c  validation-end.<
+00004c60: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
+00004c70: 5b21 5b4f 7065 6e20 496e 2043 6f6c 6162  [![Open In Colab
+00004c80: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00004c90: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00004ca0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00004cb0: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
+00004cc0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004cd0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
+00004ce0: 7269 7665 2f31 4f32 6f33 6b38 4938 6a4e  rive/1O2o3k8I8jN
+00004cf0: 3568 5269 6e33 644b 6e41 5333 5773 6747  5hRin3dKnAS3WsgG
+00004d00: 3034 746d 4954 3f75 7370 3d73 6861 7269  04tmIT?usp=shari
+00004d10: 6e67 290a 3c64 6574 6169 6c73 3e0a 3c73  ng).<details>.<s
+00004d20: 756d 6d61 7279 3e54 7261 696e 696e 6720  ummary>Training 
+00004d30: 2b20 5661 6c69 6461 7469 6f6e 205b 4c69  + Validation [Li
+00004d40: 6768 746e 696e 6720 616e 6420 6c6f 6767  ghtning and logg
+00004d50: 696e 675d 3c2f 7375 6d6d 6172 793e 0a3c  ing]</summary>.<
+00004d60: 703e 0a0a 5b63 6f6d 6d65 6e74 5d3a 6c69  p>..[comment]:li
+00004d70: 6768 746e 696e 672d 7374 6172 740a 6060  ghtning-start.``
+00004d80: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+00004d90: 7974 6f72 6368 5f6c 6967 6874 6e69 6e67  ytorch_lightning
+00004da0: 2061 7320 706c 0a69 6d70 6f72 7420 746f   as pl.import to
+00004db0: 7263 680a 0a66 726f 6d20 6f6d 6c2e 6461  rch..from oml.da
+00004dc0: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00004dd0: 7274 2044 6174 6173 6574 5175 6572 7947  rt DatasetQueryG
+00004de0: 616c 6c65 7279 2c20 4461 7461 7365 7457  allery, DatasetW
+00004df0: 6974 684c 6162 656c 730a 6672 6f6d 206f  ithLabels.from o
+00004e00: 6d6c 2e6c 6967 6874 6e69 6e67 2e6d 6f64  ml.lightning.mod
+00004e10: 756c 6573 2e65 7874 7261 6374 6f72 2069  ules.extractor i
+00004e20: 6d70 6f72 7420 4578 7472 6163 746f 724d  mport ExtractorM
+00004e30: 6f64 756c 650a 6672 6f6d 206f 6d6c 2e6c  odule.from oml.l
+00004e40: 6967 6874 6e69 6e67 2e63 616c 6c62 6163  ightning.callbac
+00004e50: 6b73 2e6d 6574 7269 6320 696d 706f 7274  ks.metric import
+00004e60: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+00004e70: 636b 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ck.from oml.loss
+00004e80: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
+00004e90: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
+00004ea0: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
+00004eb0: 6d65 7472 6963 732e 656d 6265 6464 696e  metrics.embeddin
+00004ec0: 6773 2069 6d70 6f72 7420 456d 6265 6464  gs import Embedd
+00004ed0: 696e 674d 6574 7269 6373 0a66 726f 6d20  ingMetrics.from 
+00004ee0: 6f6d 6c2e 6d69 6e65 7273 2e69 6e62 6174  oml.miners.inbat
+00004ef0: 6368 5f61 6c6c 5f74 7269 2069 6d70 6f72  ch_all_tri impor
+00004f00: 7420 416c 6c54 7269 706c 6574 734d 696e  t AllTripletsMin
+00004f10: 6572 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  er.from oml.mode
+00004f20: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+00004f30: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+00004f40: 7361 6d70 6c65 7273 2e62 616c 616e 6365  samplers.balance
+00004f50: 2069 6d70 6f72 7420 4261 6c61 6e63 6553   import BalanceS
+00004f60: 616d 706c 6572 0a66 726f 6d20 6f6d 6c2e  ampler.from oml.
+00004f70: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+00004f80: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004f90: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004fa0: 5f64 6174 6173 6574 0a66 726f 6d20 7079  _dataset.from py
+00004fb0: 746f 7263 685f 6c69 6768 746e 696e 672e  torch_lightning.
+00004fc0: 6c6f 6767 6572 7320 696d 706f 7274 204e  loggers import N
+00004fd0: 6570 7475 6e65 4c6f 6767 6572 2c20 5465  eptuneLogger, Te
+00004fe0: 6e73 6f72 426f 6172 644c 6f67 6765 722c  nsorBoardLogger,
+00004ff0: 2057 616e 6462 4c6f 6767 6572 0a0a 6461   WandbLogger..da
+00005000: 7461 7365 745f 726f 6f74 203d 2022 6d6f  taset_root = "mo
+00005010: 636b 5f64 6174 6173 6574 2f22 0a64 665f  ck_dataset/".df_
+00005020: 7472 6169 6e2c 2064 665f 7661 6c20 3d20  train, df_val = 
+00005030: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+00005040: 7461 7365 7428 6461 7461 7365 745f 726f  taset(dataset_ro
+00005050: 6f74 290a 0a23 206d 6f64 656c 0a65 7874  ot)..# model.ext
+00005060: 7261 6374 6f72 203d 2056 6954 4578 7472  ractor = ViTExtr
+00005070: 6163 746f 7228 2276 6974 7331 365f 6469  actor("vits16_di
+00005080: 6e6f 222c 2061 7263 683d 2276 6974 7331  no", arch="vits1
+00005090: 3622 2c20 6e6f 726d 616c 6973 655f 6665  6", normalise_fe
+000050a0: 6174 7572 6573 3d46 616c 7365 290a 0a23  atures=False)..#
+000050b0: 2074 7261 696e 0a6f 7074 696d 697a 6572   train.optimizer
+000050c0: 203d 2074 6f72 6368 2e6f 7074 696d 2e53   = torch.optim.S
+000050d0: 4744 2865 7874 7261 6374 6f72 2e70 6172  GD(extractor.par
+000050e0: 616d 6574 6572 7328 292c 206c 723d 3165  ameters(), lr=1e
+000050f0: 2d36 290a 7472 6169 6e5f 6461 7461 7365  -6).train_datase
+00005100: 7420 3d20 4461 7461 7365 7457 6974 684c  t = DatasetWithL
+00005110: 6162 656c 7328 6466 5f74 7261 696e 2c20  abels(df_train, 
+00005120: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00005130: 6173 6574 5f72 6f6f 7429 0a63 7269 7465  aset_root).crite
+00005140: 7269 6f6e 203d 2054 7269 706c 6574 4c6f  rion = TripletLo
+00005150: 7373 5769 7468 4d69 6e65 7228 6d61 7267  ssWithMiner(marg
+00005160: 696e 3d30 2e31 2c20 6d69 6e65 723d 416c  in=0.1, miner=Al
+00005170: 6c54 7269 706c 6574 734d 696e 6572 2829  lTripletsMiner()
+00005180: 290a 6261 7463 685f 7361 6d70 6c65 7220  ).batch_sampler 
+00005190: 3d20 4261 6c61 6e63 6553 616d 706c 6572  = BalanceSampler
+000051a0: 2874 7261 696e 5f64 6174 6173 6574 2e67  (train_dataset.g
+000051b0: 6574 5f6c 6162 656c 7328 292c 206e 5f6c  et_labels(), n_l
+000051c0: 6162 656c 733d 322c 206e 5f69 6e73 7461  abels=2, n_insta
+000051d0: 6e63 6573 3d33 290a 7472 6169 6e5f 6c6f  nces=3).train_lo
+000051e0: 6164 6572 203d 2074 6f72 6368 2e75 7469  ader = torch.uti
+000051f0: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+00005200: 6572 2874 7261 696e 5f64 6174 6173 6574  er(train_dataset
+00005210: 2c20 6261 7463 685f 7361 6d70 6c65 723d  , batch_sampler=
+00005220: 6261 7463 685f 7361 6d70 6c65 7229 0a0a  batch_sampler)..
+00005230: 2320 7661 6c0a 7661 6c5f 6461 7461 7365  # val.val_datase
+00005240: 7420 3d20 4461 7461 7365 7451 7565 7279  t = DatasetQuery
+00005250: 4761 6c6c 6572 7928 6466 5f76 616c 2c20  Gallery(df_val, 
+00005260: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00005270: 6173 6574 5f72 6f6f 7429 0a76 616c 5f6c  aset_root).val_l
+00005280: 6f61 6465 7220 3d20 746f 7263 682e 7574  oader = torch.ut
+00005290: 696c 732e 6461 7461 2e44 6174 614c 6f61  ils.data.DataLoa
+000052a0: 6465 7228 7661 6c5f 6461 7461 7365 742c  der(val_dataset,
+000052b0: 2062 6174 6368 5f73 697a 653d 3429 0a6d   batch_size=4).m
+000052c0: 6574 7269 635f 6361 6c6c 6261 636b 203d  etric_callback =
+000052d0: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+000052e0: 636b 286d 6574 7269 633d 456d 6265 6464  ck(metric=Embedd
+000052f0: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+00005300: 5f6b 6579 733d 5b74 7261 696e 5f64 6174  _keys=[train_dat
+00005310: 6173 6574 2e70 6174 6873 5f6b 6579 2c5d  aset.paths_key,]
+00005320: 292c 206c 6f67 5f69 6d61 6765 733d 5472  ), log_images=Tr
+00005330: 7565 290a 0a23 2031 2920 4c6f 6767 696e  ue)..# 1) Loggin
+00005340: 6720 7769 7468 2054 656e 736f 7262 6f61  g with Tensorboa
+00005350: 7264 0a6c 6f67 6765 7220 3d20 5465 6e73  rd.logger = Tens
+00005360: 6f72 426f 6172 644c 6f67 6765 7228 222e  orBoardLogger(".
+00005370: 2229 0a0a 2320 3229 204c 6f67 6769 6e67  ")..# 2) Logging
+00005380: 2077 6974 6820 4e65 7074 756e 650a 2320   with Neptune.# 
+00005390: 6c6f 6767 6572 203d 204e 6570 7475 6e65  logger = Neptune
+000053a0: 4c6f 6767 6572 2861 7069 5f6b 6579 3d22  Logger(api_key="
+000053b0: 222c 2070 726f 6a65 6374 3d22 222c 206c  ", project="", l
+000053c0: 6f67 5f6d 6f64 656c 5f63 6865 636b 706f  og_model_checkpo
+000053d0: 696e 7473 3d46 616c 7365 290a 0a23 2033  ints=False)..# 3
+000053e0: 2920 4c6f 6767 696e 6720 7769 7468 2057  ) Logging with W
+000053f0: 6569 6768 7473 2061 6e64 2042 6961 7365  eights and Biase
+00005400: 730a 2320 696d 706f 7274 206f 730a 2320  s.# import os.# 
+00005410: 6f73 2e65 6e76 6972 6f6e 5b22 5741 4e44  os.environ["WAND
+00005420: 425f 4150 495f 4b45 5922 5d20 3d20 2222  B_API_KEY"] = ""
+00005430: 0a23 206c 6f67 6765 7220 3d20 5761 6e64  .# logger = Wand
+00005440: 624c 6f67 6765 7228 7072 6f6a 6563 743d  bLogger(project=
+00005450: 2274 6573 745f 7072 6f6a 6563 7422 2c20  "test_project", 
+00005460: 6c6f 675f 6d6f 6465 6c3d 4661 6c73 6529  log_model=False)
+00005470: 0a0a 2320 7275 6e0a 706c 5f6d 6f64 656c  ..# run.pl_model
+00005480: 203d 2045 7874 7261 6374 6f72 4d6f 6475   = ExtractorModu
+00005490: 6c65 2865 7874 7261 6374 6f72 2c20 6372  le(extractor, cr
+000054a0: 6974 6572 696f 6e2c 206f 7074 696d 697a  iterion, optimiz
+000054b0: 6572 290a 7472 6169 6e65 7220 3d20 706c  er).trainer = pl
+000054c0: 2e54 7261 696e 6572 286d 6178 5f65 706f  .Trainer(max_epo
+000054d0: 6368 733d 332c 2063 616c 6c62 6163 6b73  chs=3, callbacks
+000054e0: 3d5b 6d65 7472 6963 5f63 616c 6c62 6163  =[metric_callbac
+000054f0: 6b5d 2c20 6e75 6d5f 7361 6e69 7479 5f76  k], num_sanity_v
+00005500: 616c 5f73 7465 7073 3d30 2c20 6c6f 6767  al_steps=0, logg
+00005510: 6572 3d6c 6f67 6765 7229 0a74 7261 696e  er=logger).train
+00005520: 6572 2e66 6974 2870 6c5f 6d6f 6465 6c2c  er.fit(pl_model,
+00005530: 2074 7261 696e 5f64 6174 616c 6f61 6465   train_dataloade
+00005540: 7273 3d74 7261 696e 5f6c 6f61 6465 722c  rs=train_loader,
+00005550: 2076 616c 5f64 6174 616c 6f61 6465 7273   val_dataloaders
+00005560: 3d76 616c 5f6c 6f61 6465 7229 0a0a 6060  =val_loader)..``
+00005570: 600a 5b63 6f6d 6d65 6e74 5d3a 6c69 6768  `.[comment]:ligh
+00005580: 746e 696e 672d 656e 640a 3c2f 703e 0a3c  tning-end.</p>.<
+00005590: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+000055a0: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+000055b0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000055c0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000055d0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000055e0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000055f0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00005600: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00005610: 3162 5655 6764 4247 5776 5167 436b 6261  1bVUgdBGWvQgCkba
+00005620: 3259 7461 4952 566c 5551 557a 3751 3630  2YtaIRVlUQUz7Q60
+00005630: 5a3f 7573 703d 7368 6172 655f 6c69 6e6b  Z?usp=share_link
+00005640: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
+00005650: 6d61 7279 3e55 7369 6e67 2061 2074 7261  mary>Using a tra
+00005660: 696e 6564 206d 6f64 656c 2066 6f72 2072  ined model for r
+00005670: 6574 7269 6576 616c 3c2f 7375 6d6d 6172  etrieval</summar
+00005680: 793e 0a3c 703e 0a0a 5b63 6f6d 6d65 6e74  y>.<p>..[comment
+00005690: 5d3a 7573 6167 652d 7265 7472 6965 7661  ]:usage-retrieva
+000056a0: 6c2d 7374 6172 740a 6060 6070 7974 686f  l-start.```pytho
+000056b0: 6e0a 696d 706f 7274 2074 6f72 6368 0a0a  n.import torch..
+000056c0: 6672 6f6d 206f 6d6c 2e63 6f6e 7374 2069  from oml.const i
+000056d0: 6d70 6f72 7420 4d4f 434b 5f44 4154 4153  mport MOCK_DATAS
+000056e0: 4554 5f50 4154 480a 6672 6f6d 206f 6d6c  ET_PATH.from oml
+000056f0: 2e69 6e66 6572 656e 6365 2e66 6c61 7420  .inference.flat 
+00005700: 696d 706f 7274 2069 6e66 6572 656e 6365  import inference
+00005710: 5f6f 6e5f 696d 6167 6573 0a66 726f 6d20  _on_images.from 
+00005720: 6f6d 6c2e 6d6f 6465 6c73 2069 6d70 6f72  oml.models impor
+00005730: 7420 5669 5445 7874 7261 6374 6f72 0a66  t ViTExtractor.f
+00005740: 726f 6d20 6f6d 6c2e 7265 6769 7374 7279  rom oml.registry
+00005750: 2e74 7261 6e73 666f 726d 7320 696d 706f  .transforms impo
+00005760: 7274 2067 6574 5f74 7261 6e73 666f 726d  rt get_transform
+00005770: 735f 666f 725f 7072 6574 7261 696e 6564  s_for_pretrained
+00005780: 0a66 726f 6d20 6f6d 6c2e 7574 696c 732e  .from oml.utils.
+00005790: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+000057a0: 7461 7365 7420 696d 706f 7274 2064 6f77  taset import dow
+000057b0: 6e6c 6f61 645f 6d6f 636b 5f64 6174 6173  nload_mock_datas
+000057c0: 6574 0a66 726f 6d20 6f6d 6c2e 7574 696c  et.from oml.util
+000057d0: 732e 6d69 7363 5f74 6f72 6368 2069 6d70  s.misc_torch imp
+000057e0: 6f72 7420 7061 6972 7769 7365 5f64 6973  ort pairwise_dis
+000057f0: 740a 0a5f 2c20 6466 5f76 616c 203d 2064  t.._, df_val = d
+00005800: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
+00005810: 6173 6574 284d 4f43 4b5f 4441 5441 5345  aset(MOCK_DATASE
+00005820: 545f 5041 5448 290a 6466 5f76 616c 5b22  T_PATH).df_val["
+00005830: 7061 7468 225d 203d 2064 665f 7661 6c5b  path"] = df_val[
+00005840: 2270 6174 6822 5d2e 6170 706c 7928 6c61  "path"].apply(la
+00005850: 6d62 6461 2078 3a20 4d4f 434b 5f44 4154  mbda x: MOCK_DAT
+00005860: 4153 4554 5f50 4154 4820 2f20 7829 0a71  ASET_PATH / x).q
+00005870: 7565 7269 6573 203d 2064 665f 7661 6c5b  ueries = df_val[
+00005880: 6466 5f76 616c 5b22 6973 5f71 7565 7279  df_val["is_query
+00005890: 225d 5d5b 2270 6174 6822 5d2e 746f 6c69  "]]["path"].toli
+000058a0: 7374 2829 0a67 616c 6c65 7269 6573 203d  st().galleries =
+000058b0: 2064 665f 7661 6c5b 6466 5f76 616c 5b22   df_val[df_val["
+000058c0: 6973 5f67 616c 6c65 7279 225d 5d5b 2270  is_gallery"]]["p
+000058d0: 6174 6822 5d2e 746f 6c69 7374 2829 0a0a  ath"].tolist()..
+000058e0: 6578 7472 6163 746f 7220 3d20 5669 5445  extractor = ViTE
+000058f0: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00005900: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00005910: 5f64 696e 6f22 290a 7472 616e 7366 6f72  _dino").transfor
+00005920: 6d2c 205f 203d 2067 6574 5f74 7261 6e73  m, _ = get_trans
+00005930: 666f 726d 735f 666f 725f 7072 6574 7261  forms_for_pretra
+00005940: 696e 6564 2822 7669 7473 3136 5f64 696e  ined("vits16_din
+00005950: 6f22 290a 0a61 7267 7320 3d20 7b22 6e75  o")..args = {"nu
+00005960: 6d5f 776f 726b 6572 7322 3a20 302c 2022  m_workers": 0, "
+00005970: 6261 7463 685f 7369 7a65 223a 2038 7d0a  batch_size": 8}.
+00005980: 6665 6174 7572 6573 5f71 7565 7269 6573  features_queries
+00005990: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+000059a0: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+000059b0: 2c20 7061 7468 733d 7175 6572 6965 732c  , paths=queries,
+000059c0: 2074 7261 6e73 666f 726d 3d74 7261 6e73   transform=trans
+000059d0: 666f 726d 2c20 2a2a 6172 6773 290a 6665  form, **args).fe
+000059e0: 6174 7572 6573 5f67 616c 6c65 7269 6573  atures_galleries
+000059f0: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+00005a00: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+00005a10: 2c20 7061 7468 733d 6761 6c6c 6572 6965  , paths=gallerie
+00005a20: 732c 2074 7261 6e73 666f 726d 3d74 7261  s, transform=tra
+00005a30: 6e73 666f 726d 2c20 2a2a 6172 6773 290a  nsform, **args).
+00005a40: 0a23 204e 6f77 2077 6520 6361 6e20 6578  .# Now we can ex
+00005a50: 706c 6963 6974 6c79 2062 7569 6c64 2070  plicitly build p
+00005a60: 6169 7277 6973 6520 6d61 7472 6978 206f  airwise matrix o
+00005a70: 6620 6469 7374 616e 6365 7320 6f72 2073  f distances or s
+00005a80: 6176 6520 796f 7520 5241 4d20 7669 6120  ave you RAM via 
+00005a90: 7573 696e 6720 6b4e 4e0a 7573 655f 6b6e  using kNN.use_kn
+00005aa0: 6e20 3d20 5472 7565 0a74 6f70 5f6b 203d  n = True.top_k =
+00005ab0: 2033 0a0a 6966 2075 7365 5f6b 6e6e 3a0a   3..if use_knn:.
+00005ac0: 2020 2020 6672 6f6d 2073 6b6c 6561 726e      from sklearn
+00005ad0: 2e6e 6569 6768 626f 7273 2069 6d70 6f72  .neighbors impor
+00005ae0: 7420 4e65 6172 6573 744e 6569 6768 626f  t NearestNeighbo
+00005af0: 7273 0a20 2020 206b 6e6e 203d 204e 6561  rs.    knn = Nea
+00005b00: 7265 7374 4e65 6967 6862 6f72 7328 616c  restNeighbors(al
+00005b10: 676f 7269 7468 6d3d 2261 7574 6f22 2c20  gorithm="auto", 
+00005b20: 703d 3229 0a20 2020 206b 6e6e 2e66 6974  p=2).    knn.fit
+00005b30: 2866 6561 7475 7265 735f 6761 6c6c 6572  (features_galler
+00005b40: 6965 7329 0a20 2020 2064 6973 7473 2c20  ies).    dists, 
+00005b50: 6969 5f63 6c6f 7365 7374 203d 206b 6e6e  ii_closest = knn
+00005b60: 2e6b 6e65 6967 6862 6f72 7328 6665 6174  .kneighbors(feat
+00005b70: 7572 6573 5f71 7565 7269 6573 2c20 6e5f  ures_queries, n_
+00005b80: 6e65 6967 6862 6f72 733d 746f 705f 6b2c  neighbors=top_k,
+00005b90: 2072 6574 7572 6e5f 6469 7374 616e 6365   return_distance
+00005ba0: 3d54 7275 6529 0a0a 656c 7365 3a0a 2020  =True)..else:.  
+00005bb0: 2020 6469 7374 5f6d 6174 203d 2070 6169    dist_mat = pai
+00005bc0: 7277 6973 655f 6469 7374 2878 313d 6665  rwise_dist(x1=fe
+00005bd0: 6174 7572 6573 5f71 7565 7269 6573 2c20  atures_queries, 
+00005be0: 7832 3d66 6561 7475 7265 735f 6761 6c6c  x2=features_gall
+00005bf0: 6572 6965 7329 0a20 2020 2064 6973 7473  eries).    dists
+00005c00: 2c20 6969 5f63 6c6f 7365 7374 203d 2074  , ii_closest = t
+00005c10: 6f72 6368 2e74 6f70 6b28 6469 7374 5f6d  orch.topk(dist_m
+00005c20: 6174 2c20 6469 6d3d 312c 206b 3d74 6f70  at, dim=1, k=top
+00005c30: 5f6b 2c20 6c61 7267 6573 743d 4661 6c73  _k, largest=Fals
+00005c40: 6529 0a0a 7072 696e 7428 6622 546f 7020  e)..print(f"Top 
+00005c50: 7b74 6f70 5f6b 7d20 6974 656d 7320 636c  {top_k} items cl
+00005c60: 6f73 6573 7420 746f 2071 7565 7269 6573  osest to queries
+00005c70: 2061 7265 3a5c 6e20 7b69 695f 636c 6f73   are:\n {ii_clos
+00005c80: 6573 747d 2229 0a60 6060 0a5b 636f 6d6d  est}").```.[comm
+00005c90: 656e 745d 3a75 7361 6765 2d72 6574 7269  ent]:usage-retri
+00005ca0: 6576 616c 2d65 6e64 0a3c 2f70 3e0a 3c2f  eval-end.</p>.</
+00005cb0: 6465 7461 696c 733e 0a0a 5b21 5b4f 7065  details>..[![Ope
+00005cc0: 6e20 496e 2043 6f6c 6162 5d28 6874 7470  n In Colab](http
+00005cd0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00005ce0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
+00005cf0: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
+00005d00: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+00005d10: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00005d20: 6f67 6c65 2e63 6f6d 2f64 7269 7665 2f31  ogle.com/drive/1
+00005d30: 5332 6e4b 364b 6152 6544 6d2d 526a 6a64  S2nK6KaReDm-Rjjd
+00005d40: 6f6a 6449 6436 4361 6b68 6853 7976 6641  ojdId6CakhhSyvfA
+00005d50: 3f75 7370 3d73 6861 7265 5f6c 696e 6b29  ?usp=share_link)
+00005d60: 0a0a 5b2a 2a53 6368 656d 6173 2c20 6578  ..[**Schemas, ex
+00005d70: 706c 616e 6174 696f 6e73 2061 6e64 2074  planations and t
+00005d80: 6970 732a 2a5d 2868 7474 7073 3a2f 2f67  ips**](https://g
+00005d90: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
+00005da0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
+00005db0: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
+00005dc0: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
+00005dd0: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
+00005de0: 0a0a 5365 6520 5b65 7874 7261 2063 6f64  ..See [extra cod
+00005df0: 6520 736e 6970 7065 7473 5d28 6874 7470  e snippets](http
+00005e00: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00005e10: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00005e20: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00005e30: 742f 6665 6174 7572 655f 6578 7472 6163  t/feature_extrac
+00005e40: 7469 6f6e 2f70 7974 686f 6e5f 6578 616d  tion/python_exam
+00005e50: 706c 6573 2e68 746d 6c29 2c20 696e 636c  ples.html), incl
+00005e60: 7564 696e 673a 0a2a 2054 7261 696e 696e  uding:.* Trainin
+00005e70: 6720 2b20 5661 6c69 6461 7469 6f6e 2077  g + Validation w
+00005e80: 6974 6820 4c69 6768 746e 696e 670a 2a20  ith Lightning.* 
+00005e90: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
+00005ea0: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
+00005eb0: 6e69 6e67 2069 6e20 4444 5020 6d6f 6465  ning in DDP mode
+00005ec0: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005ed0: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005ee0: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005ef0: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005f00: 2061 6476 616e 6365 6420 2870 6173 7369   advanced (passi
+00005f10: 6e67 2064 6973 7461 6e63 652c 2072 6564  ng distance, red
+00005f20: 7563 6572 2c20 6d69 6e65 7229 0a0a 2323  ucer, miner)..##
+00005f30: 205b 5069 7065 6c69 6e65 735d 2868 7474   [Pipelines](htt
+00005f40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005f50: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
+00005f60: 7472 6963 2d6c 6561 726e 696e 672f 7472  tric-learning/tr
+00005f70: 6565 2f6d 6169 6e2f 7069 7065 6c69 6e65  ee/main/pipeline
+00005f80: 7329 0a0a 5069 7065 6c69 6e65 7320 7072  s)..Pipelines pr
+00005f90: 6f76 6964 6520 6120 7761 7920 746f 2072  ovide a way to r
+00005fa0: 756e 206d 6574 7269 6320 6c65 6172 6e69  un metric learni
+00005fb0: 6e67 2065 7870 6572 696d 656e 7473 2076  ng experiments v
+00005fc0: 6961 2063 6861 6e67 696e 6720 6f6e 6c79  ia changing only
+00005fd0: 2074 6865 2063 6f6e 6669 6720 6669 6c65   the config file
+00005fe0: 2e0a 416c 6c20 796f 7520 6e65 6564 2069  ..All you need i
+00005ff0: 7320 746f 2070 7265 7061 7265 2079 6f75  s to prepare you
+00006000: 7220 6461 7461 7365 7420 696e 2061 2072  r dataset in a r
+00006010: 6571 7569 7265 6420 666f 726d 6174 2e0a  equired format..
+00006020: 0a53 6565 205b 5069 7065 6c69 6e65 735d  .See [Pipelines]
+00006030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006040: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
+00006050: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
+00006060: 672f 626c 6f62 2f6d 6169 6e2f 7069 7065  g/blob/main/pipe
+00006070: 6c69 6e65 732f 2920 666f 6c64 6572 2066  lines/) folder f
+00006080: 6f72 206d 6f72 6520 6465 7461 696c 733a  or more details:
+00006090: 0a2a 2046 6561 7475 7265 2065 7874 7261  .* Feature extra
+000060a0: 6374 6f72 205b 7069 7065 6c69 6e65 5d28  ctor [pipeline](
+000060b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000060c0: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
+000060d0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+000060e0: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
+000060f0: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
+00006100: 7472 6163 7469 6f6e 290a 2a20 5265 7472  traction).* Retr
+00006110: 6965 7661 6c20 706f 7374 7072 6f63 6573  ieval postproces
+00006120: 736f 7220 5b70 6970 656c 696e 655d 2868  sor [pipeline](h
+00006130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006140: 6d2f 4f4d 4c2d 5465 616d 2f6f 7065 6e2d  m/OML-Team/open-
+00006150: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
+00006160: 7472 6565 2f6d 6169 6e2f 7069 7065 6c69  tree/main/pipeli
+00006170: 6e65 732f 706f 7374 7072 6f63 6573 7369  nes/postprocessi
+00006180: 6e67 2920 2872 652d 7261 6e6b 696e 6729  ng) (re-ranking)
+00006190: 0a0a 2323 205b 5a6f 6f5d 2868 7474 7073  ..## [Zoo](https
+000061a0: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
+000061b0: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
+000061c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000061d0: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
+000061e0: 696f 6e2f 7a6f 6f2e 6874 6d6c 290a 0a42  ion/zoo.html)..B
+000061f0: 656c 6f77 2061 7265 2074 6865 206d 6f64  elow are the mod
+00006200: 656c 7320 7472 6169 6e65 6420 7769 7468  els trained with
+00006210: 204f 4d4c 206f 6e20 3420 7075 626c 6963   OML on 4 public
+00006220: 2064 6174 6173 6574 732e 0a41 6c6c 206d   datasets..All m
+00006230: 6574 7269 6373 2062 656c 6f77 2077 6572  etrics below wer
+00006240: 6520 6f62 7461 696e 6564 206f 6e20 7468  e obtained on th
+00006250: 6520 696d 6167 6573 2077 6974 6820 7468  e images with th
+00006260: 6520 7369 7a65 7320 6f66 202a 2a32 3234  e sizes of **224
+00006270: 2078 2032 3234 2a2a 3a0a 0a7c 2020 2020   x 224**:..|    
+00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006290: 2020 6d6f 6465 6c20 2020 2020 2020 2020    model         
+000062a0: 2020 2020 2020 2020 2020 2020 207c 2063               | c
+000062b0: 6d63 3120 207c 2020 2020 2020 2020 2064  mc1  |         d
+000062c0: 6174 6173 6574 2020 2020 2020 2020 2020  ataset          
+000062d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00006300: 6569 6768 7473 2020 2020 2020 2020 2020  eights          
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2020 2020 2020 2020 2065 7870 6572 696d           experim
+00006370: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2020 2020 2020 2020 7c0a 7c3a 2d2d 2d2d          |.|:----
+000063b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000063c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000063d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+000063e0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+000063f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00006400: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00006410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006460: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
 00006470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064a0: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+000064a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064c0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-000064d0: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-000064e0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-000064f0: 3a7c 0a7c 2020 2020 6056 6954 556e 6963  :|.|    `ViTUnic
-00006500: 6f6d 4578 7472 6163 746f 722e 6672 6f6d  omExtractor.from
-00006510: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-00006520: 6231 365f 756e 6963 6f6d 2229 6020 2020  b16_unicom")`   
-00006530: 2020 7c20 2020 2020 2020 2020 2030 2e37    |          0.7
-00006540: 3030 2020 2020 2020 2020 2020 207c 2020  00           |  
-00006550: 2020 2020 2030 2e37 3334 2020 2020 2020       0.734      
-00006560: 2020 7c20 2020 2030 2e38 3437 2020 2020    |    0.847    
-00006570: 207c 2020 302e 3931 3620 2020 7c0a 7c20   |  0.916   |.| 
-00006580: 2020 2060 5669 5455 6e69 636f 6d45 7874     `ViTUnicomExt
-00006590: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
-000065a0: 7261 696e 6564 2822 7669 7462 3332 5f75  rained("vitb32_u
-000065b0: 6e69 636f 6d22 2960 2020 2020 207c 2020  nicom")`     |  
-000065c0: 2020 2020 2020 2020 302e 3639 3020 2020          0.690   
-000065d0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000065e0: 302e 3732 3220 2020 2020 2020 207c 2020  0.722        |  
-000065f0: 2020 302e 3739 3620 2020 2020 7c20 2030    0.796     |  0
-00006600: 2e38 3933 2020 207c 0a7c 2020 2020 6056  .893   |.|    `V
-00006610: 6954 556e 6963 6f6d 4578 7472 6163 746f  iTUnicomExtracto
-00006620: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-00006630: 6428 2276 6974 6c31 345f 756e 6963 6f6d  d("vitl14_unicom
-00006640: 2229 6020 2020 2020 7c20 2020 2020 2020  ")`     |       
-00006650: 2020 2030 2e37 3236 2020 2020 2020 2020     0.726        
-00006660: 2020 207c 2020 2020 2020 2030 2e37 3930     |       0.790
-00006670: 2020 2020 2020 2020 7c20 2020 2030 2e38          |    0.8
-00006680: 3638 2020 2020 207c 2020 302e 3932 3220  68     |  0.922 
-00006690: 2020 7c0a 7c20 6056 6954 556e 6963 6f6d    |.| `ViTUnicom
-000066a0: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-000066b0: 7265 7472 6169 6e65 6428 2276 6974 6c31  retrained("vitl1
-000066c0: 345f 3333 3670 785f 756e 6963 6f6d 2229  4_336px_unicom")
-000066d0: 6020 207c 2020 2020 2020 2020 2020 302e  `  |          0.
-000066e0: 3734 3520 2020 2020 2020 2020 2020 7c20  745           | 
-000066f0: 2020 2020 2020 302e 3831 3020 2020 2020        0.810     
-00006700: 2020 207c 2020 2020 302e 3837 3520 2020     |    0.875   
-00006710: 2020 7c20 2030 2e39 3234 2020 207c 0a7c    |  0.924   |.|
-00006720: 2020 2020 6056 6954 434c 4950 4578 7472      `ViTCLIPExtr
-00006730: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-00006740: 6169 6e65 6428 2273 6265 725f 7669 7462  ained("sber_vitb
-00006750: 3332 5f32 3234 2229 6020 2020 2020 7c20  32_224")`     | 
-00006760: 2020 2020 2020 2020 2030 2e35 3437 2020           0.547  
-00006770: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00006780: 2030 2e35 3134 2020 2020 2020 2020 7c20   0.514        | 
-00006790: 2020 2030 2e34 3438 2020 2020 207c 2020     0.448     |  
-000067a0: 302e 3631 3820 2020 7c0a 7c20 2020 2060  0.618   |.|    `
-000067b0: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-000067c0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-000067d0: 2822 7362 6572 5f76 6974 6231 365f 3232  ("sber_vitb16_22
-000067e0: 3422 2960 2020 2020 207c 2020 2020 2020  4")`     |      
-000067f0: 2020 2020 302e 3536 3520 2020 2020 2020      0.565       
-00006800: 2020 2020 7c20 2020 2020 2020 302e 3536      |       0.56
-00006810: 3520 2020 2020 2020 207c 2020 2020 302e  5        |    0.
-00006820: 3532 3420 2020 2020 7c20 2030 2e36 3438  524     |  0.648
-00006830: 2020 207c 0a7c 2020 2020 6056 6954 434c     |.|    `ViTCL
-00006840: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-00006850: 5f70 7265 7472 6169 6e65 6428 2273 6265  _pretrained("sbe
-00006860: 725f 7669 746c 3134 5f32 3234 2229 6020  r_vitl14_224")` 
-00006870: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
-00006880: 2e35 3132 2020 2020 2020 2020 2020 207c  .512           |
-00006890: 2020 2020 2020 2030 2e35 3535 2020 2020         0.555    
-000068a0: 2020 2020 7c20 2020 2030 2e36 3036 2020      |    0.606  
-000068b0: 2020 207c 2020 302e 3730 3720 2020 7c0a     |  0.707   |.
-000068c0: 7c20 2020 6056 6954 434c 4950 4578 7472  |   `ViTCLIPExtr
-000068d0: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-000068e0: 6169 6e65 6428 226f 7065 6e61 695f 7669  ained("openai_vi
-000068f0: 7462 3332 5f32 3234 2229 6020 2020 207c  tb32_224")`    |
-00006900: 2020 2020 2020 2020 2020 302e 3631 3220            0.612 
-00006910: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00006920: 2020 302e 3439 3120 2020 2020 2020 207c    0.491        |
-00006930: 2020 2020 302e 3536 3020 2020 2020 7c20      0.560     | 
-00006940: 2030 2e36 3933 2020 207c 0a7c 2020 2060   0.693   |.|   `
-00006950: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-00006960: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-00006970: 2822 6f70 656e 6169 5f76 6974 6231 365f  ("openai_vitb16_
-00006980: 3232 3422 2960 2020 2020 7c20 2020 2020  224")`    |     
-00006990: 2020 2020 2030 2e36 3438 2020 2020 2020       0.648      
-000069a0: 2020 2020 207c 2020 2020 2020 2030 2e36       |       0.6
-000069b0: 3036 2020 2020 2020 2020 7c20 2020 2030  06        |    0
-000069c0: 2e36 3635 2020 2020 207c 2020 302e 3736  .665     |  0.76
-000069d0: 3720 2020 7c0a 7c20 2020 6056 6954 434c  7   |.|   `ViTCL
-000069e0: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-000069f0: 5f70 7265 7472 6169 6e65 6428 226f 7065  _pretrained("ope
-00006a00: 6e61 695f 7669 746c 3134 5f32 3234 2229  nai_vitl14_224")
-00006a10: 6020 2020 207c 2020 2020 2020 2020 2020  `    |          
-00006a20: 302e 3637 3020 2020 2020 2020 2020 2020  0.670           
-00006a30: 7c20 2020 2020 2020 302e 3637 3520 2020  |       0.675   
-00006a40: 2020 2020 207c 2020 2020 302e 3734 3520       |    0.745 
-00006a50: 2020 2020 7c20 2030 2e38 3434 2020 207c      |  0.844   |
-00006a60: 0a7c 2020 2020 2020 2020 6056 6954 4578  .|        `ViTEx
-00006a70: 7472 6163 746f 722e 6672 6f6d 5f70 7265  tractor.from_pre
-00006a80: 7472 6169 6e65 6428 2276 6974 7331 365f  trained("vits16_
-00006a90: 6469 6e6f 2229 6020 2020 2020 2020 2020  dino")`         
-00006aa0: 7c20 2020 2020 2020 2020 2030 2e36 3438  |          0.648
-00006ab0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00006ac0: 2020 2030 2e35 3039 2020 2020 2020 2020     0.509        
-00006ad0: 7c20 2020 2030 2e36 3237 2020 2020 207c  |    0.627     |
-00006ae0: 2020 302e 3236 3520 2020 7c0a 7c20 2020    0.265   |.|   
-00006af0: 2020 2020 2020 6056 6954 4578 7472 6163        `ViTExtrac
-00006b00: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
-00006b10: 6e65 6428 2276 6974 7338 5f64 696e 6f22  ned("vits8_dino"
-00006b20: 2960 2020 2020 2020 2020 207c 2020 2020  )`         |    
-00006b30: 2020 2020 2020 302e 3635 3120 2020 2020        0.651     
-00006b40: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
-00006b50: 3532 3420 2020 2020 2020 207c 2020 2020  524        |    
-00006b60: 302e 3636 3120 2020 2020 7c20 2030 2e33  0.661     |  0.3
-00006b70: 3135 2020 207c 0a7c 2020 2020 2020 2020  15   |.|        
-00006b80: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00006b90: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006ba0: 6974 6231 365f 6469 6e6f 2229 6020 2020  itb16_dino")`   
-00006bb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00006bc0: 2030 2e36 3538 2020 2020 2020 2020 2020   0.658          
-00006bd0: 207c 2020 2020 2020 2030 2e35 3134 2020   |       0.514  
-00006be0: 2020 2020 2020 7c20 2020 2030 2e35 3431        |    0.541
-00006bf0: 2020 2020 207c 2020 302e 3238 3820 2020       |  0.288   
-00006c00: 7c0a 7c20 2020 2020 2020 2020 6056 6954  |.|         `ViT
-00006c10: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-00006c20: 7265 7472 6169 6e65 6428 2276 6974 6238  retrained("vitb8
-00006c30: 5f64 696e 6f22 2960 2020 2020 2020 2020  _dino")`        
-00006c40: 207c 2020 2020 2020 2020 2020 302e 3638   |          0.68
-00006c50: 3920 2020 2020 2020 2020 2020 7c20 2020  9           |   
-00006c60: 2020 2020 302e 3539 3920 2020 2020 2020      0.599       
-00006c70: 207c 2020 2020 302e 3530 3620 2020 2020   |    0.506     
-00006c80: 7c20 2030 2e33 3133 2020 207c 0a7c 2020  |  0.313   |.|  
-00006c90: 2020 6052 6573 6e65 7445 7874 7261 6374    `ResnetExtract
-00006ca0: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
-00006cb0: 6564 2822 7265 736e 6574 3530 5f6d 6f63  ed("resnet50_moc
-00006cc0: 6f5f 7632 2229 6020 2020 2020 7c20 2020  o_v2")`     |   
-00006cd0: 2020 2020 2020 2030 2e34 3933 2020 2020         0.493    
-00006ce0: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
-00006cf0: 2e32 3637 2020 2020 2020 2020 7c20 2020  .267        |   
-00006d00: 2030 2e32 3634 2020 2020 207c 2020 302e   0.264     |  0.
-00006d10: 3134 3920 2020 7c0a 7c20 6052 6573 6e65  149   |.| `Resne
-00006d20: 7445 7874 7261 6374 6f72 2e66 726f 6d5f  tExtractor.from_
-00006d30: 7072 6574 7261 696e 6564 2822 7265 736e  pretrained("resn
-00006d40: 6574 3530 5f69 6d61 6765 6e65 7431 6b5f  et50_imagenet1k_
-00006d50: 7631 2229 6020 207c 2020 2020 2020 2020  v1")`  |        
-00006d60: 2020 302e 3531 3520 2020 2020 2020 2020    0.515         
-00006d70: 2020 7c20 2020 2020 2020 302e 3238 3420    |       0.284 
-00006d80: 2020 2020 2020 207c 2020 2020 302e 3435         |    0.45
-00006d90: 3520 2020 2020 7c20 2030 2e32 3437 2020  5     |  0.247  
-00006da0: 207c 0a0a 2a2a 5468 6520 6d65 7472 6963   |..**The metric
-00006db0: 7320 6d61 7920 6265 2064 6966 6665 7265  s may be differe
-00006dc0: 6e74 2066 726f 6d20 7468 6520 6f6e 6573  nt from the ones
-00006dd0: 2072 6570 6f72 7465 6420 6279 2070 6170   reported by pap
-00006de0: 6572 732c 0a62 6563 6175 7365 2074 6865  ers,.because the
-00006df0: 2076 6572 7369 6f6e 206f 6620 7472 6169   version of trai
-00006e00: 6e2f 7661 6c20 7370 6c69 7420 616e 6420  n/val split and 
-00006e10: 7573 6167 6520 6f66 2062 6f75 6e64 696e  usage of boundin
-00006e20: 6720 626f 7865 7320 6d61 7920 6469 6666  g boxes may diff
-00006e30: 6572 2e0a 5061 7274 6963 756c 6172 6c79  er..Particularly
-00006e40: 2c20 7765 2075 7365 6420 626f 756e 6469  , we used boundi
-00006e50: 6e67 2062 6f78 6573 2064 7572 696e 6720  ng boxes during 
-00006e60: 7468 6520 6576 616c 7561 7469 6f6e 2e2a  the evaluation.*
-00006e70: 0a0a 2323 2320 486f 7720 746f 2075 7365  ..### How to use
-00006e80: 206d 6f64 656c 7320 6672 6f6d 205a 6f6f   models from Zoo
-00006e90: 3f0a 0a5b 636f 6d6d 656e 745d 3a7a 6f6f  ?..[comment]:zoo
-00006ea0: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
-00006eb0: 0a66 726f 6d20 6f6d 6c2e 636f 6e73 7420  .from oml.const 
-00006ec0: 696d 706f 7274 2043 4b50 545f 5341 5645  import CKPT_SAVE
-00006ed0: 5f52 4f4f 5420 6173 2043 4b50 545f 4449  _ROOT as CKPT_DI
-00006ee0: 522c 204d 4f43 4b5f 4441 5441 5345 545f  R, MOCK_DATASET_
-00006ef0: 5041 5448 2061 7320 4441 5441 5f44 4952  PATH as DATA_DIR
-00006f00: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
-00006f10: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00006f20: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7265  ctor.from oml.re
-00006f30: 6769 7374 7279 2e74 7261 6e73 666f 726d  gistry.transform
-00006f40: 7320 696d 706f 7274 2067 6574 5f74 7261  s import get_tra
-00006f50: 6e73 666f 726d 735f 666f 725f 7072 6574  nsforms_for_pret
-00006f60: 7261 696e 6564 0a0a 6d6f 6465 6c20 3d20  rained..model = 
-00006f70: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
-00006f80: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
-00006f90: 7473 3136 5f64 696e 6f22 290a 7472 616e  ts16_dino").tran
-00006fa0: 7366 6f72 6d73 2c20 696d 5f72 6561 6465  sforms, im_reade
-00006fb0: 7220 3d20 6765 745f 7472 616e 7366 6f72  r = get_transfor
-00006fc0: 6d73 5f66 6f72 5f70 7265 7472 6169 6e65  ms_for_pretraine
-00006fd0: 6428 2276 6974 7331 365f 6469 6e6f 2229  d("vits16_dino")
-00006fe0: 0a0a 696d 6720 3d20 696d 5f72 6561 6465  ..img = im_reade
-00006ff0: 7228 4441 5441 5f44 4952 202f 2022 696d  r(DATA_DIR / "im
-00007000: 6167 6573 2220 2f20 2263 6972 636c 655f  ages" / "circle_
-00007010: 312e 6a70 6722 2920 2023 2070 7574 2070  1.jpg")  # put p
-00007020: 6174 6820 746f 2079 6f75 7220 696d 6167  ath to your imag
-00007030: 6520 6865 7265 0a69 6d67 5f74 656e 736f  e here.img_tenso
-00007040: 7220 3d20 7472 616e 7366 6f72 6d73 2869  r = transforms(i
-00007050: 6d67 290a 2320 696d 675f 7465 6e73 6f72  mg).# img_tensor
-00007060: 203d 2074 7261 6e73 666f 726d 7328 696d   = transforms(im
-00007070: 6167 653d 696d 6729 5b22 696d 6167 6522  age=img)["image"
-00007080: 5d20 2023 2066 6f72 2074 7261 6e73 666f  ]  # for transfo
-00007090: 726d 7320 6672 6f6d 2041 6c62 756d 656e  rms from Albumen
-000070a0: 7461 7469 6f6e 730a 0a66 6561 7475 7265  tations..feature
-000070b0: 7320 3d20 6d6f 6465 6c28 696d 675f 7465  s = model(img_te
-000070c0: 6e73 6f72 2e75 6e73 7175 6565 7a65 2830  nsor.unsqueeze(0
-000070d0: 2929 0a0a 2320 4368 6563 6b20 6f74 6865  ))..# Check othe
-000070e0: 7220 6176 6169 6c61 626c 6520 6d6f 6465  r available mode
-000070f0: 6c73 3a0a 7072 696e 7428 6c69 7374 2856  ls:.print(list(V
-00007100: 6954 4578 7472 6163 746f 722e 7072 6574  iTExtractor.pret
-00007110: 7261 696e 6564 5f6d 6f64 656c 732e 6b65  rained_models.ke
-00007120: 7973 2829 2929 0a0a 2320 4c6f 6164 2063  ys()))..# Load c
-00007130: 6865 636b 706f 696e 7420 7361 7665 6420  heckpoint saved 
-00007140: 6f6e 2061 2064 6973 6b3a 0a6d 6f64 656c  on a disk:.model
-00007150: 5f20 3d20 5669 5445 7874 7261 6374 6f72  _ = ViTExtractor
-00007160: 2877 6569 6768 7473 3d43 4b50 545f 4449  (weights=CKPT_DI
-00007170: 5220 2f20 2276 6974 7331 365f 6469 6e6f  R / "vits16_dino
-00007180: 2e63 6b70 7422 2c20 6172 6368 3d22 7669  .ckpt", arch="vi
-00007190: 7473 3136 222c 206e 6f72 6d61 6c69 7365  ts16", normalise
-000071a0: 5f66 6561 7475 7265 733d 4661 6c73 6529  _features=False)
-000071b0: 0a60 6060 0a5b 636f 6d6d 656e 745d 3a7a  .```.[comment]:z
-000071c0: 6f6f 2d65 6e64 0a0a 2323 205b 436f 6e74  oo-end..## [Cont
-000071d0: 7269 6275 7469 6e67 2067 7569 6465 5d28  ributing guide](
-000071e0: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
-000071f0: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
-00007200: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00007210: 6174 6573 742f 6f6d 6c2f 636f 6e74 7269  atest/oml/contri
-00007220: 6275 7469 6e67 2e68 746d 6c29 0a0a 5765  buting.html)..We
-00007230: 2077 656c 636f 6d65 206e 6577 2063 6f6e   welcome new con
-00007240: 7472 6962 7574 6f72 7321 2050 6c65 6173  tributors! Pleas
-00007250: 652c 2073 6565 206f 7572 3a0a 2a20 5b43  e, see our:.* [C
-00007260: 6f6e 7472 6962 7574 696e 6720 6775 6964  ontributing guid
-00007270: 655d 2868 7474 7073 3a2f 2f6f 7065 6e2d  e](https://open-
-00007280: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-00007290: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000072a0: 6e2f 6c61 7465 7374 2f66 726f 6d5f 7265  n/latest/from_re
-000072b0: 6164 6d65 2f63 6f6e 7472 6962 7574 696e  adme/contributin
-000072c0: 672e 6874 6d6c 290a 2a20 5b4b 616e 6261  g.html).* [Kanba
-000072d0: 6e20 626f 6172 645d 2868 7474 7073 3a2f  n board](https:/
-000072e0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
-000072f0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
-00007300: 2d6c 6561 726e 696e 672f 7072 6f6a 6563  -learning/projec
-00007310: 7473 2f31 290a 0a23 2320 4163 6b6e 6f77  ts/1)..## Acknow
-00007320: 6c65 6467 6d65 6e74 730a 0a3c 6120 6872  ledgments..<a hr
-00007330: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00007340: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00007350: 7465 616d 2f63 6174 616c 7973 7422 2074  team/catalyst" t
-00007360: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00007370: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00007380: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00007390: 6f6e 7465 6e74 2e63 6f6d 2f63 6174 616c  ontent.com/catal
-000073a0: 7973 742d 7465 616d 2f63 6174 616c 7973  yst-team/catalys
-000073b0: 742d 7069 6373 2f6d 6173 7465 722f 7069  t-pics/master/pi
-000073c0: 6373 2f63 6174 616c 7973 745f 6c6f 676f  cs/catalyst_logo
-000073d0: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
-000073e0: 222f 3e3c 2f61 3e0a 0a54 6865 2070 726f  "/></a>..The pro
-000073f0: 6a65 6374 2077 6173 2073 7461 7274 6564  ject was started
-00007400: 2069 6e20 3230 3230 2061 7320 6120 6d6f   in 2020 as a mo
-00007410: 6475 6c65 2066 6f72 205b 4361 7461 6c79  dule for [Cataly
-00007420: 7374 5d28 6874 7470 733a 2f2f 6769 7468  st](https://gith
-00007430: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00007440: 7465 616d 2f63 6174 616c 7973 7429 206c  team/catalyst) l
-00007450: 6962 7261 7279 2e0a 4920 7761 6e74 2074  ibrary..I want t
-00007460: 6f20 7468 616e 6b20 7065 6f70 6c65 2077  o thank people w
-00007470: 686f 2077 6f72 6b65 6420 7769 7468 206d  ho worked with m
-00007480: 6520 6f6e 2074 6861 7420 6d6f 6475 6c65  e on that module
-00007490: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
-000074a0: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
-000074b0: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
-000074c0: 6e73 6869 6e61 292c 0a5b 4e69 6b69 7461  nshina),.[Nikita
-000074d0: 2042 616c 6167 616e 736b 795d 2868 7474   Balagansky](htt
-000074e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000074f0: 656c 6570 6861 6e74 6d69 7074 292c 0a5b  elephantmipt),.[
-00007500: 5365 7267 6579 204b 6f6c 6573 6e69 6b6f  Sergey Kolesniko
-00007510: 765d 2868 7474 7073 3a2f 2f67 6974 6875  v](https://githu
-00007520: 622e 636f 6d2f 5363 6974 6174 6f72 290a  b.com/Scitator).
-00007530: 616e 6420 6f74 6865 7273 2e0a 0a49 2077  and others...I w
-00007540: 6f75 6c64 206c 696b 6520 746f 2074 6861  ould like to tha
-00007550: 6e6b 2070 656f 706c 6520 7768 6f20 636f  nk people who co
-00007560: 6e74 696e 7565 2077 6f72 6b69 6e67 206f  ntinue working o
-00007570: 6e20 7468 6973 2070 6970 656c 696e 6520  n this pipeline 
-00007580: 7768 656e 2069 7420 6265 6361 6d65 2061  when it became a
-00007590: 2073 6570 6172 6520 7072 6f6a 6563 743a   separe project:
-000075a0: 0a5b 4a75 6c69 6120 5368 656e 7368 696e  .[Julia Shenshin
-000075b0: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-000075c0: 622e 636f 6d2f 6a75 6c69 612d 7368 656e  b.com/julia-shen
-000075d0: 7368 696e 6129 2c0a 5b4d 6973 6861 204b  shina),.[Misha K
-000075e0: 696e 6475 6c6f 765d 2868 7474 7073 3a2f  indulov](https:/
-000075f0: 2f67 6974 6875 622e 636f 6d2f 6230 6e63  /github.com/b0nc
-00007600: 6529 2c0a 5b41 6c65 6b73 6569 2054 6172  e),.[Aleksei Tar
-00007610: 6173 6f76 5d28 6874 7470 733a 2f2f 6769  asov](https://gi
-00007620: 7468 7562 2e63 6f6d 2f44 616c 6f72 6f41  thub.com/DaloroA
-00007630: 5429 2061 6e64 0a5b 5665 726b 686f 7674  T) and.[Verkhovt
-00007640: 7365 7620 4c65 6f6e 6964 5d28 6874 7470  sev Leonid](http
-00007650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00007660: 656f 726f 6d61 6e6f 7669 6368 292e 0a0a  eoromanovich)...
-00007670: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00007680: 2f77 7777 2e6e 6577 796f 726b 6572 2e64  /www.newyorker.d
-00007690: 652f 2220 7461 7267 6574 3d22 5f62 6c61  e/" target="_bla
-000076a0: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
-000076b0: 7470 733a 2f2f 7570 6c6f 6164 2e77 696b  tps://upload.wik
-000076c0: 696d 6564 6961 2e6f 7267 2f77 696b 6970  imedia.org/wikip
-000076d0: 6564 6961 2f63 6f6d 6d6f 6e73 2f74 6875  edia/commons/thu
-000076e0: 6d62 2f64 2f64 382f 4e65 775f 596f 726b  mb/d/d8/New_York
-000076f0: 6572 2e73 7667 2f31 3238 3070 782d 4e65  er.svg/1280px-Ne
-00007700: 775f 596f 726b 6572 2e73 7667 2e70 6e67  w_Yorker.svg.png
-00007710: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
-00007720: 2f61 3e0a 0a49 2061 6c73 6f20 7761 6e74  /a>..I also want
-00007730: 2074 6f20 7468 616e 6b20 4e65 7759 6f72   to thank NewYor
-00007740: 6b65 722c 2073 696e 6365 2074 6865 2070  ker, since the p
-00007750: 6172 7420 6f66 2066 756e 6374 696f 6e61  art of functiona
-00007760: 6c69 7479 2077 6173 2064 6576 656c 6f70  lity was develop
-00007770: 6564 2028 616e 6420 7573 6564 2920 6279  ed (and used) by
-00007780: 2069 7473 2063 6f6d 7075 7465 7220 7669   its computer vi
-00007790: 7369 6f6e 2074 6561 6d20 6c65 6420 6279  sion team led by
-000077a0: 206d 652e 0a                              me..
+000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064d0: 2d2d 2d2d 2d2d 3a7c 0a7c 2060 5669 5445  ------:|.| `ViTE
+000064e0: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+000064f0: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00006500: 5f69 6e73 686f 7022 2960 207c 2030 2e39  _inshop")` | 0.9
+00006510: 3231 207c 2020 2020 4465 6570 4661 7368  21 |    DeepFash
+00006520: 696f 6e20 496e 7368 6f70 2020 2020 7c20  ion Inshop    | 
+00006530: 2020 205b 6c69 6e6b 5d28 6874 7470 733a     [link](https:
+00006540: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00006550: 6f6d 2f66 696c 652f 642f 316e 6958 2d54  om/file/d/1niX-T
+00006560: 4338 636a 366a 3336 3974 3769 5532 6261  C8cj6j369t7iU2ba
+00006570: 4851 5356 4e33 4d56 4a62 572f 7669 6577  HQSVN3MVJbW/view
+00006580: 3f75 7370 3d73 6861 7269 6e67 2920 2020  ?usp=sharing)   
+00006590: 2020 7c20 5b6c 696e 6b5d 2868 7474 7073    | [link](https
+000065a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000065b0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000065c0: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+000065d0: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+000065e0: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+000065f0: 696f 6e2f 6578 7472 6163 746f 725f 696e  ion/extractor_in
+00006600: 7368 6f70 2920 7c0a 7c20 2060 5669 5445  shop) |.|  `ViTE
+00006610: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00006620: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00006630: 5f73 6f70 2229 6020 2020 7c20 302e 3836  _sop")`   | 0.86
+00006640: 3620 7c20 5374 616e 666f 7264 204f 6e6c  6 | Stanford Onl
+00006650: 696e 6520 5072 6f64 7563 7473 207c 2020  ine Products |  
+00006660: 205b 6c69 6e6b 5d28 6874 7470 733a 2f2f   [link](https://
+00006670: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
+00006680: 2f66 696c 652f 642f 317a 7547 5248 7646  /file/d/1zuGRHvF
+00006690: 324b 4864 3539 6177 3769 3733 3637 4f48  2KHd59aw7i7367OH
+000066a0: 5f74 514e 4f47 7a37 412f 7669 6577 3f75  _tQNOGz7A/view?u
+000066b0: 7370 3d73 6861 7269 6e67 2920 2020 2020  sp=sharing)     
+000066c0: 207c 2020 5b6c 696e 6b5d 2868 7474 7073   |  [link](https
+000066d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000066e0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000066f0: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+00006700: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+00006710: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+00006720: 696f 6e2f 6578 7472 6163 746f 725f 736f  ion/extractor_so
+00006730: 7029 2020 207c 0a7c 2060 5669 5445 7874  p)   |.| `ViTExt
+00006740: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+00006750: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+00006760: 6172 7322 2960 2020 207c 2030 2e39 3037  ars")`   | 0.907
+00006770: 207c 2020 2020 2020 2020 2043 4152 5320   |         CARS 
+00006780: 3139 3620 2020 2020 2020 2020 7c20 2020  196         |   
+00006790: 5b6c 696e 6b5d 2868 7474 7073 3a2f 2f64  [link](https://d
+000067a0: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+000067b0: 6472 6976 652f 666f 6c64 6572 732f 3137  drive/folders/17
+000067c0: 6134 5f66 6739 3464 6f78 3273 666b 586d  a4_fg94dox2sfkXm
+000067d0: 772d 4b43 7469 4c42 6c78 2d75 742d 313f  w-KCtiLBlx-ut-1?
+000067e0: 7573 703d 7368 6172 696e 6729 2020 2020  usp=sharing)    
+000067f0: 7c20 205b 6c69 6e6b 5d28 6874 7470 733a  |  [link](https:
+00006800: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00006810: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00006820: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+00006830: 6d61 696e 2f70 6970 656c 696e 6573 2f66  main/pipelines/f
+00006840: 6561 7475 7265 735f 6578 7472 6163 7469  eatures_extracti
+00006850: 6f6e 2f65 7874 7261 6374 6f72 5f63 6172  on/extractor_car
+00006860: 7329 2020 7c0a 7c20 2060 5669 5445 7874  s)  |.|  `ViTExt
+00006870: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+00006880: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+00006890: 7562 2229 6020 2020 7c20 302e 3833 3720  ub")`   | 0.837 
+000068a0: 7c20 2020 2020 2020 4355 4220 3230 3020  |       CUB 200 
+000068b0: 3230 3131 2020 2020 2020 207c 2020 205b  2011       |   [
+000068c0: 6c69 6e6b 5d28 6874 7470 733a 2f2f 6472  link](https://dr
+000068d0: 6976 652e 676f 6f67 6c65 2e63 6f6d 2f64  ive.google.com/d
+000068e0: 7269 7665 2f66 6f6c 6465 7273 2f31 5450  rive/folders/1TP
+000068f0: 434e 2d65 5a46 4c71 6f71 344a 4267 6e49  CN-eZFLqoq4JBgnI
+00006900: 666c 694a 6f45 4b34 3878 396f 7a62 3f75  fliJoEK48x9ozb?u
+00006910: 7370 3d73 6861 7269 6e67 2920 2020 207c  sp=sharing)    |
+00006920: 2020 5b6c 696e 6b5d 2868 7474 7073 3a2f    [link](https:/
+00006930: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+00006940: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+00006950: 2d6c 6561 726e 696e 672f 7472 6565 2f6d  -learning/tree/m
+00006960: 6169 6e2f 7069 7065 6c69 6e65 732f 6665  ain/pipelines/fe
+00006970: 6174 7572 6573 5f65 7874 7261 6374 696f  atures_extractio
+00006980: 6e2f 6578 7472 6163 746f 725f 6375 6229  n/extractor_cub)
+00006990: 2020 207c 0a0a 5765 2061 6c73 6f20 7072     |..We also pr
+000069a0: 6f76 6964 6520 616e 2069 6e74 6567 7261  ovide an integra
+000069b0: 7469 6f6e 2077 6974 6820 7468 6520 6d6f  tion with the mo
+000069c0: 6465 6c73 2070 7265 7472 6169 6e65 6420  dels pretrained 
+000069d0: 6279 206f 7468 6572 2072 6573 6561 7263  by other researc
+000069e0: 6865 7273 2e0a 416c 6c20 6d65 7472 6963  hers..All metric
+000069f0: 7320 6265 6c6f 7720 7765 7265 206f 6274  s below were obt
+00006a00: 6169 6e65 6420 6f6e 2074 6865 2069 6d61  ained on the ima
+00006a10: 6765 7320 7769 7468 2074 6865 2073 697a  ges with the siz
+00006a20: 6573 206f 6620 2a2a 3232 3420 7820 3232  es of **224 x 22
+00006a30: 342a 2a3a 0a0a 7c20 2020 2020 2020 2020  4**:..|         
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 206d 6f64 656c 2020 2020 2020 2020     model        
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 207c 2053 7461 6e66 6f72 6420       | Stanford 
+00006a80: 4f6e 6c69 6e65 2050 726f 6475 6374 7320  Online Products 
+00006a90: 7c20 4465 6570 4661 7368 696f 6e20 496e  | DeepFashion In
+00006aa0: 5368 6f70 207c 2043 5542 2032 3030 2032  Shop | CUB 200 2
+00006ab0: 3031 3120 7c20 4341 5253 2031 3936 207c  011 | CARS 196 |
+00006ac0: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
+00006ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00006b00: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00006b10: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  ----------:|:---
+00006b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00006b30: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  |:------------:|
+00006b40: 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020  :--------:|.|   
+00006b50: 2060 5669 5455 6e69 636f 6d45 7874 7261   `ViTUnicomExtra
+00006b60: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006b70: 696e 6564 2822 7669 7462 3136 5f75 6e69  ined("vitb16_uni
+00006b80: 636f 6d22 2960 2020 2020 207c 2020 2020  com")`     |    
+00006b90: 2020 2020 2020 302e 3730 3020 2020 2020        0.700     
+00006ba0: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
+00006bb0: 3733 3420 2020 2020 2020 207c 2020 2020  734        |    
+00006bc0: 302e 3834 3720 2020 2020 7c20 2030 2e39  0.847     |  0.9
+00006bd0: 3136 2020 207c 0a7c 2020 2020 6056 6954  16   |.|    `ViT
+00006be0: 556e 6963 6f6d 4578 7472 6163 746f 722e  UnicomExtractor.
+00006bf0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+00006c00: 2276 6974 6233 325f 756e 6963 6f6d 2229  "vitb32_unicom")
+00006c10: 6020 2020 2020 7c20 2020 2020 2020 2020  `     |         
+00006c20: 2030 2e36 3930 2020 2020 2020 2020 2020   0.690          
+00006c30: 207c 2020 2020 2020 2030 2e37 3232 2020   |       0.722  
+00006c40: 2020 2020 2020 7c20 2020 2030 2e37 3936        |    0.796
+00006c50: 2020 2020 207c 2020 302e 3839 3320 2020       |  0.893   
+00006c60: 7c0a 7c20 2020 2060 5669 5455 6e69 636f  |.|    `ViTUnico
+00006c70: 6d45 7874 7261 6374 6f72 2e66 726f 6d5f  mExtractor.from_
+00006c80: 7072 6574 7261 696e 6564 2822 7669 746c  pretrained("vitl
+00006c90: 3134 5f75 6e69 636f 6d22 2960 2020 2020  14_unicom")`    
+00006ca0: 207c 2020 2020 2020 2020 2020 302e 3732   |          0.72
+00006cb0: 3620 2020 2020 2020 2020 2020 7c20 2020  6           |   
+00006cc0: 2020 2020 302e 3739 3020 2020 2020 2020      0.790       
+00006cd0: 207c 2020 2020 302e 3836 3820 2020 2020   |    0.868     
+00006ce0: 7c20 2030 2e39 3232 2020 207c 0a7c 2060  |  0.922   |.| `
+00006cf0: 5669 5455 6e69 636f 6d45 7874 7261 6374  ViTUnicomExtract
+00006d00: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00006d10: 6564 2822 7669 746c 3134 5f33 3336 7078  ed("vitl14_336px
+00006d20: 5f75 6e69 636f 6d22 2960 2020 7c20 2020  _unicom")`  |   
+00006d30: 2020 2020 2020 2030 2e37 3435 2020 2020         0.745    
+00006d40: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
+00006d50: 2e38 3130 2020 2020 2020 2020 7c20 2020  .810        |   
+00006d60: 2030 2e38 3735 2020 2020 207c 2020 302e   0.875     |  0.
+00006d70: 3932 3420 2020 7c0a 7c20 2020 2060 5669  924   |.|    `Vi
+00006d80: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+00006d90: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00006da0: 7362 6572 5f76 6974 6233 325f 3232 3422  sber_vitb32_224"
+00006db0: 2960 2020 2020 207c 2020 2020 2020 2020  )`     |        
+00006dc0: 2020 302e 3534 3720 2020 2020 2020 2020    0.547         
+00006dd0: 2020 7c20 2020 2020 2020 302e 3531 3420    |       0.514 
+00006de0: 2020 2020 2020 207c 2020 2020 302e 3434         |    0.44
+00006df0: 3820 2020 2020 7c20 2030 2e36 3138 2020  8     |  0.618  
+00006e00: 207c 0a7c 2020 2020 6056 6954 434c 4950   |.|    `ViTCLIP
+00006e10: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006e20: 7265 7472 6169 6e65 6428 2273 6265 725f  retrained("sber_
+00006e30: 7669 7462 3136 5f32 3234 2229 6020 2020  vitb16_224")`   
+00006e40: 2020 7c20 2020 2020 2020 2020 2030 2e35    |          0.5
+00006e50: 3635 2020 2020 2020 2020 2020 207c 2020  65           |  
+00006e60: 2020 2020 2030 2e35 3635 2020 2020 2020       0.565      
+00006e70: 2020 7c20 2020 2030 2e35 3234 2020 2020    |    0.524    
+00006e80: 207c 2020 302e 3634 3820 2020 7c0a 7c20   |  0.648   |.| 
+00006e90: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00006ea0: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006eb0: 696e 6564 2822 7362 6572 5f76 6974 6c31  ined("sber_vitl1
+00006ec0: 345f 3232 3422 2960 2020 2020 207c 2020  4_224")`     |  
+00006ed0: 2020 2020 2020 2020 302e 3531 3220 2020          0.512   
+00006ee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006ef0: 302e 3535 3520 2020 2020 2020 207c 2020  0.555        |  
+00006f00: 2020 302e 3630 3620 2020 2020 7c20 2030    0.606     |  0
+00006f10: 2e37 3037 2020 207c 0a7c 2020 2060 5669  .707   |.|   `Vi
+00006f20: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+00006f30: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00006f40: 6f70 656e 6169 5f76 6974 6233 325f 3232  openai_vitb32_22
+00006f50: 3422 2960 2020 2020 7c20 2020 2020 2020  4")`    |       
+00006f60: 2020 2030 2e36 3132 2020 2020 2020 2020     0.612        
+00006f70: 2020 207c 2020 2020 2020 2030 2e34 3931     |       0.491
+00006f80: 2020 2020 2020 2020 7c20 2020 2030 2e35          |    0.5
+00006f90: 3630 2020 2020 207c 2020 302e 3639 3320  60     |  0.693 
+00006fa0: 2020 7c0a 7c20 2020 6056 6954 434c 4950    |.|   `ViTCLIP
+00006fb0: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006fc0: 7265 7472 6169 6e65 6428 226f 7065 6e61  retrained("opena
+00006fd0: 695f 7669 7462 3136 5f32 3234 2229 6020  i_vitb16_224")` 
+00006fe0: 2020 207c 2020 2020 2020 2020 2020 302e     |          0.
+00006ff0: 3634 3820 2020 2020 2020 2020 2020 7c20  648           | 
+00007000: 2020 2020 2020 302e 3630 3620 2020 2020        0.606     
+00007010: 2020 207c 2020 2020 302e 3636 3520 2020     |    0.665   
+00007020: 2020 7c20 2030 2e37 3637 2020 207c 0a7c    |  0.767   |.|
+00007030: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00007040: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00007050: 696e 6564 2822 6f70 656e 6169 5f76 6974  ined("openai_vit
+00007060: 6c31 345f 3232 3422 2960 2020 2020 7c20  l14_224")`    | 
+00007070: 2020 2020 2020 2020 2030 2e36 3730 2020           0.670  
+00007080: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00007090: 2030 2e36 3735 2020 2020 2020 2020 7c20   0.675        | 
+000070a0: 2020 2030 2e37 3435 2020 2020 207c 2020     0.745     |  
+000070b0: 302e 3834 3420 2020 7c0a 7c20 2020 2020  0.844   |.|     
+000070c0: 2020 2060 5669 5445 7874 7261 6374 6f72     `ViTExtractor
+000070d0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+000070e0: 2822 7669 7473 3136 5f64 696e 6f22 2960  ("vits16_dino")`
+000070f0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00007100: 2020 2020 302e 3634 3820 2020 2020 2020      0.648       
+00007110: 2020 2020 7c20 2020 2020 2020 302e 3530      |       0.50
+00007120: 3920 2020 2020 2020 207c 2020 2020 302e  9        |    0.
+00007130: 3632 3720 2020 2020 7c20 2030 2e32 3635  627     |  0.265
+00007140: 2020 207c 0a7c 2020 2020 2020 2020 2060     |.|         `
+00007150: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
+00007160: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
+00007170: 7473 385f 6469 6e6f 2229 6020 2020 2020  ts8_dino")`     
+00007180: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
+00007190: 2e36 3531 2020 2020 2020 2020 2020 207c  .651           |
+000071a0: 2020 2020 2020 2030 2e35 3234 2020 2020         0.524    
+000071b0: 2020 2020 7c20 2020 2030 2e36 3631 2020      |    0.661  
+000071c0: 2020 207c 2020 302e 3331 3520 2020 7c0a     |  0.315   |.
+000071d0: 7c20 2020 2020 2020 2060 5669 5445 7874  |        `ViTExt
+000071e0: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+000071f0: 7261 696e 6564 2822 7669 7462 3136 5f64  rained("vitb16_d
+00007200: 696e 6f22 2960 2020 2020 2020 2020 207c  ino")`         |
+00007210: 2020 2020 2020 2020 2020 302e 3635 3820            0.658 
+00007220: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00007230: 2020 302e 3531 3420 2020 2020 2020 207c    0.514        |
+00007240: 2020 2020 302e 3534 3120 2020 2020 7c20      0.541     | 
+00007250: 2030 2e32 3838 2020 207c 0a7c 2020 2020   0.288   |.|    
+00007260: 2020 2020 2060 5669 5445 7874 7261 6374       `ViTExtract
+00007270: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00007280: 6564 2822 7669 7462 385f 6469 6e6f 2229  ed("vitb8_dino")
+00007290: 6020 2020 2020 2020 2020 7c20 2020 2020  `         |     
+000072a0: 2020 2020 2030 2e36 3839 2020 2020 2020       0.689      
+000072b0: 2020 2020 207c 2020 2020 2020 2030 2e35       |       0.5
+000072c0: 3939 2020 2020 2020 2020 7c20 2020 2030  99        |    0
+000072d0: 2e35 3036 2020 2020 207c 2020 302e 3331  .506     |  0.31
+000072e0: 3320 2020 7c0a 7c20 2020 2060 5265 736e  3   |.|    `Resn
+000072f0: 6574 4578 7472 6163 746f 722e 6672 6f6d  etExtractor.from
+00007300: 5f70 7265 7472 6169 6e65 6428 2272 6573  _pretrained("res
+00007310: 6e65 7435 305f 6d6f 636f 5f76 3222 2960  net50_moco_v2")`
+00007320: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00007330: 302e 3439 3320 2020 2020 2020 2020 2020  0.493           
+00007340: 7c20 2020 2020 2020 302e 3236 3720 2020  |       0.267   
+00007350: 2020 2020 207c 2020 2020 302e 3236 3420       |    0.264 
+00007360: 2020 2020 7c20 2030 2e31 3439 2020 207c      |  0.149   |
+00007370: 0a7c 2060 5265 736e 6574 4578 7472 6163  .| `ResnetExtrac
+00007380: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
+00007390: 6e65 6428 2272 6573 6e65 7435 305f 696d  ned("resnet50_im
+000073a0: 6167 656e 6574 316b 5f76 3122 2960 2020  agenet1k_v1")`  
+000073b0: 7c20 2020 2020 2020 2020 2030 2e35 3135  |          0.515
+000073c0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000073d0: 2020 2030 2e32 3834 2020 2020 2020 2020     0.284        
+000073e0: 7c20 2020 2030 2e34 3535 2020 2020 207c  |    0.455     |
+000073f0: 2020 302e 3234 3720 2020 7c0a 0a2a 2a54    0.247   |..**T
+00007400: 6865 206d 6574 7269 6373 206d 6179 2062  he metrics may b
+00007410: 6520 6469 6666 6572 656e 7420 6672 6f6d  e different from
+00007420: 2074 6865 206f 6e65 7320 7265 706f 7274   the ones report
+00007430: 6564 2062 7920 7061 7065 7273 2c0a 6265  ed by papers,.be
+00007440: 6361 7573 6520 7468 6520 7665 7273 696f  cause the versio
+00007450: 6e20 6f66 2074 7261 696e 2f76 616c 2073  n of train/val s
+00007460: 706c 6974 2061 6e64 2075 7361 6765 206f  plit and usage o
+00007470: 6620 626f 756e 6469 6e67 2062 6f78 6573  f bounding boxes
+00007480: 206d 6179 2064 6966 6665 722e 0a50 6172   may differ..Par
+00007490: 7469 6375 6c61 726c 792c 2077 6520 7573  ticularly, we us
+000074a0: 6564 2062 6f75 6e64 696e 6720 626f 7865  ed bounding boxe
+000074b0: 7320 6475 7269 6e67 2074 6865 2065 7661  s during the eva
+000074c0: 6c75 6174 696f 6e2e 2a0a 0a23 2323 2048  luation.*..### H
+000074d0: 6f77 2074 6f20 7573 6520 6d6f 6465 6c73  ow to use models
+000074e0: 2066 726f 6d20 5a6f 6f3f 0a0a 5b63 6f6d   from Zoo?..[com
+000074f0: 6d65 6e74 5d3a 7a6f 6f2d 7374 6172 740a  ment]:zoo-start.
+00007500: 6060 6070 7974 686f 6e0a 6672 6f6d 206f  ```python.from o
+00007510: 6d6c 2e63 6f6e 7374 2069 6d70 6f72 7420  ml.const import 
+00007520: 434b 5054 5f53 4156 455f 524f 4f54 2061  CKPT_SAVE_ROOT a
+00007530: 7320 434b 5054 5f44 4952 2c20 4d4f 434b  s CKPT_DIR, MOCK
+00007540: 5f44 4154 4153 4554 5f50 4154 4820 6173  _DATASET_PATH as
+00007550: 2044 4154 415f 4449 520a 6672 6f6d 206f   DATA_DIR.from o
+00007560: 6d6c 2e6d 6f64 656c 7320 696d 706f 7274  ml.models import
+00007570: 2056 6954 4578 7472 6163 746f 720a 6672   ViTExtractor.fr
+00007580: 6f6d 206f 6d6c 2e72 6567 6973 7472 792e  om oml.registry.
+00007590: 7472 616e 7366 6f72 6d73 2069 6d70 6f72  transforms impor
+000075a0: 7420 6765 745f 7472 616e 7366 6f72 6d73  t get_transforms
+000075b0: 5f66 6f72 5f70 7265 7472 6169 6e65 640a  _for_pretrained.
+000075c0: 0a6d 6f64 656c 203d 2056 6954 4578 7472  .model = ViTExtr
+000075d0: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
+000075e0: 6169 6e65 6428 2276 6974 7331 365f 6469  ained("vits16_di
+000075f0: 6e6f 2229 0a74 7261 6e73 666f 726d 732c  no").transforms,
+00007600: 2069 6d5f 7265 6164 6572 203d 2067 6574   im_reader = get
+00007610: 5f74 7261 6e73 666f 726d 735f 666f 725f  _transforms_for_
+00007620: 7072 6574 7261 696e 6564 2822 7669 7473  pretrained("vits
+00007630: 3136 5f64 696e 6f22 290a 0a69 6d67 203d  16_dino")..img =
+00007640: 2069 6d5f 7265 6164 6572 2844 4154 415f   im_reader(DATA_
+00007650: 4449 5220 2f20 2269 6d61 6765 7322 202f  DIR / "images" /
+00007660: 2022 6369 7263 6c65 5f31 2e6a 7067 2229   "circle_1.jpg")
+00007670: 2020 2320 7075 7420 7061 7468 2074 6f20    # put path to 
+00007680: 796f 7572 2069 6d61 6765 2068 6572 650a  your image here.
+00007690: 696d 675f 7465 6e73 6f72 203d 2074 7261  img_tensor = tra
+000076a0: 6e73 666f 726d 7328 696d 6729 0a23 2069  nsforms(img).# i
+000076b0: 6d67 5f74 656e 736f 7220 3d20 7472 616e  mg_tensor = tran
+000076c0: 7366 6f72 6d73 2869 6d61 6765 3d69 6d67  sforms(image=img
+000076d0: 295b 2269 6d61 6765 225d 2020 2320 666f  )["image"]  # fo
+000076e0: 7220 7472 616e 7366 6f72 6d73 2066 726f  r transforms fro
+000076f0: 6d20 416c 6275 6d65 6e74 6174 696f 6e73  m Albumentations
+00007700: 0a0a 6665 6174 7572 6573 203d 206d 6f64  ..features = mod
+00007710: 656c 2869 6d67 5f74 656e 736f 722e 756e  el(img_tensor.un
+00007720: 7371 7565 657a 6528 3029 290a 0a23 2043  squeeze(0))..# C
+00007730: 6865 636b 206f 7468 6572 2061 7661 696c  heck other avail
+00007740: 6162 6c65 206d 6f64 656c 733a 0a70 7269  able models:.pri
+00007750: 6e74 286c 6973 7428 5669 5445 7874 7261  nt(list(ViTExtra
+00007760: 6374 6f72 2e70 7265 7472 6169 6e65 645f  ctor.pretrained_
+00007770: 6d6f 6465 6c73 2e6b 6579 7328 2929 290a  models.keys())).
+00007780: 0a23 204c 6f61 6420 6368 6563 6b70 6f69  .# Load checkpoi
+00007790: 6e74 2073 6176 6564 206f 6e20 6120 6469  nt saved on a di
+000077a0: 736b 3a0a 6d6f 6465 6c5f 203d 2056 6954  sk:.model_ = ViT
+000077b0: 4578 7472 6163 746f 7228 7765 6967 6874  Extractor(weight
+000077c0: 733d 434b 5054 5f44 4952 202f 2022 7669  s=CKPT_DIR / "vi
+000077d0: 7473 3136 5f64 696e 6f2e 636b 7074 222c  ts16_dino.ckpt",
+000077e0: 2061 7263 683d 2276 6974 7331 3622 2c20   arch="vits16", 
+000077f0: 6e6f 726d 616c 6973 655f 6665 6174 7572  normalise_featur
+00007800: 6573 3d46 616c 7365 290a 6060 600a 5b63  es=False).```.[c
+00007810: 6f6d 6d65 6e74 5d3a 7a6f 6f2d 656e 640a  omment]:zoo-end.
+00007820: 0a23 2320 5b43 6f6e 7472 6962 7574 696e  .## [Contributin
+00007830: 6720 6775 6964 655d 2868 7474 7073 3a2f  g guide](https:/
+00007840: 2f6f 7065 6e2d 6d65 7472 6963 2d6c 6561  /open-metric-lea
+00007850: 726e 696e 672e 7265 6164 7468 6564 6f63  rning.readthedoc
+00007860: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6f  s.io/en/latest/o
+00007870: 6d6c 2f63 6f6e 7472 6962 7574 696e 672e  ml/contributing.
+00007880: 6874 6d6c 290a 0a57 6520 7765 6c63 6f6d  html)..We welcom
+00007890: 6520 6e65 7720 636f 6e74 7269 6275 746f  e new contributo
+000078a0: 7273 2120 506c 6561 7365 2c20 7365 6520  rs! Please, see 
+000078b0: 6f75 723a 0a2a 205b 436f 6e74 7269 6275  our:.* [Contribu
+000078c0: 7469 6e67 2067 7569 6465 5d28 6874 7470  ting guide](http
+000078d0: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+000078e0: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+000078f0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00007900: 742f 6f6d 6c2f 636f 6e74 7269 6275 7469  t/oml/contributi
+00007910: 6e67 2e68 746d 6c29 0a2a 205b 4b61 6e62  ng.html).* [Kanb
+00007920: 616e 2062 6f61 7264 5d28 6874 7470 733a  an board](https:
+00007930: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00007940: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00007950: 632d 6c65 6172 6e69 6e67 2f70 726f 6a65  c-learning/proje
+00007960: 6374 732f 3129 0a0a 2323 2041 636b 6e6f  cts/1)..## Ackno
+00007970: 776c 6564 676d 656e 7473 0a0a 3c61 2068  wledgments..<a h
+00007980: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00007990: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+000079a0: 2d74 6561 6d2f 6361 7461 6c79 7374 2220  -team/catalyst" 
+000079b0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000079c0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000079d0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+000079e0: 636f 6e74 656e 742e 636f 6d2f 6361 7461  content.com/cata
+000079f0: 6c79 7374 2d74 6561 6d2f 6361 7461 6c79  lyst-team/cataly
+00007a00: 7374 2d70 6963 732f 6d61 7374 6572 2f70  st-pics/master/p
+00007a10: 6963 732f 6361 7461 6c79 7374 5f6c 6f67  ics/catalyst_log
+00007a20: 6f2e 706e 6722 2077 6964 7468 3d22 3130  o.png" width="10
+00007a30: 3022 2f3e 3c2f 613e 0a0a 5468 6520 7072  0"/></a>..The pr
+00007a40: 6f6a 6563 7420 7761 7320 7374 6172 7465  oject was starte
+00007a50: 6420 696e 2032 3032 3020 6173 2061 206d  d in 2020 as a m
+00007a60: 6f64 756c 6520 666f 7220 5b43 6174 616c  odule for [Catal
+00007a70: 7973 745d 2868 7474 7073 3a2f 2f67 6974  yst](https://git
+00007a80: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+00007a90: 2d74 6561 6d2f 6361 7461 6c79 7374 2920  -team/catalyst) 
+00007aa0: 6c69 6272 6172 792e 0a49 2077 616e 7420  library..I want 
+00007ab0: 746f 2074 6861 6e6b 2070 656f 706c 6520  to thank people 
+00007ac0: 7768 6f20 776f 726b 6564 2077 6974 6820  who worked with 
+00007ad0: 6d65 206f 6e20 7468 6174 206d 6f64 756c  me on that modul
+00007ae0: 653a 0a5b 4a75 6c69 6120 5368 656e 7368  e:.[Julia Shensh
+00007af0: 696e 615d 2868 7474 7073 3a2f 2f67 6974  ina](https://git
+00007b00: 6875 622e 636f 6d2f 6a75 6c69 612d 7368  hub.com/julia-sh
+00007b10: 656e 7368 696e 6129 2c0a 5b4e 696b 6974  enshina),.[Nikit
+00007b20: 6120 4261 6c61 6761 6e73 6b79 5d28 6874  a Balagansky](ht
+00007b30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00007b40: 2f65 6c65 7068 616e 746d 6970 7429 2c0a  /elephantmipt),.
+00007b50: 5b53 6572 6765 7920 4b6f 6c65 736e 696b  [Sergey Kolesnik
+00007b60: 6f76 5d28 6874 7470 733a 2f2f 6769 7468  ov](https://gith
+00007b70: 7562 2e63 6f6d 2f53 6369 7461 746f 7229  ub.com/Scitator)
+00007b80: 0a61 6e64 206f 7468 6572 732e 0a0a 4920  .and others...I 
+00007b90: 776f 756c 6420 6c69 6b65 2074 6f20 7468  would like to th
+00007ba0: 616e 6b20 7065 6f70 6c65 2077 686f 2063  ank people who c
+00007bb0: 6f6e 7469 6e75 6520 776f 726b 696e 6720  ontinue working 
+00007bc0: 6f6e 2074 6869 7320 7069 7065 6c69 6e65  on this pipeline
+00007bd0: 2077 6865 6e20 6974 2062 6563 616d 6520   when it became 
+00007be0: 6120 7365 7061 7265 2070 726f 6a65 6374  a separe project
+00007bf0: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
+00007c00: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
+00007c10: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
+00007c20: 6e73 6869 6e61 292c 0a5b 4d69 7368 6120  nshina),.[Misha 
+00007c30: 4b69 6e64 756c 6f76 5d28 6874 7470 733a  Kindulov](https:
+00007c40: 2f2f 6769 7468 7562 2e63 6f6d 2f62 306e  //github.com/b0n
+00007c50: 6365 292c 0a5b 416c 656b 7365 6920 5461  ce),.[Aleksei Ta
+00007c60: 7261 736f 765d 2868 7474 7073 3a2f 2f67  rasov](https://g
+00007c70: 6974 6875 622e 636f 6d2f 4461 6c6f 726f  ithub.com/Daloro
+00007c80: 4154 2920 616e 640a 5b56 6572 6b68 6f76  AT) and.[Verkhov
+00007c90: 7473 6576 204c 656f 6e69 645d 2868 7474  tsev Leonid](htt
+00007ca0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00007cb0: 6c65 6f72 6f6d 616e 6f76 6963 6829 2e0a  leoromanovich)..
+00007cc0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00007cd0: 2f2f 7777 772e 6e65 7779 6f72 6b65 722e  //www.newyorker.
+00007ce0: 6465 2f22 2074 6172 6765 743d 225f 626c  de/" target="_bl
+00007cf0: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
+00007d00: 7474 7073 3a2f 2f75 706c 6f61 642e 7769  ttps://upload.wi
+00007d10: 6b69 6d65 6469 612e 6f72 672f 7769 6b69  kimedia.org/wiki
+00007d20: 7065 6469 612f 636f 6d6d 6f6e 732f 7468  pedia/commons/th
+00007d30: 756d 622f 642f 6438 2f4e 6577 5f59 6f72  umb/d/d8/New_Yor
+00007d40: 6b65 722e 7376 672f 3132 3830 7078 2d4e  ker.svg/1280px-N
+00007d50: 6577 5f59 6f72 6b65 722e 7376 672e 706e  ew_Yorker.svg.pn
+00007d60: 6722 2077 6964 7468 3d22 3130 3022 2f3e  g" width="100"/>
+00007d70: 3c2f 613e 0a0a 4920 616c 736f 2077 616e  </a>..I also wan
+00007d80: 7420 746f 2074 6861 6e6b 204e 6577 596f  t to thank NewYo
+00007d90: 726b 6572 2c20 7369 6e63 6520 7468 6520  rker, since the 
+00007da0: 7061 7274 206f 6620 6675 6e63 7469 6f6e  part of function
+00007db0: 616c 6974 7920 7761 7320 6465 7665 6c6f  ality was develo
+00007dc0: 7065 6420 2861 6e64 2075 7365 6429 2062  ped (and used) b
+00007dd0: 7920 6974 7320 636f 6d70 7574 6572 2076  y its computer v
+00007de0: 6973 696f 6e20 7465 616d 206c 6564 2062  ision team led b
+00007df0: 7920 6d65 2e0a                           y me..
```

### Comparing `open-metric-learning-0.4.3/README.md` & `open-metric-learning-0.4.4/open_metric_learning.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,1826 +1,2016 @@
-00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-00000010: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
-00000020: 7474 7073 3a2f 2f69 2e69 6262 2e63 6f2f  ttps://i.ibb.co/
-00000030: 7773 6d44 3572 342f 7068 6f74 6f2d 3230  wsmD5r4/photo-20
-00000040: 3232 2d30 362d 3036 2d31 372d 3430 2d35  22-06-06-17-40-5
-00000050: 322e 6a70 6722 2077 6964 7468 3d22 3430  2.jpg" width="40
-00000060: 3070 7822 3e0a 0a21 5b65 7861 6d70 6c65  0px">..![example
-00000070: 2077 6f72 6b66 6c6f 775d 2868 7474 7073   workflow](https
-00000080: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
-00000090: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
-000000a0: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
-000000b0: 6f6e 732f 776f 726b 666c 6f77 732f 7072  ons/workflows/pr
-000000c0: 652d 636f 6d6d 6974 2d77 6f72 6b66 6c6f  e-commit-workflo
-000000d0: 772e 7961 6d6c 2f62 6164 6765 2e73 7667  w.yaml/badge.svg
-000000e0: 290a 215b 6578 616d 706c 6520 776f 726b  ).![example work
-000000f0: 666c 6f77 5d28 6874 7470 733a 2f2f 6769  flow](https://gi
-00000100: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
-00000110: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
-00000120: 6172 6e69 6e67 2f61 6374 696f 6e73 2f77  arning/actions/w
-00000130: 6f72 6b66 6c6f 7773 2f74 6573 7473 2d77  orkflows/tests-w
-00000140: 6f72 6b66 6c6f 772e 7961 6d6c 2f62 6164  orkflow.yaml/bad
-00000150: 6765 2e73 7667 3f29 0a5b 215b 446f 6375  ge.svg?).[![Docu
-00000160: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
-00000170: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
-00000180: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000190: 7473 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ts/open-metric-l
-000001a0: 6561 726e 696e 672f 6261 6467 652f 3f76  earning/badge/?v
-000001b0: 6572 7369 6f6e 3d6c 6174 6573 7429 5d28  ersion=latest)](
-000001c0: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
-000001d0: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
-000001e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-000001f0: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
-00000200: 6573 7429 0a5b 215b 5079 5049 2053 7461  est).[![PyPI Sta
-00000210: 7475 735d 2868 7474 7073 3a2f 2f70 6570  tus](https://pep
-00000220: 792e 7465 6368 2f62 6164 6765 2f6f 7065  y.tech/badge/ope
-00000230: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-00000240: 6729 5d28 6874 7470 733a 2f2f 7065 7079  g)](https://pepy
-00000250: 2e74 6563 682f 7072 6f6a 6563 742f 6f70  .tech/project/op
-00000260: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00000270: 6e67 290a 5b21 5b50 6970 6920 7665 7273  ng).[![Pipi vers
-00000280: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000290: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000002a0: 2f76 2f6f 7065 6e2d 6d65 7472 6963 2d6c  /v/open-metric-l
-000002b0: 6561 726e 696e 672e 7376 6729 5d28 6874  earning.svg)](ht
-000002c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000002d0: 726f 6a65 6374 2f6f 7065 6e2d 6d65 7472  roject/open-metr
-000002e0: 6963 2d6c 6561 726e 696e 672f 290a 215b  ic-learning/).![
-000002f0: 6578 616d 706c 6520 776f 726b 666c 6f77  example workflow
-00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000310: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00000320: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00000330: 6e67 2f61 6374 696f 6e73 2f77 6f72 6b66  ng/actions/workf
-00000340: 6c6f 7773 2f70 7974 686f 6e2d 7665 7273  lows/python-vers
-00000350: 696f 6e73 2e79 616d 6c2f 6261 6467 652e  ions.yaml/badge.
-00000360: 7376 673f 290a 5b21 5b70 7974 686f 6e5d  svg?).[![python]
-00000370: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000380: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-00000390: 7468 6f6e 5f33 2e37 2d70 6173 7369 6e67  thon_3.7-passing
-000003a0: 2d73 7563 6365 7373 295d 2868 7474 7073  -success)](https
-000003b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
-000003c0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
-000003d0: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
-000003e0: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
-000003f0: 7468 6f6e 2d76 6572 7369 6f6e 732e 7961  thon-versions.ya
-00000400: 6d6c 2f62 6164 6765 2e73 7667 3f29 0a5b  ml/badge.svg?).[
-00000410: 215b 7079 7468 6f6e 5d28 6874 7470 733a  ![python](https:
-00000420: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000430: 2f62 6164 6765 2f70 7974 686f 6e5f 332e  /badge/python_3.
-00000440: 382d 7061 7373 696e 672d 7375 6363 6573  8-passing-succes
-00000450: 7329 5d28 6874 7470 733a 2f2f 6769 7468  s)](https://gith
-00000460: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00000470: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00000480: 6e69 6e67 2f61 6374 696f 6e73 2f77 6f72  ning/actions/wor
-00000490: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7665  kflows/python-ve
-000004a0: 7273 696f 6e73 2e79 616d 6c2f 6261 6467  rsions.yaml/badg
-000004b0: 652e 7376 673f 290a 5b21 5b70 7974 686f  e.svg?).[![pytho
-000004c0: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-000004d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000004e0: 7079 7468 6f6e 5f33 2e39 2d70 6173 7369  python_3.9-passi
-000004f0: 6e67 2d73 7563 6365 7373 295d 2868 7474  ng-success)](htt
-00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000510: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
-00000520: 7472 6963 2d6c 6561 726e 696e 672f 6163  tric-learning/ac
-00000530: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000540: 7079 7468 6f6e 2d76 6572 7369 6f6e 732e  python-versions.
-00000550: 7961 6d6c 2f62 6164 6765 2e73 7667 3f29  yaml/badge.svg?)
-00000560: 0a5b 215b 7079 7468 6f6e 5d28 6874 7470  .[![python](http
-00000570: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000580: 696f 2f62 6164 6765 2f70 7974 686f 6e5f  io/badge/python_
-00000590: 332e 3130 2d70 6173 7369 6e67 2d73 7563  3.10-passing-suc
-000005a0: 6365 7373 295d 2868 7474 7073 3a2f 2f67  cess)](https://g
-000005b0: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-000005c0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-000005d0: 6561 726e 696e 672f 6163 7469 6f6e 732f  earning/actions/
-000005e0: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
-000005f0: 2d76 6572 7369 6f6e 732e 7961 6d6c 2f62  -versions.yaml/b
-00000600: 6164 6765 2e73 7667 3f29 0a0a 3c64 6976  adge.svg?)..<div
-00000610: 2061 6c69 676e 3d22 6c65 6674 223e 0a0a   align="left">..
-00000620: 4f4d 4c20 6973 2061 2050 7954 6f72 6368  OML is a PyTorch
-00000630: 2d62 6173 6564 2066 7261 6d65 776f 726b  -based framework
-00000640: 2074 6f20 7472 6169 6e20 616e 6420 7661   to train and va
-00000650: 6c69 6461 7465 2074 6865 206d 6f64 656c  lidate the model
-00000660: 7320 7072 6f64 7563 696e 6720 6869 6768  s producing high
-00000670: 2d71 7561 6c69 7479 2065 6d62 6564 6469  -quality embeddi
-00000680: 6e67 732e 0a0a 2323 205b 4641 515d 2868  ngs...## [FAQ](h
-00000690: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
-000006a0: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
-000006b0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000006c0: 7465 7374 2f6f 6d6c 2f66 6171 2e68 746d  test/oml/faq.htm
-000006d0: 6c29 0a0a 3c64 6574 6169 6c73 3e0a 3c73  l)..<details>.<s
-000006e0: 756d 6d61 7279 3e57 6879 2064 6f20 4920  ummary>Why do I 
-000006f0: 6e65 6564 204f 4d4c 3f3c 2f73 756d 6d61  need OML?</summa
-00000700: 7279 3e0a 3c70 3e0a 0a59 6f75 206d 6179  ry>.<p>..You may
-00000710: 2074 6869 6e6b 202a 2249 6620 4920 6e65   think *"If I ne
-00000720: 6564 2069 6d61 6765 2065 6d62 6564 6469  ed image embeddi
-00000730: 6e67 7320 4920 6361 6e20 7369 6d70 6c79  ngs I can simply
-00000740: 2074 7261 696e 2061 2076 616e 696c 6c61   train a vanilla
-00000750: 2063 6c61 7373 6966 6965 7220 616e 6420   classifier and 
-00000760: 7461 6b65 2069 7473 2070 656e 756c 7469  take its penulti
-00000770: 6d61 7465 206c 6179 6572 222a 2e0a 5765  mate layer"*..We
-00000780: 6c6c 2c20 6974 206d 616b 6573 2073 656e  ll, it makes sen
-00000790: 7365 2061 7320 6120 7374 6172 7469 6e67  se as a starting
-000007a0: 2070 6f69 6e74 2e20 4275 7420 7468 6572   point. But ther
-000007b0: 6520 6172 6520 7365 7665 7261 6c20 706f  e are several po
-000007c0: 7373 6962 6c65 2064 7261 7762 6163 6b73  ssible drawbacks
-000007d0: 3a0a 0a2a 2049 6620 796f 7520 7761 6e74  :..* If you want
-000007e0: 2074 6f20 7573 6520 656d 6265 6464 696e   to use embeddin
-000007f0: 6773 2074 6f20 7065 7266 6f72 6d20 7365  gs to perform se
-00000800: 6172 6368 696e 6720 796f 7520 6e65 6564  arching you need
-00000810: 2074 6f20 6361 6c63 756c 6174 6520 736f   to calculate so
-00000820: 6d65 2064 6973 7461 6e63 6520 616d 6f6e  me distance amon
-00000830: 6720 7468 656d 2028 666f 7220 6578 616d  g them (for exam
-00000840: 706c 652c 2063 6f73 696e 6520 6f72 204c  ple, cosine or L
-00000850: 3229 2e0a 2020 5573 7561 6c6c 792c 202a  2)..  Usually, *
-00000860: 2a79 6f75 2064 6f6e 2774 2064 6972 6563  *you don't direc
-00000870: 746c 7920 6f70 7469 6d69 7a65 2074 6865  tly optimize the
-00000880: 7365 2064 6973 7461 6e63 6573 2064 7572  se distances dur
-00000890: 696e 6720 7468 6520 7472 6169 6e69 6e67  ing the training
-000008a0: 2a2a 2069 6e20 7468 6520 636c 6173 7369  ** in the classi
-000008b0: 6669 6361 7469 6f6e 2073 6574 7570 2e20  fication setup. 
-000008c0: 536f 2c20 796f 7520 6361 6e20 6f6e 6c79  So, you can only
-000008d0: 2068 6f70 6520 7468 6174 0a20 2066 696e   hope that.  fin
-000008e0: 616c 2065 6d62 6564 6469 6e67 7320 7769  al embeddings wi
-000008f0: 6c6c 2068 6176 6520 7468 6520 6465 7369  ll have the desi
-00000900: 7265 6420 7072 6f70 6572 7469 6573 2e0a  red properties..
-00000910: 0a2a 202a 2a54 6865 2073 6563 6f6e 6420  .* **The second 
-00000920: 7072 6f62 6c65 6d20 6973 2074 6865 2076  problem is the v
-00000930: 616c 6964 6174 696f 6e20 7072 6f63 6573  alidation proces
-00000940: 732a 2a2e 0a20 2049 6e20 7468 6520 7365  s**..  In the se
-00000950: 6172 6368 696e 6720 7365 7475 702c 2079  arching setup, y
-00000960: 6f75 2075 7375 616c 6c79 2063 6172 6520  ou usually care 
-00000970: 686f 7720 7265 6c61 7465 6420 796f 7572  how related your
-00000980: 2074 6f70 2d4e 206f 7574 7075 7473 2061   top-N outputs a
-00000990: 7265 2074 6f20 7468 6520 7175 6572 792e  re to the query.
-000009a0: 0a20 2054 6865 206e 6174 7572 616c 2077  .  The natural w
-000009b0: 6179 2074 6f20 6576 616c 7561 7465 2074  ay to evaluate t
-000009c0: 6865 206d 6f64 656c 2069 7320 746f 2073  he model is to s
-000009d0: 696d 756c 6174 6520 7365 6172 6368 696e  imulate searchin
-000009e0: 6720 7265 7175 6573 7473 2074 6f20 7468  g requests to th
-000009f0: 6520 7265 6665 7265 6e63 6520 7365 740a  e reference set.
-00000a00: 2020 616e 6420 6170 706c 7920 6f6e 6520    and apply one 
-00000a10: 6f66 2074 6865 2072 6574 7269 6576 616c  of the retrieval
-00000a20: 206d 6574 7269 6373 2e0a 2020 536f 2c20   metrics..  So, 
-00000a30: 7468 6572 6520 6973 206e 6f20 6775 6172  there is no guar
-00000a40: 616e 7465 6520 7468 6174 2063 6c61 7373  antee that class
-00000a50: 6966 6963 6174 696f 6e20 6163 6375 7261  ification accura
-00000a60: 6379 2077 696c 6c20 636f 7272 656c 6174  cy will correlat
-00000a70: 6520 7769 7468 2074 6865 7365 206d 6574  e with these met
-00000a80: 7269 6373 2e0a 0a2a 2046 696e 616c 6c79  rics...* Finally
-00000a90: 2c20 796f 7520 6d61 7920 7761 6e74 2074  , you may want t
-00000aa0: 6f20 696d 706c 656d 656e 7420 6120 6d65  o implement a me
-00000ab0: 7472 6963 206c 6561 726e 696e 6720 7069  tric learning pi
-00000ac0: 7065 6c69 6e65 2062 7920 796f 7572 7365  peline by yourse
-00000ad0: 6c66 2e0a 2020 2a2a 5468 6572 6520 6973  lf..  **There is
-00000ae0: 2061 206c 6f74 206f 6620 776f 726b 2a2a   a lot of work**
-00000af0: 3a20 746f 2075 7365 2074 7269 706c 6574  : to use triplet
-00000b00: 206c 6f73 7320 796f 7520 6e65 6564 2074   loss you need t
-00000b10: 6f20 666f 726d 2062 6174 6368 6573 2069  o form batches i
-00000b20: 6e20 6120 7370 6563 6966 6963 2077 6179  n a specific way
-00000b30: 2c0a 2020 696d 706c 656d 656e 7420 6469  ,.  implement di
-00000b40: 6666 6572 656e 7420 6b69 6e64 7320 6f66  fferent kinds of
-00000b50: 2074 7269 706c 6574 7320 6d69 6e69 6e67   triplets mining
-00000b60: 2c20 7472 6163 6b69 6e67 2064 6973 7461  , tracking dista
-00000b70: 6e63 6573 2c20 6574 632e 2046 6f72 2074  nces, etc. For t
-00000b80: 6865 2076 616c 6964 6174 696f 6e2c 2079  he validation, y
-00000b90: 6f75 2061 6c73 6f20 6e65 6564 2074 6f0a  ou also need to.
-00000ba0: 2020 696d 706c 656d 656e 7420 7265 7472    implement retr
-00000bb0: 6965 7661 6c20 6d65 7472 6963 732c 0a20  ieval metrics,. 
-00000bc0: 2077 6869 6368 2069 6e63 6c75 6465 2065   which include e
-00000bd0: 6666 6563 7469 7665 2065 6d62 6564 6469  ffective embeddi
-00000be0: 6e67 7320 6163 6375 6d75 6c61 7469 6f6e  ngs accumulation
-00000bf0: 2064 7572 696e 6720 7468 6520 6570 6f63   during the epoc
-00000c00: 682c 2063 6f76 6572 696e 6720 636f 726e  h, covering corn
-00000c10: 6572 2063 6173 6573 2c20 6574 632e 0a20  er cases, etc.. 
-00000c20: 2049 7427 7320 6576 656e 2068 6172 6465   It's even harde
-00000c30: 7220 6966 2079 6f75 2068 6176 6520 7365  r if you have se
-00000c40: 7665 7261 6c20 6770 7573 2061 6e64 2075  veral gpus and u
-00000c50: 7365 2044 4450 2e0a 2020 596f 7520 6d61  se DDP..  You ma
-00000c60: 7920 616c 736f 2077 616e 7420 746f 2076  y also want to v
-00000c70: 6973 7561 6c69 7a65 2079 6f75 7220 7365  isualize your se
-00000c80: 6172 6368 2072 6571 7565 7374 7320 6279  arch requests by
-00000c90: 2068 6967 686c 6967 6874 696e 6720 676f   highlighting go
-00000ca0: 6f64 2061 6e64 2062 6164 2073 6561 7263  od and bad searc
-00000cb0: 6820 7265 7375 6c74 732e 0a20 2049 6e73  h results..  Ins
-00000cc0: 7465 6164 206f 6620 646f 696e 6720 6974  tead of doing it
-00000cd0: 2062 7920 796f 7572 7365 6c66 2c20 796f   by yourself, yo
-00000ce0: 7520 6361 6e20 7369 6d70 6c79 2075 7365  u can simply use
-00000cf0: 204f 4d4c 2066 6f72 2079 6f75 7220 7075   OML for your pu
-00000d00: 7270 6f73 6573 2e0a 0a3c 2f70 3e0a 3c2f  rposes...</p>.</
-00000d10: 6465 7461 696c 733e 0a0a 0a3c 6465 7461  details>...<deta
-00000d20: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-00000d30: 6174 2069 7320 7468 6520 6469 6666 6572  at is the differ
-00000d40: 656e 6365 2062 6574 7765 656e 204f 7065  ence between Ope
-00000d50: 6e20 4d65 7472 6963 204c 6561 726e 696e  n Metric Learnin
-00000d60: 6720 616e 6420 5079 546f 7263 6820 4d65  g and PyTorch Me
-00000d70: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
-00000d80: 7375 6d6d 6172 793e 0a3c 703e 0a0a 5b50  summary>.<p>..[P
-00000d90: 4d4c 5d28 6874 7470 733a 2f2f 6769 7468  ML](https://gith
-00000da0: 7562 2e63 6f6d 2f4b 6576 696e 4d75 7367  ub.com/KevinMusg
-00000db0: 7261 7665 2f70 7974 6f72 6368 2d6d 6574  rave/pytorch-met
-00000dc0: 7269 632d 6c65 6172 6e69 6e67 2920 6973  ric-learning) is
-00000dd0: 2074 6865 2070 6f70 756c 6172 206c 6962   the popular lib
-00000de0: 7261 7279 2066 6f72 204d 6574 7269 6320  rary for Metric 
-00000df0: 4c65 6172 6e69 6e67 2c0a 616e 6420 6974  Learning,.and it
-00000e00: 2069 6e63 6c75 6465 7320 6120 7269 6368   includes a rich
-00000e10: 2063 6f6c 6c65 6374 696f 6e20 6f66 206c   collection of l
-00000e20: 6f73 7365 732c 206d 696e 6572 732c 2064  osses, miners, d
-00000e30: 6973 7461 6e63 6573 2c20 616e 6420 7265  istances, and re
-00000e40: 6475 6365 7273 3b20 7468 6174 2069 7320  ducers; that is 
-00000e50: 7768 7920 7765 2070 726f 7669 6465 2073  why we provide s
-00000e60: 7472 6169 6768 7466 6f72 7761 7264 0a5b  traightforward.[
-00000e70: 6578 616d 706c 6573 5d28 6874 7470 733a  examples](https:
-00000e80: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00000e90: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00000ea0: 632d 6c65 6172 6e69 6e67 2375 7361 6765  c-learning#usage
-00000eb0: 2d77 6974 682d 7079 746f 7263 682d 6d65  -with-pytorch-me
-00000ec0: 7472 6963 2d6c 6561 726e 696e 6729 206f  tric-learning) o
-00000ed0: 6620 7573 696e 6720 7468 656d 2077 6974  f using them wit
-00000ee0: 6820 4f4d 4c2e 0a49 6e69 7469 616c 6c79  h OML..Initially
-00000ef0: 2c20 7765 2074 7269 6564 2074 6f20 7573  , we tried to us
-00000f00: 6520 504d 4c2c 2062 7574 2069 6e20 7468  e PML, but in th
-00000f10: 6520 656e 642c 2077 6520 6361 6d65 2075  e end, we came u
-00000f20: 7020 7769 7468 206f 7572 206c 6962 7261  p with our libra
-00000f30: 7279 2c20 7768 6963 6820 6973 206d 6f72  ry, which is mor
-00000f40: 6520 7069 7065 6c69 6e65 202f 2072 6563  e pipeline / rec
-00000f50: 6970 6573 206f 7269 656e 7465 642e 0a54  ipes oriented..T
-00000f60: 6861 7420 6973 2068 6f77 204f 4d4c 2064  hat is how OML d
-00000f70: 6966 6665 7273 2066 726f 6d20 504d 4c3a  iffers from PML:
-00000f80: 0a0a 2a20 4f4d 4c20 6861 7320 5b50 6970  ..* OML has [Pip
-00000f90: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00000fa0: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-00000fb0: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00000fc0: 6c65 6172 6e69 6e67 2f74 7265 652f 6d61  learning/tree/ma
-00000fd0: 696e 2f70 6970 656c 696e 6573 290a 2020  in/pipelines).  
-00000fe0: 7768 6963 6820 616c 6c6f 7773 2074 7261  which allows tra
-00000ff0: 696e 696e 6720 6d6f 6465 6c73 2062 7920  ining models by 
-00001000: 7072 6570 6172 696e 6720 6120 636f 6e66  preparing a conf
-00001010: 6967 2061 6e64 2079 6f75 7220 6461 7461  ig and your data
-00001020: 2069 6e20 7468 6520 7265 7175 6972 6564   in the required
-00001030: 2066 6f72 6d61 740a 2020 2869 7427 7320   format.  (it's 
-00001040: 6c69 6b65 2063 6f6e 7665 7274 696e 6720  like converting 
-00001050: 6461 7461 2069 6e74 6f20 434f 434f 2066  data into COCO f
-00001060: 6f72 6d61 7420 746f 2074 7261 696e 2061  ormat to train a
-00001070: 2064 6574 6563 746f 7220 6672 6f6d 205b   detector from [
-00001080: 6d6d 6465 7465 6374 696f 6e5d 2868 7474  mmdetection](htt
-00001090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000010a0: 6f70 656e 2d6d 6d6c 6162 2f6d 6d64 6574  open-mmlab/mmdet
-000010b0: 6563 7469 6f6e 2929 2e0a 0a2a 204f 4d4c  ection))...* OML
-000010c0: 2066 6f63 7573 6573 206f 6e20 656e 642d   focuses on end-
-000010d0: 746f 2d65 6e64 2070 6970 656c 696e 6573  to-end pipelines
-000010e0: 2061 6e64 2070 7261 6374 6963 616c 2075   and practical u
-000010f0: 7365 2063 6173 6573 2e0a 2020 4974 2068  se cases..  It h
-00001100: 6173 2063 6f6e 6669 6720 6261 7365 6420  as config based 
-00001110: 6578 616d 706c 6573 206f 6e20 706f 7075  examples on popu
-00001120: 6c61 7220 6265 6e63 686d 6172 6b73 2063  lar benchmarks c
-00001130: 6c6f 7365 2074 6f20 7265 616c 206c 6966  lose to real lif
-00001140: 6520 286c 696b 6520 7068 6f74 6f73 206f  e (like photos o
-00001150: 6620 7072 6f64 7563 7473 206f 6620 7468  f products of th
-00001160: 6f75 7361 6e64 7320 6964 7329 2e0a 2020  ousands ids)..  
-00001170: 5765 2066 6f75 6e64 2073 6f6d 6520 676f  We found some go
-00001180: 6f64 2063 6f6d 6269 6e61 7469 6f6e 7320  od combinations 
-00001190: 6f66 2068 7970 6572 7061 7261 6d65 7465  of hyperparamete
-000011a0: 7273 206f 6e20 7468 6573 6520 6461 7461  rs on these data
-000011b0: 7365 7473 2c20 7472 6169 6e65 6420 616e  sets, trained an
-000011c0: 6420 7075 626c 6973 6865 6420 6d6f 6465  d published mode
-000011d0: 6c73 2061 6e64 2074 6865 6972 2063 6f6e  ls and their con
-000011e0: 6669 6773 2e0a 2020 5468 7573 2c20 6974  figs..  Thus, it
-000011f0: 206d 616b 6573 204f 4d4c 206d 6f72 6520   makes OML more 
-00001200: 7265 6369 7065 7320 6f72 6965 6e74 6564  recipes oriented
-00001210: 2074 6861 6e20 504d 4c2c 2061 6e64 2069   than PML, and i
-00001220: 7473 2061 7574 686f 720a 2020 5b63 6f6e  ts author.  [con
-00001230: 6669 726d 735d 2868 7474 7073 3a2f 2f67  firms](https://g
-00001240: 6974 6875 622e 636f 6d2f 4b65 7669 6e4d  ithub.com/KevinM
-00001250: 7573 6772 6176 652f 7079 746f 7263 682d  usgrave/pytorch-
-00001260: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
-00001270: 6973 7375 6573 2f31 3639 2369 7373 7565  issues/169#issue
-00001280: 636f 6d6d 656e 742d 3637 3038 3134 3339  comment-67081439
-00001290: 3329 0a20 2074 6869 7320 7361 7969 6e67  3).  this saying
-000012a0: 2074 6861 7420 6869 7320 6c69 6272 6172   that his librar
-000012b0: 7920 6973 2061 2073 6574 206f 6620 746f  y is a set of to
-000012c0: 6f6c 7320 7261 7468 6572 2074 6865 2072  ols rather the r
-000012d0: 6563 6970 6573 2c20 6d6f 7265 6f76 6572  ecipes, moreover
-000012e0: 2c20 7468 6520 6578 616d 706c 6573 2069  , the examples i
-000012f0: 6e20 504d 4c20 6172 6520 6d6f 7374 6c79  n PML are mostly
-00001300: 2066 6f72 2043 4946 4152 2061 6e64 204d   for CIFAR and M
-00001310: 4e49 5354 2064 6174 6173 6574 732e 0a0a  NIST datasets...
-00001320: 2a20 4f4d 4c20 6861 7320 7468 6520 5b5a  * OML has the [Z
-00001330: 6f6f 5d28 6874 7470 733a 2f2f 6769 7468  oo](https://gith
-00001340: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00001350: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00001360: 6e69 6e67 237a 6f6f 2920 6f66 2070 7265  ning#zoo) of pre
-00001370: 7472 6169 6e65 6420 6d6f 6465 6c73 2074  trained models t
-00001380: 6861 7420 6361 6e20 6265 2065 6173 696c  hat can be easil
-00001390: 7920 6163 6365 7373 6564 2066 726f 6d0a  y accessed from.
-000013a0: 2020 7468 6520 636f 6465 2069 6e20 7468    the code in th
-000013b0: 6520 7361 6d65 2077 6179 2061 7320 696e  e same way as in
-000013c0: 2060 746f 7263 6876 6973 696f 6e60 2028   `torchvision` (
-000013d0: 7768 656e 2079 6f75 2074 7970 6520 6072  when you type `r
-000013e0: 6573 6e65 7435 3028 7072 6574 7261 696e  esnet50(pretrain
-000013f0: 6564 3d54 7275 6529 6029 2e0a 0a2a 204f  ed=True)`)...* O
-00001400: 4d4c 2069 7320 696e 7465 6772 6174 6564  ML is integrated
-00001410: 2077 6974 6820 5b50 7954 6f72 6368 204c   with [PyTorch L
-00001420: 6967 6874 6e69 6e67 5d28 6874 7470 733a  ightning](https:
-00001430: 2f2f 7777 772e 7079 746f 7263 686c 6967  //www.pytorchlig
-00001440: 6874 6e69 6e67 2e61 692f 292c 2073 6f2c  htning.ai/), so,
-00001450: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-00001460: 706f 7765 7220 6f66 2069 7473 0a20 205b  power of its.  [
-00001470: 5472 6169 6e65 725d 2868 7474 7073 3a2f  Trainer](https:/
-00001480: 2f70 7974 6f72 6368 2d6c 6967 6874 6e69  /pytorch-lightni
-00001490: 6e67 2e72 6561 6474 6865 646f 6373 2e69  ng.readthedocs.i
-000014a0: 6f2f 656e 2f73 7461 626c 652f 636f 6d6d  o/en/stable/comm
-000014b0: 6f6e 2f74 7261 696e 6572 2e68 746d 6c29  on/trainer.html)
-000014c0: 2e0a 2020 5468 6973 2069 7320 6573 7065  ..  This is espe
-000014d0: 6369 616c 6c79 2068 656c 7066 756c 2077  cially helpful w
-000014e0: 6865 6e20 7765 2077 6f72 6b20 7769 7468  hen we work with
-000014f0: 2044 4450 2c20 736f 2c20 796f 7520 636f   DDP, so, you co
-00001500: 6d70 6172 6520 6f75 720a 2020 5b44 4450  mpare our.  [DDP
-00001510: 2065 7861 6d70 6c65 5d28 6874 7470 733a   example](https:
-00001520: 2f2f 6f70 656e 2d6d 6574 7269 632d 6c65  //open-metric-le
-00001530: 6172 6e69 6e67 2e72 6561 6474 6865 646f  arning.readthedo
-00001540: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001550: 6578 616d 706c 6573 2f70 7974 686f 6e2e  examples/python.
-00001560: 6874 6d6c 290a 2020 616e 6420 7468 650a  html).  and the.
-00001570: 2020 5b50 4d4c 7320 6f6e 655d 2868 7474    [PMLs one](htt
-00001580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001590: 4b65 7669 6e4d 7573 6772 6176 652f 7079  KevinMusgrave/py
-000015a0: 746f 7263 682d 6d65 7472 6963 2d6c 6561  torch-metric-lea
-000015b0: 726e 696e 672f 626c 6f62 2f6d 6173 7465  rning/blob/maste
-000015c0: 722f 6578 616d 706c 6573 2f6e 6f74 6562  r/examples/noteb
-000015d0: 6f6f 6b73 2f44 6973 7472 6962 7574 6564  ooks/Distributed
-000015e0: 5472 6970 6c65 744d 6172 6769 6e4c 6f73  TripletMarginLos
-000015f0: 734d 4e49 5354 2e69 7079 6e62 292e 0a20  sMNIST.ipynb).. 
-00001600: 2042 7920 7468 6520 7761 792c 2050 4d4c   By the way, PML
-00001610: 2061 6c73 6f20 6861 7320 5b54 7261 696e   also has [Train
-00001620: 6572 735d 2868 7474 7073 3a2f 2f6b 6576  ers](https://kev
-00001630: 696e 6d75 7367 7261 7665 2e67 6974 6875  inmusgrave.githu
-00001640: 622e 696f 2f70 7974 6f72 6368 2d6d 6574  b.io/pytorch-met
-00001650: 7269 632d 6c65 6172 6e69 6e67 2f74 7261  ric-learning/tra
-00001660: 696e 6572 732f 292c 2062 7574 2069 7427  iners/), but it'
-00001670: 7320 6e6f 740a 2020 7769 6465 6c79 2075  s not.  widely u
-00001680: 7365 6420 696e 2074 6865 2065 7861 6d70  sed in the examp
-00001690: 6c65 7320 616e 6420 6375 7374 6f6d 2060  les and custom `
-000016a0: 7472 6169 6e60 202f 2060 7465 7374 6020  train` / `test` 
-000016b0: 6675 6e63 7469 6f6e 7320 6172 6520 7573  functions are us
-000016c0: 6564 2069 6e73 7465 6164 2e0a 0a57 6520  ed instead...We 
-000016d0: 6265 6c69 6576 6520 7468 6174 2068 6176  believe that hav
-000016e0: 696e 6720 5069 7065 6c69 6e65 732c 206c  ing Pipelines, l
-000016f0: 6163 6f6e 6963 2065 7861 6d70 6c65 732c  aconic examples,
-00001700: 2061 6e64 205a 6f6f 206f 6620 7072 6574   and Zoo of pret
-00001710: 7261 696e 6564 206d 6f64 656c 7320 7365  rained models se
-00001720: 7473 2074 6865 2065 6e74 7279 2074 6872  ts the entry thr
-00001730: 6573 686f 6c64 2074 6f20 6120 7265 616c  eshold to a real
-00001740: 6c79 206c 6f77 2076 616c 7565 2e0a 0a3c  ly low value...<
-00001750: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
-00001760: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
-00001770: 6172 793e 5768 6174 2069 7320 4d65 7472  ary>What is Metr
-00001780: 6963 204c 6561 726e 696e 673f 3c2f 7375  ic Learning?</su
-00001790: 6d6d 6172 793e 0a3c 703e 0a0a 4d65 7472  mmary>.<p>..Metr
-000017a0: 6963 204c 6561 726e 696e 6720 7072 6f62  ic Learning prob
-000017b0: 6c65 6d20 2861 6c73 6f20 6b6e 6f77 6e20  lem (also known 
-000017c0: 6173 202a 6578 7472 656d 6520 636c 6173  as *extreme clas
-000017d0: 7369 6669 6361 7469 6f6e 2a20 7072 6f62  sification* prob
-000017e0: 6c65 6d29 206d 6561 6e73 2061 2073 6974  lem) means a sit
-000017f0: 7561 7469 6f6e 2069 6e20 7768 6963 6820  uation in which 
-00001800: 7765 0a68 6176 6520 7468 6f75 7361 6e64  we.have thousand
-00001810: 7320 6f66 2069 6473 206f 6620 736f 6d65  s of ids of some
-00001820: 2065 6e74 6974 6965 732c 2062 7574 206f   entities, but o
-00001830: 6e6c 7920 6120 6665 7720 7361 6d70 6c65  nly a few sample
-00001840: 7320 666f 7220 6576 6572 7920 656e 7469  s for every enti
-00001850: 7479 2e0a 4f66 7465 6e20 7765 2061 7373  ty..Often we ass
-00001860: 756d 6520 7468 6174 2064 7572 696e 6720  ume that during 
-00001870: 7468 6520 7465 7374 2073 7461 6765 2028  the test stage (
-00001880: 6f72 2070 726f 6475 6374 696f 6e29 2077  or production) w
-00001890: 6520 7769 6c6c 2064 6561 6c20 7769 7468  e will deal with
-000018a0: 2075 6e73 6565 6e20 656e 7469 7469 6573   unseen entities
-000018b0: 0a77 6869 6368 206d 616b 6573 2069 7420  .which makes it 
-000018c0: 696d 706f 7373 6962 6c65 2074 6f20 6170  impossible to ap
-000018d0: 706c 7920 7468 6520 7661 6e69 6c6c 6120  ply the vanilla 
-000018e0: 636c 6173 7369 6669 6361 7469 6f6e 2070  classification p
-000018f0: 6970 656c 696e 6520 6469 7265 6374 6c79  ipeline directly
-00001900: 2e20 496e 206d 616e 7920 6361 7365 7320  . In many cases 
-00001910: 6f62 7461 696e 6564 2065 6d62 6564 6469  obtained embeddi
-00001920: 6e67 730a 6172 6520 7573 6564 2074 6f20  ngs.are used to 
-00001930: 7065 7266 6f72 6d20 7365 6172 6368 206f  perform search o
-00001940: 7220 6d61 7463 6869 6e67 2070 726f 6365  r matching proce
-00001950: 6475 7265 7320 6f76 6572 2074 6865 6d2e  dures over them.
-00001960: 0a0a 4865 7265 2061 7265 2061 2066 6577  ..Here are a few
-00001970: 2065 7861 6d70 6c65 7320 6f66 2073 7563   examples of suc
-00001980: 6820 7461 736b 7320 6672 6f6d 2074 6865  h tasks from the
-00001990: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-000019a0: 2073 7068 6572 653a 0a2a 2050 6572 736f   sphere:.* Perso
-000019b0: 6e2f 416e 696d 616c 2052 652d 4964 656e  n/Animal Re-Iden
-000019c0: 7469 6669 6361 7469 6f6e 0a2a 2046 6163  tification.* Fac
-000019d0: 6520 5265 636f 676e 6974 696f 6e0a 2a20  e Recognition.* 
-000019e0: 4c61 6e64 6d61 726b 2052 6563 6f67 6e69  Landmark Recogni
-000019f0: 7469 6f6e 0a2a 2053 6561 7263 6869 6e67  tion.* Searching
-00001a00: 2065 6e67 696e 6573 2066 6f72 206f 6e6c   engines for onl
-00001a10: 696e 6520 7368 6f70 730a 2061 6e64 206d  ine shops. and m
-00001a20: 616e 7920 6f74 6865 7273 2e0a 3c2f 703e  any others..</p>
-00001a30: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
-00001a40: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00001a50: 3e47 6c6f 7373 6172 7920 284e 616d 696e  >Glossary (Namin
-00001a60: 6720 636f 6e76 656e 7469 6f6e 2920 3c2f  g convention) </
-00001a70: 7375 6d6d 6172 793e 0a3c 703e 0a0a 2a20  summary>.<p>..* 
-00001a80: 6065 6d62 6564 6469 6e67 6020 2d20 6d6f  `embedding` - mo
-00001a90: 6465 6c27 7320 6f75 7470 7574 2028 616c  del's output (al
-00001aa0: 736f 206b 6e6f 776e 2061 7320 6066 6561  so known as `fea
-00001ab0: 7475 7265 7320 7665 6374 6f72 6020 6f72  tures vector` or
-00001ac0: 2060 6465 7363 7269 7074 6f72 6029 2e0a   `descriptor`)..
-00001ad0: 2a20 6071 7565 7279 6020 2d20 6120 7361  * `query` - a sa
-00001ae0: 6d70 6c65 2077 6869 6368 2069 7320 7573  mple which is us
-00001af0: 6564 2061 7320 6120 7265 7175 6573 7420  ed as a request 
-00001b00: 696e 2074 6865 2072 6574 7269 6576 616c  in the retrieval
-00001b10: 2070 726f 6365 6475 7265 2e0a 2a20 6067   procedure..* `g
-00001b20: 616c 6c65 7279 2073 6574 6020 2d20 7468  allery set` - th
-00001b30: 6520 7365 7420 6f66 2065 6e74 6974 6965  e set of entitie
-00001b40: 7320 746f 2073 6561 7263 6820 6974 656d  s to search item
-00001b50: 7320 7369 6d69 6c61 7220 746f 2060 7175  s similar to `qu
-00001b60: 6572 7960 2028 616c 736f 206b 6e6f 776e  ery` (also known
-00001b70: 2061 7320 6072 6566 6572 656e 6365 6020   as `reference` 
-00001b80: 6f72 2060 696e 6465 7860 292e 0a2a 2060  or `index`)..* `
-00001b90: 5361 6d70 6c65 7260 202d 2061 6e20 6172  Sampler` - an ar
-00001ba0: 6775 6d65 6e74 2066 6f72 2060 4461 7461  gument for `Data
-00001bb0: 4c6f 6164 6572 6020 7768 6963 6820 6973  Loader` which is
-00001bc0: 2075 7365 6420 746f 2066 6f72 6d20 6261   used to form ba
-00001bd0: 7463 6865 730a 2a20 604d 696e 6572 6020  tches.* `Miner` 
-00001be0: 2d20 7468 6520 6f62 6a65 6374 2074 6f20  - the object to 
-00001bf0: 666f 726d 2070 6169 7273 206f 7220 7472  form pairs or tr
-00001c00: 6970 6c65 7473 2061 6674 6572 2074 6865  iplets after the
-00001c10: 2062 6174 6368 2077 6173 2066 6f72 6d65   batch was forme
-00001c20: 6420 6279 2060 5361 6d70 6c65 7260 2e20  d by `Sampler`. 
-00001c30: 4974 2773 206e 6f74 206e 6563 6573 7361  It's not necessa
-00001c40: 7279 2074 6f20 666f 726d 0a20 2074 6865  ry to form.  the
-00001c50: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
-00001c60: 2073 616d 706c 6573 206f 6e6c 7920 696e   samples only in
-00001c70: 7369 6465 2074 6865 2063 7572 7265 6e74  side the current
-00001c80: 2062 6174 6368 2c20 7468 7573 2c20 7468   batch, thus, th
-00001c90: 6520 6d65 6d6f 7279 2062 616e 6b20 6d61  e memory bank ma
-00001ca0: 7920 6265 2061 2070 6172 7420 6f66 2060  y be a part of `
-00001cb0: 4d69 6e65 7260 2e0a 2a20 6053 616d 706c  Miner`..* `Sampl
-00001cc0: 6573 602f 604c 6162 656c 7360 2f60 496e  es`/`Labels`/`In
-00001cd0: 7374 616e 6365 7360 202d 2061 7320 616e  stances` - as an
-00001ce0: 2065 7861 6d70 6c65 206c 6574 2773 2063   example let's c
-00001cf0: 6f6e 7369 6465 7220 4465 6570 4661 7368  onsider DeepFash
-00001d00: 696f 6e20 6461 7461 7365 742e 2049 7420  ion dataset. It 
-00001d10: 696e 636c 7564 6573 2074 686f 7573 616e  includes thousan
-00001d20: 6473 206f 660a 2020 6661 7368 696f 6e20  ds of.  fashion 
-00001d30: 6974 656d 2069 6473 2028 7765 206e 616d  item ids (we nam
-00001d40: 6520 7468 656d 2060 6c61 6265 6c73 6029  e them `labels`)
-00001d50: 2061 6e64 2073 6576 6572 616c 2070 686f   and several pho
-00001d60: 746f 7320 666f 7220 6561 6368 2069 7465  tos for each ite
-00001d70: 6d20 6964 0a20 2028 7765 206e 616d 6520  m id.  (we name 
-00001d80: 7468 6520 696e 6469 7669 6475 616c 2070  the individual p
-00001d90: 686f 746f 2061 7320 6069 6e73 7461 6e63  hoto as `instanc
-00001da0: 6560 206f 7220 6073 616d 706c 6560 292e  e` or `sample`).
-00001db0: 2041 6c6c 206f 6620 7468 6520 6661 7368   All of the fash
-00001dc0: 696f 6e20 6974 656d 2069 6473 2068 6176  ion item ids hav
-00001dd0: 6520 7468 6569 7220 6772 6f75 7073 206c  e their groups l
-00001de0: 696b 650a 2020 2273 6b69 7274 7322 2c20  ike.  "skirts", 
-00001df0: 226a 6163 6b65 7473 222c 2022 7368 6f72  "jackets", "shor
-00001e00: 7473 2220 616e 6420 736f 206f 6e20 2877  ts" and so on (w
-00001e10: 6520 6e61 6d65 2074 6865 6d20 6063 6174  e name them `cat
-00001e20: 6567 6f72 6965 7360 292e 0a20 204e 6f74  egories`)..  Not
-00001e30: 652c 2077 6520 6176 6f69 6420 7573 696e  e, we avoid usin
-00001e40: 6720 7468 6520 7465 726d 2060 636c 6173  g the term `clas
-00001e50: 7360 2074 6f20 6176 6f69 6420 6d69 7375  s` to avoid misu
-00001e60: 6e64 6572 7374 616e 6469 6e67 2e0a 2a20  nderstanding..* 
-00001e70: 6074 7261 696e 696e 6720 6570 6f63 6860  `training epoch`
-00001e80: 202d 2062 6174 6368 2073 616d 706c 6572   - batch sampler
-00001e90: 7320 7768 6963 6820 7765 2075 7365 2066  s which we use f
-00001ea0: 6f72 2063 6f6d 6269 6e61 7469 6f6e 2d62  or combination-b
-00001eb0: 6173 6564 206c 6f73 7365 7320 7573 7561  ased losses usua
-00001ec0: 6c6c 7920 6861 7665 2061 206c 656e 6774  lly have a lengt
-00001ed0: 6820 6571 7561 6c20 746f 0a20 2060 5b6e  h equal to.  `[n
-00001ee0: 756d 6265 7220 6f66 206c 6162 656c 7320  umber of labels 
-00001ef0: 696e 2074 7261 696e 696e 6720 6461 7461  in training data
-00001f00: 7365 745d 202f 205b 6e75 6d62 6572 7320  set] / [numbers 
-00001f10: 6f66 206c 6162 656c 7320 696e 206f 6e65  of labels in one
-00001f20: 2062 6174 6368 5d60 2e20 4974 206d 6561   batch]`. It mea
-00001f30: 6e73 2074 6861 7420 7765 2064 6f6e 2774  ns that we don't
-00001f40: 206f 6273 6572 7665 2061 6c6c 206f 660a   observe all of.
-00001f50: 2020 7468 6520 6176 6169 6c61 626c 6520    the available 
-00001f60: 7472 6169 6e69 6e67 2073 616d 706c 6573  training samples
-00001f70: 2069 6e20 6f6e 6520 6570 6f63 6820 2861   in one epoch (a
-00001f80: 7320 6f70 706f 7365 6420 746f 2076 616e  s opposed to van
-00001f90: 696c 6c61 2063 6c61 7373 6966 6963 6174  illa classificat
-00001fa0: 696f 6e29 2c0a 2020 696e 7374 6561 642c  ion),.  instead,
-00001fb0: 2077 6520 6f62 7365 7276 6520 616c 6c20   we observe all 
-00001fc0: 6f66 2074 6865 2061 7661 696c 6162 6c65  of the available
-00001fd0: 206c 6162 656c 732e 0a0a 3c2f 703e 0a3c   labels...</p>.<
-00001fe0: 2f64 6574 6169 6c73 3e0a 0a0a 3c64 6574  /details>...<det
-00001ff0: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e48  ails>.<summary>H
-00002000: 6f77 2067 6f6f 6420 6d61 7920 6265 2061  ow good may be a
-00002010: 206d 6f64 656c 2074 7261 696e 6564 2077   model trained w
-00002020: 6974 6820 4f4d 4c3f 203c 2f73 756d 6d61  ith OML? </summa
-00002030: 7279 3e0a 3c70 3e0a 0a49 7420 6d61 7920  ry>.<p>..It may 
-00002040: 6265 2063 6f6d 7061 7261 626c 6520 7769  be comparable wi
-00002050: 7468 2074 6865 2063 7572 7265 6e74 2028  th the current (
-00002060: 3230 3232 2079 6561 7229 205b 536f 7441  2022 year) [SotA
-00002070: 5d28 6874 7470 733a 2f2f 7061 7065 7273  ](https://papers
-00002080: 7769 7468 636f 6465 2e63 6f6d 2f74 6173  withcode.com/tas
-00002090: 6b2f 6d65 7472 6963 2d6c 6561 726e 696e  k/metric-learnin
-000020a0: 6729 206d 6574 686f 6473 2c0a 666f 7220  g) methods,.for 
-000020b0: 6578 616d 706c 652c 205b 4879 702d 5669  example, [Hyp-Vi
-000020c0: 545d 2868 7474 7073 3a2f 2f61 7278 6976  T](https://arxiv
-000020d0: 2e6f 7267 2f70 6466 2f32 3230 332e 3130  .org/pdf/2203.10
-000020e0: 3833 332e 7064 6629 2e0a 2a28 4665 7720  833.pdf)..*(Few 
-000020f0: 776f 7264 7320 6162 6f75 7420 7468 6973  words about this
-00002100: 2061 7070 726f 6163 683a 2069 7427 7320   approach: it's 
-00002110: 6120 5669 5420 6172 6368 6974 6563 7475  a ViT architectu
-00002120: 7265 2074 7261 696e 6564 2077 6974 6820  re trained with 
-00002130: 636f 6e74 7261 7374 6976 6520 6c6f 7373  contrastive loss
-00002140: 2c0a 6275 7420 7468 6520 656d 6265 6464  ,.but the embedd
-00002150: 696e 6773 2077 6572 6520 7072 6f6a 6563  ings were projec
-00002160: 7465 6420 696e 746f 2073 6f6d 6520 6879  ted into some hy
-00002170: 7065 7262 6f6c 6963 2073 7061 6365 2e0a  perbolic space..
-00002180: 4173 2074 6865 2061 7574 686f 7273 2063  As the authors c
-00002190: 6c61 696d 6564 2c20 7375 6368 2061 2073  laimed, such a s
-000021a0: 7061 6365 2069 7320 6162 6c65 2074 6f20  pace is able to 
-000021b0: 6465 7363 7269 6265 2074 6865 206e 6573  describe the nes
-000021c0: 7465 6420 7374 7275 6374 7572 6520 6f66  ted structure of
-000021d0: 2072 6561 6c2d 776f 726c 6420 6461 7461   real-world data
-000021e0: 2e0a 536f 2c20 7468 6520 7061 7065 7220  ..So, the paper 
-000021f0: 7265 7175 6972 6573 2073 6f6d 6520 6865  requires some he
-00002200: 6176 7920 6d61 7468 2074 6f20 6164 6170  avy math to adap
-00002210: 7420 7468 6520 7573 7561 6c20 6f70 6572  t the usual oper
-00002220: 6174 696f 6e73 2066 6f72 2074 6865 2068  ations for the h
-00002230: 7970 6572 626f 6c69 6361 6c20 7370 6163  yperbolical spac
-00002240: 652e 292a 0a0a 5765 2074 7261 696e 6564  e.)*..We trained
-00002250: 2074 6865 2073 616d 6520 6172 6368 6974   the same archit
-00002260: 6563 7475 7265 2077 6974 6820 7472 6970  ecture with trip
-00002270: 6c65 7420 6c6f 7373 2c20 6669 7869 6e67  let loss, fixing
-00002280: 2074 6865 2072 6573 7420 6f66 2074 6865   the rest of the
-00002290: 2070 6172 616d 6574 6572 733a 0a74 7261   parameters:.tra
-000022a0: 696e 696e 6720 616e 6420 7465 7374 2074  ining and test t
-000022b0: 7261 6e73 666f 726d 6174 696f 6e73 2c20  ransformations, 
-000022c0: 696d 6167 6520 7369 7a65 2c20 616e 6420  image size, and 
-000022d0: 6f70 7469 6d69 7a65 722e 2053 6565 2063  optimizer. See c
-000022e0: 6f6e 6669 6773 2069 6e20 5b4d 6f64 656c  onfigs in [Model
-000022f0: 7320 5a6f 6f5d 2868 7474 7073 3a2f 2f67  s Zoo](https://g
-00002300: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-00002310: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-00002320: 6561 726e 696e 6723 7a6f 6f29 2e0a 5468  earning#zoo)..Th
-00002330: 6520 7472 6963 6b20 7761 7320 696e 2068  e trick was in h
-00002340: 6575 7269 7374 6963 7320 696e 206f 7572  euristics in our
-00002350: 206d 696e 6572 2061 6e64 2073 616d 706c   miner and sampl
-00002360: 6572 3a0a 0a2a 205b 4361 7465 676f 7279  er:..* [Category
-00002370: 2042 616c 616e 6365 2053 616d 706c 6572   Balance Sampler
-00002380: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00002390: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-000023a0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000023b0: 2f6c 6174 6573 742f 636f 6e74 656e 7473  /latest/contents
-000023c0: 2f73 616d 706c 6572 732e 6874 6d6c 2363  /samplers.html#c
-000023d0: 6174 6567 6f72 7962 616c 616e 6365 7361  ategorybalancesa
-000023e0: 6d70 6c65 7229 0a20 2066 6f72 6d73 2074  mpler).  forms t
-000023f0: 6865 2062 6174 6368 6573 206c 696d 6974  he batches limit
-00002400: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
-00002410: 6620 6361 7465 676f 7269 6573 202a 432a  f categories *C*
-00002420: 2069 6e20 6974 2e0a 2020 466f 7220 696e   in it..  For in
-00002430: 7374 616e 6365 2c20 7768 656e 202a 4320  stance, when *C 
-00002440: 3d20 312a 2069 7420 7075 7473 206f 6e6c  = 1* it puts onl
-00002450: 7920 6a61 636b 6574 7320 696e 206f 6e65  y jackets in one
-00002460: 2062 6174 6368 2061 6e64 206f 6e6c 7920   batch and only 
-00002470: 6a65 616e 7320 696e 746f 2061 6e6f 7468  jeans into anoth
-00002480: 6572 206f 6e65 2028 6a75 7374 2061 6e20  er one (just an 
-00002490: 6578 616d 706c 6529 2e0a 2020 4974 2061  example)..  It a
-000024a0: 7574 6f6d 6174 6963 616c 6c79 206d 616b  utomatically mak
-000024b0: 6573 2074 6865 206e 6567 6174 6976 6520  es the negative 
-000024c0: 7061 6972 7320 6861 7264 6572 3a20 6974  pairs harder: it
-000024d0: 2773 206d 6f72 6520 6d65 616e 696e 6766  's more meaningf
-000024e0: 756c 2066 6f72 2061 206d 6f64 656c 2074  ul for a model t
-000024f0: 6f20 7265 616c 6973 6520 7768 7920 7477  o realise why tw
-00002500: 6f20 6a61 636b 6574 730a 2020 6172 6520  o jackets.  are 
-00002510: 6469 6666 6572 656e 7420 7468 616e 2074  different than t
-00002520: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00002530: 2073 616d 6520 6162 6f75 7420 6120 6a61   same about a ja
-00002540: 636b 6574 2061 6e64 2061 2074 2d73 6869  cket and a t-shi
-00002550: 7274 2e0a 0a2a 205b 4861 7264 2054 7269  rt...* [Hard Tri
-00002560: 706c 6574 7320 4d69 6e65 725d 2868 7474  plets Miner](htt
-00002570: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-00002580: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-00002590: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000025a0: 7374 2f63 6f6e 7465 6e74 732f 6d69 6e65  st/contents/mine
-000025b0: 7273 2e68 746d 6c23 6861 7264 7472 6970  rs.html#hardtrip
-000025c0: 6c65 7473 6d69 6e65 7229 0a20 206d 616b  letsminer).  mak
-000025d0: 6573 2074 6865 2074 6173 6b20 6576 656e  es the task even
-000025e0: 2068 6172 6465 7220 6b65 6570 696e 6720   harder keeping 
-000025f0: 6f6e 6c79 2074 6865 2068 6172 6465 7374  only the hardest
-00002600: 2074 7269 706c 6574 7320 2877 6974 6820   triplets (with 
-00002610: 6d61 7869 6d61 6c20 706f 7369 7469 7665  maximal positive
-00002620: 2061 6e64 206d 696e 696d 616c 206e 6567   and minimal neg
-00002630: 6174 6976 6520 6469 7374 616e 6365 7329  ative distances)
-00002640: 2e0a 0a48 6572 6520 6172 6520 2a43 4d43  ...Here are *CMC
-00002650: 4031 2a20 7363 6f72 6573 2066 6f72 2032  @1* scores for 2
-00002660: 2070 6f70 756c 6172 2062 656e 6368 6d61   popular benchma
-00002670: 726b 732e 0a53 4f50 2064 6174 6173 6574  rks..SOP dataset
-00002680: 3a20 4879 702d 5669 5420 e280 9420 3835  : Hyp-ViT ... 85
-00002690: 2e39 2c20 6f75 7273 20e2 8094 2038 362e  .9, ours ... 86.
-000026a0: 362e 2044 6565 7046 6173 6869 6f6e 2064  6. DeepFashion d
-000026b0: 6174 6173 6574 3a20 4879 702d 5669 5420  ataset: Hyp-ViT 
-000026c0: e280 9420 3932 2e35 2c20 6f75 7273 20e2  ... 92.5, ours .
-000026d0: 8094 2039 322e 312e 0a54 6875 732c 2075  .. 92.1..Thus, u
-000026e0: 7469 6c69 7369 6e67 2073 696d 706c 6520  tilising simple 
-000026f0: 6865 7572 6973 7469 6373 2061 6e64 2061  heuristics and a
-00002700: 766f 6964 696e 6720 6865 6176 7920 6d61  voiding heavy ma
-00002710: 7468 2077 6520 6172 6520 6162 6c65 2074  th we are able t
-00002720: 6f20 7065 7266 6f72 6d20 6f6e 2053 6f74  o perform on Sot
-00002730: 4120 6c65 7665 6c2e 0a0a 3c2f 703e 0a3c  A level...</p>.<
-00002740: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-00002750: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-00002760: 6174 2061 626f 7574 2053 656c 662d 5375  at about Self-Su
-00002770: 7065 7276 6973 6564 204c 6561 726e 696e  pervised Learnin
-00002780: 673f 3c2f 7375 6d6d 6172 793e 0a3c 703e  g?</summary>.<p>
-00002790: 0a0a 5265 6365 6e74 2072 6573 6561 7263  ..Recent researc
-000027a0: 6820 696e 2053 534c 2064 6566 696e 6974  h in SSL definit
-000027b0: 656c 7920 6f62 7461 696e 6564 2067 7265  ely obtained gre
-000027c0: 6174 2072 6573 756c 7473 2e20 5468 6520  at results. The 
-000027d0: 7072 6f62 6c65 6d20 6973 2074 6861 7420  problem is that 
-000027e0: 7468 6573 6520 6170 7072 6f61 6368 6573  these approaches
-000027f0: 0a72 6571 7569 7265 6420 616e 2065 6e6f  .required an eno
-00002800: 726d 6f75 7320 616d 6f75 6e74 206f 6620  rmous amount of 
-00002810: 636f 6d70 7574 696e 6720 746f 2074 7261  computing to tra
-00002820: 696e 2074 6865 206d 6f64 656c 2e20 4275  in the model. Bu
-00002830: 7420 696e 206f 7572 2066 7261 6d65 776f  t in our framewo
-00002840: 726b 2c20 7765 2063 6f6e 7369 6465 7220  rk, we consider 
-00002850: 7468 6520 6d6f 7374 2063 6f6d 6d6f 6e20  the most common 
-00002860: 6361 7365 0a77 6865 6e20 7468 6520 6176  case.when the av
-00002870: 6572 6167 6520 7573 6572 2068 6173 206e  erage user has n
-00002880: 6f20 6d6f 7265 2074 6861 6e20 6120 6665  o more than a fe
-00002890: 7720 4750 5573 2e0a 0a41 7420 7468 6520  w GPUs...At the 
-000028a0: 7361 6d65 2074 696d 652c 2069 7420 776f  same time, it wo
-000028b0: 756c 6420 6265 2075 6e77 6973 6520 746f  uld be unwise to
-000028c0: 2069 676e 6f72 6520 7375 6363 6573 7320   ignore success 
-000028d0: 696e 2074 6869 7320 7370 6865 7265 2c20  in this sphere, 
-000028e0: 736f 2077 6520 7374 696c 6c20 6578 706c  so we still expl
-000028f0: 6f69 7420 6974 2069 6e20 7477 6f20 7761  oit it in two wa
-00002900: 7973 3a0a 2a20 4173 2061 2073 6f75 7263  ys:.* As a sourc
-00002910: 6520 6f66 2063 6865 636b 706f 696e 7473  e of checkpoints
-00002920: 2074 6861 7420 776f 756c 6420 6265 2067   that would be g
-00002930: 7265 6174 2074 6f20 7374 6172 7420 7472  reat to start tr
-00002940: 6169 6e69 6e67 2077 6974 682e 2046 726f  aining with. Fro
-00002950: 6d20 7075 626c 6963 6174 696f 6e73 2061  m publications a
-00002960: 6e64 206f 7572 2065 7870 6572 6965 6e63  nd our experienc
-00002970: 652c 0a20 2074 6865 7920 6172 6520 6d75  e,.  they are mu
-00002980: 6368 2062 6574 7465 7220 6173 2069 6e69  ch better as ini
-00002990: 7469 616c 6973 6174 696f 6e20 7468 616e  tialisation than
-000029a0: 2074 6865 2064 6566 6175 6c74 2073 7570   the default sup
-000029b0: 6572 7669 7365 6420 6d6f 6465 6c20 7472  ervised model tr
-000029c0: 6169 6e65 6420 6f6e 2049 6d61 6765 4e65  ained on ImageNe
-000029d0: 742e 2054 6875 732c 2077 6520 6164 6465  t. Thus, we adde
-000029e0: 6420 7468 6520 706f 7373 6962 696c 6974  d the possibilit
-000029f0: 790a 2020 746f 2069 6e69 7469 616c 6973  y.  to initialis
-00002a00: 6520 796f 7572 206d 6f64 656c 7320 7573  e your models us
-00002a10: 696e 6720 7468 6573 6520 7072 6574 7261  ing these pretra
-00002a20: 696e 6564 2063 6865 636b 706f 696e 7473  ined checkpoints
-00002a30: 206f 6e6c 7920 6279 2070 6173 7369 6e67   only by passing
-00002a40: 2061 6e20 6172 6775 6d65 6e74 2069 6e20   an argument in 
-00002a50: 7468 6520 636f 6e66 6967 206f 7220 7468  the config or th
-00002a60: 6520 636f 6e73 7472 7563 746f 722e 0a2a  e constructor..*
-00002a70: 2041 7320 6120 736f 7572 6365 206f 6620   As a source of 
-00002a80: 696e 7370 6972 6174 696f 6e2e 2046 6f72  inspiration. For
-00002a90: 2065 7861 6d70 6c65 2c20 7765 2061 6461   example, we ada
-00002aa0: 7074 6564 2074 6865 2069 6465 6120 6f66  pted the idea of
-00002ab0: 2061 206d 656d 6f72 7920 6261 6e6b 2066   a memory bank f
-00002ac0: 726f 6d20 2a4d 6f43 6f2a 2066 6f72 2074  rom *MoCo* for t
-00002ad0: 6865 202a 5472 6970 6c65 744c 6f73 732a  he *TripletLoss*
-00002ae0: 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461 696c  ...</p>.</detail
-00002af0: 733e 0a0a 0a3c 6465 7461 696c 733e 0a3c  s>...<details>.<
-00002b00: 7375 6d6d 6172 793e 446f 2049 206e 6565  summary>Do I nee
-00002b10: 6420 746f 206b 6e6f 7720 6f74 6865 7220  d to know other 
-00002b20: 6672 616d 6577 6f72 6b73 2074 6f20 7573  frameworks to us
-00002b30: 6520 4f4d 4c3f 3c2f 7375 6d6d 6172 793e  e OML?</summary>
-00002b40: 0a3c 703e 0a0a 4e6f 2c20 796f 7520 646f  .<p>..No, you do
-00002b50: 6e27 742e 204f 4d4c 2069 7320 6120 6672  n't. OML is a fr
-00002b60: 616d 6577 6f72 6b2d 6167 6e6f 7374 6963  amework-agnostic
-00002b70: 2e20 4465 7370 6974 6520 7765 2075 7365  . Despite we use
-00002b80: 2050 7954 6f72 6368 204c 6967 6874 6e69   PyTorch Lightni
-00002b90: 6e67 2061 7320 6120 6c6f 6f70 0a72 756e  ng as a loop.run
-00002ba0: 6e65 7220 666f 7220 7468 6520 6578 7065  ner for the expe
-00002bb0: 7269 6d65 6e74 732c 2077 6520 616c 736f  riments, we also
-00002bc0: 206b 6565 7020 7468 6520 706f 7373 6962   keep the possib
-00002bd0: 696c 6974 7920 746f 2072 756e 2065 7665  ility to run eve
-00002be0: 7279 7468 696e 6720 6f6e 2070 7572 6520  rything on pure 
-00002bf0: 5079 546f 7263 682e 0a54 6875 732c 206f  PyTorch..Thus, o
-00002c00: 6e6c 7920 7468 6520 7469 6e79 2070 6172  nly the tiny par
-00002c10: 7420 6f66 204f 4d4c 2069 7320 4c69 6768  t of OML is Ligh
-00002c20: 746e 696e 672d 7370 6563 6966 6963 2061  tning-specific a
-00002c30: 6e64 2077 6520 6b65 6570 2074 6869 7320  nd we keep this 
-00002c40: 6c6f 6769 6320 7365 7061 7261 7465 6c79  logic separately
-00002c50: 2066 726f 6d0a 6f74 6865 7220 636f 6465   from.other code
-00002c60: 2028 7365 6520 606f 6d6c 2e6c 6967 6874   (see `oml.light
-00002c70: 6e69 6e67 6029 2e20 4576 656e 2077 6865  ning`). Even whe
-00002c80: 6e20 796f 7520 7573 6520 4c69 6768 746e  n you use Lightn
-00002c90: 696e 672c 2079 6f75 2064 6f6e 2774 206e  ing, you don't n
-00002ca0: 6565 6420 746f 206b 6e6f 7720 6974 2c20  eed to know it, 
-00002cb0: 7369 6e63 650a 7765 2070 726f 7669 6465  since.we provide
-00002cc0: 2072 6561 6479 2074 6f20 7573 6520 5b50   ready to use [P
-00002cd0: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
-00002ce0: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00002cf0: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00002d00: 632d 6c65 6172 6e69 6e67 2f62 6c6f 622f  c-learning/blob/
-00002d10: 6d61 696e 2f70 6970 656c 696e 6573 2f29  main/pipelines/)
-00002d20: 2e0a 0a54 6865 2070 6f73 7369 6269 6c69  ...The possibili
-00002d30: 7479 206f 6620 7573 696e 6720 7075 7265  ty of using pure
-00002d40: 2050 7954 6f72 6368 2061 6e64 206d 6f64   PyTorch and mod
-00002d50: 756c 6172 2073 7472 7563 7475 7265 206f  ular structure o
-00002d60: 6620 7468 6520 636f 6465 206c 6561 7665  f the code leave
-00002d70: 7320 6120 726f 6f6d 2066 6f72 2075 7469  s a room for uti
-00002d80: 6c69 7a69 6e67 0a4f 4d4c 2077 6974 6820  lizing.OML with 
-00002d90: 796f 7572 2066 6176 6f75 7269 7465 2066  your favourite f
-00002da0: 7261 6d65 776f 726b 2061 6674 6572 2074  ramework after t
-00002db0: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
-00002dc0: 6e20 6f66 2074 6865 206e 6563 6573 7361  n of the necessa
-00002dd0: 7279 2077 7261 7070 6572 732e 0a0a 3c2f  ry wrappers...</
-00002de0: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
-00002df0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
-00002e00: 7279 3e43 616e 2049 2075 7365 204f 4d4c  ry>Can I use OML
-00002e10: 2077 6974 686f 7574 2061 6e79 206b 6e6f   without any kno
-00002e20: 776c 6564 6765 2069 6e20 4461 7461 5363  wledge in DataSc
-00002e30: 6965 6e63 653f 3c2f 7375 6d6d 6172 793e  ience?</summary>
-00002e40: 0a3c 703e 0a0a 5965 732e 2054 6f20 7275  .<p>..Yes. To ru
-00002e50: 6e20 7468 6520 6578 7065 7269 6d65 6e74  n the experiment
-00002e60: 2077 6974 6820 5b50 6970 656c 696e 6573   with [Pipelines
-00002e70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002e80: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00002e90: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00002ea0: 6e67 2f62 6c6f 622f 6d61 696e 2f70 6970  ng/blob/main/pip
-00002eb0: 656c 696e 6573 2f29 0a79 6f75 206f 6e6c  elines/).you onl
-00002ec0: 7920 6e65 6564 2074 6f20 7772 6974 6520  y need to write 
-00002ed0: 6120 636f 6e76 6572 7465 720a 746f 206f  a converter.to o
-00002ee0: 7572 2066 6f72 6d61 7420 2869 7420 6d65  ur format (it me
-00002ef0: 616e 7320 7072 6570 6172 696e 6720 7468  ans preparing th
-00002f00: 650a 602e 6373 7660 2074 6162 6c65 2077  e.`.csv` table w
-00002f10: 6974 6820 3520 7072 6564 6566 696e 6564  ith 5 predefined
-00002f20: 2063 6f6c 756d 6e73 292e 0a54 6861 7427   columns)..That'
-00002f30: 7320 6974 210a 0a50 726f 6261 626c 7920  s it!..Probably 
-00002f40: 7765 2061 6c72 6561 6479 2068 6176 6520  we already have 
-00002f50: 6120 7375 6974 6162 6c65 2070 7265 2d74  a suitable pre-t
-00002f60: 7261 696e 6564 206d 6f64 656c 2066 6f72  rained model for
-00002f70: 2079 6f75 7220 646f 6d61 696e 0a69 6e20   your domain.in 
-00002f80: 6f75 7220 2a4d 6f64 656c 7320 5a6f 6f2a  our *Models Zoo*
-00002f90: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
-00002fa0: 796f 7520 646f 6e27 7420 6576 656e 206e  you don't even n
-00002fb0: 6565 6420 746f 2074 7261 696e 2069 742e  eed to train it.
-00002fc0: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-00002fd0: 0a0a 2323 205b 446f 6375 6d65 6e74 6174  ..## [Documentat
-00002fe0: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
-00002ff0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-00003000: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
-00003010: 2f65 6e2f 6c61 7465 7374 2f69 6e64 6578  /en/latest/index
-00003020: 2e68 746d 6c29 0a0a 446f 6375 6d65 6e74  .html)..Document
-00003030: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-00003040: 6c65 2076 6961 2074 6865 205b 6c69 6e6b  le via the [link
-00003050: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00003060: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00003070: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00003080: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
-00003090: 6d6c 292e 0a0a 596f 7520 6361 6e20 616c  ml)...You can al
-000030a0: 736f 2072 6561 6420 736f 6d65 2065 7874  so read some ext
-000030b0: 7261 206d 6174 6572 6961 6c73 2072 656c  ra materials rel
-000030c0: 6174 6564 2074 6f20 4f4d 4c3a 0a0a 2a20  ated to OML:..* 
-000030d0: 5468 656f 7279 2061 6e64 2070 7261 6374  Theory and pract
-000030e0: 6963 6520 6f66 206d 6574 7269 6320 6c65  ice of metric le
-000030f0: 6172 6e69 6e67 2077 6974 6820 7468 6520  arning with the 
-00003100: 7573 6167 6520 6f66 204f 4d4c 2e0a 5b50  usage of OML..[P
-00003110: 6f73 7420 696e 2045 6e67 6c69 7368 206f  ost in English o
-00003120: 6e20 4d65 6469 756d 5d28 6874 7470 733a  n Medium](https:
-00003130: 2f2f 6d65 6469 756d 2e63 6f6d 2f40 416c  //medium.com/@Al
-00003140: 656b 7365 6953 6861 6261 6e6f 762f 7072  ekseiShabanov/pr
-00003150: 6163 7469 6361 6c2d 6d65 7472 6963 2d6c  actical-metric-l
-00003160: 6561 726e 696e 672d 6230 3431 3063 6461  earning-b0410cda
-00003170: 3232 3031 2920 7c0a 5b50 6f73 7420 696e  2201) |.[Post in
-00003180: 2052 7573 7369 616e 206f 6e20 4861 6272   Russian on Habr
-00003190: 5d28 6874 7470 733a 2f2f 6861 6272 2e63  ](https://habr.c
-000031a0: 6f6d 2f72 752f 636f 6d70 616e 792f 6f64  om/ru/company/od
-000031b0: 732f 626c 6f67 2f36 3935 3338 302f 2920  s/blog/695380/) 
-000031c0: 7c0a 5b50 6f73 7420 696e 2043 6869 6e65  |.[Post in Chine
-000031d0: 7365 206f 6e20 4353 444e 5d28 6874 7470  se on CSDN](http
-000031e0: 733a 2f2f 626c 6f67 2e63 7364 6e2e 6e65  s://blog.csdn.ne
-000031f0: 742f 6665 726d 696f 6e30 3231 372f 6172  t/fermion0217/ar
-00003200: 7469 636c 652f 6465 7461 696c 732f 3132  ticle/details/12
-00003210: 3739 3332 3038 3729 2c20 7472 616e 736c  7932087), transl
-00003220: 6174 6564 2062 7920 4368 6961 2d43 6865  ated by Chia-Che
-00003230: 6e20 4368 616e 672e 0a0a 2a20 5468 650a  n Chang...* The.
-00003240: 5b44 454d 4f5d 2868 7474 7073 3a2f 2f64  [DEMO](https://d
-00003250: 6170 6c61 646f 632d 6f6d 6c2d 706f 7374  apladoc-oml-post
-00003260: 7072 6f63 6573 7369 6e67 2d64 656d 6f2d  processing-demo-
-00003270: 7372 6361 7070 6d61 696e 2d70 6668 3267  srcappmain-pfh2g
-00003280: 302e 7374 7265 616d 6c69 742e 6170 702f  0.streamlit.app/
-00003290: 290a 666f 7220 6f75 7220 7061 7065 720a  ).for our paper.
-000032a0: 5b53 5449 523a 2053 6961 6d65 7365 2054  [STIR: Siamese T
-000032b0: 7261 6e73 666f 726d 6572 7320 666f 7220  ransformers for 
-000032c0: 496d 6167 6520 5265 7472 6965 7661 6c20  Image Retrieval 
-000032d0: 506f 7374 7072 6f63 6573 7369 6e67 5d28  Postprocessing](
-000032e0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-000032f0: 672f 6162 732f 3233 3034 2e31 3333 3933  g/abs/2304.13393
-00003300: 290a 0a2a 2054 6865 2072 6570 6f72 7420  )..* The report 
-00003310: 666f 7220 4265 726c 696e 2d62 6173 6564  for Berlin-based
-00003320: 206d 6565 7475 703a 2022 436f 6d70 7574   meetup: "Comput
-00003330: 6572 2056 6973 696f 6e20 696e 2070 726f  er Vision in pro
-00003340: 6475 6374 696f 6e22 2e20 4e6f 7665 6d62  duction". Novemb
-00003350: 6572 2c20 3230 3232 2e0a 5b4c 696e 6b5d  er, 2022..[Link]
-00003360: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00003370: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00003380: 666f 6c64 6572 732f 3175 486d 4c55 3876  folders/1uHmLU8v
-00003390: 4d72 4d56 4d46 6f64 7433 3675 3075 5841  MrMVMFodt36u0uXA
-000033a0: 6759 6a47 5f33 4433 303f 7573 703d 7368  gYjG_3D30?usp=sh
-000033b0: 6172 655f 6c69 6e6b 290a 0a23 2320 5b49  are_link)..## [I
-000033c0: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
-000033d0: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-000033e0: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-000033f0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003400: 7374 2f6f 6d6c 2f69 6e73 7461 6c6c 6174  st/oml/installat
-00003410: 696f 6e2e 6874 6d6c 290a 0a4f 4d4c 2069  ion.html)..OML i
-00003420: 7320 6176 6169 6c61 626c 6520 696e 2050  s available in P
-00003430: 7950 493a 0a0a 6060 6073 6865 6c6c 0a70  yPI:..```shell.p
-00003440: 6970 2069 6e73 7461 6c6c 202d 5520 6f70  ip install -U op
-00003450: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00003460: 6e67 0a60 6060 0a0a 596f 7520 6361 6e20  ng.```..You can 
-00003470: 616c 736f 2070 756c 6c20 7468 6520 7072  also pull the pr
-00003480: 6570 6172 6564 2069 6d61 6765 2066 726f  epared image fro
-00003490: 6d20 446f 636b 6572 4875 622e 2e2e 0a0a  m DockerHub.....
-000034a0: 6060 6073 6865 6c6c 0a64 6f63 6b65 7220  ```shell.docker 
-000034b0: 7075 6c6c 206f 6d6c 7465 616d 2f6f 6d6c  pull omlteam/oml
-000034c0: 3a67 7075 0a64 6f63 6b65 7220 7075 6c6c  :gpu.docker pull
-000034d0: 206f 6d6c 7465 616d 2f6f 6d6c 3a63 7075   omlteam/oml:cpu
-000034e0: 0a60 6060 0a0a 2e2e 2e6f 7220 6275 696c  .```.....or buil
-000034f0: 6420 6f6e 6520 6279 2079 6f75 7220 6f77  d one by your ow
-00003500: 6e0a 0a60 6060 7368 656c 6c0a 6d61 6b65  n..```shell.make
-00003510: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
-00003520: 4e54 494d 453d 6370 750a 6d61 6b65 2064  NTIME=cpu.make d
-00003530: 6f63 6b65 725f 6275 696c 6420 5255 4e54  ocker_build RUNT
-00003540: 494d 453d 6770 750a 6060 600a 0a23 2320  IME=gpu.```..## 
-00003550: 5b45 7861 6d70 6c65 735d 2868 7474 7073  [Examples](https
-00003560: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
-00003570: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
-00003580: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003590: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
-000035a0: 696f 6e2f 7079 7468 6f6e 5f65 7861 6d70  ion/python_examp
-000035b0: 6c65 732e 6874 6d6c 2329 0a0a 3c64 6574  les.html#)..<det
-000035c0: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e54  ails>.<summary>T
-000035d0: 7261 696e 696e 673c 2f73 756d 6d61 7279  raining</summary
-000035e0: 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e 745d  >.<p>..[comment]
-000035f0: 3a76 616e 696c 6c61 2d74 7261 696e 2d73  :vanilla-train-s
-00003600: 7461 7274 0a60 6060 7079 7468 6f6e 0a69  tart.```python.i
-00003610: 6d70 6f72 7420 746f 7263 680a 6672 6f6d  mport torch.from
-00003620: 2074 7164 6d20 696d 706f 7274 2074 7164   tqdm import tqd
-00003630: 6d0a 0a66 726f 6d20 6f6d 6c2e 6461 7461  m..from oml.data
-00003640: 7365 7473 2e62 6173 6520 696d 706f 7274  sets.base import
-00003650: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
-00003660: 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ls.from oml.loss
-00003670: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
-00003680: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
-00003690: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
-000036a0: 6d69 6e65 7273 2e69 6e62 6174 6368 5f61  miners.inbatch_a
-000036b0: 6c6c 5f74 7269 2069 6d70 6f72 7420 416c  ll_tri import Al
-000036c0: 6c54 7269 706c 6574 734d 696e 6572 0a66  lTripletsMiner.f
-000036d0: 726f 6d20 6f6d 6c2e 6d6f 6465 6c73 2069  rom oml.models i
-000036e0: 6d70 6f72 7420 5669 5445 7874 7261 6374  mport ViTExtract
-000036f0: 6f72 0a66 726f 6d20 6f6d 6c2e 7361 6d70  or.from oml.samp
-00003700: 6c65 7273 2e62 616c 616e 6365 2069 6d70  lers.balance imp
-00003710: 6f72 7420 4261 6c61 6e63 6553 616d 706c  ort BalanceSampl
-00003720: 6572 0a66 726f 6d20 6f6d 6c2e 7574 696c  er.from oml.util
-00003730: 732e 646f 776e 6c6f 6164 5f6d 6f63 6b5f  s.download_mock_
-00003740: 6461 7461 7365 7420 696d 706f 7274 2064  dataset import d
-00003750: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
-00003760: 6173 6574 0a0a 6461 7461 7365 745f 726f  aset..dataset_ro
-00003770: 6f74 203d 2022 6d6f 636b 5f64 6174 6173  ot = "mock_datas
-00003780: 6574 2f22 0a64 665f 7472 6169 6e2c 205f  et/".df_train, _
-00003790: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-000037a0: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-000037b0: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-000037c0: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-000037d0: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-000037e0: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-000037f0: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00003800: 733d 4661 6c73 6529 2e74 7261 696e 2829  s=False).train()
-00003810: 0a6f 7074 696d 697a 6572 203d 2074 6f72  .optimizer = tor
-00003820: 6368 2e6f 7074 696d 2e53 4744 2865 7874  ch.optim.SGD(ext
-00003830: 7261 6374 6f72 2e70 6172 616d 6574 6572  ractor.parameter
-00003840: 7328 292c 206c 723d 3165 2d36 290a 0a74  s(), lr=1e-6)..t
-00003850: 7261 696e 5f64 6174 6173 6574 203d 2044  rain_dataset = D
-00003860: 6174 6173 6574 5769 7468 4c61 6265 6c73  atasetWithLabels
-00003870: 2864 665f 7472 6169 6e2c 2064 6174 6173  (df_train, datas
-00003880: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00003890: 726f 6f74 290a 6372 6974 6572 696f 6e20  root).criterion 
-000038a0: 3d20 5472 6970 6c65 744c 6f73 7357 6974  = TripletLossWit
-000038b0: 684d 696e 6572 286d 6172 6769 6e3d 302e  hMiner(margin=0.
-000038c0: 312c 206d 696e 6572 3d41 6c6c 5472 6970  1, miner=AllTrip
-000038d0: 6c65 7473 4d69 6e65 7228 292c 206e 6565  letsMiner(), nee
-000038e0: 645f 6c6f 6773 3d54 7275 6529 0a73 616d  d_logs=True).sam
-000038f0: 706c 6572 203d 2042 616c 616e 6365 5361  pler = BalanceSa
-00003900: 6d70 6c65 7228 7472 6169 6e5f 6461 7461  mpler(train_data
-00003910: 7365 742e 6765 745f 6c61 6265 6c73 2829  set.get_labels()
-00003920: 2c20 6e5f 6c61 6265 6c73 3d32 2c20 6e5f  , n_labels=2, n_
-00003930: 696e 7374 616e 6365 733d 3229 0a74 7261  instances=2).tra
-00003940: 696e 5f6c 6f61 6465 7220 3d20 746f 7263  in_loader = torc
-00003950: 682e 7574 696c 732e 6461 7461 2e44 6174  h.utils.data.Dat
-00003960: 614c 6f61 6465 7228 7472 6169 6e5f 6461  aLoader(train_da
-00003970: 7461 7365 742c 2062 6174 6368 5f73 616d  taset, batch_sam
-00003980: 706c 6572 3d73 616d 706c 6572 290a 0a66  pler=sampler)..f
-00003990: 6f72 2062 6174 6368 2069 6e20 7471 646d  or batch in tqdm
-000039a0: 2874 7261 696e 5f6c 6f61 6465 7229 3a0a  (train_loader):.
-000039b0: 2020 2020 656d 6265 6464 696e 6773 203d      embeddings =
-000039c0: 2065 7874 7261 6374 6f72 2862 6174 6368   extractor(batch
-000039d0: 5b22 696e 7075 745f 7465 6e73 6f72 7322  ["input_tensors"
-000039e0: 5d29 0a20 2020 206c 6f73 7320 3d20 6372  ]).    loss = cr
-000039f0: 6974 6572 696f 6e28 656d 6265 6464 696e  iterion(embeddin
-00003a00: 6773 2c20 6261 7463 685b 226c 6162 656c  gs, batch["label
-00003a10: 7322 5d29 0a20 2020 206c 6f73 732e 6261  s"]).    loss.ba
-00003a20: 636b 7761 7264 2829 0a20 2020 206f 7074  ckward().    opt
-00003a30: 696d 697a 6572 2e73 7465 7028 290a 2020  imizer.step().  
-00003a40: 2020 6f70 7469 6d69 7a65 722e 7a65 726f    optimizer.zero
-00003a50: 5f67 7261 6428 290a 0a20 2020 2023 2069  _grad()..    # i
-00003a60: 6e66 6f20 666f 7220 6c6f 6767 696e 673a  nfo for logging:
-00003a70: 2070 6f73 6974 6976 652f 6e65 6761 7469   positive/negati
-00003a80: 7665 2064 6973 7461 6e63 6573 2c20 6e75  ve distances, nu
-00003a90: 6d62 6572 206f 6620 6163 7469 7665 2074  mber of active t
-00003aa0: 7269 706c 6574 730a 2020 2020 7072 696e  riplets.    prin
-00003ab0: 7428 6372 6974 6572 696f 6e2e 6c61 7374  t(criterion.last
-00003ac0: 5f6c 6f67 7329 0a0a 6060 600a 5b63 6f6d  _logs)..```.[com
-00003ad0: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7472  ment]:vanilla-tr
-00003ae0: 6169 6e2d 656e 640a 3c2f 703e 0a3c 2f64  ain-end.</p>.</d
-00003af0: 6574 6169 6c73 3e0a 0a5b 215b 4f70 656e  etails>..[![Open
-00003b00: 2049 6e20 436f 6c61 625d 2868 7474 7073   In Colab](https
-00003b10: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00003b20: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-00003b30: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-00003b40: 7376 6729 5d28 6874 7470 733a 2f2f 636f  svg)](https://co
-00003b50: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00003b60: 676c 652e 636f 6d2f 6472 6976 652f 316b  gle.com/drive/1k
-00003b70: 6e74 4441 4964 495a 394c 3430 6a63 6e64  ntDAIdIZ9L40jcnd
-00003b80: 6775 4c41 622d 5871 6d43 464f 6753 353f  guLAb-XqmCFOgS5?
-00003b90: 7573 703d 7368 6172 696e 6729 0a3c 6465  usp=sharing).<de
-00003ba0: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
-00003bb0: 5661 6c69 6461 7469 6f6e 3c2f 7375 6d6d  Validation</summ
-00003bc0: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-00003bd0: 6e74 5d3a 7661 6e69 6c6c 612d 7661 6c69  nt]:vanilla-vali
-00003be0: 6461 7469 6f6e 2d73 7461 7274 0a60 6060  dation-start.```
-00003bf0: 7079 7468 6f6e 0a69 6d70 6f72 7420 746f  python.import to
-00003c00: 7263 680a 6672 6f6d 2074 7164 6d20 696d  rch.from tqdm im
-00003c10: 706f 7274 2074 7164 6d0a 0a66 726f 6d20  port tqdm..from 
-00003c20: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-00003c30: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-00003c40: 5175 6572 7947 616c 6c65 7279 0a66 726f  QueryGallery.fro
-00003c50: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-00003c60: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00003c70: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
-00003c80: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
-00003c90: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00003ca0: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7574  ctor.from oml.ut
-00003cb0: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
-00003cc0: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
-00003cd0: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
-00003ce0: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
-00003cf0: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
-00003d00: 6173 6574 2f22 0a5f 2c20 6466 5f76 616c  aset/"._, df_val
-00003d10: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-00003d20: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-00003d30: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-00003d40: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-00003d50: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-00003d60: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-00003d70: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00003d80: 733d 4661 6c73 6529 2e65 7661 6c28 290a  s=False).eval().
-00003d90: 0a76 616c 5f64 6174 6173 6574 203d 2044  .val_dataset = D
-00003da0: 6174 6173 6574 5175 6572 7947 616c 6c65  atasetQueryGalle
-00003db0: 7279 2864 665f 7661 6c2c 2064 6174 6173  ry(df_val, datas
-00003dc0: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00003dd0: 726f 6f74 290a 0a76 616c 5f6c 6f61 6465  root)..val_loade
-00003de0: 7220 3d20 746f 7263 682e 7574 696c 732e  r = torch.utils.
-00003df0: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
-00003e00: 7661 6c5f 6461 7461 7365 742c 2062 6174  val_dataset, bat
-00003e10: 6368 5f73 697a 653d 3429 0a63 616c 6375  ch_size=4).calcu
-00003e20: 6c61 746f 7220 3d20 456d 6265 6464 696e  lator = Embeddin
-00003e30: 674d 6574 7269 6373 2865 7874 7261 5f6b  gMetrics(extra_k
-00003e40: 6579 733d 2822 7061 7468 7322 2c29 290a  eys=("paths",)).
-00003e50: 6361 6c63 756c 6174 6f72 2e73 6574 7570  calculator.setup
-00003e60: 286e 756d 5f73 616d 706c 6573 3d6c 656e  (num_samples=len
-00003e70: 2876 616c 5f64 6174 6173 6574 2929 0a0a  (val_dataset))..
-00003e80: 7769 7468 2074 6f72 6368 2e6e 6f5f 6772  with torch.no_gr
-00003e90: 6164 2829 3a0a 2020 2020 666f 7220 6261  ad():.    for ba
-00003ea0: 7463 6820 696e 2074 7164 6d28 7661 6c5f  tch in tqdm(val_
-00003eb0: 6c6f 6164 6572 293a 0a20 2020 2020 2020  loader):.       
-00003ec0: 2062 6174 6368 5b22 656d 6265 6464 696e   batch["embeddin
-00003ed0: 6773 225d 203d 2065 7874 7261 6374 6f72  gs"] = extractor
-00003ee0: 2862 6174 6368 5b22 696e 7075 745f 7465  (batch["input_te
-00003ef0: 6e73 6f72 7322 5d29 0a20 2020 2020 2020  nsors"]).       
-00003f00: 2063 616c 6375 6c61 746f 722e 7570 6461   calculator.upda
-00003f10: 7465 5f64 6174 6128 6261 7463 6829 0a0a  te_data(batch)..
-00003f20: 6d65 7472 6963 7320 3d20 6361 6c63 756c  metrics = calcul
-00003f30: 6174 6f72 2e63 6f6d 7075 7465 5f6d 6574  ator.compute_met
-00003f40: 7269 6373 2829 0a0a 2320 4c6f 6767 696e  rics()..# Loggin
-00003f50: 670a 7072 696e 7428 6361 6c63 756c 6174  g.print(calculat
-00003f60: 6f72 2e6d 6574 7269 6373 2920 2023 206d  or.metrics)  # m
-00003f70: 6574 7269 6373 0a70 7269 6e74 2863 616c  etrics.print(cal
-00003f80: 6375 6c61 746f 722e 6d65 7472 6963 735f  culator.metrics_
-00003f90: 756e 7265 6475 6365 6429 2020 2320 6d65  unreduced)  # me
-00003fa0: 7472 6963 7320 7769 7468 6f75 7420 6176  trics without av
-00003fb0: 6572 6167 696e 6720 6f76 6572 2071 7565  eraging over que
-00003fc0: 7269 6573 0a0a 2320 5669 7375 616c 6973  ries..# Visualis
-00003fd0: 6174 696f 6e0a 6361 6c63 756c 6174 6f72  ation.calculator
-00003fe0: 2e67 6574 5f70 6c6f 745f 666f 725f 7175  .get_plot_for_qu
-00003ff0: 6572 6965 7328 7175 6572 795f 6964 733d  eries(query_ids=
-00004000: 5b30 2c20 325d 2c20 6e5f 696e 7374 616e  [0, 2], n_instan
-00004010: 6365 733d 3529 2020 2320 6472 6177 2070  ces=5)  # draw p
-00004020: 7265 6469 6374 696f 6e73 206f 6e20 7072  redictions on pr
-00004030: 6564 6566 696e 6564 2071 7565 7269 6573  edefined queries
-00004040: 0a63 616c 6375 6c61 746f 722e 6765 745f  .calculator.get_
-00004050: 706c 6f74 5f66 6f72 5f77 6f72 7374 5f71  plot_for_worst_q
-00004060: 7565 7269 6573 286d 6574 7269 635f 6e61  ueries(metric_na
-00004070: 6d65 3d22 4f56 4552 414c 4c2f 6d61 702f  me="OVERALL/map/
-00004080: 3522 2c20 6e5f 7175 6572 6965 733d 322c  5", n_queries=2,
-00004090: 206e 5f69 6e73 7461 6e63 6573 3d35 2920   n_instances=5) 
-000040a0: 2023 2064 7261 7720 6d69 7374 616b 6573   # draw mistakes
-000040b0: 0a63 616c 6375 6c61 746f 722e 7669 7375  .calculator.visu
-000040c0: 616c 697a 6528 2920 2023 2064 7261 7720  alize()  # draw 
-000040d0: 6d69 7374 616b 6573 2066 6f72 2061 6c6c  mistakes for all
-000040e0: 2074 6865 2061 7661 696c 6162 6c65 206d   the available m
-000040f0: 6574 7269 6373 0a0a 6060 600a 5b63 6f6d  etrics..```.[com
-00004100: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
-00004110: 6c69 6461 7469 6f6e 2d65 6e64 0a3c 2f70  lidation-end.</p
-00004120: 3e0a 3c2f 6465 7461 696c 733e 0a0a 5b21  >.</details>..[!
-00004130: 5b4f 7065 6e20 496e 2043 6f6c 6162 5d28  [Open In Colab](
-00004140: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00004150: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00004160: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
-00004170: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00004180: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00004190: 682e 676f 6f67 6c65 2e63 6f6d 2f64 7269  h.google.com/dri
-000041a0: 7665 2f31 4f32 6f33 6b38 4938 6a4e 3568  ve/1O2o3k8I8jN5h
-000041b0: 5269 6e33 644b 6e41 5333 5773 6747 3034  Rin3dKnAS3WsgG04
-000041c0: 746d 4954 3f75 7370 3d73 6861 7269 6e67  tmIT?usp=sharing
-000041d0: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
-000041e0: 6d61 7279 3e54 7261 696e 696e 6720 2b20  mary>Training + 
-000041f0: 5661 6c69 6461 7469 6f6e 205b 4c69 6768  Validation [Ligh
-00004200: 746e 696e 6720 616e 6420 4e65 7074 756e  tning and Neptun
-00004210: 6520 6c6f 6767 696e 675d 3c2f 7375 6d6d  e logging]</summ
-00004220: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-00004230: 6e74 5d3a 6c69 6768 746e 696e 672d 7374  nt]:lightning-st
-00004240: 6172 740a 6060 6070 7974 686f 6e0a 696d  art.```python.im
-00004250: 706f 7274 2070 7974 6f72 6368 5f6c 6967  port pytorch_lig
-00004260: 6874 6e69 6e67 2061 7320 706c 0a69 6d70  htning as pl.imp
-00004270: 6f72 7420 746f 7263 680a 0a66 726f 6d20  ort torch..from 
-00004280: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-00004290: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-000042a0: 5175 6572 7947 616c 6c65 7279 2c20 4461  QueryGallery, Da
-000042b0: 7461 7365 7457 6974 684c 6162 656c 730a  tasetWithLabels.
-000042c0: 6672 6f6d 206f 6d6c 2e6c 6967 6874 6e69  from oml.lightni
-000042d0: 6e67 2e6d 6f64 756c 6573 2e65 7874 7261  ng.modules.extra
-000042e0: 6374 6f72 2069 6d70 6f72 7420 4578 7472  ctor import Extr
-000042f0: 6163 746f 724d 6f64 756c 650a 6672 6f6d  actorModule.from
-00004300: 206f 6d6c 2e6c 6967 6874 6e69 6e67 2e63   oml.lightning.c
-00004310: 616c 6c62 6163 6b73 2e6d 6574 7269 6320  allbacks.metric 
-00004320: 696d 706f 7274 204d 6574 7269 6356 616c  import MetricVal
-00004330: 4361 6c6c 6261 636b 0a66 726f 6d20 6f6d  Callback.from om
-00004340: 6c2e 6c6f 7373 6573 2e74 7269 706c 6574  l.losses.triplet
-00004350: 2069 6d70 6f72 7420 5472 6970 6c65 744c   import TripletL
-00004360: 6f73 7357 6974 684d 696e 6572 0a66 726f  ossWithMiner.fro
-00004370: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-00004380: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00004390: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
-000043a0: 0a66 726f 6d20 6f6d 6c2e 6d69 6e65 7273  .from oml.miners
-000043b0: 2e69 6e62 6174 6368 5f61 6c6c 5f74 7269  .inbatch_all_tri
-000043c0: 2069 6d70 6f72 7420 416c 6c54 7269 706c   import AllTripl
-000043d0: 6574 734d 696e 6572 0a66 726f 6d20 6f6d  etsMiner.from om
-000043e0: 6c2e 6d6f 6465 6c73 2069 6d70 6f72 7420  l.models import 
-000043f0: 5669 5445 7874 7261 6374 6f72 0a66 726f  ViTExtractor.fro
-00004400: 6d20 6f6d 6c2e 7361 6d70 6c65 7273 2e62  m oml.samplers.b
-00004410: 616c 616e 6365 2069 6d70 6f72 7420 4261  alance import Ba
-00004420: 6c61 6e63 6553 616d 706c 6572 0a66 726f  lanceSampler.fro
-00004430: 6d20 6f6d 6c2e 7574 696c 732e 646f 776e  m oml.utils.down
-00004440: 6c6f 6164 5f6d 6f63 6b5f 6461 7461 7365  load_mock_datase
-00004450: 7420 696d 706f 7274 2064 6f77 6e6c 6f61  t import downloa
-00004460: 645f 6d6f 636b 5f64 6174 6173 6574 0a66  d_mock_dataset.f
-00004470: 726f 6d20 7079 746f 7263 685f 6c69 6768  rom pytorch_ligh
-00004480: 746e 696e 672e 6c6f 6767 6572 7320 696d  tning.loggers im
-00004490: 706f 7274 204e 6570 7475 6e65 4c6f 6767  port NeptuneLogg
-000044a0: 6572 2c20 5465 6e73 6f72 426f 6172 644c  er, TensorBoardL
-000044b0: 6f67 6765 720a 0a64 6174 6173 6574 5f72  ogger..dataset_r
-000044c0: 6f6f 7420 3d20 226d 6f63 6b5f 6461 7461  oot = "mock_data
-000044d0: 7365 742f 220a 6466 5f74 7261 696e 2c20  set/".df_train, 
-000044e0: 6466 5f76 616c 203d 2064 6f77 6e6c 6f61  df_val = downloa
-000044f0: 645f 6d6f 636b 5f64 6174 6173 6574 2864  d_mock_dataset(d
-00004500: 6174 6173 6574 5f72 6f6f 7429 0a0a 2320  ataset_root)..# 
-00004510: 6d6f 6465 6c0a 6578 7472 6163 746f 7220  model.extractor 
-00004520: 3d20 5669 5445 7874 7261 6374 6f72 2822  = ViTExtractor("
-00004530: 7669 7473 3136 5f64 696e 6f22 2c20 6172  vits16_dino", ar
-00004540: 6368 3d22 7669 7473 3136 222c 206e 6f72  ch="vits16", nor
-00004550: 6d61 6c69 7365 5f66 6561 7475 7265 733d  malise_features=
-00004560: 4661 6c73 6529 0a0a 2320 7472 6169 6e0a  False)..# train.
-00004570: 6f70 7469 6d69 7a65 7220 3d20 746f 7263  optimizer = torc
-00004580: 682e 6f70 7469 6d2e 5347 4428 6578 7472  h.optim.SGD(extr
-00004590: 6163 746f 722e 7061 7261 6d65 7465 7273  actor.parameters
-000045a0: 2829 2c20 6c72 3d31 652d 3629 0a74 7261  (), lr=1e-6).tra
-000045b0: 696e 5f64 6174 6173 6574 203d 2044 6174  in_dataset = Dat
-000045c0: 6173 6574 5769 7468 4c61 6265 6c73 2864  asetWithLabels(d
-000045d0: 665f 7472 6169 6e2c 2064 6174 6173 6574  f_train, dataset
-000045e0: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-000045f0: 6f74 290a 6372 6974 6572 696f 6e20 3d20  ot).criterion = 
-00004600: 5472 6970 6c65 744c 6f73 7357 6974 684d  TripletLossWithM
-00004610: 696e 6572 286d 6172 6769 6e3d 302e 312c  iner(margin=0.1,
-00004620: 206d 696e 6572 3d41 6c6c 5472 6970 6c65   miner=AllTriple
-00004630: 7473 4d69 6e65 7228 2929 0a62 6174 6368  tsMiner()).batch
-00004640: 5f73 616d 706c 6572 203d 2042 616c 616e  _sampler = Balan
-00004650: 6365 5361 6d70 6c65 7228 7472 6169 6e5f  ceSampler(train_
-00004660: 6461 7461 7365 742e 6765 745f 6c61 6265  dataset.get_labe
-00004670: 6c73 2829 2c20 6e5f 6c61 6265 6c73 3d32  ls(), n_labels=2
-00004680: 2c20 6e5f 696e 7374 616e 6365 733d 3329  , n_instances=3)
-00004690: 0a74 7261 696e 5f6c 6f61 6465 7220 3d20  .train_loader = 
-000046a0: 746f 7263 682e 7574 696c 732e 6461 7461  torch.utils.data
-000046b0: 2e44 6174 614c 6f61 6465 7228 7472 6169  .DataLoader(trai
-000046c0: 6e5f 6461 7461 7365 742c 2062 6174 6368  n_dataset, batch
-000046d0: 5f73 616d 706c 6572 3d62 6174 6368 5f73  _sampler=batch_s
-000046e0: 616d 706c 6572 290a 0a23 2076 616c 0a76  ampler)..# val.v
-000046f0: 616c 5f64 6174 6173 6574 203d 2044 6174  al_dataset = Dat
-00004700: 6173 6574 5175 6572 7947 616c 6c65 7279  asetQueryGallery
-00004710: 2864 665f 7661 6c2c 2064 6174 6173 6574  (df_val, dataset
-00004720: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-00004730: 6f74 290a 7661 6c5f 6c6f 6164 6572 203d  ot).val_loader =
-00004740: 2074 6f72 6368 2e75 7469 6c73 2e64 6174   torch.utils.dat
-00004750: 612e 4461 7461 4c6f 6164 6572 2876 616c  a.DataLoader(val
-00004760: 5f64 6174 6173 6574 2c20 6261 7463 685f  _dataset, batch_
-00004770: 7369 7a65 3d34 290a 6d65 7472 6963 5f63  size=4).metric_c
-00004780: 616c 6c62 6163 6b20 3d20 4d65 7472 6963  allback = Metric
-00004790: 5661 6c43 616c 6c62 6163 6b28 6d65 7472  ValCallback(metr
-000047a0: 6963 3d45 6d62 6564 6469 6e67 4d65 7472  ic=EmbeddingMetr
-000047b0: 6963 7328 6578 7472 615f 6b65 7973 3d5b  ics(extra_keys=[
-000047c0: 7472 6169 6e5f 6461 7461 7365 742e 7061  train_dataset.pa
-000047d0: 7468 735f 6b65 792c 5d29 2c20 6c6f 675f  ths_key,]), log_
-000047e0: 696d 6167 6573 3d54 7275 6529 0a0a 2320  images=True)..# 
-000047f0: 6c6f 6767 696e 670a 6c6f 6767 6572 203d  logging.logger =
-00004800: 2054 656e 736f 7242 6f61 7264 4c6f 6767   TensorBoardLogg
-00004810: 6572 2822 2e22 2920 2023 2046 6f72 2054  er(".")  # For T
-00004820: 656e 736f 7242 6f61 7264 0a23 206c 6f67  ensorBoard.# log
-00004830: 6765 7220 3d20 4e65 7074 756e 654c 6f67  ger = NeptuneLog
-00004840: 6765 7228 6170 695f 6b65 793d 2222 2c20  ger(api_key="", 
-00004850: 7072 6f6a 6563 743d 2222 2c20 6c6f 675f  project="", log_
-00004860: 6d6f 6465 6c5f 6368 6563 6b70 6f69 6e74  model_checkpoint
-00004870: 733d 4661 6c73 6529 2020 2320 466f 7220  s=False)  # For 
-00004880: 4e65 7074 756e 650a 0a23 2072 756e 0a70  Neptune..# run.p
-00004890: 6c5f 6d6f 6465 6c20 3d20 4578 7472 6163  l_model = Extrac
-000048a0: 746f 724d 6f64 756c 6528 6578 7472 6163  torModule(extrac
-000048b0: 746f 722c 2063 7269 7465 7269 6f6e 2c20  tor, criterion, 
-000048c0: 6f70 7469 6d69 7a65 7229 0a74 7261 696e  optimizer).train
-000048d0: 6572 203d 2070 6c2e 5472 6169 6e65 7228  er = pl.Trainer(
-000048e0: 6d61 785f 6570 6f63 6873 3d33 2c20 6361  max_epochs=3, ca
-000048f0: 6c6c 6261 636b 733d 5b6d 6574 7269 635f  llbacks=[metric_
-00004900: 6361 6c6c 6261 636b 5d2c 206e 756d 5f73  callback], num_s
-00004910: 616e 6974 795f 7661 6c5f 7374 6570 733d  anity_val_steps=
-00004920: 302c 206c 6f67 6765 723d 6c6f 6767 6572  0, logger=logger
-00004930: 290a 7472 6169 6e65 722e 6669 7428 706c  ).trainer.fit(pl
-00004940: 5f6d 6f64 656c 2c20 7472 6169 6e5f 6461  _model, train_da
-00004950: 7461 6c6f 6164 6572 733d 7472 6169 6e5f  taloaders=train_
-00004960: 6c6f 6164 6572 2c20 7661 6c5f 6461 7461  loader, val_data
-00004970: 6c6f 6164 6572 733d 7661 6c5f 6c6f 6164  loaders=val_load
-00004980: 6572 290a 0a60 6060 0a5b 636f 6d6d 656e  er)..```.[commen
-00004990: 745d 3a6c 6967 6874 6e69 6e67 2d65 6e64  t]:lightning-end
-000049a0: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-000049b0: 0a0a 5b21 5b4f 7065 6e20 496e 2043 6f6c  ..[![Open In Col
-000049c0: 6162 5d28 6874 7470 733a 2f2f 636f 6c61  ab](https://cola
-000049d0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-000049e0: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
-000049f0: 6162 2d62 6164 6765 2e73 7667 295d 2868  ab-badge.svg)](h
-00004a00: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00004a10: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00004a20: 2f64 7269 7665 2f31 6256 5567 6442 4757  /drive/1bVUgdBGW
-00004a30: 7651 6743 6b62 6132 5974 6149 5256 6c55  vQgCkba2YtaIRVlU
-00004a40: 5155 7a37 5136 305a 3f75 7370 3d73 6861  QUz7Q60Z?usp=sha
-00004a50: 7265 5f6c 696e 6b29 0a3c 6465 7461 696c  re_link).<detail
-00004a60: 733e 0a3c 7375 6d6d 6172 793e 5573 696e  s>.<summary>Usin
-00004a70: 6720 6120 7472 6169 6e65 6420 6d6f 6465  g a trained mode
-00004a80: 6c20 666f 7220 7265 7472 6965 7661 6c3c  l for retrieval<
-00004a90: 2f73 756d 6d61 7279 3e0a 3c70 3e0a 0a5b  /summary>.<p>..[
-00004aa0: 636f 6d6d 656e 745d 3a75 7361 6765 2d72  comment]:usage-r
-00004ab0: 6574 7269 6576 616c 2d73 7461 7274 0a60  etrieval-start.`
-00004ac0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00004ad0: 746f 7263 680a 0a66 726f 6d20 6f6d 6c2e  torch..from oml.
-00004ae0: 636f 6e73 7420 696d 706f 7274 204d 4f43  const import MOC
-00004af0: 4b5f 4441 5441 5345 545f 5041 5448 0a66  K_DATASET_PATH.f
-00004b00: 726f 6d20 6f6d 6c2e 696e 6665 7265 6e63  rom oml.inferenc
-00004b10: 652e 666c 6174 2069 6d70 6f72 7420 696e  e.flat import in
-00004b20: 6665 7265 6e63 655f 6f6e 5f69 6d61 6765  ference_on_image
-00004b30: 730a 6672 6f6d 206f 6d6c 2e6d 6f64 656c  s.from oml.model
-00004b40: 7320 696d 706f 7274 2056 6954 4578 7472  s import ViTExtr
-00004b50: 6163 746f 720a 6672 6f6d 206f 6d6c 2e72  actor.from oml.r
-00004b60: 6567 6973 7472 792e 7472 616e 7366 6f72  egistry.transfor
-00004b70: 6d73 2069 6d70 6f72 7420 6765 745f 7472  ms import get_tr
-00004b80: 616e 7366 6f72 6d73 5f66 6f72 5f70 7265  ansforms_for_pre
-00004b90: 7472 6169 6e65 640a 6672 6f6d 206f 6d6c  trained.from oml
-00004ba0: 2e75 7469 6c73 2e64 6f77 6e6c 6f61 645f  .utils.download_
-00004bb0: 6d6f 636b 5f64 6174 6173 6574 2069 6d70  mock_dataset imp
-00004bc0: 6f72 7420 646f 776e 6c6f 6164 5f6d 6f63  ort download_moc
-00004bd0: 6b5f 6461 7461 7365 740a 6672 6f6d 206f  k_dataset.from o
-00004be0: 6d6c 2e75 7469 6c73 2e6d 6973 635f 746f  ml.utils.misc_to
-00004bf0: 7263 6820 696d 706f 7274 2070 6169 7277  rch import pairw
-00004c00: 6973 655f 6469 7374 0a0a 5f2c 2064 665f  ise_dist.._, df_
-00004c10: 7661 6c20 3d20 646f 776e 6c6f 6164 5f6d  val = download_m
-00004c20: 6f63 6b5f 6461 7461 7365 7428 4d4f 434b  ock_dataset(MOCK
-00004c30: 5f44 4154 4153 4554 5f50 4154 4829 0a64  _DATASET_PATH).d
-00004c40: 665f 7661 6c5b 2270 6174 6822 5d20 3d20  f_val["path"] = 
-00004c50: 6466 5f76 616c 5b22 7061 7468 225d 2e61  df_val["path"].a
-00004c60: 7070 6c79 286c 616d 6264 6120 783a 204d  pply(lambda x: M
-00004c70: 4f43 4b5f 4441 5441 5345 545f 5041 5448  OCK_DATASET_PATH
-00004c80: 202f 2078 290a 7175 6572 6965 7320 3d20   / x).queries = 
-00004c90: 6466 5f76 616c 5b64 665f 7661 6c5b 2269  df_val[df_val["i
-00004ca0: 735f 7175 6572 7922 5d5d 5b22 7061 7468  s_query"]]["path
-00004cb0: 225d 2e74 6f6c 6973 7428 290a 6761 6c6c  "].tolist().gall
-00004cc0: 6572 6965 7320 3d20 6466 5f76 616c 5b64  eries = df_val[d
-00004cd0: 665f 7661 6c5b 2269 735f 6761 6c6c 6572  f_val["is_galler
-00004ce0: 7922 5d5d 5b22 7061 7468 225d 2e74 6f6c  y"]]["path"].tol
-00004cf0: 6973 7428 290a 0a65 7874 7261 6374 6f72  ist()..extractor
-00004d00: 203d 2056 6954 4578 7472 6163 746f 722e   = ViTExtractor.
-00004d10: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00004d20: 2276 6974 7331 365f 6469 6e6f 2229 0a74  "vits16_dino").t
-00004d30: 7261 6e73 666f 726d 2c20 5f20 3d20 6765  ransform, _ = ge
-00004d40: 745f 7472 616e 7366 6f72 6d73 5f66 6f72  t_transforms_for
-00004d50: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-00004d60: 7331 365f 6469 6e6f 2229 0a0a 6172 6773  s16_dino")..args
-00004d70: 203d 207b 226e 756d 5f77 6f72 6b65 7273   = {"num_workers
-00004d80: 223a 2030 2c20 2262 6174 6368 5f73 697a  ": 0, "batch_siz
-00004d90: 6522 3a20 387d 0a66 6561 7475 7265 735f  e": 8}.features_
-00004da0: 7175 6572 6965 7320 3d20 696e 6665 7265  queries = infere
-00004db0: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-00004dc0: 7472 6163 746f 722c 2070 6174 6873 3d71  tractor, paths=q
-00004dd0: 7565 7269 6573 2c20 7472 616e 7366 6f72  ueries, transfor
-00004de0: 6d3d 7472 616e 7366 6f72 6d2c 202a 2a61  m=transform, **a
-00004df0: 7267 7329 0a66 6561 7475 7265 735f 6761  rgs).features_ga
-00004e00: 6c6c 6572 6965 7320 3d20 696e 6665 7265  lleries = infere
-00004e10: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-00004e20: 7472 6163 746f 722c 2070 6174 6873 3d67  tractor, paths=g
-00004e30: 616c 6c65 7269 6573 2c20 7472 616e 7366  alleries, transf
-00004e40: 6f72 6d3d 7472 616e 7366 6f72 6d2c 202a  orm=transform, *
-00004e50: 2a61 7267 7329 0a0a 2320 4e6f 7720 7765  *args)..# Now we
-00004e60: 2063 616e 2065 7870 6c69 6369 746c 7920   can explicitly 
-00004e70: 6275 696c 6420 7061 6972 7769 7365 206d  build pairwise m
-00004e80: 6174 7269 7820 6f66 2064 6973 7461 6e63  atrix of distanc
-00004e90: 6573 206f 7220 7361 7665 2079 6f75 2052  es or save you R
-00004ea0: 414d 2076 6961 2075 7369 6e67 206b 4e4e  AM via using kNN
-00004eb0: 0a75 7365 5f6b 6e6e 203d 2054 7275 650a  .use_knn = True.
-00004ec0: 746f 705f 6b20 3d20 330a 0a69 6620 7573  top_k = 3..if us
-00004ed0: 655f 6b6e 6e3a 0a20 2020 2066 726f 6d20  e_knn:.    from 
-00004ee0: 736b 6c65 6172 6e2e 6e65 6967 6862 6f72  sklearn.neighbor
-00004ef0: 7320 696d 706f 7274 204e 6561 7265 7374  s import Nearest
-00004f00: 4e65 6967 6862 6f72 730a 2020 2020 6b6e  Neighbors.    kn
-00004f10: 6e20 3d20 4e65 6172 6573 744e 6569 6768  n = NearestNeigh
-00004f20: 626f 7273 2861 6c67 6f72 6974 686d 3d22  bors(algorithm="
-00004f30: 6175 746f 222c 2070 3d32 290a 2020 2020  auto", p=2).    
-00004f40: 6b6e 6e2e 6669 7428 6665 6174 7572 6573  knn.fit(features
-00004f50: 5f67 616c 6c65 7269 6573 290a 2020 2020  _galleries).    
-00004f60: 6469 7374 732c 2069 695f 636c 6f73 6573  dists, ii_closes
-00004f70: 7420 3d20 6b6e 6e2e 6b6e 6569 6768 626f  t = knn.kneighbo
-00004f80: 7273 2866 6561 7475 7265 735f 7175 6572  rs(features_quer
-00004f90: 6965 732c 206e 5f6e 6569 6768 626f 7273  ies, n_neighbors
-00004fa0: 3d74 6f70 5f6b 2c20 7265 7475 726e 5f64  =top_k, return_d
-00004fb0: 6973 7461 6e63 653d 5472 7565 290a 0a65  istance=True)..e
-00004fc0: 6c73 653a 0a20 2020 2064 6973 745f 6d61  lse:.    dist_ma
-00004fd0: 7420 3d20 7061 6972 7769 7365 5f64 6973  t = pairwise_dis
-00004fe0: 7428 7831 3d66 6561 7475 7265 735f 7175  t(x1=features_qu
-00004ff0: 6572 6965 732c 2078 323d 6665 6174 7572  eries, x2=featur
-00005000: 6573 5f67 616c 6c65 7269 6573 290a 2020  es_galleries).  
-00005010: 2020 6469 7374 732c 2069 695f 636c 6f73    dists, ii_clos
-00005020: 6573 7420 3d20 746f 7263 682e 746f 706b  est = torch.topk
-00005030: 2864 6973 745f 6d61 742c 2064 696d 3d31  (dist_mat, dim=1
-00005040: 2c20 6b3d 746f 705f 6b2c 206c 6172 6765  , k=top_k, large
-00005050: 7374 3d46 616c 7365 290a 0a70 7269 6e74  st=False)..print
-00005060: 2866 2254 6f70 207b 746f 705f 6b7d 2069  (f"Top {top_k} i
-00005070: 7465 6d73 2063 6c6f 7365 7374 2074 6f20  tems closest to 
-00005080: 7175 6572 6965 7320 6172 653a 5c6e 207b  queries are:\n {
-00005090: 6969 5f63 6c6f 7365 7374 7d22 290a 6060  ii_closest}").``
-000050a0: 600a 5b63 6f6d 6d65 6e74 5d3a 7573 6167  `.[comment]:usag
-000050b0: 652d 7265 7472 6965 7661 6c2d 656e 640a  e-retrieval-end.
-000050c0: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
-000050d0: 0a5b 215b 4f70 656e 2049 6e20 436f 6c61  .[![Open In Cola
-000050e0: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
-000050f0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00005100: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
-00005110: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
-00005120: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-00005130: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-00005140: 6472 6976 652f 3153 326e 4b36 4b61 5265  drive/1S2nK6KaRe
-00005150: 446d 2d52 6a6a 646f 6a64 4964 3643 616b  Dm-RjjdojdId6Cak
-00005160: 6868 5379 7666 413f 7573 703d 7368 6172  hhSyvfA?usp=shar
-00005170: 655f 6c69 6e6b 290a 0a5b 2a2a 5363 6865  e_link)..[**Sche
-00005180: 6d61 732c 2065 7870 6c61 6e61 7469 6f6e  mas, explanation
-00005190: 7320 616e 6420 7469 7073 2a2a 5d28 6874  s and tips**](ht
-000051a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000051b0: 2f4f 4d4c 2d54 6561 6d2f 6f70 656e 2d6d  /OML-Team/open-m
-000051c0: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
-000051d0: 7265 652f 6d61 696e 2f70 6970 656c 696e  ree/main/pipelin
-000051e0: 6573 2f66 6561 7475 7265 735f 6578 7472  es/features_extr
-000051f0: 6163 7469 6f6e 290a 0a53 6565 205b 6578  action)..See [ex
-00005200: 7472 6120 636f 6465 2073 6e69 7070 6574  tra code snippet
-00005210: 735d 2868 7474 7073 3a2f 2f6f 7065 6e2d  s](https://open-
-00005220: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-00005230: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00005240: 6e2f 6c61 7465 7374 2f66 6561 7475 7265  n/latest/feature
-00005250: 5f65 7874 7261 6374 696f 6e2f 7079 7468  _extraction/pyth
-00005260: 6f6e 5f65 7861 6d70 6c65 732e 6874 6d6c  on_examples.html
-00005270: 292c 2069 6e63 6c75 6469 6e67 3a0a 2a20  ), including:.* 
-00005280: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
-00005290: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
-000052a0: 6e69 6e67 0a2a 2054 7261 696e 696e 6720  ning.* Training 
-000052b0: 2b20 5661 6c69 6461 7469 6f6e 2077 6974  + Validation wit
-000052c0: 6820 4c69 6768 746e 696e 6720 696e 2044  h Lightning in D
-000052d0: 4450 206d 6f64 650a 2a20 5472 6169 6e69  DP mode.* Traini
-000052e0: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-000052f0: 726f 6d20 504d 4c0a 2a20 5472 6169 6e69  rom PML.* Traini
-00005300: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-00005310: 726f 6d20 504d 4c20 6164 7661 6e63 6564  rom PML advanced
-00005320: 2028 7061 7373 696e 6720 6469 7374 616e   (passing distan
-00005330: 6365 2c20 7265 6475 6365 722c 206d 696e  ce, reducer, min
-00005340: 6572 290a 0a23 2320 5b50 6970 656c 696e  er)..## [Pipelin
-00005350: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00005360: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00005370: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00005380: 6e69 6e67 2f74 7265 652f 6d61 696e 2f70  ning/tree/main/p
-00005390: 6970 656c 696e 6573 290a 0a50 6970 656c  ipelines)..Pipel
-000053a0: 696e 6573 2070 726f 7669 6465 2061 2077  ines provide a w
-000053b0: 6179 2074 6f20 7275 6e20 6d65 7472 6963  ay to run metric
-000053c0: 206c 6561 726e 696e 6720 6578 7065 7269   learning experi
-000053d0: 6d65 6e74 7320 7669 6120 6368 616e 6769  ments via changi
-000053e0: 6e67 206f 6e6c 7920 7468 6520 636f 6e66  ng only the conf
-000053f0: 6967 2066 696c 652e 0a41 6c6c 2079 6f75  ig file..All you
-00005400: 206e 6565 6420 6973 2074 6f20 7072 6570   need is to prep
-00005410: 6172 6520 796f 7572 2064 6174 6173 6574  are your dataset
-00005420: 2069 6e20 6120 7265 7175 6972 6564 2066   in a required f
-00005430: 6f72 6d61 742e 0a0a 5365 6520 5b50 6970  ormat...See [Pip
-00005440: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00005450: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-00005460: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00005470: 6c65 6172 6e69 6e67 2f62 6c6f 622f 6d61  learning/blob/ma
-00005480: 696e 2f70 6970 656c 696e 6573 2f29 2066  in/pipelines/) f
-00005490: 6f6c 6465 7220 666f 7220 6d6f 7265 2064  older for more d
-000054a0: 6574 6169 6c73 3a0a 2a20 4665 6174 7572  etails:.* Featur
-000054b0: 6520 6578 7472 6163 746f 7220 5b70 6970  e extractor [pip
-000054c0: 656c 696e 655d 2868 7474 7073 3a2f 2f67  eline](https://g
-000054d0: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-000054e0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-000054f0: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
-00005500: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
-00005510: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
-00005520: 0a2a 2052 6574 7269 6576 616c 2070 6f73  .* Retrieval pos
-00005530: 7470 726f 6365 7373 6f72 205b 7069 7065  tprocessor [pipe
-00005540: 6c69 6e65 5d28 6874 7470 733a 2f2f 6769  line](https://gi
-00005550: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
-00005560: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
-00005570: 6172 6e69 6e67 2f74 7265 652f 6d61 696e  arning/tree/main
-00005580: 2f70 6970 656c 696e 6573 2f70 6f73 7470  /pipelines/postp
-00005590: 726f 6365 7373 696e 6729 2028 7265 2d72  rocessing) (re-r
-000055a0: 616e 6b69 6e67 290a 0a23 2320 5b5a 6f6f  anking)..## [Zoo
-000055b0: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-000055c0: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-000055d0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000055e0: 2f6c 6174 6573 742f 6665 6174 7572 655f  /latest/feature_
-000055f0: 6578 7472 6163 7469 6f6e 2f7a 6f6f 2e68  extraction/zoo.h
-00005600: 746d 6c29 0a0a 4265 6c6f 7720 6172 6520  tml)..Below are 
-00005610: 7468 6520 6d6f 6465 6c73 2074 7261 696e  the models train
-00005620: 6564 2077 6974 6820 4f4d 4c20 6f6e 2034  ed with OML on 4
-00005630: 2070 7562 6c69 6320 6461 7461 7365 7473   public datasets
-00005640: 2e0a 416c 6c20 6d65 7472 6963 7320 6265  ..All metrics be
-00005650: 6c6f 7720 7765 7265 206f 6274 6169 6e65  low were obtaine
-00005660: 6420 6f6e 2074 6865 2069 6d61 6765 7320  d on the images 
-00005670: 7769 7468 2074 6865 2073 697a 6573 206f  with the sizes o
-00005680: 6620 2a2a 3232 3420 7820 3232 342a 2a3a  f **224 x 224**:
-00005690: 0a0a 7c20 2020 2020 2020 2020 2020 2020  ..|             
-000056a0: 2020 2020 2020 2020 206d 6f64 656c 2020           model  
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056c0: 2020 2020 7c20 636d 6331 2020 7c20 2020      | cmc1  |   
-000056d0: 2020 2020 2020 6461 7461 7365 7420 2020        dataset   
-000056e0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 2020 7765 6967 6874 7320 2020        weights   
-00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 6578 7065 7269 6d65 6e74 2020 2020 2020  experiment      
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000057c0: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
-000057d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000057f0: 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 3a2d 2d2d  --:|:-----:|:---
-00005800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005810: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00005820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005870: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
-00005880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000058e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
-000058f0: 7c20 6056 6954 4578 7472 6163 746f 722e  | `ViTExtractor.
-00005900: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005910: 2276 6974 7331 365f 696e 7368 6f70 2229  "vits16_inshop")
-00005920: 6020 7c20 302e 3932 3120 7c20 2020 2044  ` | 0.921 |    D
-00005930: 6565 7046 6173 6869 6f6e 2049 6e73 686f  eepFashion Insho
-00005940: 7020 2020 207c 2020 2020 5b6c 696e 6b5d  p    |    [link]
-00005950: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00005960: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
-00005970: 2f31 6e69 582d 5443 3863 6a36 6a33 3639  /1niX-TC8cj6j369
-00005980: 7437 6955 3262 6148 5153 564e 334d 564a  t7iU2baHQSVN3MVJ
-00005990: 6257 2f76 6965 773f 7573 703d 7368 6172  bW/view?usp=shar
-000059a0: 696e 6729 2020 2020 207c 205b 6c69 6e6b  ing)     | [link
-000059b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000059c0: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-000059d0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000059e0: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-000059f0: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-00005a00: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-00005a10: 6374 6f72 5f69 6e73 686f 7029 207c 0a7c  ctor_inshop) |.|
-00005a20: 2020 6056 6954 4578 7472 6163 746f 722e    `ViTExtractor.
-00005a30: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005a40: 2276 6974 7331 365f 736f 7022 2960 2020  "vits16_sop")`  
-00005a50: 207c 2030 2e38 3636 207c 2053 7461 6e66   | 0.866 | Stanf
-00005a60: 6f72 6420 4f6e 6c69 6e65 2050 726f 6475  ord Online Produ
-00005a70: 6374 7320 7c20 2020 5b6c 696e 6b5d 2868  cts |   [link](h
-00005a80: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-00005a90: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
-00005aa0: 7a75 4752 4876 4632 4b48 6435 3961 7737  zuGRHvF2KHd59aw7
-00005ab0: 6937 3336 374f 485f 7451 4e4f 477a 3741  i7367OH_tQNOGz7A
-00005ac0: 2f76 6965 773f 7573 703d 7368 6172 696e  /view?usp=sharin
-00005ad0: 6729 2020 2020 2020 7c20 205b 6c69 6e6b  g)      |  [link
-00005ae0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005af0: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00005b00: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00005b10: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-00005b20: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-00005b30: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-00005b40: 6374 6f72 5f73 6f70 2920 2020 7c0a 7c20  ctor_sop)   |.| 
-00005b50: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00005b60: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00005b70: 6974 7331 365f 6361 7273 2229 6020 2020  its16_cars")`   
-00005b80: 7c20 302e 3930 3720 7c20 2020 2020 2020  | 0.907 |       
-00005b90: 2020 4341 5253 2031 3936 2020 2020 2020    CARS 196      
-00005ba0: 2020 207c 2020 205b 6c69 6e6b 5d28 6874     |   [link](ht
-00005bb0: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00005bc0: 6c65 2e63 6f6d 2f64 7269 7665 2f66 6f6c  le.com/drive/fol
-00005bd0: 6465 7273 2f31 3761 345f 6667 3934 646f  ders/17a4_fg94do
-00005be0: 7832 7366 6b58 6d77 2d4b 4374 694c 426c  x2sfkXmw-KCtiLBl
-00005bf0: 782d 7574 2d31 3f75 7370 3d73 6861 7269  x-ut-1?usp=shari
-00005c00: 6e67 2920 2020 207c 2020 5b6c 696e 6b5d  ng)    |  [link]
-00005c10: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00005c20: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
-00005c30: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-00005c40: 672f 7472 6565 2f6d 6169 6e2f 7069 7065  g/tree/main/pipe
-00005c50: 6c69 6e65 732f 6665 6174 7572 6573 5f65  lines/features_e
-00005c60: 7874 7261 6374 696f 6e2f 6578 7472 6163  xtraction/extrac
-00005c70: 746f 725f 6361 7273 2920 207c 0a7c 2020  tor_cars)  |.|  
-00005c80: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00005c90: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00005ca0: 6974 7331 365f 6375 6222 2960 2020 207c  its16_cub")`   |
-00005cb0: 2030 2e38 3337 207c 2020 2020 2020 2043   0.837 |       C
-00005cc0: 5542 2032 3030 2032 3031 3120 2020 2020  UB 200 2011     
-00005cd0: 2020 7c20 2020 5b6c 696e 6b5d 2868 7474    |   [link](htt
-00005ce0: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
-00005cf0: 652e 636f 6d2f 6472 6976 652f 666f 6c64  e.com/drive/fold
-00005d00: 6572 732f 3154 5043 4e2d 655a 464c 716f  ers/1TPCN-eZFLqo
-00005d10: 7134 4a42 676e 4966 6c69 4a6f 454b 3438  q4JBgnIfliJoEK48
-00005d20: 7839 6f7a 623f 7573 703d 7368 6172 696e  x9ozb?usp=sharin
-00005d30: 6729 2020 2020 7c20 205b 6c69 6e6b 5d28  g)    |  [link](
-00005d40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00005d50: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
-00005d60: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00005d70: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
-00005d80: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
-00005d90: 7472 6163 7469 6f6e 2f65 7874 7261 6374  traction/extract
-00005da0: 6f72 5f63 7562 2920 2020 7c0a 0a57 6520  or_cub)   |..We 
-00005db0: 616c 736f 2070 726f 7669 6465 2061 6e20  also provide an 
-00005dc0: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
-00005dd0: 2074 6865 206d 6f64 656c 7320 7072 6574   the models pret
-00005de0: 7261 696e 6564 2062 7920 6f74 6865 7220  rained by other 
-00005df0: 7265 7365 6172 6368 6572 732e 0a41 6c6c  researchers..All
-00005e00: 206d 6574 7269 6373 2062 656c 6f77 2077   metrics below w
-00005e10: 6572 6520 6f62 7461 696e 6564 206f 6e20  ere obtained on 
-00005e20: 7468 6520 696d 6167 6573 2077 6974 6820  the images with 
-00005e30: 7468 6520 7369 7a65 7320 6f66 202a 2a32  the sizes of **2
-00005e40: 3234 2078 2032 3234 2a2a 3a0a 0a7c 2020  24 x 224**:..|  
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e80: 2020 2020 2020 2020 2020 2020 7c20 5374              | St
-00005e90: 616e 666f 7264 204f 6e6c 696e 6520 5072  anford Online Pr
-00005ea0: 6f64 7563 7473 207c 2044 6565 7046 6173  oducts | DeepFas
-00005eb0: 6869 6f6e 2049 6e53 686f 7020 7c20 4355  hion InShop | CU
-00005ec0: 4220 3230 3020 3230 3131 207c 2043 4152  B 200 2011 | CAR
-00005ed0: 5320 3139 3620 7c0a 7c3a 2d2d 2d2d 2d2d  S 196 |.|:------
-00005ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f10: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00005f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f30: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-00005f40: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-00005f50: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00005f60: 3a7c 0a7c 2020 2020 6056 6954 556e 6963  :|.|    `ViTUnic
-00005f70: 6f6d 4578 7472 6163 746f 722e 6672 6f6d  omExtractor.from
-00005f80: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-00005f90: 6231 365f 756e 6963 6f6d 2229 6020 2020  b16_unicom")`   
-00005fa0: 2020 7c20 2020 2020 2020 2020 2030 2e37    |          0.7
-00005fb0: 3030 2020 2020 2020 2020 2020 207c 2020  00           |  
-00005fc0: 2020 2020 2030 2e37 3334 2020 2020 2020       0.734      
-00005fd0: 2020 7c20 2020 2030 2e38 3437 2020 2020    |    0.847    
-00005fe0: 207c 2020 302e 3931 3620 2020 7c0a 7c20   |  0.916   |.| 
-00005ff0: 2020 2060 5669 5455 6e69 636f 6d45 7874     `ViTUnicomExt
-00006000: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
-00006010: 7261 696e 6564 2822 7669 7462 3332 5f75  rained("vitb32_u
-00006020: 6e69 636f 6d22 2960 2020 2020 207c 2020  nicom")`     |  
-00006030: 2020 2020 2020 2020 302e 3639 3020 2020          0.690   
-00006040: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00006050: 302e 3732 3220 2020 2020 2020 207c 2020  0.722        |  
-00006060: 2020 302e 3739 3620 2020 2020 7c20 2030    0.796     |  0
-00006070: 2e38 3933 2020 207c 0a7c 2020 2020 6056  .893   |.|    `V
-00006080: 6954 556e 6963 6f6d 4578 7472 6163 746f  iTUnicomExtracto
-00006090: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-000060a0: 6428 2276 6974 6c31 345f 756e 6963 6f6d  d("vitl14_unicom
-000060b0: 2229 6020 2020 2020 7c20 2020 2020 2020  ")`     |       
-000060c0: 2020 2030 2e37 3236 2020 2020 2020 2020     0.726        
-000060d0: 2020 207c 2020 2020 2020 2030 2e37 3930     |       0.790
-000060e0: 2020 2020 2020 2020 7c20 2020 2030 2e38          |    0.8
-000060f0: 3638 2020 2020 207c 2020 302e 3932 3220  68     |  0.922 
-00006100: 2020 7c0a 7c20 6056 6954 556e 6963 6f6d    |.| `ViTUnicom
-00006110: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-00006120: 7265 7472 6169 6e65 6428 2276 6974 6c31  retrained("vitl1
-00006130: 345f 3333 3670 785f 756e 6963 6f6d 2229  4_336px_unicom")
-00006140: 6020 207c 2020 2020 2020 2020 2020 302e  `  |          0.
-00006150: 3734 3520 2020 2020 2020 2020 2020 7c20  745           | 
-00006160: 2020 2020 2020 302e 3831 3020 2020 2020        0.810     
-00006170: 2020 207c 2020 2020 302e 3837 3520 2020     |    0.875   
-00006180: 2020 7c20 2030 2e39 3234 2020 207c 0a7c    |  0.924   |.|
-00006190: 2020 2020 6056 6954 434c 4950 4578 7472      `ViTCLIPExtr
-000061a0: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-000061b0: 6169 6e65 6428 2273 6265 725f 7669 7462  ained("sber_vitb
-000061c0: 3332 5f32 3234 2229 6020 2020 2020 7c20  32_224")`     | 
-000061d0: 2020 2020 2020 2020 2030 2e35 3437 2020           0.547  
-000061e0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000061f0: 2030 2e35 3134 2020 2020 2020 2020 7c20   0.514        | 
-00006200: 2020 2030 2e34 3438 2020 2020 207c 2020     0.448     |  
-00006210: 302e 3631 3820 2020 7c0a 7c20 2020 2060  0.618   |.|    `
-00006220: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-00006230: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-00006240: 2822 7362 6572 5f76 6974 6231 365f 3232  ("sber_vitb16_22
-00006250: 3422 2960 2020 2020 207c 2020 2020 2020  4")`     |      
-00006260: 2020 2020 302e 3536 3520 2020 2020 2020      0.565       
-00006270: 2020 2020 7c20 2020 2020 2020 302e 3536      |       0.56
-00006280: 3520 2020 2020 2020 207c 2020 2020 302e  5        |    0.
-00006290: 3532 3420 2020 2020 7c20 2030 2e36 3438  524     |  0.648
-000062a0: 2020 207c 0a7c 2020 2020 6056 6954 434c     |.|    `ViTCL
-000062b0: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-000062c0: 5f70 7265 7472 6169 6e65 6428 2273 6265  _pretrained("sbe
-000062d0: 725f 7669 746c 3134 5f32 3234 2229 6020  r_vitl14_224")` 
-000062e0: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
-000062f0: 2e35 3132 2020 2020 2020 2020 2020 207c  .512           |
-00006300: 2020 2020 2020 2030 2e35 3535 2020 2020         0.555    
-00006310: 2020 2020 7c20 2020 2030 2e36 3036 2020      |    0.606  
-00006320: 2020 207c 2020 302e 3730 3720 2020 7c0a     |  0.707   |.
-00006330: 7c20 2020 6056 6954 434c 4950 4578 7472  |   `ViTCLIPExtr
-00006340: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-00006350: 6169 6e65 6428 226f 7065 6e61 695f 7669  ained("openai_vi
-00006360: 7462 3332 5f32 3234 2229 6020 2020 207c  tb32_224")`    |
-00006370: 2020 2020 2020 2020 2020 302e 3631 3220            0.612 
-00006380: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00006390: 2020 302e 3439 3120 2020 2020 2020 207c    0.491        |
-000063a0: 2020 2020 302e 3536 3020 2020 2020 7c20      0.560     | 
-000063b0: 2030 2e36 3933 2020 207c 0a7c 2020 2060   0.693   |.|   `
-000063c0: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-000063d0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-000063e0: 2822 6f70 656e 6169 5f76 6974 6231 365f  ("openai_vitb16_
-000063f0: 3232 3422 2960 2020 2020 7c20 2020 2020  224")`    |     
-00006400: 2020 2020 2030 2e36 3438 2020 2020 2020       0.648      
-00006410: 2020 2020 207c 2020 2020 2020 2030 2e36       |       0.6
-00006420: 3036 2020 2020 2020 2020 7c20 2020 2030  06        |    0
-00006430: 2e36 3635 2020 2020 207c 2020 302e 3736  .665     |  0.76
-00006440: 3720 2020 7c0a 7c20 2020 6056 6954 434c  7   |.|   `ViTCL
-00006450: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-00006460: 5f70 7265 7472 6169 6e65 6428 226f 7065  _pretrained("ope
-00006470: 6e61 695f 7669 746c 3134 5f32 3234 2229  nai_vitl14_224")
-00006480: 6020 2020 207c 2020 2020 2020 2020 2020  `    |          
-00006490: 302e 3637 3020 2020 2020 2020 2020 2020  0.670           
-000064a0: 7c20 2020 2020 2020 302e 3637 3520 2020  |       0.675   
-000064b0: 2020 2020 207c 2020 2020 302e 3734 3520       |    0.745 
-000064c0: 2020 2020 7c20 2030 2e38 3434 2020 207c      |  0.844   |
-000064d0: 0a7c 2020 2020 2020 2020 6056 6954 4578  .|        `ViTEx
-000064e0: 7472 6163 746f 722e 6672 6f6d 5f70 7265  tractor.from_pre
-000064f0: 7472 6169 6e65 6428 2276 6974 7331 365f  trained("vits16_
-00006500: 6469 6e6f 2229 6020 2020 2020 2020 2020  dino")`         
-00006510: 7c20 2020 2020 2020 2020 2030 2e36 3438  |          0.648
-00006520: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00006530: 2020 2030 2e35 3039 2020 2020 2020 2020     0.509        
-00006540: 7c20 2020 2030 2e36 3237 2020 2020 207c  |    0.627     |
-00006550: 2020 302e 3236 3520 2020 7c0a 7c20 2020    0.265   |.|   
-00006560: 2020 2020 2020 6056 6954 4578 7472 6163        `ViTExtrac
-00006570: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
-00006580: 6e65 6428 2276 6974 7338 5f64 696e 6f22  ned("vits8_dino"
-00006590: 2960 2020 2020 2020 2020 207c 2020 2020  )`         |    
-000065a0: 2020 2020 2020 302e 3635 3120 2020 2020        0.651     
-000065b0: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
-000065c0: 3532 3420 2020 2020 2020 207c 2020 2020  524        |    
-000065d0: 302e 3636 3120 2020 2020 7c20 2030 2e33  0.661     |  0.3
-000065e0: 3135 2020 207c 0a7c 2020 2020 2020 2020  15   |.|        
-000065f0: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00006600: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006610: 6974 6231 365f 6469 6e6f 2229 6020 2020  itb16_dino")`   
-00006620: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00006630: 2030 2e36 3538 2020 2020 2020 2020 2020   0.658          
-00006640: 207c 2020 2020 2020 2030 2e35 3134 2020   |       0.514  
-00006650: 2020 2020 2020 7c20 2020 2030 2e35 3431        |    0.541
-00006660: 2020 2020 207c 2020 302e 3238 3820 2020       |  0.288   
-00006670: 7c0a 7c20 2020 2020 2020 2020 6056 6954  |.|         `ViT
-00006680: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-00006690: 7265 7472 6169 6e65 6428 2276 6974 6238  retrained("vitb8
-000066a0: 5f64 696e 6f22 2960 2020 2020 2020 2020  _dino")`        
-000066b0: 207c 2020 2020 2020 2020 2020 302e 3638   |          0.68
-000066c0: 3920 2020 2020 2020 2020 2020 7c20 2020  9           |   
-000066d0: 2020 2020 302e 3539 3920 2020 2020 2020      0.599       
-000066e0: 207c 2020 2020 302e 3530 3620 2020 2020   |    0.506     
-000066f0: 7c20 2030 2e33 3133 2020 207c 0a7c 2020  |  0.313   |.|  
-00006700: 2020 6052 6573 6e65 7445 7874 7261 6374    `ResnetExtract
-00006710: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
-00006720: 6564 2822 7265 736e 6574 3530 5f6d 6f63  ed("resnet50_moc
-00006730: 6f5f 7632 2229 6020 2020 2020 7c20 2020  o_v2")`     |   
-00006740: 2020 2020 2020 2030 2e34 3933 2020 2020         0.493    
-00006750: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
-00006760: 2e32 3637 2020 2020 2020 2020 7c20 2020  .267        |   
-00006770: 2030 2e32 3634 2020 2020 207c 2020 302e   0.264     |  0.
-00006780: 3134 3920 2020 7c0a 7c20 6052 6573 6e65  149   |.| `Resne
-00006790: 7445 7874 7261 6374 6f72 2e66 726f 6d5f  tExtractor.from_
-000067a0: 7072 6574 7261 696e 6564 2822 7265 736e  pretrained("resn
-000067b0: 6574 3530 5f69 6d61 6765 6e65 7431 6b5f  et50_imagenet1k_
-000067c0: 7631 2229 6020 207c 2020 2020 2020 2020  v1")`  |        
-000067d0: 2020 302e 3531 3520 2020 2020 2020 2020    0.515         
-000067e0: 2020 7c20 2020 2020 2020 302e 3238 3420    |       0.284 
-000067f0: 2020 2020 2020 207c 2020 2020 302e 3435         |    0.45
-00006800: 3520 2020 2020 7c20 2030 2e32 3437 2020  5     |  0.247  
-00006810: 207c 0a0a 2a2a 5468 6520 6d65 7472 6963   |..**The metric
-00006820: 7320 6d61 7920 6265 2064 6966 6665 7265  s may be differe
-00006830: 6e74 2066 726f 6d20 7468 6520 6f6e 6573  nt from the ones
-00006840: 2072 6570 6f72 7465 6420 6279 2070 6170   reported by pap
-00006850: 6572 732c 0a62 6563 6175 7365 2074 6865  ers,.because the
-00006860: 2076 6572 7369 6f6e 206f 6620 7472 6169   version of trai
-00006870: 6e2f 7661 6c20 7370 6c69 7420 616e 6420  n/val split and 
-00006880: 7573 6167 6520 6f66 2062 6f75 6e64 696e  usage of boundin
-00006890: 6720 626f 7865 7320 6d61 7920 6469 6666  g boxes may diff
-000068a0: 6572 2e0a 5061 7274 6963 756c 6172 6c79  er..Particularly
-000068b0: 2c20 7765 2075 7365 6420 626f 756e 6469  , we used boundi
-000068c0: 6e67 2062 6f78 6573 2064 7572 696e 6720  ng boxes during 
-000068d0: 7468 6520 6576 616c 7561 7469 6f6e 2e2a  the evaluation.*
-000068e0: 0a0a 2323 2320 486f 7720 746f 2075 7365  ..### How to use
-000068f0: 206d 6f64 656c 7320 6672 6f6d 205a 6f6f   models from Zoo
-00006900: 3f0a 0a5b 636f 6d6d 656e 745d 3a7a 6f6f  ?..[comment]:zoo
-00006910: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
-00006920: 0a66 726f 6d20 6f6d 6c2e 636f 6e73 7420  .from oml.const 
-00006930: 696d 706f 7274 2043 4b50 545f 5341 5645  import CKPT_SAVE
-00006940: 5f52 4f4f 5420 6173 2043 4b50 545f 4449  _ROOT as CKPT_DI
-00006950: 522c 204d 4f43 4b5f 4441 5441 5345 545f  R, MOCK_DATASET_
-00006960: 5041 5448 2061 7320 4441 5441 5f44 4952  PATH as DATA_DIR
-00006970: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
-00006980: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00006990: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7265  ctor.from oml.re
-000069a0: 6769 7374 7279 2e74 7261 6e73 666f 726d  gistry.transform
-000069b0: 7320 696d 706f 7274 2067 6574 5f74 7261  s import get_tra
-000069c0: 6e73 666f 726d 735f 666f 725f 7072 6574  nsforms_for_pret
-000069d0: 7261 696e 6564 0a0a 6d6f 6465 6c20 3d20  rained..model = 
-000069e0: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
-000069f0: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
-00006a00: 7473 3136 5f64 696e 6f22 290a 7472 616e  ts16_dino").tran
-00006a10: 7366 6f72 6d73 2c20 696d 5f72 6561 6465  sforms, im_reade
-00006a20: 7220 3d20 6765 745f 7472 616e 7366 6f72  r = get_transfor
-00006a30: 6d73 5f66 6f72 5f70 7265 7472 6169 6e65  ms_for_pretraine
-00006a40: 6428 2276 6974 7331 365f 6469 6e6f 2229  d("vits16_dino")
-00006a50: 0a0a 696d 6720 3d20 696d 5f72 6561 6465  ..img = im_reade
-00006a60: 7228 4441 5441 5f44 4952 202f 2022 696d  r(DATA_DIR / "im
-00006a70: 6167 6573 2220 2f20 2263 6972 636c 655f  ages" / "circle_
-00006a80: 312e 6a70 6722 2920 2023 2070 7574 2070  1.jpg")  # put p
-00006a90: 6174 6820 746f 2079 6f75 7220 696d 6167  ath to your imag
-00006aa0: 6520 6865 7265 0a69 6d67 5f74 656e 736f  e here.img_tenso
-00006ab0: 7220 3d20 7472 616e 7366 6f72 6d73 2869  r = transforms(i
-00006ac0: 6d67 290a 2320 696d 675f 7465 6e73 6f72  mg).# img_tensor
-00006ad0: 203d 2074 7261 6e73 666f 726d 7328 696d   = transforms(im
-00006ae0: 6167 653d 696d 6729 5b22 696d 6167 6522  age=img)["image"
-00006af0: 5d20 2023 2066 6f72 2074 7261 6e73 666f  ]  # for transfo
-00006b00: 726d 7320 6672 6f6d 2041 6c62 756d 656e  rms from Albumen
-00006b10: 7461 7469 6f6e 730a 0a66 6561 7475 7265  tations..feature
-00006b20: 7320 3d20 6d6f 6465 6c28 696d 675f 7465  s = model(img_te
-00006b30: 6e73 6f72 2e75 6e73 7175 6565 7a65 2830  nsor.unsqueeze(0
-00006b40: 2929 0a0a 2320 4368 6563 6b20 6f74 6865  ))..# Check othe
-00006b50: 7220 6176 6169 6c61 626c 6520 6d6f 6465  r available mode
-00006b60: 6c73 3a0a 7072 696e 7428 6c69 7374 2856  ls:.print(list(V
-00006b70: 6954 4578 7472 6163 746f 722e 7072 6574  iTExtractor.pret
-00006b80: 7261 696e 6564 5f6d 6f64 656c 732e 6b65  rained_models.ke
-00006b90: 7973 2829 2929 0a0a 2320 4c6f 6164 2063  ys()))..# Load c
-00006ba0: 6865 636b 706f 696e 7420 7361 7665 6420  heckpoint saved 
-00006bb0: 6f6e 2061 2064 6973 6b3a 0a6d 6f64 656c  on a disk:.model
-00006bc0: 5f20 3d20 5669 5445 7874 7261 6374 6f72  _ = ViTExtractor
-00006bd0: 2877 6569 6768 7473 3d43 4b50 545f 4449  (weights=CKPT_DI
-00006be0: 5220 2f20 2276 6974 7331 365f 6469 6e6f  R / "vits16_dino
-00006bf0: 2e63 6b70 7422 2c20 6172 6368 3d22 7669  .ckpt", arch="vi
-00006c00: 7473 3136 222c 206e 6f72 6d61 6c69 7365  ts16", normalise
-00006c10: 5f66 6561 7475 7265 733d 4661 6c73 6529  _features=False)
-00006c20: 0a60 6060 0a5b 636f 6d6d 656e 745d 3a7a  .```.[comment]:z
-00006c30: 6f6f 2d65 6e64 0a0a 2323 205b 436f 6e74  oo-end..## [Cont
-00006c40: 7269 6275 7469 6e67 2067 7569 6465 5d28  ributing guide](
-00006c50: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
-00006c60: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
-00006c70: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00006c80: 6174 6573 742f 6f6d 6c2f 636f 6e74 7269  atest/oml/contri
-00006c90: 6275 7469 6e67 2e68 746d 6c29 0a0a 5765  buting.html)..We
-00006ca0: 2077 656c 636f 6d65 206e 6577 2063 6f6e   welcome new con
-00006cb0: 7472 6962 7574 6f72 7321 2050 6c65 6173  tributors! Pleas
-00006cc0: 652c 2073 6565 206f 7572 3a0a 2a20 5b43  e, see our:.* [C
-00006cd0: 6f6e 7472 6962 7574 696e 6720 6775 6964  ontributing guid
-00006ce0: 655d 2868 7474 7073 3a2f 2f6f 7065 6e2d  e](https://open-
-00006cf0: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-00006d00: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00006d10: 6e2f 6c61 7465 7374 2f66 726f 6d5f 7265  n/latest/from_re
-00006d20: 6164 6d65 2f63 6f6e 7472 6962 7574 696e  adme/contributin
-00006d30: 672e 6874 6d6c 290a 2a20 5b4b 616e 6261  g.html).* [Kanba
-00006d40: 6e20 626f 6172 645d 2868 7474 7073 3a2f  n board](https:/
-00006d50: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
-00006d60: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
-00006d70: 2d6c 6561 726e 696e 672f 7072 6f6a 6563  -learning/projec
-00006d80: 7473 2f31 290a 0a23 2320 4163 6b6e 6f77  ts/1)..## Acknow
-00006d90: 6c65 6467 6d65 6e74 730a 0a3c 6120 6872  ledgments..<a hr
-00006da0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00006db0: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00006dc0: 7465 616d 2f63 6174 616c 7973 7422 2074  team/catalyst" t
-00006dd0: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00006de0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00006df0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00006e00: 6f6e 7465 6e74 2e63 6f6d 2f63 6174 616c  ontent.com/catal
-00006e10: 7973 742d 7465 616d 2f63 6174 616c 7973  yst-team/catalys
-00006e20: 742d 7069 6373 2f6d 6173 7465 722f 7069  t-pics/master/pi
-00006e30: 6373 2f63 6174 616c 7973 745f 6c6f 676f  cs/catalyst_logo
-00006e40: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
-00006e50: 222f 3e3c 2f61 3e0a 0a54 6865 2070 726f  "/></a>..The pro
-00006e60: 6a65 6374 2077 6173 2073 7461 7274 6564  ject was started
-00006e70: 2069 6e20 3230 3230 2061 7320 6120 6d6f   in 2020 as a mo
-00006e80: 6475 6c65 2066 6f72 205b 4361 7461 6c79  dule for [Cataly
-00006e90: 7374 5d28 6874 7470 733a 2f2f 6769 7468  st](https://gith
-00006ea0: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00006eb0: 7465 616d 2f63 6174 616c 7973 7429 206c  team/catalyst) l
-00006ec0: 6962 7261 7279 2e0a 4920 7761 6e74 2074  ibrary..I want t
-00006ed0: 6f20 7468 616e 6b20 7065 6f70 6c65 2077  o thank people w
-00006ee0: 686f 2077 6f72 6b65 6420 7769 7468 206d  ho worked with m
-00006ef0: 6520 6f6e 2074 6861 7420 6d6f 6475 6c65  e on that module
-00006f00: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
-00006f10: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
-00006f20: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
-00006f30: 6e73 6869 6e61 292c 0a5b 4e69 6b69 7461  nshina),.[Nikita
-00006f40: 2042 616c 6167 616e 736b 795d 2868 7474   Balagansky](htt
-00006f50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00006f60: 656c 6570 6861 6e74 6d69 7074 292c 0a5b  elephantmipt),.[
-00006f70: 5365 7267 6579 204b 6f6c 6573 6e69 6b6f  Sergey Kolesniko
-00006f80: 765d 2868 7474 7073 3a2f 2f67 6974 6875  v](https://githu
-00006f90: 622e 636f 6d2f 5363 6974 6174 6f72 290a  b.com/Scitator).
-00006fa0: 616e 6420 6f74 6865 7273 2e0a 0a49 2077  and others...I w
-00006fb0: 6f75 6c64 206c 696b 6520 746f 2074 6861  ould like to tha
-00006fc0: 6e6b 2070 656f 706c 6520 7768 6f20 636f  nk people who co
-00006fd0: 6e74 696e 7565 2077 6f72 6b69 6e67 206f  ntinue working o
-00006fe0: 6e20 7468 6973 2070 6970 656c 696e 6520  n this pipeline 
-00006ff0: 7768 656e 2069 7420 6265 6361 6d65 2061  when it became a
-00007000: 2073 6570 6172 6520 7072 6f6a 6563 743a   separe project:
-00007010: 0a5b 4a75 6c69 6120 5368 656e 7368 696e  .[Julia Shenshin
-00007020: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00007030: 622e 636f 6d2f 6a75 6c69 612d 7368 656e  b.com/julia-shen
-00007040: 7368 696e 6129 2c0a 5b4d 6973 6861 204b  shina),.[Misha K
-00007050: 696e 6475 6c6f 765d 2868 7474 7073 3a2f  indulov](https:/
-00007060: 2f67 6974 6875 622e 636f 6d2f 6230 6e63  /github.com/b0nc
-00007070: 6529 2c0a 5b41 6c65 6b73 6569 2054 6172  e),.[Aleksei Tar
-00007080: 6173 6f76 5d28 6874 7470 733a 2f2f 6769  asov](https://gi
-00007090: 7468 7562 2e63 6f6d 2f44 616c 6f72 6f41  thub.com/DaloroA
-000070a0: 5429 2061 6e64 0a5b 5665 726b 686f 7674  T) and.[Verkhovt
-000070b0: 7365 7620 4c65 6f6e 6964 5d28 6874 7470  sev Leonid](http
-000070c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-000070d0: 656f 726f 6d61 6e6f 7669 6368 292e 0a0a  eoromanovich)...
-000070e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000070f0: 2f77 7777 2e6e 6577 796f 726b 6572 2e64  /www.newyorker.d
-00007100: 652f 2220 7461 7267 6574 3d22 5f62 6c61  e/" target="_bla
-00007110: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
-00007120: 7470 733a 2f2f 7570 6c6f 6164 2e77 696b  tps://upload.wik
-00007130: 696d 6564 6961 2e6f 7267 2f77 696b 6970  imedia.org/wikip
-00007140: 6564 6961 2f63 6f6d 6d6f 6e73 2f74 6875  edia/commons/thu
-00007150: 6d62 2f64 2f64 382f 4e65 775f 596f 726b  mb/d/d8/New_York
-00007160: 6572 2e73 7667 2f31 3238 3070 782d 4e65  er.svg/1280px-Ne
-00007170: 775f 596f 726b 6572 2e73 7667 2e70 6e67  w_Yorker.svg.png
-00007180: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
-00007190: 2f61 3e0a 0a49 2061 6c73 6f20 7761 6e74  /a>..I also want
-000071a0: 2074 6f20 7468 616e 6b20 4e65 7759 6f72   to thank NewYor
-000071b0: 6b65 722c 2073 696e 6365 2074 6865 2070  ker, since the p
-000071c0: 6172 7420 6f66 2066 756e 6374 696f 6e61  art of functiona
-000071d0: 6c69 7479 2077 6173 2064 6576 656c 6f70  lity was develop
-000071e0: 6564 2028 616e 6420 7573 6564 2920 6279  ed (and used) by
-000071f0: 2069 7473 2063 6f6d 7075 7465 7220 7669   its computer vi
-00007200: 7369 6f6e 2074 6561 6d20 6c65 6420 6279  sion team led by
-00007210: 206d 652e 0a                              me..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
+00000020: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00000030: 0a56 6572 7369 6f6e 3a20 302e 342e 340a  .Version: 0.4.4.
+00000040: 5375 6d6d 6172 793a 204f 4d4c 2069 7320  Summary: OML is 
+00000050: 6120 5079 546f 7263 682d 6261 7365 6420  a PyTorch-based 
+00000060: 6672 616d 6577 6f72 6b20 746f 2074 7261  framework to tra
+00000070: 696e 2061 6e64 2076 616c 6964 6174 6520  in and validate 
+00000080: 7468 6520 6d6f 6465 6c73 2070 726f 6475  the models produ
+00000090: 6369 6e67 2068 6967 682d 7175 616c 6974  cing high-qualit
+000000a0: 7920 656d 6265 6464 696e 6773 2e0a 486f  y embeddings..Ho
+000000b0: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+000000c0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+000000d0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+000000e0: 2d6c 6561 726e 696e 670a 4175 7468 6f72  -learning.Author
+000000f0: 3a20 5368 6162 616e 6f76 2041 6c65 6b73  : Shabanov Aleks
+00000100: 6569 0a41 7574 686f 722d 656d 6169 6c3a  ei.Author-email:
+00000110: 2073 6861 6261 6e6f 6666 2e61 6c65 6b73   shabanoff.aleks
+00000120: 6569 4067 6d61 696c 2e63 6f6d 0a4c 6963  ei@gmail.com.Lic
+00000130: 656e 7365 3a20 4170 6163 6865 204c 6963  ense: Apache Lic
+00000140: 656e 7365 2032 2e30 0a50 726f 6a65 6374  ense 2.0.Project
+00000150: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
+00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000170: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
+00000180: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00000190: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
+000001a0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000001c0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000001d0: 6963 2d6c 6561 726e 696e 672f 6973 7375  ic-learning/issu
+000001e0: 6573 0a4b 6579 776f 7264 733a 2064 6174  es.Keywords: dat
+000001f0: 612d 7363 6965 6e63 652c 636f 6d70 7574  a-science,comput
+00000200: 6572 2d76 6973 696f 6e2c 6465 6570 2d6c  er-vision,deep-l
+00000210: 6561 726e 696e 672c 7079 746f 7263 682c  earning,pytorch,
+00000220: 6d65 7472 6963 2d6c 6561 726e 696e 672c  metric-learning,
+00000230: 7265 7072 6573 656e 7461 7469 6f6e 2d6c  representation-l
+00000240: 6561 726e 696e 672c 7079 746f 7263 682d  earning,pytorch-
+00000250: 6c69 6768 746e 696e 670a 436c 6173 7369  lightning.Classi
+00000260: 6669 6572 3a20 456e 7669 726f 6e6d 656e  fier: Environmen
+00000270: 7420 3a3a 2043 6f6e 736f 6c65 0a43 6c61  t :: Console.Cla
+00000280: 7373 6966 6965 723a 204e 6174 7572 616c  ssifier: Natural
+00000290: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
+000002a0: 6c69 7368 0a43 6c61 7373 6966 6965 723a  lish.Classifier:
+000002b0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+000002c0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000002d0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
+000002e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000002f0: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
+00000300: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
+00000310: 7365 0a43 6c61 7373 6966 6965 723a 2049  se.Classifier: I
+00000320: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000330: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
+00000340: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00000350: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000360: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+00000370: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000380: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
+00000390: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
+000003a0: 4172 7469 6669 6369 616c 2049 6e74 656c  Artificial Intel
+000003b0: 6c69 6765 6e63 650a 436c 6173 7369 6669  ligence.Classifi
+000003c0: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
+000003d0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+000003e0: 696e 6720 3a3a 2049 6d61 6765 2052 6563  ing :: Image Rec
+000003f0: 6f67 6e69 7469 6f6e 0a43 6c61 7373 6966  ognition.Classif
+00000400: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000410: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000420: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
+00000430: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000440: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000450: 3a20 332e 370a 436c 6173 7369 6669 6572  : 3.7.Classifier
+00000460: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000470: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000480: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+00000490: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000004a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000004b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
+000004c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000004d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000004e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
+000004f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000500: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000510: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
+00000520: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
+00000530: 7468 6f6e 0a52 6571 7569 7265 732d 5079  thon.Requires-Py
+00000540: 7468 6f6e 3a20 3e3d 332e 372c 3c34 2e30  thon: >=3.7,<4.0
+00000550: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000560: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000570: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000580: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+00000590: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+000005a0: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+000005b0: 7474 7073 3a2f 2f69 2e69 6262 2e63 6f2f  ttps://i.ibb.co/
+000005c0: 7773 6d44 3572 342f 7068 6f74 6f2d 3230  wsmD5r4/photo-20
+000005d0: 3232 2d30 362d 3036 2d31 372d 3430 2d35  22-06-06-17-40-5
+000005e0: 322e 6a70 6722 2077 6964 7468 3d22 3430  2.jpg" width="40
+000005f0: 3070 7822 3e0a 0a21 5b65 7861 6d70 6c65  0px">..![example
+00000600: 2077 6f72 6b66 6c6f 775d 2868 7474 7073   workflow](https
+00000610: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+00000620: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+00000630: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
+00000640: 6f6e 732f 776f 726b 666c 6f77 732f 7072  ons/workflows/pr
+00000650: 652d 636f 6d6d 6974 2d77 6f72 6b66 6c6f  e-commit-workflo
+00000660: 772e 7961 6d6c 2f62 6164 6765 2e73 7667  w.yaml/badge.svg
+00000670: 290a 215b 6578 616d 706c 6520 776f 726b  ).![example work
+00000680: 666c 6f77 5d28 6874 7470 733a 2f2f 6769  flow](https://gi
+00000690: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
+000006a0: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
+000006b0: 6172 6e69 6e67 2f61 6374 696f 6e73 2f77  arning/actions/w
+000006c0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2d77  orkflows/tests-w
+000006d0: 6f72 6b66 6c6f 772e 7961 6d6c 2f62 6164  orkflow.yaml/bad
+000006e0: 6765 2e73 7667 3f29 0a5b 215b 446f 6375  ge.svg?).[![Docu
+000006f0: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000700: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
+00000710: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000720: 7473 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ts/open-metric-l
+00000730: 6561 726e 696e 672f 6261 6467 652f 3f76  earning/badge/?v
+00000740: 6572 7369 6f6e 3d6c 6174 6573 7429 5d28  ersion=latest)](
+00000750: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
+00000760: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
+00000770: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000780: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+00000790: 6573 7429 0a5b 215b 5079 5049 2053 7461  est).[![PyPI Sta
+000007a0: 7475 735d 2868 7474 7073 3a2f 2f70 6570  tus](https://pep
+000007b0: 792e 7465 6368 2f62 6164 6765 2f6f 7065  y.tech/badge/ope
+000007c0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
+000007d0: 6729 5d28 6874 7470 733a 2f2f 7065 7079  g)](https://pepy
+000007e0: 2e74 6563 682f 7072 6f6a 6563 742f 6f70  .tech/project/op
+000007f0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
+00000800: 6e67 290a 5b21 5b50 6970 6920 7665 7273  ng).[![Pipi vers
+00000810: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
+00000820: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000830: 2f76 2f6f 7065 6e2d 6d65 7472 6963 2d6c  /v/open-metric-l
+00000840: 6561 726e 696e 672e 7376 6729 5d28 6874  earning.svg)](ht
+00000850: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000860: 726f 6a65 6374 2f6f 7065 6e2d 6d65 7472  roject/open-metr
+00000870: 6963 2d6c 6561 726e 696e 672f 290a 215b  ic-learning/).![
+00000880: 6578 616d 706c 6520 776f 726b 666c 6f77  example workflow
+00000890: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008a0: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
+000008b0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
+000008c0: 6e67 2f61 6374 696f 6e73 2f77 6f72 6b66  ng/actions/workf
+000008d0: 6c6f 7773 2f70 7974 686f 6e2d 7665 7273  lows/python-vers
+000008e0: 696f 6e73 2e79 616d 6c2f 6261 6467 652e  ions.yaml/badge.
+000008f0: 7376 673f 290a 5b21 5b70 7974 686f 6e5d  svg?).[![python]
+00000900: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000910: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00000920: 7468 6f6e 5f33 2e37 2d70 6173 7369 6e67  thon_3.7-passing
+00000930: 2d73 7563 6365 7373 295d 2868 7474 7073  -success)](https
+00000940: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+00000950: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+00000960: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
+00000970: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+00000980: 7468 6f6e 2d76 6572 7369 6f6e 732e 7961  thon-versions.ya
+00000990: 6d6c 2f62 6164 6765 2e73 7667 3f29 0a5b  ml/badge.svg?).[
+000009a0: 215b 7079 7468 6f6e 5d28 6874 7470 733a  ![python](https:
+000009b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000009c0: 2f62 6164 6765 2f70 7974 686f 6e5f 332e  /badge/python_3.
+000009d0: 382d 7061 7373 696e 672d 7375 6363 6573  8-passing-succes
+000009e0: 7329 5d28 6874 7470 733a 2f2f 6769 7468  s)](https://gith
+000009f0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
+00000a00: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00000a10: 6e69 6e67 2f61 6374 696f 6e73 2f77 6f72  ning/actions/wor
+00000a20: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7665  kflows/python-ve
+00000a30: 7273 696f 6e73 2e79 616d 6c2f 6261 6467  rsions.yaml/badg
+00000a40: 652e 7376 673f 290a 5b21 5b70 7974 686f  e.svg?).[![pytho
+00000a50: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000a60: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000a70: 7079 7468 6f6e 5f33 2e39 2d70 6173 7369  python_3.9-passi
+00000a80: 6e67 2d73 7563 6365 7373 295d 2868 7474  ng-success)](htt
+00000a90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000aa0: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
+00000ab0: 7472 6963 2d6c 6561 726e 696e 672f 6163  tric-learning/ac
+00000ac0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000ad0: 7079 7468 6f6e 2d76 6572 7369 6f6e 732e  python-versions.
+00000ae0: 7961 6d6c 2f62 6164 6765 2e73 7667 3f29  yaml/badge.svg?)
+00000af0: 0a5b 215b 7079 7468 6f6e 5d28 6874 7470  .[![python](http
+00000b00: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b10: 696f 2f62 6164 6765 2f70 7974 686f 6e5f  io/badge/python_
+00000b20: 332e 3130 2d70 6173 7369 6e67 2d73 7563  3.10-passing-suc
+00000b30: 6365 7373 295d 2868 7474 7073 3a2f 2f67  cess)](https://g
+00000b40: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
+00000b50: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
+00000b60: 6561 726e 696e 672f 6163 7469 6f6e 732f  earning/actions/
+00000b70: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
+00000b80: 2d76 6572 7369 6f6e 732e 7961 6d6c 2f62  -versions.yaml/b
+00000b90: 6164 6765 2e73 7667 3f29 0a0a 4f4d 4c20  adge.svg?)..OML 
+00000ba0: 6973 2061 2050 7954 6f72 6368 2d62 6173  is a PyTorch-bas
+00000bb0: 6564 2066 7261 6d65 776f 726b 2074 6f20  ed framework to 
+00000bc0: 7472 6169 6e20 616e 6420 7661 6c69 6461  train and valida
+00000bd0: 7465 2074 6865 206d 6f64 656c 7320 7072  te the models pr
+00000be0: 6f64 7563 696e 6720 6869 6768 2d71 7561  oducing high-qua
+00000bf0: 6c69 7479 2065 6d62 6564 6469 6e67 732e  lity embeddings.
+00000c00: 0a0a 2323 2320 5472 7573 7465 6420 6279  ..### Trusted by
+00000c10: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000c20: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+00000c30: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+00000c40: 7475 6e65 2e61 692f 696e 7465 6772 6174  tune.ai/integrat
+00000c50: 696f 6e73 2f63 6f6d 6d75 6e69 7479 5f64  ions/community_d
+00000c60: 6576 656c 6f70 6564 2f22 2074 6172 6765  eveloped/" targe
+00000c70: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+00000c80: 7372 633d 2268 7474 7073 3a2f 2f73 6563  src="https://sec
+00000c90: 7572 6974 792e 6e65 7074 756e 652e 6169  urity.neptune.ai
+00000ca0: 2f61 7069 2f73 6861 7265 2f62 3730 3766  /api/share/b707f
+00000cb0: 3165 382d 6532 3837 2d34 6630 312d 6235  1e8-e287-4f01-b5
+00000cc0: 3930 2d33 3961 3666 6137 6539 6661 612f  90-39a6fa7e9faa/
+00000cd0: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
+00000ce0: 2231 3030 222f 3e3c 2f61 3ee3 85a4 e385  "100"/></a>.....
+00000cf0: a40a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000d00: 3a2f 2f77 7777 2e6e 6577 796f 726b 6572  ://www.newyorker
+00000d10: 2e64 652f 2220 7461 7267 6574 3d22 5f62  .de/" target="_b
+00000d20: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+00000d30: 6874 7470 733a 2f2f 7570 6c6f 6164 2e77  https://upload.w
+00000d40: 696b 696d 6564 6961 2e6f 7267 2f77 696b  ikimedia.org/wik
+00000d50: 6970 6564 6961 2f63 6f6d 6d6f 6e73 2f74  ipedia/commons/t
+00000d60: 6875 6d62 2f64 2f64 382f 4e65 775f 596f  humb/d/d8/New_Yo
+00000d70: 726b 6572 2e73 7667 2f31 3238 3070 782d  rker.svg/1280px-
+00000d80: 4e65 775f 596f 726b 6572 2e73 7667 2e70  New_Yorker.svg.p
+00000d90: 6e67 2220 7769 6474 683d 2231 3030 222f  ng" width="100"/
+00000da0: 3e3c 2f61 3ee3 85a4 e385 a40a 3c61 2068  ></a>.......<a h
+00000db0: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000dc0: 2e65 706f 6368 382e 636f 2f22 2074 6172  .epoch8.co/" tar
+00000dd0: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+00000de0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000df0: 2e69 6262 2e63 6f2f 4764 4e56 5479 742f  .ibb.co/GdNVTyt/
+00000e00: 5363 7265 656e 7368 6f74 2d32 3032 332d  Screenshot-2023-
+00000e10: 3037 2d30 342d 6174 2d31 312d 3139 2d32  07-04-at-11-19-2
+00000e20: 342e 706e 6722 2077 6964 7468 3d22 3130  4.png" width="10
+00000e30: 3022 2f3e 3c2f 613e e385 a4e3 85a4 0a3c  0"/></a>.......<
+00000e40: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000e50: 7777 772e 6d65 6974 7561 6e2e 636f 6d22  www.meituan.com"
+00000e60: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000e70: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000e80: 3a2f 2f75 706c 6f61 642e 7769 6b69 6d65  ://upload.wikime
+00000e90: 6469 612e 6f72 672f 7769 6b69 7065 6469  dia.org/wikipedi
+00000ea0: 612f 636f 6d6d 6f6e 732f 362f 3631 2f4d  a/commons/6/61/M
+00000eb0: 6569 7475 616e 5f45 6e67 6c69 7368 5f4c  eituan_English_L
+00000ec0: 6f67 6f2e 706e 6722 2077 6964 7468 3d22  ogo.png" width="
+00000ed0: 3130 3022 2f3e 3c2f 613e 0a0a 3c61 2068  100"/></a>..<a h
+00000ee0: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000ef0: 2e6f 782e 6163 2e75 6b2f 2220 7461 7267  .ox.ac.uk/" targ
+00000f00: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00000f10: 2073 7263 3d22 6874 7470 733a 2f2f 7570   src="https://up
+00000f20: 6c6f 6164 2e77 696b 696d 6564 6961 2e6f  load.wikimedia.o
+00000f30: 7267 2f77 696b 6970 6564 6961 2f65 6e2f  rg/wikipedia/en/
+00000f40: 7468 756d 622f 322f 3266 2f55 6e69 7665  thumb/2/2f/Unive
+00000f50: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+00000f60: 7376 672f 3235 3630 7078 2d55 6e69 7665  svg/2560px-Unive
+00000f70: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+00000f80: 7376 672e 706e 6722 2077 6964 7468 3d22  svg.png" width="
+00000f90: 3132 3022 2f3e 3c2f 613e e385 a4e3 85a4  120"/></a>......
+00000fa0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000fb0: 2f2f 7777 772e 6873 652e 7275 2f65 6e2f  //www.hse.ru/en/
+00000fc0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000fd0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000fe0: 733a 2f2f 7777 772e 6873 652e 7275 2f64  s://www.hse.ru/d
+00000ff0: 6174 612f 3230 3230 2f31 312f 3136 2f31  ata/2020/11/16/1
+00001000: 3336 3732 3734 3034 342f 4853 455f 556e  367274044/HSE_Un
+00001010: 6976 6572 7369 7479 5f62 6c75 652e 6a70  iversity_blue.jp
+00001020: 672e 2832 3330 7838 3678 3132 3329 2e6a  g.(230x86x123).j
+00001030: 7067 2220 7769 6474 683d 2231 3030 222f  pg" width="100"/
+00001040: 3e3c 2f61 3e0a 0a54 6865 7265 2069 7320  ></a>..There is 
+00001050: 6120 6e75 6d62 6572 206f 6620 7065 6f70  a number of peop
+00001060: 6c65 2066 726f 6d0a 5b4f 7866 6f72 645d  le from.[Oxford]
+00001070: 2868 7474 7073 3a2f 2f77 7777 2e6f 782e  (https://www.ox.
+00001080: 6163 2e75 6b2f 2920 616e 640a 5b48 5345  ac.uk/) and.[HSE
+00001090: 5d28 6874 7470 733a 2f2f 7777 772e 6873  ](https://www.hs
+000010a0: 652e 7275 2f65 6e2f 290a 756e 6976 6572  e.ru/en/).univer
+000010b0: 7369 7469 6573 2077 686f 2068 6176 6520  sities who have 
+000010c0: 7573 6564 204f 4d4c 2069 6e20 7468 6569  used OML in thei
+000010d0: 7220 7468 6573 6573 2e0a 5b5b 315d 5d28  r theses..[[1]](
+000010e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000010f0: 6f6d 2f6e 696c 6f6d 722f 6f70 656e 2d6d  om/nilomr/open-m
+00001100: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+00001110: 7265 652f 6772 6561 742d 7469 742f 6772  ree/great-tit/gr
+00001120: 6561 742d 7469 742d 7472 6169 6e29 0a5b  eat-tit-train).[
+00001130: 5b32 5d5d 2868 7474 7073 3a2f 2f67 6974  [2]](https://git
+00001140: 6875 622e 636f 6d2f 6e61 7374 7967 6f72  hub.com/nastygor
+00001150: 6f64 692f 5052 4f4a 4543 542d 4465 6570  odi/PROJECT-Deep
+00001160: 5f4d 6574 7269 635f 4c65 6172 6e69 6e67  _Metric_Learning
+00001170: 290a 5b5b 335d 5d28 6874 7470 733a 2f2f  ).[[3]](https://
+00001180: 6769 7468 7562 2e63 6f6d 2f6e 696b 2d66  github.com/nik-f
+00001190: 6564 6f72 6f76 2f74 6572 6d5f 7061 7065  edorov/term_pape
+000011a0: 725f 6d65 7472 6963 5f6c 6561 726e 696e  r_metric_learnin
+000011b0: 6729 0a0a 3c64 6976 2061 6c69 676e 3d22  g)..<div align="
+000011c0: 6c65 6674 223e 0a0a 2323 205b 4641 515d  left">..## [FAQ]
+000011d0: 2868 7474 7073 3a2f 2f6f 7065 6e2d 6d65  (https://open-me
+000011e0: 7472 6963 2d6c 6561 726e 696e 672e 7265  tric-learning.re
+000011f0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001200: 6c61 7465 7374 2f6f 6d6c 2f66 6171 2e68  latest/oml/faq.h
+00001210: 746d 6c29 0a0a 3c64 6574 6169 6c73 3e0a  tml)..<details>.
+00001220: 3c73 756d 6d61 7279 3e57 6879 2064 6f20  <summary>Why do 
+00001230: 4920 6e65 6564 204f 4d4c 3f3c 2f73 756d  I need OML?</sum
+00001240: 6d61 7279 3e0a 3c70 3e0a 0a59 6f75 206d  mary>.<p>..You m
+00001250: 6179 2074 6869 6e6b 202a 2249 6620 4920  ay think *"If I 
+00001260: 6e65 6564 2069 6d61 6765 2065 6d62 6564  need image embed
+00001270: 6469 6e67 7320 4920 6361 6e20 7369 6d70  dings I can simp
+00001280: 6c79 2074 7261 696e 2061 2076 616e 696c  ly train a vanil
+00001290: 6c61 2063 6c61 7373 6966 6965 7220 616e  la classifier an
+000012a0: 6420 7461 6b65 2069 7473 2070 656e 756c  d take its penul
+000012b0: 7469 6d61 7465 206c 6179 6572 222a 2e0a  timate layer"*..
+000012c0: 5765 6c6c 2c20 6974 206d 616b 6573 2073  Well, it makes s
+000012d0: 656e 7365 2061 7320 6120 7374 6172 7469  ense as a starti
+000012e0: 6e67 2070 6f69 6e74 2e20 4275 7420 7468  ng point. But th
+000012f0: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
+00001300: 706f 7373 6962 6c65 2064 7261 7762 6163  possible drawbac
+00001310: 6b73 3a0a 0a2a 2049 6620 796f 7520 7761  ks:..* If you wa
+00001320: 6e74 2074 6f20 7573 6520 656d 6265 6464  nt to use embedd
+00001330: 696e 6773 2074 6f20 7065 7266 6f72 6d20  ings to perform 
+00001340: 7365 6172 6368 696e 6720 796f 7520 6e65  searching you ne
+00001350: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+00001360: 736f 6d65 2064 6973 7461 6e63 6520 616d  some distance am
+00001370: 6f6e 6720 7468 656d 2028 666f 7220 6578  ong them (for ex
+00001380: 616d 706c 652c 2063 6f73 696e 6520 6f72  ample, cosine or
+00001390: 204c 3229 2e0a 2020 5573 7561 6c6c 792c   L2)..  Usually,
+000013a0: 202a 2a79 6f75 2064 6f6e 2774 2064 6972   **you don't dir
+000013b0: 6563 746c 7920 6f70 7469 6d69 7a65 2074  ectly optimize t
+000013c0: 6865 7365 2064 6973 7461 6e63 6573 2064  hese distances d
+000013d0: 7572 696e 6720 7468 6520 7472 6169 6e69  uring the traini
+000013e0: 6e67 2a2a 2069 6e20 7468 6520 636c 6173  ng** in the clas
+000013f0: 7369 6669 6361 7469 6f6e 2073 6574 7570  sification setup
+00001400: 2e20 536f 2c20 796f 7520 6361 6e20 6f6e  . So, you can on
+00001410: 6c79 2068 6f70 6520 7468 6174 0a20 2066  ly hope that.  f
+00001420: 696e 616c 2065 6d62 6564 6469 6e67 7320  inal embeddings 
+00001430: 7769 6c6c 2068 6176 6520 7468 6520 6465  will have the de
+00001440: 7369 7265 6420 7072 6f70 6572 7469 6573  sired properties
+00001450: 2e0a 0a2a 202a 2a54 6865 2073 6563 6f6e  ...* **The secon
+00001460: 6420 7072 6f62 6c65 6d20 6973 2074 6865  d problem is the
+00001470: 2076 616c 6964 6174 696f 6e20 7072 6f63   validation proc
+00001480: 6573 732a 2a2e 0a20 2049 6e20 7468 6520  ess**..  In the 
+00001490: 7365 6172 6368 696e 6720 7365 7475 702c  searching setup,
+000014a0: 2079 6f75 2075 7375 616c 6c79 2063 6172   you usually car
+000014b0: 6520 686f 7720 7265 6c61 7465 6420 796f  e how related yo
+000014c0: 7572 2074 6f70 2d4e 206f 7574 7075 7473  ur top-N outputs
+000014d0: 2061 7265 2074 6f20 7468 6520 7175 6572   are to the quer
+000014e0: 792e 0a20 2054 6865 206e 6174 7572 616c  y..  The natural
+000014f0: 2077 6179 2074 6f20 6576 616c 7561 7465   way to evaluate
+00001500: 2074 6865 206d 6f64 656c 2069 7320 746f   the model is to
+00001510: 2073 696d 756c 6174 6520 7365 6172 6368   simulate search
+00001520: 696e 6720 7265 7175 6573 7473 2074 6f20  ing requests to 
+00001530: 7468 6520 7265 6665 7265 6e63 6520 7365  the reference se
+00001540: 740a 2020 616e 6420 6170 706c 7920 6f6e  t.  and apply on
+00001550: 6520 6f66 2074 6865 2072 6574 7269 6576  e of the retriev
+00001560: 616c 206d 6574 7269 6373 2e0a 2020 536f  al metrics..  So
+00001570: 2c20 7468 6572 6520 6973 206e 6f20 6775  , there is no gu
+00001580: 6172 616e 7465 6520 7468 6174 2063 6c61  arantee that cla
+00001590: 7373 6966 6963 6174 696f 6e20 6163 6375  ssification accu
+000015a0: 7261 6379 2077 696c 6c20 636f 7272 656c  racy will correl
+000015b0: 6174 6520 7769 7468 2074 6865 7365 206d  ate with these m
+000015c0: 6574 7269 6373 2e0a 0a2a 2046 696e 616c  etrics...* Final
+000015d0: 6c79 2c20 796f 7520 6d61 7920 7761 6e74  ly, you may want
+000015e0: 2074 6f20 696d 706c 656d 656e 7420 6120   to implement a 
+000015f0: 6d65 7472 6963 206c 6561 726e 696e 6720  metric learning 
+00001600: 7069 7065 6c69 6e65 2062 7920 796f 7572  pipeline by your
+00001610: 7365 6c66 2e0a 2020 2a2a 5468 6572 6520  self..  **There 
+00001620: 6973 2061 206c 6f74 206f 6620 776f 726b  is a lot of work
+00001630: 2a2a 3a20 746f 2075 7365 2074 7269 706c  **: to use tripl
+00001640: 6574 206c 6f73 7320 796f 7520 6e65 6564  et loss you need
+00001650: 2074 6f20 666f 726d 2062 6174 6368 6573   to form batches
+00001660: 2069 6e20 6120 7370 6563 6966 6963 2077   in a specific w
+00001670: 6179 2c0a 2020 696d 706c 656d 656e 7420  ay,.  implement 
+00001680: 6469 6666 6572 656e 7420 6b69 6e64 7320  different kinds 
+00001690: 6f66 2074 7269 706c 6574 7320 6d69 6e69  of triplets mini
+000016a0: 6e67 2c20 7472 6163 6b69 6e67 2064 6973  ng, tracking dis
+000016b0: 7461 6e63 6573 2c20 6574 632e 2046 6f72  tances, etc. For
+000016c0: 2074 6865 2076 616c 6964 6174 696f 6e2c   the validation,
+000016d0: 2079 6f75 2061 6c73 6f20 6e65 6564 2074   you also need t
+000016e0: 6f0a 2020 696d 706c 656d 656e 7420 7265  o.  implement re
+000016f0: 7472 6965 7661 6c20 6d65 7472 6963 732c  trieval metrics,
+00001700: 0a20 2077 6869 6368 2069 6e63 6c75 6465  .  which include
+00001710: 2065 6666 6563 7469 7665 2065 6d62 6564   effective embed
+00001720: 6469 6e67 7320 6163 6375 6d75 6c61 7469  dings accumulati
+00001730: 6f6e 2064 7572 696e 6720 7468 6520 6570  on during the ep
+00001740: 6f63 682c 2063 6f76 6572 696e 6720 636f  och, covering co
+00001750: 726e 6572 2063 6173 6573 2c20 6574 632e  rner cases, etc.
+00001760: 0a20 2049 7427 7320 6576 656e 2068 6172  .  It's even har
+00001770: 6465 7220 6966 2079 6f75 2068 6176 6520  der if you have 
+00001780: 7365 7665 7261 6c20 6770 7573 2061 6e64  several gpus and
+00001790: 2075 7365 2044 4450 2e0a 2020 596f 7520   use DDP..  You 
+000017a0: 6d61 7920 616c 736f 2077 616e 7420 746f  may also want to
+000017b0: 2076 6973 7561 6c69 7a65 2079 6f75 7220   visualize your 
+000017c0: 7365 6172 6368 2072 6571 7565 7374 7320  search requests 
+000017d0: 6279 2068 6967 686c 6967 6874 696e 6720  by highlighting 
+000017e0: 676f 6f64 2061 6e64 2062 6164 2073 6561  good and bad sea
+000017f0: 7263 6820 7265 7375 6c74 732e 0a20 2049  rch results..  I
+00001800: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
+00001810: 6974 2062 7920 796f 7572 7365 6c66 2c20  it by yourself, 
+00001820: 796f 7520 6361 6e20 7369 6d70 6c79 2075  you can simply u
+00001830: 7365 204f 4d4c 2066 6f72 2079 6f75 7220  se OML for your 
+00001840: 7075 7270 6f73 6573 2e0a 0a3c 2f70 3e0a  purposes...</p>.
+00001850: 3c2f 6465 7461 696c 733e 0a0a 0a3c 6465  </details>...<de
+00001860: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+00001870: 5768 6174 2069 7320 7468 6520 6469 6666  What is the diff
+00001880: 6572 656e 6365 2062 6574 7765 656e 204f  erence between O
+00001890: 7065 6e20 4d65 7472 6963 204c 6561 726e  pen Metric Learn
+000018a0: 696e 6720 616e 6420 5079 546f 7263 6820  ing and PyTorch 
+000018b0: 4d65 7472 6963 204c 6561 726e 696e 673f  Metric Learning?
+000018c0: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+000018d0: 5b50 4d4c 5d28 6874 7470 733a 2f2f 6769  [PML](https://gi
+000018e0: 7468 7562 2e63 6f6d 2f4b 6576 696e 4d75  thub.com/KevinMu
+000018f0: 7367 7261 7665 2f70 7974 6f72 6368 2d6d  sgrave/pytorch-m
+00001900: 6574 7269 632d 6c65 6172 6e69 6e67 2920  etric-learning) 
+00001910: 6973 2074 6865 2070 6f70 756c 6172 206c  is the popular l
+00001920: 6962 7261 7279 2066 6f72 204d 6574 7269  ibrary for Metri
+00001930: 6320 4c65 6172 6e69 6e67 2c0a 616e 6420  c Learning,.and 
+00001940: 6974 2069 6e63 6c75 6465 7320 6120 7269  it includes a ri
+00001950: 6368 2063 6f6c 6c65 6374 696f 6e20 6f66  ch collection of
+00001960: 206c 6f73 7365 732c 206d 696e 6572 732c   losses, miners,
+00001970: 2064 6973 7461 6e63 6573 2c20 616e 6420   distances, and 
+00001980: 7265 6475 6365 7273 3b20 7468 6174 2069  reducers; that i
+00001990: 7320 7768 7920 7765 2070 726f 7669 6465  s why we provide
+000019a0: 2073 7472 6169 6768 7466 6f72 7761 7264   straightforward
+000019b0: 0a5b 6578 616d 706c 6573 5d28 6874 7470  .[examples](http
+000019c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+000019d0: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+000019e0: 7269 632d 6c65 6172 6e69 6e67 2375 7361  ric-learning#usa
+000019f0: 6765 2d77 6974 682d 7079 746f 7263 682d  ge-with-pytorch-
+00001a00: 6d65 7472 6963 2d6c 6561 726e 696e 6729  metric-learning)
+00001a10: 206f 6620 7573 696e 6720 7468 656d 2077   of using them w
+00001a20: 6974 6820 4f4d 4c2e 0a49 6e69 7469 616c  ith OML..Initial
+00001a30: 6c79 2c20 7765 2074 7269 6564 2074 6f20  ly, we tried to 
+00001a40: 7573 6520 504d 4c2c 2062 7574 2069 6e20  use PML, but in 
+00001a50: 7468 6520 656e 642c 2077 6520 6361 6d65  the end, we came
+00001a60: 2075 7020 7769 7468 206f 7572 206c 6962   up with our lib
+00001a70: 7261 7279 2c20 7768 6963 6820 6973 206d  rary, which is m
+00001a80: 6f72 6520 7069 7065 6c69 6e65 202f 2072  ore pipeline / r
+00001a90: 6563 6970 6573 206f 7269 656e 7465 642e  ecipes oriented.
+00001aa0: 0a54 6861 7420 6973 2068 6f77 204f 4d4c  .That is how OML
+00001ab0: 2064 6966 6665 7273 2066 726f 6d20 504d   differs from PM
+00001ac0: 4c3a 0a0a 2a20 4f4d 4c20 6861 7320 5b50  L:..* OML has [P
+00001ad0: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
+00001ae0: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00001af0: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00001b00: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+00001b10: 6d61 696e 2f70 6970 656c 696e 6573 290a  main/pipelines).
+00001b20: 2020 7768 6963 6820 616c 6c6f 7773 2074    which allows t
+00001b30: 7261 696e 696e 6720 6d6f 6465 6c73 2062  raining models b
+00001b40: 7920 7072 6570 6172 696e 6720 6120 636f  y preparing a co
+00001b50: 6e66 6967 2061 6e64 2079 6f75 7220 6461  nfig and your da
+00001b60: 7461 2069 6e20 7468 6520 7265 7175 6972  ta in the requir
+00001b70: 6564 2066 6f72 6d61 740a 2020 2869 7427  ed format.  (it'
+00001b80: 7320 6c69 6b65 2063 6f6e 7665 7274 696e  s like convertin
+00001b90: 6720 6461 7461 2069 6e74 6f20 434f 434f  g data into COCO
+00001ba0: 2066 6f72 6d61 7420 746f 2074 7261 696e   format to train
+00001bb0: 2061 2064 6574 6563 746f 7220 6672 6f6d   a detector from
+00001bc0: 205b 6d6d 6465 7465 6374 696f 6e5d 2868   [mmdetection](h
+00001bd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001be0: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d64  m/open-mmlab/mmd
+00001bf0: 6574 6563 7469 6f6e 2929 2e0a 0a2a 204f  etection))...* O
+00001c00: 4d4c 2066 6f63 7573 6573 206f 6e20 656e  ML focuses on en
+00001c10: 642d 746f 2d65 6e64 2070 6970 656c 696e  d-to-end pipelin
+00001c20: 6573 2061 6e64 2070 7261 6374 6963 616c  es and practical
+00001c30: 2075 7365 2063 6173 6573 2e0a 2020 4974   use cases..  It
+00001c40: 2068 6173 2063 6f6e 6669 6720 6261 7365   has config base
+00001c50: 6420 6578 616d 706c 6573 206f 6e20 706f  d examples on po
+00001c60: 7075 6c61 7220 6265 6e63 686d 6172 6b73  pular benchmarks
+00001c70: 2063 6c6f 7365 2074 6f20 7265 616c 206c   close to real l
+00001c80: 6966 6520 286c 696b 6520 7068 6f74 6f73  ife (like photos
+00001c90: 206f 6620 7072 6f64 7563 7473 206f 6620   of products of 
+00001ca0: 7468 6f75 7361 6e64 7320 6964 7329 2e0a  thousands ids)..
+00001cb0: 2020 5765 2066 6f75 6e64 2073 6f6d 6520    We found some 
+00001cc0: 676f 6f64 2063 6f6d 6269 6e61 7469 6f6e  good combination
+00001cd0: 7320 6f66 2068 7970 6572 7061 7261 6d65  s of hyperparame
+00001ce0: 7465 7273 206f 6e20 7468 6573 6520 6461  ters on these da
+00001cf0: 7461 7365 7473 2c20 7472 6169 6e65 6420  tasets, trained 
+00001d00: 616e 6420 7075 626c 6973 6865 6420 6d6f  and published mo
+00001d10: 6465 6c73 2061 6e64 2074 6865 6972 2063  dels and their c
+00001d20: 6f6e 6669 6773 2e0a 2020 5468 7573 2c20  onfigs..  Thus, 
+00001d30: 6974 206d 616b 6573 204f 4d4c 206d 6f72  it makes OML mor
+00001d40: 6520 7265 6369 7065 7320 6f72 6965 6e74  e recipes orient
+00001d50: 6564 2074 6861 6e20 504d 4c2c 2061 6e64  ed than PML, and
+00001d60: 2069 7473 2061 7574 686f 720a 2020 5b63   its author.  [c
+00001d70: 6f6e 6669 726d 735d 2868 7474 7073 3a2f  onfirms](https:/
+00001d80: 2f67 6974 6875 622e 636f 6d2f 4b65 7669  /github.com/Kevi
+00001d90: 6e4d 7573 6772 6176 652f 7079 746f 7263  nMusgrave/pytorc
+00001da0: 682d 6d65 7472 6963 2d6c 6561 726e 696e  h-metric-learnin
+00001db0: 672f 6973 7375 6573 2f31 3639 2369 7373  g/issues/169#iss
+00001dc0: 7565 636f 6d6d 656e 742d 3637 3038 3134  uecomment-670814
+00001dd0: 3339 3329 0a20 2074 6869 7320 7361 7969  393).  this sayi
+00001de0: 6e67 2074 6861 7420 6869 7320 6c69 6272  ng that his libr
+00001df0: 6172 7920 6973 2061 2073 6574 206f 6620  ary is a set of 
+00001e00: 746f 6f6c 7320 7261 7468 6572 2074 6865  tools rather the
+00001e10: 2072 6563 6970 6573 2c20 6d6f 7265 6f76   recipes, moreov
+00001e20: 6572 2c20 7468 6520 6578 616d 706c 6573  er, the examples
+00001e30: 2069 6e20 504d 4c20 6172 6520 6d6f 7374   in PML are most
+00001e40: 6c79 2066 6f72 2043 4946 4152 2061 6e64  ly for CIFAR and
+00001e50: 204d 4e49 5354 2064 6174 6173 6574 732e   MNIST datasets.
+00001e60: 0a0a 2a20 4f4d 4c20 6861 7320 7468 6520  ..* OML has the 
+00001e70: 5b5a 6f6f 5d28 6874 7470 733a 2f2f 6769  [Zoo](https://gi
+00001e80: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
+00001e90: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
+00001ea0: 6172 6e69 6e67 237a 6f6f 2920 6f66 2070  arning#zoo) of p
+00001eb0: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
+00001ec0: 2074 6861 7420 6361 6e20 6265 2065 6173   that can be eas
+00001ed0: 696c 7920 6163 6365 7373 6564 2066 726f  ily accessed fro
+00001ee0: 6d0a 2020 7468 6520 636f 6465 2069 6e20  m.  the code in 
+00001ef0: 7468 6520 7361 6d65 2077 6179 2061 7320  the same way as 
+00001f00: 696e 2060 746f 7263 6876 6973 696f 6e60  in `torchvision`
+00001f10: 2028 7768 656e 2079 6f75 2074 7970 6520   (when you type 
+00001f20: 6072 6573 6e65 7435 3028 7072 6574 7261  `resnet50(pretra
+00001f30: 696e 6564 3d54 7275 6529 6029 2e0a 0a2a  ined=True)`)...*
+00001f40: 204f 4d4c 2069 7320 696e 7465 6772 6174   OML is integrat
+00001f50: 6564 2077 6974 6820 5b50 7954 6f72 6368  ed with [PyTorch
+00001f60: 204c 6967 6874 6e69 6e67 5d28 6874 7470   Lightning](http
+00001f70: 733a 2f2f 7777 772e 7079 746f 7263 686c  s://www.pytorchl
+00001f80: 6967 6874 6e69 6e67 2e61 692f 292c 2073  ightning.ai/), s
+00001f90: 6f2c 2077 6520 6361 6e20 7573 6520 7468  o, we can use th
+00001fa0: 6520 706f 7765 7220 6f66 2069 7473 0a20  e power of its. 
+00001fb0: 205b 5472 6169 6e65 725d 2868 7474 7073   [Trainer](https
+00001fc0: 3a2f 2f70 7974 6f72 6368 2d6c 6967 6874  ://pytorch-light
+00001fd0: 6e69 6e67 2e72 6561 6474 6865 646f 6373  ning.readthedocs
+00001fe0: 2e69 6f2f 656e 2f73 7461 626c 652f 636f  .io/en/stable/co
+00001ff0: 6d6d 6f6e 2f74 7261 696e 6572 2e68 746d  mmon/trainer.htm
+00002000: 6c29 2e0a 2020 5468 6973 2069 7320 6573  l)..  This is es
+00002010: 7065 6369 616c 6c79 2068 656c 7066 756c  pecially helpful
+00002020: 2077 6865 6e20 7765 2077 6f72 6b20 7769   when we work wi
+00002030: 7468 2044 4450 2c20 736f 2c20 796f 7520  th DDP, so, you 
+00002040: 636f 6d70 6172 6520 6f75 720a 2020 5b44  compare our.  [D
+00002050: 4450 2065 7861 6d70 6c65 5d28 6874 7470  DP example](http
+00002060: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00002070: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00002080: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00002090: 742f 6578 616d 706c 6573 2f70 7974 686f  t/examples/pytho
+000020a0: 6e2e 6874 6d6c 290a 2020 616e 6420 7468  n.html).  and th
+000020b0: 650a 2020 5b50 4d4c 7320 6f6e 655d 2868  e.  [PMLs one](h
+000020c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000020d0: 6d2f 4b65 7669 6e4d 7573 6772 6176 652f  m/KevinMusgrave/
+000020e0: 7079 746f 7263 682d 6d65 7472 6963 2d6c  pytorch-metric-l
+000020f0: 6561 726e 696e 672f 626c 6f62 2f6d 6173  earning/blob/mas
+00002100: 7465 722f 6578 616d 706c 6573 2f6e 6f74  ter/examples/not
+00002110: 6562 6f6f 6b73 2f44 6973 7472 6962 7574  ebooks/Distribut
+00002120: 6564 5472 6970 6c65 744d 6172 6769 6e4c  edTripletMarginL
+00002130: 6f73 734d 4e49 5354 2e69 7079 6e62 292e  ossMNIST.ipynb).
+00002140: 0a20 2042 7920 7468 6520 7761 792c 2050  .  By the way, P
+00002150: 4d4c 2061 6c73 6f20 6861 7320 5b54 7261  ML also has [Tra
+00002160: 696e 6572 735d 2868 7474 7073 3a2f 2f6b  iners](https://k
+00002170: 6576 696e 6d75 7367 7261 7665 2e67 6974  evinmusgrave.git
+00002180: 6875 622e 696f 2f70 7974 6f72 6368 2d6d  hub.io/pytorch-m
+00002190: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+000021a0: 7261 696e 6572 732f 292c 2062 7574 2069  rainers/), but i
+000021b0: 7427 7320 6e6f 740a 2020 7769 6465 6c79  t's not.  widely
+000021c0: 2075 7365 6420 696e 2074 6865 2065 7861   used in the exa
+000021d0: 6d70 6c65 7320 616e 6420 6375 7374 6f6d  mples and custom
+000021e0: 2060 7472 6169 6e60 202f 2060 7465 7374   `train` / `test
+000021f0: 6020 6675 6e63 7469 6f6e 7320 6172 6520  ` functions are 
+00002200: 7573 6564 2069 6e73 7465 6164 2e0a 0a57  used instead...W
+00002210: 6520 6265 6c69 6576 6520 7468 6174 2068  e believe that h
+00002220: 6176 696e 6720 5069 7065 6c69 6e65 732c  aving Pipelines,
+00002230: 206c 6163 6f6e 6963 2065 7861 6d70 6c65   laconic example
+00002240: 732c 2061 6e64 205a 6f6f 206f 6620 7072  s, and Zoo of pr
+00002250: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
+00002260: 7365 7473 2074 6865 2065 6e74 7279 2074  sets the entry t
+00002270: 6872 6573 686f 6c64 2074 6f20 6120 7265  hreshold to a re
+00002280: 616c 6c79 206c 6f77 2076 616c 7565 2e0a  ally low value..
+00002290: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
+000022a0: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
+000022b0: 6d6d 6172 793e 5768 6174 2069 7320 4d65  mmary>What is Me
+000022c0: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
+000022d0: 7375 6d6d 6172 793e 0a3c 703e 0a0a 4d65  summary>.<p>..Me
+000022e0: 7472 6963 204c 6561 726e 696e 6720 7072  tric Learning pr
+000022f0: 6f62 6c65 6d20 2861 6c73 6f20 6b6e 6f77  oblem (also know
+00002300: 6e20 6173 202a 6578 7472 656d 6520 636c  n as *extreme cl
+00002310: 6173 7369 6669 6361 7469 6f6e 2a20 7072  assification* pr
+00002320: 6f62 6c65 6d29 206d 6561 6e73 2061 2073  oblem) means a s
+00002330: 6974 7561 7469 6f6e 2069 6e20 7768 6963  ituation in whic
+00002340: 6820 7765 0a68 6176 6520 7468 6f75 7361  h we.have thousa
+00002350: 6e64 7320 6f66 2069 6473 206f 6620 736f  nds of ids of so
+00002360: 6d65 2065 6e74 6974 6965 732c 2062 7574  me entities, but
+00002370: 206f 6e6c 7920 6120 6665 7720 7361 6d70   only a few samp
+00002380: 6c65 7320 666f 7220 6576 6572 7920 656e  les for every en
+00002390: 7469 7479 2e0a 4f66 7465 6e20 7765 2061  tity..Often we a
+000023a0: 7373 756d 6520 7468 6174 2064 7572 696e  ssume that durin
+000023b0: 6720 7468 6520 7465 7374 2073 7461 6765  g the test stage
+000023c0: 2028 6f72 2070 726f 6475 6374 696f 6e29   (or production)
+000023d0: 2077 6520 7769 6c6c 2064 6561 6c20 7769   we will deal wi
+000023e0: 7468 2075 6e73 6565 6e20 656e 7469 7469  th unseen entiti
+000023f0: 6573 0a77 6869 6368 206d 616b 6573 2069  es.which makes i
+00002400: 7420 696d 706f 7373 6962 6c65 2074 6f20  t impossible to 
+00002410: 6170 706c 7920 7468 6520 7661 6e69 6c6c  apply the vanill
+00002420: 6120 636c 6173 7369 6669 6361 7469 6f6e  a classification
+00002430: 2070 6970 656c 696e 6520 6469 7265 6374   pipeline direct
+00002440: 6c79 2e20 496e 206d 616e 7920 6361 7365  ly. In many case
+00002450: 7320 6f62 7461 696e 6564 2065 6d62 6564  s obtained embed
+00002460: 6469 6e67 730a 6172 6520 7573 6564 2074  dings.are used t
+00002470: 6f20 7065 7266 6f72 6d20 7365 6172 6368  o perform search
+00002480: 206f 7220 6d61 7463 6869 6e67 2070 726f   or matching pro
+00002490: 6365 6475 7265 7320 6f76 6572 2074 6865  cedures over the
+000024a0: 6d2e 0a0a 4865 7265 2061 7265 2061 2066  m...Here are a f
+000024b0: 6577 2065 7861 6d70 6c65 7320 6f66 2073  ew examples of s
+000024c0: 7563 6820 7461 736b 7320 6672 6f6d 2074  uch tasks from t
+000024d0: 6865 2063 6f6d 7075 7465 7220 7669 7369  he computer visi
+000024e0: 6f6e 2073 7068 6572 653a 0a2a 2050 6572  on sphere:.* Per
+000024f0: 736f 6e2f 416e 696d 616c 2052 652d 4964  son/Animal Re-Id
+00002500: 656e 7469 6669 6361 7469 6f6e 0a2a 2046  entification.* F
+00002510: 6163 6520 5265 636f 676e 6974 696f 6e0a  ace Recognition.
+00002520: 2a20 4c61 6e64 6d61 726b 2052 6563 6f67  * Landmark Recog
+00002530: 6e69 7469 6f6e 0a2a 2053 6561 7263 6869  nition.* Searchi
+00002540: 6e67 2065 6e67 696e 6573 2066 6f72 206f  ng engines for o
+00002550: 6e6c 696e 6520 7368 6f70 730a 2061 6e64  nline shops. and
+00002560: 206d 616e 7920 6f74 6865 7273 2e0a 3c2f   many others..</
+00002570: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
+00002580: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+00002590: 7279 3e47 6c6f 7373 6172 7920 284e 616d  ry>Glossary (Nam
+000025a0: 696e 6720 636f 6e76 656e 7469 6f6e 2920  ing convention) 
+000025b0: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+000025c0: 2a20 6065 6d62 6564 6469 6e67 6020 2d20  * `embedding` - 
+000025d0: 6d6f 6465 6c27 7320 6f75 7470 7574 2028  model's output (
+000025e0: 616c 736f 206b 6e6f 776e 2061 7320 6066  also known as `f
+000025f0: 6561 7475 7265 7320 7665 6374 6f72 6020  eatures vector` 
+00002600: 6f72 2060 6465 7363 7269 7074 6f72 6029  or `descriptor`)
+00002610: 2e0a 2a20 6071 7565 7279 6020 2d20 6120  ..* `query` - a 
+00002620: 7361 6d70 6c65 2077 6869 6368 2069 7320  sample which is 
+00002630: 7573 6564 2061 7320 6120 7265 7175 6573  used as a reques
+00002640: 7420 696e 2074 6865 2072 6574 7269 6576  t in the retriev
+00002650: 616c 2070 726f 6365 6475 7265 2e0a 2a20  al procedure..* 
+00002660: 6067 616c 6c65 7279 2073 6574 6020 2d20  `gallery set` - 
+00002670: 7468 6520 7365 7420 6f66 2065 6e74 6974  the set of entit
+00002680: 6965 7320 746f 2073 6561 7263 6820 6974  ies to search it
+00002690: 656d 7320 7369 6d69 6c61 7220 746f 2060  ems similar to `
+000026a0: 7175 6572 7960 2028 616c 736f 206b 6e6f  query` (also kno
+000026b0: 776e 2061 7320 6072 6566 6572 656e 6365  wn as `reference
+000026c0: 6020 6f72 2060 696e 6465 7860 292e 0a2a  ` or `index`)..*
+000026d0: 2060 5361 6d70 6c65 7260 202d 2061 6e20   `Sampler` - an 
+000026e0: 6172 6775 6d65 6e74 2066 6f72 2060 4461  argument for `Da
+000026f0: 7461 4c6f 6164 6572 6020 7768 6963 6820  taLoader` which 
+00002700: 6973 2075 7365 6420 746f 2066 6f72 6d20  is used to form 
+00002710: 6261 7463 6865 730a 2a20 604d 696e 6572  batches.* `Miner
+00002720: 6020 2d20 7468 6520 6f62 6a65 6374 2074  ` - the object t
+00002730: 6f20 666f 726d 2070 6169 7273 206f 7220  o form pairs or 
+00002740: 7472 6970 6c65 7473 2061 6674 6572 2074  triplets after t
+00002750: 6865 2062 6174 6368 2077 6173 2066 6f72  he batch was for
+00002760: 6d65 6420 6279 2060 5361 6d70 6c65 7260  med by `Sampler`
+00002770: 2e20 4974 2773 206e 6f74 206e 6563 6573  . It's not neces
+00002780: 7361 7279 2074 6f20 666f 726d 0a20 2074  sary to form.  t
+00002790: 6865 2063 6f6d 6269 6e61 7469 6f6e 7320  he combinations 
+000027a0: 6f66 2073 616d 706c 6573 206f 6e6c 7920  of samples only 
+000027b0: 696e 7369 6465 2074 6865 2063 7572 7265  inside the curre
+000027c0: 6e74 2062 6174 6368 2c20 7468 7573 2c20  nt batch, thus, 
+000027d0: 7468 6520 6d65 6d6f 7279 2062 616e 6b20  the memory bank 
+000027e0: 6d61 7920 6265 2061 2070 6172 7420 6f66  may be a part of
+000027f0: 2060 4d69 6e65 7260 2e0a 2a20 6053 616d   `Miner`..* `Sam
+00002800: 706c 6573 602f 604c 6162 656c 7360 2f60  ples`/`Labels`/`
+00002810: 496e 7374 616e 6365 7360 202d 2061 7320  Instances` - as 
+00002820: 616e 2065 7861 6d70 6c65 206c 6574 2773  an example let's
+00002830: 2063 6f6e 7369 6465 7220 4465 6570 4661   consider DeepFa
+00002840: 7368 696f 6e20 6461 7461 7365 742e 2049  shion dataset. I
+00002850: 7420 696e 636c 7564 6573 2074 686f 7573  t includes thous
+00002860: 616e 6473 206f 660a 2020 6661 7368 696f  ands of.  fashio
+00002870: 6e20 6974 656d 2069 6473 2028 7765 206e  n item ids (we n
+00002880: 616d 6520 7468 656d 2060 6c61 6265 6c73  ame them `labels
+00002890: 6029 2061 6e64 2073 6576 6572 616c 2070  `) and several p
+000028a0: 686f 746f 7320 666f 7220 6561 6368 2069  hotos for each i
+000028b0: 7465 6d20 6964 0a20 2028 7765 206e 616d  tem id.  (we nam
+000028c0: 6520 7468 6520 696e 6469 7669 6475 616c  e the individual
+000028d0: 2070 686f 746f 2061 7320 6069 6e73 7461   photo as `insta
+000028e0: 6e63 6560 206f 7220 6073 616d 706c 6560  nce` or `sample`
+000028f0: 292e 2041 6c6c 206f 6620 7468 6520 6661  ). All of the fa
+00002900: 7368 696f 6e20 6974 656d 2069 6473 2068  shion item ids h
+00002910: 6176 6520 7468 6569 7220 6772 6f75 7073  ave their groups
+00002920: 206c 696b 650a 2020 2273 6b69 7274 7322   like.  "skirts"
+00002930: 2c20 226a 6163 6b65 7473 222c 2022 7368  , "jackets", "sh
+00002940: 6f72 7473 2220 616e 6420 736f 206f 6e20  orts" and so on 
+00002950: 2877 6520 6e61 6d65 2074 6865 6d20 6063  (we name them `c
+00002960: 6174 6567 6f72 6965 7360 292e 0a20 204e  ategories`)..  N
+00002970: 6f74 652c 2077 6520 6176 6f69 6420 7573  ote, we avoid us
+00002980: 696e 6720 7468 6520 7465 726d 2060 636c  ing the term `cl
+00002990: 6173 7360 2074 6f20 6176 6f69 6420 6d69  ass` to avoid mi
+000029a0: 7375 6e64 6572 7374 616e 6469 6e67 2e0a  sunderstanding..
+000029b0: 2a20 6074 7261 696e 696e 6720 6570 6f63  * `training epoc
+000029c0: 6860 202d 2062 6174 6368 2073 616d 706c  h` - batch sampl
+000029d0: 6572 7320 7768 6963 6820 7765 2075 7365  ers which we use
+000029e0: 2066 6f72 2063 6f6d 6269 6e61 7469 6f6e   for combination
+000029f0: 2d62 6173 6564 206c 6f73 7365 7320 7573  -based losses us
+00002a00: 7561 6c6c 7920 6861 7665 2061 206c 656e  ually have a len
+00002a10: 6774 6820 6571 7561 6c20 746f 0a20 2060  gth equal to.  `
+00002a20: 5b6e 756d 6265 7220 6f66 206c 6162 656c  [number of label
+00002a30: 7320 696e 2074 7261 696e 696e 6720 6461  s in training da
+00002a40: 7461 7365 745d 202f 205b 6e75 6d62 6572  taset] / [number
+00002a50: 7320 6f66 206c 6162 656c 7320 696e 206f  s of labels in o
+00002a60: 6e65 2062 6174 6368 5d60 2e20 4974 206d  ne batch]`. It m
+00002a70: 6561 6e73 2074 6861 7420 7765 2064 6f6e  eans that we don
+00002a80: 2774 206f 6273 6572 7665 2061 6c6c 206f  't observe all o
+00002a90: 660a 2020 7468 6520 6176 6169 6c61 626c  f.  the availabl
+00002aa0: 6520 7472 6169 6e69 6e67 2073 616d 706c  e training sampl
+00002ab0: 6573 2069 6e20 6f6e 6520 6570 6f63 6820  es in one epoch 
+00002ac0: 2861 7320 6f70 706f 7365 6420 746f 2076  (as opposed to v
+00002ad0: 616e 696c 6c61 2063 6c61 7373 6966 6963  anilla classific
+00002ae0: 6174 696f 6e29 2c0a 2020 696e 7374 6561  ation),.  instea
+00002af0: 642c 2077 6520 6f62 7365 7276 6520 616c  d, we observe al
+00002b00: 6c20 6f66 2074 6865 2061 7661 696c 6162  l of the availab
+00002b10: 6c65 206c 6162 656c 732e 0a0a 3c2f 703e  le labels...</p>
+00002b20: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
+00002b30: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00002b40: 3e48 6f77 2067 6f6f 6420 6d61 7920 6265  >How good may be
+00002b50: 2061 206d 6f64 656c 2074 7261 696e 6564   a model trained
+00002b60: 2077 6974 6820 4f4d 4c3f 203c 2f73 756d   with OML? </sum
+00002b70: 6d61 7279 3e0a 3c70 3e0a 0a49 7420 6d61  mary>.<p>..It ma
+00002b80: 7920 6265 2063 6f6d 7061 7261 626c 6520  y be comparable 
+00002b90: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
+00002ba0: 2028 3230 3232 2079 6561 7229 205b 536f   (2022 year) [So
+00002bb0: 7441 5d28 6874 7470 733a 2f2f 7061 7065  tA](https://pape
+00002bc0: 7273 7769 7468 636f 6465 2e63 6f6d 2f74  rswithcode.com/t
+00002bd0: 6173 6b2f 6d65 7472 6963 2d6c 6561 726e  ask/metric-learn
+00002be0: 696e 6729 206d 6574 686f 6473 2c0a 666f  ing) methods,.fo
+00002bf0: 7220 6578 616d 706c 652c 205b 4879 702d  r example, [Hyp-
+00002c00: 5669 545d 2868 7474 7073 3a2f 2f61 7278  ViT](https://arx
+00002c10: 6976 2e6f 7267 2f70 6466 2f32 3230 332e  iv.org/pdf/2203.
+00002c20: 3130 3833 332e 7064 6629 2e0a 2a28 4665  10833.pdf)..*(Fe
+00002c30: 7720 776f 7264 7320 6162 6f75 7420 7468  w words about th
+00002c40: 6973 2061 7070 726f 6163 683a 2069 7427  is approach: it'
+00002c50: 7320 6120 5669 5420 6172 6368 6974 6563  s a ViT architec
+00002c60: 7475 7265 2074 7261 696e 6564 2077 6974  ture trained wit
+00002c70: 6820 636f 6e74 7261 7374 6976 6520 6c6f  h contrastive lo
+00002c80: 7373 2c0a 6275 7420 7468 6520 656d 6265  ss,.but the embe
+00002c90: 6464 696e 6773 2077 6572 6520 7072 6f6a  ddings were proj
+00002ca0: 6563 7465 6420 696e 746f 2073 6f6d 6520  ected into some 
+00002cb0: 6879 7065 7262 6f6c 6963 2073 7061 6365  hyperbolic space
+00002cc0: 2e0a 4173 2074 6865 2061 7574 686f 7273  ..As the authors
+00002cd0: 2063 6c61 696d 6564 2c20 7375 6368 2061   claimed, such a
+00002ce0: 2073 7061 6365 2069 7320 6162 6c65 2074   space is able t
+00002cf0: 6f20 6465 7363 7269 6265 2074 6865 206e  o describe the n
+00002d00: 6573 7465 6420 7374 7275 6374 7572 6520  ested structure 
+00002d10: 6f66 2072 6561 6c2d 776f 726c 6420 6461  of real-world da
+00002d20: 7461 2e0a 536f 2c20 7468 6520 7061 7065  ta..So, the pape
+00002d30: 7220 7265 7175 6972 6573 2073 6f6d 6520  r requires some 
+00002d40: 6865 6176 7920 6d61 7468 2074 6f20 6164  heavy math to ad
+00002d50: 6170 7420 7468 6520 7573 7561 6c20 6f70  apt the usual op
+00002d60: 6572 6174 696f 6e73 2066 6f72 2074 6865  erations for the
+00002d70: 2068 7970 6572 626f 6c69 6361 6c20 7370   hyperbolical sp
+00002d80: 6163 652e 292a 0a0a 5765 2074 7261 696e  ace.)*..We train
+00002d90: 6564 2074 6865 2073 616d 6520 6172 6368  ed the same arch
+00002da0: 6974 6563 7475 7265 2077 6974 6820 7472  itecture with tr
+00002db0: 6970 6c65 7420 6c6f 7373 2c20 6669 7869  iplet loss, fixi
+00002dc0: 6e67 2074 6865 2072 6573 7420 6f66 2074  ng the rest of t
+00002dd0: 6865 2070 6172 616d 6574 6572 733a 0a74  he parameters:.t
+00002de0: 7261 696e 696e 6720 616e 6420 7465 7374  raining and test
+00002df0: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+00002e00: 2c20 696d 6167 6520 7369 7a65 2c20 616e  , image size, an
+00002e10: 6420 6f70 7469 6d69 7a65 722e 2053 6565  d optimizer. See
+00002e20: 2063 6f6e 6669 6773 2069 6e20 5b4d 6f64   configs in [Mod
+00002e30: 656c 7320 5a6f 6f5d 2868 7474 7073 3a2f  els Zoo](https:/
+00002e40: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+00002e50: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+00002e60: 2d6c 6561 726e 696e 6723 7a6f 6f29 2e0a  -learning#zoo)..
+00002e70: 5468 6520 7472 6963 6b20 7761 7320 696e  The trick was in
+00002e80: 2068 6575 7269 7374 6963 7320 696e 206f   heuristics in o
+00002e90: 7572 206d 696e 6572 2061 6e64 2073 616d  ur miner and sam
+00002ea0: 706c 6572 3a0a 0a2a 205b 4361 7465 676f  pler:..* [Catego
+00002eb0: 7279 2042 616c 616e 6365 2053 616d 706c  ry Balance Sampl
+00002ec0: 6572 5d28 6874 7470 733a 2f2f 6f70 656e  er](https://open
+00002ed0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00002ee0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002ef0: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
+00002f00: 7473 2f73 616d 706c 6572 732e 6874 6d6c  ts/samplers.html
+00002f10: 2363 6174 6567 6f72 7962 616c 616e 6365  #categorybalance
+00002f20: 7361 6d70 6c65 7229 0a20 2066 6f72 6d73  sampler).  forms
+00002f30: 2074 6865 2062 6174 6368 6573 206c 696d   the batches lim
+00002f40: 6974 696e 6720 7468 6520 6e75 6d62 6572  iting the number
+00002f50: 206f 6620 6361 7465 676f 7269 6573 202a   of categories *
+00002f60: 432a 2069 6e20 6974 2e0a 2020 466f 7220  C* in it..  For 
+00002f70: 696e 7374 616e 6365 2c20 7768 656e 202a  instance, when *
+00002f80: 4320 3d20 312a 2069 7420 7075 7473 206f  C = 1* it puts o
+00002f90: 6e6c 7920 6a61 636b 6574 7320 696e 206f  nly jackets in o
+00002fa0: 6e65 2062 6174 6368 2061 6e64 206f 6e6c  ne batch and onl
+00002fb0: 7920 6a65 616e 7320 696e 746f 2061 6e6f  y jeans into ano
+00002fc0: 7468 6572 206f 6e65 2028 6a75 7374 2061  ther one (just a
+00002fd0: 6e20 6578 616d 706c 6529 2e0a 2020 4974  n example)..  It
+00002fe0: 2061 7574 6f6d 6174 6963 616c 6c79 206d   automatically m
+00002ff0: 616b 6573 2074 6865 206e 6567 6174 6976  akes the negativ
+00003000: 6520 7061 6972 7320 6861 7264 6572 3a20  e pairs harder: 
+00003010: 6974 2773 206d 6f72 6520 6d65 616e 696e  it's more meanin
+00003020: 6766 756c 2066 6f72 2061 206d 6f64 656c  gful for a model
+00003030: 2074 6f20 7265 616c 6973 6520 7768 7920   to realise why 
+00003040: 7477 6f20 6a61 636b 6574 730a 2020 6172  two jackets.  ar
+00003050: 6520 6469 6666 6572 656e 7420 7468 616e  e different than
+00003060: 2074 6f20 756e 6465 7273 7461 6e64 2074   to understand t
+00003070: 6865 2073 616d 6520 6162 6f75 7420 6120  he same about a 
+00003080: 6a61 636b 6574 2061 6e64 2061 2074 2d73  jacket and a t-s
+00003090: 6869 7274 2e0a 0a2a 205b 4861 7264 2054  hirt...* [Hard T
+000030a0: 7269 706c 6574 7320 4d69 6e65 725d 2868  riplets Miner](h
+000030b0: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+000030c0: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+000030d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000030e0: 7465 7374 2f63 6f6e 7465 6e74 732f 6d69  test/contents/mi
+000030f0: 6e65 7273 2e68 746d 6c23 6861 7264 7472  ners.html#hardtr
+00003100: 6970 6c65 7473 6d69 6e65 7229 0a20 206d  ipletsminer).  m
+00003110: 616b 6573 2074 6865 2074 6173 6b20 6576  akes the task ev
+00003120: 656e 2068 6172 6465 7220 6b65 6570 696e  en harder keepin
+00003130: 6720 6f6e 6c79 2074 6865 2068 6172 6465  g only the harde
+00003140: 7374 2074 7269 706c 6574 7320 2877 6974  st triplets (wit
+00003150: 6820 6d61 7869 6d61 6c20 706f 7369 7469  h maximal positi
+00003160: 7665 2061 6e64 206d 696e 696d 616c 206e  ve and minimal n
+00003170: 6567 6174 6976 6520 6469 7374 616e 6365  egative distance
+00003180: 7329 2e0a 0a48 6572 6520 6172 6520 2a43  s)...Here are *C
+00003190: 4d43 4031 2a20 7363 6f72 6573 2066 6f72  MC@1* scores for
+000031a0: 2032 2070 6f70 756c 6172 2062 656e 6368   2 popular bench
+000031b0: 6d61 726b 732e 0a53 4f50 2064 6174 6173  marks..SOP datas
+000031c0: 6574 3a20 4879 702d 5669 5420 e280 9420  et: Hyp-ViT ... 
+000031d0: 3835 2e39 2c20 6f75 7273 20e2 8094 2038  85.9, ours ... 8
+000031e0: 362e 362e 2044 6565 7046 6173 6869 6f6e  6.6. DeepFashion
+000031f0: 2064 6174 6173 6574 3a20 4879 702d 5669   dataset: Hyp-Vi
+00003200: 5420 e280 9420 3932 2e35 2c20 6f75 7273  T ... 92.5, ours
+00003210: 20e2 8094 2039 322e 312e 0a54 6875 732c   ... 92.1..Thus,
+00003220: 2075 7469 6c69 7369 6e67 2073 696d 706c   utilising simpl
+00003230: 6520 6865 7572 6973 7469 6373 2061 6e64  e heuristics and
+00003240: 2061 766f 6964 696e 6720 6865 6176 7920   avoiding heavy 
+00003250: 6d61 7468 2077 6520 6172 6520 6162 6c65  math we are able
+00003260: 2074 6f20 7065 7266 6f72 6d20 6f6e 2053   to perform on S
+00003270: 6f74 4120 6c65 7665 6c2e 0a0a 3c2f 703e  otA level...</p>
+00003280: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00003290: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+000032a0: 5768 6174 2061 626f 7574 2053 656c 662d  What about Self-
+000032b0: 5375 7065 7276 6973 6564 204c 6561 726e  Supervised Learn
+000032c0: 696e 673f 3c2f 7375 6d6d 6172 793e 0a3c  ing?</summary>.<
+000032d0: 703e 0a0a 5265 6365 6e74 2072 6573 6561  p>..Recent resea
+000032e0: 7263 6820 696e 2053 534c 2064 6566 696e  rch in SSL defin
+000032f0: 6974 656c 7920 6f62 7461 696e 6564 2067  itely obtained g
+00003300: 7265 6174 2072 6573 756c 7473 2e20 5468  reat results. Th
+00003310: 6520 7072 6f62 6c65 6d20 6973 2074 6861  e problem is tha
+00003320: 7420 7468 6573 6520 6170 7072 6f61 6368  t these approach
+00003330: 6573 0a72 6571 7569 7265 6420 616e 2065  es.required an e
+00003340: 6e6f 726d 6f75 7320 616d 6f75 6e74 206f  normous amount o
+00003350: 6620 636f 6d70 7574 696e 6720 746f 2074  f computing to t
+00003360: 7261 696e 2074 6865 206d 6f64 656c 2e20  rain the model. 
+00003370: 4275 7420 696e 206f 7572 2066 7261 6d65  But in our frame
+00003380: 776f 726b 2c20 7765 2063 6f6e 7369 6465  work, we conside
+00003390: 7220 7468 6520 6d6f 7374 2063 6f6d 6d6f  r the most commo
+000033a0: 6e20 6361 7365 0a77 6865 6e20 7468 6520  n case.when the 
+000033b0: 6176 6572 6167 6520 7573 6572 2068 6173  average user has
+000033c0: 206e 6f20 6d6f 7265 2074 6861 6e20 6120   no more than a 
+000033d0: 6665 7720 4750 5573 2e0a 0a41 7420 7468  few GPUs...At th
+000033e0: 6520 7361 6d65 2074 696d 652c 2069 7420  e same time, it 
+000033f0: 776f 756c 6420 6265 2075 6e77 6973 6520  would be unwise 
+00003400: 746f 2069 676e 6f72 6520 7375 6363 6573  to ignore succes
+00003410: 7320 696e 2074 6869 7320 7370 6865 7265  s in this sphere
+00003420: 2c20 736f 2077 6520 7374 696c 6c20 6578  , so we still ex
+00003430: 706c 6f69 7420 6974 2069 6e20 7477 6f20  ploit it in two 
+00003440: 7761 7973 3a0a 2a20 4173 2061 2073 6f75  ways:.* As a sou
+00003450: 7263 6520 6f66 2063 6865 636b 706f 696e  rce of checkpoin
+00003460: 7473 2074 6861 7420 776f 756c 6420 6265  ts that would be
+00003470: 2067 7265 6174 2074 6f20 7374 6172 7420   great to start 
+00003480: 7472 6169 6e69 6e67 2077 6974 682e 2046  training with. F
+00003490: 726f 6d20 7075 626c 6963 6174 696f 6e73  rom publications
+000034a0: 2061 6e64 206f 7572 2065 7870 6572 6965   and our experie
+000034b0: 6e63 652c 0a20 2074 6865 7920 6172 6520  nce,.  they are 
+000034c0: 6d75 6368 2062 6574 7465 7220 6173 2069  much better as i
+000034d0: 6e69 7469 616c 6973 6174 696f 6e20 7468  nitialisation th
+000034e0: 616e 2074 6865 2064 6566 6175 6c74 2073  an the default s
+000034f0: 7570 6572 7669 7365 6420 6d6f 6465 6c20  upervised model 
+00003500: 7472 6169 6e65 6420 6f6e 2049 6d61 6765  trained on Image
+00003510: 4e65 742e 2054 6875 732c 2077 6520 6164  Net. Thus, we ad
+00003520: 6465 6420 7468 6520 706f 7373 6962 696c  ded the possibil
+00003530: 6974 790a 2020 746f 2069 6e69 7469 616c  ity.  to initial
+00003540: 6973 6520 796f 7572 206d 6f64 656c 7320  ise your models 
+00003550: 7573 696e 6720 7468 6573 6520 7072 6574  using these pret
+00003560: 7261 696e 6564 2063 6865 636b 706f 696e  rained checkpoin
+00003570: 7473 206f 6e6c 7920 6279 2070 6173 7369  ts only by passi
+00003580: 6e67 2061 6e20 6172 6775 6d65 6e74 2069  ng an argument i
+00003590: 6e20 7468 6520 636f 6e66 6967 206f 7220  n the config or 
+000035a0: 7468 6520 636f 6e73 7472 7563 746f 722e  the constructor.
+000035b0: 0a2a 2041 7320 6120 736f 7572 6365 206f  .* As a source o
+000035c0: 6620 696e 7370 6972 6174 696f 6e2e 2046  f inspiration. F
+000035d0: 6f72 2065 7861 6d70 6c65 2c20 7765 2061  or example, we a
+000035e0: 6461 7074 6564 2074 6865 2069 6465 6120  dapted the idea 
+000035f0: 6f66 2061 206d 656d 6f72 7920 6261 6e6b  of a memory bank
+00003600: 2066 726f 6d20 2a4d 6f43 6f2a 2066 6f72   from *MoCo* for
+00003610: 2074 6865 202a 5472 6970 6c65 744c 6f73   the *TripletLos
+00003620: 732a 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461  s*...</p>.</deta
+00003630: 696c 733e 0a0a 0a3c 6465 7461 696c 733e  ils>...<details>
+00003640: 0a3c 7375 6d6d 6172 793e 446f 2049 206e  .<summary>Do I n
+00003650: 6565 6420 746f 206b 6e6f 7720 6f74 6865  eed to know othe
+00003660: 7220 6672 616d 6577 6f72 6b73 2074 6f20  r frameworks to 
+00003670: 7573 6520 4f4d 4c3f 3c2f 7375 6d6d 6172  use OML?</summar
+00003680: 793e 0a3c 703e 0a0a 4e6f 2c20 796f 7520  y>.<p>..No, you 
+00003690: 646f 6e27 742e 204f 4d4c 2069 7320 6120  don't. OML is a 
+000036a0: 6672 616d 6577 6f72 6b2d 6167 6e6f 7374  framework-agnost
+000036b0: 6963 2e20 4465 7370 6974 6520 7765 2075  ic. Despite we u
+000036c0: 7365 2050 7954 6f72 6368 204c 6967 6874  se PyTorch Light
+000036d0: 6e69 6e67 2061 7320 6120 6c6f 6f70 0a72  ning as a loop.r
+000036e0: 756e 6e65 7220 666f 7220 7468 6520 6578  unner for the ex
+000036f0: 7065 7269 6d65 6e74 732c 2077 6520 616c  periments, we al
+00003700: 736f 206b 6565 7020 7468 6520 706f 7373  so keep the poss
+00003710: 6962 696c 6974 7920 746f 2072 756e 2065  ibility to run e
+00003720: 7665 7279 7468 696e 6720 6f6e 2070 7572  verything on pur
+00003730: 6520 5079 546f 7263 682e 0a54 6875 732c  e PyTorch..Thus,
+00003740: 206f 6e6c 7920 7468 6520 7469 6e79 2070   only the tiny p
+00003750: 6172 7420 6f66 204f 4d4c 2069 7320 4c69  art of OML is Li
+00003760: 6768 746e 696e 672d 7370 6563 6966 6963  ghtning-specific
+00003770: 2061 6e64 2077 6520 6b65 6570 2074 6869   and we keep thi
+00003780: 7320 6c6f 6769 6320 7365 7061 7261 7465  s logic separate
+00003790: 6c79 2066 726f 6d0a 6f74 6865 7220 636f  ly from.other co
+000037a0: 6465 2028 7365 6520 606f 6d6c 2e6c 6967  de (see `oml.lig
+000037b0: 6874 6e69 6e67 6029 2e20 4576 656e 2077  htning`). Even w
+000037c0: 6865 6e20 796f 7520 7573 6520 4c69 6768  hen you use Ligh
+000037d0: 746e 696e 672c 2079 6f75 2064 6f6e 2774  tning, you don't
+000037e0: 206e 6565 6420 746f 206b 6e6f 7720 6974   need to know it
+000037f0: 2c20 7369 6e63 650a 7765 2070 726f 7669  , since.we provi
+00003800: 6465 2072 6561 6479 2074 6f20 7573 6520  de ready to use 
+00003810: 5b50 6970 656c 696e 6573 5d28 6874 7470  [Pipelines](http
+00003820: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+00003830: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+00003840: 7269 632d 6c65 6172 6e69 6e67 2f62 6c6f  ric-learning/blo
+00003850: 622f 6d61 696e 2f70 6970 656c 696e 6573  b/main/pipelines
+00003860: 2f29 2e0a 0a54 6865 2070 6f73 7369 6269  /)...The possibi
+00003870: 6c69 7479 206f 6620 7573 696e 6720 7075  lity of using pu
+00003880: 7265 2050 7954 6f72 6368 2061 6e64 206d  re PyTorch and m
+00003890: 6f64 756c 6172 2073 7472 7563 7475 7265  odular structure
+000038a0: 206f 6620 7468 6520 636f 6465 206c 6561   of the code lea
+000038b0: 7665 7320 6120 726f 6f6d 2066 6f72 2075  ves a room for u
+000038c0: 7469 6c69 7a69 6e67 0a4f 4d4c 2077 6974  tilizing.OML wit
+000038d0: 6820 796f 7572 2066 6176 6f75 7269 7465  h your favourite
+000038e0: 2066 7261 6d65 776f 726b 2061 6674 6572   framework after
+000038f0: 2074 6865 2069 6d70 6c65 6d65 6e74 6174   the implementat
+00003900: 696f 6e20 6f66 2074 6865 206e 6563 6573  ion of the neces
+00003910: 7361 7279 2077 7261 7070 6572 732e 0a0a  sary wrappers...
+00003920: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
+00003930: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
+00003940: 6d61 7279 3e43 616e 2049 2075 7365 204f  mary>Can I use O
+00003950: 4d4c 2077 6974 686f 7574 2061 6e79 206b  ML without any k
+00003960: 6e6f 776c 6564 6765 2069 6e20 4461 7461  nowledge in Data
+00003970: 5363 6965 6e63 653f 3c2f 7375 6d6d 6172  Science?</summar
+00003980: 793e 0a3c 703e 0a0a 5965 732e 2054 6f20  y>.<p>..Yes. To 
+00003990: 7275 6e20 7468 6520 6578 7065 7269 6d65  run the experime
+000039a0: 6e74 2077 6974 6820 5b50 6970 656c 696e  nt with [Pipelin
+000039b0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+000039c0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
+000039d0: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+000039e0: 6e69 6e67 2f62 6c6f 622f 6d61 696e 2f70  ning/blob/main/p
+000039f0: 6970 656c 696e 6573 2f29 0a79 6f75 206f  ipelines/).you o
+00003a00: 6e6c 7920 6e65 6564 2074 6f20 7772 6974  nly need to writ
+00003a10: 6520 6120 636f 6e76 6572 7465 720a 746f  e a converter.to
+00003a20: 206f 7572 2066 6f72 6d61 7420 2869 7420   our format (it 
+00003a30: 6d65 616e 7320 7072 6570 6172 696e 6720  means preparing 
+00003a40: 7468 650a 602e 6373 7660 2074 6162 6c65  the.`.csv` table
+00003a50: 2077 6974 6820 3520 7072 6564 6566 696e   with 5 predefin
+00003a60: 6564 2063 6f6c 756d 6e73 292e 0a54 6861  ed columns)..Tha
+00003a70: 7427 7320 6974 210a 0a50 726f 6261 626c  t's it!..Probabl
+00003a80: 7920 7765 2061 6c72 6561 6479 2068 6176  y we already hav
+00003a90: 6520 6120 7375 6974 6162 6c65 2070 7265  e a suitable pre
+00003aa0: 2d74 7261 696e 6564 206d 6f64 656c 2066  -trained model f
+00003ab0: 6f72 2079 6f75 7220 646f 6d61 696e 0a69  or your domain.i
+00003ac0: 6e20 6f75 7220 2a4d 6f64 656c 7320 5a6f  n our *Models Zo
+00003ad0: 6f2a 2e20 496e 2074 6869 7320 6361 7365  o*. In this case
+00003ae0: 2c20 796f 7520 646f 6e27 7420 6576 656e  , you don't even
+00003af0: 206e 6565 6420 746f 2074 7261 696e 2069   need to train i
+00003b00: 742e 0a3c 2f70 3e0a 3c2f 6465 7461 696c  t..</p>.</detail
+00003b10: 733e 0a0a 2323 205b 446f 6375 6d65 6e74  s>..## [Document
+00003b20: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+00003b30: 7065 6e2d 6d65 7472 6963 2d6c 6561 726e  pen-metric-learn
+00003b40: 696e 672e 7265 6164 7468 6564 6f63 732e  ing.readthedocs.
+00003b50: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
+00003b60: 6578 2e68 746d 6c29 0a0a 446f 6375 6d65  ex.html)..Docume
+00003b70: 6e74 6174 696f 6e20 6973 2061 7661 696c  ntation is avail
+00003b80: 6162 6c65 2076 6961 2074 6865 205b 6c69  able via the [li
+00003b90: 6e6b 5d28 6874 7470 733a 2f2f 6f70 656e  nk](https://open
+00003ba0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00003bb0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003bc0: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
+00003bd0: 6874 6d6c 292e 0a0a 596f 7520 6361 6e20  html)...You can 
+00003be0: 616c 736f 2072 6561 6420 736f 6d65 2065  also read some e
+00003bf0: 7874 7261 206d 6174 6572 6961 6c73 2072  xtra materials r
+00003c00: 656c 6174 6564 2074 6f20 4f4d 4c3a 0a0a  elated to OML:..
+00003c10: 2a20 5468 656f 7279 2061 6e64 2070 7261  * Theory and pra
+00003c20: 6374 6963 6520 6f66 206d 6574 7269 6320  ctice of metric 
+00003c30: 6c65 6172 6e69 6e67 2077 6974 6820 7468  learning with th
+00003c40: 6520 7573 6167 6520 6f66 204f 4d4c 2e0a  e usage of OML..
+00003c50: 5b50 6f73 7420 696e 2045 6e67 6c69 7368  [Post in English
+00003c60: 206f 6e20 4d65 6469 756d 5d28 6874 7470   on Medium](http
+00003c70: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f40  s://medium.com/@
+00003c80: 416c 656b 7365 6953 6861 6261 6e6f 762f  AlekseiShabanov/
+00003c90: 7072 6163 7469 6361 6c2d 6d65 7472 6963  practical-metric
+00003ca0: 2d6c 6561 726e 696e 672d 6230 3431 3063  -learning-b0410c
+00003cb0: 6461 3232 3031 2920 7c0a 5b50 6f73 7420  da2201) |.[Post 
+00003cc0: 696e 2052 7573 7369 616e 206f 6e20 4861  in Russian on Ha
+00003cd0: 6272 5d28 6874 7470 733a 2f2f 6861 6272  br](https://habr
+00003ce0: 2e63 6f6d 2f72 752f 636f 6d70 616e 792f  .com/ru/company/
+00003cf0: 6f64 732f 626c 6f67 2f36 3935 3338 302f  ods/blog/695380/
+00003d00: 2920 7c0a 5b50 6f73 7420 696e 2043 6869  ) |.[Post in Chi
+00003d10: 6e65 7365 206f 6e20 4353 444e 5d28 6874  nese on CSDN](ht
+00003d20: 7470 733a 2f2f 626c 6f67 2e63 7364 6e2e  tps://blog.csdn.
+00003d30: 6e65 742f 6665 726d 696f 6e30 3231 372f  net/fermion0217/
+00003d40: 6172 7469 636c 652f 6465 7461 696c 732f  article/details/
+00003d50: 3132 3739 3332 3038 3729 2c20 7472 616e  127932087), tran
+00003d60: 736c 6174 6564 2062 7920 4368 6961 2d43  slated by Chia-C
+00003d70: 6865 6e20 4368 616e 672e 0a0a 2a20 5468  hen Chang...* Th
+00003d80: 650a 5b44 454d 4f5d 2868 7474 7073 3a2f  e.[DEMO](https:/
+00003d90: 2f64 6170 6c61 646f 632d 6f6d 6c2d 706f  /dapladoc-oml-po
+00003da0: 7374 7072 6f63 6573 7369 6e67 2d64 656d  stprocessing-dem
+00003db0: 6f2d 7372 6361 7070 6d61 696e 2d70 6668  o-srcappmain-pfh
+00003dc0: 3267 302e 7374 7265 616d 6c69 742e 6170  2g0.streamlit.ap
+00003dd0: 702f 290a 666f 7220 6f75 7220 7061 7065  p/).for our pape
+00003de0: 720a 5b53 5449 523a 2053 6961 6d65 7365  r.[STIR: Siamese
+00003df0: 2054 7261 6e73 666f 726d 6572 7320 666f   Transformers fo
+00003e00: 7220 496d 6167 6520 5265 7472 6965 7661  r Image Retrieva
+00003e10: 6c20 506f 7374 7072 6f63 6573 7369 6e67  l Postprocessing
+00003e20: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00003e30: 6f72 672f 6162 732f 3233 3034 2e31 3333  org/abs/2304.133
+00003e40: 3933 290a 0a2a 2054 6865 2072 6570 6f72  93)..* The repor
+00003e50: 7420 666f 7220 4265 726c 696e 2d62 6173  t for Berlin-bas
+00003e60: 6564 206d 6565 7475 703a 2022 436f 6d70  ed meetup: "Comp
+00003e70: 7574 6572 2056 6973 696f 6e20 696e 2070  uter Vision in p
+00003e80: 726f 6475 6374 696f 6e22 2e20 4e6f 7665  roduction". Nove
+00003e90: 6d62 6572 2c20 3230 3232 2e0a 5b4c 696e  mber, 2022..[Lin
+00003ea0: 6b5d 2868 7474 7073 3a2f 2f64 7269 7665  k](https://drive
+00003eb0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00003ec0: 652f 666f 6c64 6572 732f 3175 486d 4c55  e/folders/1uHmLU
+00003ed0: 3876 4d72 4d56 4d46 6f64 7433 3675 3075  8vMrMVMFodt36u0u
+00003ee0: 5841 6759 6a47 5f33 4433 303f 7573 703d  XAgYjG_3D30?usp=
+00003ef0: 7368 6172 655f 6c69 6e6b 290a 0a23 2320  share_link)..## 
+00003f00: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2868  [Installation](h
+00003f10: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+00003f20: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+00003f30: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00003f40: 7465 7374 2f6f 6d6c 2f69 6e73 7461 6c6c  test/oml/install
+00003f50: 6174 696f 6e2e 6874 6d6c 290a 0a4f 4d4c  ation.html)..OML
+00003f60: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
+00003f70: 2050 7950 493a 0a0a 6060 6073 6865 6c6c   PyPI:..```shell
+00003f80: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00003f90: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00003fa0: 6e69 6e67 0a60 6060 0a0a 596f 7520 6361  ning.```..You ca
+00003fb0: 6e20 616c 736f 2070 756c 6c20 7468 6520  n also pull the 
+00003fc0: 7072 6570 6172 6564 2069 6d61 6765 2066  prepared image f
+00003fd0: 726f 6d20 446f 636b 6572 4875 622e 2e2e  rom DockerHub...
+00003fe0: 0a0a 6060 6073 6865 6c6c 0a64 6f63 6b65  ..```shell.docke
+00003ff0: 7220 7075 6c6c 206f 6d6c 7465 616d 2f6f  r pull omlteam/o
+00004000: 6d6c 3a67 7075 0a64 6f63 6b65 7220 7075  ml:gpu.docker pu
+00004010: 6c6c 206f 6d6c 7465 616d 2f6f 6d6c 3a63  ll omlteam/oml:c
+00004020: 7075 0a60 6060 0a0a 2e2e 2e6f 7220 6275  pu.```.....or bu
+00004030: 696c 6420 6f6e 6520 6279 2079 6f75 7220  ild one by your 
+00004040: 6f77 6e0a 0a60 6060 7368 656c 6c0a 6d61  own..```shell.ma
+00004050: 6b65 2064 6f63 6b65 725f 6275 696c 6420  ke docker_build 
+00004060: 5255 4e54 494d 453d 6370 750a 6d61 6b65  RUNTIME=cpu.make
+00004070: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
+00004080: 4e54 494d 453d 6770 750a 6060 600a 0a23  NTIME=gpu.```..#
+00004090: 2320 5b45 7861 6d70 6c65 735d 2868 7474  # [Examples](htt
+000040a0: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
+000040b0: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
+000040c0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000040d0: 7374 2f66 6561 7475 7265 5f65 7874 7261  st/feature_extra
+000040e0: 6374 696f 6e2f 7079 7468 6f6e 5f65 7861  ction/python_exa
+000040f0: 6d70 6c65 732e 6874 6d6c 2329 0a0a 3c64  mples.html#)..<d
+00004100: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00004110: 3e54 7261 696e 696e 673c 2f73 756d 6d61  >Training</summa
+00004120: 7279 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e  ry>.<p>..[commen
+00004130: 745d 3a76 616e 696c 6c61 2d74 7261 696e  t]:vanilla-train
+00004140: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
+00004150: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
+00004160: 6f6d 2074 7164 6d20 696d 706f 7274 2074  om tqdm import t
+00004170: 7164 6d0a 0a66 726f 6d20 6f6d 6c2e 6461  qdm..from oml.da
+00004180: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00004190: 7274 2044 6174 6173 6574 5769 7468 4c61  rt DatasetWithLa
+000041a0: 6265 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f  bels.from oml.lo
+000041b0: 7373 6573 2e74 7269 706c 6574 2069 6d70  sses.triplet imp
+000041c0: 6f72 7420 5472 6970 6c65 744c 6f73 7357  ort TripletLossW
+000041d0: 6974 684d 696e 6572 0a66 726f 6d20 6f6d  ithMiner.from om
+000041e0: 6c2e 6d69 6e65 7273 2e69 6e62 6174 6368  l.miners.inbatch
+000041f0: 5f61 6c6c 5f74 7269 2069 6d70 6f72 7420  _all_tri import 
+00004200: 416c 6c54 7269 706c 6574 734d 696e 6572  AllTripletsMiner
+00004210: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
+00004220: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
+00004230: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7361  ctor.from oml.sa
+00004240: 6d70 6c65 7273 2e62 616c 616e 6365 2069  mplers.balance i
+00004250: 6d70 6f72 7420 4261 6c61 6e63 6553 616d  mport BalanceSam
+00004260: 706c 6572 0a66 726f 6d20 6f6d 6c2e 7574  pler.from oml.ut
+00004270: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
+00004280: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
+00004290: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
+000042a0: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
+000042b0: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
+000042c0: 6173 6574 2f22 0a64 665f 7472 6169 6e2c  aset/".df_train,
+000042d0: 205f 203d 2064 6f77 6e6c 6f61 645f 6d6f   _ = download_mo
+000042e0: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+000042f0: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+00004300: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00004310: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+00004320: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+00004330: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+00004340: 7265 733d 4661 6c73 6529 2e74 7261 696e  res=False).train
+00004350: 2829 0a6f 7074 696d 697a 6572 203d 2074  ().optimizer = t
+00004360: 6f72 6368 2e6f 7074 696d 2e53 4744 2865  orch.optim.SGD(e
+00004370: 7874 7261 6374 6f72 2e70 6172 616d 6574  xtractor.paramet
+00004380: 6572 7328 292c 206c 723d 3165 2d36 290a  ers(), lr=1e-6).
+00004390: 0a74 7261 696e 5f64 6174 6173 6574 203d  .train_dataset =
+000043a0: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
+000043b0: 6c73 2864 665f 7472 6169 6e2c 2064 6174  ls(df_train, dat
+000043c0: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+000043d0: 745f 726f 6f74 290a 6372 6974 6572 696f  t_root).criterio
+000043e0: 6e20 3d20 5472 6970 6c65 744c 6f73 7357  n = TripletLossW
+000043f0: 6974 684d 696e 6572 286d 6172 6769 6e3d  ithMiner(margin=
+00004400: 302e 312c 206d 696e 6572 3d41 6c6c 5472  0.1, miner=AllTr
+00004410: 6970 6c65 7473 4d69 6e65 7228 292c 206e  ipletsMiner(), n
+00004420: 6565 645f 6c6f 6773 3d54 7275 6529 0a73  eed_logs=True).s
+00004430: 616d 706c 6572 203d 2042 616c 616e 6365  ampler = Balance
+00004440: 5361 6d70 6c65 7228 7472 6169 6e5f 6461  Sampler(train_da
+00004450: 7461 7365 742e 6765 745f 6c61 6265 6c73  taset.get_labels
+00004460: 2829 2c20 6e5f 6c61 6265 6c73 3d32 2c20  (), n_labels=2, 
+00004470: 6e5f 696e 7374 616e 6365 733d 3229 0a74  n_instances=2).t
+00004480: 7261 696e 5f6c 6f61 6465 7220 3d20 746f  rain_loader = to
+00004490: 7263 682e 7574 696c 732e 6461 7461 2e44  rch.utils.data.D
+000044a0: 6174 614c 6f61 6465 7228 7472 6169 6e5f  ataLoader(train_
+000044b0: 6461 7461 7365 742c 2062 6174 6368 5f73  dataset, batch_s
+000044c0: 616d 706c 6572 3d73 616d 706c 6572 290a  ampler=sampler).
+000044d0: 0a66 6f72 2062 6174 6368 2069 6e20 7471  .for batch in tq
+000044e0: 646d 2874 7261 696e 5f6c 6f61 6465 7229  dm(train_loader)
+000044f0: 3a0a 2020 2020 656d 6265 6464 696e 6773  :.    embeddings
+00004500: 203d 2065 7874 7261 6374 6f72 2862 6174   = extractor(bat
+00004510: 6368 5b22 696e 7075 745f 7465 6e73 6f72  ch["input_tensor
+00004520: 7322 5d29 0a20 2020 206c 6f73 7320 3d20  s"]).    loss = 
+00004530: 6372 6974 6572 696f 6e28 656d 6265 6464  criterion(embedd
+00004540: 696e 6773 2c20 6261 7463 685b 226c 6162  ings, batch["lab
+00004550: 656c 7322 5d29 0a20 2020 206c 6f73 732e  els"]).    loss.
+00004560: 6261 636b 7761 7264 2829 0a20 2020 206f  backward().    o
+00004570: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00004580: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
+00004590: 726f 5f67 7261 6428 290a 0a20 2020 2023  ro_grad()..    #
+000045a0: 2069 6e66 6f20 666f 7220 6c6f 6767 696e   info for loggin
+000045b0: 673a 2070 6f73 6974 6976 652f 6e65 6761  g: positive/nega
+000045c0: 7469 7665 2064 6973 7461 6e63 6573 2c20  tive distances, 
+000045d0: 6e75 6d62 6572 206f 6620 6163 7469 7665  number of active
+000045e0: 2074 7269 706c 6574 730a 2020 2020 7072   triplets.    pr
+000045f0: 696e 7428 6372 6974 6572 696f 6e2e 6c61  int(criterion.la
+00004600: 7374 5f6c 6f67 7329 0a0a 6060 600a 5b63  st_logs)..```.[c
+00004610: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+00004620: 7472 6169 6e2d 656e 640a 3c2f 703e 0a3c  train-end.</p>.<
+00004630: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+00004640: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+00004650: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004660: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+00004670: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+00004680: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00004690: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+000046a0: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+000046b0: 316b 6e74 4441 4964 495a 394c 3430 6a63  1kntDAIdIZ9L40jc
+000046c0: 6e64 6775 4c41 622d 5871 6d43 464f 6753  ndguLAb-XqmCFOgS
+000046d0: 353f 7573 703d 7368 6172 696e 6729 0a3c  5?usp=sharing).<
+000046e0: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+000046f0: 793e 5661 6c69 6461 7469 6f6e 3c2f 7375  y>Validation</su
+00004700: 6d6d 6172 793e 0a3c 703e 0a0a 5b63 6f6d  mmary>.<p>..[com
+00004710: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
+00004720: 6c69 6461 7469 6f6e 2d73 7461 7274 0a60  lidation-start.`
+00004730: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00004740: 746f 7263 680a 6672 6f6d 2074 7164 6d20  torch.from tqdm 
+00004750: 696d 706f 7274 2074 7164 6d0a 0a66 726f  import tqdm..fro
+00004760: 6d20 6f6d 6c2e 6461 7461 7365 7473 2e62  m oml.datasets.b
+00004770: 6173 6520 696d 706f 7274 2044 6174 6173  ase import Datas
+00004780: 6574 5175 6572 7947 616c 6c65 7279 0a66  etQueryGallery.f
+00004790: 726f 6d20 6f6d 6c2e 6d65 7472 6963 732e  rom oml.metrics.
+000047a0: 656d 6265 6464 696e 6773 2069 6d70 6f72  embeddings impor
+000047b0: 7420 456d 6265 6464 696e 674d 6574 7269  t EmbeddingMetri
+000047c0: 6373 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  cs.from oml.mode
+000047d0: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+000047e0: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+000047f0: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+00004800: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004810: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004820: 5f64 6174 6173 6574 0a0a 6461 7461 7365  _dataset..datase
+00004830: 745f 726f 6f74 203d 2022 6d6f 636b 5f64  t_root = "mock_d
+00004840: 6174 6173 6574 2f22 0a5f 2c20 6466 5f76  ataset/"._, df_v
+00004850: 616c 203d 2064 6f77 6e6c 6f61 645f 6d6f  al = download_mo
+00004860: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+00004870: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+00004880: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00004890: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+000048a0: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+000048b0: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+000048c0: 7265 733d 4661 6c73 6529 2e65 7661 6c28  res=False).eval(
+000048d0: 290a 0a76 616c 5f64 6174 6173 6574 203d  )..val_dataset =
+000048e0: 2044 6174 6173 6574 5175 6572 7947 616c   DatasetQueryGal
+000048f0: 6c65 7279 2864 665f 7661 6c2c 2064 6174  lery(df_val, dat
+00004900: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+00004910: 745f 726f 6f74 290a 0a76 616c 5f6c 6f61  t_root)..val_loa
+00004920: 6465 7220 3d20 746f 7263 682e 7574 696c  der = torch.util
+00004930: 732e 6461 7461 2e44 6174 614c 6f61 6465  s.data.DataLoade
+00004940: 7228 7661 6c5f 6461 7461 7365 742c 2062  r(val_dataset, b
+00004950: 6174 6368 5f73 697a 653d 3429 0a63 616c  atch_size=4).cal
+00004960: 6375 6c61 746f 7220 3d20 456d 6265 6464  culator = Embedd
+00004970: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+00004980: 5f6b 6579 733d 2822 7061 7468 7322 2c29  _keys=("paths",)
+00004990: 290a 6361 6c63 756c 6174 6f72 2e73 6574  ).calculator.set
+000049a0: 7570 286e 756d 5f73 616d 706c 6573 3d6c  up(num_samples=l
+000049b0: 656e 2876 616c 5f64 6174 6173 6574 2929  en(val_dataset))
+000049c0: 0a0a 7769 7468 2074 6f72 6368 2e6e 6f5f  ..with torch.no_
+000049d0: 6772 6164 2829 3a0a 2020 2020 666f 7220  grad():.    for 
+000049e0: 6261 7463 6820 696e 2074 7164 6d28 7661  batch in tqdm(va
+000049f0: 6c5f 6c6f 6164 6572 293a 0a20 2020 2020  l_loader):.     
+00004a00: 2020 2062 6174 6368 5b22 656d 6265 6464     batch["embedd
+00004a10: 696e 6773 225d 203d 2065 7874 7261 6374  ings"] = extract
+00004a20: 6f72 2862 6174 6368 5b22 696e 7075 745f  or(batch["input_
+00004a30: 7465 6e73 6f72 7322 5d29 0a20 2020 2020  tensors"]).     
+00004a40: 2020 2063 616c 6375 6c61 746f 722e 7570     calculator.up
+00004a50: 6461 7465 5f64 6174 6128 6261 7463 6829  date_data(batch)
+00004a60: 0a0a 6d65 7472 6963 7320 3d20 6361 6c63  ..metrics = calc
+00004a70: 756c 6174 6f72 2e63 6f6d 7075 7465 5f6d  ulator.compute_m
+00004a80: 6574 7269 6373 2829 0a0a 2320 4c6f 6767  etrics()..# Logg
+00004a90: 696e 670a 7072 696e 7428 6361 6c63 756c  ing.print(calcul
+00004aa0: 6174 6f72 2e6d 6574 7269 6373 2920 2023  ator.metrics)  #
+00004ab0: 206d 6574 7269 6373 0a70 7269 6e74 2863   metrics.print(c
+00004ac0: 616c 6375 6c61 746f 722e 6d65 7472 6963  alculator.metric
+00004ad0: 735f 756e 7265 6475 6365 6429 2020 2320  s_unreduced)  # 
+00004ae0: 6d65 7472 6963 7320 7769 7468 6f75 7420  metrics without 
+00004af0: 6176 6572 6167 696e 6720 6f76 6572 2071  averaging over q
+00004b00: 7565 7269 6573 0a0a 2320 5669 7375 616c  ueries..# Visual
+00004b10: 6973 6174 696f 6e0a 6361 6c63 756c 6174  isation.calculat
+00004b20: 6f72 2e67 6574 5f70 6c6f 745f 666f 725f  or.get_plot_for_
+00004b30: 7175 6572 6965 7328 7175 6572 795f 6964  queries(query_id
+00004b40: 733d 5b30 2c20 325d 2c20 6e5f 696e 7374  s=[0, 2], n_inst
+00004b50: 616e 6365 733d 3529 2020 2320 6472 6177  ances=5)  # draw
+00004b60: 2070 7265 6469 6374 696f 6e73 206f 6e20   predictions on 
+00004b70: 7072 6564 6566 696e 6564 2071 7565 7269  predefined queri
+00004b80: 6573 0a63 616c 6375 6c61 746f 722e 6765  es.calculator.ge
+00004b90: 745f 706c 6f74 5f66 6f72 5f77 6f72 7374  t_plot_for_worst
+00004ba0: 5f71 7565 7269 6573 286d 6574 7269 635f  _queries(metric_
+00004bb0: 6e61 6d65 3d22 4f56 4552 414c 4c2f 6d61  name="OVERALL/ma
+00004bc0: 702f 3522 2c20 6e5f 7175 6572 6965 733d  p/5", n_queries=
+00004bd0: 322c 206e 5f69 6e73 7461 6e63 6573 3d35  2, n_instances=5
+00004be0: 2920 2023 2064 7261 7720 6d69 7374 616b  )  # draw mistak
+00004bf0: 6573 0a63 616c 6375 6c61 746f 722e 7669  es.calculator.vi
+00004c00: 7375 616c 697a 6528 2920 2023 2064 7261  sualize()  # dra
+00004c10: 7720 6d69 7374 616b 6573 2066 6f72 2061  w mistakes for a
+00004c20: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+00004c30: 206d 6574 7269 6373 0a0a 6060 600a 5b63   metrics..```.[c
+00004c40: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+00004c50: 7661 6c69 6461 7469 6f6e 2d65 6e64 0a3c  validation-end.<
+00004c60: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
+00004c70: 5b21 5b4f 7065 6e20 496e 2043 6f6c 6162  [![Open In Colab
+00004c80: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00004c90: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00004ca0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00004cb0: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
+00004cc0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004cd0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
+00004ce0: 7269 7665 2f31 4f32 6f33 6b38 4938 6a4e  rive/1O2o3k8I8jN
+00004cf0: 3568 5269 6e33 644b 6e41 5333 5773 6747  5hRin3dKnAS3WsgG
+00004d00: 3034 746d 4954 3f75 7370 3d73 6861 7269  04tmIT?usp=shari
+00004d10: 6e67 290a 3c64 6574 6169 6c73 3e0a 3c73  ng).<details>.<s
+00004d20: 756d 6d61 7279 3e54 7261 696e 696e 6720  ummary>Training 
+00004d30: 2b20 5661 6c69 6461 7469 6f6e 205b 4c69  + Validation [Li
+00004d40: 6768 746e 696e 6720 616e 6420 6c6f 6767  ghtning and logg
+00004d50: 696e 675d 3c2f 7375 6d6d 6172 793e 0a3c  ing]</summary>.<
+00004d60: 703e 0a0a 5b63 6f6d 6d65 6e74 5d3a 6c69  p>..[comment]:li
+00004d70: 6768 746e 696e 672d 7374 6172 740a 6060  ghtning-start.``
+00004d80: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+00004d90: 7974 6f72 6368 5f6c 6967 6874 6e69 6e67  ytorch_lightning
+00004da0: 2061 7320 706c 0a69 6d70 6f72 7420 746f   as pl.import to
+00004db0: 7263 680a 0a66 726f 6d20 6f6d 6c2e 6461  rch..from oml.da
+00004dc0: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00004dd0: 7274 2044 6174 6173 6574 5175 6572 7947  rt DatasetQueryG
+00004de0: 616c 6c65 7279 2c20 4461 7461 7365 7457  allery, DatasetW
+00004df0: 6974 684c 6162 656c 730a 6672 6f6d 206f  ithLabels.from o
+00004e00: 6d6c 2e6c 6967 6874 6e69 6e67 2e6d 6f64  ml.lightning.mod
+00004e10: 756c 6573 2e65 7874 7261 6374 6f72 2069  ules.extractor i
+00004e20: 6d70 6f72 7420 4578 7472 6163 746f 724d  mport ExtractorM
+00004e30: 6f64 756c 650a 6672 6f6d 206f 6d6c 2e6c  odule.from oml.l
+00004e40: 6967 6874 6e69 6e67 2e63 616c 6c62 6163  ightning.callbac
+00004e50: 6b73 2e6d 6574 7269 6320 696d 706f 7274  ks.metric import
+00004e60: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+00004e70: 636b 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ck.from oml.loss
+00004e80: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
+00004e90: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
+00004ea0: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
+00004eb0: 6d65 7472 6963 732e 656d 6265 6464 696e  metrics.embeddin
+00004ec0: 6773 2069 6d70 6f72 7420 456d 6265 6464  gs import Embedd
+00004ed0: 696e 674d 6574 7269 6373 0a66 726f 6d20  ingMetrics.from 
+00004ee0: 6f6d 6c2e 6d69 6e65 7273 2e69 6e62 6174  oml.miners.inbat
+00004ef0: 6368 5f61 6c6c 5f74 7269 2069 6d70 6f72  ch_all_tri impor
+00004f00: 7420 416c 6c54 7269 706c 6574 734d 696e  t AllTripletsMin
+00004f10: 6572 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  er.from oml.mode
+00004f20: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+00004f30: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+00004f40: 7361 6d70 6c65 7273 2e62 616c 616e 6365  samplers.balance
+00004f50: 2069 6d70 6f72 7420 4261 6c61 6e63 6553   import BalanceS
+00004f60: 616d 706c 6572 0a66 726f 6d20 6f6d 6c2e  ampler.from oml.
+00004f70: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+00004f80: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004f90: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004fa0: 5f64 6174 6173 6574 0a66 726f 6d20 7079  _dataset.from py
+00004fb0: 746f 7263 685f 6c69 6768 746e 696e 672e  torch_lightning.
+00004fc0: 6c6f 6767 6572 7320 696d 706f 7274 204e  loggers import N
+00004fd0: 6570 7475 6e65 4c6f 6767 6572 2c20 5465  eptuneLogger, Te
+00004fe0: 6e73 6f72 426f 6172 644c 6f67 6765 722c  nsorBoardLogger,
+00004ff0: 2057 616e 6462 4c6f 6767 6572 0a0a 6461   WandbLogger..da
+00005000: 7461 7365 745f 726f 6f74 203d 2022 6d6f  taset_root = "mo
+00005010: 636b 5f64 6174 6173 6574 2f22 0a64 665f  ck_dataset/".df_
+00005020: 7472 6169 6e2c 2064 665f 7661 6c20 3d20  train, df_val = 
+00005030: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+00005040: 7461 7365 7428 6461 7461 7365 745f 726f  taset(dataset_ro
+00005050: 6f74 290a 0a23 206d 6f64 656c 0a65 7874  ot)..# model.ext
+00005060: 7261 6374 6f72 203d 2056 6954 4578 7472  ractor = ViTExtr
+00005070: 6163 746f 7228 2276 6974 7331 365f 6469  actor("vits16_di
+00005080: 6e6f 222c 2061 7263 683d 2276 6974 7331  no", arch="vits1
+00005090: 3622 2c20 6e6f 726d 616c 6973 655f 6665  6", normalise_fe
+000050a0: 6174 7572 6573 3d46 616c 7365 290a 0a23  atures=False)..#
+000050b0: 2074 7261 696e 0a6f 7074 696d 697a 6572   train.optimizer
+000050c0: 203d 2074 6f72 6368 2e6f 7074 696d 2e53   = torch.optim.S
+000050d0: 4744 2865 7874 7261 6374 6f72 2e70 6172  GD(extractor.par
+000050e0: 616d 6574 6572 7328 292c 206c 723d 3165  ameters(), lr=1e
+000050f0: 2d36 290a 7472 6169 6e5f 6461 7461 7365  -6).train_datase
+00005100: 7420 3d20 4461 7461 7365 7457 6974 684c  t = DatasetWithL
+00005110: 6162 656c 7328 6466 5f74 7261 696e 2c20  abels(df_train, 
+00005120: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00005130: 6173 6574 5f72 6f6f 7429 0a63 7269 7465  aset_root).crite
+00005140: 7269 6f6e 203d 2054 7269 706c 6574 4c6f  rion = TripletLo
+00005150: 7373 5769 7468 4d69 6e65 7228 6d61 7267  ssWithMiner(marg
+00005160: 696e 3d30 2e31 2c20 6d69 6e65 723d 416c  in=0.1, miner=Al
+00005170: 6c54 7269 706c 6574 734d 696e 6572 2829  lTripletsMiner()
+00005180: 290a 6261 7463 685f 7361 6d70 6c65 7220  ).batch_sampler 
+00005190: 3d20 4261 6c61 6e63 6553 616d 706c 6572  = BalanceSampler
+000051a0: 2874 7261 696e 5f64 6174 6173 6574 2e67  (train_dataset.g
+000051b0: 6574 5f6c 6162 656c 7328 292c 206e 5f6c  et_labels(), n_l
+000051c0: 6162 656c 733d 322c 206e 5f69 6e73 7461  abels=2, n_insta
+000051d0: 6e63 6573 3d33 290a 7472 6169 6e5f 6c6f  nces=3).train_lo
+000051e0: 6164 6572 203d 2074 6f72 6368 2e75 7469  ader = torch.uti
+000051f0: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+00005200: 6572 2874 7261 696e 5f64 6174 6173 6574  er(train_dataset
+00005210: 2c20 6261 7463 685f 7361 6d70 6c65 723d  , batch_sampler=
+00005220: 6261 7463 685f 7361 6d70 6c65 7229 0a0a  batch_sampler)..
+00005230: 2320 7661 6c0a 7661 6c5f 6461 7461 7365  # val.val_datase
+00005240: 7420 3d20 4461 7461 7365 7451 7565 7279  t = DatasetQuery
+00005250: 4761 6c6c 6572 7928 6466 5f76 616c 2c20  Gallery(df_val, 
+00005260: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00005270: 6173 6574 5f72 6f6f 7429 0a76 616c 5f6c  aset_root).val_l
+00005280: 6f61 6465 7220 3d20 746f 7263 682e 7574  oader = torch.ut
+00005290: 696c 732e 6461 7461 2e44 6174 614c 6f61  ils.data.DataLoa
+000052a0: 6465 7228 7661 6c5f 6461 7461 7365 742c  der(val_dataset,
+000052b0: 2062 6174 6368 5f73 697a 653d 3429 0a6d   batch_size=4).m
+000052c0: 6574 7269 635f 6361 6c6c 6261 636b 203d  etric_callback =
+000052d0: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+000052e0: 636b 286d 6574 7269 633d 456d 6265 6464  ck(metric=Embedd
+000052f0: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+00005300: 5f6b 6579 733d 5b74 7261 696e 5f64 6174  _keys=[train_dat
+00005310: 6173 6574 2e70 6174 6873 5f6b 6579 2c5d  aset.paths_key,]
+00005320: 292c 206c 6f67 5f69 6d61 6765 733d 5472  ), log_images=Tr
+00005330: 7565 290a 0a23 2031 2920 4c6f 6767 696e  ue)..# 1) Loggin
+00005340: 6720 7769 7468 2054 656e 736f 7262 6f61  g with Tensorboa
+00005350: 7264 0a6c 6f67 6765 7220 3d20 5465 6e73  rd.logger = Tens
+00005360: 6f72 426f 6172 644c 6f67 6765 7228 222e  orBoardLogger(".
+00005370: 2229 0a0a 2320 3229 204c 6f67 6769 6e67  ")..# 2) Logging
+00005380: 2077 6974 6820 4e65 7074 756e 650a 2320   with Neptune.# 
+00005390: 6c6f 6767 6572 203d 204e 6570 7475 6e65  logger = Neptune
+000053a0: 4c6f 6767 6572 2861 7069 5f6b 6579 3d22  Logger(api_key="
+000053b0: 222c 2070 726f 6a65 6374 3d22 222c 206c  ", project="", l
+000053c0: 6f67 5f6d 6f64 656c 5f63 6865 636b 706f  og_model_checkpo
+000053d0: 696e 7473 3d46 616c 7365 290a 0a23 2033  ints=False)..# 3
+000053e0: 2920 4c6f 6767 696e 6720 7769 7468 2057  ) Logging with W
+000053f0: 6569 6768 7473 2061 6e64 2042 6961 7365  eights and Biase
+00005400: 730a 2320 696d 706f 7274 206f 730a 2320  s.# import os.# 
+00005410: 6f73 2e65 6e76 6972 6f6e 5b22 5741 4e44  os.environ["WAND
+00005420: 425f 4150 495f 4b45 5922 5d20 3d20 2222  B_API_KEY"] = ""
+00005430: 0a23 206c 6f67 6765 7220 3d20 5761 6e64  .# logger = Wand
+00005440: 624c 6f67 6765 7228 7072 6f6a 6563 743d  bLogger(project=
+00005450: 2274 6573 745f 7072 6f6a 6563 7422 2c20  "test_project", 
+00005460: 6c6f 675f 6d6f 6465 6c3d 4661 6c73 6529  log_model=False)
+00005470: 0a0a 2320 7275 6e0a 706c 5f6d 6f64 656c  ..# run.pl_model
+00005480: 203d 2045 7874 7261 6374 6f72 4d6f 6475   = ExtractorModu
+00005490: 6c65 2865 7874 7261 6374 6f72 2c20 6372  le(extractor, cr
+000054a0: 6974 6572 696f 6e2c 206f 7074 696d 697a  iterion, optimiz
+000054b0: 6572 290a 7472 6169 6e65 7220 3d20 706c  er).trainer = pl
+000054c0: 2e54 7261 696e 6572 286d 6178 5f65 706f  .Trainer(max_epo
+000054d0: 6368 733d 332c 2063 616c 6c62 6163 6b73  chs=3, callbacks
+000054e0: 3d5b 6d65 7472 6963 5f63 616c 6c62 6163  =[metric_callbac
+000054f0: 6b5d 2c20 6e75 6d5f 7361 6e69 7479 5f76  k], num_sanity_v
+00005500: 616c 5f73 7465 7073 3d30 2c20 6c6f 6767  al_steps=0, logg
+00005510: 6572 3d6c 6f67 6765 7229 0a74 7261 696e  er=logger).train
+00005520: 6572 2e66 6974 2870 6c5f 6d6f 6465 6c2c  er.fit(pl_model,
+00005530: 2074 7261 696e 5f64 6174 616c 6f61 6465   train_dataloade
+00005540: 7273 3d74 7261 696e 5f6c 6f61 6465 722c  rs=train_loader,
+00005550: 2076 616c 5f64 6174 616c 6f61 6465 7273   val_dataloaders
+00005560: 3d76 616c 5f6c 6f61 6465 7229 0a0a 6060  =val_loader)..``
+00005570: 600a 5b63 6f6d 6d65 6e74 5d3a 6c69 6768  `.[comment]:ligh
+00005580: 746e 696e 672d 656e 640a 3c2f 703e 0a3c  tning-end.</p>.<
+00005590: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+000055a0: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+000055b0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000055c0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000055d0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000055e0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000055f0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00005600: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00005610: 3162 5655 6764 4247 5776 5167 436b 6261  1bVUgdBGWvQgCkba
+00005620: 3259 7461 4952 566c 5551 557a 3751 3630  2YtaIRVlUQUz7Q60
+00005630: 5a3f 7573 703d 7368 6172 655f 6c69 6e6b  Z?usp=share_link
+00005640: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
+00005650: 6d61 7279 3e55 7369 6e67 2061 2074 7261  mary>Using a tra
+00005660: 696e 6564 206d 6f64 656c 2066 6f72 2072  ined model for r
+00005670: 6574 7269 6576 616c 3c2f 7375 6d6d 6172  etrieval</summar
+00005680: 793e 0a3c 703e 0a0a 5b63 6f6d 6d65 6e74  y>.<p>..[comment
+00005690: 5d3a 7573 6167 652d 7265 7472 6965 7661  ]:usage-retrieva
+000056a0: 6c2d 7374 6172 740a 6060 6070 7974 686f  l-start.```pytho
+000056b0: 6e0a 696d 706f 7274 2074 6f72 6368 0a0a  n.import torch..
+000056c0: 6672 6f6d 206f 6d6c 2e63 6f6e 7374 2069  from oml.const i
+000056d0: 6d70 6f72 7420 4d4f 434b 5f44 4154 4153  mport MOCK_DATAS
+000056e0: 4554 5f50 4154 480a 6672 6f6d 206f 6d6c  ET_PATH.from oml
+000056f0: 2e69 6e66 6572 656e 6365 2e66 6c61 7420  .inference.flat 
+00005700: 696d 706f 7274 2069 6e66 6572 656e 6365  import inference
+00005710: 5f6f 6e5f 696d 6167 6573 0a66 726f 6d20  _on_images.from 
+00005720: 6f6d 6c2e 6d6f 6465 6c73 2069 6d70 6f72  oml.models impor
+00005730: 7420 5669 5445 7874 7261 6374 6f72 0a66  t ViTExtractor.f
+00005740: 726f 6d20 6f6d 6c2e 7265 6769 7374 7279  rom oml.registry
+00005750: 2e74 7261 6e73 666f 726d 7320 696d 706f  .transforms impo
+00005760: 7274 2067 6574 5f74 7261 6e73 666f 726d  rt get_transform
+00005770: 735f 666f 725f 7072 6574 7261 696e 6564  s_for_pretrained
+00005780: 0a66 726f 6d20 6f6d 6c2e 7574 696c 732e  .from oml.utils.
+00005790: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+000057a0: 7461 7365 7420 696d 706f 7274 2064 6f77  taset import dow
+000057b0: 6e6c 6f61 645f 6d6f 636b 5f64 6174 6173  nload_mock_datas
+000057c0: 6574 0a66 726f 6d20 6f6d 6c2e 7574 696c  et.from oml.util
+000057d0: 732e 6d69 7363 5f74 6f72 6368 2069 6d70  s.misc_torch imp
+000057e0: 6f72 7420 7061 6972 7769 7365 5f64 6973  ort pairwise_dis
+000057f0: 740a 0a5f 2c20 6466 5f76 616c 203d 2064  t.._, df_val = d
+00005800: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
+00005810: 6173 6574 284d 4f43 4b5f 4441 5441 5345  aset(MOCK_DATASE
+00005820: 545f 5041 5448 290a 6466 5f76 616c 5b22  T_PATH).df_val["
+00005830: 7061 7468 225d 203d 2064 665f 7661 6c5b  path"] = df_val[
+00005840: 2270 6174 6822 5d2e 6170 706c 7928 6c61  "path"].apply(la
+00005850: 6d62 6461 2078 3a20 4d4f 434b 5f44 4154  mbda x: MOCK_DAT
+00005860: 4153 4554 5f50 4154 4820 2f20 7829 0a71  ASET_PATH / x).q
+00005870: 7565 7269 6573 203d 2064 665f 7661 6c5b  ueries = df_val[
+00005880: 6466 5f76 616c 5b22 6973 5f71 7565 7279  df_val["is_query
+00005890: 225d 5d5b 2270 6174 6822 5d2e 746f 6c69  "]]["path"].toli
+000058a0: 7374 2829 0a67 616c 6c65 7269 6573 203d  st().galleries =
+000058b0: 2064 665f 7661 6c5b 6466 5f76 616c 5b22   df_val[df_val["
+000058c0: 6973 5f67 616c 6c65 7279 225d 5d5b 2270  is_gallery"]]["p
+000058d0: 6174 6822 5d2e 746f 6c69 7374 2829 0a0a  ath"].tolist()..
+000058e0: 6578 7472 6163 746f 7220 3d20 5669 5445  extractor = ViTE
+000058f0: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00005900: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00005910: 5f64 696e 6f22 290a 7472 616e 7366 6f72  _dino").transfor
+00005920: 6d2c 205f 203d 2067 6574 5f74 7261 6e73  m, _ = get_trans
+00005930: 666f 726d 735f 666f 725f 7072 6574 7261  forms_for_pretra
+00005940: 696e 6564 2822 7669 7473 3136 5f64 696e  ined("vits16_din
+00005950: 6f22 290a 0a61 7267 7320 3d20 7b22 6e75  o")..args = {"nu
+00005960: 6d5f 776f 726b 6572 7322 3a20 302c 2022  m_workers": 0, "
+00005970: 6261 7463 685f 7369 7a65 223a 2038 7d0a  batch_size": 8}.
+00005980: 6665 6174 7572 6573 5f71 7565 7269 6573  features_queries
+00005990: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+000059a0: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+000059b0: 2c20 7061 7468 733d 7175 6572 6965 732c  , paths=queries,
+000059c0: 2074 7261 6e73 666f 726d 3d74 7261 6e73   transform=trans
+000059d0: 666f 726d 2c20 2a2a 6172 6773 290a 6665  form, **args).fe
+000059e0: 6174 7572 6573 5f67 616c 6c65 7269 6573  atures_galleries
+000059f0: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+00005a00: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+00005a10: 2c20 7061 7468 733d 6761 6c6c 6572 6965  , paths=gallerie
+00005a20: 732c 2074 7261 6e73 666f 726d 3d74 7261  s, transform=tra
+00005a30: 6e73 666f 726d 2c20 2a2a 6172 6773 290a  nsform, **args).
+00005a40: 0a23 204e 6f77 2077 6520 6361 6e20 6578  .# Now we can ex
+00005a50: 706c 6963 6974 6c79 2062 7569 6c64 2070  plicitly build p
+00005a60: 6169 7277 6973 6520 6d61 7472 6978 206f  airwise matrix o
+00005a70: 6620 6469 7374 616e 6365 7320 6f72 2073  f distances or s
+00005a80: 6176 6520 796f 7520 5241 4d20 7669 6120  ave you RAM via 
+00005a90: 7573 696e 6720 6b4e 4e0a 7573 655f 6b6e  using kNN.use_kn
+00005aa0: 6e20 3d20 5472 7565 0a74 6f70 5f6b 203d  n = True.top_k =
+00005ab0: 2033 0a0a 6966 2075 7365 5f6b 6e6e 3a0a   3..if use_knn:.
+00005ac0: 2020 2020 6672 6f6d 2073 6b6c 6561 726e      from sklearn
+00005ad0: 2e6e 6569 6768 626f 7273 2069 6d70 6f72  .neighbors impor
+00005ae0: 7420 4e65 6172 6573 744e 6569 6768 626f  t NearestNeighbo
+00005af0: 7273 0a20 2020 206b 6e6e 203d 204e 6561  rs.    knn = Nea
+00005b00: 7265 7374 4e65 6967 6862 6f72 7328 616c  restNeighbors(al
+00005b10: 676f 7269 7468 6d3d 2261 7574 6f22 2c20  gorithm="auto", 
+00005b20: 703d 3229 0a20 2020 206b 6e6e 2e66 6974  p=2).    knn.fit
+00005b30: 2866 6561 7475 7265 735f 6761 6c6c 6572  (features_galler
+00005b40: 6965 7329 0a20 2020 2064 6973 7473 2c20  ies).    dists, 
+00005b50: 6969 5f63 6c6f 7365 7374 203d 206b 6e6e  ii_closest = knn
+00005b60: 2e6b 6e65 6967 6862 6f72 7328 6665 6174  .kneighbors(feat
+00005b70: 7572 6573 5f71 7565 7269 6573 2c20 6e5f  ures_queries, n_
+00005b80: 6e65 6967 6862 6f72 733d 746f 705f 6b2c  neighbors=top_k,
+00005b90: 2072 6574 7572 6e5f 6469 7374 616e 6365   return_distance
+00005ba0: 3d54 7275 6529 0a0a 656c 7365 3a0a 2020  =True)..else:.  
+00005bb0: 2020 6469 7374 5f6d 6174 203d 2070 6169    dist_mat = pai
+00005bc0: 7277 6973 655f 6469 7374 2878 313d 6665  rwise_dist(x1=fe
+00005bd0: 6174 7572 6573 5f71 7565 7269 6573 2c20  atures_queries, 
+00005be0: 7832 3d66 6561 7475 7265 735f 6761 6c6c  x2=features_gall
+00005bf0: 6572 6965 7329 0a20 2020 2064 6973 7473  eries).    dists
+00005c00: 2c20 6969 5f63 6c6f 7365 7374 203d 2074  , ii_closest = t
+00005c10: 6f72 6368 2e74 6f70 6b28 6469 7374 5f6d  orch.topk(dist_m
+00005c20: 6174 2c20 6469 6d3d 312c 206b 3d74 6f70  at, dim=1, k=top
+00005c30: 5f6b 2c20 6c61 7267 6573 743d 4661 6c73  _k, largest=Fals
+00005c40: 6529 0a0a 7072 696e 7428 6622 546f 7020  e)..print(f"Top 
+00005c50: 7b74 6f70 5f6b 7d20 6974 656d 7320 636c  {top_k} items cl
+00005c60: 6f73 6573 7420 746f 2071 7565 7269 6573  osest to queries
+00005c70: 2061 7265 3a5c 6e20 7b69 695f 636c 6f73   are:\n {ii_clos
+00005c80: 6573 747d 2229 0a60 6060 0a5b 636f 6d6d  est}").```.[comm
+00005c90: 656e 745d 3a75 7361 6765 2d72 6574 7269  ent]:usage-retri
+00005ca0: 6576 616c 2d65 6e64 0a3c 2f70 3e0a 3c2f  eval-end.</p>.</
+00005cb0: 6465 7461 696c 733e 0a0a 5b21 5b4f 7065  details>..[![Ope
+00005cc0: 6e20 496e 2043 6f6c 6162 5d28 6874 7470  n In Colab](http
+00005cd0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00005ce0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
+00005cf0: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
+00005d00: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+00005d10: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00005d20: 6f67 6c65 2e63 6f6d 2f64 7269 7665 2f31  ogle.com/drive/1
+00005d30: 5332 6e4b 364b 6152 6544 6d2d 526a 6a64  S2nK6KaReDm-Rjjd
+00005d40: 6f6a 6449 6436 4361 6b68 6853 7976 6641  ojdId6CakhhSyvfA
+00005d50: 3f75 7370 3d73 6861 7265 5f6c 696e 6b29  ?usp=share_link)
+00005d60: 0a0a 5b2a 2a53 6368 656d 6173 2c20 6578  ..[**Schemas, ex
+00005d70: 706c 616e 6174 696f 6e73 2061 6e64 2074  planations and t
+00005d80: 6970 732a 2a5d 2868 7474 7073 3a2f 2f67  ips**](https://g
+00005d90: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
+00005da0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
+00005db0: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
+00005dc0: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
+00005dd0: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
+00005de0: 0a0a 5365 6520 5b65 7874 7261 2063 6f64  ..See [extra cod
+00005df0: 6520 736e 6970 7065 7473 5d28 6874 7470  e snippets](http
+00005e00: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00005e10: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00005e20: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00005e30: 742f 6665 6174 7572 655f 6578 7472 6163  t/feature_extrac
+00005e40: 7469 6f6e 2f70 7974 686f 6e5f 6578 616d  tion/python_exam
+00005e50: 706c 6573 2e68 746d 6c29 2c20 696e 636c  ples.html), incl
+00005e60: 7564 696e 673a 0a2a 2054 7261 696e 696e  uding:.* Trainin
+00005e70: 6720 2b20 5661 6c69 6461 7469 6f6e 2077  g + Validation w
+00005e80: 6974 6820 4c69 6768 746e 696e 670a 2a20  ith Lightning.* 
+00005e90: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
+00005ea0: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
+00005eb0: 6e69 6e67 2069 6e20 4444 5020 6d6f 6465  ning in DDP mode
+00005ec0: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005ed0: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005ee0: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005ef0: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005f00: 2061 6476 616e 6365 6420 2870 6173 7369   advanced (passi
+00005f10: 6e67 2064 6973 7461 6e63 652c 2072 6564  ng distance, red
+00005f20: 7563 6572 2c20 6d69 6e65 7229 0a0a 2323  ucer, miner)..##
+00005f30: 205b 5069 7065 6c69 6e65 735d 2868 7474   [Pipelines](htt
+00005f40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00005f50: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
+00005f60: 7472 6963 2d6c 6561 726e 696e 672f 7472  tric-learning/tr
+00005f70: 6565 2f6d 6169 6e2f 7069 7065 6c69 6e65  ee/main/pipeline
+00005f80: 7329 0a0a 5069 7065 6c69 6e65 7320 7072  s)..Pipelines pr
+00005f90: 6f76 6964 6520 6120 7761 7920 746f 2072  ovide a way to r
+00005fa0: 756e 206d 6574 7269 6320 6c65 6172 6e69  un metric learni
+00005fb0: 6e67 2065 7870 6572 696d 656e 7473 2076  ng experiments v
+00005fc0: 6961 2063 6861 6e67 696e 6720 6f6e 6c79  ia changing only
+00005fd0: 2074 6865 2063 6f6e 6669 6720 6669 6c65   the config file
+00005fe0: 2e0a 416c 6c20 796f 7520 6e65 6564 2069  ..All you need i
+00005ff0: 7320 746f 2070 7265 7061 7265 2079 6f75  s to prepare you
+00006000: 7220 6461 7461 7365 7420 696e 2061 2072  r dataset in a r
+00006010: 6571 7569 7265 6420 666f 726d 6174 2e0a  equired format..
+00006020: 0a53 6565 205b 5069 7065 6c69 6e65 735d  .See [Pipelines]
+00006030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006040: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
+00006050: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
+00006060: 672f 626c 6f62 2f6d 6169 6e2f 7069 7065  g/blob/main/pipe
+00006070: 6c69 6e65 732f 2920 666f 6c64 6572 2066  lines/) folder f
+00006080: 6f72 206d 6f72 6520 6465 7461 696c 733a  or more details:
+00006090: 0a2a 2046 6561 7475 7265 2065 7874 7261  .* Feature extra
+000060a0: 6374 6f72 205b 7069 7065 6c69 6e65 5d28  ctor [pipeline](
+000060b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000060c0: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
+000060d0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+000060e0: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
+000060f0: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
+00006100: 7472 6163 7469 6f6e 290a 2a20 5265 7472  traction).* Retr
+00006110: 6965 7661 6c20 706f 7374 7072 6f63 6573  ieval postproces
+00006120: 736f 7220 5b70 6970 656c 696e 655d 2868  sor [pipeline](h
+00006130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00006140: 6d2f 4f4d 4c2d 5465 616d 2f6f 7065 6e2d  m/OML-Team/open-
+00006150: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
+00006160: 7472 6565 2f6d 6169 6e2f 7069 7065 6c69  tree/main/pipeli
+00006170: 6e65 732f 706f 7374 7072 6f63 6573 7369  nes/postprocessi
+00006180: 6e67 2920 2872 652d 7261 6e6b 696e 6729  ng) (re-ranking)
+00006190: 0a0a 2323 205b 5a6f 6f5d 2868 7474 7073  ..## [Zoo](https
+000061a0: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
+000061b0: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
+000061c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000061d0: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
+000061e0: 696f 6e2f 7a6f 6f2e 6874 6d6c 290a 0a42  ion/zoo.html)..B
+000061f0: 656c 6f77 2061 7265 2074 6865 206d 6f64  elow are the mod
+00006200: 656c 7320 7472 6169 6e65 6420 7769 7468  els trained with
+00006210: 204f 4d4c 206f 6e20 3420 7075 626c 6963   OML on 4 public
+00006220: 2064 6174 6173 6574 732e 0a41 6c6c 206d   datasets..All m
+00006230: 6574 7269 6373 2062 656c 6f77 2077 6572  etrics below wer
+00006240: 6520 6f62 7461 696e 6564 206f 6e20 7468  e obtained on th
+00006250: 6520 696d 6167 6573 2077 6974 6820 7468  e images with th
+00006260: 6520 7369 7a65 7320 6f66 202a 2a32 3234  e sizes of **224
+00006270: 2078 2032 3234 2a2a 3a0a 0a7c 2020 2020   x 224**:..|    
+00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006290: 2020 6d6f 6465 6c20 2020 2020 2020 2020    model         
+000062a0: 2020 2020 2020 2020 2020 2020 207c 2063               | c
+000062b0: 6d63 3120 207c 2020 2020 2020 2020 2064  mc1  |         d
+000062c0: 6174 6173 6574 2020 2020 2020 2020 2020  ataset          
+000062d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00006300: 6569 6768 7473 2020 2020 2020 2020 2020  eights          
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006360: 2020 2020 2020 2020 2065 7870 6572 696d           experim
+00006370: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 2020 2020 2020 2020 7c0a 7c3a 2d2d 2d2d          |.|:----
+000063b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000063c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000063d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+000063e0: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+000063f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00006400: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00006410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006460: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00006470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064d0: 2d2d 2d2d 2d2d 3a7c 0a7c 2060 5669 5445  ------:|.| `ViTE
+000064e0: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+000064f0: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00006500: 5f69 6e73 686f 7022 2960 207c 2030 2e39  _inshop")` | 0.9
+00006510: 3231 207c 2020 2020 4465 6570 4661 7368  21 |    DeepFash
+00006520: 696f 6e20 496e 7368 6f70 2020 2020 7c20  ion Inshop    | 
+00006530: 2020 205b 6c69 6e6b 5d28 6874 7470 733a     [link](https:
+00006540: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00006550: 6f6d 2f66 696c 652f 642f 316e 6958 2d54  om/file/d/1niX-T
+00006560: 4338 636a 366a 3336 3974 3769 5532 6261  C8cj6j369t7iU2ba
+00006570: 4851 5356 4e33 4d56 4a62 572f 7669 6577  HQSVN3MVJbW/view
+00006580: 3f75 7370 3d73 6861 7269 6e67 2920 2020  ?usp=sharing)   
+00006590: 2020 7c20 5b6c 696e 6b5d 2868 7474 7073    | [link](https
+000065a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000065b0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000065c0: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+000065d0: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+000065e0: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+000065f0: 696f 6e2f 6578 7472 6163 746f 725f 696e  ion/extractor_in
+00006600: 7368 6f70 2920 7c0a 7c20 2060 5669 5445  shop) |.|  `ViTE
+00006610: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00006620: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00006630: 5f73 6f70 2229 6020 2020 7c20 302e 3836  _sop")`   | 0.86
+00006640: 3620 7c20 5374 616e 666f 7264 204f 6e6c  6 | Stanford Onl
+00006650: 696e 6520 5072 6f64 7563 7473 207c 2020  ine Products |  
+00006660: 205b 6c69 6e6b 5d28 6874 7470 733a 2f2f   [link](https://
+00006670: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
+00006680: 2f66 696c 652f 642f 317a 7547 5248 7646  /file/d/1zuGRHvF
+00006690: 324b 4864 3539 6177 3769 3733 3637 4f48  2KHd59aw7i7367OH
+000066a0: 5f74 514e 4f47 7a37 412f 7669 6577 3f75  _tQNOGz7A/view?u
+000066b0: 7370 3d73 6861 7269 6e67 2920 2020 2020  sp=sharing)     
+000066c0: 207c 2020 5b6c 696e 6b5d 2868 7474 7073   |  [link](https
+000066d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000066e0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000066f0: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+00006700: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+00006710: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+00006720: 696f 6e2f 6578 7472 6163 746f 725f 736f  ion/extractor_so
+00006730: 7029 2020 207c 0a7c 2060 5669 5445 7874  p)   |.| `ViTExt
+00006740: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+00006750: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+00006760: 6172 7322 2960 2020 207c 2030 2e39 3037  ars")`   | 0.907
+00006770: 207c 2020 2020 2020 2020 2043 4152 5320   |         CARS 
+00006780: 3139 3620 2020 2020 2020 2020 7c20 2020  196         |   
+00006790: 5b6c 696e 6b5d 2868 7474 7073 3a2f 2f64  [link](https://d
+000067a0: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+000067b0: 6472 6976 652f 666f 6c64 6572 732f 3137  drive/folders/17
+000067c0: 6134 5f66 6739 3464 6f78 3273 666b 586d  a4_fg94dox2sfkXm
+000067d0: 772d 4b43 7469 4c42 6c78 2d75 742d 313f  w-KCtiLBlx-ut-1?
+000067e0: 7573 703d 7368 6172 696e 6729 2020 2020  usp=sharing)    
+000067f0: 7c20 205b 6c69 6e6b 5d28 6874 7470 733a  |  [link](https:
+00006800: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00006810: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00006820: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+00006830: 6d61 696e 2f70 6970 656c 696e 6573 2f66  main/pipelines/f
+00006840: 6561 7475 7265 735f 6578 7472 6163 7469  eatures_extracti
+00006850: 6f6e 2f65 7874 7261 6374 6f72 5f63 6172  on/extractor_car
+00006860: 7329 2020 7c0a 7c20 2060 5669 5445 7874  s)  |.|  `ViTExt
+00006870: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+00006880: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+00006890: 7562 2229 6020 2020 7c20 302e 3833 3720  ub")`   | 0.837 
+000068a0: 7c20 2020 2020 2020 4355 4220 3230 3020  |       CUB 200 
+000068b0: 3230 3131 2020 2020 2020 207c 2020 205b  2011       |   [
+000068c0: 6c69 6e6b 5d28 6874 7470 733a 2f2f 6472  link](https://dr
+000068d0: 6976 652e 676f 6f67 6c65 2e63 6f6d 2f64  ive.google.com/d
+000068e0: 7269 7665 2f66 6f6c 6465 7273 2f31 5450  rive/folders/1TP
+000068f0: 434e 2d65 5a46 4c71 6f71 344a 4267 6e49  CN-eZFLqoq4JBgnI
+00006900: 666c 694a 6f45 4b34 3878 396f 7a62 3f75  fliJoEK48x9ozb?u
+00006910: 7370 3d73 6861 7269 6e67 2920 2020 207c  sp=sharing)    |
+00006920: 2020 5b6c 696e 6b5d 2868 7474 7073 3a2f    [link](https:/
+00006930: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+00006940: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+00006950: 2d6c 6561 726e 696e 672f 7472 6565 2f6d  -learning/tree/m
+00006960: 6169 6e2f 7069 7065 6c69 6e65 732f 6665  ain/pipelines/fe
+00006970: 6174 7572 6573 5f65 7874 7261 6374 696f  atures_extractio
+00006980: 6e2f 6578 7472 6163 746f 725f 6375 6229  n/extractor_cub)
+00006990: 2020 207c 0a0a 5765 2061 6c73 6f20 7072     |..We also pr
+000069a0: 6f76 6964 6520 616e 2069 6e74 6567 7261  ovide an integra
+000069b0: 7469 6f6e 2077 6974 6820 7468 6520 6d6f  tion with the mo
+000069c0: 6465 6c73 2070 7265 7472 6169 6e65 6420  dels pretrained 
+000069d0: 6279 206f 7468 6572 2072 6573 6561 7263  by other researc
+000069e0: 6865 7273 2e0a 416c 6c20 6d65 7472 6963  hers..All metric
+000069f0: 7320 6265 6c6f 7720 7765 7265 206f 6274  s below were obt
+00006a00: 6169 6e65 6420 6f6e 2074 6865 2069 6d61  ained on the ima
+00006a10: 6765 7320 7769 7468 2074 6865 2073 697a  ges with the siz
+00006a20: 6573 206f 6620 2a2a 3232 3420 7820 3232  es of **224 x 22
+00006a30: 342a 2a3a 0a0a 7c20 2020 2020 2020 2020  4**:..|         
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 206d 6f64 656c 2020 2020 2020 2020     model        
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a70: 2020 2020 207c 2053 7461 6e66 6f72 6420       | Stanford 
+00006a80: 4f6e 6c69 6e65 2050 726f 6475 6374 7320  Online Products 
+00006a90: 7c20 4465 6570 4661 7368 696f 6e20 496e  | DeepFashion In
+00006aa0: 5368 6f70 207c 2043 5542 2032 3030 2032  Shop | CUB 200 2
+00006ab0: 3031 3120 7c20 4341 5253 2031 3936 207c  011 | CARS 196 |
+00006ac0: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
+00006ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00006b00: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00006b10: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  ----------:|:---
+00006b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00006b30: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  |:------------:|
+00006b40: 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020  :--------:|.|   
+00006b50: 2060 5669 5455 6e69 636f 6d45 7874 7261   `ViTUnicomExtra
+00006b60: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006b70: 696e 6564 2822 7669 7462 3136 5f75 6e69  ined("vitb16_uni
+00006b80: 636f 6d22 2960 2020 2020 207c 2020 2020  com")`     |    
+00006b90: 2020 2020 2020 302e 3730 3020 2020 2020        0.700     
+00006ba0: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
+00006bb0: 3733 3420 2020 2020 2020 207c 2020 2020  734        |    
+00006bc0: 302e 3834 3720 2020 2020 7c20 2030 2e39  0.847     |  0.9
+00006bd0: 3136 2020 207c 0a7c 2020 2020 6056 6954  16   |.|    `ViT
+00006be0: 556e 6963 6f6d 4578 7472 6163 746f 722e  UnicomExtractor.
+00006bf0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+00006c00: 2276 6974 6233 325f 756e 6963 6f6d 2229  "vitb32_unicom")
+00006c10: 6020 2020 2020 7c20 2020 2020 2020 2020  `     |         
+00006c20: 2030 2e36 3930 2020 2020 2020 2020 2020   0.690          
+00006c30: 207c 2020 2020 2020 2030 2e37 3232 2020   |       0.722  
+00006c40: 2020 2020 2020 7c20 2020 2030 2e37 3936        |    0.796
+00006c50: 2020 2020 207c 2020 302e 3839 3320 2020       |  0.893   
+00006c60: 7c0a 7c20 2020 2060 5669 5455 6e69 636f  |.|    `ViTUnico
+00006c70: 6d45 7874 7261 6374 6f72 2e66 726f 6d5f  mExtractor.from_
+00006c80: 7072 6574 7261 696e 6564 2822 7669 746c  pretrained("vitl
+00006c90: 3134 5f75 6e69 636f 6d22 2960 2020 2020  14_unicom")`    
+00006ca0: 207c 2020 2020 2020 2020 2020 302e 3732   |          0.72
+00006cb0: 3620 2020 2020 2020 2020 2020 7c20 2020  6           |   
+00006cc0: 2020 2020 302e 3739 3020 2020 2020 2020      0.790       
+00006cd0: 207c 2020 2020 302e 3836 3820 2020 2020   |    0.868     
+00006ce0: 7c20 2030 2e39 3232 2020 207c 0a7c 2060  |  0.922   |.| `
+00006cf0: 5669 5455 6e69 636f 6d45 7874 7261 6374  ViTUnicomExtract
+00006d00: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00006d10: 6564 2822 7669 746c 3134 5f33 3336 7078  ed("vitl14_336px
+00006d20: 5f75 6e69 636f 6d22 2960 2020 7c20 2020  _unicom")`  |   
+00006d30: 2020 2020 2020 2030 2e37 3435 2020 2020         0.745    
+00006d40: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
+00006d50: 2e38 3130 2020 2020 2020 2020 7c20 2020  .810        |   
+00006d60: 2030 2e38 3735 2020 2020 207c 2020 302e   0.875     |  0.
+00006d70: 3932 3420 2020 7c0a 7c20 2020 2060 5669  924   |.|    `Vi
+00006d80: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+00006d90: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00006da0: 7362 6572 5f76 6974 6233 325f 3232 3422  sber_vitb32_224"
+00006db0: 2960 2020 2020 207c 2020 2020 2020 2020  )`     |        
+00006dc0: 2020 302e 3534 3720 2020 2020 2020 2020    0.547         
+00006dd0: 2020 7c20 2020 2020 2020 302e 3531 3420    |       0.514 
+00006de0: 2020 2020 2020 207c 2020 2020 302e 3434         |    0.44
+00006df0: 3820 2020 2020 7c20 2030 2e36 3138 2020  8     |  0.618  
+00006e00: 207c 0a7c 2020 2020 6056 6954 434c 4950   |.|    `ViTCLIP
+00006e10: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006e20: 7265 7472 6169 6e65 6428 2273 6265 725f  retrained("sber_
+00006e30: 7669 7462 3136 5f32 3234 2229 6020 2020  vitb16_224")`   
+00006e40: 2020 7c20 2020 2020 2020 2020 2030 2e35    |          0.5
+00006e50: 3635 2020 2020 2020 2020 2020 207c 2020  65           |  
+00006e60: 2020 2020 2030 2e35 3635 2020 2020 2020       0.565      
+00006e70: 2020 7c20 2020 2030 2e35 3234 2020 2020    |    0.524    
+00006e80: 207c 2020 302e 3634 3820 2020 7c0a 7c20   |  0.648   |.| 
+00006e90: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00006ea0: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006eb0: 696e 6564 2822 7362 6572 5f76 6974 6c31  ined("sber_vitl1
+00006ec0: 345f 3232 3422 2960 2020 2020 207c 2020  4_224")`     |  
+00006ed0: 2020 2020 2020 2020 302e 3531 3220 2020          0.512   
+00006ee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006ef0: 302e 3535 3520 2020 2020 2020 207c 2020  0.555        |  
+00006f00: 2020 302e 3630 3620 2020 2020 7c20 2030    0.606     |  0
+00006f10: 2e37 3037 2020 207c 0a7c 2020 2060 5669  .707   |.|   `Vi
+00006f20: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+00006f30: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00006f40: 6f70 656e 6169 5f76 6974 6233 325f 3232  openai_vitb32_22
+00006f50: 3422 2960 2020 2020 7c20 2020 2020 2020  4")`    |       
+00006f60: 2020 2030 2e36 3132 2020 2020 2020 2020     0.612        
+00006f70: 2020 207c 2020 2020 2020 2030 2e34 3931     |       0.491
+00006f80: 2020 2020 2020 2020 7c20 2020 2030 2e35          |    0.5
+00006f90: 3630 2020 2020 207c 2020 302e 3639 3320  60     |  0.693 
+00006fa0: 2020 7c0a 7c20 2020 6056 6954 434c 4950    |.|   `ViTCLIP
+00006fb0: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006fc0: 7265 7472 6169 6e65 6428 226f 7065 6e61  retrained("opena
+00006fd0: 695f 7669 7462 3136 5f32 3234 2229 6020  i_vitb16_224")` 
+00006fe0: 2020 207c 2020 2020 2020 2020 2020 302e     |          0.
+00006ff0: 3634 3820 2020 2020 2020 2020 2020 7c20  648           | 
+00007000: 2020 2020 2020 302e 3630 3620 2020 2020        0.606     
+00007010: 2020 207c 2020 2020 302e 3636 3520 2020     |    0.665   
+00007020: 2020 7c20 2030 2e37 3637 2020 207c 0a7c    |  0.767   |.|
+00007030: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00007040: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00007050: 696e 6564 2822 6f70 656e 6169 5f76 6974  ined("openai_vit
+00007060: 6c31 345f 3232 3422 2960 2020 2020 7c20  l14_224")`    | 
+00007070: 2020 2020 2020 2020 2030 2e36 3730 2020           0.670  
+00007080: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00007090: 2030 2e36 3735 2020 2020 2020 2020 7c20   0.675        | 
+000070a0: 2020 2030 2e37 3435 2020 2020 207c 2020     0.745     |  
+000070b0: 302e 3834 3420 2020 7c0a 7c20 2020 2020  0.844   |.|     
+000070c0: 2020 2060 5669 5445 7874 7261 6374 6f72     `ViTExtractor
+000070d0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+000070e0: 2822 7669 7473 3136 5f64 696e 6f22 2960  ("vits16_dino")`
+000070f0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00007100: 2020 2020 302e 3634 3820 2020 2020 2020      0.648       
+00007110: 2020 2020 7c20 2020 2020 2020 302e 3530      |       0.50
+00007120: 3920 2020 2020 2020 207c 2020 2020 302e  9        |    0.
+00007130: 3632 3720 2020 2020 7c20 2030 2e32 3635  627     |  0.265
+00007140: 2020 207c 0a7c 2020 2020 2020 2020 2060     |.|         `
+00007150: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
+00007160: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
+00007170: 7473 385f 6469 6e6f 2229 6020 2020 2020  ts8_dino")`     
+00007180: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
+00007190: 2e36 3531 2020 2020 2020 2020 2020 207c  .651           |
+000071a0: 2020 2020 2020 2030 2e35 3234 2020 2020         0.524    
+000071b0: 2020 2020 7c20 2020 2030 2e36 3631 2020      |    0.661  
+000071c0: 2020 207c 2020 302e 3331 3520 2020 7c0a     |  0.315   |.
+000071d0: 7c20 2020 2020 2020 2060 5669 5445 7874  |        `ViTExt
+000071e0: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+000071f0: 7261 696e 6564 2822 7669 7462 3136 5f64  rained("vitb16_d
+00007200: 696e 6f22 2960 2020 2020 2020 2020 207c  ino")`         |
+00007210: 2020 2020 2020 2020 2020 302e 3635 3820            0.658 
+00007220: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00007230: 2020 302e 3531 3420 2020 2020 2020 207c    0.514        |
+00007240: 2020 2020 302e 3534 3120 2020 2020 7c20      0.541     | 
+00007250: 2030 2e32 3838 2020 207c 0a7c 2020 2020   0.288   |.|    
+00007260: 2020 2020 2060 5669 5445 7874 7261 6374       `ViTExtract
+00007270: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00007280: 6564 2822 7669 7462 385f 6469 6e6f 2229  ed("vitb8_dino")
+00007290: 6020 2020 2020 2020 2020 7c20 2020 2020  `         |     
+000072a0: 2020 2020 2030 2e36 3839 2020 2020 2020       0.689      
+000072b0: 2020 2020 207c 2020 2020 2020 2030 2e35       |       0.5
+000072c0: 3939 2020 2020 2020 2020 7c20 2020 2030  99        |    0
+000072d0: 2e35 3036 2020 2020 207c 2020 302e 3331  .506     |  0.31
+000072e0: 3320 2020 7c0a 7c20 2020 2060 5265 736e  3   |.|    `Resn
+000072f0: 6574 4578 7472 6163 746f 722e 6672 6f6d  etExtractor.from
+00007300: 5f70 7265 7472 6169 6e65 6428 2272 6573  _pretrained("res
+00007310: 6e65 7435 305f 6d6f 636f 5f76 3222 2960  net50_moco_v2")`
+00007320: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00007330: 302e 3439 3320 2020 2020 2020 2020 2020  0.493           
+00007340: 7c20 2020 2020 2020 302e 3236 3720 2020  |       0.267   
+00007350: 2020 2020 207c 2020 2020 302e 3236 3420       |    0.264 
+00007360: 2020 2020 7c20 2030 2e31 3439 2020 207c      |  0.149   |
+00007370: 0a7c 2060 5265 736e 6574 4578 7472 6163  .| `ResnetExtrac
+00007380: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
+00007390: 6e65 6428 2272 6573 6e65 7435 305f 696d  ned("resnet50_im
+000073a0: 6167 656e 6574 316b 5f76 3122 2960 2020  agenet1k_v1")`  
+000073b0: 7c20 2020 2020 2020 2020 2030 2e35 3135  |          0.515
+000073c0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000073d0: 2020 2030 2e32 3834 2020 2020 2020 2020     0.284        
+000073e0: 7c20 2020 2030 2e34 3535 2020 2020 207c  |    0.455     |
+000073f0: 2020 302e 3234 3720 2020 7c0a 0a2a 2a54    0.247   |..**T
+00007400: 6865 206d 6574 7269 6373 206d 6179 2062  he metrics may b
+00007410: 6520 6469 6666 6572 656e 7420 6672 6f6d  e different from
+00007420: 2074 6865 206f 6e65 7320 7265 706f 7274   the ones report
+00007430: 6564 2062 7920 7061 7065 7273 2c0a 6265  ed by papers,.be
+00007440: 6361 7573 6520 7468 6520 7665 7273 696f  cause the versio
+00007450: 6e20 6f66 2074 7261 696e 2f76 616c 2073  n of train/val s
+00007460: 706c 6974 2061 6e64 2075 7361 6765 206f  plit and usage o
+00007470: 6620 626f 756e 6469 6e67 2062 6f78 6573  f bounding boxes
+00007480: 206d 6179 2064 6966 6665 722e 0a50 6172   may differ..Par
+00007490: 7469 6375 6c61 726c 792c 2077 6520 7573  ticularly, we us
+000074a0: 6564 2062 6f75 6e64 696e 6720 626f 7865  ed bounding boxe
+000074b0: 7320 6475 7269 6e67 2074 6865 2065 7661  s during the eva
+000074c0: 6c75 6174 696f 6e2e 2a0a 0a23 2323 2048  luation.*..### H
+000074d0: 6f77 2074 6f20 7573 6520 6d6f 6465 6c73  ow to use models
+000074e0: 2066 726f 6d20 5a6f 6f3f 0a0a 5b63 6f6d   from Zoo?..[com
+000074f0: 6d65 6e74 5d3a 7a6f 6f2d 7374 6172 740a  ment]:zoo-start.
+00007500: 6060 6070 7974 686f 6e0a 6672 6f6d 206f  ```python.from o
+00007510: 6d6c 2e63 6f6e 7374 2069 6d70 6f72 7420  ml.const import 
+00007520: 434b 5054 5f53 4156 455f 524f 4f54 2061  CKPT_SAVE_ROOT a
+00007530: 7320 434b 5054 5f44 4952 2c20 4d4f 434b  s CKPT_DIR, MOCK
+00007540: 5f44 4154 4153 4554 5f50 4154 4820 6173  _DATASET_PATH as
+00007550: 2044 4154 415f 4449 520a 6672 6f6d 206f   DATA_DIR.from o
+00007560: 6d6c 2e6d 6f64 656c 7320 696d 706f 7274  ml.models import
+00007570: 2056 6954 4578 7472 6163 746f 720a 6672   ViTExtractor.fr
+00007580: 6f6d 206f 6d6c 2e72 6567 6973 7472 792e  om oml.registry.
+00007590: 7472 616e 7366 6f72 6d73 2069 6d70 6f72  transforms impor
+000075a0: 7420 6765 745f 7472 616e 7366 6f72 6d73  t get_transforms
+000075b0: 5f66 6f72 5f70 7265 7472 6169 6e65 640a  _for_pretrained.
+000075c0: 0a6d 6f64 656c 203d 2056 6954 4578 7472  .model = ViTExtr
+000075d0: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
+000075e0: 6169 6e65 6428 2276 6974 7331 365f 6469  ained("vits16_di
+000075f0: 6e6f 2229 0a74 7261 6e73 666f 726d 732c  no").transforms,
+00007600: 2069 6d5f 7265 6164 6572 203d 2067 6574   im_reader = get
+00007610: 5f74 7261 6e73 666f 726d 735f 666f 725f  _transforms_for_
+00007620: 7072 6574 7261 696e 6564 2822 7669 7473  pretrained("vits
+00007630: 3136 5f64 696e 6f22 290a 0a69 6d67 203d  16_dino")..img =
+00007640: 2069 6d5f 7265 6164 6572 2844 4154 415f   im_reader(DATA_
+00007650: 4449 5220 2f20 2269 6d61 6765 7322 202f  DIR / "images" /
+00007660: 2022 6369 7263 6c65 5f31 2e6a 7067 2229   "circle_1.jpg")
+00007670: 2020 2320 7075 7420 7061 7468 2074 6f20    # put path to 
+00007680: 796f 7572 2069 6d61 6765 2068 6572 650a  your image here.
+00007690: 696d 675f 7465 6e73 6f72 203d 2074 7261  img_tensor = tra
+000076a0: 6e73 666f 726d 7328 696d 6729 0a23 2069  nsforms(img).# i
+000076b0: 6d67 5f74 656e 736f 7220 3d20 7472 616e  mg_tensor = tran
+000076c0: 7366 6f72 6d73 2869 6d61 6765 3d69 6d67  sforms(image=img
+000076d0: 295b 2269 6d61 6765 225d 2020 2320 666f  )["image"]  # fo
+000076e0: 7220 7472 616e 7366 6f72 6d73 2066 726f  r transforms fro
+000076f0: 6d20 416c 6275 6d65 6e74 6174 696f 6e73  m Albumentations
+00007700: 0a0a 6665 6174 7572 6573 203d 206d 6f64  ..features = mod
+00007710: 656c 2869 6d67 5f74 656e 736f 722e 756e  el(img_tensor.un
+00007720: 7371 7565 657a 6528 3029 290a 0a23 2043  squeeze(0))..# C
+00007730: 6865 636b 206f 7468 6572 2061 7661 696c  heck other avail
+00007740: 6162 6c65 206d 6f64 656c 733a 0a70 7269  able models:.pri
+00007750: 6e74 286c 6973 7428 5669 5445 7874 7261  nt(list(ViTExtra
+00007760: 6374 6f72 2e70 7265 7472 6169 6e65 645f  ctor.pretrained_
+00007770: 6d6f 6465 6c73 2e6b 6579 7328 2929 290a  models.keys())).
+00007780: 0a23 204c 6f61 6420 6368 6563 6b70 6f69  .# Load checkpoi
+00007790: 6e74 2073 6176 6564 206f 6e20 6120 6469  nt saved on a di
+000077a0: 736b 3a0a 6d6f 6465 6c5f 203d 2056 6954  sk:.model_ = ViT
+000077b0: 4578 7472 6163 746f 7228 7765 6967 6874  Extractor(weight
+000077c0: 733d 434b 5054 5f44 4952 202f 2022 7669  s=CKPT_DIR / "vi
+000077d0: 7473 3136 5f64 696e 6f2e 636b 7074 222c  ts16_dino.ckpt",
+000077e0: 2061 7263 683d 2276 6974 7331 3622 2c20   arch="vits16", 
+000077f0: 6e6f 726d 616c 6973 655f 6665 6174 7572  normalise_featur
+00007800: 6573 3d46 616c 7365 290a 6060 600a 5b63  es=False).```.[c
+00007810: 6f6d 6d65 6e74 5d3a 7a6f 6f2d 656e 640a  omment]:zoo-end.
+00007820: 0a23 2320 5b43 6f6e 7472 6962 7574 696e  .## [Contributin
+00007830: 6720 6775 6964 655d 2868 7474 7073 3a2f  g guide](https:/
+00007840: 2f6f 7065 6e2d 6d65 7472 6963 2d6c 6561  /open-metric-lea
+00007850: 726e 696e 672e 7265 6164 7468 6564 6f63  rning.readthedoc
+00007860: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6f  s.io/en/latest/o
+00007870: 6d6c 2f63 6f6e 7472 6962 7574 696e 672e  ml/contributing.
+00007880: 6874 6d6c 290a 0a57 6520 7765 6c63 6f6d  html)..We welcom
+00007890: 6520 6e65 7720 636f 6e74 7269 6275 746f  e new contributo
+000078a0: 7273 2120 506c 6561 7365 2c20 7365 6520  rs! Please, see 
+000078b0: 6f75 723a 0a2a 205b 436f 6e74 7269 6275  our:.* [Contribu
+000078c0: 7469 6e67 2067 7569 6465 5d28 6874 7470  ting guide](http
+000078d0: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+000078e0: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+000078f0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00007900: 742f 6f6d 6c2f 636f 6e74 7269 6275 7469  t/oml/contributi
+00007910: 6e67 2e68 746d 6c29 0a2a 205b 4b61 6e62  ng.html).* [Kanb
+00007920: 616e 2062 6f61 7264 5d28 6874 7470 733a  an board](https:
+00007930: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00007940: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00007950: 632d 6c65 6172 6e69 6e67 2f70 726f 6a65  c-learning/proje
+00007960: 6374 732f 3129 0a0a 2323 2041 636b 6e6f  cts/1)..## Ackno
+00007970: 776c 6564 676d 656e 7473 0a0a 3c61 2068  wledgments..<a h
+00007980: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00007990: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+000079a0: 2d74 6561 6d2f 6361 7461 6c79 7374 2220  -team/catalyst" 
+000079b0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000079c0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000079d0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+000079e0: 636f 6e74 656e 742e 636f 6d2f 6361 7461  content.com/cata
+000079f0: 6c79 7374 2d74 6561 6d2f 6361 7461 6c79  lyst-team/cataly
+00007a00: 7374 2d70 6963 732f 6d61 7374 6572 2f70  st-pics/master/p
+00007a10: 6963 732f 6361 7461 6c79 7374 5f6c 6f67  ics/catalyst_log
+00007a20: 6f2e 706e 6722 2077 6964 7468 3d22 3130  o.png" width="10
+00007a30: 3022 2f3e 3c2f 613e 0a0a 5468 6520 7072  0"/></a>..The pr
+00007a40: 6f6a 6563 7420 7761 7320 7374 6172 7465  oject was starte
+00007a50: 6420 696e 2032 3032 3020 6173 2061 206d  d in 2020 as a m
+00007a60: 6f64 756c 6520 666f 7220 5b43 6174 616c  odule for [Catal
+00007a70: 7973 745d 2868 7474 7073 3a2f 2f67 6974  yst](https://git
+00007a80: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+00007a90: 2d74 6561 6d2f 6361 7461 6c79 7374 2920  -team/catalyst) 
+00007aa0: 6c69 6272 6172 792e 0a49 2077 616e 7420  library..I want 
+00007ab0: 746f 2074 6861 6e6b 2070 656f 706c 6520  to thank people 
+00007ac0: 7768 6f20 776f 726b 6564 2077 6974 6820  who worked with 
+00007ad0: 6d65 206f 6e20 7468 6174 206d 6f64 756c  me on that modul
+00007ae0: 653a 0a5b 4a75 6c69 6120 5368 656e 7368  e:.[Julia Shensh
+00007af0: 696e 615d 2868 7474 7073 3a2f 2f67 6974  ina](https://git
+00007b00: 6875 622e 636f 6d2f 6a75 6c69 612d 7368  hub.com/julia-sh
+00007b10: 656e 7368 696e 6129 2c0a 5b4e 696b 6974  enshina),.[Nikit
+00007b20: 6120 4261 6c61 6761 6e73 6b79 5d28 6874  a Balagansky](ht
+00007b30: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00007b40: 2f65 6c65 7068 616e 746d 6970 7429 2c0a  /elephantmipt),.
+00007b50: 5b53 6572 6765 7920 4b6f 6c65 736e 696b  [Sergey Kolesnik
+00007b60: 6f76 5d28 6874 7470 733a 2f2f 6769 7468  ov](https://gith
+00007b70: 7562 2e63 6f6d 2f53 6369 7461 746f 7229  ub.com/Scitator)
+00007b80: 0a61 6e64 206f 7468 6572 732e 0a0a 4920  .and others...I 
+00007b90: 776f 756c 6420 6c69 6b65 2074 6f20 7468  would like to th
+00007ba0: 616e 6b20 7065 6f70 6c65 2077 686f 2063  ank people who c
+00007bb0: 6f6e 7469 6e75 6520 776f 726b 696e 6720  ontinue working 
+00007bc0: 6f6e 2074 6869 7320 7069 7065 6c69 6e65  on this pipeline
+00007bd0: 2077 6865 6e20 6974 2062 6563 616d 6520   when it became 
+00007be0: 6120 7365 7061 7265 2070 726f 6a65 6374  a separe project
+00007bf0: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
+00007c00: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
+00007c10: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
+00007c20: 6e73 6869 6e61 292c 0a5b 4d69 7368 6120  nshina),.[Misha 
+00007c30: 4b69 6e64 756c 6f76 5d28 6874 7470 733a  Kindulov](https:
+00007c40: 2f2f 6769 7468 7562 2e63 6f6d 2f62 306e  //github.com/b0n
+00007c50: 6365 292c 0a5b 416c 656b 7365 6920 5461  ce),.[Aleksei Ta
+00007c60: 7261 736f 765d 2868 7474 7073 3a2f 2f67  rasov](https://g
+00007c70: 6974 6875 622e 636f 6d2f 4461 6c6f 726f  ithub.com/Daloro
+00007c80: 4154 2920 616e 640a 5b56 6572 6b68 6f76  AT) and.[Verkhov
+00007c90: 7473 6576 204c 656f 6e69 645d 2868 7474  tsev Leonid](htt
+00007ca0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00007cb0: 6c65 6f72 6f6d 616e 6f76 6963 6829 2e0a  leoromanovich)..
+00007cc0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00007cd0: 2f2f 7777 772e 6e65 7779 6f72 6b65 722e  //www.newyorker.
+00007ce0: 6465 2f22 2074 6172 6765 743d 225f 626c  de/" target="_bl
+00007cf0: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
+00007d00: 7474 7073 3a2f 2f75 706c 6f61 642e 7769  ttps://upload.wi
+00007d10: 6b69 6d65 6469 612e 6f72 672f 7769 6b69  kimedia.org/wiki
+00007d20: 7065 6469 612f 636f 6d6d 6f6e 732f 7468  pedia/commons/th
+00007d30: 756d 622f 642f 6438 2f4e 6577 5f59 6f72  umb/d/d8/New_Yor
+00007d40: 6b65 722e 7376 672f 3132 3830 7078 2d4e  ker.svg/1280px-N
+00007d50: 6577 5f59 6f72 6b65 722e 7376 672e 706e  ew_Yorker.svg.pn
+00007d60: 6722 2077 6964 7468 3d22 3130 3022 2f3e  g" width="100"/>
+00007d70: 3c2f 613e 0a0a 4920 616c 736f 2077 616e  </a>..I also wan
+00007d80: 7420 746f 2074 6861 6e6b 204e 6577 596f  t to thank NewYo
+00007d90: 726b 6572 2c20 7369 6e63 6520 7468 6520  rker, since the 
+00007da0: 7061 7274 206f 6620 6675 6e63 7469 6f6e  part of function
+00007db0: 616c 6974 7920 7761 7320 6465 7665 6c6f  ality was develo
+00007dc0: 7065 6420 2861 6e64 2075 7365 6429 2062  ped (and used) b
+00007dd0: 7920 6974 7320 636f 6d70 7574 6572 2076  y its computer v
+00007de0: 6973 696f 6e20 7465 616d 206c 6564 2062  ision team led b
+00007df0: 7920 6d65 2e0a                           y me..
```

### Comparing `open-metric-learning-0.4.3/oml/const.py` & `open-metric-learning-0.4.4/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/datasets/base.py` & `open-metric-learning-0.4.4/oml/datasets/base.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/datasets/list_dataset.py` & `open-metric-learning-0.4.4/oml/datasets/list_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/datasets/pairs.py` & `open-metric-learning-0.4.4/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/datasets/triplet.py` & `open-metric-learning-0.4.4/oml/datasets/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/ddp/patching.py` & `open-metric-learning-0.4.4/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/ddp/utils.py` & `open-metric-learning-0.4.4/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/functional/label_smoothing.py` & `open-metric-learning-0.4.4/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/functional/losses.py` & `open-metric-learning-0.4.4/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/functional/metrics.py` & `open-metric-learning-0.4.4/oml/functional/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/inference/abstract.py` & `open-metric-learning-0.4.4/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/inference/flat.py` & `open-metric-learning-0.4.4/oml/inference/flat.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/inference/pairs.py` & `open-metric-learning-0.4.4/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/criterions.py` & `open-metric-learning-0.4.4/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/datasets.py` & `open-metric-learning-0.4.4/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/metrics.py` & `open-metric-learning-0.4.4/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/miners.py` & `open-metric-learning-0.4.4/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/models.py` & `open-metric-learning-0.4.4/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/retrieval.py` & `open-metric-learning-0.4.4/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/interfaces/samplers.py` & `open-metric-learning-0.4.4/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/callbacks/metric.py` & `open-metric-learning-0.4.4/oml/lightning/callbacks/metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from math import ceil
 from typing import Any, Optional
 
 import numpy as np
 import pytorch_lightning as pl
+from matplotlib import pyplot as plt
 from neptune.new.types import File
 from pytorch_lightning import Callback
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger
+from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 
 from oml.const import LOG_IMAGE_FOLDER
 from oml.ddp.patching import check_loaders_is_patched, patch_dataloader_to_ddp
 from oml.interfaces.metrics import IBasicMetric, IMetricDDP, IMetricVisualisable
 from oml.lightning.modules.ddp import ModuleDDP
 from oml.utils.misc import flatten_dict
@@ -97,19 +98,25 @@
         if not isinstance(self.metric, IMetricVisualisable):
             return
 
         for fig, metric_log_str in zip(*self.metric.visualize()):
             log_str = f"{LOG_IMAGE_FOLDER}/{metric_log_str}"
             if isinstance(pl_module.logger, NeptuneLogger):
                 pl_module.logger.experiment[log_str].log(File.as_image(fig))
+            elif isinstance(pl_module.logger, WandbLogger):
+                fig.canvas.draw()
+                fig_img = np.array(fig.canvas.renderer.buffer_rgba())[..., :3]
+                pl_module.logger.log_image(images=[fig_img], key=metric_log_str)
+                plt.close(fig)
             elif isinstance(pl_module.logger, TensorBoardLogger):
                 fig.canvas.draw()
                 data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
                 data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
                 pl_module.logger.experiment.add_image(log_str, np.transpose(data, (2, 0, 1)), pl_module.current_epoch)
+                plt.close(fig)
             else:
                 raise ValueError(f"Logging with {type(pl_module.logger)} is not supported yet.")
 
     def on_validation_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         self._ready_to_accumulate = False
         if self._collected_samples != self._expected_samples:
             self._raise_computation_error()
```

### Comparing `open-metric-learning-0.4.3/oml/lightning/modules/ddp.py` & `open-metric-learning-0.4.4/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/modules/extractor.py` & `open-metric-learning-0.4.4/oml/lightning/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-0.4.4/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/pipelines/parser.py` & `open-metric-learning-0.4.4/oml/lightning/pipelines/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-import os
 import warnings
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 import albumentations as albu
 import torch
 from pytorch_lightning.callbacks import ModelCheckpoint
-from pytorch_lightning.loggers import NeptuneLogger
+from pytorch_lightning.loggers import (
+    LightningLoggerBase,
+    NeptuneLogger,
+    TensorBoardLogger,
+    WandbLogger,
+)
 from pytorch_lightning.plugins import DDPPlugin
 
 from oml.const import PROJECT_ROOT, TCfg
 from oml.datasets.base import DatasetWithLabels
 from oml.interfaces.samplers import IBatchSampler
+from oml.registry.loggers import get_logger_by_cfg
 from oml.registry.samplers import SAMPLERS_CATEGORIES_BASED, get_sampler_by_cfg
 from oml.registry.schedulers import get_scheduler_by_cfg
 from oml.registry.transforms import get_transforms_by_cfg
 from oml.utils.misc import dictconfig_to_dict, flatten_dict
 
 
 def parse_engine_params_from_config(cfg: TCfg) -> Dict[str, Any]:
@@ -56,43 +61,46 @@
     }
 
 
 def check_is_config_for_ddp(cfg: TCfg) -> bool:
     return bool(cfg["strategy"])
 
 
-def initialize_logging(cfg: TCfg) -> Union[bool, NeptuneLogger]:
-    """
-    Logger initialisation.
+def parse_logger_from_config(cfg: TCfg) -> LightningLoggerBase:
+    logger = TensorBoardLogger(".") if cfg.get("logger", None) is None else get_logger_by_cfg(cfg["logger"])
+    return logger
 
-    If Neptune Logger is used, we also upload to its cloud some files
-    which are good to have for reproducibility.
 
-    """
-    if ("NEPTUNE_API_TOKEN" in os.environ.keys()) and (cfg["neptune_project"] is not None):
+def initialize_logging(cfg: TCfg) -> LightningLoggerBase:
+    logger = parse_logger_from_config(cfg)
+    cwd = Path.cwd().name
+
+    dict_to_log = flatten_dict({**dictconfig_to_dict(cfg), **{"dir": cwd}}, sep="|")
+
+    if isinstance(logger, NeptuneLogger):
         warnings.warn(
             "Unfortunately, in the case of using Neptune, you may experience that long experiments are"
-            "stacked and not responding. It's not an issue on OML's side, so, we cannot fix it. You can use"
-            "Tensorboard logger instead, for this simply leave <NEPTUNE_API_TOKEN> unfilled."
+            "stacked and not responding. It's not an issue on OML's side, so, we cannot fix it."
         )
-
-        cwd = Path.cwd()
-        logger = NeptuneLogger(
-            api_key=os.environ["NEPTUNE_API_TOKEN"],
-            project=cfg["neptune_project"],
-            tags=list(cfg.get("tags", [])) + [cfg.get("postfix", "")] + [cwd.name],
-            log_model_checkpoints=False,
-        )
-        dict_to_log = {**dictconfig_to_dict(cfg), **{"dir": cwd}}
-        logger.log_hyperparams(flatten_dict(dict_to_log, sep="|"))
+        logger.log_hyperparams(dict_to_log)
         upload_files_to_neptune_cloud(logger, cfg)
 
+        tags = list(cfg.get("tags", [])) + [cfg.get("postfix", "")] + [cwd]
+        logger.run["sys/tags"].add(tags)
+
+    elif isinstance(logger, WandbLogger):
+        logger.log_hyperparams(dict_to_log)
+        # todo: upload files
+        # todo: add tags
+
+    elif isinstance(logger, TensorBoardLogger):
+        pass
+
     else:
-        print(f"Your current logger is not able to log your files, you can use {NeptuneLogger.__name__} for this.")
-        logger = True
+        raise ValueError(f"Unexpected logger {type(logger)}")
 
     return logger
 
 
 def upload_files_to_neptune_cloud(logger: NeptuneLogger, cfg: TCfg) -> None:
     assert isinstance(logger, NeptuneLogger)
```

### Comparing `open-metric-learning-0.4.3/oml/lightning/pipelines/predict.py` & `open-metric-learning-0.4.4/oml/lightning/pipelines/predict.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/pipelines/train.py` & `open-metric-learning-0.4.4/oml/lightning/pipelines/train.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/pipelines/train_postprocessor.py` & `open-metric-learning-0.4.4/oml/lightning/pipelines/train_postprocessor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/lightning/pipelines/validate.py` & `open-metric-learning-0.4.4/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/losses/arcface.py` & `open-metric-learning-0.4.4/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/losses/surrogate_precision.py` & `open-metric-learning-0.4.4/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/losses/triplet.py` & `open-metric-learning-0.4.4/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/metrics/accumulation.py` & `open-metric-learning-0.4.4/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/metrics/embeddings.py` & `open-metric-learning-0.4.4/oml/metrics/embeddings.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/metrics/triplets.py` & `open-metric-learning-0.4.4/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/cross_batch.py` & `open-metric-learning-0.4.4/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/inbatch_all_tri.py` & `open-metric-learning-0.4.4/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-0.4.4/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-0.4.4/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-0.4.4/oml/miners/inbatch_nhard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/miner_with_bank.py` & `open-metric-learning-0.4.4/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/miners/pairs.py` & `open-metric-learning-0.4.4/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/meta/projection.py` & `open-metric-learning-0.4.4/oml/models/meta/projection.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/meta/siamese.py` & `open-metric-learning-0.4.4/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/resnet/extractor.py` & `open-metric-learning-0.4.4/oml/models/resnet/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/resnet/pooling.py` & `open-metric-learning-0.4.4/oml/models/resnet/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/utils.py` & `open-metric-learning-0.4.4/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_clip/external/model.py` & `open-metric-learning-0.4.4/oml/models/vit_clip/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_clip/extractor.py` & `open-metric-learning-0.4.4/oml/models/vit_clip/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_dino/external/hubconf.py` & `open-metric-learning-0.4.4/oml/models/vit_dino/external/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_dino/external/vision_transformer.py` & `open-metric-learning-0.4.4/oml/models/vit_dino/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_dino/extractor.py` & `open-metric-learning-0.4.4/oml/models/vit_dino/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_unicom/external/model.py` & `open-metric-learning-0.4.4/oml/models/vit_unicom/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_unicom/external/vision_transformer.py` & `open-metric-learning-0.4.4/oml/models/vit_unicom/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/models/vit_unicom/extractor.py` & `open-metric-learning-0.4.4/oml/models/vit_unicom/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/__init__.py` & `open-metric-learning-0.4.4/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/losses.py` & `open-metric-learning-0.4.4/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/miners.py` & `open-metric-learning-0.4.4/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/models.py` & `open-metric-learning-0.4.4/oml/registry/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/optimizers.py` & `open-metric-learning-0.4.4/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/postprocessors.py` & `open-metric-learning-0.4.4/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/samplers.py` & `open-metric-learning-0.4.4/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/schedulers.py` & `open-metric-learning-0.4.4/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/registry/transforms.py` & `open-metric-learning-0.4.4/oml/registry/transforms.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-0.4.4/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/samplers/balance.py` & `open-metric-learning-0.4.4/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/samplers/category_balance.py` & `open-metric-learning-0.4.4/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/samplers/distinct_category_balance.py` & `open-metric-learning-0.4.4/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/transforms/images/albumentations.py` & `open-metric-learning-0.4.4/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/transforms/images/torchvision.py` & `open-metric-learning-0.4.4/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/dataframe_format.py` & `open-metric-learning-0.4.4/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/download_mock_dataset.py` & `open-metric-learning-0.4.4/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/images/images.py` & `open-metric-learning-0.4.4/oml/utils/images/images.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/images/images_resize.py` & `open-metric-learning-0.4.4/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/io.py` & `open-metric-learning-0.4.4/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/misc.py` & `open-metric-learning-0.4.4/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/misc_torch.py` & `open-metric-learning-0.4.4/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/oml/utils/remote_storage.py` & `open-metric-learning-0.4.4/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/open_metric_learning.egg-info/PKG-INFO` & `open-metric-learning-0.4.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,1915 +1,1927 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
-00000020: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00000030: 0a56 6572 7369 6f6e 3a20 302e 342e 330a  .Version: 0.4.3.
-00000040: 5375 6d6d 6172 793a 204f 4d4c 2069 7320  Summary: OML is 
-00000050: 6120 5079 546f 7263 682d 6261 7365 6420  a PyTorch-based 
-00000060: 6672 616d 6577 6f72 6b20 746f 2074 7261  framework to tra
-00000070: 696e 2061 6e64 2076 616c 6964 6174 6520  in and validate 
-00000080: 7468 6520 6d6f 6465 6c73 2070 726f 6475  the models produ
-00000090: 6369 6e67 2068 6967 682d 7175 616c 6974  cing high-qualit
-000000a0: 7920 656d 6265 6464 696e 6773 2e0a 486f  y embeddings..Ho
-000000b0: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-000000c0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
-000000d0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
-000000e0: 2d6c 6561 726e 696e 670a 4175 7468 6f72  -learning.Author
-000000f0: 3a20 5368 6162 616e 6f76 2041 6c65 6b73  : Shabanov Aleks
-00000100: 6569 0a41 7574 686f 722d 656d 6169 6c3a  ei.Author-email:
-00000110: 2073 6861 6261 6e6f 6666 2e61 6c65 6b73   shabanoff.aleks
-00000120: 6569 4067 6d61 696c 2e63 6f6d 0a4c 6963  ei@gmail.com.Lic
-00000130: 656e 7365 3a20 4170 6163 6865 204c 6963  ense: Apache Lic
-00000140: 656e 7365 2032 2e30 0a50 726f 6a65 6374  ense 2.0.Project
-00000150: 2d55 524c 3a20 486f 6d65 7061 6765 2c20  -URL: Homepage, 
-00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000170: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
-00000180: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00000190: 0a50 726f 6a65 6374 2d55 524c 3a20 4275  .Project-URL: Bu
-000001a0: 6720 5472 6163 6b65 722c 2068 7474 7073  g Tracker, https
-000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
-000001c0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
-000001d0: 6963 2d6c 6561 726e 696e 672f 6973 7375  ic-learning/issu
-000001e0: 6573 0a4b 6579 776f 7264 733a 2064 6174  es.Keywords: dat
-000001f0: 612d 7363 6965 6e63 652c 636f 6d70 7574  a-science,comput
-00000200: 6572 2d76 6973 696f 6e2c 6465 6570 2d6c  er-vision,deep-l
-00000210: 6561 726e 696e 672c 7079 746f 7263 682c  earning,pytorch,
-00000220: 6d65 7472 6963 2d6c 6561 726e 696e 672c  metric-learning,
-00000230: 7265 7072 6573 656e 7461 7469 6f6e 2d6c  representation-l
-00000240: 6561 726e 696e 672c 7079 746f 7263 682d  earning,pytorch-
-00000250: 6c69 6768 746e 696e 670a 436c 6173 7369  lightning.Classi
-00000260: 6669 6572 3a20 456e 7669 726f 6e6d 656e  fier: Environmen
-00000270: 7420 3a3a 2043 6f6e 736f 6c65 0a43 6c61  t :: Console.Cla
-00000280: 7373 6966 6965 723a 204e 6174 7572 616c  ssifier: Natural
-00000290: 204c 616e 6775 6167 6520 3a3a 2045 6e67   Language :: Eng
-000002a0: 6c69 7368 0a43 6c61 7373 6966 6965 723a  lish.Classifier:
-000002b0: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
-000002c0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000002d0: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
-000002e0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000002f0: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000300: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000310: 7365 0a43 6c61 7373 6966 6965 723a 2049  se.Classifier: I
-00000320: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-00000330: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
-00000340: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000350: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000360: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
-00000370: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-00000380: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
-00000390: 2f45 6e67 696e 6565 7269 6e67 203a 3a20  /Engineering :: 
-000003a0: 4172 7469 6669 6369 616c 2049 6e74 656c  Artificial Intel
-000003b0: 6c69 6765 6e63 650a 436c 6173 7369 6669  ligence.Classifi
-000003c0: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
-000003d0: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
-000003e0: 696e 6720 3a3a 2049 6d61 6765 2052 6563  ing :: Image Rec
-000003f0: 6f67 6e69 7469 6f6e 0a43 6c61 7373 6966  ognition.Classif
-00000400: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000410: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000420: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
-00000430: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000440: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000450: 3a20 332e 370a 436c 6173 7369 6669 6572  : 3.7.Classifier
-00000460: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000470: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000480: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
-00000490: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000004a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000004b0: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
-000004c0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000004d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000004e0: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
-000004f0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000500: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000510: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
-00000520: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
-00000530: 7468 6f6e 0a52 6571 7569 7265 732d 5079  thon.Requires-Py
-00000540: 7468 6f6e 3a20 3e3d 332e 372c 3c34 2e30  thon: >=3.7,<4.0
-00000550: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000560: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000570: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-00000580: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000590: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
-000005a0: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
-000005b0: 7474 7073 3a2f 2f69 2e69 6262 2e63 6f2f  ttps://i.ibb.co/
-000005c0: 7773 6d44 3572 342f 7068 6f74 6f2d 3230  wsmD5r4/photo-20
-000005d0: 3232 2d30 362d 3036 2d31 372d 3430 2d35  22-06-06-17-40-5
-000005e0: 322e 6a70 6722 2077 6964 7468 3d22 3430  2.jpg" width="40
-000005f0: 3070 7822 3e0a 0a21 5b65 7861 6d70 6c65  0px">..![example
-00000600: 2077 6f72 6b66 6c6f 775d 2868 7474 7073   workflow](https
-00000610: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
-00000620: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
-00000630: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
-00000640: 6f6e 732f 776f 726b 666c 6f77 732f 7072  ons/workflows/pr
-00000650: 652d 636f 6d6d 6974 2d77 6f72 6b66 6c6f  e-commit-workflo
-00000660: 772e 7961 6d6c 2f62 6164 6765 2e73 7667  w.yaml/badge.svg
-00000670: 290a 215b 6578 616d 706c 6520 776f 726b  ).![example work
-00000680: 666c 6f77 5d28 6874 7470 733a 2f2f 6769  flow](https://gi
-00000690: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
-000006a0: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
-000006b0: 6172 6e69 6e67 2f61 6374 696f 6e73 2f77  arning/actions/w
-000006c0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2d77  orkflows/tests-w
-000006d0: 6f72 6b66 6c6f 772e 7961 6d6c 2f62 6164  orkflow.yaml/bad
-000006e0: 6765 2e73 7667 3f29 0a5b 215b 446f 6375  ge.svg?).[![Docu
-000006f0: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
-00000700: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
-00000710: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000720: 7473 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ts/open-metric-l
-00000730: 6561 726e 696e 672f 6261 6467 652f 3f76  earning/badge/?v
-00000740: 6572 7369 6f6e 3d6c 6174 6573 7429 5d28  ersion=latest)](
-00000750: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
-00000760: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
-00000770: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000780: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
-00000790: 6573 7429 0a5b 215b 5079 5049 2053 7461  est).[![PyPI Sta
-000007a0: 7475 735d 2868 7474 7073 3a2f 2f70 6570  tus](https://pep
-000007b0: 792e 7465 6368 2f62 6164 6765 2f6f 7065  y.tech/badge/ope
-000007c0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-000007d0: 6729 5d28 6874 7470 733a 2f2f 7065 7079  g)](https://pepy
-000007e0: 2e74 6563 682f 7072 6f6a 6563 742f 6f70  .tech/project/op
-000007f0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00000800: 6e67 290a 5b21 5b50 6970 6920 7665 7273  ng).[![Pipi vers
-00000810: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000820: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000830: 2f76 2f6f 7065 6e2d 6d65 7472 6963 2d6c  /v/open-metric-l
-00000840: 6561 726e 696e 672e 7376 6729 5d28 6874  earning.svg)](ht
-00000850: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000860: 726f 6a65 6374 2f6f 7065 6e2d 6d65 7472  roject/open-metr
-00000870: 6963 2d6c 6561 726e 696e 672f 290a 215b  ic-learning/).![
-00000880: 6578 616d 706c 6520 776f 726b 666c 6f77  example workflow
-00000890: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000008a0: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-000008b0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000008c0: 6e67 2f61 6374 696f 6e73 2f77 6f72 6b66  ng/actions/workf
-000008d0: 6c6f 7773 2f70 7974 686f 6e2d 7665 7273  lows/python-vers
-000008e0: 696f 6e73 2e79 616d 6c2f 6261 6467 652e  ions.yaml/badge.
-000008f0: 7376 673f 290a 5b21 5b70 7974 686f 6e5d  svg?).[![python]
-00000900: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000910: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-00000920: 7468 6f6e 5f33 2e37 2d70 6173 7369 6e67  thon_3.7-passing
-00000930: 2d73 7563 6365 7373 295d 2868 7474 7073  -success)](https
-00000940: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
-00000950: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
-00000960: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
-00000970: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
-00000980: 7468 6f6e 2d76 6572 7369 6f6e 732e 7961  thon-versions.ya
-00000990: 6d6c 2f62 6164 6765 2e73 7667 3f29 0a5b  ml/badge.svg?).[
-000009a0: 215b 7079 7468 6f6e 5d28 6874 7470 733a  ![python](https:
-000009b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000009c0: 2f62 6164 6765 2f70 7974 686f 6e5f 332e  /badge/python_3.
-000009d0: 382d 7061 7373 696e 672d 7375 6363 6573  8-passing-succes
-000009e0: 7329 5d28 6874 7470 733a 2f2f 6769 7468  s)](https://gith
-000009f0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00000a00: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00000a10: 6e69 6e67 2f61 6374 696f 6e73 2f77 6f72  ning/actions/wor
-00000a20: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7665  kflows/python-ve
-00000a30: 7273 696f 6e73 2e79 616d 6c2f 6261 6467  rsions.yaml/badg
-00000a40: 652e 7376 673f 290a 5b21 5b70 7974 686f  e.svg?).[![pytho
-00000a50: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-00000a60: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000a70: 7079 7468 6f6e 5f33 2e39 2d70 6173 7369  python_3.9-passi
-00000a80: 6e67 2d73 7563 6365 7373 295d 2868 7474  ng-success)](htt
-00000a90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000aa0: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
-00000ab0: 7472 6963 2d6c 6561 726e 696e 672f 6163  tric-learning/ac
-00000ac0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000ad0: 7079 7468 6f6e 2d76 6572 7369 6f6e 732e  python-versions.
-00000ae0: 7961 6d6c 2f62 6164 6765 2e73 7667 3f29  yaml/badge.svg?)
-00000af0: 0a5b 215b 7079 7468 6f6e 5d28 6874 7470  .[![python](http
-00000b00: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000b10: 696f 2f62 6164 6765 2f70 7974 686f 6e5f  io/badge/python_
-00000b20: 332e 3130 2d70 6173 7369 6e67 2d73 7563  3.10-passing-suc
-00000b30: 6365 7373 295d 2868 7474 7073 3a2f 2f67  cess)](https://g
-00000b40: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-00000b50: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-00000b60: 6561 726e 696e 672f 6163 7469 6f6e 732f  earning/actions/
-00000b70: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
-00000b80: 2d76 6572 7369 6f6e 732e 7961 6d6c 2f62  -versions.yaml/b
-00000b90: 6164 6765 2e73 7667 3f29 0a0a 3c64 6976  adge.svg?)..<div
-00000ba0: 2061 6c69 676e 3d22 6c65 6674 223e 0a0a   align="left">..
-00000bb0: 4f4d 4c20 6973 2061 2050 7954 6f72 6368  OML is a PyTorch
-00000bc0: 2d62 6173 6564 2066 7261 6d65 776f 726b  -based framework
-00000bd0: 2074 6f20 7472 6169 6e20 616e 6420 7661   to train and va
-00000be0: 6c69 6461 7465 2074 6865 206d 6f64 656c  lidate the model
-00000bf0: 7320 7072 6f64 7563 696e 6720 6869 6768  s producing high
-00000c00: 2d71 7561 6c69 7479 2065 6d62 6564 6469  -quality embeddi
-00000c10: 6e67 732e 0a0a 2323 205b 4641 515d 2868  ngs...## [FAQ](h
-00000c20: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
-00000c30: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
-00000c40: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000c50: 7465 7374 2f6f 6d6c 2f66 6171 2e68 746d  test/oml/faq.htm
-00000c60: 6c29 0a0a 3c64 6574 6169 6c73 3e0a 3c73  l)..<details>.<s
-00000c70: 756d 6d61 7279 3e57 6879 2064 6f20 4920  ummary>Why do I 
-00000c80: 6e65 6564 204f 4d4c 3f3c 2f73 756d 6d61  need OML?</summa
-00000c90: 7279 3e0a 3c70 3e0a 0a59 6f75 206d 6179  ry>.<p>..You may
-00000ca0: 2074 6869 6e6b 202a 2249 6620 4920 6e65   think *"If I ne
-00000cb0: 6564 2069 6d61 6765 2065 6d62 6564 6469  ed image embeddi
-00000cc0: 6e67 7320 4920 6361 6e20 7369 6d70 6c79  ngs I can simply
-00000cd0: 2074 7261 696e 2061 2076 616e 696c 6c61   train a vanilla
-00000ce0: 2063 6c61 7373 6966 6965 7220 616e 6420   classifier and 
-00000cf0: 7461 6b65 2069 7473 2070 656e 756c 7469  take its penulti
-00000d00: 6d61 7465 206c 6179 6572 222a 2e0a 5765  mate layer"*..We
-00000d10: 6c6c 2c20 6974 206d 616b 6573 2073 656e  ll, it makes sen
-00000d20: 7365 2061 7320 6120 7374 6172 7469 6e67  se as a starting
-00000d30: 2070 6f69 6e74 2e20 4275 7420 7468 6572   point. But ther
-00000d40: 6520 6172 6520 7365 7665 7261 6c20 706f  e are several po
-00000d50: 7373 6962 6c65 2064 7261 7762 6163 6b73  ssible drawbacks
-00000d60: 3a0a 0a2a 2049 6620 796f 7520 7761 6e74  :..* If you want
-00000d70: 2074 6f20 7573 6520 656d 6265 6464 696e   to use embeddin
-00000d80: 6773 2074 6f20 7065 7266 6f72 6d20 7365  gs to perform se
-00000d90: 6172 6368 696e 6720 796f 7520 6e65 6564  arching you need
-00000da0: 2074 6f20 6361 6c63 756c 6174 6520 736f   to calculate so
-00000db0: 6d65 2064 6973 7461 6e63 6520 616d 6f6e  me distance amon
-00000dc0: 6720 7468 656d 2028 666f 7220 6578 616d  g them (for exam
-00000dd0: 706c 652c 2063 6f73 696e 6520 6f72 204c  ple, cosine or L
-00000de0: 3229 2e0a 2020 5573 7561 6c6c 792c 202a  2)..  Usually, *
-00000df0: 2a79 6f75 2064 6f6e 2774 2064 6972 6563  *you don't direc
-00000e00: 746c 7920 6f70 7469 6d69 7a65 2074 6865  tly optimize the
-00000e10: 7365 2064 6973 7461 6e63 6573 2064 7572  se distances dur
-00000e20: 696e 6720 7468 6520 7472 6169 6e69 6e67  ing the training
-00000e30: 2a2a 2069 6e20 7468 6520 636c 6173 7369  ** in the classi
-00000e40: 6669 6361 7469 6f6e 2073 6574 7570 2e20  fication setup. 
-00000e50: 536f 2c20 796f 7520 6361 6e20 6f6e 6c79  So, you can only
-00000e60: 2068 6f70 6520 7468 6174 0a20 2066 696e   hope that.  fin
-00000e70: 616c 2065 6d62 6564 6469 6e67 7320 7769  al embeddings wi
-00000e80: 6c6c 2068 6176 6520 7468 6520 6465 7369  ll have the desi
-00000e90: 7265 6420 7072 6f70 6572 7469 6573 2e0a  red properties..
-00000ea0: 0a2a 202a 2a54 6865 2073 6563 6f6e 6420  .* **The second 
-00000eb0: 7072 6f62 6c65 6d20 6973 2074 6865 2076  problem is the v
-00000ec0: 616c 6964 6174 696f 6e20 7072 6f63 6573  alidation proces
-00000ed0: 732a 2a2e 0a20 2049 6e20 7468 6520 7365  s**..  In the se
-00000ee0: 6172 6368 696e 6720 7365 7475 702c 2079  arching setup, y
-00000ef0: 6f75 2075 7375 616c 6c79 2063 6172 6520  ou usually care 
-00000f00: 686f 7720 7265 6c61 7465 6420 796f 7572  how related your
-00000f10: 2074 6f70 2d4e 206f 7574 7075 7473 2061   top-N outputs a
-00000f20: 7265 2074 6f20 7468 6520 7175 6572 792e  re to the query.
-00000f30: 0a20 2054 6865 206e 6174 7572 616c 2077  .  The natural w
-00000f40: 6179 2074 6f20 6576 616c 7561 7465 2074  ay to evaluate t
-00000f50: 6865 206d 6f64 656c 2069 7320 746f 2073  he model is to s
-00000f60: 696d 756c 6174 6520 7365 6172 6368 696e  imulate searchin
-00000f70: 6720 7265 7175 6573 7473 2074 6f20 7468  g requests to th
-00000f80: 6520 7265 6665 7265 6e63 6520 7365 740a  e reference set.
-00000f90: 2020 616e 6420 6170 706c 7920 6f6e 6520    and apply one 
-00000fa0: 6f66 2074 6865 2072 6574 7269 6576 616c  of the retrieval
-00000fb0: 206d 6574 7269 6373 2e0a 2020 536f 2c20   metrics..  So, 
-00000fc0: 7468 6572 6520 6973 206e 6f20 6775 6172  there is no guar
-00000fd0: 616e 7465 6520 7468 6174 2063 6c61 7373  antee that class
-00000fe0: 6966 6963 6174 696f 6e20 6163 6375 7261  ification accura
-00000ff0: 6379 2077 696c 6c20 636f 7272 656c 6174  cy will correlat
-00001000: 6520 7769 7468 2074 6865 7365 206d 6574  e with these met
-00001010: 7269 6373 2e0a 0a2a 2046 696e 616c 6c79  rics...* Finally
-00001020: 2c20 796f 7520 6d61 7920 7761 6e74 2074  , you may want t
-00001030: 6f20 696d 706c 656d 656e 7420 6120 6d65  o implement a me
-00001040: 7472 6963 206c 6561 726e 696e 6720 7069  tric learning pi
-00001050: 7065 6c69 6e65 2062 7920 796f 7572 7365  peline by yourse
-00001060: 6c66 2e0a 2020 2a2a 5468 6572 6520 6973  lf..  **There is
-00001070: 2061 206c 6f74 206f 6620 776f 726b 2a2a   a lot of work**
-00001080: 3a20 746f 2075 7365 2074 7269 706c 6574  : to use triplet
-00001090: 206c 6f73 7320 796f 7520 6e65 6564 2074   loss you need t
-000010a0: 6f20 666f 726d 2062 6174 6368 6573 2069  o form batches i
-000010b0: 6e20 6120 7370 6563 6966 6963 2077 6179  n a specific way
-000010c0: 2c0a 2020 696d 706c 656d 656e 7420 6469  ,.  implement di
-000010d0: 6666 6572 656e 7420 6b69 6e64 7320 6f66  fferent kinds of
-000010e0: 2074 7269 706c 6574 7320 6d69 6e69 6e67   triplets mining
-000010f0: 2c20 7472 6163 6b69 6e67 2064 6973 7461  , tracking dista
-00001100: 6e63 6573 2c20 6574 632e 2046 6f72 2074  nces, etc. For t
-00001110: 6865 2076 616c 6964 6174 696f 6e2c 2079  he validation, y
-00001120: 6f75 2061 6c73 6f20 6e65 6564 2074 6f0a  ou also need to.
-00001130: 2020 696d 706c 656d 656e 7420 7265 7472    implement retr
-00001140: 6965 7661 6c20 6d65 7472 6963 732c 0a20  ieval metrics,. 
-00001150: 2077 6869 6368 2069 6e63 6c75 6465 2065   which include e
-00001160: 6666 6563 7469 7665 2065 6d62 6564 6469  ffective embeddi
-00001170: 6e67 7320 6163 6375 6d75 6c61 7469 6f6e  ngs accumulation
-00001180: 2064 7572 696e 6720 7468 6520 6570 6f63   during the epoc
-00001190: 682c 2063 6f76 6572 696e 6720 636f 726e  h, covering corn
-000011a0: 6572 2063 6173 6573 2c20 6574 632e 0a20  er cases, etc.. 
-000011b0: 2049 7427 7320 6576 656e 2068 6172 6465   It's even harde
-000011c0: 7220 6966 2079 6f75 2068 6176 6520 7365  r if you have se
-000011d0: 7665 7261 6c20 6770 7573 2061 6e64 2075  veral gpus and u
-000011e0: 7365 2044 4450 2e0a 2020 596f 7520 6d61  se DDP..  You ma
-000011f0: 7920 616c 736f 2077 616e 7420 746f 2076  y also want to v
-00001200: 6973 7561 6c69 7a65 2079 6f75 7220 7365  isualize your se
-00001210: 6172 6368 2072 6571 7565 7374 7320 6279  arch requests by
-00001220: 2068 6967 686c 6967 6874 696e 6720 676f   highlighting go
-00001230: 6f64 2061 6e64 2062 6164 2073 6561 7263  od and bad searc
-00001240: 6820 7265 7375 6c74 732e 0a20 2049 6e73  h results..  Ins
-00001250: 7465 6164 206f 6620 646f 696e 6720 6974  tead of doing it
-00001260: 2062 7920 796f 7572 7365 6c66 2c20 796f   by yourself, yo
-00001270: 7520 6361 6e20 7369 6d70 6c79 2075 7365  u can simply use
-00001280: 204f 4d4c 2066 6f72 2079 6f75 7220 7075   OML for your pu
-00001290: 7270 6f73 6573 2e0a 0a3c 2f70 3e0a 3c2f  rposes...</p>.</
-000012a0: 6465 7461 696c 733e 0a0a 0a3c 6465 7461  details>...<deta
-000012b0: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-000012c0: 6174 2069 7320 7468 6520 6469 6666 6572  at is the differ
-000012d0: 656e 6365 2062 6574 7765 656e 204f 7065  ence between Ope
-000012e0: 6e20 4d65 7472 6963 204c 6561 726e 696e  n Metric Learnin
-000012f0: 6720 616e 6420 5079 546f 7263 6820 4d65  g and PyTorch Me
-00001300: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
-00001310: 7375 6d6d 6172 793e 0a3c 703e 0a0a 5b50  summary>.<p>..[P
-00001320: 4d4c 5d28 6874 7470 733a 2f2f 6769 7468  ML](https://gith
-00001330: 7562 2e63 6f6d 2f4b 6576 696e 4d75 7367  ub.com/KevinMusg
-00001340: 7261 7665 2f70 7974 6f72 6368 2d6d 6574  rave/pytorch-met
-00001350: 7269 632d 6c65 6172 6e69 6e67 2920 6973  ric-learning) is
-00001360: 2074 6865 2070 6f70 756c 6172 206c 6962   the popular lib
-00001370: 7261 7279 2066 6f72 204d 6574 7269 6320  rary for Metric 
-00001380: 4c65 6172 6e69 6e67 2c0a 616e 6420 6974  Learning,.and it
-00001390: 2069 6e63 6c75 6465 7320 6120 7269 6368   includes a rich
-000013a0: 2063 6f6c 6c65 6374 696f 6e20 6f66 206c   collection of l
-000013b0: 6f73 7365 732c 206d 696e 6572 732c 2064  osses, miners, d
-000013c0: 6973 7461 6e63 6573 2c20 616e 6420 7265  istances, and re
-000013d0: 6475 6365 7273 3b20 7468 6174 2069 7320  ducers; that is 
-000013e0: 7768 7920 7765 2070 726f 7669 6465 2073  why we provide s
-000013f0: 7472 6169 6768 7466 6f72 7761 7264 0a5b  traightforward.[
-00001400: 6578 616d 706c 6573 5d28 6874 7470 733a  examples](https:
-00001410: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00001420: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00001430: 632d 6c65 6172 6e69 6e67 2375 7361 6765  c-learning#usage
-00001440: 2d77 6974 682d 7079 746f 7263 682d 6d65  -with-pytorch-me
-00001450: 7472 6963 2d6c 6561 726e 696e 6729 206f  tric-learning) o
-00001460: 6620 7573 696e 6720 7468 656d 2077 6974  f using them wit
-00001470: 6820 4f4d 4c2e 0a49 6e69 7469 616c 6c79  h OML..Initially
-00001480: 2c20 7765 2074 7269 6564 2074 6f20 7573  , we tried to us
-00001490: 6520 504d 4c2c 2062 7574 2069 6e20 7468  e PML, but in th
-000014a0: 6520 656e 642c 2077 6520 6361 6d65 2075  e end, we came u
-000014b0: 7020 7769 7468 206f 7572 206c 6962 7261  p with our libra
-000014c0: 7279 2c20 7768 6963 6820 6973 206d 6f72  ry, which is mor
-000014d0: 6520 7069 7065 6c69 6e65 202f 2072 6563  e pipeline / rec
-000014e0: 6970 6573 206f 7269 656e 7465 642e 0a54  ipes oriented..T
-000014f0: 6861 7420 6973 2068 6f77 204f 4d4c 2064  hat is how OML d
-00001500: 6966 6665 7273 2066 726f 6d20 504d 4c3a  iffers from PML:
-00001510: 0a0a 2a20 4f4d 4c20 6861 7320 5b50 6970  ..* OML has [Pip
-00001520: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00001530: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-00001540: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00001550: 6c65 6172 6e69 6e67 2f74 7265 652f 6d61  learning/tree/ma
-00001560: 696e 2f70 6970 656c 696e 6573 290a 2020  in/pipelines).  
-00001570: 7768 6963 6820 616c 6c6f 7773 2074 7261  which allows tra
-00001580: 696e 696e 6720 6d6f 6465 6c73 2062 7920  ining models by 
-00001590: 7072 6570 6172 696e 6720 6120 636f 6e66  preparing a conf
-000015a0: 6967 2061 6e64 2079 6f75 7220 6461 7461  ig and your data
-000015b0: 2069 6e20 7468 6520 7265 7175 6972 6564   in the required
-000015c0: 2066 6f72 6d61 740a 2020 2869 7427 7320   format.  (it's 
-000015d0: 6c69 6b65 2063 6f6e 7665 7274 696e 6720  like converting 
-000015e0: 6461 7461 2069 6e74 6f20 434f 434f 2066  data into COCO f
-000015f0: 6f72 6d61 7420 746f 2074 7261 696e 2061  ormat to train a
-00001600: 2064 6574 6563 746f 7220 6672 6f6d 205b   detector from [
-00001610: 6d6d 6465 7465 6374 696f 6e5d 2868 7474  mmdetection](htt
-00001620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001630: 6f70 656e 2d6d 6d6c 6162 2f6d 6d64 6574  open-mmlab/mmdet
-00001640: 6563 7469 6f6e 2929 2e0a 0a2a 204f 4d4c  ection))...* OML
-00001650: 2066 6f63 7573 6573 206f 6e20 656e 642d   focuses on end-
-00001660: 746f 2d65 6e64 2070 6970 656c 696e 6573  to-end pipelines
-00001670: 2061 6e64 2070 7261 6374 6963 616c 2075   and practical u
-00001680: 7365 2063 6173 6573 2e0a 2020 4974 2068  se cases..  It h
-00001690: 6173 2063 6f6e 6669 6720 6261 7365 6420  as config based 
-000016a0: 6578 616d 706c 6573 206f 6e20 706f 7075  examples on popu
-000016b0: 6c61 7220 6265 6e63 686d 6172 6b73 2063  lar benchmarks c
-000016c0: 6c6f 7365 2074 6f20 7265 616c 206c 6966  lose to real lif
-000016d0: 6520 286c 696b 6520 7068 6f74 6f73 206f  e (like photos o
-000016e0: 6620 7072 6f64 7563 7473 206f 6620 7468  f products of th
-000016f0: 6f75 7361 6e64 7320 6964 7329 2e0a 2020  ousands ids)..  
-00001700: 5765 2066 6f75 6e64 2073 6f6d 6520 676f  We found some go
-00001710: 6f64 2063 6f6d 6269 6e61 7469 6f6e 7320  od combinations 
-00001720: 6f66 2068 7970 6572 7061 7261 6d65 7465  of hyperparamete
-00001730: 7273 206f 6e20 7468 6573 6520 6461 7461  rs on these data
-00001740: 7365 7473 2c20 7472 6169 6e65 6420 616e  sets, trained an
-00001750: 6420 7075 626c 6973 6865 6420 6d6f 6465  d published mode
-00001760: 6c73 2061 6e64 2074 6865 6972 2063 6f6e  ls and their con
-00001770: 6669 6773 2e0a 2020 5468 7573 2c20 6974  figs..  Thus, it
-00001780: 206d 616b 6573 204f 4d4c 206d 6f72 6520   makes OML more 
-00001790: 7265 6369 7065 7320 6f72 6965 6e74 6564  recipes oriented
-000017a0: 2074 6861 6e20 504d 4c2c 2061 6e64 2069   than PML, and i
-000017b0: 7473 2061 7574 686f 720a 2020 5b63 6f6e  ts author.  [con
-000017c0: 6669 726d 735d 2868 7474 7073 3a2f 2f67  firms](https://g
-000017d0: 6974 6875 622e 636f 6d2f 4b65 7669 6e4d  ithub.com/KevinM
-000017e0: 7573 6772 6176 652f 7079 746f 7263 682d  usgrave/pytorch-
-000017f0: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
-00001800: 6973 7375 6573 2f31 3639 2369 7373 7565  issues/169#issue
-00001810: 636f 6d6d 656e 742d 3637 3038 3134 3339  comment-67081439
-00001820: 3329 0a20 2074 6869 7320 7361 7969 6e67  3).  this saying
-00001830: 2074 6861 7420 6869 7320 6c69 6272 6172   that his librar
-00001840: 7920 6973 2061 2073 6574 206f 6620 746f  y is a set of to
-00001850: 6f6c 7320 7261 7468 6572 2074 6865 2072  ols rather the r
-00001860: 6563 6970 6573 2c20 6d6f 7265 6f76 6572  ecipes, moreover
-00001870: 2c20 7468 6520 6578 616d 706c 6573 2069  , the examples i
-00001880: 6e20 504d 4c20 6172 6520 6d6f 7374 6c79  n PML are mostly
-00001890: 2066 6f72 2043 4946 4152 2061 6e64 204d   for CIFAR and M
-000018a0: 4e49 5354 2064 6174 6173 6574 732e 0a0a  NIST datasets...
-000018b0: 2a20 4f4d 4c20 6861 7320 7468 6520 5b5a  * OML has the [Z
-000018c0: 6f6f 5d28 6874 7470 733a 2f2f 6769 7468  oo](https://gith
-000018d0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-000018e0: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-000018f0: 6e69 6e67 237a 6f6f 2920 6f66 2070 7265  ning#zoo) of pre
-00001900: 7472 6169 6e65 6420 6d6f 6465 6c73 2074  trained models t
-00001910: 6861 7420 6361 6e20 6265 2065 6173 696c  hat can be easil
-00001920: 7920 6163 6365 7373 6564 2066 726f 6d0a  y accessed from.
-00001930: 2020 7468 6520 636f 6465 2069 6e20 7468    the code in th
-00001940: 6520 7361 6d65 2077 6179 2061 7320 696e  e same way as in
-00001950: 2060 746f 7263 6876 6973 696f 6e60 2028   `torchvision` (
-00001960: 7768 656e 2079 6f75 2074 7970 6520 6072  when you type `r
-00001970: 6573 6e65 7435 3028 7072 6574 7261 696e  esnet50(pretrain
-00001980: 6564 3d54 7275 6529 6029 2e0a 0a2a 204f  ed=True)`)...* O
-00001990: 4d4c 2069 7320 696e 7465 6772 6174 6564  ML is integrated
-000019a0: 2077 6974 6820 5b50 7954 6f72 6368 204c   with [PyTorch L
-000019b0: 6967 6874 6e69 6e67 5d28 6874 7470 733a  ightning](https:
-000019c0: 2f2f 7777 772e 7079 746f 7263 686c 6967  //www.pytorchlig
-000019d0: 6874 6e69 6e67 2e61 692f 292c 2073 6f2c  htning.ai/), so,
-000019e0: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
-000019f0: 706f 7765 7220 6f66 2069 7473 0a20 205b  power of its.  [
-00001a00: 5472 6169 6e65 725d 2868 7474 7073 3a2f  Trainer](https:/
-00001a10: 2f70 7974 6f72 6368 2d6c 6967 6874 6e69  /pytorch-lightni
-00001a20: 6e67 2e72 6561 6474 6865 646f 6373 2e69  ng.readthedocs.i
-00001a30: 6f2f 656e 2f73 7461 626c 652f 636f 6d6d  o/en/stable/comm
-00001a40: 6f6e 2f74 7261 696e 6572 2e68 746d 6c29  on/trainer.html)
-00001a50: 2e0a 2020 5468 6973 2069 7320 6573 7065  ..  This is espe
-00001a60: 6369 616c 6c79 2068 656c 7066 756c 2077  cially helpful w
-00001a70: 6865 6e20 7765 2077 6f72 6b20 7769 7468  hen we work with
-00001a80: 2044 4450 2c20 736f 2c20 796f 7520 636f   DDP, so, you co
-00001a90: 6d70 6172 6520 6f75 720a 2020 5b44 4450  mpare our.  [DDP
-00001aa0: 2065 7861 6d70 6c65 5d28 6874 7470 733a   example](https:
-00001ab0: 2f2f 6f70 656e 2d6d 6574 7269 632d 6c65  //open-metric-le
-00001ac0: 6172 6e69 6e67 2e72 6561 6474 6865 646f  arning.readthedo
-00001ad0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001ae0: 6578 616d 706c 6573 2f70 7974 686f 6e2e  examples/python.
-00001af0: 6874 6d6c 290a 2020 616e 6420 7468 650a  html).  and the.
-00001b00: 2020 5b50 4d4c 7320 6f6e 655d 2868 7474    [PMLs one](htt
-00001b10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001b20: 4b65 7669 6e4d 7573 6772 6176 652f 7079  KevinMusgrave/py
-00001b30: 746f 7263 682d 6d65 7472 6963 2d6c 6561  torch-metric-lea
-00001b40: 726e 696e 672f 626c 6f62 2f6d 6173 7465  rning/blob/maste
-00001b50: 722f 6578 616d 706c 6573 2f6e 6f74 6562  r/examples/noteb
-00001b60: 6f6f 6b73 2f44 6973 7472 6962 7574 6564  ooks/Distributed
-00001b70: 5472 6970 6c65 744d 6172 6769 6e4c 6f73  TripletMarginLos
-00001b80: 734d 4e49 5354 2e69 7079 6e62 292e 0a20  sMNIST.ipynb).. 
-00001b90: 2042 7920 7468 6520 7761 792c 2050 4d4c   By the way, PML
-00001ba0: 2061 6c73 6f20 6861 7320 5b54 7261 696e   also has [Train
-00001bb0: 6572 735d 2868 7474 7073 3a2f 2f6b 6576  ers](https://kev
-00001bc0: 696e 6d75 7367 7261 7665 2e67 6974 6875  inmusgrave.githu
-00001bd0: 622e 696f 2f70 7974 6f72 6368 2d6d 6574  b.io/pytorch-met
-00001be0: 7269 632d 6c65 6172 6e69 6e67 2f74 7261  ric-learning/tra
-00001bf0: 696e 6572 732f 292c 2062 7574 2069 7427  iners/), but it'
-00001c00: 7320 6e6f 740a 2020 7769 6465 6c79 2075  s not.  widely u
-00001c10: 7365 6420 696e 2074 6865 2065 7861 6d70  sed in the examp
-00001c20: 6c65 7320 616e 6420 6375 7374 6f6d 2060  les and custom `
-00001c30: 7472 6169 6e60 202f 2060 7465 7374 6020  train` / `test` 
-00001c40: 6675 6e63 7469 6f6e 7320 6172 6520 7573  functions are us
-00001c50: 6564 2069 6e73 7465 6164 2e0a 0a57 6520  ed instead...We 
-00001c60: 6265 6c69 6576 6520 7468 6174 2068 6176  believe that hav
-00001c70: 696e 6720 5069 7065 6c69 6e65 732c 206c  ing Pipelines, l
-00001c80: 6163 6f6e 6963 2065 7861 6d70 6c65 732c  aconic examples,
-00001c90: 2061 6e64 205a 6f6f 206f 6620 7072 6574   and Zoo of pret
-00001ca0: 7261 696e 6564 206d 6f64 656c 7320 7365  rained models se
-00001cb0: 7473 2074 6865 2065 6e74 7279 2074 6872  ts the entry thr
-00001cc0: 6573 686f 6c64 2074 6f20 6120 7265 616c  eshold to a real
-00001cd0: 6c79 206c 6f77 2076 616c 7565 2e0a 0a3c  ly low value...<
-00001ce0: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
-00001cf0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
-00001d00: 6172 793e 5768 6174 2069 7320 4d65 7472  ary>What is Metr
-00001d10: 6963 204c 6561 726e 696e 673f 3c2f 7375  ic Learning?</su
-00001d20: 6d6d 6172 793e 0a3c 703e 0a0a 4d65 7472  mmary>.<p>..Metr
-00001d30: 6963 204c 6561 726e 696e 6720 7072 6f62  ic Learning prob
-00001d40: 6c65 6d20 2861 6c73 6f20 6b6e 6f77 6e20  lem (also known 
-00001d50: 6173 202a 6578 7472 656d 6520 636c 6173  as *extreme clas
-00001d60: 7369 6669 6361 7469 6f6e 2a20 7072 6f62  sification* prob
-00001d70: 6c65 6d29 206d 6561 6e73 2061 2073 6974  lem) means a sit
-00001d80: 7561 7469 6f6e 2069 6e20 7768 6963 6820  uation in which 
-00001d90: 7765 0a68 6176 6520 7468 6f75 7361 6e64  we.have thousand
-00001da0: 7320 6f66 2069 6473 206f 6620 736f 6d65  s of ids of some
-00001db0: 2065 6e74 6974 6965 732c 2062 7574 206f   entities, but o
-00001dc0: 6e6c 7920 6120 6665 7720 7361 6d70 6c65  nly a few sample
-00001dd0: 7320 666f 7220 6576 6572 7920 656e 7469  s for every enti
-00001de0: 7479 2e0a 4f66 7465 6e20 7765 2061 7373  ty..Often we ass
-00001df0: 756d 6520 7468 6174 2064 7572 696e 6720  ume that during 
-00001e00: 7468 6520 7465 7374 2073 7461 6765 2028  the test stage (
-00001e10: 6f72 2070 726f 6475 6374 696f 6e29 2077  or production) w
-00001e20: 6520 7769 6c6c 2064 6561 6c20 7769 7468  e will deal with
-00001e30: 2075 6e73 6565 6e20 656e 7469 7469 6573   unseen entities
-00001e40: 0a77 6869 6368 206d 616b 6573 2069 7420  .which makes it 
-00001e50: 696d 706f 7373 6962 6c65 2074 6f20 6170  impossible to ap
-00001e60: 706c 7920 7468 6520 7661 6e69 6c6c 6120  ply the vanilla 
-00001e70: 636c 6173 7369 6669 6361 7469 6f6e 2070  classification p
-00001e80: 6970 656c 696e 6520 6469 7265 6374 6c79  ipeline directly
-00001e90: 2e20 496e 206d 616e 7920 6361 7365 7320  . In many cases 
-00001ea0: 6f62 7461 696e 6564 2065 6d62 6564 6469  obtained embeddi
-00001eb0: 6e67 730a 6172 6520 7573 6564 2074 6f20  ngs.are used to 
-00001ec0: 7065 7266 6f72 6d20 7365 6172 6368 206f  perform search o
-00001ed0: 7220 6d61 7463 6869 6e67 2070 726f 6365  r matching proce
-00001ee0: 6475 7265 7320 6f76 6572 2074 6865 6d2e  dures over them.
-00001ef0: 0a0a 4865 7265 2061 7265 2061 2066 6577  ..Here are a few
-00001f00: 2065 7861 6d70 6c65 7320 6f66 2073 7563   examples of suc
-00001f10: 6820 7461 736b 7320 6672 6f6d 2074 6865  h tasks from the
-00001f20: 2063 6f6d 7075 7465 7220 7669 7369 6f6e   computer vision
-00001f30: 2073 7068 6572 653a 0a2a 2050 6572 736f   sphere:.* Perso
-00001f40: 6e2f 416e 696d 616c 2052 652d 4964 656e  n/Animal Re-Iden
-00001f50: 7469 6669 6361 7469 6f6e 0a2a 2046 6163  tification.* Fac
-00001f60: 6520 5265 636f 676e 6974 696f 6e0a 2a20  e Recognition.* 
-00001f70: 4c61 6e64 6d61 726b 2052 6563 6f67 6e69  Landmark Recogni
-00001f80: 7469 6f6e 0a2a 2053 6561 7263 6869 6e67  tion.* Searching
-00001f90: 2065 6e67 696e 6573 2066 6f72 206f 6e6c   engines for onl
-00001fa0: 696e 6520 7368 6f70 730a 2061 6e64 206d  ine shops. and m
-00001fb0: 616e 7920 6f74 6865 7273 2e0a 3c2f 703e  any others..</p>
-00001fc0: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
-00001fd0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00001fe0: 3e47 6c6f 7373 6172 7920 284e 616d 696e  >Glossary (Namin
-00001ff0: 6720 636f 6e76 656e 7469 6f6e 2920 3c2f  g convention) </
-00002000: 7375 6d6d 6172 793e 0a3c 703e 0a0a 2a20  summary>.<p>..* 
-00002010: 6065 6d62 6564 6469 6e67 6020 2d20 6d6f  `embedding` - mo
-00002020: 6465 6c27 7320 6f75 7470 7574 2028 616c  del's output (al
-00002030: 736f 206b 6e6f 776e 2061 7320 6066 6561  so known as `fea
-00002040: 7475 7265 7320 7665 6374 6f72 6020 6f72  tures vector` or
-00002050: 2060 6465 7363 7269 7074 6f72 6029 2e0a   `descriptor`)..
-00002060: 2a20 6071 7565 7279 6020 2d20 6120 7361  * `query` - a sa
-00002070: 6d70 6c65 2077 6869 6368 2069 7320 7573  mple which is us
-00002080: 6564 2061 7320 6120 7265 7175 6573 7420  ed as a request 
-00002090: 696e 2074 6865 2072 6574 7269 6576 616c  in the retrieval
-000020a0: 2070 726f 6365 6475 7265 2e0a 2a20 6067   procedure..* `g
-000020b0: 616c 6c65 7279 2073 6574 6020 2d20 7468  allery set` - th
-000020c0: 6520 7365 7420 6f66 2065 6e74 6974 6965  e set of entitie
-000020d0: 7320 746f 2073 6561 7263 6820 6974 656d  s to search item
-000020e0: 7320 7369 6d69 6c61 7220 746f 2060 7175  s similar to `qu
-000020f0: 6572 7960 2028 616c 736f 206b 6e6f 776e  ery` (also known
-00002100: 2061 7320 6072 6566 6572 656e 6365 6020   as `reference` 
-00002110: 6f72 2060 696e 6465 7860 292e 0a2a 2060  or `index`)..* `
-00002120: 5361 6d70 6c65 7260 202d 2061 6e20 6172  Sampler` - an ar
-00002130: 6775 6d65 6e74 2066 6f72 2060 4461 7461  gument for `Data
-00002140: 4c6f 6164 6572 6020 7768 6963 6820 6973  Loader` which is
-00002150: 2075 7365 6420 746f 2066 6f72 6d20 6261   used to form ba
-00002160: 7463 6865 730a 2a20 604d 696e 6572 6020  tches.* `Miner` 
-00002170: 2d20 7468 6520 6f62 6a65 6374 2074 6f20  - the object to 
-00002180: 666f 726d 2070 6169 7273 206f 7220 7472  form pairs or tr
-00002190: 6970 6c65 7473 2061 6674 6572 2074 6865  iplets after the
-000021a0: 2062 6174 6368 2077 6173 2066 6f72 6d65   batch was forme
-000021b0: 6420 6279 2060 5361 6d70 6c65 7260 2e20  d by `Sampler`. 
-000021c0: 4974 2773 206e 6f74 206e 6563 6573 7361  It's not necessa
-000021d0: 7279 2074 6f20 666f 726d 0a20 2074 6865  ry to form.  the
-000021e0: 2063 6f6d 6269 6e61 7469 6f6e 7320 6f66   combinations of
-000021f0: 2073 616d 706c 6573 206f 6e6c 7920 696e   samples only in
-00002200: 7369 6465 2074 6865 2063 7572 7265 6e74  side the current
-00002210: 2062 6174 6368 2c20 7468 7573 2c20 7468   batch, thus, th
-00002220: 6520 6d65 6d6f 7279 2062 616e 6b20 6d61  e memory bank ma
-00002230: 7920 6265 2061 2070 6172 7420 6f66 2060  y be a part of `
-00002240: 4d69 6e65 7260 2e0a 2a20 6053 616d 706c  Miner`..* `Sampl
-00002250: 6573 602f 604c 6162 656c 7360 2f60 496e  es`/`Labels`/`In
-00002260: 7374 616e 6365 7360 202d 2061 7320 616e  stances` - as an
-00002270: 2065 7861 6d70 6c65 206c 6574 2773 2063   example let's c
-00002280: 6f6e 7369 6465 7220 4465 6570 4661 7368  onsider DeepFash
-00002290: 696f 6e20 6461 7461 7365 742e 2049 7420  ion dataset. It 
-000022a0: 696e 636c 7564 6573 2074 686f 7573 616e  includes thousan
-000022b0: 6473 206f 660a 2020 6661 7368 696f 6e20  ds of.  fashion 
-000022c0: 6974 656d 2069 6473 2028 7765 206e 616d  item ids (we nam
-000022d0: 6520 7468 656d 2060 6c61 6265 6c73 6029  e them `labels`)
-000022e0: 2061 6e64 2073 6576 6572 616c 2070 686f   and several pho
-000022f0: 746f 7320 666f 7220 6561 6368 2069 7465  tos for each ite
-00002300: 6d20 6964 0a20 2028 7765 206e 616d 6520  m id.  (we name 
-00002310: 7468 6520 696e 6469 7669 6475 616c 2070  the individual p
-00002320: 686f 746f 2061 7320 6069 6e73 7461 6e63  hoto as `instanc
-00002330: 6560 206f 7220 6073 616d 706c 6560 292e  e` or `sample`).
-00002340: 2041 6c6c 206f 6620 7468 6520 6661 7368   All of the fash
-00002350: 696f 6e20 6974 656d 2069 6473 2068 6176  ion item ids hav
-00002360: 6520 7468 6569 7220 6772 6f75 7073 206c  e their groups l
-00002370: 696b 650a 2020 2273 6b69 7274 7322 2c20  ike.  "skirts", 
-00002380: 226a 6163 6b65 7473 222c 2022 7368 6f72  "jackets", "shor
-00002390: 7473 2220 616e 6420 736f 206f 6e20 2877  ts" and so on (w
-000023a0: 6520 6e61 6d65 2074 6865 6d20 6063 6174  e name them `cat
-000023b0: 6567 6f72 6965 7360 292e 0a20 204e 6f74  egories`)..  Not
-000023c0: 652c 2077 6520 6176 6f69 6420 7573 696e  e, we avoid usin
-000023d0: 6720 7468 6520 7465 726d 2060 636c 6173  g the term `clas
-000023e0: 7360 2074 6f20 6176 6f69 6420 6d69 7375  s` to avoid misu
-000023f0: 6e64 6572 7374 616e 6469 6e67 2e0a 2a20  nderstanding..* 
-00002400: 6074 7261 696e 696e 6720 6570 6f63 6860  `training epoch`
-00002410: 202d 2062 6174 6368 2073 616d 706c 6572   - batch sampler
-00002420: 7320 7768 6963 6820 7765 2075 7365 2066  s which we use f
-00002430: 6f72 2063 6f6d 6269 6e61 7469 6f6e 2d62  or combination-b
-00002440: 6173 6564 206c 6f73 7365 7320 7573 7561  ased losses usua
-00002450: 6c6c 7920 6861 7665 2061 206c 656e 6774  lly have a lengt
-00002460: 6820 6571 7561 6c20 746f 0a20 2060 5b6e  h equal to.  `[n
-00002470: 756d 6265 7220 6f66 206c 6162 656c 7320  umber of labels 
-00002480: 696e 2074 7261 696e 696e 6720 6461 7461  in training data
-00002490: 7365 745d 202f 205b 6e75 6d62 6572 7320  set] / [numbers 
-000024a0: 6f66 206c 6162 656c 7320 696e 206f 6e65  of labels in one
-000024b0: 2062 6174 6368 5d60 2e20 4974 206d 6561   batch]`. It mea
-000024c0: 6e73 2074 6861 7420 7765 2064 6f6e 2774  ns that we don't
-000024d0: 206f 6273 6572 7665 2061 6c6c 206f 660a   observe all of.
-000024e0: 2020 7468 6520 6176 6169 6c61 626c 6520    the available 
-000024f0: 7472 6169 6e69 6e67 2073 616d 706c 6573  training samples
-00002500: 2069 6e20 6f6e 6520 6570 6f63 6820 2861   in one epoch (a
-00002510: 7320 6f70 706f 7365 6420 746f 2076 616e  s opposed to van
-00002520: 696c 6c61 2063 6c61 7373 6966 6963 6174  illa classificat
-00002530: 696f 6e29 2c0a 2020 696e 7374 6561 642c  ion),.  instead,
-00002540: 2077 6520 6f62 7365 7276 6520 616c 6c20   we observe all 
-00002550: 6f66 2074 6865 2061 7661 696c 6162 6c65  of the available
-00002560: 206c 6162 656c 732e 0a0a 3c2f 703e 0a3c   labels...</p>.<
-00002570: 2f64 6574 6169 6c73 3e0a 0a0a 3c64 6574  /details>...<det
-00002580: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e48  ails>.<summary>H
-00002590: 6f77 2067 6f6f 6420 6d61 7920 6265 2061  ow good may be a
-000025a0: 206d 6f64 656c 2074 7261 696e 6564 2077   model trained w
-000025b0: 6974 6820 4f4d 4c3f 203c 2f73 756d 6d61  ith OML? </summa
-000025c0: 7279 3e0a 3c70 3e0a 0a49 7420 6d61 7920  ry>.<p>..It may 
-000025d0: 6265 2063 6f6d 7061 7261 626c 6520 7769  be comparable wi
-000025e0: 7468 2074 6865 2063 7572 7265 6e74 2028  th the current (
-000025f0: 3230 3232 2079 6561 7229 205b 536f 7441  2022 year) [SotA
-00002600: 5d28 6874 7470 733a 2f2f 7061 7065 7273  ](https://papers
-00002610: 7769 7468 636f 6465 2e63 6f6d 2f74 6173  withcode.com/tas
-00002620: 6b2f 6d65 7472 6963 2d6c 6561 726e 696e  k/metric-learnin
-00002630: 6729 206d 6574 686f 6473 2c0a 666f 7220  g) methods,.for 
-00002640: 6578 616d 706c 652c 205b 4879 702d 5669  example, [Hyp-Vi
-00002650: 545d 2868 7474 7073 3a2f 2f61 7278 6976  T](https://arxiv
-00002660: 2e6f 7267 2f70 6466 2f32 3230 332e 3130  .org/pdf/2203.10
-00002670: 3833 332e 7064 6629 2e0a 2a28 4665 7720  833.pdf)..*(Few 
-00002680: 776f 7264 7320 6162 6f75 7420 7468 6973  words about this
-00002690: 2061 7070 726f 6163 683a 2069 7427 7320   approach: it's 
-000026a0: 6120 5669 5420 6172 6368 6974 6563 7475  a ViT architectu
-000026b0: 7265 2074 7261 696e 6564 2077 6974 6820  re trained with 
-000026c0: 636f 6e74 7261 7374 6976 6520 6c6f 7373  contrastive loss
-000026d0: 2c0a 6275 7420 7468 6520 656d 6265 6464  ,.but the embedd
-000026e0: 696e 6773 2077 6572 6520 7072 6f6a 6563  ings were projec
-000026f0: 7465 6420 696e 746f 2073 6f6d 6520 6879  ted into some hy
-00002700: 7065 7262 6f6c 6963 2073 7061 6365 2e0a  perbolic space..
-00002710: 4173 2074 6865 2061 7574 686f 7273 2063  As the authors c
-00002720: 6c61 696d 6564 2c20 7375 6368 2061 2073  laimed, such a s
-00002730: 7061 6365 2069 7320 6162 6c65 2074 6f20  pace is able to 
-00002740: 6465 7363 7269 6265 2074 6865 206e 6573  describe the nes
-00002750: 7465 6420 7374 7275 6374 7572 6520 6f66  ted structure of
-00002760: 2072 6561 6c2d 776f 726c 6420 6461 7461   real-world data
-00002770: 2e0a 536f 2c20 7468 6520 7061 7065 7220  ..So, the paper 
-00002780: 7265 7175 6972 6573 2073 6f6d 6520 6865  requires some he
-00002790: 6176 7920 6d61 7468 2074 6f20 6164 6170  avy math to adap
-000027a0: 7420 7468 6520 7573 7561 6c20 6f70 6572  t the usual oper
-000027b0: 6174 696f 6e73 2066 6f72 2074 6865 2068  ations for the h
-000027c0: 7970 6572 626f 6c69 6361 6c20 7370 6163  yperbolical spac
-000027d0: 652e 292a 0a0a 5765 2074 7261 696e 6564  e.)*..We trained
-000027e0: 2074 6865 2073 616d 6520 6172 6368 6974   the same archit
-000027f0: 6563 7475 7265 2077 6974 6820 7472 6970  ecture with trip
-00002800: 6c65 7420 6c6f 7373 2c20 6669 7869 6e67  let loss, fixing
-00002810: 2074 6865 2072 6573 7420 6f66 2074 6865   the rest of the
-00002820: 2070 6172 616d 6574 6572 733a 0a74 7261   parameters:.tra
-00002830: 696e 696e 6720 616e 6420 7465 7374 2074  ining and test t
-00002840: 7261 6e73 666f 726d 6174 696f 6e73 2c20  ransformations, 
-00002850: 696d 6167 6520 7369 7a65 2c20 616e 6420  image size, and 
-00002860: 6f70 7469 6d69 7a65 722e 2053 6565 2063  optimizer. See c
-00002870: 6f6e 6669 6773 2069 6e20 5b4d 6f64 656c  onfigs in [Model
-00002880: 7320 5a6f 6f5d 2868 7474 7073 3a2f 2f67  s Zoo](https://g
-00002890: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-000028a0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-000028b0: 6561 726e 696e 6723 7a6f 6f29 2e0a 5468  earning#zoo)..Th
-000028c0: 6520 7472 6963 6b20 7761 7320 696e 2068  e trick was in h
-000028d0: 6575 7269 7374 6963 7320 696e 206f 7572  euristics in our
-000028e0: 206d 696e 6572 2061 6e64 2073 616d 706c   miner and sampl
-000028f0: 6572 3a0a 0a2a 205b 4361 7465 676f 7279  er:..* [Category
-00002900: 2042 616c 616e 6365 2053 616d 706c 6572   Balance Sampler
-00002910: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00002920: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00002930: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00002940: 2f6c 6174 6573 742f 636f 6e74 656e 7473  /latest/contents
-00002950: 2f73 616d 706c 6572 732e 6874 6d6c 2363  /samplers.html#c
-00002960: 6174 6567 6f72 7962 616c 616e 6365 7361  ategorybalancesa
-00002970: 6d70 6c65 7229 0a20 2066 6f72 6d73 2074  mpler).  forms t
-00002980: 6865 2062 6174 6368 6573 206c 696d 6974  he batches limit
-00002990: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
-000029a0: 6620 6361 7465 676f 7269 6573 202a 432a  f categories *C*
-000029b0: 2069 6e20 6974 2e0a 2020 466f 7220 696e   in it..  For in
-000029c0: 7374 616e 6365 2c20 7768 656e 202a 4320  stance, when *C 
-000029d0: 3d20 312a 2069 7420 7075 7473 206f 6e6c  = 1* it puts onl
-000029e0: 7920 6a61 636b 6574 7320 696e 206f 6e65  y jackets in one
-000029f0: 2062 6174 6368 2061 6e64 206f 6e6c 7920   batch and only 
-00002a00: 6a65 616e 7320 696e 746f 2061 6e6f 7468  jeans into anoth
-00002a10: 6572 206f 6e65 2028 6a75 7374 2061 6e20  er one (just an 
-00002a20: 6578 616d 706c 6529 2e0a 2020 4974 2061  example)..  It a
-00002a30: 7574 6f6d 6174 6963 616c 6c79 206d 616b  utomatically mak
-00002a40: 6573 2074 6865 206e 6567 6174 6976 6520  es the negative 
-00002a50: 7061 6972 7320 6861 7264 6572 3a20 6974  pairs harder: it
-00002a60: 2773 206d 6f72 6520 6d65 616e 696e 6766  's more meaningf
-00002a70: 756c 2066 6f72 2061 206d 6f64 656c 2074  ul for a model t
-00002a80: 6f20 7265 616c 6973 6520 7768 7920 7477  o realise why tw
-00002a90: 6f20 6a61 636b 6574 730a 2020 6172 6520  o jackets.  are 
-00002aa0: 6469 6666 6572 656e 7420 7468 616e 2074  different than t
-00002ab0: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00002ac0: 2073 616d 6520 6162 6f75 7420 6120 6a61   same about a ja
-00002ad0: 636b 6574 2061 6e64 2061 2074 2d73 6869  cket and a t-shi
-00002ae0: 7274 2e0a 0a2a 205b 4861 7264 2054 7269  rt...* [Hard Tri
-00002af0: 706c 6574 7320 4d69 6e65 725d 2868 7474  plets Miner](htt
-00002b00: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-00002b10: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-00002b20: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00002b30: 7374 2f63 6f6e 7465 6e74 732f 6d69 6e65  st/contents/mine
-00002b40: 7273 2e68 746d 6c23 6861 7264 7472 6970  rs.html#hardtrip
-00002b50: 6c65 7473 6d69 6e65 7229 0a20 206d 616b  letsminer).  mak
-00002b60: 6573 2074 6865 2074 6173 6b20 6576 656e  es the task even
-00002b70: 2068 6172 6465 7220 6b65 6570 696e 6720   harder keeping 
-00002b80: 6f6e 6c79 2074 6865 2068 6172 6465 7374  only the hardest
-00002b90: 2074 7269 706c 6574 7320 2877 6974 6820   triplets (with 
-00002ba0: 6d61 7869 6d61 6c20 706f 7369 7469 7665  maximal positive
-00002bb0: 2061 6e64 206d 696e 696d 616c 206e 6567   and minimal neg
-00002bc0: 6174 6976 6520 6469 7374 616e 6365 7329  ative distances)
-00002bd0: 2e0a 0a48 6572 6520 6172 6520 2a43 4d43  ...Here are *CMC
-00002be0: 4031 2a20 7363 6f72 6573 2066 6f72 2032  @1* scores for 2
-00002bf0: 2070 6f70 756c 6172 2062 656e 6368 6d61   popular benchma
-00002c00: 726b 732e 0a53 4f50 2064 6174 6173 6574  rks..SOP dataset
-00002c10: 3a20 4879 702d 5669 5420 e280 9420 3835  : Hyp-ViT ... 85
-00002c20: 2e39 2c20 6f75 7273 20e2 8094 2038 362e  .9, ours ... 86.
-00002c30: 362e 2044 6565 7046 6173 6869 6f6e 2064  6. DeepFashion d
-00002c40: 6174 6173 6574 3a20 4879 702d 5669 5420  ataset: Hyp-ViT 
-00002c50: e280 9420 3932 2e35 2c20 6f75 7273 20e2  ... 92.5, ours .
-00002c60: 8094 2039 322e 312e 0a54 6875 732c 2075  .. 92.1..Thus, u
-00002c70: 7469 6c69 7369 6e67 2073 696d 706c 6520  tilising simple 
-00002c80: 6865 7572 6973 7469 6373 2061 6e64 2061  heuristics and a
-00002c90: 766f 6964 696e 6720 6865 6176 7920 6d61  voiding heavy ma
-00002ca0: 7468 2077 6520 6172 6520 6162 6c65 2074  th we are able t
-00002cb0: 6f20 7065 7266 6f72 6d20 6f6e 2053 6f74  o perform on Sot
-00002cc0: 4120 6c65 7665 6c2e 0a0a 3c2f 703e 0a3c  A level...</p>.<
-00002cd0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-00002ce0: 696c 733e 0a3c 7375 6d6d 6172 793e 5768  ils>.<summary>Wh
-00002cf0: 6174 2061 626f 7574 2053 656c 662d 5375  at about Self-Su
-00002d00: 7065 7276 6973 6564 204c 6561 726e 696e  pervised Learnin
-00002d10: 673f 3c2f 7375 6d6d 6172 793e 0a3c 703e  g?</summary>.<p>
-00002d20: 0a0a 5265 6365 6e74 2072 6573 6561 7263  ..Recent researc
-00002d30: 6820 696e 2053 534c 2064 6566 696e 6974  h in SSL definit
-00002d40: 656c 7920 6f62 7461 696e 6564 2067 7265  ely obtained gre
-00002d50: 6174 2072 6573 756c 7473 2e20 5468 6520  at results. The 
-00002d60: 7072 6f62 6c65 6d20 6973 2074 6861 7420  problem is that 
-00002d70: 7468 6573 6520 6170 7072 6f61 6368 6573  these approaches
-00002d80: 0a72 6571 7569 7265 6420 616e 2065 6e6f  .required an eno
-00002d90: 726d 6f75 7320 616d 6f75 6e74 206f 6620  rmous amount of 
-00002da0: 636f 6d70 7574 696e 6720 746f 2074 7261  computing to tra
-00002db0: 696e 2074 6865 206d 6f64 656c 2e20 4275  in the model. Bu
-00002dc0: 7420 696e 206f 7572 2066 7261 6d65 776f  t in our framewo
-00002dd0: 726b 2c20 7765 2063 6f6e 7369 6465 7220  rk, we consider 
-00002de0: 7468 6520 6d6f 7374 2063 6f6d 6d6f 6e20  the most common 
-00002df0: 6361 7365 0a77 6865 6e20 7468 6520 6176  case.when the av
-00002e00: 6572 6167 6520 7573 6572 2068 6173 206e  erage user has n
-00002e10: 6f20 6d6f 7265 2074 6861 6e20 6120 6665  o more than a fe
-00002e20: 7720 4750 5573 2e0a 0a41 7420 7468 6520  w GPUs...At the 
-00002e30: 7361 6d65 2074 696d 652c 2069 7420 776f  same time, it wo
-00002e40: 756c 6420 6265 2075 6e77 6973 6520 746f  uld be unwise to
-00002e50: 2069 676e 6f72 6520 7375 6363 6573 7320   ignore success 
-00002e60: 696e 2074 6869 7320 7370 6865 7265 2c20  in this sphere, 
-00002e70: 736f 2077 6520 7374 696c 6c20 6578 706c  so we still expl
-00002e80: 6f69 7420 6974 2069 6e20 7477 6f20 7761  oit it in two wa
-00002e90: 7973 3a0a 2a20 4173 2061 2073 6f75 7263  ys:.* As a sourc
-00002ea0: 6520 6f66 2063 6865 636b 706f 696e 7473  e of checkpoints
-00002eb0: 2074 6861 7420 776f 756c 6420 6265 2067   that would be g
-00002ec0: 7265 6174 2074 6f20 7374 6172 7420 7472  reat to start tr
-00002ed0: 6169 6e69 6e67 2077 6974 682e 2046 726f  aining with. Fro
-00002ee0: 6d20 7075 626c 6963 6174 696f 6e73 2061  m publications a
-00002ef0: 6e64 206f 7572 2065 7870 6572 6965 6e63  nd our experienc
-00002f00: 652c 0a20 2074 6865 7920 6172 6520 6d75  e,.  they are mu
-00002f10: 6368 2062 6574 7465 7220 6173 2069 6e69  ch better as ini
-00002f20: 7469 616c 6973 6174 696f 6e20 7468 616e  tialisation than
-00002f30: 2074 6865 2064 6566 6175 6c74 2073 7570   the default sup
-00002f40: 6572 7669 7365 6420 6d6f 6465 6c20 7472  ervised model tr
-00002f50: 6169 6e65 6420 6f6e 2049 6d61 6765 4e65  ained on ImageNe
-00002f60: 742e 2054 6875 732c 2077 6520 6164 6465  t. Thus, we adde
-00002f70: 6420 7468 6520 706f 7373 6962 696c 6974  d the possibilit
-00002f80: 790a 2020 746f 2069 6e69 7469 616c 6973  y.  to initialis
-00002f90: 6520 796f 7572 206d 6f64 656c 7320 7573  e your models us
-00002fa0: 696e 6720 7468 6573 6520 7072 6574 7261  ing these pretra
-00002fb0: 696e 6564 2063 6865 636b 706f 696e 7473  ined checkpoints
-00002fc0: 206f 6e6c 7920 6279 2070 6173 7369 6e67   only by passing
-00002fd0: 2061 6e20 6172 6775 6d65 6e74 2069 6e20   an argument in 
-00002fe0: 7468 6520 636f 6e66 6967 206f 7220 7468  the config or th
-00002ff0: 6520 636f 6e73 7472 7563 746f 722e 0a2a  e constructor..*
-00003000: 2041 7320 6120 736f 7572 6365 206f 6620   As a source of 
-00003010: 696e 7370 6972 6174 696f 6e2e 2046 6f72  inspiration. For
-00003020: 2065 7861 6d70 6c65 2c20 7765 2061 6461   example, we ada
-00003030: 7074 6564 2074 6865 2069 6465 6120 6f66  pted the idea of
-00003040: 2061 206d 656d 6f72 7920 6261 6e6b 2066   a memory bank f
-00003050: 726f 6d20 2a4d 6f43 6f2a 2066 6f72 2074  rom *MoCo* for t
-00003060: 6865 202a 5472 6970 6c65 744c 6f73 732a  he *TripletLoss*
-00003070: 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461 696c  ...</p>.</detail
-00003080: 733e 0a0a 0a3c 6465 7461 696c 733e 0a3c  s>...<details>.<
-00003090: 7375 6d6d 6172 793e 446f 2049 206e 6565  summary>Do I nee
-000030a0: 6420 746f 206b 6e6f 7720 6f74 6865 7220  d to know other 
-000030b0: 6672 616d 6577 6f72 6b73 2074 6f20 7573  frameworks to us
-000030c0: 6520 4f4d 4c3f 3c2f 7375 6d6d 6172 793e  e OML?</summary>
-000030d0: 0a3c 703e 0a0a 4e6f 2c20 796f 7520 646f  .<p>..No, you do
-000030e0: 6e27 742e 204f 4d4c 2069 7320 6120 6672  n't. OML is a fr
-000030f0: 616d 6577 6f72 6b2d 6167 6e6f 7374 6963  amework-agnostic
-00003100: 2e20 4465 7370 6974 6520 7765 2075 7365  . Despite we use
-00003110: 2050 7954 6f72 6368 204c 6967 6874 6e69   PyTorch Lightni
-00003120: 6e67 2061 7320 6120 6c6f 6f70 0a72 756e  ng as a loop.run
-00003130: 6e65 7220 666f 7220 7468 6520 6578 7065  ner for the expe
-00003140: 7269 6d65 6e74 732c 2077 6520 616c 736f  riments, we also
-00003150: 206b 6565 7020 7468 6520 706f 7373 6962   keep the possib
-00003160: 696c 6974 7920 746f 2072 756e 2065 7665  ility to run eve
-00003170: 7279 7468 696e 6720 6f6e 2070 7572 6520  rything on pure 
-00003180: 5079 546f 7263 682e 0a54 6875 732c 206f  PyTorch..Thus, o
-00003190: 6e6c 7920 7468 6520 7469 6e79 2070 6172  nly the tiny par
-000031a0: 7420 6f66 204f 4d4c 2069 7320 4c69 6768  t of OML is Ligh
-000031b0: 746e 696e 672d 7370 6563 6966 6963 2061  tning-specific a
-000031c0: 6e64 2077 6520 6b65 6570 2074 6869 7320  nd we keep this 
-000031d0: 6c6f 6769 6320 7365 7061 7261 7465 6c79  logic separately
-000031e0: 2066 726f 6d0a 6f74 6865 7220 636f 6465   from.other code
-000031f0: 2028 7365 6520 606f 6d6c 2e6c 6967 6874   (see `oml.light
-00003200: 6e69 6e67 6029 2e20 4576 656e 2077 6865  ning`). Even whe
-00003210: 6e20 796f 7520 7573 6520 4c69 6768 746e  n you use Lightn
-00003220: 696e 672c 2079 6f75 2064 6f6e 2774 206e  ing, you don't n
-00003230: 6565 6420 746f 206b 6e6f 7720 6974 2c20  eed to know it, 
-00003240: 7369 6e63 650a 7765 2070 726f 7669 6465  since.we provide
-00003250: 2072 6561 6479 2074 6f20 7573 6520 5b50   ready to use [P
-00003260: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
-00003270: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
-00003280: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
-00003290: 632d 6c65 6172 6e69 6e67 2f62 6c6f 622f  c-learning/blob/
-000032a0: 6d61 696e 2f70 6970 656c 696e 6573 2f29  main/pipelines/)
-000032b0: 2e0a 0a54 6865 2070 6f73 7369 6269 6c69  ...The possibili
-000032c0: 7479 206f 6620 7573 696e 6720 7075 7265  ty of using pure
-000032d0: 2050 7954 6f72 6368 2061 6e64 206d 6f64   PyTorch and mod
-000032e0: 756c 6172 2073 7472 7563 7475 7265 206f  ular structure o
-000032f0: 6620 7468 6520 636f 6465 206c 6561 7665  f the code leave
-00003300: 7320 6120 726f 6f6d 2066 6f72 2075 7469  s a room for uti
-00003310: 6c69 7a69 6e67 0a4f 4d4c 2077 6974 6820  lizing.OML with 
-00003320: 796f 7572 2066 6176 6f75 7269 7465 2066  your favourite f
-00003330: 7261 6d65 776f 726b 2061 6674 6572 2074  ramework after t
-00003340: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
-00003350: 6e20 6f66 2074 6865 206e 6563 6573 7361  n of the necessa
-00003360: 7279 2077 7261 7070 6572 732e 0a0a 3c2f  ry wrappers...</
-00003370: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
-00003380: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
-00003390: 7279 3e43 616e 2049 2075 7365 204f 4d4c  ry>Can I use OML
-000033a0: 2077 6974 686f 7574 2061 6e79 206b 6e6f   without any kno
-000033b0: 776c 6564 6765 2069 6e20 4461 7461 5363  wledge in DataSc
-000033c0: 6965 6e63 653f 3c2f 7375 6d6d 6172 793e  ience?</summary>
-000033d0: 0a3c 703e 0a0a 5965 732e 2054 6f20 7275  .<p>..Yes. To ru
-000033e0: 6e20 7468 6520 6578 7065 7269 6d65 6e74  n the experiment
-000033f0: 2077 6974 6820 5b50 6970 656c 696e 6573   with [Pipelines
-00003400: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003410: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00003420: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00003430: 6e67 2f62 6c6f 622f 6d61 696e 2f70 6970  ng/blob/main/pip
-00003440: 656c 696e 6573 2f29 0a79 6f75 206f 6e6c  elines/).you onl
-00003450: 7920 6e65 6564 2074 6f20 7772 6974 6520  y need to write 
-00003460: 6120 636f 6e76 6572 7465 720a 746f 206f  a converter.to o
-00003470: 7572 2066 6f72 6d61 7420 2869 7420 6d65  ur format (it me
-00003480: 616e 7320 7072 6570 6172 696e 6720 7468  ans preparing th
-00003490: 650a 602e 6373 7660 2074 6162 6c65 2077  e.`.csv` table w
-000034a0: 6974 6820 3520 7072 6564 6566 696e 6564  ith 5 predefined
-000034b0: 2063 6f6c 756d 6e73 292e 0a54 6861 7427   columns)..That'
-000034c0: 7320 6974 210a 0a50 726f 6261 626c 7920  s it!..Probably 
-000034d0: 7765 2061 6c72 6561 6479 2068 6176 6520  we already have 
-000034e0: 6120 7375 6974 6162 6c65 2070 7265 2d74  a suitable pre-t
-000034f0: 7261 696e 6564 206d 6f64 656c 2066 6f72  rained model for
-00003500: 2079 6f75 7220 646f 6d61 696e 0a69 6e20   your domain.in 
-00003510: 6f75 7220 2a4d 6f64 656c 7320 5a6f 6f2a  our *Models Zoo*
-00003520: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
-00003530: 796f 7520 646f 6e27 7420 6576 656e 206e  you don't even n
-00003540: 6565 6420 746f 2074 7261 696e 2069 742e  eed to train it.
-00003550: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-00003560: 0a0a 2323 205b 446f 6375 6d65 6e74 6174  ..## [Documentat
-00003570: 696f 6e5d 2868 7474 7073 3a2f 2f6f 7065  ion](https://ope
-00003580: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-00003590: 672e 7265 6164 7468 6564 6f63 732e 696f  g.readthedocs.io
-000035a0: 2f65 6e2f 6c61 7465 7374 2f69 6e64 6578  /en/latest/index
-000035b0: 2e68 746d 6c29 0a0a 446f 6375 6d65 6e74  .html)..Document
-000035c0: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-000035d0: 6c65 2076 6961 2074 6865 205b 6c69 6e6b  le via the [link
-000035e0: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-000035f0: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00003600: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00003610: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
-00003620: 6d6c 292e 0a0a 596f 7520 6361 6e20 616c  ml)...You can al
-00003630: 736f 2072 6561 6420 736f 6d65 2065 7874  so read some ext
-00003640: 7261 206d 6174 6572 6961 6c73 2072 656c  ra materials rel
-00003650: 6174 6564 2074 6f20 4f4d 4c3a 0a0a 2a20  ated to OML:..* 
-00003660: 5468 656f 7279 2061 6e64 2070 7261 6374  Theory and pract
-00003670: 6963 6520 6f66 206d 6574 7269 6320 6c65  ice of metric le
-00003680: 6172 6e69 6e67 2077 6974 6820 7468 6520  arning with the 
-00003690: 7573 6167 6520 6f66 204f 4d4c 2e0a 5b50  usage of OML..[P
-000036a0: 6f73 7420 696e 2045 6e67 6c69 7368 206f  ost in English o
-000036b0: 6e20 4d65 6469 756d 5d28 6874 7470 733a  n Medium](https:
-000036c0: 2f2f 6d65 6469 756d 2e63 6f6d 2f40 416c  //medium.com/@Al
-000036d0: 656b 7365 6953 6861 6261 6e6f 762f 7072  ekseiShabanov/pr
-000036e0: 6163 7469 6361 6c2d 6d65 7472 6963 2d6c  actical-metric-l
-000036f0: 6561 726e 696e 672d 6230 3431 3063 6461  earning-b0410cda
-00003700: 3232 3031 2920 7c0a 5b50 6f73 7420 696e  2201) |.[Post in
-00003710: 2052 7573 7369 616e 206f 6e20 4861 6272   Russian on Habr
-00003720: 5d28 6874 7470 733a 2f2f 6861 6272 2e63  ](https://habr.c
-00003730: 6f6d 2f72 752f 636f 6d70 616e 792f 6f64  om/ru/company/od
-00003740: 732f 626c 6f67 2f36 3935 3338 302f 2920  s/blog/695380/) 
-00003750: 7c0a 5b50 6f73 7420 696e 2043 6869 6e65  |.[Post in Chine
-00003760: 7365 206f 6e20 4353 444e 5d28 6874 7470  se on CSDN](http
-00003770: 733a 2f2f 626c 6f67 2e63 7364 6e2e 6e65  s://blog.csdn.ne
-00003780: 742f 6665 726d 696f 6e30 3231 372f 6172  t/fermion0217/ar
-00003790: 7469 636c 652f 6465 7461 696c 732f 3132  ticle/details/12
-000037a0: 3739 3332 3038 3729 2c20 7472 616e 736c  7932087), transl
-000037b0: 6174 6564 2062 7920 4368 6961 2d43 6865  ated by Chia-Che
-000037c0: 6e20 4368 616e 672e 0a0a 2a20 5468 650a  n Chang...* The.
-000037d0: 5b44 454d 4f5d 2868 7474 7073 3a2f 2f64  [DEMO](https://d
-000037e0: 6170 6c61 646f 632d 6f6d 6c2d 706f 7374  apladoc-oml-post
-000037f0: 7072 6f63 6573 7369 6e67 2d64 656d 6f2d  processing-demo-
-00003800: 7372 6361 7070 6d61 696e 2d70 6668 3267  srcappmain-pfh2g
-00003810: 302e 7374 7265 616d 6c69 742e 6170 702f  0.streamlit.app/
-00003820: 290a 666f 7220 6f75 7220 7061 7065 720a  ).for our paper.
-00003830: 5b53 5449 523a 2053 6961 6d65 7365 2054  [STIR: Siamese T
-00003840: 7261 6e73 666f 726d 6572 7320 666f 7220  ransformers for 
-00003850: 496d 6167 6520 5265 7472 6965 7661 6c20  Image Retrieval 
-00003860: 506f 7374 7072 6f63 6573 7369 6e67 5d28  Postprocessing](
-00003870: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00003880: 672f 6162 732f 3233 3034 2e31 3333 3933  g/abs/2304.13393
-00003890: 290a 0a2a 2054 6865 2072 6570 6f72 7420  )..* The report 
-000038a0: 666f 7220 4265 726c 696e 2d62 6173 6564  for Berlin-based
-000038b0: 206d 6565 7475 703a 2022 436f 6d70 7574   meetup: "Comput
-000038c0: 6572 2056 6973 696f 6e20 696e 2070 726f  er Vision in pro
-000038d0: 6475 6374 696f 6e22 2e20 4e6f 7665 6d62  duction". Novemb
-000038e0: 6572 2c20 3230 3232 2e0a 5b4c 696e 6b5d  er, 2022..[Link]
-000038f0: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00003900: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00003910: 666f 6c64 6572 732f 3175 486d 4c55 3876  folders/1uHmLU8v
-00003920: 4d72 4d56 4d46 6f64 7433 3675 3075 5841  MrMVMFodt36u0uXA
-00003930: 6759 6a47 5f33 4433 303f 7573 703d 7368  gYjG_3D30?usp=sh
-00003940: 6172 655f 6c69 6e6b 290a 0a23 2320 5b49  are_link)..## [I
-00003950: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
-00003960: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
-00003970: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
-00003980: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00003990: 7374 2f6f 6d6c 2f69 6e73 7461 6c6c 6174  st/oml/installat
-000039a0: 696f 6e2e 6874 6d6c 290a 0a4f 4d4c 2069  ion.html)..OML i
-000039b0: 7320 6176 6169 6c61 626c 6520 696e 2050  s available in P
-000039c0: 7950 493a 0a0a 6060 6073 6865 6c6c 0a70  yPI:..```shell.p
-000039d0: 6970 2069 6e73 7461 6c6c 202d 5520 6f70  ip install -U op
-000039e0: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000039f0: 6e67 0a60 6060 0a0a 596f 7520 6361 6e20  ng.```..You can 
-00003a00: 616c 736f 2070 756c 6c20 7468 6520 7072  also pull the pr
-00003a10: 6570 6172 6564 2069 6d61 6765 2066 726f  epared image fro
-00003a20: 6d20 446f 636b 6572 4875 622e 2e2e 0a0a  m DockerHub.....
-00003a30: 6060 6073 6865 6c6c 0a64 6f63 6b65 7220  ```shell.docker 
-00003a40: 7075 6c6c 206f 6d6c 7465 616d 2f6f 6d6c  pull omlteam/oml
-00003a50: 3a67 7075 0a64 6f63 6b65 7220 7075 6c6c  :gpu.docker pull
-00003a60: 206f 6d6c 7465 616d 2f6f 6d6c 3a63 7075   omlteam/oml:cpu
-00003a70: 0a60 6060 0a0a 2e2e 2e6f 7220 6275 696c  .```.....or buil
-00003a80: 6420 6f6e 6520 6279 2079 6f75 7220 6f77  d one by your ow
-00003a90: 6e0a 0a60 6060 7368 656c 6c0a 6d61 6b65  n..```shell.make
-00003aa0: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
-00003ab0: 4e54 494d 453d 6370 750a 6d61 6b65 2064  NTIME=cpu.make d
-00003ac0: 6f63 6b65 725f 6275 696c 6420 5255 4e54  ocker_build RUNT
-00003ad0: 494d 453d 6770 750a 6060 600a 0a23 2320  IME=gpu.```..## 
-00003ae0: 5b45 7861 6d70 6c65 735d 2868 7474 7073  [Examples](https
-00003af0: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
-00003b00: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
-00003b10: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003b20: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
-00003b30: 696f 6e2f 7079 7468 6f6e 5f65 7861 6d70  ion/python_examp
-00003b40: 6c65 732e 6874 6d6c 2329 0a0a 3c64 6574  les.html#)..<det
-00003b50: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e54  ails>.<summary>T
-00003b60: 7261 696e 696e 673c 2f73 756d 6d61 7279  raining</summary
-00003b70: 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e 745d  >.<p>..[comment]
-00003b80: 3a76 616e 696c 6c61 2d74 7261 696e 2d73  :vanilla-train-s
-00003b90: 7461 7274 0a60 6060 7079 7468 6f6e 0a69  tart.```python.i
-00003ba0: 6d70 6f72 7420 746f 7263 680a 6672 6f6d  mport torch.from
-00003bb0: 2074 7164 6d20 696d 706f 7274 2074 7164   tqdm import tqd
-00003bc0: 6d0a 0a66 726f 6d20 6f6d 6c2e 6461 7461  m..from oml.data
-00003bd0: 7365 7473 2e62 6173 6520 696d 706f 7274  sets.base import
-00003be0: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
-00003bf0: 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ls.from oml.loss
-00003c00: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
-00003c10: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
-00003c20: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
-00003c30: 6d69 6e65 7273 2e69 6e62 6174 6368 5f61  miners.inbatch_a
-00003c40: 6c6c 5f74 7269 2069 6d70 6f72 7420 416c  ll_tri import Al
-00003c50: 6c54 7269 706c 6574 734d 696e 6572 0a66  lTripletsMiner.f
-00003c60: 726f 6d20 6f6d 6c2e 6d6f 6465 6c73 2069  rom oml.models i
-00003c70: 6d70 6f72 7420 5669 5445 7874 7261 6374  mport ViTExtract
-00003c80: 6f72 0a66 726f 6d20 6f6d 6c2e 7361 6d70  or.from oml.samp
-00003c90: 6c65 7273 2e62 616c 616e 6365 2069 6d70  lers.balance imp
-00003ca0: 6f72 7420 4261 6c61 6e63 6553 616d 706c  ort BalanceSampl
-00003cb0: 6572 0a66 726f 6d20 6f6d 6c2e 7574 696c  er.from oml.util
-00003cc0: 732e 646f 776e 6c6f 6164 5f6d 6f63 6b5f  s.download_mock_
-00003cd0: 6461 7461 7365 7420 696d 706f 7274 2064  dataset import d
-00003ce0: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
-00003cf0: 6173 6574 0a0a 6461 7461 7365 745f 726f  aset..dataset_ro
-00003d00: 6f74 203d 2022 6d6f 636b 5f64 6174 6173  ot = "mock_datas
-00003d10: 6574 2f22 0a64 665f 7472 6169 6e2c 205f  et/".df_train, _
-00003d20: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-00003d30: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-00003d40: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-00003d50: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-00003d60: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-00003d70: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-00003d80: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00003d90: 733d 4661 6c73 6529 2e74 7261 696e 2829  s=False).train()
-00003da0: 0a6f 7074 696d 697a 6572 203d 2074 6f72  .optimizer = tor
-00003db0: 6368 2e6f 7074 696d 2e53 4744 2865 7874  ch.optim.SGD(ext
-00003dc0: 7261 6374 6f72 2e70 6172 616d 6574 6572  ractor.parameter
-00003dd0: 7328 292c 206c 723d 3165 2d36 290a 0a74  s(), lr=1e-6)..t
-00003de0: 7261 696e 5f64 6174 6173 6574 203d 2044  rain_dataset = D
-00003df0: 6174 6173 6574 5769 7468 4c61 6265 6c73  atasetWithLabels
-00003e00: 2864 665f 7472 6169 6e2c 2064 6174 6173  (df_train, datas
-00003e10: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00003e20: 726f 6f74 290a 6372 6974 6572 696f 6e20  root).criterion 
-00003e30: 3d20 5472 6970 6c65 744c 6f73 7357 6974  = TripletLossWit
-00003e40: 684d 696e 6572 286d 6172 6769 6e3d 302e  hMiner(margin=0.
-00003e50: 312c 206d 696e 6572 3d41 6c6c 5472 6970  1, miner=AllTrip
-00003e60: 6c65 7473 4d69 6e65 7228 292c 206e 6565  letsMiner(), nee
-00003e70: 645f 6c6f 6773 3d54 7275 6529 0a73 616d  d_logs=True).sam
-00003e80: 706c 6572 203d 2042 616c 616e 6365 5361  pler = BalanceSa
-00003e90: 6d70 6c65 7228 7472 6169 6e5f 6461 7461  mpler(train_data
-00003ea0: 7365 742e 6765 745f 6c61 6265 6c73 2829  set.get_labels()
-00003eb0: 2c20 6e5f 6c61 6265 6c73 3d32 2c20 6e5f  , n_labels=2, n_
-00003ec0: 696e 7374 616e 6365 733d 3229 0a74 7261  instances=2).tra
-00003ed0: 696e 5f6c 6f61 6465 7220 3d20 746f 7263  in_loader = torc
-00003ee0: 682e 7574 696c 732e 6461 7461 2e44 6174  h.utils.data.Dat
-00003ef0: 614c 6f61 6465 7228 7472 6169 6e5f 6461  aLoader(train_da
-00003f00: 7461 7365 742c 2062 6174 6368 5f73 616d  taset, batch_sam
-00003f10: 706c 6572 3d73 616d 706c 6572 290a 0a66  pler=sampler)..f
-00003f20: 6f72 2062 6174 6368 2069 6e20 7471 646d  or batch in tqdm
-00003f30: 2874 7261 696e 5f6c 6f61 6465 7229 3a0a  (train_loader):.
-00003f40: 2020 2020 656d 6265 6464 696e 6773 203d      embeddings =
-00003f50: 2065 7874 7261 6374 6f72 2862 6174 6368   extractor(batch
-00003f60: 5b22 696e 7075 745f 7465 6e73 6f72 7322  ["input_tensors"
-00003f70: 5d29 0a20 2020 206c 6f73 7320 3d20 6372  ]).    loss = cr
-00003f80: 6974 6572 696f 6e28 656d 6265 6464 696e  iterion(embeddin
-00003f90: 6773 2c20 6261 7463 685b 226c 6162 656c  gs, batch["label
-00003fa0: 7322 5d29 0a20 2020 206c 6f73 732e 6261  s"]).    loss.ba
-00003fb0: 636b 7761 7264 2829 0a20 2020 206f 7074  ckward().    opt
-00003fc0: 696d 697a 6572 2e73 7465 7028 290a 2020  imizer.step().  
-00003fd0: 2020 6f70 7469 6d69 7a65 722e 7a65 726f    optimizer.zero
-00003fe0: 5f67 7261 6428 290a 0a20 2020 2023 2069  _grad()..    # i
-00003ff0: 6e66 6f20 666f 7220 6c6f 6767 696e 673a  nfo for logging:
-00004000: 2070 6f73 6974 6976 652f 6e65 6761 7469   positive/negati
-00004010: 7665 2064 6973 7461 6e63 6573 2c20 6e75  ve distances, nu
-00004020: 6d62 6572 206f 6620 6163 7469 7665 2074  mber of active t
-00004030: 7269 706c 6574 730a 2020 2020 7072 696e  riplets.    prin
-00004040: 7428 6372 6974 6572 696f 6e2e 6c61 7374  t(criterion.last
-00004050: 5f6c 6f67 7329 0a0a 6060 600a 5b63 6f6d  _logs)..```.[com
-00004060: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7472  ment]:vanilla-tr
-00004070: 6169 6e2d 656e 640a 3c2f 703e 0a3c 2f64  ain-end.</p>.</d
-00004080: 6574 6169 6c73 3e0a 0a5b 215b 4f70 656e  etails>..[![Open
-00004090: 2049 6e20 436f 6c61 625d 2868 7474 7073   In Colab](https
-000040a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-000040b0: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-000040c0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-000040d0: 7376 6729 5d28 6874 7470 733a 2f2f 636f  svg)](https://co
-000040e0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-000040f0: 676c 652e 636f 6d2f 6472 6976 652f 316b  gle.com/drive/1k
-00004100: 6e74 4441 4964 495a 394c 3430 6a63 6e64  ntDAIdIZ9L40jcnd
-00004110: 6775 4c41 622d 5871 6d43 464f 6753 353f  guLAb-XqmCFOgS5?
-00004120: 7573 703d 7368 6172 696e 6729 0a3c 6465  usp=sharing).<de
-00004130: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
-00004140: 5661 6c69 6461 7469 6f6e 3c2f 7375 6d6d  Validation</summ
-00004150: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-00004160: 6e74 5d3a 7661 6e69 6c6c 612d 7661 6c69  nt]:vanilla-vali
-00004170: 6461 7469 6f6e 2d73 7461 7274 0a60 6060  dation-start.```
-00004180: 7079 7468 6f6e 0a69 6d70 6f72 7420 746f  python.import to
-00004190: 7263 680a 6672 6f6d 2074 7164 6d20 696d  rch.from tqdm im
-000041a0: 706f 7274 2074 7164 6d0a 0a66 726f 6d20  port tqdm..from 
-000041b0: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-000041c0: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-000041d0: 5175 6572 7947 616c 6c65 7279 0a66 726f  QueryGallery.fro
-000041e0: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-000041f0: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00004200: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
-00004210: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
-00004220: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00004230: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7574  ctor.from oml.ut
-00004240: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
-00004250: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
-00004260: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
-00004270: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
-00004280: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
-00004290: 6173 6574 2f22 0a5f 2c20 6466 5f76 616c  aset/"._, df_val
-000042a0: 203d 2064 6f77 6e6c 6f61 645f 6d6f 636b   = download_mock
-000042b0: 5f64 6174 6173 6574 2864 6174 6173 6574  _dataset(dataset
-000042c0: 5f72 6f6f 7429 0a0a 6578 7472 6163 746f  _root)..extracto
-000042d0: 7220 3d20 5669 5445 7874 7261 6374 6f72  r = ViTExtractor
-000042e0: 2822 7669 7473 3136 5f64 696e 6f22 2c20  ("vits16_dino", 
-000042f0: 6172 6368 3d22 7669 7473 3136 222c 206e  arch="vits16", n
-00004300: 6f72 6d61 6c69 7365 5f66 6561 7475 7265  ormalise_feature
-00004310: 733d 4661 6c73 6529 2e65 7661 6c28 290a  s=False).eval().
-00004320: 0a76 616c 5f64 6174 6173 6574 203d 2044  .val_dataset = D
-00004330: 6174 6173 6574 5175 6572 7947 616c 6c65  atasetQueryGalle
-00004340: 7279 2864 665f 7661 6c2c 2064 6174 6173  ry(df_val, datas
-00004350: 6574 5f72 6f6f 743d 6461 7461 7365 745f  et_root=dataset_
-00004360: 726f 6f74 290a 0a76 616c 5f6c 6f61 6465  root)..val_loade
-00004370: 7220 3d20 746f 7263 682e 7574 696c 732e  r = torch.utils.
-00004380: 6461 7461 2e44 6174 614c 6f61 6465 7228  data.DataLoader(
-00004390: 7661 6c5f 6461 7461 7365 742c 2062 6174  val_dataset, bat
-000043a0: 6368 5f73 697a 653d 3429 0a63 616c 6375  ch_size=4).calcu
-000043b0: 6c61 746f 7220 3d20 456d 6265 6464 696e  lator = Embeddin
-000043c0: 674d 6574 7269 6373 2865 7874 7261 5f6b  gMetrics(extra_k
-000043d0: 6579 733d 2822 7061 7468 7322 2c29 290a  eys=("paths",)).
-000043e0: 6361 6c63 756c 6174 6f72 2e73 6574 7570  calculator.setup
-000043f0: 286e 756d 5f73 616d 706c 6573 3d6c 656e  (num_samples=len
-00004400: 2876 616c 5f64 6174 6173 6574 2929 0a0a  (val_dataset))..
-00004410: 7769 7468 2074 6f72 6368 2e6e 6f5f 6772  with torch.no_gr
-00004420: 6164 2829 3a0a 2020 2020 666f 7220 6261  ad():.    for ba
-00004430: 7463 6820 696e 2074 7164 6d28 7661 6c5f  tch in tqdm(val_
-00004440: 6c6f 6164 6572 293a 0a20 2020 2020 2020  loader):.       
-00004450: 2062 6174 6368 5b22 656d 6265 6464 696e   batch["embeddin
-00004460: 6773 225d 203d 2065 7874 7261 6374 6f72  gs"] = extractor
-00004470: 2862 6174 6368 5b22 696e 7075 745f 7465  (batch["input_te
-00004480: 6e73 6f72 7322 5d29 0a20 2020 2020 2020  nsors"]).       
-00004490: 2063 616c 6375 6c61 746f 722e 7570 6461   calculator.upda
-000044a0: 7465 5f64 6174 6128 6261 7463 6829 0a0a  te_data(batch)..
-000044b0: 6d65 7472 6963 7320 3d20 6361 6c63 756c  metrics = calcul
-000044c0: 6174 6f72 2e63 6f6d 7075 7465 5f6d 6574  ator.compute_met
-000044d0: 7269 6373 2829 0a0a 2320 4c6f 6767 696e  rics()..# Loggin
-000044e0: 670a 7072 696e 7428 6361 6c63 756c 6174  g.print(calculat
-000044f0: 6f72 2e6d 6574 7269 6373 2920 2023 206d  or.metrics)  # m
-00004500: 6574 7269 6373 0a70 7269 6e74 2863 616c  etrics.print(cal
-00004510: 6375 6c61 746f 722e 6d65 7472 6963 735f  culator.metrics_
-00004520: 756e 7265 6475 6365 6429 2020 2320 6d65  unreduced)  # me
-00004530: 7472 6963 7320 7769 7468 6f75 7420 6176  trics without av
-00004540: 6572 6167 696e 6720 6f76 6572 2071 7565  eraging over que
-00004550: 7269 6573 0a0a 2320 5669 7375 616c 6973  ries..# Visualis
-00004560: 6174 696f 6e0a 6361 6c63 756c 6174 6f72  ation.calculator
-00004570: 2e67 6574 5f70 6c6f 745f 666f 725f 7175  .get_plot_for_qu
-00004580: 6572 6965 7328 7175 6572 795f 6964 733d  eries(query_ids=
-00004590: 5b30 2c20 325d 2c20 6e5f 696e 7374 616e  [0, 2], n_instan
-000045a0: 6365 733d 3529 2020 2320 6472 6177 2070  ces=5)  # draw p
-000045b0: 7265 6469 6374 696f 6e73 206f 6e20 7072  redictions on pr
-000045c0: 6564 6566 696e 6564 2071 7565 7269 6573  edefined queries
-000045d0: 0a63 616c 6375 6c61 746f 722e 6765 745f  .calculator.get_
-000045e0: 706c 6f74 5f66 6f72 5f77 6f72 7374 5f71  plot_for_worst_q
-000045f0: 7565 7269 6573 286d 6574 7269 635f 6e61  ueries(metric_na
-00004600: 6d65 3d22 4f56 4552 414c 4c2f 6d61 702f  me="OVERALL/map/
-00004610: 3522 2c20 6e5f 7175 6572 6965 733d 322c  5", n_queries=2,
-00004620: 206e 5f69 6e73 7461 6e63 6573 3d35 2920   n_instances=5) 
-00004630: 2023 2064 7261 7720 6d69 7374 616b 6573   # draw mistakes
-00004640: 0a63 616c 6375 6c61 746f 722e 7669 7375  .calculator.visu
-00004650: 616c 697a 6528 2920 2023 2064 7261 7720  alize()  # draw 
-00004660: 6d69 7374 616b 6573 2066 6f72 2061 6c6c  mistakes for all
-00004670: 2074 6865 2061 7661 696c 6162 6c65 206d   the available m
-00004680: 6574 7269 6373 0a0a 6060 600a 5b63 6f6d  etrics..```.[com
-00004690: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
-000046a0: 6c69 6461 7469 6f6e 2d65 6e64 0a3c 2f70  lidation-end.</p
-000046b0: 3e0a 3c2f 6465 7461 696c 733e 0a0a 5b21  >.</details>..[!
-000046c0: 5b4f 7065 6e20 496e 2043 6f6c 6162 5d28  [Open In Colab](
-000046d0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-000046e0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-000046f0: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
-00004700: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00004710: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00004720: 682e 676f 6f67 6c65 2e63 6f6d 2f64 7269  h.google.com/dri
-00004730: 7665 2f31 4f32 6f33 6b38 4938 6a4e 3568  ve/1O2o3k8I8jN5h
-00004740: 5269 6e33 644b 6e41 5333 5773 6747 3034  Rin3dKnAS3WsgG04
-00004750: 746d 4954 3f75 7370 3d73 6861 7269 6e67  tmIT?usp=sharing
-00004760: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
-00004770: 6d61 7279 3e54 7261 696e 696e 6720 2b20  mary>Training + 
-00004780: 5661 6c69 6461 7469 6f6e 205b 4c69 6768  Validation [Ligh
-00004790: 746e 696e 6720 616e 6420 4e65 7074 756e  tning and Neptun
-000047a0: 6520 6c6f 6767 696e 675d 3c2f 7375 6d6d  e logging]</summ
-000047b0: 6172 793e 0a3c 703e 0a0a 5b63 6f6d 6d65  ary>.<p>..[comme
-000047c0: 6e74 5d3a 6c69 6768 746e 696e 672d 7374  nt]:lightning-st
-000047d0: 6172 740a 6060 6070 7974 686f 6e0a 696d  art.```python.im
-000047e0: 706f 7274 2070 7974 6f72 6368 5f6c 6967  port pytorch_lig
-000047f0: 6874 6e69 6e67 2061 7320 706c 0a69 6d70  htning as pl.imp
-00004800: 6f72 7420 746f 7263 680a 0a66 726f 6d20  ort torch..from 
-00004810: 6f6d 6c2e 6461 7461 7365 7473 2e62 6173  oml.datasets.bas
-00004820: 6520 696d 706f 7274 2044 6174 6173 6574  e import Dataset
-00004830: 5175 6572 7947 616c 6c65 7279 2c20 4461  QueryGallery, Da
-00004840: 7461 7365 7457 6974 684c 6162 656c 730a  tasetWithLabels.
-00004850: 6672 6f6d 206f 6d6c 2e6c 6967 6874 6e69  from oml.lightni
-00004860: 6e67 2e6d 6f64 756c 6573 2e65 7874 7261  ng.modules.extra
-00004870: 6374 6f72 2069 6d70 6f72 7420 4578 7472  ctor import Extr
-00004880: 6163 746f 724d 6f64 756c 650a 6672 6f6d  actorModule.from
-00004890: 206f 6d6c 2e6c 6967 6874 6e69 6e67 2e63   oml.lightning.c
-000048a0: 616c 6c62 6163 6b73 2e6d 6574 7269 6320  allbacks.metric 
-000048b0: 696d 706f 7274 204d 6574 7269 6356 616c  import MetricVal
-000048c0: 4361 6c6c 6261 636b 0a66 726f 6d20 6f6d  Callback.from om
-000048d0: 6c2e 6c6f 7373 6573 2e74 7269 706c 6574  l.losses.triplet
-000048e0: 2069 6d70 6f72 7420 5472 6970 6c65 744c   import TripletL
-000048f0: 6f73 7357 6974 684d 696e 6572 0a66 726f  ossWithMiner.fro
-00004900: 6d20 6f6d 6c2e 6d65 7472 6963 732e 656d  m oml.metrics.em
-00004910: 6265 6464 696e 6773 2069 6d70 6f72 7420  beddings import 
-00004920: 456d 6265 6464 696e 674d 6574 7269 6373  EmbeddingMetrics
-00004930: 0a66 726f 6d20 6f6d 6c2e 6d69 6e65 7273  .from oml.miners
-00004940: 2e69 6e62 6174 6368 5f61 6c6c 5f74 7269  .inbatch_all_tri
-00004950: 2069 6d70 6f72 7420 416c 6c54 7269 706c   import AllTripl
-00004960: 6574 734d 696e 6572 0a66 726f 6d20 6f6d  etsMiner.from om
-00004970: 6c2e 6d6f 6465 6c73 2069 6d70 6f72 7420  l.models import 
-00004980: 5669 5445 7874 7261 6374 6f72 0a66 726f  ViTExtractor.fro
-00004990: 6d20 6f6d 6c2e 7361 6d70 6c65 7273 2e62  m oml.samplers.b
-000049a0: 616c 616e 6365 2069 6d70 6f72 7420 4261  alance import Ba
-000049b0: 6c61 6e63 6553 616d 706c 6572 0a66 726f  lanceSampler.fro
-000049c0: 6d20 6f6d 6c2e 7574 696c 732e 646f 776e  m oml.utils.down
-000049d0: 6c6f 6164 5f6d 6f63 6b5f 6461 7461 7365  load_mock_datase
-000049e0: 7420 696d 706f 7274 2064 6f77 6e6c 6f61  t import downloa
-000049f0: 645f 6d6f 636b 5f64 6174 6173 6574 0a66  d_mock_dataset.f
-00004a00: 726f 6d20 7079 746f 7263 685f 6c69 6768  rom pytorch_ligh
-00004a10: 746e 696e 672e 6c6f 6767 6572 7320 696d  tning.loggers im
-00004a20: 706f 7274 204e 6570 7475 6e65 4c6f 6767  port NeptuneLogg
-00004a30: 6572 2c20 5465 6e73 6f72 426f 6172 644c  er, TensorBoardL
-00004a40: 6f67 6765 720a 0a64 6174 6173 6574 5f72  ogger..dataset_r
-00004a50: 6f6f 7420 3d20 226d 6f63 6b5f 6461 7461  oot = "mock_data
-00004a60: 7365 742f 220a 6466 5f74 7261 696e 2c20  set/".df_train, 
-00004a70: 6466 5f76 616c 203d 2064 6f77 6e6c 6f61  df_val = downloa
-00004a80: 645f 6d6f 636b 5f64 6174 6173 6574 2864  d_mock_dataset(d
-00004a90: 6174 6173 6574 5f72 6f6f 7429 0a0a 2320  ataset_root)..# 
-00004aa0: 6d6f 6465 6c0a 6578 7472 6163 746f 7220  model.extractor 
-00004ab0: 3d20 5669 5445 7874 7261 6374 6f72 2822  = ViTExtractor("
-00004ac0: 7669 7473 3136 5f64 696e 6f22 2c20 6172  vits16_dino", ar
-00004ad0: 6368 3d22 7669 7473 3136 222c 206e 6f72  ch="vits16", nor
-00004ae0: 6d61 6c69 7365 5f66 6561 7475 7265 733d  malise_features=
-00004af0: 4661 6c73 6529 0a0a 2320 7472 6169 6e0a  False)..# train.
-00004b00: 6f70 7469 6d69 7a65 7220 3d20 746f 7263  optimizer = torc
-00004b10: 682e 6f70 7469 6d2e 5347 4428 6578 7472  h.optim.SGD(extr
-00004b20: 6163 746f 722e 7061 7261 6d65 7465 7273  actor.parameters
-00004b30: 2829 2c20 6c72 3d31 652d 3629 0a74 7261  (), lr=1e-6).tra
-00004b40: 696e 5f64 6174 6173 6574 203d 2044 6174  in_dataset = Dat
-00004b50: 6173 6574 5769 7468 4c61 6265 6c73 2864  asetWithLabels(d
-00004b60: 665f 7472 6169 6e2c 2064 6174 6173 6574  f_train, dataset
-00004b70: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-00004b80: 6f74 290a 6372 6974 6572 696f 6e20 3d20  ot).criterion = 
-00004b90: 5472 6970 6c65 744c 6f73 7357 6974 684d  TripletLossWithM
-00004ba0: 696e 6572 286d 6172 6769 6e3d 302e 312c  iner(margin=0.1,
-00004bb0: 206d 696e 6572 3d41 6c6c 5472 6970 6c65   miner=AllTriple
-00004bc0: 7473 4d69 6e65 7228 2929 0a62 6174 6368  tsMiner()).batch
-00004bd0: 5f73 616d 706c 6572 203d 2042 616c 616e  _sampler = Balan
-00004be0: 6365 5361 6d70 6c65 7228 7472 6169 6e5f  ceSampler(train_
-00004bf0: 6461 7461 7365 742e 6765 745f 6c61 6265  dataset.get_labe
-00004c00: 6c73 2829 2c20 6e5f 6c61 6265 6c73 3d32  ls(), n_labels=2
-00004c10: 2c20 6e5f 696e 7374 616e 6365 733d 3329  , n_instances=3)
-00004c20: 0a74 7261 696e 5f6c 6f61 6465 7220 3d20  .train_loader = 
-00004c30: 746f 7263 682e 7574 696c 732e 6461 7461  torch.utils.data
-00004c40: 2e44 6174 614c 6f61 6465 7228 7472 6169  .DataLoader(trai
-00004c50: 6e5f 6461 7461 7365 742c 2062 6174 6368  n_dataset, batch
-00004c60: 5f73 616d 706c 6572 3d62 6174 6368 5f73  _sampler=batch_s
-00004c70: 616d 706c 6572 290a 0a23 2076 616c 0a76  ampler)..# val.v
-00004c80: 616c 5f64 6174 6173 6574 203d 2044 6174  al_dataset = Dat
-00004c90: 6173 6574 5175 6572 7947 616c 6c65 7279  asetQueryGallery
-00004ca0: 2864 665f 7661 6c2c 2064 6174 6173 6574  (df_val, dataset
-00004cb0: 5f72 6f6f 743d 6461 7461 7365 745f 726f  _root=dataset_ro
-00004cc0: 6f74 290a 7661 6c5f 6c6f 6164 6572 203d  ot).val_loader =
-00004cd0: 2074 6f72 6368 2e75 7469 6c73 2e64 6174   torch.utils.dat
-00004ce0: 612e 4461 7461 4c6f 6164 6572 2876 616c  a.DataLoader(val
-00004cf0: 5f64 6174 6173 6574 2c20 6261 7463 685f  _dataset, batch_
-00004d00: 7369 7a65 3d34 290a 6d65 7472 6963 5f63  size=4).metric_c
-00004d10: 616c 6c62 6163 6b20 3d20 4d65 7472 6963  allback = Metric
-00004d20: 5661 6c43 616c 6c62 6163 6b28 6d65 7472  ValCallback(metr
-00004d30: 6963 3d45 6d62 6564 6469 6e67 4d65 7472  ic=EmbeddingMetr
-00004d40: 6963 7328 6578 7472 615f 6b65 7973 3d5b  ics(extra_keys=[
-00004d50: 7472 6169 6e5f 6461 7461 7365 742e 7061  train_dataset.pa
-00004d60: 7468 735f 6b65 792c 5d29 2c20 6c6f 675f  ths_key,]), log_
-00004d70: 696d 6167 6573 3d54 7275 6529 0a0a 2320  images=True)..# 
-00004d80: 6c6f 6767 696e 670a 6c6f 6767 6572 203d  logging.logger =
-00004d90: 2054 656e 736f 7242 6f61 7264 4c6f 6767   TensorBoardLogg
-00004da0: 6572 2822 2e22 2920 2023 2046 6f72 2054  er(".")  # For T
-00004db0: 656e 736f 7242 6f61 7264 0a23 206c 6f67  ensorBoard.# log
-00004dc0: 6765 7220 3d20 4e65 7074 756e 654c 6f67  ger = NeptuneLog
-00004dd0: 6765 7228 6170 695f 6b65 793d 2222 2c20  ger(api_key="", 
-00004de0: 7072 6f6a 6563 743d 2222 2c20 6c6f 675f  project="", log_
-00004df0: 6d6f 6465 6c5f 6368 6563 6b70 6f69 6e74  model_checkpoint
-00004e00: 733d 4661 6c73 6529 2020 2320 466f 7220  s=False)  # For 
-00004e10: 4e65 7074 756e 650a 0a23 2072 756e 0a70  Neptune..# run.p
-00004e20: 6c5f 6d6f 6465 6c20 3d20 4578 7472 6163  l_model = Extrac
-00004e30: 746f 724d 6f64 756c 6528 6578 7472 6163  torModule(extrac
-00004e40: 746f 722c 2063 7269 7465 7269 6f6e 2c20  tor, criterion, 
-00004e50: 6f70 7469 6d69 7a65 7229 0a74 7261 696e  optimizer).train
-00004e60: 6572 203d 2070 6c2e 5472 6169 6e65 7228  er = pl.Trainer(
-00004e70: 6d61 785f 6570 6f63 6873 3d33 2c20 6361  max_epochs=3, ca
-00004e80: 6c6c 6261 636b 733d 5b6d 6574 7269 635f  llbacks=[metric_
-00004e90: 6361 6c6c 6261 636b 5d2c 206e 756d 5f73  callback], num_s
-00004ea0: 616e 6974 795f 7661 6c5f 7374 6570 733d  anity_val_steps=
-00004eb0: 302c 206c 6f67 6765 723d 6c6f 6767 6572  0, logger=logger
-00004ec0: 290a 7472 6169 6e65 722e 6669 7428 706c  ).trainer.fit(pl
-00004ed0: 5f6d 6f64 656c 2c20 7472 6169 6e5f 6461  _model, train_da
-00004ee0: 7461 6c6f 6164 6572 733d 7472 6169 6e5f  taloaders=train_
-00004ef0: 6c6f 6164 6572 2c20 7661 6c5f 6461 7461  loader, val_data
-00004f00: 6c6f 6164 6572 733d 7661 6c5f 6c6f 6164  loaders=val_load
-00004f10: 6572 290a 0a60 6060 0a5b 636f 6d6d 656e  er)..```.[commen
-00004f20: 745d 3a6c 6967 6874 6e69 6e67 2d65 6e64  t]:lightning-end
-00004f30: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
-00004f40: 0a0a 5b21 5b4f 7065 6e20 496e 2043 6f6c  ..[![Open In Col
-00004f50: 6162 5d28 6874 7470 733a 2f2f 636f 6c61  ab](https://cola
-00004f60: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-00004f70: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
-00004f80: 6162 2d62 6164 6765 2e73 7667 295d 2868  ab-badge.svg)](h
-00004f90: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00004fa0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00004fb0: 2f64 7269 7665 2f31 6256 5567 6442 4757  /drive/1bVUgdBGW
-00004fc0: 7651 6743 6b62 6132 5974 6149 5256 6c55  vQgCkba2YtaIRVlU
-00004fd0: 5155 7a37 5136 305a 3f75 7370 3d73 6861  QUz7Q60Z?usp=sha
-00004fe0: 7265 5f6c 696e 6b29 0a3c 6465 7461 696c  re_link).<detail
-00004ff0: 733e 0a3c 7375 6d6d 6172 793e 5573 696e  s>.<summary>Usin
-00005000: 6720 6120 7472 6169 6e65 6420 6d6f 6465  g a trained mode
-00005010: 6c20 666f 7220 7265 7472 6965 7661 6c3c  l for retrieval<
-00005020: 2f73 756d 6d61 7279 3e0a 3c70 3e0a 0a5b  /summary>.<p>..[
-00005030: 636f 6d6d 656e 745d 3a75 7361 6765 2d72  comment]:usage-r
-00005040: 6574 7269 6576 616c 2d73 7461 7274 0a60  etrieval-start.`
-00005050: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00005060: 746f 7263 680a 0a66 726f 6d20 6f6d 6c2e  torch..from oml.
-00005070: 636f 6e73 7420 696d 706f 7274 204d 4f43  const import MOC
-00005080: 4b5f 4441 5441 5345 545f 5041 5448 0a66  K_DATASET_PATH.f
-00005090: 726f 6d20 6f6d 6c2e 696e 6665 7265 6e63  rom oml.inferenc
-000050a0: 652e 666c 6174 2069 6d70 6f72 7420 696e  e.flat import in
-000050b0: 6665 7265 6e63 655f 6f6e 5f69 6d61 6765  ference_on_image
-000050c0: 730a 6672 6f6d 206f 6d6c 2e6d 6f64 656c  s.from oml.model
-000050d0: 7320 696d 706f 7274 2056 6954 4578 7472  s import ViTExtr
-000050e0: 6163 746f 720a 6672 6f6d 206f 6d6c 2e72  actor.from oml.r
-000050f0: 6567 6973 7472 792e 7472 616e 7366 6f72  egistry.transfor
-00005100: 6d73 2069 6d70 6f72 7420 6765 745f 7472  ms import get_tr
-00005110: 616e 7366 6f72 6d73 5f66 6f72 5f70 7265  ansforms_for_pre
-00005120: 7472 6169 6e65 640a 6672 6f6d 206f 6d6c  trained.from oml
-00005130: 2e75 7469 6c73 2e64 6f77 6e6c 6f61 645f  .utils.download_
-00005140: 6d6f 636b 5f64 6174 6173 6574 2069 6d70  mock_dataset imp
-00005150: 6f72 7420 646f 776e 6c6f 6164 5f6d 6f63  ort download_moc
-00005160: 6b5f 6461 7461 7365 740a 6672 6f6d 206f  k_dataset.from o
-00005170: 6d6c 2e75 7469 6c73 2e6d 6973 635f 746f  ml.utils.misc_to
-00005180: 7263 6820 696d 706f 7274 2070 6169 7277  rch import pairw
-00005190: 6973 655f 6469 7374 0a0a 5f2c 2064 665f  ise_dist.._, df_
-000051a0: 7661 6c20 3d20 646f 776e 6c6f 6164 5f6d  val = download_m
-000051b0: 6f63 6b5f 6461 7461 7365 7428 4d4f 434b  ock_dataset(MOCK
-000051c0: 5f44 4154 4153 4554 5f50 4154 4829 0a64  _DATASET_PATH).d
-000051d0: 665f 7661 6c5b 2270 6174 6822 5d20 3d20  f_val["path"] = 
-000051e0: 6466 5f76 616c 5b22 7061 7468 225d 2e61  df_val["path"].a
-000051f0: 7070 6c79 286c 616d 6264 6120 783a 204d  pply(lambda x: M
-00005200: 4f43 4b5f 4441 5441 5345 545f 5041 5448  OCK_DATASET_PATH
-00005210: 202f 2078 290a 7175 6572 6965 7320 3d20   / x).queries = 
-00005220: 6466 5f76 616c 5b64 665f 7661 6c5b 2269  df_val[df_val["i
-00005230: 735f 7175 6572 7922 5d5d 5b22 7061 7468  s_query"]]["path
-00005240: 225d 2e74 6f6c 6973 7428 290a 6761 6c6c  "].tolist().gall
-00005250: 6572 6965 7320 3d20 6466 5f76 616c 5b64  eries = df_val[d
-00005260: 665f 7661 6c5b 2269 735f 6761 6c6c 6572  f_val["is_galler
-00005270: 7922 5d5d 5b22 7061 7468 225d 2e74 6f6c  y"]]["path"].tol
-00005280: 6973 7428 290a 0a65 7874 7261 6374 6f72  ist()..extractor
-00005290: 203d 2056 6954 4578 7472 6163 746f 722e   = ViTExtractor.
-000052a0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-000052b0: 2276 6974 7331 365f 6469 6e6f 2229 0a74  "vits16_dino").t
-000052c0: 7261 6e73 666f 726d 2c20 5f20 3d20 6765  ransform, _ = ge
-000052d0: 745f 7472 616e 7366 6f72 6d73 5f66 6f72  t_transforms_for
-000052e0: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-000052f0: 7331 365f 6469 6e6f 2229 0a0a 6172 6773  s16_dino")..args
-00005300: 203d 207b 226e 756d 5f77 6f72 6b65 7273   = {"num_workers
-00005310: 223a 2030 2c20 2262 6174 6368 5f73 697a  ": 0, "batch_siz
-00005320: 6522 3a20 387d 0a66 6561 7475 7265 735f  e": 8}.features_
-00005330: 7175 6572 6965 7320 3d20 696e 6665 7265  queries = infere
-00005340: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-00005350: 7472 6163 746f 722c 2070 6174 6873 3d71  tractor, paths=q
-00005360: 7565 7269 6573 2c20 7472 616e 7366 6f72  ueries, transfor
-00005370: 6d3d 7472 616e 7366 6f72 6d2c 202a 2a61  m=transform, **a
-00005380: 7267 7329 0a66 6561 7475 7265 735f 6761  rgs).features_ga
-00005390: 6c6c 6572 6965 7320 3d20 696e 6665 7265  lleries = infere
-000053a0: 6e63 655f 6f6e 5f69 6d61 6765 7328 6578  nce_on_images(ex
-000053b0: 7472 6163 746f 722c 2070 6174 6873 3d67  tractor, paths=g
-000053c0: 616c 6c65 7269 6573 2c20 7472 616e 7366  alleries, transf
-000053d0: 6f72 6d3d 7472 616e 7366 6f72 6d2c 202a  orm=transform, *
-000053e0: 2a61 7267 7329 0a0a 2320 4e6f 7720 7765  *args)..# Now we
-000053f0: 2063 616e 2065 7870 6c69 6369 746c 7920   can explicitly 
-00005400: 6275 696c 6420 7061 6972 7769 7365 206d  build pairwise m
-00005410: 6174 7269 7820 6f66 2064 6973 7461 6e63  atrix of distanc
-00005420: 6573 206f 7220 7361 7665 2079 6f75 2052  es or save you R
-00005430: 414d 2076 6961 2075 7369 6e67 206b 4e4e  AM via using kNN
-00005440: 0a75 7365 5f6b 6e6e 203d 2054 7275 650a  .use_knn = True.
-00005450: 746f 705f 6b20 3d20 330a 0a69 6620 7573  top_k = 3..if us
-00005460: 655f 6b6e 6e3a 0a20 2020 2066 726f 6d20  e_knn:.    from 
-00005470: 736b 6c65 6172 6e2e 6e65 6967 6862 6f72  sklearn.neighbor
-00005480: 7320 696d 706f 7274 204e 6561 7265 7374  s import Nearest
-00005490: 4e65 6967 6862 6f72 730a 2020 2020 6b6e  Neighbors.    kn
-000054a0: 6e20 3d20 4e65 6172 6573 744e 6569 6768  n = NearestNeigh
-000054b0: 626f 7273 2861 6c67 6f72 6974 686d 3d22  bors(algorithm="
-000054c0: 6175 746f 222c 2070 3d32 290a 2020 2020  auto", p=2).    
-000054d0: 6b6e 6e2e 6669 7428 6665 6174 7572 6573  knn.fit(features
-000054e0: 5f67 616c 6c65 7269 6573 290a 2020 2020  _galleries).    
-000054f0: 6469 7374 732c 2069 695f 636c 6f73 6573  dists, ii_closes
-00005500: 7420 3d20 6b6e 6e2e 6b6e 6569 6768 626f  t = knn.kneighbo
-00005510: 7273 2866 6561 7475 7265 735f 7175 6572  rs(features_quer
-00005520: 6965 732c 206e 5f6e 6569 6768 626f 7273  ies, n_neighbors
-00005530: 3d74 6f70 5f6b 2c20 7265 7475 726e 5f64  =top_k, return_d
-00005540: 6973 7461 6e63 653d 5472 7565 290a 0a65  istance=True)..e
-00005550: 6c73 653a 0a20 2020 2064 6973 745f 6d61  lse:.    dist_ma
-00005560: 7420 3d20 7061 6972 7769 7365 5f64 6973  t = pairwise_dis
-00005570: 7428 7831 3d66 6561 7475 7265 735f 7175  t(x1=features_qu
-00005580: 6572 6965 732c 2078 323d 6665 6174 7572  eries, x2=featur
-00005590: 6573 5f67 616c 6c65 7269 6573 290a 2020  es_galleries).  
-000055a0: 2020 6469 7374 732c 2069 695f 636c 6f73    dists, ii_clos
-000055b0: 6573 7420 3d20 746f 7263 682e 746f 706b  est = torch.topk
-000055c0: 2864 6973 745f 6d61 742c 2064 696d 3d31  (dist_mat, dim=1
-000055d0: 2c20 6b3d 746f 705f 6b2c 206c 6172 6765  , k=top_k, large
-000055e0: 7374 3d46 616c 7365 290a 0a70 7269 6e74  st=False)..print
-000055f0: 2866 2254 6f70 207b 746f 705f 6b7d 2069  (f"Top {top_k} i
-00005600: 7465 6d73 2063 6c6f 7365 7374 2074 6f20  tems closest to 
-00005610: 7175 6572 6965 7320 6172 653a 5c6e 207b  queries are:\n {
-00005620: 6969 5f63 6c6f 7365 7374 7d22 290a 6060  ii_closest}").``
-00005630: 600a 5b63 6f6d 6d65 6e74 5d3a 7573 6167  `.[comment]:usag
-00005640: 652d 7265 7472 6965 7661 6c2d 656e 640a  e-retrieval-end.
-00005650: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
-00005660: 0a5b 215b 4f70 656e 2049 6e20 436f 6c61  .[![Open In Cola
-00005670: 625d 2868 7474 7073 3a2f 2f63 6f6c 6162  b](https://colab
-00005680: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00005690: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
-000056a0: 622d 6261 6467 652e 7376 6729 5d28 6874  b-badge.svg)](ht
-000056b0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-000056c0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-000056d0: 6472 6976 652f 3153 326e 4b36 4b61 5265  drive/1S2nK6KaRe
-000056e0: 446d 2d52 6a6a 646f 6a64 4964 3643 616b  Dm-RjjdojdId6Cak
-000056f0: 6868 5379 7666 413f 7573 703d 7368 6172  hhSyvfA?usp=shar
-00005700: 655f 6c69 6e6b 290a 0a5b 2a2a 5363 6865  e_link)..[**Sche
-00005710: 6d61 732c 2065 7870 6c61 6e61 7469 6f6e  mas, explanation
-00005720: 7320 616e 6420 7469 7073 2a2a 5d28 6874  s and tips**](ht
-00005730: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005740: 2f4f 4d4c 2d54 6561 6d2f 6f70 656e 2d6d  /OML-Team/open-m
-00005750: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
-00005760: 7265 652f 6d61 696e 2f70 6970 656c 696e  ree/main/pipelin
-00005770: 6573 2f66 6561 7475 7265 735f 6578 7472  es/features_extr
-00005780: 6163 7469 6f6e 290a 0a53 6565 205b 6578  action)..See [ex
-00005790: 7472 6120 636f 6465 2073 6e69 7070 6574  tra code snippet
-000057a0: 735d 2868 7474 7073 3a2f 2f6f 7065 6e2d  s](https://open-
-000057b0: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-000057c0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000057d0: 6e2f 6c61 7465 7374 2f66 6561 7475 7265  n/latest/feature
-000057e0: 5f65 7874 7261 6374 696f 6e2f 7079 7468  _extraction/pyth
-000057f0: 6f6e 5f65 7861 6d70 6c65 732e 6874 6d6c  on_examples.html
-00005800: 292c 2069 6e63 6c75 6469 6e67 3a0a 2a20  ), including:.* 
-00005810: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
-00005820: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
-00005830: 6e69 6e67 0a2a 2054 7261 696e 696e 6720  ning.* Training 
-00005840: 2b20 5661 6c69 6461 7469 6f6e 2077 6974  + Validation wit
-00005850: 6820 4c69 6768 746e 696e 6720 696e 2044  h Lightning in D
-00005860: 4450 206d 6f64 650a 2a20 5472 6169 6e69  DP mode.* Traini
-00005870: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-00005880: 726f 6d20 504d 4c0a 2a20 5472 6169 6e69  rom PML.* Traini
-00005890: 6e67 2077 6974 6820 6c6f 7373 6573 2066  ng with losses f
-000058a0: 726f 6d20 504d 4c20 6164 7661 6e63 6564  rom PML advanced
-000058b0: 2028 7061 7373 696e 6720 6469 7374 616e   (passing distan
-000058c0: 6365 2c20 7265 6475 6365 722c 206d 696e  ce, reducer, min
-000058d0: 6572 290a 0a23 2320 5b50 6970 656c 696e  er)..## [Pipelin
-000058e0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-000058f0: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
-00005900: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
-00005910: 6e69 6e67 2f74 7265 652f 6d61 696e 2f70  ning/tree/main/p
-00005920: 6970 656c 696e 6573 290a 0a50 6970 656c  ipelines)..Pipel
-00005930: 696e 6573 2070 726f 7669 6465 2061 2077  ines provide a w
-00005940: 6179 2074 6f20 7275 6e20 6d65 7472 6963  ay to run metric
-00005950: 206c 6561 726e 696e 6720 6578 7065 7269   learning experi
-00005960: 6d65 6e74 7320 7669 6120 6368 616e 6769  ments via changi
-00005970: 6e67 206f 6e6c 7920 7468 6520 636f 6e66  ng only the conf
-00005980: 6967 2066 696c 652e 0a41 6c6c 2079 6f75  ig file..All you
-00005990: 206e 6565 6420 6973 2074 6f20 7072 6570   need is to prep
-000059a0: 6172 6520 796f 7572 2064 6174 6173 6574  are your dataset
-000059b0: 2069 6e20 6120 7265 7175 6972 6564 2066   in a required f
-000059c0: 6f72 6d61 742e 0a0a 5365 6520 5b50 6970  ormat...See [Pip
-000059d0: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-000059e0: 6769 7468 7562 2e63 6f6d 2f4f 4d4c 2d54  github.com/OML-T
-000059f0: 6561 6d2f 6f70 656e 2d6d 6574 7269 632d  eam/open-metric-
-00005a00: 6c65 6172 6e69 6e67 2f62 6c6f 622f 6d61  learning/blob/ma
-00005a10: 696e 2f70 6970 656c 696e 6573 2f29 2066  in/pipelines/) f
-00005a20: 6f6c 6465 7220 666f 7220 6d6f 7265 2064  older for more d
-00005a30: 6574 6169 6c73 3a0a 2a20 4665 6174 7572  etails:.* Featur
-00005a40: 6520 6578 7472 6163 746f 7220 5b70 6970  e extractor [pip
-00005a50: 656c 696e 655d 2868 7474 7073 3a2f 2f67  eline](https://g
-00005a60: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
-00005a70: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
-00005a80: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
-00005a90: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
-00005aa0: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
-00005ab0: 0a2a 2052 6574 7269 6576 616c 2070 6f73  .* Retrieval pos
-00005ac0: 7470 726f 6365 7373 6f72 205b 7069 7065  tprocessor [pipe
-00005ad0: 6c69 6e65 5d28 6874 7470 733a 2f2f 6769  line](https://gi
-00005ae0: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
-00005af0: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
-00005b00: 6172 6e69 6e67 2f74 7265 652f 6d61 696e  arning/tree/main
-00005b10: 2f70 6970 656c 696e 6573 2f70 6f73 7470  /pipelines/postp
-00005b20: 726f 6365 7373 696e 6729 2028 7265 2d72  rocessing) (re-r
-00005b30: 616e 6b69 6e67 290a 0a23 2320 5b5a 6f6f  anking)..## [Zoo
-00005b40: 5d28 6874 7470 733a 2f2f 6f70 656e 2d6d  ](https://open-m
-00005b50: 6574 7269 632d 6c65 6172 6e69 6e67 2e72  etric-learning.r
-00005b60: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00005b70: 2f6c 6174 6573 742f 6665 6174 7572 655f  /latest/feature_
-00005b80: 6578 7472 6163 7469 6f6e 2f7a 6f6f 2e68  extraction/zoo.h
-00005b90: 746d 6c29 0a0a 4265 6c6f 7720 6172 6520  tml)..Below are 
-00005ba0: 7468 6520 6d6f 6465 6c73 2074 7261 696e  the models train
-00005bb0: 6564 2077 6974 6820 4f4d 4c20 6f6e 2034  ed with OML on 4
-00005bc0: 2070 7562 6c69 6320 6461 7461 7365 7473   public datasets
-00005bd0: 2e0a 416c 6c20 6d65 7472 6963 7320 6265  ..All metrics be
-00005be0: 6c6f 7720 7765 7265 206f 6274 6169 6e65  low were obtaine
-00005bf0: 6420 6f6e 2074 6865 2069 6d61 6765 7320  d on the images 
-00005c00: 7769 7468 2074 6865 2073 697a 6573 206f  with the sizes o
-00005c10: 6620 2a2a 3232 3420 7820 3232 342a 2a3a  f **224 x 224**:
-00005c20: 0a0a 7c20 2020 2020 2020 2020 2020 2020  ..|             
-00005c30: 2020 2020 2020 2020 206d 6f64 656c 2020           model  
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 7c20 636d 6331 2020 7c20 2020      | cmc1  |   
-00005c60: 2020 2020 2020 6461 7461 7365 7420 2020        dataset   
-00005c70: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 7765 6967 6874 7320 2020        weights   
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+00000020: 7474 7073 3a2f 2f69 2e69 6262 2e63 6f2f  ttps://i.ibb.co/
+00000030: 7773 6d44 3572 342f 7068 6f74 6f2d 3230  wsmD5r4/photo-20
+00000040: 3232 2d30 362d 3036 2d31 372d 3430 2d35  22-06-06-17-40-5
+00000050: 322e 6a70 6722 2077 6964 7468 3d22 3430  2.jpg" width="40
+00000060: 3070 7822 3e0a 0a21 5b65 7861 6d70 6c65  0px">..![example
+00000070: 2077 6f72 6b66 6c6f 775d 2868 7474 7073   workflow](https
+00000080: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+00000090: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000000a0: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
+000000b0: 6f6e 732f 776f 726b 666c 6f77 732f 7072  ons/workflows/pr
+000000c0: 652d 636f 6d6d 6974 2d77 6f72 6b66 6c6f  e-commit-workflo
+000000d0: 772e 7961 6d6c 2f62 6164 6765 2e73 7667  w.yaml/badge.svg
+000000e0: 290a 215b 6578 616d 706c 6520 776f 726b  ).![example work
+000000f0: 666c 6f77 5d28 6874 7470 733a 2f2f 6769  flow](https://gi
+00000100: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
+00000110: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
+00000120: 6172 6e69 6e67 2f61 6374 696f 6e73 2f77  arning/actions/w
+00000130: 6f72 6b66 6c6f 7773 2f74 6573 7473 2d77  orkflows/tests-w
+00000140: 6f72 6b66 6c6f 772e 7961 6d6c 2f62 6164  orkflow.yaml/bad
+00000150: 6765 2e73 7667 3f29 0a5b 215b 446f 6375  ge.svg?).[![Docu
+00000160: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000170: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
+00000180: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+00000190: 7473 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ts/open-metric-l
+000001a0: 6561 726e 696e 672f 6261 6467 652f 3f76  earning/badge/?v
+000001b0: 6572 7369 6f6e 3d6c 6174 6573 7429 5d28  ersion=latest)](
+000001c0: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
+000001d0: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
+000001e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000001f0: 6174 6573 742f 3f62 6164 6765 3d6c 6174  atest/?badge=lat
+00000200: 6573 7429 0a5b 215b 5079 5049 2053 7461  est).[![PyPI Sta
+00000210: 7475 735d 2868 7474 7073 3a2f 2f70 6570  tus](https://pep
+00000220: 792e 7465 6368 2f62 6164 6765 2f6f 7065  y.tech/badge/ope
+00000230: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
+00000240: 6729 5d28 6874 7470 733a 2f2f 7065 7079  g)](https://pepy
+00000250: 2e74 6563 682f 7072 6f6a 6563 742f 6f70  .tech/project/op
+00000260: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
+00000270: 6e67 290a 5b21 5b50 6970 6920 7665 7273  ng).[![Pipi vers
+00000280: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
+00000290: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000002a0: 2f76 2f6f 7065 6e2d 6d65 7472 6963 2d6c  /v/open-metric-l
+000002b0: 6561 726e 696e 672e 7376 6729 5d28 6874  earning.svg)](ht
+000002c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000002d0: 726f 6a65 6374 2f6f 7065 6e2d 6d65 7472  roject/open-metr
+000002e0: 6963 2d6c 6561 726e 696e 672f 290a 215b  ic-learning/).![
+000002f0: 6578 616d 706c 6520 776f 726b 666c 6f77  example workflow
+00000300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000310: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
+00000320: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
+00000330: 6e67 2f61 6374 696f 6e73 2f77 6f72 6b66  ng/actions/workf
+00000340: 6c6f 7773 2f70 7974 686f 6e2d 7665 7273  lows/python-vers
+00000350: 696f 6e73 2e79 616d 6c2f 6261 6467 652e  ions.yaml/badge.
+00000360: 7376 673f 290a 5b21 5b70 7974 686f 6e5d  svg?).[![python]
+00000370: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000380: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00000390: 7468 6f6e 5f33 2e37 2d70 6173 7369 6e67  thon_3.7-passing
+000003a0: 2d73 7563 6365 7373 295d 2868 7474 7073  -success)](https
+000003b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+000003c0: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+000003d0: 6963 2d6c 6561 726e 696e 672f 6163 7469  ic-learning/acti
+000003e0: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+000003f0: 7468 6f6e 2d76 6572 7369 6f6e 732e 7961  thon-versions.ya
+00000400: 6d6c 2f62 6164 6765 2e73 7667 3f29 0a5b  ml/badge.svg?).[
+00000410: 215b 7079 7468 6f6e 5d28 6874 7470 733a  ![python](https:
+00000420: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000430: 2f62 6164 6765 2f70 7974 686f 6e5f 332e  /badge/python_3.
+00000440: 382d 7061 7373 696e 672d 7375 6363 6573  8-passing-succes
+00000450: 7329 5d28 6874 7470 733a 2f2f 6769 7468  s)](https://gith
+00000460: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
+00000470: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00000480: 6e69 6e67 2f61 6374 696f 6e73 2f77 6f72  ning/actions/wor
+00000490: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7665  kflows/python-ve
+000004a0: 7273 696f 6e73 2e79 616d 6c2f 6261 6467  rsions.yaml/badg
+000004b0: 652e 7376 673f 290a 5b21 5b70 7974 686f  e.svg?).[![pytho
+000004c0: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+000004d0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000004e0: 7079 7468 6f6e 5f33 2e39 2d70 6173 7369  python_3.9-passi
+000004f0: 6e67 2d73 7563 6365 7373 295d 2868 7474  ng-success)](htt
+00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000510: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
+00000520: 7472 6963 2d6c 6561 726e 696e 672f 6163  tric-learning/ac
+00000530: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000540: 7079 7468 6f6e 2d76 6572 7369 6f6e 732e  python-versions.
+00000550: 7961 6d6c 2f62 6164 6765 2e73 7667 3f29  yaml/badge.svg?)
+00000560: 0a5b 215b 7079 7468 6f6e 5d28 6874 7470  .[![python](http
+00000570: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000580: 696f 2f62 6164 6765 2f70 7974 686f 6e5f  io/badge/python_
+00000590: 332e 3130 2d70 6173 7369 6e67 2d73 7563  3.10-passing-suc
+000005a0: 6365 7373 295d 2868 7474 7073 3a2f 2f67  cess)](https://g
+000005b0: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
+000005c0: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
+000005d0: 6561 726e 696e 672f 6163 7469 6f6e 732f  earning/actions/
+000005e0: 776f 726b 666c 6f77 732f 7079 7468 6f6e  workflows/python
+000005f0: 2d76 6572 7369 6f6e 732e 7961 6d6c 2f62  -versions.yaml/b
+00000600: 6164 6765 2e73 7667 3f29 0a0a 4f4d 4c20  adge.svg?)..OML 
+00000610: 6973 2061 2050 7954 6f72 6368 2d62 6173  is a PyTorch-bas
+00000620: 6564 2066 7261 6d65 776f 726b 2074 6f20  ed framework to 
+00000630: 7472 6169 6e20 616e 6420 7661 6c69 6461  train and valida
+00000640: 7465 2074 6865 206d 6f64 656c 7320 7072  te the models pr
+00000650: 6f64 7563 696e 6720 6869 6768 2d71 7561  oducing high-qua
+00000660: 6c69 7479 2065 6d62 6564 6469 6e67 732e  lity embeddings.
+00000670: 0a0a 2323 2320 5472 7573 7465 6420 6279  ..### Trusted by
+00000680: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000690: 6e74 6572 223e 0a3c 6120 6872 6566 3d22  nter">.<a href="
+000006a0: 6874 7470 733a 2f2f 646f 6373 2e6e 6570  https://docs.nep
+000006b0: 7475 6e65 2e61 692f 696e 7465 6772 6174  tune.ai/integrat
+000006c0: 696f 6e73 2f63 6f6d 6d75 6e69 7479 5f64  ions/community_d
+000006d0: 6576 656c 6f70 6564 2f22 2074 6172 6765  eveloped/" targe
+000006e0: 743d 225f 626c 616e 6b22 3e3c 696d 6720  t="_blank"><img 
+000006f0: 7372 633d 2268 7474 7073 3a2f 2f73 6563  src="https://sec
+00000700: 7572 6974 792e 6e65 7074 756e 652e 6169  urity.neptune.ai
+00000710: 2f61 7069 2f73 6861 7265 2f62 3730 3766  /api/share/b707f
+00000720: 3165 382d 6532 3837 2d34 6630 312d 6235  1e8-e287-4f01-b5
+00000730: 3930 2d33 3961 3666 6137 6539 6661 612f  90-39a6fa7e9faa/
+00000740: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
+00000750: 2231 3030 222f 3e3c 2f61 3ee3 85a4 e385  "100"/></a>.....
+00000760: a40a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000770: 3a2f 2f77 7777 2e6e 6577 796f 726b 6572  ://www.newyorker
+00000780: 2e64 652f 2220 7461 7267 6574 3d22 5f62  .de/" target="_b
+00000790: 6c61 6e6b 223e 3c69 6d67 2073 7263 3d22  lank"><img src="
+000007a0: 6874 7470 733a 2f2f 7570 6c6f 6164 2e77  https://upload.w
+000007b0: 696b 696d 6564 6961 2e6f 7267 2f77 696b  ikimedia.org/wik
+000007c0: 6970 6564 6961 2f63 6f6d 6d6f 6e73 2f74  ipedia/commons/t
+000007d0: 6875 6d62 2f64 2f64 382f 4e65 775f 596f  humb/d/d8/New_Yo
+000007e0: 726b 6572 2e73 7667 2f31 3238 3070 782d  rker.svg/1280px-
+000007f0: 4e65 775f 596f 726b 6572 2e73 7667 2e70  New_Yorker.svg.p
+00000800: 6e67 2220 7769 6474 683d 2231 3030 222f  ng" width="100"/
+00000810: 3e3c 2f61 3ee3 85a4 e385 a40a 3c61 2068  ></a>.......<a h
+00000820: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000830: 2e65 706f 6368 382e 636f 2f22 2074 6172  .epoch8.co/" tar
+00000840: 6765 743d 225f 626c 616e 6b22 3e3c 696d  get="_blank"><im
+00000850: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000860: 2e69 6262 2e63 6f2f 4764 4e56 5479 742f  .ibb.co/GdNVTyt/
+00000870: 5363 7265 656e 7368 6f74 2d32 3032 332d  Screenshot-2023-
+00000880: 3037 2d30 342d 6174 2d31 312d 3139 2d32  07-04-at-11-19-2
+00000890: 342e 706e 6722 2077 6964 7468 3d22 3130  4.png" width="10
+000008a0: 3022 2f3e 3c2f 613e e385 a4e3 85a4 0a3c  0"/></a>.......<
+000008b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000008c0: 7777 772e 6d65 6974 7561 6e2e 636f 6d22  www.meituan.com"
+000008d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000008e0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+000008f0: 3a2f 2f75 706c 6f61 642e 7769 6b69 6d65  ://upload.wikime
+00000900: 6469 612e 6f72 672f 7769 6b69 7065 6469  dia.org/wikipedi
+00000910: 612f 636f 6d6d 6f6e 732f 362f 3631 2f4d  a/commons/6/61/M
+00000920: 6569 7475 616e 5f45 6e67 6c69 7368 5f4c  eituan_English_L
+00000930: 6f67 6f2e 706e 6722 2077 6964 7468 3d22  ogo.png" width="
+00000940: 3130 3022 2f3e 3c2f 613e 0a0a 3c61 2068  100"/></a>..<a h
+00000950: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00000960: 2e6f 782e 6163 2e75 6b2f 2220 7461 7267  .ox.ac.uk/" targ
+00000970: 6574 3d22 5f62 6c61 6e6b 223e 3c69 6d67  et="_blank"><img
+00000980: 2073 7263 3d22 6874 7470 733a 2f2f 7570   src="https://up
+00000990: 6c6f 6164 2e77 696b 696d 6564 6961 2e6f  load.wikimedia.o
+000009a0: 7267 2f77 696b 6970 6564 6961 2f65 6e2f  rg/wikipedia/en/
+000009b0: 7468 756d 622f 322f 3266 2f55 6e69 7665  thumb/2/2f/Unive
+000009c0: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+000009d0: 7376 672f 3235 3630 7078 2d55 6e69 7665  svg/2560px-Unive
+000009e0: 7273 6974 795f 6f66 5f4f 7866 6f72 642e  rsity_of_Oxford.
+000009f0: 7376 672e 706e 6722 2077 6964 7468 3d22  svg.png" width="
+00000a00: 3132 3022 2f3e 3c2f 613e e385 a4e3 85a4  120"/></a>......
+00000a10: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000a20: 2f2f 7777 772e 6873 652e 7275 2f65 6e2f  //www.hse.ru/en/
+00000a30: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000a40: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000a50: 733a 2f2f 7777 772e 6873 652e 7275 2f64  s://www.hse.ru/d
+00000a60: 6174 612f 3230 3230 2f31 312f 3136 2f31  ata/2020/11/16/1
+00000a70: 3336 3732 3734 3034 342f 4853 455f 556e  367274044/HSE_Un
+00000a80: 6976 6572 7369 7479 5f62 6c75 652e 6a70  iversity_blue.jp
+00000a90: 672e 2832 3330 7838 3678 3132 3329 2e6a  g.(230x86x123).j
+00000aa0: 7067 2220 7769 6474 683d 2231 3030 222f  pg" width="100"/
+00000ab0: 3e3c 2f61 3e0a 0a54 6865 7265 2069 7320  ></a>..There is 
+00000ac0: 6120 6e75 6d62 6572 206f 6620 7065 6f70  a number of peop
+00000ad0: 6c65 2066 726f 6d0a 5b4f 7866 6f72 645d  le from.[Oxford]
+00000ae0: 2868 7474 7073 3a2f 2f77 7777 2e6f 782e  (https://www.ox.
+00000af0: 6163 2e75 6b2f 2920 616e 640a 5b48 5345  ac.uk/) and.[HSE
+00000b00: 5d28 6874 7470 733a 2f2f 7777 772e 6873  ](https://www.hs
+00000b10: 652e 7275 2f65 6e2f 290a 756e 6976 6572  e.ru/en/).univer
+00000b20: 7369 7469 6573 2077 686f 2068 6176 6520  sities who have 
+00000b30: 7573 6564 204f 4d4c 2069 6e20 7468 6569  used OML in thei
+00000b40: 7220 7468 6573 6573 2e0a 5b5b 315d 5d28  r theses..[[1]](
+00000b50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b60: 6f6d 2f6e 696c 6f6d 722f 6f70 656e 2d6d  om/nilomr/open-m
+00000b70: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+00000b80: 7265 652f 6772 6561 742d 7469 742f 6772  ree/great-tit/gr
+00000b90: 6561 742d 7469 742d 7472 6169 6e29 0a5b  eat-tit-train).[
+00000ba0: 5b32 5d5d 2868 7474 7073 3a2f 2f67 6974  [2]](https://git
+00000bb0: 6875 622e 636f 6d2f 6e61 7374 7967 6f72  hub.com/nastygor
+00000bc0: 6f64 692f 5052 4f4a 4543 542d 4465 6570  odi/PROJECT-Deep
+00000bd0: 5f4d 6574 7269 635f 4c65 6172 6e69 6e67  _Metric_Learning
+00000be0: 290a 5b5b 335d 5d28 6874 7470 733a 2f2f  ).[[3]](https://
+00000bf0: 6769 7468 7562 2e63 6f6d 2f6e 696b 2d66  github.com/nik-f
+00000c00: 6564 6f72 6f76 2f74 6572 6d5f 7061 7065  edorov/term_pape
+00000c10: 725f 6d65 7472 6963 5f6c 6561 726e 696e  r_metric_learnin
+00000c20: 6729 0a0a 3c64 6976 2061 6c69 676e 3d22  g)..<div align="
+00000c30: 6c65 6674 223e 0a0a 2323 205b 4641 515d  left">..## [FAQ]
+00000c40: 2868 7474 7073 3a2f 2f6f 7065 6e2d 6d65  (https://open-me
+00000c50: 7472 6963 2d6c 6561 726e 696e 672e 7265  tric-learning.re
+00000c60: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000c70: 6c61 7465 7374 2f6f 6d6c 2f66 6171 2e68  latest/oml/faq.h
+00000c80: 746d 6c29 0a0a 3c64 6574 6169 6c73 3e0a  tml)..<details>.
+00000c90: 3c73 756d 6d61 7279 3e57 6879 2064 6f20  <summary>Why do 
+00000ca0: 4920 6e65 6564 204f 4d4c 3f3c 2f73 756d  I need OML?</sum
+00000cb0: 6d61 7279 3e0a 3c70 3e0a 0a59 6f75 206d  mary>.<p>..You m
+00000cc0: 6179 2074 6869 6e6b 202a 2249 6620 4920  ay think *"If I 
+00000cd0: 6e65 6564 2069 6d61 6765 2065 6d62 6564  need image embed
+00000ce0: 6469 6e67 7320 4920 6361 6e20 7369 6d70  dings I can simp
+00000cf0: 6c79 2074 7261 696e 2061 2076 616e 696c  ly train a vanil
+00000d00: 6c61 2063 6c61 7373 6966 6965 7220 616e  la classifier an
+00000d10: 6420 7461 6b65 2069 7473 2070 656e 756c  d take its penul
+00000d20: 7469 6d61 7465 206c 6179 6572 222a 2e0a  timate layer"*..
+00000d30: 5765 6c6c 2c20 6974 206d 616b 6573 2073  Well, it makes s
+00000d40: 656e 7365 2061 7320 6120 7374 6172 7469  ense as a starti
+00000d50: 6e67 2070 6f69 6e74 2e20 4275 7420 7468  ng point. But th
+00000d60: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
+00000d70: 706f 7373 6962 6c65 2064 7261 7762 6163  possible drawbac
+00000d80: 6b73 3a0a 0a2a 2049 6620 796f 7520 7761  ks:..* If you wa
+00000d90: 6e74 2074 6f20 7573 6520 656d 6265 6464  nt to use embedd
+00000da0: 696e 6773 2074 6f20 7065 7266 6f72 6d20  ings to perform 
+00000db0: 7365 6172 6368 696e 6720 796f 7520 6e65  searching you ne
+00000dc0: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
+00000dd0: 736f 6d65 2064 6973 7461 6e63 6520 616d  some distance am
+00000de0: 6f6e 6720 7468 656d 2028 666f 7220 6578  ong them (for ex
+00000df0: 616d 706c 652c 2063 6f73 696e 6520 6f72  ample, cosine or
+00000e00: 204c 3229 2e0a 2020 5573 7561 6c6c 792c   L2)..  Usually,
+00000e10: 202a 2a79 6f75 2064 6f6e 2774 2064 6972   **you don't dir
+00000e20: 6563 746c 7920 6f70 7469 6d69 7a65 2074  ectly optimize t
+00000e30: 6865 7365 2064 6973 7461 6e63 6573 2064  hese distances d
+00000e40: 7572 696e 6720 7468 6520 7472 6169 6e69  uring the traini
+00000e50: 6e67 2a2a 2069 6e20 7468 6520 636c 6173  ng** in the clas
+00000e60: 7369 6669 6361 7469 6f6e 2073 6574 7570  sification setup
+00000e70: 2e20 536f 2c20 796f 7520 6361 6e20 6f6e  . So, you can on
+00000e80: 6c79 2068 6f70 6520 7468 6174 0a20 2066  ly hope that.  f
+00000e90: 696e 616c 2065 6d62 6564 6469 6e67 7320  inal embeddings 
+00000ea0: 7769 6c6c 2068 6176 6520 7468 6520 6465  will have the de
+00000eb0: 7369 7265 6420 7072 6f70 6572 7469 6573  sired properties
+00000ec0: 2e0a 0a2a 202a 2a54 6865 2073 6563 6f6e  ...* **The secon
+00000ed0: 6420 7072 6f62 6c65 6d20 6973 2074 6865  d problem is the
+00000ee0: 2076 616c 6964 6174 696f 6e20 7072 6f63   validation proc
+00000ef0: 6573 732a 2a2e 0a20 2049 6e20 7468 6520  ess**..  In the 
+00000f00: 7365 6172 6368 696e 6720 7365 7475 702c  searching setup,
+00000f10: 2079 6f75 2075 7375 616c 6c79 2063 6172   you usually car
+00000f20: 6520 686f 7720 7265 6c61 7465 6420 796f  e how related yo
+00000f30: 7572 2074 6f70 2d4e 206f 7574 7075 7473  ur top-N outputs
+00000f40: 2061 7265 2074 6f20 7468 6520 7175 6572   are to the quer
+00000f50: 792e 0a20 2054 6865 206e 6174 7572 616c  y..  The natural
+00000f60: 2077 6179 2074 6f20 6576 616c 7561 7465   way to evaluate
+00000f70: 2074 6865 206d 6f64 656c 2069 7320 746f   the model is to
+00000f80: 2073 696d 756c 6174 6520 7365 6172 6368   simulate search
+00000f90: 696e 6720 7265 7175 6573 7473 2074 6f20  ing requests to 
+00000fa0: 7468 6520 7265 6665 7265 6e63 6520 7365  the reference se
+00000fb0: 740a 2020 616e 6420 6170 706c 7920 6f6e  t.  and apply on
+00000fc0: 6520 6f66 2074 6865 2072 6574 7269 6576  e of the retriev
+00000fd0: 616c 206d 6574 7269 6373 2e0a 2020 536f  al metrics..  So
+00000fe0: 2c20 7468 6572 6520 6973 206e 6f20 6775  , there is no gu
+00000ff0: 6172 616e 7465 6520 7468 6174 2063 6c61  arantee that cla
+00001000: 7373 6966 6963 6174 696f 6e20 6163 6375  ssification accu
+00001010: 7261 6379 2077 696c 6c20 636f 7272 656c  racy will correl
+00001020: 6174 6520 7769 7468 2074 6865 7365 206d  ate with these m
+00001030: 6574 7269 6373 2e0a 0a2a 2046 696e 616c  etrics...* Final
+00001040: 6c79 2c20 796f 7520 6d61 7920 7761 6e74  ly, you may want
+00001050: 2074 6f20 696d 706c 656d 656e 7420 6120   to implement a 
+00001060: 6d65 7472 6963 206c 6561 726e 696e 6720  metric learning 
+00001070: 7069 7065 6c69 6e65 2062 7920 796f 7572  pipeline by your
+00001080: 7365 6c66 2e0a 2020 2a2a 5468 6572 6520  self..  **There 
+00001090: 6973 2061 206c 6f74 206f 6620 776f 726b  is a lot of work
+000010a0: 2a2a 3a20 746f 2075 7365 2074 7269 706c  **: to use tripl
+000010b0: 6574 206c 6f73 7320 796f 7520 6e65 6564  et loss you need
+000010c0: 2074 6f20 666f 726d 2062 6174 6368 6573   to form batches
+000010d0: 2069 6e20 6120 7370 6563 6966 6963 2077   in a specific w
+000010e0: 6179 2c0a 2020 696d 706c 656d 656e 7420  ay,.  implement 
+000010f0: 6469 6666 6572 656e 7420 6b69 6e64 7320  different kinds 
+00001100: 6f66 2074 7269 706c 6574 7320 6d69 6e69  of triplets mini
+00001110: 6e67 2c20 7472 6163 6b69 6e67 2064 6973  ng, tracking dis
+00001120: 7461 6e63 6573 2c20 6574 632e 2046 6f72  tances, etc. For
+00001130: 2074 6865 2076 616c 6964 6174 696f 6e2c   the validation,
+00001140: 2079 6f75 2061 6c73 6f20 6e65 6564 2074   you also need t
+00001150: 6f0a 2020 696d 706c 656d 656e 7420 7265  o.  implement re
+00001160: 7472 6965 7661 6c20 6d65 7472 6963 732c  trieval metrics,
+00001170: 0a20 2077 6869 6368 2069 6e63 6c75 6465  .  which include
+00001180: 2065 6666 6563 7469 7665 2065 6d62 6564   effective embed
+00001190: 6469 6e67 7320 6163 6375 6d75 6c61 7469  dings accumulati
+000011a0: 6f6e 2064 7572 696e 6720 7468 6520 6570  on during the ep
+000011b0: 6f63 682c 2063 6f76 6572 696e 6720 636f  och, covering co
+000011c0: 726e 6572 2063 6173 6573 2c20 6574 632e  rner cases, etc.
+000011d0: 0a20 2049 7427 7320 6576 656e 2068 6172  .  It's even har
+000011e0: 6465 7220 6966 2079 6f75 2068 6176 6520  der if you have 
+000011f0: 7365 7665 7261 6c20 6770 7573 2061 6e64  several gpus and
+00001200: 2075 7365 2044 4450 2e0a 2020 596f 7520   use DDP..  You 
+00001210: 6d61 7920 616c 736f 2077 616e 7420 746f  may also want to
+00001220: 2076 6973 7561 6c69 7a65 2079 6f75 7220   visualize your 
+00001230: 7365 6172 6368 2072 6571 7565 7374 7320  search requests 
+00001240: 6279 2068 6967 686c 6967 6874 696e 6720  by highlighting 
+00001250: 676f 6f64 2061 6e64 2062 6164 2073 6561  good and bad sea
+00001260: 7263 6820 7265 7375 6c74 732e 0a20 2049  rch results..  I
+00001270: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
+00001280: 6974 2062 7920 796f 7572 7365 6c66 2c20  it by yourself, 
+00001290: 796f 7520 6361 6e20 7369 6d70 6c79 2075  you can simply u
+000012a0: 7365 204f 4d4c 2066 6f72 2079 6f75 7220  se OML for your 
+000012b0: 7075 7270 6f73 6573 2e0a 0a3c 2f70 3e0a  purposes...</p>.
+000012c0: 3c2f 6465 7461 696c 733e 0a0a 0a3c 6465  </details>...<de
+000012d0: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+000012e0: 5768 6174 2069 7320 7468 6520 6469 6666  What is the diff
+000012f0: 6572 656e 6365 2062 6574 7765 656e 204f  erence between O
+00001300: 7065 6e20 4d65 7472 6963 204c 6561 726e  pen Metric Learn
+00001310: 696e 6720 616e 6420 5079 546f 7263 6820  ing and PyTorch 
+00001320: 4d65 7472 6963 204c 6561 726e 696e 673f  Metric Learning?
+00001330: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+00001340: 5b50 4d4c 5d28 6874 7470 733a 2f2f 6769  [PML](https://gi
+00001350: 7468 7562 2e63 6f6d 2f4b 6576 696e 4d75  thub.com/KevinMu
+00001360: 7367 7261 7665 2f70 7974 6f72 6368 2d6d  sgrave/pytorch-m
+00001370: 6574 7269 632d 6c65 6172 6e69 6e67 2920  etric-learning) 
+00001380: 6973 2074 6865 2070 6f70 756c 6172 206c  is the popular l
+00001390: 6962 7261 7279 2066 6f72 204d 6574 7269  ibrary for Metri
+000013a0: 6320 4c65 6172 6e69 6e67 2c0a 616e 6420  c Learning,.and 
+000013b0: 6974 2069 6e63 6c75 6465 7320 6120 7269  it includes a ri
+000013c0: 6368 2063 6f6c 6c65 6374 696f 6e20 6f66  ch collection of
+000013d0: 206c 6f73 7365 732c 206d 696e 6572 732c   losses, miners,
+000013e0: 2064 6973 7461 6e63 6573 2c20 616e 6420   distances, and 
+000013f0: 7265 6475 6365 7273 3b20 7468 6174 2069  reducers; that i
+00001400: 7320 7768 7920 7765 2070 726f 7669 6465  s why we provide
+00001410: 2073 7472 6169 6768 7466 6f72 7761 7264   straightforward
+00001420: 0a5b 6578 616d 706c 6573 5d28 6874 7470  .[examples](http
+00001430: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+00001440: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+00001450: 7269 632d 6c65 6172 6e69 6e67 2375 7361  ric-learning#usa
+00001460: 6765 2d77 6974 682d 7079 746f 7263 682d  ge-with-pytorch-
+00001470: 6d65 7472 6963 2d6c 6561 726e 696e 6729  metric-learning)
+00001480: 206f 6620 7573 696e 6720 7468 656d 2077   of using them w
+00001490: 6974 6820 4f4d 4c2e 0a49 6e69 7469 616c  ith OML..Initial
+000014a0: 6c79 2c20 7765 2074 7269 6564 2074 6f20  ly, we tried to 
+000014b0: 7573 6520 504d 4c2c 2062 7574 2069 6e20  use PML, but in 
+000014c0: 7468 6520 656e 642c 2077 6520 6361 6d65  the end, we came
+000014d0: 2075 7020 7769 7468 206f 7572 206c 6962   up with our lib
+000014e0: 7261 7279 2c20 7768 6963 6820 6973 206d  rary, which is m
+000014f0: 6f72 6520 7069 7065 6c69 6e65 202f 2072  ore pipeline / r
+00001500: 6563 6970 6573 206f 7269 656e 7465 642e  ecipes oriented.
+00001510: 0a54 6861 7420 6973 2068 6f77 204f 4d4c  .That is how OML
+00001520: 2064 6966 6665 7273 2066 726f 6d20 504d   differs from PM
+00001530: 4c3a 0a0a 2a20 4f4d 4c20 6861 7320 5b50  L:..* OML has [P
+00001540: 6970 656c 696e 6573 5d28 6874 7470 733a  ipelines](https:
+00001550: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00001560: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00001570: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+00001580: 6d61 696e 2f70 6970 656c 696e 6573 290a  main/pipelines).
+00001590: 2020 7768 6963 6820 616c 6c6f 7773 2074    which allows t
+000015a0: 7261 696e 696e 6720 6d6f 6465 6c73 2062  raining models b
+000015b0: 7920 7072 6570 6172 696e 6720 6120 636f  y preparing a co
+000015c0: 6e66 6967 2061 6e64 2079 6f75 7220 6461  nfig and your da
+000015d0: 7461 2069 6e20 7468 6520 7265 7175 6972  ta in the requir
+000015e0: 6564 2066 6f72 6d61 740a 2020 2869 7427  ed format.  (it'
+000015f0: 7320 6c69 6b65 2063 6f6e 7665 7274 696e  s like convertin
+00001600: 6720 6461 7461 2069 6e74 6f20 434f 434f  g data into COCO
+00001610: 2066 6f72 6d61 7420 746f 2074 7261 696e   format to train
+00001620: 2061 2064 6574 6563 746f 7220 6672 6f6d   a detector from
+00001630: 205b 6d6d 6465 7465 6374 696f 6e5d 2868   [mmdetection](h
+00001640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001650: 6d2f 6f70 656e 2d6d 6d6c 6162 2f6d 6d64  m/open-mmlab/mmd
+00001660: 6574 6563 7469 6f6e 2929 2e0a 0a2a 204f  etection))...* O
+00001670: 4d4c 2066 6f63 7573 6573 206f 6e20 656e  ML focuses on en
+00001680: 642d 746f 2d65 6e64 2070 6970 656c 696e  d-to-end pipelin
+00001690: 6573 2061 6e64 2070 7261 6374 6963 616c  es and practical
+000016a0: 2075 7365 2063 6173 6573 2e0a 2020 4974   use cases..  It
+000016b0: 2068 6173 2063 6f6e 6669 6720 6261 7365   has config base
+000016c0: 6420 6578 616d 706c 6573 206f 6e20 706f  d examples on po
+000016d0: 7075 6c61 7220 6265 6e63 686d 6172 6b73  pular benchmarks
+000016e0: 2063 6c6f 7365 2074 6f20 7265 616c 206c   close to real l
+000016f0: 6966 6520 286c 696b 6520 7068 6f74 6f73  ife (like photos
+00001700: 206f 6620 7072 6f64 7563 7473 206f 6620   of products of 
+00001710: 7468 6f75 7361 6e64 7320 6964 7329 2e0a  thousands ids)..
+00001720: 2020 5765 2066 6f75 6e64 2073 6f6d 6520    We found some 
+00001730: 676f 6f64 2063 6f6d 6269 6e61 7469 6f6e  good combination
+00001740: 7320 6f66 2068 7970 6572 7061 7261 6d65  s of hyperparame
+00001750: 7465 7273 206f 6e20 7468 6573 6520 6461  ters on these da
+00001760: 7461 7365 7473 2c20 7472 6169 6e65 6420  tasets, trained 
+00001770: 616e 6420 7075 626c 6973 6865 6420 6d6f  and published mo
+00001780: 6465 6c73 2061 6e64 2074 6865 6972 2063  dels and their c
+00001790: 6f6e 6669 6773 2e0a 2020 5468 7573 2c20  onfigs..  Thus, 
+000017a0: 6974 206d 616b 6573 204f 4d4c 206d 6f72  it makes OML mor
+000017b0: 6520 7265 6369 7065 7320 6f72 6965 6e74  e recipes orient
+000017c0: 6564 2074 6861 6e20 504d 4c2c 2061 6e64  ed than PML, and
+000017d0: 2069 7473 2061 7574 686f 720a 2020 5b63   its author.  [c
+000017e0: 6f6e 6669 726d 735d 2868 7474 7073 3a2f  onfirms](https:/
+000017f0: 2f67 6974 6875 622e 636f 6d2f 4b65 7669  /github.com/Kevi
+00001800: 6e4d 7573 6772 6176 652f 7079 746f 7263  nMusgrave/pytorc
+00001810: 682d 6d65 7472 6963 2d6c 6561 726e 696e  h-metric-learnin
+00001820: 672f 6973 7375 6573 2f31 3639 2369 7373  g/issues/169#iss
+00001830: 7565 636f 6d6d 656e 742d 3637 3038 3134  uecomment-670814
+00001840: 3339 3329 0a20 2074 6869 7320 7361 7969  393).  this sayi
+00001850: 6e67 2074 6861 7420 6869 7320 6c69 6272  ng that his libr
+00001860: 6172 7920 6973 2061 2073 6574 206f 6620  ary is a set of 
+00001870: 746f 6f6c 7320 7261 7468 6572 2074 6865  tools rather the
+00001880: 2072 6563 6970 6573 2c20 6d6f 7265 6f76   recipes, moreov
+00001890: 6572 2c20 7468 6520 6578 616d 706c 6573  er, the examples
+000018a0: 2069 6e20 504d 4c20 6172 6520 6d6f 7374   in PML are most
+000018b0: 6c79 2066 6f72 2043 4946 4152 2061 6e64  ly for CIFAR and
+000018c0: 204d 4e49 5354 2064 6174 6173 6574 732e   MNIST datasets.
+000018d0: 0a0a 2a20 4f4d 4c20 6861 7320 7468 6520  ..* OML has the 
+000018e0: 5b5a 6f6f 5d28 6874 7470 733a 2f2f 6769  [Zoo](https://gi
+000018f0: 7468 7562 2e63 6f6d 2f4f 4d4c 2d54 6561  thub.com/OML-Tea
+00001900: 6d2f 6f70 656e 2d6d 6574 7269 632d 6c65  m/open-metric-le
+00001910: 6172 6e69 6e67 237a 6f6f 2920 6f66 2070  arning#zoo) of p
+00001920: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
+00001930: 2074 6861 7420 6361 6e20 6265 2065 6173   that can be eas
+00001940: 696c 7920 6163 6365 7373 6564 2066 726f  ily accessed fro
+00001950: 6d0a 2020 7468 6520 636f 6465 2069 6e20  m.  the code in 
+00001960: 7468 6520 7361 6d65 2077 6179 2061 7320  the same way as 
+00001970: 696e 2060 746f 7263 6876 6973 696f 6e60  in `torchvision`
+00001980: 2028 7768 656e 2079 6f75 2074 7970 6520   (when you type 
+00001990: 6072 6573 6e65 7435 3028 7072 6574 7261  `resnet50(pretra
+000019a0: 696e 6564 3d54 7275 6529 6029 2e0a 0a2a  ined=True)`)...*
+000019b0: 204f 4d4c 2069 7320 696e 7465 6772 6174   OML is integrat
+000019c0: 6564 2077 6974 6820 5b50 7954 6f72 6368  ed with [PyTorch
+000019d0: 204c 6967 6874 6e69 6e67 5d28 6874 7470   Lightning](http
+000019e0: 733a 2f2f 7777 772e 7079 746f 7263 686c  s://www.pytorchl
+000019f0: 6967 6874 6e69 6e67 2e61 692f 292c 2073  ightning.ai/), s
+00001a00: 6f2c 2077 6520 6361 6e20 7573 6520 7468  o, we can use th
+00001a10: 6520 706f 7765 7220 6f66 2069 7473 0a20  e power of its. 
+00001a20: 205b 5472 6169 6e65 725d 2868 7474 7073   [Trainer](https
+00001a30: 3a2f 2f70 7974 6f72 6368 2d6c 6967 6874  ://pytorch-light
+00001a40: 6e69 6e67 2e72 6561 6474 6865 646f 6373  ning.readthedocs
+00001a50: 2e69 6f2f 656e 2f73 7461 626c 652f 636f  .io/en/stable/co
+00001a60: 6d6d 6f6e 2f74 7261 696e 6572 2e68 746d  mmon/trainer.htm
+00001a70: 6c29 2e0a 2020 5468 6973 2069 7320 6573  l)..  This is es
+00001a80: 7065 6369 616c 6c79 2068 656c 7066 756c  pecially helpful
+00001a90: 2077 6865 6e20 7765 2077 6f72 6b20 7769   when we work wi
+00001aa0: 7468 2044 4450 2c20 736f 2c20 796f 7520  th DDP, so, you 
+00001ab0: 636f 6d70 6172 6520 6f75 720a 2020 5b44  compare our.  [D
+00001ac0: 4450 2065 7861 6d70 6c65 5d28 6874 7470  DP example](http
+00001ad0: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00001ae0: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00001af0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00001b00: 742f 6578 616d 706c 6573 2f70 7974 686f  t/examples/pytho
+00001b10: 6e2e 6874 6d6c 290a 2020 616e 6420 7468  n.html).  and th
+00001b20: 650a 2020 5b50 4d4c 7320 6f6e 655d 2868  e.  [PMLs one](h
+00001b30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001b40: 6d2f 4b65 7669 6e4d 7573 6772 6176 652f  m/KevinMusgrave/
+00001b50: 7079 746f 7263 682d 6d65 7472 6963 2d6c  pytorch-metric-l
+00001b60: 6561 726e 696e 672f 626c 6f62 2f6d 6173  earning/blob/mas
+00001b70: 7465 722f 6578 616d 706c 6573 2f6e 6f74  ter/examples/not
+00001b80: 6562 6f6f 6b73 2f44 6973 7472 6962 7574  ebooks/Distribut
+00001b90: 6564 5472 6970 6c65 744d 6172 6769 6e4c  edTripletMarginL
+00001ba0: 6f73 734d 4e49 5354 2e69 7079 6e62 292e  ossMNIST.ipynb).
+00001bb0: 0a20 2042 7920 7468 6520 7761 792c 2050  .  By the way, P
+00001bc0: 4d4c 2061 6c73 6f20 6861 7320 5b54 7261  ML also has [Tra
+00001bd0: 696e 6572 735d 2868 7474 7073 3a2f 2f6b  iners](https://k
+00001be0: 6576 696e 6d75 7367 7261 7665 2e67 6974  evinmusgrave.git
+00001bf0: 6875 622e 696f 2f70 7974 6f72 6368 2d6d  hub.io/pytorch-m
+00001c00: 6574 7269 632d 6c65 6172 6e69 6e67 2f74  etric-learning/t
+00001c10: 7261 696e 6572 732f 292c 2062 7574 2069  rainers/), but i
+00001c20: 7427 7320 6e6f 740a 2020 7769 6465 6c79  t's not.  widely
+00001c30: 2075 7365 6420 696e 2074 6865 2065 7861   used in the exa
+00001c40: 6d70 6c65 7320 616e 6420 6375 7374 6f6d  mples and custom
+00001c50: 2060 7472 6169 6e60 202f 2060 7465 7374   `train` / `test
+00001c60: 6020 6675 6e63 7469 6f6e 7320 6172 6520  ` functions are 
+00001c70: 7573 6564 2069 6e73 7465 6164 2e0a 0a57  used instead...W
+00001c80: 6520 6265 6c69 6576 6520 7468 6174 2068  e believe that h
+00001c90: 6176 696e 6720 5069 7065 6c69 6e65 732c  aving Pipelines,
+00001ca0: 206c 6163 6f6e 6963 2065 7861 6d70 6c65   laconic example
+00001cb0: 732c 2061 6e64 205a 6f6f 206f 6620 7072  s, and Zoo of pr
+00001cc0: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
+00001cd0: 7365 7473 2074 6865 2065 6e74 7279 2074  sets the entry t
+00001ce0: 6872 6573 686f 6c64 2074 6f20 6120 7265  hreshold to a re
+00001cf0: 616c 6c79 206c 6f77 2076 616c 7565 2e0a  ally low value..
+00001d00: 0a3c 2f70 3e0a 3c2f 6465 7461 696c 733e  .</p>.</details>
+00001d10: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
+00001d20: 6d6d 6172 793e 5768 6174 2069 7320 4d65  mmary>What is Me
+00001d30: 7472 6963 204c 6561 726e 696e 673f 3c2f  tric Learning?</
+00001d40: 7375 6d6d 6172 793e 0a3c 703e 0a0a 4d65  summary>.<p>..Me
+00001d50: 7472 6963 204c 6561 726e 696e 6720 7072  tric Learning pr
+00001d60: 6f62 6c65 6d20 2861 6c73 6f20 6b6e 6f77  oblem (also know
+00001d70: 6e20 6173 202a 6578 7472 656d 6520 636c  n as *extreme cl
+00001d80: 6173 7369 6669 6361 7469 6f6e 2a20 7072  assification* pr
+00001d90: 6f62 6c65 6d29 206d 6561 6e73 2061 2073  oblem) means a s
+00001da0: 6974 7561 7469 6f6e 2069 6e20 7768 6963  ituation in whic
+00001db0: 6820 7765 0a68 6176 6520 7468 6f75 7361  h we.have thousa
+00001dc0: 6e64 7320 6f66 2069 6473 206f 6620 736f  nds of ids of so
+00001dd0: 6d65 2065 6e74 6974 6965 732c 2062 7574  me entities, but
+00001de0: 206f 6e6c 7920 6120 6665 7720 7361 6d70   only a few samp
+00001df0: 6c65 7320 666f 7220 6576 6572 7920 656e  les for every en
+00001e00: 7469 7479 2e0a 4f66 7465 6e20 7765 2061  tity..Often we a
+00001e10: 7373 756d 6520 7468 6174 2064 7572 696e  ssume that durin
+00001e20: 6720 7468 6520 7465 7374 2073 7461 6765  g the test stage
+00001e30: 2028 6f72 2070 726f 6475 6374 696f 6e29   (or production)
+00001e40: 2077 6520 7769 6c6c 2064 6561 6c20 7769   we will deal wi
+00001e50: 7468 2075 6e73 6565 6e20 656e 7469 7469  th unseen entiti
+00001e60: 6573 0a77 6869 6368 206d 616b 6573 2069  es.which makes i
+00001e70: 7420 696d 706f 7373 6962 6c65 2074 6f20  t impossible to 
+00001e80: 6170 706c 7920 7468 6520 7661 6e69 6c6c  apply the vanill
+00001e90: 6120 636c 6173 7369 6669 6361 7469 6f6e  a classification
+00001ea0: 2070 6970 656c 696e 6520 6469 7265 6374   pipeline direct
+00001eb0: 6c79 2e20 496e 206d 616e 7920 6361 7365  ly. In many case
+00001ec0: 7320 6f62 7461 696e 6564 2065 6d62 6564  s obtained embed
+00001ed0: 6469 6e67 730a 6172 6520 7573 6564 2074  dings.are used t
+00001ee0: 6f20 7065 7266 6f72 6d20 7365 6172 6368  o perform search
+00001ef0: 206f 7220 6d61 7463 6869 6e67 2070 726f   or matching pro
+00001f00: 6365 6475 7265 7320 6f76 6572 2074 6865  cedures over the
+00001f10: 6d2e 0a0a 4865 7265 2061 7265 2061 2066  m...Here are a f
+00001f20: 6577 2065 7861 6d70 6c65 7320 6f66 2073  ew examples of s
+00001f30: 7563 6820 7461 736b 7320 6672 6f6d 2074  uch tasks from t
+00001f40: 6865 2063 6f6d 7075 7465 7220 7669 7369  he computer visi
+00001f50: 6f6e 2073 7068 6572 653a 0a2a 2050 6572  on sphere:.* Per
+00001f60: 736f 6e2f 416e 696d 616c 2052 652d 4964  son/Animal Re-Id
+00001f70: 656e 7469 6669 6361 7469 6f6e 0a2a 2046  entification.* F
+00001f80: 6163 6520 5265 636f 676e 6974 696f 6e0a  ace Recognition.
+00001f90: 2a20 4c61 6e64 6d61 726b 2052 6563 6f67  * Landmark Recog
+00001fa0: 6e69 7469 6f6e 0a2a 2053 6561 7263 6869  nition.* Searchi
+00001fb0: 6e67 2065 6e67 696e 6573 2066 6f72 206f  ng engines for o
+00001fc0: 6e6c 696e 6520 7368 6f70 730a 2061 6e64  nline shops. and
+00001fd0: 206d 616e 7920 6f74 6865 7273 2e0a 3c2f   many others..</
+00001fe0: 703e 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  p>.</details>...
+00001ff0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+00002000: 7279 3e47 6c6f 7373 6172 7920 284e 616d  ry>Glossary (Nam
+00002010: 696e 6720 636f 6e76 656e 7469 6f6e 2920  ing convention) 
+00002020: 3c2f 7375 6d6d 6172 793e 0a3c 703e 0a0a  </summary>.<p>..
+00002030: 2a20 6065 6d62 6564 6469 6e67 6020 2d20  * `embedding` - 
+00002040: 6d6f 6465 6c27 7320 6f75 7470 7574 2028  model's output (
+00002050: 616c 736f 206b 6e6f 776e 2061 7320 6066  also known as `f
+00002060: 6561 7475 7265 7320 7665 6374 6f72 6020  eatures vector` 
+00002070: 6f72 2060 6465 7363 7269 7074 6f72 6029  or `descriptor`)
+00002080: 2e0a 2a20 6071 7565 7279 6020 2d20 6120  ..* `query` - a 
+00002090: 7361 6d70 6c65 2077 6869 6368 2069 7320  sample which is 
+000020a0: 7573 6564 2061 7320 6120 7265 7175 6573  used as a reques
+000020b0: 7420 696e 2074 6865 2072 6574 7269 6576  t in the retriev
+000020c0: 616c 2070 726f 6365 6475 7265 2e0a 2a20  al procedure..* 
+000020d0: 6067 616c 6c65 7279 2073 6574 6020 2d20  `gallery set` - 
+000020e0: 7468 6520 7365 7420 6f66 2065 6e74 6974  the set of entit
+000020f0: 6965 7320 746f 2073 6561 7263 6820 6974  ies to search it
+00002100: 656d 7320 7369 6d69 6c61 7220 746f 2060  ems similar to `
+00002110: 7175 6572 7960 2028 616c 736f 206b 6e6f  query` (also kno
+00002120: 776e 2061 7320 6072 6566 6572 656e 6365  wn as `reference
+00002130: 6020 6f72 2060 696e 6465 7860 292e 0a2a  ` or `index`)..*
+00002140: 2060 5361 6d70 6c65 7260 202d 2061 6e20   `Sampler` - an 
+00002150: 6172 6775 6d65 6e74 2066 6f72 2060 4461  argument for `Da
+00002160: 7461 4c6f 6164 6572 6020 7768 6963 6820  taLoader` which 
+00002170: 6973 2075 7365 6420 746f 2066 6f72 6d20  is used to form 
+00002180: 6261 7463 6865 730a 2a20 604d 696e 6572  batches.* `Miner
+00002190: 6020 2d20 7468 6520 6f62 6a65 6374 2074  ` - the object t
+000021a0: 6f20 666f 726d 2070 6169 7273 206f 7220  o form pairs or 
+000021b0: 7472 6970 6c65 7473 2061 6674 6572 2074  triplets after t
+000021c0: 6865 2062 6174 6368 2077 6173 2066 6f72  he batch was for
+000021d0: 6d65 6420 6279 2060 5361 6d70 6c65 7260  med by `Sampler`
+000021e0: 2e20 4974 2773 206e 6f74 206e 6563 6573  . It's not neces
+000021f0: 7361 7279 2074 6f20 666f 726d 0a20 2074  sary to form.  t
+00002200: 6865 2063 6f6d 6269 6e61 7469 6f6e 7320  he combinations 
+00002210: 6f66 2073 616d 706c 6573 206f 6e6c 7920  of samples only 
+00002220: 696e 7369 6465 2074 6865 2063 7572 7265  inside the curre
+00002230: 6e74 2062 6174 6368 2c20 7468 7573 2c20  nt batch, thus, 
+00002240: 7468 6520 6d65 6d6f 7279 2062 616e 6b20  the memory bank 
+00002250: 6d61 7920 6265 2061 2070 6172 7420 6f66  may be a part of
+00002260: 2060 4d69 6e65 7260 2e0a 2a20 6053 616d   `Miner`..* `Sam
+00002270: 706c 6573 602f 604c 6162 656c 7360 2f60  ples`/`Labels`/`
+00002280: 496e 7374 616e 6365 7360 202d 2061 7320  Instances` - as 
+00002290: 616e 2065 7861 6d70 6c65 206c 6574 2773  an example let's
+000022a0: 2063 6f6e 7369 6465 7220 4465 6570 4661   consider DeepFa
+000022b0: 7368 696f 6e20 6461 7461 7365 742e 2049  shion dataset. I
+000022c0: 7420 696e 636c 7564 6573 2074 686f 7573  t includes thous
+000022d0: 616e 6473 206f 660a 2020 6661 7368 696f  ands of.  fashio
+000022e0: 6e20 6974 656d 2069 6473 2028 7765 206e  n item ids (we n
+000022f0: 616d 6520 7468 656d 2060 6c61 6265 6c73  ame them `labels
+00002300: 6029 2061 6e64 2073 6576 6572 616c 2070  `) and several p
+00002310: 686f 746f 7320 666f 7220 6561 6368 2069  hotos for each i
+00002320: 7465 6d20 6964 0a20 2028 7765 206e 616d  tem id.  (we nam
+00002330: 6520 7468 6520 696e 6469 7669 6475 616c  e the individual
+00002340: 2070 686f 746f 2061 7320 6069 6e73 7461   photo as `insta
+00002350: 6e63 6560 206f 7220 6073 616d 706c 6560  nce` or `sample`
+00002360: 292e 2041 6c6c 206f 6620 7468 6520 6661  ). All of the fa
+00002370: 7368 696f 6e20 6974 656d 2069 6473 2068  shion item ids h
+00002380: 6176 6520 7468 6569 7220 6772 6f75 7073  ave their groups
+00002390: 206c 696b 650a 2020 2273 6b69 7274 7322   like.  "skirts"
+000023a0: 2c20 226a 6163 6b65 7473 222c 2022 7368  , "jackets", "sh
+000023b0: 6f72 7473 2220 616e 6420 736f 206f 6e20  orts" and so on 
+000023c0: 2877 6520 6e61 6d65 2074 6865 6d20 6063  (we name them `c
+000023d0: 6174 6567 6f72 6965 7360 292e 0a20 204e  ategories`)..  N
+000023e0: 6f74 652c 2077 6520 6176 6f69 6420 7573  ote, we avoid us
+000023f0: 696e 6720 7468 6520 7465 726d 2060 636c  ing the term `cl
+00002400: 6173 7360 2074 6f20 6176 6f69 6420 6d69  ass` to avoid mi
+00002410: 7375 6e64 6572 7374 616e 6469 6e67 2e0a  sunderstanding..
+00002420: 2a20 6074 7261 696e 696e 6720 6570 6f63  * `training epoc
+00002430: 6860 202d 2062 6174 6368 2073 616d 706c  h` - batch sampl
+00002440: 6572 7320 7768 6963 6820 7765 2075 7365  ers which we use
+00002450: 2066 6f72 2063 6f6d 6269 6e61 7469 6f6e   for combination
+00002460: 2d62 6173 6564 206c 6f73 7365 7320 7573  -based losses us
+00002470: 7561 6c6c 7920 6861 7665 2061 206c 656e  ually have a len
+00002480: 6774 6820 6571 7561 6c20 746f 0a20 2060  gth equal to.  `
+00002490: 5b6e 756d 6265 7220 6f66 206c 6162 656c  [number of label
+000024a0: 7320 696e 2074 7261 696e 696e 6720 6461  s in training da
+000024b0: 7461 7365 745d 202f 205b 6e75 6d62 6572  taset] / [number
+000024c0: 7320 6f66 206c 6162 656c 7320 696e 206f  s of labels in o
+000024d0: 6e65 2062 6174 6368 5d60 2e20 4974 206d  ne batch]`. It m
+000024e0: 6561 6e73 2074 6861 7420 7765 2064 6f6e  eans that we don
+000024f0: 2774 206f 6273 6572 7665 2061 6c6c 206f  't observe all o
+00002500: 660a 2020 7468 6520 6176 6169 6c61 626c  f.  the availabl
+00002510: 6520 7472 6169 6e69 6e67 2073 616d 706c  e training sampl
+00002520: 6573 2069 6e20 6f6e 6520 6570 6f63 6820  es in one epoch 
+00002530: 2861 7320 6f70 706f 7365 6420 746f 2076  (as opposed to v
+00002540: 616e 696c 6c61 2063 6c61 7373 6966 6963  anilla classific
+00002550: 6174 696f 6e29 2c0a 2020 696e 7374 6561  ation),.  instea
+00002560: 642c 2077 6520 6f62 7365 7276 6520 616c  d, we observe al
+00002570: 6c20 6f66 2074 6865 2061 7661 696c 6162  l of the availab
+00002580: 6c65 206c 6162 656c 732e 0a0a 3c2f 703e  le labels...</p>
+00002590: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 3c64  .</details>...<d
+000025a0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+000025b0: 3e48 6f77 2067 6f6f 6420 6d61 7920 6265  >How good may be
+000025c0: 2061 206d 6f64 656c 2074 7261 696e 6564   a model trained
+000025d0: 2077 6974 6820 4f4d 4c3f 203c 2f73 756d   with OML? </sum
+000025e0: 6d61 7279 3e0a 3c70 3e0a 0a49 7420 6d61  mary>.<p>..It ma
+000025f0: 7920 6265 2063 6f6d 7061 7261 626c 6520  y be comparable 
+00002600: 7769 7468 2074 6865 2063 7572 7265 6e74  with the current
+00002610: 2028 3230 3232 2079 6561 7229 205b 536f   (2022 year) [So
+00002620: 7441 5d28 6874 7470 733a 2f2f 7061 7065  tA](https://pape
+00002630: 7273 7769 7468 636f 6465 2e63 6f6d 2f74  rswithcode.com/t
+00002640: 6173 6b2f 6d65 7472 6963 2d6c 6561 726e  ask/metric-learn
+00002650: 696e 6729 206d 6574 686f 6473 2c0a 666f  ing) methods,.fo
+00002660: 7220 6578 616d 706c 652c 205b 4879 702d  r example, [Hyp-
+00002670: 5669 545d 2868 7474 7073 3a2f 2f61 7278  ViT](https://arx
+00002680: 6976 2e6f 7267 2f70 6466 2f32 3230 332e  iv.org/pdf/2203.
+00002690: 3130 3833 332e 7064 6629 2e0a 2a28 4665  10833.pdf)..*(Fe
+000026a0: 7720 776f 7264 7320 6162 6f75 7420 7468  w words about th
+000026b0: 6973 2061 7070 726f 6163 683a 2069 7427  is approach: it'
+000026c0: 7320 6120 5669 5420 6172 6368 6974 6563  s a ViT architec
+000026d0: 7475 7265 2074 7261 696e 6564 2077 6974  ture trained wit
+000026e0: 6820 636f 6e74 7261 7374 6976 6520 6c6f  h contrastive lo
+000026f0: 7373 2c0a 6275 7420 7468 6520 656d 6265  ss,.but the embe
+00002700: 6464 696e 6773 2077 6572 6520 7072 6f6a  ddings were proj
+00002710: 6563 7465 6420 696e 746f 2073 6f6d 6520  ected into some 
+00002720: 6879 7065 7262 6f6c 6963 2073 7061 6365  hyperbolic space
+00002730: 2e0a 4173 2074 6865 2061 7574 686f 7273  ..As the authors
+00002740: 2063 6c61 696d 6564 2c20 7375 6368 2061   claimed, such a
+00002750: 2073 7061 6365 2069 7320 6162 6c65 2074   space is able t
+00002760: 6f20 6465 7363 7269 6265 2074 6865 206e  o describe the n
+00002770: 6573 7465 6420 7374 7275 6374 7572 6520  ested structure 
+00002780: 6f66 2072 6561 6c2d 776f 726c 6420 6461  of real-world da
+00002790: 7461 2e0a 536f 2c20 7468 6520 7061 7065  ta..So, the pape
+000027a0: 7220 7265 7175 6972 6573 2073 6f6d 6520  r requires some 
+000027b0: 6865 6176 7920 6d61 7468 2074 6f20 6164  heavy math to ad
+000027c0: 6170 7420 7468 6520 7573 7561 6c20 6f70  apt the usual op
+000027d0: 6572 6174 696f 6e73 2066 6f72 2074 6865  erations for the
+000027e0: 2068 7970 6572 626f 6c69 6361 6c20 7370   hyperbolical sp
+000027f0: 6163 652e 292a 0a0a 5765 2074 7261 696e  ace.)*..We train
+00002800: 6564 2074 6865 2073 616d 6520 6172 6368  ed the same arch
+00002810: 6974 6563 7475 7265 2077 6974 6820 7472  itecture with tr
+00002820: 6970 6c65 7420 6c6f 7373 2c20 6669 7869  iplet loss, fixi
+00002830: 6e67 2074 6865 2072 6573 7420 6f66 2074  ng the rest of t
+00002840: 6865 2070 6172 616d 6574 6572 733a 0a74  he parameters:.t
+00002850: 7261 696e 696e 6720 616e 6420 7465 7374  raining and test
+00002860: 2074 7261 6e73 666f 726d 6174 696f 6e73   transformations
+00002870: 2c20 696d 6167 6520 7369 7a65 2c20 616e  , image size, an
+00002880: 6420 6f70 7469 6d69 7a65 722e 2053 6565  d optimizer. See
+00002890: 2063 6f6e 6669 6773 2069 6e20 5b4d 6f64   configs in [Mod
+000028a0: 656c 7320 5a6f 6f5d 2868 7474 7073 3a2f  els Zoo](https:/
+000028b0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+000028c0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+000028d0: 2d6c 6561 726e 696e 6723 7a6f 6f29 2e0a  -learning#zoo)..
+000028e0: 5468 6520 7472 6963 6b20 7761 7320 696e  The trick was in
+000028f0: 2068 6575 7269 7374 6963 7320 696e 206f   heuristics in o
+00002900: 7572 206d 696e 6572 2061 6e64 2073 616d  ur miner and sam
+00002910: 706c 6572 3a0a 0a2a 205b 4361 7465 676f  pler:..* [Catego
+00002920: 7279 2042 616c 616e 6365 2053 616d 706c  ry Balance Sampl
+00002930: 6572 5d28 6874 7470 733a 2f2f 6f70 656e  er](https://open
+00002940: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00002950: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002960: 656e 2f6c 6174 6573 742f 636f 6e74 656e  en/latest/conten
+00002970: 7473 2f73 616d 706c 6572 732e 6874 6d6c  ts/samplers.html
+00002980: 2363 6174 6567 6f72 7962 616c 616e 6365  #categorybalance
+00002990: 7361 6d70 6c65 7229 0a20 2066 6f72 6d73  sampler).  forms
+000029a0: 2074 6865 2062 6174 6368 6573 206c 696d   the batches lim
+000029b0: 6974 696e 6720 7468 6520 6e75 6d62 6572  iting the number
+000029c0: 206f 6620 6361 7465 676f 7269 6573 202a   of categories *
+000029d0: 432a 2069 6e20 6974 2e0a 2020 466f 7220  C* in it..  For 
+000029e0: 696e 7374 616e 6365 2c20 7768 656e 202a  instance, when *
+000029f0: 4320 3d20 312a 2069 7420 7075 7473 206f  C = 1* it puts o
+00002a00: 6e6c 7920 6a61 636b 6574 7320 696e 206f  nly jackets in o
+00002a10: 6e65 2062 6174 6368 2061 6e64 206f 6e6c  ne batch and onl
+00002a20: 7920 6a65 616e 7320 696e 746f 2061 6e6f  y jeans into ano
+00002a30: 7468 6572 206f 6e65 2028 6a75 7374 2061  ther one (just a
+00002a40: 6e20 6578 616d 706c 6529 2e0a 2020 4974  n example)..  It
+00002a50: 2061 7574 6f6d 6174 6963 616c 6c79 206d   automatically m
+00002a60: 616b 6573 2074 6865 206e 6567 6174 6976  akes the negativ
+00002a70: 6520 7061 6972 7320 6861 7264 6572 3a20  e pairs harder: 
+00002a80: 6974 2773 206d 6f72 6520 6d65 616e 696e  it's more meanin
+00002a90: 6766 756c 2066 6f72 2061 206d 6f64 656c  gful for a model
+00002aa0: 2074 6f20 7265 616c 6973 6520 7768 7920   to realise why 
+00002ab0: 7477 6f20 6a61 636b 6574 730a 2020 6172  two jackets.  ar
+00002ac0: 6520 6469 6666 6572 656e 7420 7468 616e  e different than
+00002ad0: 2074 6f20 756e 6465 7273 7461 6e64 2074   to understand t
+00002ae0: 6865 2073 616d 6520 6162 6f75 7420 6120  he same about a 
+00002af0: 6a61 636b 6574 2061 6e64 2061 2074 2d73  jacket and a t-s
+00002b00: 6869 7274 2e0a 0a2a 205b 4861 7264 2054  hirt...* [Hard T
+00002b10: 7269 706c 6574 7320 4d69 6e65 725d 2868  riplets Miner](h
+00002b20: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+00002b30: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+00002b40: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00002b50: 7465 7374 2f63 6f6e 7465 6e74 732f 6d69  test/contents/mi
+00002b60: 6e65 7273 2e68 746d 6c23 6861 7264 7472  ners.html#hardtr
+00002b70: 6970 6c65 7473 6d69 6e65 7229 0a20 206d  ipletsminer).  m
+00002b80: 616b 6573 2074 6865 2074 6173 6b20 6576  akes the task ev
+00002b90: 656e 2068 6172 6465 7220 6b65 6570 696e  en harder keepin
+00002ba0: 6720 6f6e 6c79 2074 6865 2068 6172 6465  g only the harde
+00002bb0: 7374 2074 7269 706c 6574 7320 2877 6974  st triplets (wit
+00002bc0: 6820 6d61 7869 6d61 6c20 706f 7369 7469  h maximal positi
+00002bd0: 7665 2061 6e64 206d 696e 696d 616c 206e  ve and minimal n
+00002be0: 6567 6174 6976 6520 6469 7374 616e 6365  egative distance
+00002bf0: 7329 2e0a 0a48 6572 6520 6172 6520 2a43  s)...Here are *C
+00002c00: 4d43 4031 2a20 7363 6f72 6573 2066 6f72  MC@1* scores for
+00002c10: 2032 2070 6f70 756c 6172 2062 656e 6368   2 popular bench
+00002c20: 6d61 726b 732e 0a53 4f50 2064 6174 6173  marks..SOP datas
+00002c30: 6574 3a20 4879 702d 5669 5420 e280 9420  et: Hyp-ViT ... 
+00002c40: 3835 2e39 2c20 6f75 7273 20e2 8094 2038  85.9, ours ... 8
+00002c50: 362e 362e 2044 6565 7046 6173 6869 6f6e  6.6. DeepFashion
+00002c60: 2064 6174 6173 6574 3a20 4879 702d 5669   dataset: Hyp-Vi
+00002c70: 5420 e280 9420 3932 2e35 2c20 6f75 7273  T ... 92.5, ours
+00002c80: 20e2 8094 2039 322e 312e 0a54 6875 732c   ... 92.1..Thus,
+00002c90: 2075 7469 6c69 7369 6e67 2073 696d 706c   utilising simpl
+00002ca0: 6520 6865 7572 6973 7469 6373 2061 6e64  e heuristics and
+00002cb0: 2061 766f 6964 696e 6720 6865 6176 7920   avoiding heavy 
+00002cc0: 6d61 7468 2077 6520 6172 6520 6162 6c65  math we are able
+00002cd0: 2074 6f20 7065 7266 6f72 6d20 6f6e 2053   to perform on S
+00002ce0: 6f74 4120 6c65 7665 6c2e 0a0a 3c2f 703e  otA level...</p>
+00002cf0: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00002d00: 7461 696c 733e 0a3c 7375 6d6d 6172 793e  tails>.<summary>
+00002d10: 5768 6174 2061 626f 7574 2053 656c 662d  What about Self-
+00002d20: 5375 7065 7276 6973 6564 204c 6561 726e  Supervised Learn
+00002d30: 696e 673f 3c2f 7375 6d6d 6172 793e 0a3c  ing?</summary>.<
+00002d40: 703e 0a0a 5265 6365 6e74 2072 6573 6561  p>..Recent resea
+00002d50: 7263 6820 696e 2053 534c 2064 6566 696e  rch in SSL defin
+00002d60: 6974 656c 7920 6f62 7461 696e 6564 2067  itely obtained g
+00002d70: 7265 6174 2072 6573 756c 7473 2e20 5468  reat results. Th
+00002d80: 6520 7072 6f62 6c65 6d20 6973 2074 6861  e problem is tha
+00002d90: 7420 7468 6573 6520 6170 7072 6f61 6368  t these approach
+00002da0: 6573 0a72 6571 7569 7265 6420 616e 2065  es.required an e
+00002db0: 6e6f 726d 6f75 7320 616d 6f75 6e74 206f  normous amount o
+00002dc0: 6620 636f 6d70 7574 696e 6720 746f 2074  f computing to t
+00002dd0: 7261 696e 2074 6865 206d 6f64 656c 2e20  rain the model. 
+00002de0: 4275 7420 696e 206f 7572 2066 7261 6d65  But in our frame
+00002df0: 776f 726b 2c20 7765 2063 6f6e 7369 6465  work, we conside
+00002e00: 7220 7468 6520 6d6f 7374 2063 6f6d 6d6f  r the most commo
+00002e10: 6e20 6361 7365 0a77 6865 6e20 7468 6520  n case.when the 
+00002e20: 6176 6572 6167 6520 7573 6572 2068 6173  average user has
+00002e30: 206e 6f20 6d6f 7265 2074 6861 6e20 6120   no more than a 
+00002e40: 6665 7720 4750 5573 2e0a 0a41 7420 7468  few GPUs...At th
+00002e50: 6520 7361 6d65 2074 696d 652c 2069 7420  e same time, it 
+00002e60: 776f 756c 6420 6265 2075 6e77 6973 6520  would be unwise 
+00002e70: 746f 2069 676e 6f72 6520 7375 6363 6573  to ignore succes
+00002e80: 7320 696e 2074 6869 7320 7370 6865 7265  s in this sphere
+00002e90: 2c20 736f 2077 6520 7374 696c 6c20 6578  , so we still ex
+00002ea0: 706c 6f69 7420 6974 2069 6e20 7477 6f20  ploit it in two 
+00002eb0: 7761 7973 3a0a 2a20 4173 2061 2073 6f75  ways:.* As a sou
+00002ec0: 7263 6520 6f66 2063 6865 636b 706f 696e  rce of checkpoin
+00002ed0: 7473 2074 6861 7420 776f 756c 6420 6265  ts that would be
+00002ee0: 2067 7265 6174 2074 6f20 7374 6172 7420   great to start 
+00002ef0: 7472 6169 6e69 6e67 2077 6974 682e 2046  training with. F
+00002f00: 726f 6d20 7075 626c 6963 6174 696f 6e73  rom publications
+00002f10: 2061 6e64 206f 7572 2065 7870 6572 6965   and our experie
+00002f20: 6e63 652c 0a20 2074 6865 7920 6172 6520  nce,.  they are 
+00002f30: 6d75 6368 2062 6574 7465 7220 6173 2069  much better as i
+00002f40: 6e69 7469 616c 6973 6174 696f 6e20 7468  nitialisation th
+00002f50: 616e 2074 6865 2064 6566 6175 6c74 2073  an the default s
+00002f60: 7570 6572 7669 7365 6420 6d6f 6465 6c20  upervised model 
+00002f70: 7472 6169 6e65 6420 6f6e 2049 6d61 6765  trained on Image
+00002f80: 4e65 742e 2054 6875 732c 2077 6520 6164  Net. Thus, we ad
+00002f90: 6465 6420 7468 6520 706f 7373 6962 696c  ded the possibil
+00002fa0: 6974 790a 2020 746f 2069 6e69 7469 616c  ity.  to initial
+00002fb0: 6973 6520 796f 7572 206d 6f64 656c 7320  ise your models 
+00002fc0: 7573 696e 6720 7468 6573 6520 7072 6574  using these pret
+00002fd0: 7261 696e 6564 2063 6865 636b 706f 696e  rained checkpoin
+00002fe0: 7473 206f 6e6c 7920 6279 2070 6173 7369  ts only by passi
+00002ff0: 6e67 2061 6e20 6172 6775 6d65 6e74 2069  ng an argument i
+00003000: 6e20 7468 6520 636f 6e66 6967 206f 7220  n the config or 
+00003010: 7468 6520 636f 6e73 7472 7563 746f 722e  the constructor.
+00003020: 0a2a 2041 7320 6120 736f 7572 6365 206f  .* As a source o
+00003030: 6620 696e 7370 6972 6174 696f 6e2e 2046  f inspiration. F
+00003040: 6f72 2065 7861 6d70 6c65 2c20 7765 2061  or example, we a
+00003050: 6461 7074 6564 2074 6865 2069 6465 6120  dapted the idea 
+00003060: 6f66 2061 206d 656d 6f72 7920 6261 6e6b  of a memory bank
+00003070: 2066 726f 6d20 2a4d 6f43 6f2a 2066 6f72   from *MoCo* for
+00003080: 2074 6865 202a 5472 6970 6c65 744c 6f73   the *TripletLos
+00003090: 732a 2e0a 0a3c 2f70 3e0a 3c2f 6465 7461  s*...</p>.</deta
+000030a0: 696c 733e 0a0a 0a3c 6465 7461 696c 733e  ils>...<details>
+000030b0: 0a3c 7375 6d6d 6172 793e 446f 2049 206e  .<summary>Do I n
+000030c0: 6565 6420 746f 206b 6e6f 7720 6f74 6865  eed to know othe
+000030d0: 7220 6672 616d 6577 6f72 6b73 2074 6f20  r frameworks to 
+000030e0: 7573 6520 4f4d 4c3f 3c2f 7375 6d6d 6172  use OML?</summar
+000030f0: 793e 0a3c 703e 0a0a 4e6f 2c20 796f 7520  y>.<p>..No, you 
+00003100: 646f 6e27 742e 204f 4d4c 2069 7320 6120  don't. OML is a 
+00003110: 6672 616d 6577 6f72 6b2d 6167 6e6f 7374  framework-agnost
+00003120: 6963 2e20 4465 7370 6974 6520 7765 2075  ic. Despite we u
+00003130: 7365 2050 7954 6f72 6368 204c 6967 6874  se PyTorch Light
+00003140: 6e69 6e67 2061 7320 6120 6c6f 6f70 0a72  ning as a loop.r
+00003150: 756e 6e65 7220 666f 7220 7468 6520 6578  unner for the ex
+00003160: 7065 7269 6d65 6e74 732c 2077 6520 616c  periments, we al
+00003170: 736f 206b 6565 7020 7468 6520 706f 7373  so keep the poss
+00003180: 6962 696c 6974 7920 746f 2072 756e 2065  ibility to run e
+00003190: 7665 7279 7468 696e 6720 6f6e 2070 7572  verything on pur
+000031a0: 6520 5079 546f 7263 682e 0a54 6875 732c  e PyTorch..Thus,
+000031b0: 206f 6e6c 7920 7468 6520 7469 6e79 2070   only the tiny p
+000031c0: 6172 7420 6f66 204f 4d4c 2069 7320 4c69  art of OML is Li
+000031d0: 6768 746e 696e 672d 7370 6563 6966 6963  ghtning-specific
+000031e0: 2061 6e64 2077 6520 6b65 6570 2074 6869   and we keep thi
+000031f0: 7320 6c6f 6769 6320 7365 7061 7261 7465  s logic separate
+00003200: 6c79 2066 726f 6d0a 6f74 6865 7220 636f  ly from.other co
+00003210: 6465 2028 7365 6520 606f 6d6c 2e6c 6967  de (see `oml.lig
+00003220: 6874 6e69 6e67 6029 2e20 4576 656e 2077  htning`). Even w
+00003230: 6865 6e20 796f 7520 7573 6520 4c69 6768  hen you use Ligh
+00003240: 746e 696e 672c 2079 6f75 2064 6f6e 2774  tning, you don't
+00003250: 206e 6565 6420 746f 206b 6e6f 7720 6974   need to know it
+00003260: 2c20 7369 6e63 650a 7765 2070 726f 7669  , since.we provi
+00003270: 6465 2072 6561 6479 2074 6f20 7573 6520  de ready to use 
+00003280: 5b50 6970 656c 696e 6573 5d28 6874 7470  [Pipelines](http
+00003290: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
+000032a0: 4d4c 2d54 6561 6d2f 6f70 656e 2d6d 6574  ML-Team/open-met
+000032b0: 7269 632d 6c65 6172 6e69 6e67 2f62 6c6f  ric-learning/blo
+000032c0: 622f 6d61 696e 2f70 6970 656c 696e 6573  b/main/pipelines
+000032d0: 2f29 2e0a 0a54 6865 2070 6f73 7369 6269  /)...The possibi
+000032e0: 6c69 7479 206f 6620 7573 696e 6720 7075  lity of using pu
+000032f0: 7265 2050 7954 6f72 6368 2061 6e64 206d  re PyTorch and m
+00003300: 6f64 756c 6172 2073 7472 7563 7475 7265  odular structure
+00003310: 206f 6620 7468 6520 636f 6465 206c 6561   of the code lea
+00003320: 7665 7320 6120 726f 6f6d 2066 6f72 2075  ves a room for u
+00003330: 7469 6c69 7a69 6e67 0a4f 4d4c 2077 6974  tilizing.OML wit
+00003340: 6820 796f 7572 2066 6176 6f75 7269 7465  h your favourite
+00003350: 2066 7261 6d65 776f 726b 2061 6674 6572   framework after
+00003360: 2074 6865 2069 6d70 6c65 6d65 6e74 6174   the implementat
+00003370: 696f 6e20 6f66 2074 6865 206e 6563 6573  ion of the neces
+00003380: 7361 7279 2077 7261 7070 6572 732e 0a0a  sary wrappers...
+00003390: 3c2f 703e 0a3c 2f64 6574 6169 6c73 3e0a  </p>.</details>.
+000033a0: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
+000033b0: 6d61 7279 3e43 616e 2049 2075 7365 204f  mary>Can I use O
+000033c0: 4d4c 2077 6974 686f 7574 2061 6e79 206b  ML without any k
+000033d0: 6e6f 776c 6564 6765 2069 6e20 4461 7461  nowledge in Data
+000033e0: 5363 6965 6e63 653f 3c2f 7375 6d6d 6172  Science?</summar
+000033f0: 793e 0a3c 703e 0a0a 5965 732e 2054 6f20  y>.<p>..Yes. To 
+00003400: 7275 6e20 7468 6520 6578 7065 7269 6d65  run the experime
+00003410: 6e74 2077 6974 6820 5b50 6970 656c 696e  nt with [Pipelin
+00003420: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00003430: 7562 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f  ub.com/OML-Team/
+00003440: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00003450: 6e69 6e67 2f62 6c6f 622f 6d61 696e 2f70  ning/blob/main/p
+00003460: 6970 656c 696e 6573 2f29 0a79 6f75 206f  ipelines/).you o
+00003470: 6e6c 7920 6e65 6564 2074 6f20 7772 6974  nly need to writ
+00003480: 6520 6120 636f 6e76 6572 7465 720a 746f  e a converter.to
+00003490: 206f 7572 2066 6f72 6d61 7420 2869 7420   our format (it 
+000034a0: 6d65 616e 7320 7072 6570 6172 696e 6720  means preparing 
+000034b0: 7468 650a 602e 6373 7660 2074 6162 6c65  the.`.csv` table
+000034c0: 2077 6974 6820 3520 7072 6564 6566 696e   with 5 predefin
+000034d0: 6564 2063 6f6c 756d 6e73 292e 0a54 6861  ed columns)..Tha
+000034e0: 7427 7320 6974 210a 0a50 726f 6261 626c  t's it!..Probabl
+000034f0: 7920 7765 2061 6c72 6561 6479 2068 6176  y we already hav
+00003500: 6520 6120 7375 6974 6162 6c65 2070 7265  e a suitable pre
+00003510: 2d74 7261 696e 6564 206d 6f64 656c 2066  -trained model f
+00003520: 6f72 2079 6f75 7220 646f 6d61 696e 0a69  or your domain.i
+00003530: 6e20 6f75 7220 2a4d 6f64 656c 7320 5a6f  n our *Models Zo
+00003540: 6f2a 2e20 496e 2074 6869 7320 6361 7365  o*. In this case
+00003550: 2c20 796f 7520 646f 6e27 7420 6576 656e  , you don't even
+00003560: 206e 6565 6420 746f 2074 7261 696e 2069   need to train i
+00003570: 742e 0a3c 2f70 3e0a 3c2f 6465 7461 696c  t..</p>.</detail
+00003580: 733e 0a0a 2323 205b 446f 6375 6d65 6e74  s>..## [Document
+00003590: 6174 696f 6e5d 2868 7474 7073 3a2f 2f6f  ation](https://o
+000035a0: 7065 6e2d 6d65 7472 6963 2d6c 6561 726e  pen-metric-learn
+000035b0: 696e 672e 7265 6164 7468 6564 6f63 732e  ing.readthedocs.
+000035c0: 696f 2f65 6e2f 6c61 7465 7374 2f69 6e64  io/en/latest/ind
+000035d0: 6578 2e68 746d 6c29 0a0a 446f 6375 6d65  ex.html)..Docume
+000035e0: 6e74 6174 696f 6e20 6973 2061 7661 696c  ntation is avail
+000035f0: 6162 6c65 2076 6961 2074 6865 205b 6c69  able via the [li
+00003600: 6e6b 5d28 6874 7470 733a 2f2f 6f70 656e  nk](https://open
+00003610: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00003620: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00003630: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
+00003640: 6874 6d6c 292e 0a0a 596f 7520 6361 6e20  html)...You can 
+00003650: 616c 736f 2072 6561 6420 736f 6d65 2065  also read some e
+00003660: 7874 7261 206d 6174 6572 6961 6c73 2072  xtra materials r
+00003670: 656c 6174 6564 2074 6f20 4f4d 4c3a 0a0a  elated to OML:..
+00003680: 2a20 5468 656f 7279 2061 6e64 2070 7261  * Theory and pra
+00003690: 6374 6963 6520 6f66 206d 6574 7269 6320  ctice of metric 
+000036a0: 6c65 6172 6e69 6e67 2077 6974 6820 7468  learning with th
+000036b0: 6520 7573 6167 6520 6f66 204f 4d4c 2e0a  e usage of OML..
+000036c0: 5b50 6f73 7420 696e 2045 6e67 6c69 7368  [Post in English
+000036d0: 206f 6e20 4d65 6469 756d 5d28 6874 7470   on Medium](http
+000036e0: 733a 2f2f 6d65 6469 756d 2e63 6f6d 2f40  s://medium.com/@
+000036f0: 416c 656b 7365 6953 6861 6261 6e6f 762f  AlekseiShabanov/
+00003700: 7072 6163 7469 6361 6c2d 6d65 7472 6963  practical-metric
+00003710: 2d6c 6561 726e 696e 672d 6230 3431 3063  -learning-b0410c
+00003720: 6461 3232 3031 2920 7c0a 5b50 6f73 7420  da2201) |.[Post 
+00003730: 696e 2052 7573 7369 616e 206f 6e20 4861  in Russian on Ha
+00003740: 6272 5d28 6874 7470 733a 2f2f 6861 6272  br](https://habr
+00003750: 2e63 6f6d 2f72 752f 636f 6d70 616e 792f  .com/ru/company/
+00003760: 6f64 732f 626c 6f67 2f36 3935 3338 302f  ods/blog/695380/
+00003770: 2920 7c0a 5b50 6f73 7420 696e 2043 6869  ) |.[Post in Chi
+00003780: 6e65 7365 206f 6e20 4353 444e 5d28 6874  nese on CSDN](ht
+00003790: 7470 733a 2f2f 626c 6f67 2e63 7364 6e2e  tps://blog.csdn.
+000037a0: 6e65 742f 6665 726d 696f 6e30 3231 372f  net/fermion0217/
+000037b0: 6172 7469 636c 652f 6465 7461 696c 732f  article/details/
+000037c0: 3132 3739 3332 3038 3729 2c20 7472 616e  127932087), tran
+000037d0: 736c 6174 6564 2062 7920 4368 6961 2d43  slated by Chia-C
+000037e0: 6865 6e20 4368 616e 672e 0a0a 2a20 5468  hen Chang...* Th
+000037f0: 650a 5b44 454d 4f5d 2868 7474 7073 3a2f  e.[DEMO](https:/
+00003800: 2f64 6170 6c61 646f 632d 6f6d 6c2d 706f  /dapladoc-oml-po
+00003810: 7374 7072 6f63 6573 7369 6e67 2d64 656d  stprocessing-dem
+00003820: 6f2d 7372 6361 7070 6d61 696e 2d70 6668  o-srcappmain-pfh
+00003830: 3267 302e 7374 7265 616d 6c69 742e 6170  2g0.streamlit.ap
+00003840: 702f 290a 666f 7220 6f75 7220 7061 7065  p/).for our pape
+00003850: 720a 5b53 5449 523a 2053 6961 6d65 7365  r.[STIR: Siamese
+00003860: 2054 7261 6e73 666f 726d 6572 7320 666f   Transformers fo
+00003870: 7220 496d 6167 6520 5265 7472 6965 7661  r Image Retrieva
+00003880: 6c20 506f 7374 7072 6f63 6573 7369 6e67  l Postprocessing
+00003890: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+000038a0: 6f72 672f 6162 732f 3233 3034 2e31 3333  org/abs/2304.133
+000038b0: 3933 290a 0a2a 2054 6865 2072 6570 6f72  93)..* The repor
+000038c0: 7420 666f 7220 4265 726c 696e 2d62 6173  t for Berlin-bas
+000038d0: 6564 206d 6565 7475 703a 2022 436f 6d70  ed meetup: "Comp
+000038e0: 7574 6572 2056 6973 696f 6e20 696e 2070  uter Vision in p
+000038f0: 726f 6475 6374 696f 6e22 2e20 4e6f 7665  roduction". Nove
+00003900: 6d62 6572 2c20 3230 3232 2e0a 5b4c 696e  mber, 2022..[Lin
+00003910: 6b5d 2868 7474 7073 3a2f 2f64 7269 7665  k](https://drive
+00003920: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00003930: 652f 666f 6c64 6572 732f 3175 486d 4c55  e/folders/1uHmLU
+00003940: 3876 4d72 4d56 4d46 6f64 7433 3675 3075  8vMrMVMFodt36u0u
+00003950: 5841 6759 6a47 5f33 4433 303f 7573 703d  XAgYjG_3D30?usp=
+00003960: 7368 6172 655f 6c69 6e6b 290a 0a23 2320  share_link)..## 
+00003970: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2868  [Installation](h
+00003980: 7474 7073 3a2f 2f6f 7065 6e2d 6d65 7472  ttps://open-metr
+00003990: 6963 2d6c 6561 726e 696e 672e 7265 6164  ic-learning.read
+000039a0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000039b0: 7465 7374 2f6f 6d6c 2f69 6e73 7461 6c6c  test/oml/install
+000039c0: 6174 696f 6e2e 6874 6d6c 290a 0a4f 4d4c  ation.html)..OML
+000039d0: 2069 7320 6176 6169 6c61 626c 6520 696e   is available in
+000039e0: 2050 7950 493a 0a0a 6060 6073 6865 6c6c   PyPI:..```shell
+000039f0: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00003a00: 6f70 656e 2d6d 6574 7269 632d 6c65 6172  open-metric-lear
+00003a10: 6e69 6e67 0a60 6060 0a0a 596f 7520 6361  ning.```..You ca
+00003a20: 6e20 616c 736f 2070 756c 6c20 7468 6520  n also pull the 
+00003a30: 7072 6570 6172 6564 2069 6d61 6765 2066  prepared image f
+00003a40: 726f 6d20 446f 636b 6572 4875 622e 2e2e  rom DockerHub...
+00003a50: 0a0a 6060 6073 6865 6c6c 0a64 6f63 6b65  ..```shell.docke
+00003a60: 7220 7075 6c6c 206f 6d6c 7465 616d 2f6f  r pull omlteam/o
+00003a70: 6d6c 3a67 7075 0a64 6f63 6b65 7220 7075  ml:gpu.docker pu
+00003a80: 6c6c 206f 6d6c 7465 616d 2f6f 6d6c 3a63  ll omlteam/oml:c
+00003a90: 7075 0a60 6060 0a0a 2e2e 2e6f 7220 6275  pu.```.....or bu
+00003aa0: 696c 6420 6f6e 6520 6279 2079 6f75 7220  ild one by your 
+00003ab0: 6f77 6e0a 0a60 6060 7368 656c 6c0a 6d61  own..```shell.ma
+00003ac0: 6b65 2064 6f63 6b65 725f 6275 696c 6420  ke docker_build 
+00003ad0: 5255 4e54 494d 453d 6370 750a 6d61 6b65  RUNTIME=cpu.make
+00003ae0: 2064 6f63 6b65 725f 6275 696c 6420 5255   docker_build RU
+00003af0: 4e54 494d 453d 6770 750a 6060 600a 0a23  NTIME=gpu.```..#
+00003b00: 2320 5b45 7861 6d70 6c65 735d 2868 7474  # [Examples](htt
+00003b10: 7073 3a2f 2f6f 7065 6e2d 6d65 7472 6963  ps://open-metric
+00003b20: 2d6c 6561 726e 696e 672e 7265 6164 7468  -learning.readth
+00003b30: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00003b40: 7374 2f66 6561 7475 7265 5f65 7874 7261  st/feature_extra
+00003b50: 6374 696f 6e2f 7079 7468 6f6e 5f65 7861  ction/python_exa
+00003b60: 6d70 6c65 732e 6874 6d6c 2329 0a0a 3c64  mples.html#)..<d
+00003b70: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00003b80: 3e54 7261 696e 696e 673c 2f73 756d 6d61  >Training</summa
+00003b90: 7279 3e0a 3c70 3e0a 0a5b 636f 6d6d 656e  ry>.<p>..[commen
+00003ba0: 745d 3a76 616e 696c 6c61 2d74 7261 696e  t]:vanilla-train
+00003bb0: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
+00003bc0: 0a69 6d70 6f72 7420 746f 7263 680a 6672  .import torch.fr
+00003bd0: 6f6d 2074 7164 6d20 696d 706f 7274 2074  om tqdm import t
+00003be0: 7164 6d0a 0a66 726f 6d20 6f6d 6c2e 6461  qdm..from oml.da
+00003bf0: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00003c00: 7274 2044 6174 6173 6574 5769 7468 4c61  rt DatasetWithLa
+00003c10: 6265 6c73 0a66 726f 6d20 6f6d 6c2e 6c6f  bels.from oml.lo
+00003c20: 7373 6573 2e74 7269 706c 6574 2069 6d70  sses.triplet imp
+00003c30: 6f72 7420 5472 6970 6c65 744c 6f73 7357  ort TripletLossW
+00003c40: 6974 684d 696e 6572 0a66 726f 6d20 6f6d  ithMiner.from om
+00003c50: 6c2e 6d69 6e65 7273 2e69 6e62 6174 6368  l.miners.inbatch
+00003c60: 5f61 6c6c 5f74 7269 2069 6d70 6f72 7420  _all_tri import 
+00003c70: 416c 6c54 7269 706c 6574 734d 696e 6572  AllTripletsMiner
+00003c80: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
+00003c90: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
+00003ca0: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7361  ctor.from oml.sa
+00003cb0: 6d70 6c65 7273 2e62 616c 616e 6365 2069  mplers.balance i
+00003cc0: 6d70 6f72 7420 4261 6c61 6e63 6553 616d  mport BalanceSam
+00003cd0: 706c 6572 0a66 726f 6d20 6f6d 6c2e 7574  pler.from oml.ut
+00003ce0: 696c 732e 646f 776e 6c6f 6164 5f6d 6f63  ils.download_moc
+00003cf0: 6b5f 6461 7461 7365 7420 696d 706f 7274  k_dataset import
+00003d00: 2064 6f77 6e6c 6f61 645f 6d6f 636b 5f64   download_mock_d
+00003d10: 6174 6173 6574 0a0a 6461 7461 7365 745f  ataset..dataset_
+00003d20: 726f 6f74 203d 2022 6d6f 636b 5f64 6174  root = "mock_dat
+00003d30: 6173 6574 2f22 0a64 665f 7472 6169 6e2c  aset/".df_train,
+00003d40: 205f 203d 2064 6f77 6e6c 6f61 645f 6d6f   _ = download_mo
+00003d50: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+00003d60: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+00003d70: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00003d80: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+00003d90: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+00003da0: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+00003db0: 7265 733d 4661 6c73 6529 2e74 7261 696e  res=False).train
+00003dc0: 2829 0a6f 7074 696d 697a 6572 203d 2074  ().optimizer = t
+00003dd0: 6f72 6368 2e6f 7074 696d 2e53 4744 2865  orch.optim.SGD(e
+00003de0: 7874 7261 6374 6f72 2e70 6172 616d 6574  xtractor.paramet
+00003df0: 6572 7328 292c 206c 723d 3165 2d36 290a  ers(), lr=1e-6).
+00003e00: 0a74 7261 696e 5f64 6174 6173 6574 203d  .train_dataset =
+00003e10: 2044 6174 6173 6574 5769 7468 4c61 6265   DatasetWithLabe
+00003e20: 6c73 2864 665f 7472 6169 6e2c 2064 6174  ls(df_train, dat
+00003e30: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+00003e40: 745f 726f 6f74 290a 6372 6974 6572 696f  t_root).criterio
+00003e50: 6e20 3d20 5472 6970 6c65 744c 6f73 7357  n = TripletLossW
+00003e60: 6974 684d 696e 6572 286d 6172 6769 6e3d  ithMiner(margin=
+00003e70: 302e 312c 206d 696e 6572 3d41 6c6c 5472  0.1, miner=AllTr
+00003e80: 6970 6c65 7473 4d69 6e65 7228 292c 206e  ipletsMiner(), n
+00003e90: 6565 645f 6c6f 6773 3d54 7275 6529 0a73  eed_logs=True).s
+00003ea0: 616d 706c 6572 203d 2042 616c 616e 6365  ampler = Balance
+00003eb0: 5361 6d70 6c65 7228 7472 6169 6e5f 6461  Sampler(train_da
+00003ec0: 7461 7365 742e 6765 745f 6c61 6265 6c73  taset.get_labels
+00003ed0: 2829 2c20 6e5f 6c61 6265 6c73 3d32 2c20  (), n_labels=2, 
+00003ee0: 6e5f 696e 7374 616e 6365 733d 3229 0a74  n_instances=2).t
+00003ef0: 7261 696e 5f6c 6f61 6465 7220 3d20 746f  rain_loader = to
+00003f00: 7263 682e 7574 696c 732e 6461 7461 2e44  rch.utils.data.D
+00003f10: 6174 614c 6f61 6465 7228 7472 6169 6e5f  ataLoader(train_
+00003f20: 6461 7461 7365 742c 2062 6174 6368 5f73  dataset, batch_s
+00003f30: 616d 706c 6572 3d73 616d 706c 6572 290a  ampler=sampler).
+00003f40: 0a66 6f72 2062 6174 6368 2069 6e20 7471  .for batch in tq
+00003f50: 646d 2874 7261 696e 5f6c 6f61 6465 7229  dm(train_loader)
+00003f60: 3a0a 2020 2020 656d 6265 6464 696e 6773  :.    embeddings
+00003f70: 203d 2065 7874 7261 6374 6f72 2862 6174   = extractor(bat
+00003f80: 6368 5b22 696e 7075 745f 7465 6e73 6f72  ch["input_tensor
+00003f90: 7322 5d29 0a20 2020 206c 6f73 7320 3d20  s"]).    loss = 
+00003fa0: 6372 6974 6572 696f 6e28 656d 6265 6464  criterion(embedd
+00003fb0: 696e 6773 2c20 6261 7463 685b 226c 6162  ings, batch["lab
+00003fc0: 656c 7322 5d29 0a20 2020 206c 6f73 732e  els"]).    loss.
+00003fd0: 6261 636b 7761 7264 2829 0a20 2020 206f  backward().    o
+00003fe0: 7074 696d 697a 6572 2e73 7465 7028 290a  ptimizer.step().
+00003ff0: 2020 2020 6f70 7469 6d69 7a65 722e 7a65      optimizer.ze
+00004000: 726f 5f67 7261 6428 290a 0a20 2020 2023  ro_grad()..    #
+00004010: 2069 6e66 6f20 666f 7220 6c6f 6767 696e   info for loggin
+00004020: 673a 2070 6f73 6974 6976 652f 6e65 6761  g: positive/nega
+00004030: 7469 7665 2064 6973 7461 6e63 6573 2c20  tive distances, 
+00004040: 6e75 6d62 6572 206f 6620 6163 7469 7665  number of active
+00004050: 2074 7269 706c 6574 730a 2020 2020 7072   triplets.    pr
+00004060: 696e 7428 6372 6974 6572 696f 6e2e 6c61  int(criterion.la
+00004070: 7374 5f6c 6f67 7329 0a0a 6060 600a 5b63  st_logs)..```.[c
+00004080: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+00004090: 7472 6169 6e2d 656e 640a 3c2f 703e 0a3c  train-end.</p>.<
+000040a0: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+000040b0: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+000040c0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+000040d0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+000040e0: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+000040f0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00004100: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00004110: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00004120: 316b 6e74 4441 4964 495a 394c 3430 6a63  1kntDAIdIZ9L40jc
+00004130: 6e64 6775 4c41 622d 5871 6d43 464f 6753  ndguLAb-XqmCFOgS
+00004140: 353f 7573 703d 7368 6172 696e 6729 0a3c  5?usp=sharing).<
+00004150: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00004160: 793e 5661 6c69 6461 7469 6f6e 3c2f 7375  y>Validation</su
+00004170: 6d6d 6172 793e 0a3c 703e 0a0a 5b63 6f6d  mmary>.<p>..[com
+00004180: 6d65 6e74 5d3a 7661 6e69 6c6c 612d 7661  ment]:vanilla-va
+00004190: 6c69 6461 7469 6f6e 2d73 7461 7274 0a60  lidation-start.`
+000041a0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+000041b0: 746f 7263 680a 6672 6f6d 2074 7164 6d20  torch.from tqdm 
+000041c0: 696d 706f 7274 2074 7164 6d0a 0a66 726f  import tqdm..fro
+000041d0: 6d20 6f6d 6c2e 6461 7461 7365 7473 2e62  m oml.datasets.b
+000041e0: 6173 6520 696d 706f 7274 2044 6174 6173  ase import Datas
+000041f0: 6574 5175 6572 7947 616c 6c65 7279 0a66  etQueryGallery.f
+00004200: 726f 6d20 6f6d 6c2e 6d65 7472 6963 732e  rom oml.metrics.
+00004210: 656d 6265 6464 696e 6773 2069 6d70 6f72  embeddings impor
+00004220: 7420 456d 6265 6464 696e 674d 6574 7269  t EmbeddingMetri
+00004230: 6373 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  cs.from oml.mode
+00004240: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+00004250: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+00004260: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+00004270: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004280: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004290: 5f64 6174 6173 6574 0a0a 6461 7461 7365  _dataset..datase
+000042a0: 745f 726f 6f74 203d 2022 6d6f 636b 5f64  t_root = "mock_d
+000042b0: 6174 6173 6574 2f22 0a5f 2c20 6466 5f76  ataset/"._, df_v
+000042c0: 616c 203d 2064 6f77 6e6c 6f61 645f 6d6f  al = download_mo
+000042d0: 636b 5f64 6174 6173 6574 2864 6174 6173  ck_dataset(datas
+000042e0: 6574 5f72 6f6f 7429 0a0a 6578 7472 6163  et_root)..extrac
+000042f0: 746f 7220 3d20 5669 5445 7874 7261 6374  tor = ViTExtract
+00004300: 6f72 2822 7669 7473 3136 5f64 696e 6f22  or("vits16_dino"
+00004310: 2c20 6172 6368 3d22 7669 7473 3136 222c  , arch="vits16",
+00004320: 206e 6f72 6d61 6c69 7365 5f66 6561 7475   normalise_featu
+00004330: 7265 733d 4661 6c73 6529 2e65 7661 6c28  res=False).eval(
+00004340: 290a 0a76 616c 5f64 6174 6173 6574 203d  )..val_dataset =
+00004350: 2044 6174 6173 6574 5175 6572 7947 616c   DatasetQueryGal
+00004360: 6c65 7279 2864 665f 7661 6c2c 2064 6174  lery(df_val, dat
+00004370: 6173 6574 5f72 6f6f 743d 6461 7461 7365  aset_root=datase
+00004380: 745f 726f 6f74 290a 0a76 616c 5f6c 6f61  t_root)..val_loa
+00004390: 6465 7220 3d20 746f 7263 682e 7574 696c  der = torch.util
+000043a0: 732e 6461 7461 2e44 6174 614c 6f61 6465  s.data.DataLoade
+000043b0: 7228 7661 6c5f 6461 7461 7365 742c 2062  r(val_dataset, b
+000043c0: 6174 6368 5f73 697a 653d 3429 0a63 616c  atch_size=4).cal
+000043d0: 6375 6c61 746f 7220 3d20 456d 6265 6464  culator = Embedd
+000043e0: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+000043f0: 5f6b 6579 733d 2822 7061 7468 7322 2c29  _keys=("paths",)
+00004400: 290a 6361 6c63 756c 6174 6f72 2e73 6574  ).calculator.set
+00004410: 7570 286e 756d 5f73 616d 706c 6573 3d6c  up(num_samples=l
+00004420: 656e 2876 616c 5f64 6174 6173 6574 2929  en(val_dataset))
+00004430: 0a0a 7769 7468 2074 6f72 6368 2e6e 6f5f  ..with torch.no_
+00004440: 6772 6164 2829 3a0a 2020 2020 666f 7220  grad():.    for 
+00004450: 6261 7463 6820 696e 2074 7164 6d28 7661  batch in tqdm(va
+00004460: 6c5f 6c6f 6164 6572 293a 0a20 2020 2020  l_loader):.     
+00004470: 2020 2062 6174 6368 5b22 656d 6265 6464     batch["embedd
+00004480: 696e 6773 225d 203d 2065 7874 7261 6374  ings"] = extract
+00004490: 6f72 2862 6174 6368 5b22 696e 7075 745f  or(batch["input_
+000044a0: 7465 6e73 6f72 7322 5d29 0a20 2020 2020  tensors"]).     
+000044b0: 2020 2063 616c 6375 6c61 746f 722e 7570     calculator.up
+000044c0: 6461 7465 5f64 6174 6128 6261 7463 6829  date_data(batch)
+000044d0: 0a0a 6d65 7472 6963 7320 3d20 6361 6c63  ..metrics = calc
+000044e0: 756c 6174 6f72 2e63 6f6d 7075 7465 5f6d  ulator.compute_m
+000044f0: 6574 7269 6373 2829 0a0a 2320 4c6f 6767  etrics()..# Logg
+00004500: 696e 670a 7072 696e 7428 6361 6c63 756c  ing.print(calcul
+00004510: 6174 6f72 2e6d 6574 7269 6373 2920 2023  ator.metrics)  #
+00004520: 206d 6574 7269 6373 0a70 7269 6e74 2863   metrics.print(c
+00004530: 616c 6375 6c61 746f 722e 6d65 7472 6963  alculator.metric
+00004540: 735f 756e 7265 6475 6365 6429 2020 2320  s_unreduced)  # 
+00004550: 6d65 7472 6963 7320 7769 7468 6f75 7420  metrics without 
+00004560: 6176 6572 6167 696e 6720 6f76 6572 2071  averaging over q
+00004570: 7565 7269 6573 0a0a 2320 5669 7375 616c  ueries..# Visual
+00004580: 6973 6174 696f 6e0a 6361 6c63 756c 6174  isation.calculat
+00004590: 6f72 2e67 6574 5f70 6c6f 745f 666f 725f  or.get_plot_for_
+000045a0: 7175 6572 6965 7328 7175 6572 795f 6964  queries(query_id
+000045b0: 733d 5b30 2c20 325d 2c20 6e5f 696e 7374  s=[0, 2], n_inst
+000045c0: 616e 6365 733d 3529 2020 2320 6472 6177  ances=5)  # draw
+000045d0: 2070 7265 6469 6374 696f 6e73 206f 6e20   predictions on 
+000045e0: 7072 6564 6566 696e 6564 2071 7565 7269  predefined queri
+000045f0: 6573 0a63 616c 6375 6c61 746f 722e 6765  es.calculator.ge
+00004600: 745f 706c 6f74 5f66 6f72 5f77 6f72 7374  t_plot_for_worst
+00004610: 5f71 7565 7269 6573 286d 6574 7269 635f  _queries(metric_
+00004620: 6e61 6d65 3d22 4f56 4552 414c 4c2f 6d61  name="OVERALL/ma
+00004630: 702f 3522 2c20 6e5f 7175 6572 6965 733d  p/5", n_queries=
+00004640: 322c 206e 5f69 6e73 7461 6e63 6573 3d35  2, n_instances=5
+00004650: 2920 2023 2064 7261 7720 6d69 7374 616b  )  # draw mistak
+00004660: 6573 0a63 616c 6375 6c61 746f 722e 7669  es.calculator.vi
+00004670: 7375 616c 697a 6528 2920 2023 2064 7261  sualize()  # dra
+00004680: 7720 6d69 7374 616b 6573 2066 6f72 2061  w mistakes for a
+00004690: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+000046a0: 206d 6574 7269 6373 0a0a 6060 600a 5b63   metrics..```.[c
+000046b0: 6f6d 6d65 6e74 5d3a 7661 6e69 6c6c 612d  omment]:vanilla-
+000046c0: 7661 6c69 6461 7469 6f6e 2d65 6e64 0a3c  validation-end.<
+000046d0: 2f70 3e0a 3c2f 6465 7461 696c 733e 0a0a  /p>.</details>..
+000046e0: 5b21 5b4f 7065 6e20 496e 2043 6f6c 6162  [![Open In Colab
+000046f0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00004700: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00004710: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00004720: 2d62 6164 6765 2e73 7667 295d 2868 7474  -badge.svg)](htt
+00004730: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004740: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
+00004750: 7269 7665 2f31 4f32 6f33 6b38 4938 6a4e  rive/1O2o3k8I8jN
+00004760: 3568 5269 6e33 644b 6e41 5333 5773 6747  5hRin3dKnAS3WsgG
+00004770: 3034 746d 4954 3f75 7370 3d73 6861 7269  04tmIT?usp=shari
+00004780: 6e67 290a 3c64 6574 6169 6c73 3e0a 3c73  ng).<details>.<s
+00004790: 756d 6d61 7279 3e54 7261 696e 696e 6720  ummary>Training 
+000047a0: 2b20 5661 6c69 6461 7469 6f6e 205b 4c69  + Validation [Li
+000047b0: 6768 746e 696e 6720 616e 6420 6c6f 6767  ghtning and logg
+000047c0: 696e 675d 3c2f 7375 6d6d 6172 793e 0a3c  ing]</summary>.<
+000047d0: 703e 0a0a 5b63 6f6d 6d65 6e74 5d3a 6c69  p>..[comment]:li
+000047e0: 6768 746e 696e 672d 7374 6172 740a 6060  ghtning-start.``
+000047f0: 6070 7974 686f 6e0a 696d 706f 7274 2070  `python.import p
+00004800: 7974 6f72 6368 5f6c 6967 6874 6e69 6e67  ytorch_lightning
+00004810: 2061 7320 706c 0a69 6d70 6f72 7420 746f   as pl.import to
+00004820: 7263 680a 0a66 726f 6d20 6f6d 6c2e 6461  rch..from oml.da
+00004830: 7461 7365 7473 2e62 6173 6520 696d 706f  tasets.base impo
+00004840: 7274 2044 6174 6173 6574 5175 6572 7947  rt DatasetQueryG
+00004850: 616c 6c65 7279 2c20 4461 7461 7365 7457  allery, DatasetW
+00004860: 6974 684c 6162 656c 730a 6672 6f6d 206f  ithLabels.from o
+00004870: 6d6c 2e6c 6967 6874 6e69 6e67 2e6d 6f64  ml.lightning.mod
+00004880: 756c 6573 2e65 7874 7261 6374 6f72 2069  ules.extractor i
+00004890: 6d70 6f72 7420 4578 7472 6163 746f 724d  mport ExtractorM
+000048a0: 6f64 756c 650a 6672 6f6d 206f 6d6c 2e6c  odule.from oml.l
+000048b0: 6967 6874 6e69 6e67 2e63 616c 6c62 6163  ightning.callbac
+000048c0: 6b73 2e6d 6574 7269 6320 696d 706f 7274  ks.metric import
+000048d0: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+000048e0: 636b 0a66 726f 6d20 6f6d 6c2e 6c6f 7373  ck.from oml.loss
+000048f0: 6573 2e74 7269 706c 6574 2069 6d70 6f72  es.triplet impor
+00004900: 7420 5472 6970 6c65 744c 6f73 7357 6974  t TripletLossWit
+00004910: 684d 696e 6572 0a66 726f 6d20 6f6d 6c2e  hMiner.from oml.
+00004920: 6d65 7472 6963 732e 656d 6265 6464 696e  metrics.embeddin
+00004930: 6773 2069 6d70 6f72 7420 456d 6265 6464  gs import Embedd
+00004940: 696e 674d 6574 7269 6373 0a66 726f 6d20  ingMetrics.from 
+00004950: 6f6d 6c2e 6d69 6e65 7273 2e69 6e62 6174  oml.miners.inbat
+00004960: 6368 5f61 6c6c 5f74 7269 2069 6d70 6f72  ch_all_tri impor
+00004970: 7420 416c 6c54 7269 706c 6574 734d 696e  t AllTripletsMin
+00004980: 6572 0a66 726f 6d20 6f6d 6c2e 6d6f 6465  er.from oml.mode
+00004990: 6c73 2069 6d70 6f72 7420 5669 5445 7874  ls import ViTExt
+000049a0: 7261 6374 6f72 0a66 726f 6d20 6f6d 6c2e  ractor.from oml.
+000049b0: 7361 6d70 6c65 7273 2e62 616c 616e 6365  samplers.balance
+000049c0: 2069 6d70 6f72 7420 4261 6c61 6e63 6553   import BalanceS
+000049d0: 616d 706c 6572 0a66 726f 6d20 6f6d 6c2e  ampler.from oml.
+000049e0: 7574 696c 732e 646f 776e 6c6f 6164 5f6d  utils.download_m
+000049f0: 6f63 6b5f 6461 7461 7365 7420 696d 706f  ock_dataset impo
+00004a00: 7274 2064 6f77 6e6c 6f61 645f 6d6f 636b  rt download_mock
+00004a10: 5f64 6174 6173 6574 0a66 726f 6d20 7079  _dataset.from py
+00004a20: 746f 7263 685f 6c69 6768 746e 696e 672e  torch_lightning.
+00004a30: 6c6f 6767 6572 7320 696d 706f 7274 204e  loggers import N
+00004a40: 6570 7475 6e65 4c6f 6767 6572 2c20 5465  eptuneLogger, Te
+00004a50: 6e73 6f72 426f 6172 644c 6f67 6765 722c  nsorBoardLogger,
+00004a60: 2057 616e 6462 4c6f 6767 6572 0a0a 6461   WandbLogger..da
+00004a70: 7461 7365 745f 726f 6f74 203d 2022 6d6f  taset_root = "mo
+00004a80: 636b 5f64 6174 6173 6574 2f22 0a64 665f  ck_dataset/".df_
+00004a90: 7472 6169 6e2c 2064 665f 7661 6c20 3d20  train, df_val = 
+00004aa0: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+00004ab0: 7461 7365 7428 6461 7461 7365 745f 726f  taset(dataset_ro
+00004ac0: 6f74 290a 0a23 206d 6f64 656c 0a65 7874  ot)..# model.ext
+00004ad0: 7261 6374 6f72 203d 2056 6954 4578 7472  ractor = ViTExtr
+00004ae0: 6163 746f 7228 2276 6974 7331 365f 6469  actor("vits16_di
+00004af0: 6e6f 222c 2061 7263 683d 2276 6974 7331  no", arch="vits1
+00004b00: 3622 2c20 6e6f 726d 616c 6973 655f 6665  6", normalise_fe
+00004b10: 6174 7572 6573 3d46 616c 7365 290a 0a23  atures=False)..#
+00004b20: 2074 7261 696e 0a6f 7074 696d 697a 6572   train.optimizer
+00004b30: 203d 2074 6f72 6368 2e6f 7074 696d 2e53   = torch.optim.S
+00004b40: 4744 2865 7874 7261 6374 6f72 2e70 6172  GD(extractor.par
+00004b50: 616d 6574 6572 7328 292c 206c 723d 3165  ameters(), lr=1e
+00004b60: 2d36 290a 7472 6169 6e5f 6461 7461 7365  -6).train_datase
+00004b70: 7420 3d20 4461 7461 7365 7457 6974 684c  t = DatasetWithL
+00004b80: 6162 656c 7328 6466 5f74 7261 696e 2c20  abels(df_train, 
+00004b90: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00004ba0: 6173 6574 5f72 6f6f 7429 0a63 7269 7465  aset_root).crite
+00004bb0: 7269 6f6e 203d 2054 7269 706c 6574 4c6f  rion = TripletLo
+00004bc0: 7373 5769 7468 4d69 6e65 7228 6d61 7267  ssWithMiner(marg
+00004bd0: 696e 3d30 2e31 2c20 6d69 6e65 723d 416c  in=0.1, miner=Al
+00004be0: 6c54 7269 706c 6574 734d 696e 6572 2829  lTripletsMiner()
+00004bf0: 290a 6261 7463 685f 7361 6d70 6c65 7220  ).batch_sampler 
+00004c00: 3d20 4261 6c61 6e63 6553 616d 706c 6572  = BalanceSampler
+00004c10: 2874 7261 696e 5f64 6174 6173 6574 2e67  (train_dataset.g
+00004c20: 6574 5f6c 6162 656c 7328 292c 206e 5f6c  et_labels(), n_l
+00004c30: 6162 656c 733d 322c 206e 5f69 6e73 7461  abels=2, n_insta
+00004c40: 6e63 6573 3d33 290a 7472 6169 6e5f 6c6f  nces=3).train_lo
+00004c50: 6164 6572 203d 2074 6f72 6368 2e75 7469  ader = torch.uti
+00004c60: 6c73 2e64 6174 612e 4461 7461 4c6f 6164  ls.data.DataLoad
+00004c70: 6572 2874 7261 696e 5f64 6174 6173 6574  er(train_dataset
+00004c80: 2c20 6261 7463 685f 7361 6d70 6c65 723d  , batch_sampler=
+00004c90: 6261 7463 685f 7361 6d70 6c65 7229 0a0a  batch_sampler)..
+00004ca0: 2320 7661 6c0a 7661 6c5f 6461 7461 7365  # val.val_datase
+00004cb0: 7420 3d20 4461 7461 7365 7451 7565 7279  t = DatasetQuery
+00004cc0: 4761 6c6c 6572 7928 6466 5f76 616c 2c20  Gallery(df_val, 
+00004cd0: 6461 7461 7365 745f 726f 6f74 3d64 6174  dataset_root=dat
+00004ce0: 6173 6574 5f72 6f6f 7429 0a76 616c 5f6c  aset_root).val_l
+00004cf0: 6f61 6465 7220 3d20 746f 7263 682e 7574  oader = torch.ut
+00004d00: 696c 732e 6461 7461 2e44 6174 614c 6f61  ils.data.DataLoa
+00004d10: 6465 7228 7661 6c5f 6461 7461 7365 742c  der(val_dataset,
+00004d20: 2062 6174 6368 5f73 697a 653d 3429 0a6d   batch_size=4).m
+00004d30: 6574 7269 635f 6361 6c6c 6261 636b 203d  etric_callback =
+00004d40: 204d 6574 7269 6356 616c 4361 6c6c 6261   MetricValCallba
+00004d50: 636b 286d 6574 7269 633d 456d 6265 6464  ck(metric=Embedd
+00004d60: 696e 674d 6574 7269 6373 2865 7874 7261  ingMetrics(extra
+00004d70: 5f6b 6579 733d 5b74 7261 696e 5f64 6174  _keys=[train_dat
+00004d80: 6173 6574 2e70 6174 6873 5f6b 6579 2c5d  aset.paths_key,]
+00004d90: 292c 206c 6f67 5f69 6d61 6765 733d 5472  ), log_images=Tr
+00004da0: 7565 290a 0a23 2031 2920 4c6f 6767 696e  ue)..# 1) Loggin
+00004db0: 6720 7769 7468 2054 656e 736f 7262 6f61  g with Tensorboa
+00004dc0: 7264 0a6c 6f67 6765 7220 3d20 5465 6e73  rd.logger = Tens
+00004dd0: 6f72 426f 6172 644c 6f67 6765 7228 222e  orBoardLogger(".
+00004de0: 2229 0a0a 2320 3229 204c 6f67 6769 6e67  ")..# 2) Logging
+00004df0: 2077 6974 6820 4e65 7074 756e 650a 2320   with Neptune.# 
+00004e00: 6c6f 6767 6572 203d 204e 6570 7475 6e65  logger = Neptune
+00004e10: 4c6f 6767 6572 2861 7069 5f6b 6579 3d22  Logger(api_key="
+00004e20: 222c 2070 726f 6a65 6374 3d22 222c 206c  ", project="", l
+00004e30: 6f67 5f6d 6f64 656c 5f63 6865 636b 706f  og_model_checkpo
+00004e40: 696e 7473 3d46 616c 7365 290a 0a23 2033  ints=False)..# 3
+00004e50: 2920 4c6f 6767 696e 6720 7769 7468 2057  ) Logging with W
+00004e60: 6569 6768 7473 2061 6e64 2042 6961 7365  eights and Biase
+00004e70: 730a 2320 696d 706f 7274 206f 730a 2320  s.# import os.# 
+00004e80: 6f73 2e65 6e76 6972 6f6e 5b22 5741 4e44  os.environ["WAND
+00004e90: 425f 4150 495f 4b45 5922 5d20 3d20 2222  B_API_KEY"] = ""
+00004ea0: 0a23 206c 6f67 6765 7220 3d20 5761 6e64  .# logger = Wand
+00004eb0: 624c 6f67 6765 7228 7072 6f6a 6563 743d  bLogger(project=
+00004ec0: 2274 6573 745f 7072 6f6a 6563 7422 2c20  "test_project", 
+00004ed0: 6c6f 675f 6d6f 6465 6c3d 4661 6c73 6529  log_model=False)
+00004ee0: 0a0a 2320 7275 6e0a 706c 5f6d 6f64 656c  ..# run.pl_model
+00004ef0: 203d 2045 7874 7261 6374 6f72 4d6f 6475   = ExtractorModu
+00004f00: 6c65 2865 7874 7261 6374 6f72 2c20 6372  le(extractor, cr
+00004f10: 6974 6572 696f 6e2c 206f 7074 696d 697a  iterion, optimiz
+00004f20: 6572 290a 7472 6169 6e65 7220 3d20 706c  er).trainer = pl
+00004f30: 2e54 7261 696e 6572 286d 6178 5f65 706f  .Trainer(max_epo
+00004f40: 6368 733d 332c 2063 616c 6c62 6163 6b73  chs=3, callbacks
+00004f50: 3d5b 6d65 7472 6963 5f63 616c 6c62 6163  =[metric_callbac
+00004f60: 6b5d 2c20 6e75 6d5f 7361 6e69 7479 5f76  k], num_sanity_v
+00004f70: 616c 5f73 7465 7073 3d30 2c20 6c6f 6767  al_steps=0, logg
+00004f80: 6572 3d6c 6f67 6765 7229 0a74 7261 696e  er=logger).train
+00004f90: 6572 2e66 6974 2870 6c5f 6d6f 6465 6c2c  er.fit(pl_model,
+00004fa0: 2074 7261 696e 5f64 6174 616c 6f61 6465   train_dataloade
+00004fb0: 7273 3d74 7261 696e 5f6c 6f61 6465 722c  rs=train_loader,
+00004fc0: 2076 616c 5f64 6174 616c 6f61 6465 7273   val_dataloaders
+00004fd0: 3d76 616c 5f6c 6f61 6465 7229 0a0a 6060  =val_loader)..``
+00004fe0: 600a 5b63 6f6d 6d65 6e74 5d3a 6c69 6768  `.[comment]:ligh
+00004ff0: 746e 696e 672d 656e 640a 3c2f 703e 0a3c  tning-end.</p>.<
+00005000: 2f64 6574 6169 6c73 3e0a 0a5b 215b 4f70  /details>..[![Op
+00005010: 656e 2049 6e20 436f 6c61 625d 2868 7474  en In Colab](htt
+00005020: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00005030: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+00005040: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+00005050: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00005060: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00005070: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
+00005080: 3162 5655 6764 4247 5776 5167 436b 6261  1bVUgdBGWvQgCkba
+00005090: 3259 7461 4952 566c 5551 557a 3751 3630  2YtaIRVlUQUz7Q60
+000050a0: 5a3f 7573 703d 7368 6172 655f 6c69 6e6b  Z?usp=share_link
+000050b0: 290a 3c64 6574 6169 6c73 3e0a 3c73 756d  ).<details>.<sum
+000050c0: 6d61 7279 3e55 7369 6e67 2061 2074 7261  mary>Using a tra
+000050d0: 696e 6564 206d 6f64 656c 2066 6f72 2072  ined model for r
+000050e0: 6574 7269 6576 616c 3c2f 7375 6d6d 6172  etrieval</summar
+000050f0: 793e 0a3c 703e 0a0a 5b63 6f6d 6d65 6e74  y>.<p>..[comment
+00005100: 5d3a 7573 6167 652d 7265 7472 6965 7661  ]:usage-retrieva
+00005110: 6c2d 7374 6172 740a 6060 6070 7974 686f  l-start.```pytho
+00005120: 6e0a 696d 706f 7274 2074 6f72 6368 0a0a  n.import torch..
+00005130: 6672 6f6d 206f 6d6c 2e63 6f6e 7374 2069  from oml.const i
+00005140: 6d70 6f72 7420 4d4f 434b 5f44 4154 4153  mport MOCK_DATAS
+00005150: 4554 5f50 4154 480a 6672 6f6d 206f 6d6c  ET_PATH.from oml
+00005160: 2e69 6e66 6572 656e 6365 2e66 6c61 7420  .inference.flat 
+00005170: 696d 706f 7274 2069 6e66 6572 656e 6365  import inference
+00005180: 5f6f 6e5f 696d 6167 6573 0a66 726f 6d20  _on_images.from 
+00005190: 6f6d 6c2e 6d6f 6465 6c73 2069 6d70 6f72  oml.models impor
+000051a0: 7420 5669 5445 7874 7261 6374 6f72 0a66  t ViTExtractor.f
+000051b0: 726f 6d20 6f6d 6c2e 7265 6769 7374 7279  rom oml.registry
+000051c0: 2e74 7261 6e73 666f 726d 7320 696d 706f  .transforms impo
+000051d0: 7274 2067 6574 5f74 7261 6e73 666f 726d  rt get_transform
+000051e0: 735f 666f 725f 7072 6574 7261 696e 6564  s_for_pretrained
+000051f0: 0a66 726f 6d20 6f6d 6c2e 7574 696c 732e  .from oml.utils.
+00005200: 646f 776e 6c6f 6164 5f6d 6f63 6b5f 6461  download_mock_da
+00005210: 7461 7365 7420 696d 706f 7274 2064 6f77  taset import dow
+00005220: 6e6c 6f61 645f 6d6f 636b 5f64 6174 6173  nload_mock_datas
+00005230: 6574 0a66 726f 6d20 6f6d 6c2e 7574 696c  et.from oml.util
+00005240: 732e 6d69 7363 5f74 6f72 6368 2069 6d70  s.misc_torch imp
+00005250: 6f72 7420 7061 6972 7769 7365 5f64 6973  ort pairwise_dis
+00005260: 740a 0a5f 2c20 6466 5f76 616c 203d 2064  t.._, df_val = d
+00005270: 6f77 6e6c 6f61 645f 6d6f 636b 5f64 6174  ownload_mock_dat
+00005280: 6173 6574 284d 4f43 4b5f 4441 5441 5345  aset(MOCK_DATASE
+00005290: 545f 5041 5448 290a 6466 5f76 616c 5b22  T_PATH).df_val["
+000052a0: 7061 7468 225d 203d 2064 665f 7661 6c5b  path"] = df_val[
+000052b0: 2270 6174 6822 5d2e 6170 706c 7928 6c61  "path"].apply(la
+000052c0: 6d62 6461 2078 3a20 4d4f 434b 5f44 4154  mbda x: MOCK_DAT
+000052d0: 4153 4554 5f50 4154 4820 2f20 7829 0a71  ASET_PATH / x).q
+000052e0: 7565 7269 6573 203d 2064 665f 7661 6c5b  ueries = df_val[
+000052f0: 6466 5f76 616c 5b22 6973 5f71 7565 7279  df_val["is_query
+00005300: 225d 5d5b 2270 6174 6822 5d2e 746f 6c69  "]]["path"].toli
+00005310: 7374 2829 0a67 616c 6c65 7269 6573 203d  st().galleries =
+00005320: 2064 665f 7661 6c5b 6466 5f76 616c 5b22   df_val[df_val["
+00005330: 6973 5f67 616c 6c65 7279 225d 5d5b 2270  is_gallery"]]["p
+00005340: 6174 6822 5d2e 746f 6c69 7374 2829 0a0a  ath"].tolist()..
+00005350: 6578 7472 6163 746f 7220 3d20 5669 5445  extractor = ViTE
+00005360: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00005370: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00005380: 5f64 696e 6f22 290a 7472 616e 7366 6f72  _dino").transfor
+00005390: 6d2c 205f 203d 2067 6574 5f74 7261 6e73  m, _ = get_trans
+000053a0: 666f 726d 735f 666f 725f 7072 6574 7261  forms_for_pretra
+000053b0: 696e 6564 2822 7669 7473 3136 5f64 696e  ined("vits16_din
+000053c0: 6f22 290a 0a61 7267 7320 3d20 7b22 6e75  o")..args = {"nu
+000053d0: 6d5f 776f 726b 6572 7322 3a20 302c 2022  m_workers": 0, "
+000053e0: 6261 7463 685f 7369 7a65 223a 2038 7d0a  batch_size": 8}.
+000053f0: 6665 6174 7572 6573 5f71 7565 7269 6573  features_queries
+00005400: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+00005410: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+00005420: 2c20 7061 7468 733d 7175 6572 6965 732c  , paths=queries,
+00005430: 2074 7261 6e73 666f 726d 3d74 7261 6e73   transform=trans
+00005440: 666f 726d 2c20 2a2a 6172 6773 290a 6665  form, **args).fe
+00005450: 6174 7572 6573 5f67 616c 6c65 7269 6573  atures_galleries
+00005460: 203d 2069 6e66 6572 656e 6365 5f6f 6e5f   = inference_on_
+00005470: 696d 6167 6573 2865 7874 7261 6374 6f72  images(extractor
+00005480: 2c20 7061 7468 733d 6761 6c6c 6572 6965  , paths=gallerie
+00005490: 732c 2074 7261 6e73 666f 726d 3d74 7261  s, transform=tra
+000054a0: 6e73 666f 726d 2c20 2a2a 6172 6773 290a  nsform, **args).
+000054b0: 0a23 204e 6f77 2077 6520 6361 6e20 6578  .# Now we can ex
+000054c0: 706c 6963 6974 6c79 2062 7569 6c64 2070  plicitly build p
+000054d0: 6169 7277 6973 6520 6d61 7472 6978 206f  airwise matrix o
+000054e0: 6620 6469 7374 616e 6365 7320 6f72 2073  f distances or s
+000054f0: 6176 6520 796f 7520 5241 4d20 7669 6120  ave you RAM via 
+00005500: 7573 696e 6720 6b4e 4e0a 7573 655f 6b6e  using kNN.use_kn
+00005510: 6e20 3d20 5472 7565 0a74 6f70 5f6b 203d  n = True.top_k =
+00005520: 2033 0a0a 6966 2075 7365 5f6b 6e6e 3a0a   3..if use_knn:.
+00005530: 2020 2020 6672 6f6d 2073 6b6c 6561 726e      from sklearn
+00005540: 2e6e 6569 6768 626f 7273 2069 6d70 6f72  .neighbors impor
+00005550: 7420 4e65 6172 6573 744e 6569 6768 626f  t NearestNeighbo
+00005560: 7273 0a20 2020 206b 6e6e 203d 204e 6561  rs.    knn = Nea
+00005570: 7265 7374 4e65 6967 6862 6f72 7328 616c  restNeighbors(al
+00005580: 676f 7269 7468 6d3d 2261 7574 6f22 2c20  gorithm="auto", 
+00005590: 703d 3229 0a20 2020 206b 6e6e 2e66 6974  p=2).    knn.fit
+000055a0: 2866 6561 7475 7265 735f 6761 6c6c 6572  (features_galler
+000055b0: 6965 7329 0a20 2020 2064 6973 7473 2c20  ies).    dists, 
+000055c0: 6969 5f63 6c6f 7365 7374 203d 206b 6e6e  ii_closest = knn
+000055d0: 2e6b 6e65 6967 6862 6f72 7328 6665 6174  .kneighbors(feat
+000055e0: 7572 6573 5f71 7565 7269 6573 2c20 6e5f  ures_queries, n_
+000055f0: 6e65 6967 6862 6f72 733d 746f 705f 6b2c  neighbors=top_k,
+00005600: 2072 6574 7572 6e5f 6469 7374 616e 6365   return_distance
+00005610: 3d54 7275 6529 0a0a 656c 7365 3a0a 2020  =True)..else:.  
+00005620: 2020 6469 7374 5f6d 6174 203d 2070 6169    dist_mat = pai
+00005630: 7277 6973 655f 6469 7374 2878 313d 6665  rwise_dist(x1=fe
+00005640: 6174 7572 6573 5f71 7565 7269 6573 2c20  atures_queries, 
+00005650: 7832 3d66 6561 7475 7265 735f 6761 6c6c  x2=features_gall
+00005660: 6572 6965 7329 0a20 2020 2064 6973 7473  eries).    dists
+00005670: 2c20 6969 5f63 6c6f 7365 7374 203d 2074  , ii_closest = t
+00005680: 6f72 6368 2e74 6f70 6b28 6469 7374 5f6d  orch.topk(dist_m
+00005690: 6174 2c20 6469 6d3d 312c 206b 3d74 6f70  at, dim=1, k=top
+000056a0: 5f6b 2c20 6c61 7267 6573 743d 4661 6c73  _k, largest=Fals
+000056b0: 6529 0a0a 7072 696e 7428 6622 546f 7020  e)..print(f"Top 
+000056c0: 7b74 6f70 5f6b 7d20 6974 656d 7320 636c  {top_k} items cl
+000056d0: 6f73 6573 7420 746f 2071 7565 7269 6573  osest to queries
+000056e0: 2061 7265 3a5c 6e20 7b69 695f 636c 6f73   are:\n {ii_clos
+000056f0: 6573 747d 2229 0a60 6060 0a5b 636f 6d6d  est}").```.[comm
+00005700: 656e 745d 3a75 7361 6765 2d72 6574 7269  ent]:usage-retri
+00005710: 6576 616c 2d65 6e64 0a3c 2f70 3e0a 3c2f  eval-end.</p>.</
+00005720: 6465 7461 696c 733e 0a0a 5b21 5b4f 7065  details>..[![Ope
+00005730: 6e20 496e 2043 6f6c 6162 5d28 6874 7470  n In Colab](http
+00005740: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00005750: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
+00005760: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
+00005770: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
+00005780: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00005790: 6f67 6c65 2e63 6f6d 2f64 7269 7665 2f31  ogle.com/drive/1
+000057a0: 5332 6e4b 364b 6152 6544 6d2d 526a 6a64  S2nK6KaReDm-Rjjd
+000057b0: 6f6a 6449 6436 4361 6b68 6853 7976 6641  ojdId6CakhhSyvfA
+000057c0: 3f75 7370 3d73 6861 7265 5f6c 696e 6b29  ?usp=share_link)
+000057d0: 0a0a 5b2a 2a53 6368 656d 6173 2c20 6578  ..[**Schemas, ex
+000057e0: 706c 616e 6174 696f 6e73 2061 6e64 2074  planations and t
+000057f0: 6970 732a 2a5d 2868 7474 7073 3a2f 2f67  ips**](https://g
+00005800: 6974 6875 622e 636f 6d2f 4f4d 4c2d 5465  ithub.com/OML-Te
+00005810: 616d 2f6f 7065 6e2d 6d65 7472 6963 2d6c  am/open-metric-l
+00005820: 6561 726e 696e 672f 7472 6565 2f6d 6169  earning/tree/mai
+00005830: 6e2f 7069 7065 6c69 6e65 732f 6665 6174  n/pipelines/feat
+00005840: 7572 6573 5f65 7874 7261 6374 696f 6e29  ures_extraction)
+00005850: 0a0a 5365 6520 5b65 7874 7261 2063 6f64  ..See [extra cod
+00005860: 6520 736e 6970 7065 7473 5d28 6874 7470  e snippets](http
+00005870: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00005880: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00005890: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000058a0: 742f 6665 6174 7572 655f 6578 7472 6163  t/feature_extrac
+000058b0: 7469 6f6e 2f70 7974 686f 6e5f 6578 616d  tion/python_exam
+000058c0: 706c 6573 2e68 746d 6c29 2c20 696e 636c  ples.html), incl
+000058d0: 7564 696e 673a 0a2a 2054 7261 696e 696e  uding:.* Trainin
+000058e0: 6720 2b20 5661 6c69 6461 7469 6f6e 2077  g + Validation w
+000058f0: 6974 6820 4c69 6768 746e 696e 670a 2a20  ith Lightning.* 
+00005900: 5472 6169 6e69 6e67 202b 2056 616c 6964  Training + Valid
+00005910: 6174 696f 6e20 7769 7468 204c 6967 6874  ation with Light
+00005920: 6e69 6e67 2069 6e20 4444 5020 6d6f 6465  ning in DDP mode
+00005930: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005940: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005950: 0a2a 2054 7261 696e 696e 6720 7769 7468  .* Training with
+00005960: 206c 6f73 7365 7320 6672 6f6d 2050 4d4c   losses from PML
+00005970: 2061 6476 616e 6365 6420 2870 6173 7369   advanced (passi
+00005980: 6e67 2064 6973 7461 6e63 652c 2072 6564  ng distance, red
+00005990: 7563 6572 2c20 6d69 6e65 7229 0a0a 2323  ucer, miner)..##
+000059a0: 205b 5069 7065 6c69 6e65 735d 2868 7474   [Pipelines](htt
+000059b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000059c0: 4f4d 4c2d 5465 616d 2f6f 7065 6e2d 6d65  OML-Team/open-me
+000059d0: 7472 6963 2d6c 6561 726e 696e 672f 7472  tric-learning/tr
+000059e0: 6565 2f6d 6169 6e2f 7069 7065 6c69 6e65  ee/main/pipeline
+000059f0: 7329 0a0a 5069 7065 6c69 6e65 7320 7072  s)..Pipelines pr
+00005a00: 6f76 6964 6520 6120 7761 7920 746f 2072  ovide a way to r
+00005a10: 756e 206d 6574 7269 6320 6c65 6172 6e69  un metric learni
+00005a20: 6e67 2065 7870 6572 696d 656e 7473 2076  ng experiments v
+00005a30: 6961 2063 6861 6e67 696e 6720 6f6e 6c79  ia changing only
+00005a40: 2074 6865 2063 6f6e 6669 6720 6669 6c65   the config file
+00005a50: 2e0a 416c 6c20 796f 7520 6e65 6564 2069  ..All you need i
+00005a60: 7320 746f 2070 7265 7061 7265 2079 6f75  s to prepare you
+00005a70: 7220 6461 7461 7365 7420 696e 2061 2072  r dataset in a r
+00005a80: 6571 7569 7265 6420 666f 726d 6174 2e0a  equired format..
+00005a90: 0a53 6565 205b 5069 7065 6c69 6e65 735d  .See [Pipelines]
+00005aa0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00005ab0: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
+00005ac0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
+00005ad0: 672f 626c 6f62 2f6d 6169 6e2f 7069 7065  g/blob/main/pipe
+00005ae0: 6c69 6e65 732f 2920 666f 6c64 6572 2066  lines/) folder f
+00005af0: 6f72 206d 6f72 6520 6465 7461 696c 733a  or more details:
+00005b00: 0a2a 2046 6561 7475 7265 2065 7874 7261  .* Feature extra
+00005b10: 6374 6f72 205b 7069 7065 6c69 6e65 5d28  ctor [pipeline](
+00005b20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00005b30: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
+00005b40: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
+00005b50: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
+00005b60: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
+00005b70: 7472 6163 7469 6f6e 290a 2a20 5265 7472  traction).* Retr
+00005b80: 6965 7661 6c20 706f 7374 7072 6f63 6573  ieval postproces
+00005b90: 736f 7220 5b70 6970 656c 696e 655d 2868  sor [pipeline](h
+00005ba0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00005bb0: 6d2f 4f4d 4c2d 5465 616d 2f6f 7065 6e2d  m/OML-Team/open-
+00005bc0: 6d65 7472 6963 2d6c 6561 726e 696e 672f  metric-learning/
+00005bd0: 7472 6565 2f6d 6169 6e2f 7069 7065 6c69  tree/main/pipeli
+00005be0: 6e65 732f 706f 7374 7072 6f63 6573 7369  nes/postprocessi
+00005bf0: 6e67 2920 2872 652d 7261 6e6b 696e 6729  ng) (re-ranking)
+00005c00: 0a0a 2323 205b 5a6f 6f5d 2868 7474 7073  ..## [Zoo](https
+00005c10: 3a2f 2f6f 7065 6e2d 6d65 7472 6963 2d6c  ://open-metric-l
+00005c20: 6561 726e 696e 672e 7265 6164 7468 6564  earning.readthed
+00005c30: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00005c40: 2f66 6561 7475 7265 5f65 7874 7261 6374  /feature_extract
+00005c50: 696f 6e2f 7a6f 6f2e 6874 6d6c 290a 0a42  ion/zoo.html)..B
+00005c60: 656c 6f77 2061 7265 2074 6865 206d 6f64  elow are the mod
+00005c70: 656c 7320 7472 6169 6e65 6420 7769 7468  els trained with
+00005c80: 204f 4d4c 206f 6e20 3420 7075 626c 6963   OML on 4 public
+00005c90: 2064 6174 6173 6574 732e 0a41 6c6c 206d   datasets..All m
+00005ca0: 6574 7269 6373 2062 656c 6f77 2077 6572  etrics below wer
+00005cb0: 6520 6f62 7461 696e 6564 206f 6e20 7468  e obtained on th
+00005cc0: 6520 696d 6167 6573 2077 6974 6820 7468  e images with th
+00005cd0: 6520 7369 7a65 7320 6f66 202a 2a32 3234  e sizes of **224
+00005ce0: 2078 2032 3234 2a2a 3a0a 0a7c 2020 2020   x 224**:..|    
 00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d10: 6578 7065 7269 6d65 6e74 2020 2020 2020  experiment      
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005d50: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
-00005d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d80: 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 3a2d 2d2d  --:|:-----:|:---
-00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005da0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00005db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e00: 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d  ---------:|:----
-00005e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d00: 2020 6d6f 6465 6c20 2020 2020 2020 2020    model         
+00005d10: 2020 2020 2020 2020 2020 2020 207c 2063               | c
+00005d20: 6d63 3120 207c 2020 2020 2020 2020 2064  mc1  |         d
+00005d30: 6174 6173 6574 2020 2020 2020 2020 2020  ataset          
+00005d40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005d70: 6569 6768 7473 2020 2020 2020 2020 2020  eights          
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dd0: 2020 2020 2020 2020 2065 7870 6572 696d           experim
+00005de0: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 2020 2020 2020 2020 7c0a 7c3a 2d2d 2d2d          |.|:----
 00005e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00005e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
-00005e80: 7c20 6056 6954 4578 7472 6163 746f 722e  | `ViTExtractor.
-00005e90: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005ea0: 2276 6974 7331 365f 696e 7368 6f70 2229  "vits16_inshop")
-00005eb0: 6020 7c20 302e 3932 3120 7c20 2020 2044  ` | 0.921 |    D
-00005ec0: 6565 7046 6173 6869 6f6e 2049 6e73 686f  eepFashion Insho
-00005ed0: 7020 2020 207c 2020 2020 5b6c 696e 6b5d  p    |    [link]
-00005ee0: 2868 7474 7073 3a2f 2f64 7269 7665 2e67  (https://drive.g
-00005ef0: 6f6f 676c 652e 636f 6d2f 6669 6c65 2f64  oogle.com/file/d
-00005f00: 2f31 6e69 582d 5443 3863 6a36 6a33 3639  /1niX-TC8cj6j369
-00005f10: 7437 6955 3262 6148 5153 564e 334d 564a  t7iU2baHQSVN3MVJ
-00005f20: 6257 2f76 6965 773f 7573 703d 7368 6172  bW/view?usp=shar
-00005f30: 696e 6729 2020 2020 207c 205b 6c69 6e6b  ing)     | [link
-00005f40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005f50: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00005f60: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-00005f70: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-00005f80: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-00005f90: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-00005fa0: 6374 6f72 5f69 6e73 686f 7029 207c 0a7c  ctor_inshop) |.|
-00005fb0: 2020 6056 6954 4578 7472 6163 746f 722e    `ViTExtractor.
-00005fc0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00005fd0: 2276 6974 7331 365f 736f 7022 2960 2020  "vits16_sop")`  
-00005fe0: 207c 2030 2e38 3636 207c 2053 7461 6e66   | 0.866 | Stanf
-00005ff0: 6f72 6420 4f6e 6c69 6e65 2050 726f 6475  ord Online Produ
-00006000: 6374 7320 7c20 2020 5b6c 696e 6b5d 2868  cts |   [link](h
-00006010: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-00006020: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
-00006030: 7a75 4752 4876 4632 4b48 6435 3961 7737  zuGRHvF2KHd59aw7
-00006040: 6937 3336 374f 485f 7451 4e4f 477a 3741  i7367OH_tQNOGz7A
-00006050: 2f76 6965 773f 7573 703d 7368 6172 696e  /view?usp=sharin
-00006060: 6729 2020 2020 2020 7c20 205b 6c69 6e6b  g)      |  [link
-00006070: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00006080: 2e63 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70  .com/OML-Team/op
-00006090: 656e 2d6d 6574 7269 632d 6c65 6172 6e69  en-metric-learni
-000060a0: 6e67 2f74 7265 652f 6d61 696e 2f70 6970  ng/tree/main/pip
-000060b0: 656c 696e 6573 2f66 6561 7475 7265 735f  elines/features_
-000060c0: 6578 7472 6163 7469 6f6e 2f65 7874 7261  extraction/extra
-000060d0: 6374 6f72 5f73 6f70 2920 2020 7c0a 7c20  ctor_sop)   |.| 
-000060e0: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-000060f0: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006100: 6974 7331 365f 6361 7273 2229 6020 2020  its16_cars")`   
-00006110: 7c20 302e 3930 3720 7c20 2020 2020 2020  | 0.907 |       
-00006120: 2020 4341 5253 2031 3936 2020 2020 2020    CARS 196      
-00006130: 2020 207c 2020 205b 6c69 6e6b 5d28 6874     |   [link](ht
-00006140: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00006150: 6c65 2e63 6f6d 2f64 7269 7665 2f66 6f6c  le.com/drive/fol
-00006160: 6465 7273 2f31 3761 345f 6667 3934 646f  ders/17a4_fg94do
-00006170: 7832 7366 6b58 6d77 2d4b 4374 694c 426c  x2sfkXmw-KCtiLBl
-00006180: 782d 7574 2d31 3f75 7370 3d73 6861 7269  x-ut-1?usp=shari
-00006190: 6e67 2920 2020 207c 2020 5b6c 696e 6b5d  ng)    |  [link]
-000061a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000061b0: 636f 6d2f 4f4d 4c2d 5465 616d 2f6f 7065  com/OML-Team/ope
-000061c0: 6e2d 6d65 7472 6963 2d6c 6561 726e 696e  n-metric-learnin
-000061d0: 672f 7472 6565 2f6d 6169 6e2f 7069 7065  g/tree/main/pipe
-000061e0: 6c69 6e65 732f 6665 6174 7572 6573 5f65  lines/features_e
-000061f0: 7874 7261 6374 696f 6e2f 6578 7472 6163  xtraction/extrac
-00006200: 746f 725f 6361 7273 2920 207c 0a7c 2020  tor_cars)  |.|  
-00006210: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00006220: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006230: 6974 7331 365f 6375 6222 2960 2020 207c  its16_cub")`   |
-00006240: 2030 2e38 3337 207c 2020 2020 2020 2043   0.837 |       C
-00006250: 5542 2032 3030 2032 3031 3120 2020 2020  UB 200 2011     
-00006260: 2020 7c20 2020 5b6c 696e 6b5d 2868 7474    |   [link](htt
-00006270: 7073 3a2f 2f64 7269 7665 2e67 6f6f 676c  ps://drive.googl
-00006280: 652e 636f 6d2f 6472 6976 652f 666f 6c64  e.com/drive/fold
-00006290: 6572 732f 3154 5043 4e2d 655a 464c 716f  ers/1TPCN-eZFLqo
-000062a0: 7134 4a42 676e 4966 6c69 4a6f 454b 3438  q4JBgnIfliJoEK48
-000062b0: 7839 6f7a 623f 7573 703d 7368 6172 696e  x9ozb?usp=sharin
-000062c0: 6729 2020 2020 7c20 205b 6c69 6e6b 5d28  g)    |  [link](
-000062d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000062e0: 6f6d 2f4f 4d4c 2d54 6561 6d2f 6f70 656e  om/OML-Team/open
-000062f0: 2d6d 6574 7269 632d 6c65 6172 6e69 6e67  -metric-learning
-00006300: 2f74 7265 652f 6d61 696e 2f70 6970 656c  /tree/main/pipel
-00006310: 696e 6573 2f66 6561 7475 7265 735f 6578  ines/features_ex
-00006320: 7472 6163 7469 6f6e 2f65 7874 7261 6374  traction/extract
-00006330: 6f72 5f63 7562 2920 2020 7c0a 0a57 6520  or_cub)   |..We 
-00006340: 616c 736f 2070 726f 7669 6465 2061 6e20  also provide an 
-00006350: 696e 7465 6772 6174 696f 6e20 7769 7468  integration with
-00006360: 2074 6865 206d 6f64 656c 7320 7072 6574   the models pret
-00006370: 7261 696e 6564 2062 7920 6f74 6865 7220  rained by other 
-00006380: 7265 7365 6172 6368 6572 732e 0a41 6c6c  researchers..All
-00006390: 206d 6574 7269 6373 2062 656c 6f77 2077   metrics below w
-000063a0: 6572 6520 6f62 7461 696e 6564 206f 6e20  ere obtained on 
-000063b0: 7468 6520 696d 6167 6573 2077 6974 6820  the images with 
-000063c0: 7468 6520 7369 7a65 7320 6f66 202a 2a32  the sizes of **2
-000063d0: 3234 2078 2032 3234 2a2a 3a0a 0a7c 2020  24 x 224**:..|  
-000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063f0: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2020 2020 2020 2020 7c20 5374              | St
-00006420: 616e 666f 7264 204f 6e6c 696e 6520 5072  anford Online Pr
-00006430: 6f64 7563 7473 207c 2044 6565 7046 6173  oducts | DeepFas
-00006440: 6869 6f6e 2049 6e53 686f 7020 7c20 4355  hion InShop | CU
-00006450: 4220 3230 3020 3230 3131 207c 2043 4152  B 200 2011 | CAR
-00006460: 5320 3139 3620 7c0a 7c3a 2d2d 2d2d 2d2d  S 196 |.|:------
-00006470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064a0: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000064c0: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -:|:------------
-000064d0: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
-000064e0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-000064f0: 3a7c 0a7c 2020 2020 6056 6954 556e 6963  :|.|    `ViTUnic
-00006500: 6f6d 4578 7472 6163 746f 722e 6672 6f6d  omExtractor.from
-00006510: 5f70 7265 7472 6169 6e65 6428 2276 6974  _pretrained("vit
-00006520: 6231 365f 756e 6963 6f6d 2229 6020 2020  b16_unicom")`   
-00006530: 2020 7c20 2020 2020 2020 2020 2030 2e37    |          0.7
-00006540: 3030 2020 2020 2020 2020 2020 207c 2020  00           |  
-00006550: 2020 2020 2030 2e37 3334 2020 2020 2020       0.734      
-00006560: 2020 7c20 2020 2030 2e38 3437 2020 2020    |    0.847    
-00006570: 207c 2020 302e 3931 3620 2020 7c0a 7c20   |  0.916   |.| 
-00006580: 2020 2060 5669 5455 6e69 636f 6d45 7874     `ViTUnicomExt
-00006590: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
-000065a0: 7261 696e 6564 2822 7669 7462 3332 5f75  rained("vitb32_u
-000065b0: 6e69 636f 6d22 2960 2020 2020 207c 2020  nicom")`     |  
-000065c0: 2020 2020 2020 2020 302e 3639 3020 2020          0.690   
-000065d0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000065e0: 302e 3732 3220 2020 2020 2020 207c 2020  0.722        |  
-000065f0: 2020 302e 3739 3620 2020 2020 7c20 2030    0.796     |  0
-00006600: 2e38 3933 2020 207c 0a7c 2020 2020 6056  .893   |.|    `V
-00006610: 6954 556e 6963 6f6d 4578 7472 6163 746f  iTUnicomExtracto
-00006620: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-00006630: 6428 2276 6974 6c31 345f 756e 6963 6f6d  d("vitl14_unicom
-00006640: 2229 6020 2020 2020 7c20 2020 2020 2020  ")`     |       
-00006650: 2020 2030 2e37 3236 2020 2020 2020 2020     0.726        
-00006660: 2020 207c 2020 2020 2020 2030 2e37 3930     |       0.790
-00006670: 2020 2020 2020 2020 7c20 2020 2030 2e38          |    0.8
-00006680: 3638 2020 2020 207c 2020 302e 3932 3220  68     |  0.922 
-00006690: 2020 7c0a 7c20 6056 6954 556e 6963 6f6d    |.| `ViTUnicom
-000066a0: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-000066b0: 7265 7472 6169 6e65 6428 2276 6974 6c31  retrained("vitl1
-000066c0: 345f 3333 3670 785f 756e 6963 6f6d 2229  4_336px_unicom")
-000066d0: 6020 207c 2020 2020 2020 2020 2020 302e  `  |          0.
-000066e0: 3734 3520 2020 2020 2020 2020 2020 7c20  745           | 
-000066f0: 2020 2020 2020 302e 3831 3020 2020 2020        0.810     
-00006700: 2020 207c 2020 2020 302e 3837 3520 2020     |    0.875   
-00006710: 2020 7c20 2030 2e39 3234 2020 207c 0a7c    |  0.924   |.|
-00006720: 2020 2020 6056 6954 434c 4950 4578 7472      `ViTCLIPExtr
-00006730: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-00006740: 6169 6e65 6428 2273 6265 725f 7669 7462  ained("sber_vitb
-00006750: 3332 5f32 3234 2229 6020 2020 2020 7c20  32_224")`     | 
-00006760: 2020 2020 2020 2020 2030 2e35 3437 2020           0.547  
-00006770: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00006780: 2030 2e35 3134 2020 2020 2020 2020 7c20   0.514        | 
-00006790: 2020 2030 2e34 3438 2020 2020 207c 2020     0.448     |  
-000067a0: 302e 3631 3820 2020 7c0a 7c20 2020 2060  0.618   |.|    `
-000067b0: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-000067c0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-000067d0: 2822 7362 6572 5f76 6974 6231 365f 3232  ("sber_vitb16_22
-000067e0: 3422 2960 2020 2020 207c 2020 2020 2020  4")`     |      
-000067f0: 2020 2020 302e 3536 3520 2020 2020 2020      0.565       
-00006800: 2020 2020 7c20 2020 2020 2020 302e 3536      |       0.56
-00006810: 3520 2020 2020 2020 207c 2020 2020 302e  5        |    0.
-00006820: 3532 3420 2020 2020 7c20 2030 2e36 3438  524     |  0.648
-00006830: 2020 207c 0a7c 2020 2020 6056 6954 434c     |.|    `ViTCL
-00006840: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-00006850: 5f70 7265 7472 6169 6e65 6428 2273 6265  _pretrained("sbe
-00006860: 725f 7669 746c 3134 5f32 3234 2229 6020  r_vitl14_224")` 
-00006870: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
-00006880: 2e35 3132 2020 2020 2020 2020 2020 207c  .512           |
-00006890: 2020 2020 2020 2030 2e35 3535 2020 2020         0.555    
-000068a0: 2020 2020 7c20 2020 2030 2e36 3036 2020      |    0.606  
-000068b0: 2020 207c 2020 302e 3730 3720 2020 7c0a     |  0.707   |.
-000068c0: 7c20 2020 6056 6954 434c 4950 4578 7472  |   `ViTCLIPExtr
-000068d0: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
-000068e0: 6169 6e65 6428 226f 7065 6e61 695f 7669  ained("openai_vi
-000068f0: 7462 3332 5f32 3234 2229 6020 2020 207c  tb32_224")`    |
-00006900: 2020 2020 2020 2020 2020 302e 3631 3220            0.612 
-00006910: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00006920: 2020 302e 3439 3120 2020 2020 2020 207c    0.491        |
-00006930: 2020 2020 302e 3536 3020 2020 2020 7c20      0.560     | 
-00006940: 2030 2e36 3933 2020 207c 0a7c 2020 2060   0.693   |.|   `
-00006950: 5669 5443 4c49 5045 7874 7261 6374 6f72  ViTCLIPExtractor
-00006960: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
-00006970: 2822 6f70 656e 6169 5f76 6974 6231 365f  ("openai_vitb16_
-00006980: 3232 3422 2960 2020 2020 7c20 2020 2020  224")`    |     
-00006990: 2020 2020 2030 2e36 3438 2020 2020 2020       0.648      
-000069a0: 2020 2020 207c 2020 2020 2020 2030 2e36       |       0.6
-000069b0: 3036 2020 2020 2020 2020 7c20 2020 2030  06        |    0
-000069c0: 2e36 3635 2020 2020 207c 2020 302e 3736  .665     |  0.76
-000069d0: 3720 2020 7c0a 7c20 2020 6056 6954 434c  7   |.|   `ViTCL
-000069e0: 4950 4578 7472 6163 746f 722e 6672 6f6d  IPExtractor.from
-000069f0: 5f70 7265 7472 6169 6e65 6428 226f 7065  _pretrained("ope
-00006a00: 6e61 695f 7669 746c 3134 5f32 3234 2229  nai_vitl14_224")
-00006a10: 6020 2020 207c 2020 2020 2020 2020 2020  `    |          
-00006a20: 302e 3637 3020 2020 2020 2020 2020 2020  0.670           
-00006a30: 7c20 2020 2020 2020 302e 3637 3520 2020  |       0.675   
-00006a40: 2020 2020 207c 2020 2020 302e 3734 3520       |    0.745 
-00006a50: 2020 2020 7c20 2030 2e38 3434 2020 207c      |  0.844   |
-00006a60: 0a7c 2020 2020 2020 2020 6056 6954 4578  .|        `ViTEx
-00006a70: 7472 6163 746f 722e 6672 6f6d 5f70 7265  tractor.from_pre
-00006a80: 7472 6169 6e65 6428 2276 6974 7331 365f  trained("vits16_
-00006a90: 6469 6e6f 2229 6020 2020 2020 2020 2020  dino")`         
-00006aa0: 7c20 2020 2020 2020 2020 2030 2e36 3438  |          0.648
-00006ab0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00006ac0: 2020 2030 2e35 3039 2020 2020 2020 2020     0.509        
-00006ad0: 7c20 2020 2030 2e36 3237 2020 2020 207c  |    0.627     |
-00006ae0: 2020 302e 3236 3520 2020 7c0a 7c20 2020    0.265   |.|   
-00006af0: 2020 2020 2020 6056 6954 4578 7472 6163        `ViTExtrac
-00006b00: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
-00006b10: 6e65 6428 2276 6974 7338 5f64 696e 6f22  ned("vits8_dino"
-00006b20: 2960 2020 2020 2020 2020 207c 2020 2020  )`         |    
-00006b30: 2020 2020 2020 302e 3635 3120 2020 2020        0.651     
-00006b40: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
-00006b50: 3532 3420 2020 2020 2020 207c 2020 2020  524        |    
-00006b60: 302e 3636 3120 2020 2020 7c20 2030 2e33  0.661     |  0.3
-00006b70: 3135 2020 207c 0a7c 2020 2020 2020 2020  15   |.|        
-00006b80: 6056 6954 4578 7472 6163 746f 722e 6672  `ViTExtractor.fr
-00006b90: 6f6d 5f70 7265 7472 6169 6e65 6428 2276  om_pretrained("v
-00006ba0: 6974 6231 365f 6469 6e6f 2229 6020 2020  itb16_dino")`   
-00006bb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00006bc0: 2030 2e36 3538 2020 2020 2020 2020 2020   0.658          
-00006bd0: 207c 2020 2020 2020 2030 2e35 3134 2020   |       0.514  
-00006be0: 2020 2020 2020 7c20 2020 2030 2e35 3431        |    0.541
-00006bf0: 2020 2020 207c 2020 302e 3238 3820 2020       |  0.288   
-00006c00: 7c0a 7c20 2020 2020 2020 2020 6056 6954  |.|         `ViT
-00006c10: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
-00006c20: 7265 7472 6169 6e65 6428 2276 6974 6238  retrained("vitb8
-00006c30: 5f64 696e 6f22 2960 2020 2020 2020 2020  _dino")`        
-00006c40: 207c 2020 2020 2020 2020 2020 302e 3638   |          0.68
-00006c50: 3920 2020 2020 2020 2020 2020 7c20 2020  9           |   
-00006c60: 2020 2020 302e 3539 3920 2020 2020 2020      0.599       
-00006c70: 207c 2020 2020 302e 3530 3620 2020 2020   |    0.506     
-00006c80: 7c20 2030 2e33 3133 2020 207c 0a7c 2020  |  0.313   |.|  
-00006c90: 2020 6052 6573 6e65 7445 7874 7261 6374    `ResnetExtract
-00006ca0: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
-00006cb0: 6564 2822 7265 736e 6574 3530 5f6d 6f63  ed("resnet50_moc
-00006cc0: 6f5f 7632 2229 6020 2020 2020 7c20 2020  o_v2")`     |   
-00006cd0: 2020 2020 2020 2030 2e34 3933 2020 2020         0.493    
-00006ce0: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
-00006cf0: 2e32 3637 2020 2020 2020 2020 7c20 2020  .267        |   
-00006d00: 2030 2e32 3634 2020 2020 207c 2020 302e   0.264     |  0.
-00006d10: 3134 3920 2020 7c0a 7c20 6052 6573 6e65  149   |.| `Resne
-00006d20: 7445 7874 7261 6374 6f72 2e66 726f 6d5f  tExtractor.from_
-00006d30: 7072 6574 7261 696e 6564 2822 7265 736e  pretrained("resn
-00006d40: 6574 3530 5f69 6d61 6765 6e65 7431 6b5f  et50_imagenet1k_
-00006d50: 7631 2229 6020 207c 2020 2020 2020 2020  v1")`  |        
-00006d60: 2020 302e 3531 3520 2020 2020 2020 2020    0.515         
-00006d70: 2020 7c20 2020 2020 2020 302e 3238 3420    |       0.284 
-00006d80: 2020 2020 2020 207c 2020 2020 302e 3435         |    0.45
-00006d90: 3520 2020 2020 7c20 2030 2e32 3437 2020  5     |  0.247  
-00006da0: 207c 0a0a 2a2a 5468 6520 6d65 7472 6963   |..**The metric
-00006db0: 7320 6d61 7920 6265 2064 6966 6665 7265  s may be differe
-00006dc0: 6e74 2066 726f 6d20 7468 6520 6f6e 6573  nt from the ones
-00006dd0: 2072 6570 6f72 7465 6420 6279 2070 6170   reported by pap
-00006de0: 6572 732c 0a62 6563 6175 7365 2074 6865  ers,.because the
-00006df0: 2076 6572 7369 6f6e 206f 6620 7472 6169   version of trai
-00006e00: 6e2f 7661 6c20 7370 6c69 7420 616e 6420  n/val split and 
-00006e10: 7573 6167 6520 6f66 2062 6f75 6e64 696e  usage of boundin
-00006e20: 6720 626f 7865 7320 6d61 7920 6469 6666  g boxes may diff
-00006e30: 6572 2e0a 5061 7274 6963 756c 6172 6c79  er..Particularly
-00006e40: 2c20 7765 2075 7365 6420 626f 756e 6469  , we used boundi
-00006e50: 6e67 2062 6f78 6573 2064 7572 696e 6720  ng boxes during 
-00006e60: 7468 6520 6576 616c 7561 7469 6f6e 2e2a  the evaluation.*
-00006e70: 0a0a 2323 2320 486f 7720 746f 2075 7365  ..### How to use
-00006e80: 206d 6f64 656c 7320 6672 6f6d 205a 6f6f   models from Zoo
-00006e90: 3f0a 0a5b 636f 6d6d 656e 745d 3a7a 6f6f  ?..[comment]:zoo
-00006ea0: 2d73 7461 7274 0a60 6060 7079 7468 6f6e  -start.```python
-00006eb0: 0a66 726f 6d20 6f6d 6c2e 636f 6e73 7420  .from oml.const 
-00006ec0: 696d 706f 7274 2043 4b50 545f 5341 5645  import CKPT_SAVE
-00006ed0: 5f52 4f4f 5420 6173 2043 4b50 545f 4449  _ROOT as CKPT_DI
-00006ee0: 522c 204d 4f43 4b5f 4441 5441 5345 545f  R, MOCK_DATASET_
-00006ef0: 5041 5448 2061 7320 4441 5441 5f44 4952  PATH as DATA_DIR
-00006f00: 0a66 726f 6d20 6f6d 6c2e 6d6f 6465 6c73  .from oml.models
-00006f10: 2069 6d70 6f72 7420 5669 5445 7874 7261   import ViTExtra
-00006f20: 6374 6f72 0a66 726f 6d20 6f6d 6c2e 7265  ctor.from oml.re
-00006f30: 6769 7374 7279 2e74 7261 6e73 666f 726d  gistry.transform
-00006f40: 7320 696d 706f 7274 2067 6574 5f74 7261  s import get_tra
-00006f50: 6e73 666f 726d 735f 666f 725f 7072 6574  nsforms_for_pret
-00006f60: 7261 696e 6564 0a0a 6d6f 6465 6c20 3d20  rained..model = 
-00006f70: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
-00006f80: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
-00006f90: 7473 3136 5f64 696e 6f22 290a 7472 616e  ts16_dino").tran
-00006fa0: 7366 6f72 6d73 2c20 696d 5f72 6561 6465  sforms, im_reade
-00006fb0: 7220 3d20 6765 745f 7472 616e 7366 6f72  r = get_transfor
-00006fc0: 6d73 5f66 6f72 5f70 7265 7472 6169 6e65  ms_for_pretraine
-00006fd0: 6428 2276 6974 7331 365f 6469 6e6f 2229  d("vits16_dino")
-00006fe0: 0a0a 696d 6720 3d20 696d 5f72 6561 6465  ..img = im_reade
-00006ff0: 7228 4441 5441 5f44 4952 202f 2022 696d  r(DATA_DIR / "im
-00007000: 6167 6573 2220 2f20 2263 6972 636c 655f  ages" / "circle_
-00007010: 312e 6a70 6722 2920 2023 2070 7574 2070  1.jpg")  # put p
-00007020: 6174 6820 746f 2079 6f75 7220 696d 6167  ath to your imag
-00007030: 6520 6865 7265 0a69 6d67 5f74 656e 736f  e here.img_tenso
-00007040: 7220 3d20 7472 616e 7366 6f72 6d73 2869  r = transforms(i
-00007050: 6d67 290a 2320 696d 675f 7465 6e73 6f72  mg).# img_tensor
-00007060: 203d 2074 7261 6e73 666f 726d 7328 696d   = transforms(im
-00007070: 6167 653d 696d 6729 5b22 696d 6167 6522  age=img)["image"
-00007080: 5d20 2023 2066 6f72 2074 7261 6e73 666f  ]  # for transfo
-00007090: 726d 7320 6672 6f6d 2041 6c62 756d 656e  rms from Albumen
-000070a0: 7461 7469 6f6e 730a 0a66 6561 7475 7265  tations..feature
-000070b0: 7320 3d20 6d6f 6465 6c28 696d 675f 7465  s = model(img_te
-000070c0: 6e73 6f72 2e75 6e73 7175 6565 7a65 2830  nsor.unsqueeze(0
-000070d0: 2929 0a0a 2320 4368 6563 6b20 6f74 6865  ))..# Check othe
-000070e0: 7220 6176 6169 6c61 626c 6520 6d6f 6465  r available mode
-000070f0: 6c73 3a0a 7072 696e 7428 6c69 7374 2856  ls:.print(list(V
-00007100: 6954 4578 7472 6163 746f 722e 7072 6574  iTExtractor.pret
-00007110: 7261 696e 6564 5f6d 6f64 656c 732e 6b65  rained_models.ke
-00007120: 7973 2829 2929 0a0a 2320 4c6f 6164 2063  ys()))..# Load c
-00007130: 6865 636b 706f 696e 7420 7361 7665 6420  heckpoint saved 
-00007140: 6f6e 2061 2064 6973 6b3a 0a6d 6f64 656c  on a disk:.model
-00007150: 5f20 3d20 5669 5445 7874 7261 6374 6f72  _ = ViTExtractor
-00007160: 2877 6569 6768 7473 3d43 4b50 545f 4449  (weights=CKPT_DI
-00007170: 5220 2f20 2276 6974 7331 365f 6469 6e6f  R / "vits16_dino
-00007180: 2e63 6b70 7422 2c20 6172 6368 3d22 7669  .ckpt", arch="vi
-00007190: 7473 3136 222c 206e 6f72 6d61 6c69 7365  ts16", normalise
-000071a0: 5f66 6561 7475 7265 733d 4661 6c73 6529  _features=False)
-000071b0: 0a60 6060 0a5b 636f 6d6d 656e 745d 3a7a  .```.[comment]:z
-000071c0: 6f6f 2d65 6e64 0a0a 2323 205b 436f 6e74  oo-end..## [Cont
-000071d0: 7269 6275 7469 6e67 2067 7569 6465 5d28  ributing guide](
-000071e0: 6874 7470 733a 2f2f 6f70 656e 2d6d 6574  https://open-met
-000071f0: 7269 632d 6c65 6172 6e69 6e67 2e72 6561  ric-learning.rea
-00007200: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00007210: 6174 6573 742f 6f6d 6c2f 636f 6e74 7269  atest/oml/contri
-00007220: 6275 7469 6e67 2e68 746d 6c29 0a0a 5765  buting.html)..We
-00007230: 2077 656c 636f 6d65 206e 6577 2063 6f6e   welcome new con
-00007240: 7472 6962 7574 6f72 7321 2050 6c65 6173  tributors! Pleas
-00007250: 652c 2073 6565 206f 7572 3a0a 2a20 5b43  e, see our:.* [C
-00007260: 6f6e 7472 6962 7574 696e 6720 6775 6964  ontributing guid
-00007270: 655d 2868 7474 7073 3a2f 2f6f 7065 6e2d  e](https://open-
-00007280: 6d65 7472 6963 2d6c 6561 726e 696e 672e  metric-learning.
-00007290: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-000072a0: 6e2f 6c61 7465 7374 2f66 726f 6d5f 7265  n/latest/from_re
-000072b0: 6164 6d65 2f63 6f6e 7472 6962 7574 696e  adme/contributin
-000072c0: 672e 6874 6d6c 290a 2a20 5b4b 616e 6261  g.html).* [Kanba
-000072d0: 6e20 626f 6172 645d 2868 7474 7073 3a2f  n board](https:/
-000072e0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
-000072f0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
-00007300: 2d6c 6561 726e 696e 672f 7072 6f6a 6563  -learning/projec
-00007310: 7473 2f31 290a 0a23 2320 4163 6b6e 6f77  ts/1)..## Acknow
-00007320: 6c65 6467 6d65 6e74 730a 0a3c 6120 6872  ledgments..<a hr
-00007330: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00007340: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00007350: 7465 616d 2f63 6174 616c 7973 7422 2074  team/catalyst" t
-00007360: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00007370: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00007380: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00007390: 6f6e 7465 6e74 2e63 6f6d 2f63 6174 616c  ontent.com/catal
-000073a0: 7973 742d 7465 616d 2f63 6174 616c 7973  yst-team/catalys
-000073b0: 742d 7069 6373 2f6d 6173 7465 722f 7069  t-pics/master/pi
-000073c0: 6373 2f63 6174 616c 7973 745f 6c6f 676f  cs/catalyst_logo
-000073d0: 2e70 6e67 2220 7769 6474 683d 2231 3030  .png" width="100
-000073e0: 222f 3e3c 2f61 3e0a 0a54 6865 2070 726f  "/></a>..The pro
-000073f0: 6a65 6374 2077 6173 2073 7461 7274 6564  ject was started
-00007400: 2069 6e20 3230 3230 2061 7320 6120 6d6f   in 2020 as a mo
-00007410: 6475 6c65 2066 6f72 205b 4361 7461 6c79  dule for [Cataly
-00007420: 7374 5d28 6874 7470 733a 2f2f 6769 7468  st](https://gith
-00007430: 7562 2e63 6f6d 2f63 6174 616c 7973 742d  ub.com/catalyst-
-00007440: 7465 616d 2f63 6174 616c 7973 7429 206c  team/catalyst) l
-00007450: 6962 7261 7279 2e0a 4920 7761 6e74 2074  ibrary..I want t
-00007460: 6f20 7468 616e 6b20 7065 6f70 6c65 2077  o thank people w
-00007470: 686f 2077 6f72 6b65 6420 7769 7468 206d  ho worked with m
-00007480: 6520 6f6e 2074 6861 7420 6d6f 6475 6c65  e on that module
-00007490: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
-000074a0: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
-000074b0: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
-000074c0: 6e73 6869 6e61 292c 0a5b 4e69 6b69 7461  nshina),.[Nikita
-000074d0: 2042 616c 6167 616e 736b 795d 2868 7474   Balagansky](htt
-000074e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000074f0: 656c 6570 6861 6e74 6d69 7074 292c 0a5b  elephantmipt),.[
-00007500: 5365 7267 6579 204b 6f6c 6573 6e69 6b6f  Sergey Kolesniko
-00007510: 765d 2868 7474 7073 3a2f 2f67 6974 6875  v](https://githu
-00007520: 622e 636f 6d2f 5363 6974 6174 6f72 290a  b.com/Scitator).
-00007530: 616e 6420 6f74 6865 7273 2e0a 0a49 2077  and others...I w
-00007540: 6f75 6c64 206c 696b 6520 746f 2074 6861  ould like to tha
-00007550: 6e6b 2070 656f 706c 6520 7768 6f20 636f  nk people who co
-00007560: 6e74 696e 7565 2077 6f72 6b69 6e67 206f  ntinue working o
-00007570: 6e20 7468 6973 2070 6970 656c 696e 6520  n this pipeline 
-00007580: 7768 656e 2069 7420 6265 6361 6d65 2061  when it became a
-00007590: 2073 6570 6172 6520 7072 6f6a 6563 743a   separe project:
-000075a0: 0a5b 4a75 6c69 6120 5368 656e 7368 696e  .[Julia Shenshin
-000075b0: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-000075c0: 622e 636f 6d2f 6a75 6c69 612d 7368 656e  b.com/julia-shen
-000075d0: 7368 696e 6129 2c0a 5b4d 6973 6861 204b  shina),.[Misha K
-000075e0: 696e 6475 6c6f 765d 2868 7474 7073 3a2f  indulov](https:/
-000075f0: 2f67 6974 6875 622e 636f 6d2f 6230 6e63  /github.com/b0nc
-00007600: 6529 2c0a 5b41 6c65 6b73 6569 2054 6172  e),.[Aleksei Tar
-00007610: 6173 6f76 5d28 6874 7470 733a 2f2f 6769  asov](https://gi
-00007620: 7468 7562 2e63 6f6d 2f44 616c 6f72 6f41  thub.com/DaloroA
-00007630: 5429 2061 6e64 0a5b 5665 726b 686f 7674  T) and.[Verkhovt
-00007640: 7365 7620 4c65 6f6e 6964 5d28 6874 7470  sev Leonid](http
-00007650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00007660: 656f 726f 6d61 6e6f 7669 6368 292e 0a0a  eoromanovich)...
-00007670: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00007680: 2f77 7777 2e6e 6577 796f 726b 6572 2e64  /www.newyorker.d
-00007690: 652f 2220 7461 7267 6574 3d22 5f62 6c61  e/" target="_bla
-000076a0: 6e6b 223e 3c69 6d67 2073 7263 3d22 6874  nk"><img src="ht
-000076b0: 7470 733a 2f2f 7570 6c6f 6164 2e77 696b  tps://upload.wik
-000076c0: 696d 6564 6961 2e6f 7267 2f77 696b 6970  imedia.org/wikip
-000076d0: 6564 6961 2f63 6f6d 6d6f 6e73 2f74 6875  edia/commons/thu
-000076e0: 6d62 2f64 2f64 382f 4e65 775f 596f 726b  mb/d/d8/New_York
-000076f0: 6572 2e73 7667 2f31 3238 3070 782d 4e65  er.svg/1280px-Ne
-00007700: 775f 596f 726b 6572 2e73 7667 2e70 6e67  w_Yorker.svg.png
-00007710: 2220 7769 6474 683d 2231 3030 222f 3e3c  " width="100"/><
-00007720: 2f61 3e0a 0a49 2061 6c73 6f20 7761 6e74  /a>..I also want
-00007730: 2074 6f20 7468 616e 6b20 4e65 7759 6f72   to thank NewYor
-00007740: 6b65 722c 2073 696e 6365 2074 6865 2070  ker, since the p
-00007750: 6172 7420 6f66 2066 756e 6374 696f 6e61  art of functiona
-00007760: 6c69 7479 2077 6173 2064 6576 656c 6f70  lity was develop
-00007770: 6564 2028 616e 6420 7573 6564 2920 6279  ed (and used) by
-00007780: 2069 7473 2063 6f6d 7075 7465 7220 7669   its computer vi
-00007790: 7369 6f6e 2074 6561 6d20 6c65 6420 6279  sion team led by
-000077a0: 206d 652e 0a                              me..
+00005e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
+00005e50: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00005e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00005e70: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00005e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ed0: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00005ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f40: 2d2d 2d2d 2d2d 3a7c 0a7c 2060 5669 5445  ------:|.| `ViTE
+00005f50: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00005f60: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+00005f70: 5f69 6e73 686f 7022 2960 207c 2030 2e39  _inshop")` | 0.9
+00005f80: 3231 207c 2020 2020 4465 6570 4661 7368  21 |    DeepFash
+00005f90: 696f 6e20 496e 7368 6f70 2020 2020 7c20  ion Inshop    | 
+00005fa0: 2020 205b 6c69 6e6b 5d28 6874 7470 733a     [link](https:
+00005fb0: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
+00005fc0: 6f6d 2f66 696c 652f 642f 316e 6958 2d54  om/file/d/1niX-T
+00005fd0: 4338 636a 366a 3336 3974 3769 5532 6261  C8cj6j369t7iU2ba
+00005fe0: 4851 5356 4e33 4d56 4a62 572f 7669 6577  HQSVN3MVJbW/view
+00005ff0: 3f75 7370 3d73 6861 7269 6e67 2920 2020  ?usp=sharing)   
+00006000: 2020 7c20 5b6c 696e 6b5d 2868 7474 7073    | [link](https
+00006010: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+00006020: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+00006030: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+00006040: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+00006050: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+00006060: 696f 6e2f 6578 7472 6163 746f 725f 696e  ion/extractor_in
+00006070: 7368 6f70 2920 7c0a 7c20 2060 5669 5445  shop) |.|  `ViTE
+00006080: 7874 7261 6374 6f72 2e66 726f 6d5f 7072  xtractor.from_pr
+00006090: 6574 7261 696e 6564 2822 7669 7473 3136  etrained("vits16
+000060a0: 5f73 6f70 2229 6020 2020 7c20 302e 3836  _sop")`   | 0.86
+000060b0: 3620 7c20 5374 616e 666f 7264 204f 6e6c  6 | Stanford Onl
+000060c0: 696e 6520 5072 6f64 7563 7473 207c 2020  ine Products |  
+000060d0: 205b 6c69 6e6b 5d28 6874 7470 733a 2f2f   [link](https://
+000060e0: 6472 6976 652e 676f 6f67 6c65 2e63 6f6d  drive.google.com
+000060f0: 2f66 696c 652f 642f 317a 7547 5248 7646  /file/d/1zuGRHvF
+00006100: 324b 4864 3539 6177 3769 3733 3637 4f48  2KHd59aw7i7367OH
+00006110: 5f74 514e 4f47 7a37 412f 7669 6577 3f75  _tQNOGz7A/view?u
+00006120: 7370 3d73 6861 7269 6e67 2920 2020 2020  sp=sharing)     
+00006130: 207c 2020 5b6c 696e 6b5d 2868 7474 7073   |  [link](https
+00006140: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f4d  ://github.com/OM
+00006150: 4c2d 5465 616d 2f6f 7065 6e2d 6d65 7472  L-Team/open-metr
+00006160: 6963 2d6c 6561 726e 696e 672f 7472 6565  ic-learning/tree
+00006170: 2f6d 6169 6e2f 7069 7065 6c69 6e65 732f  /main/pipelines/
+00006180: 6665 6174 7572 6573 5f65 7874 7261 6374  features_extract
+00006190: 696f 6e2f 6578 7472 6163 746f 725f 736f  ion/extractor_so
+000061a0: 7029 2020 207c 0a7c 2060 5669 5445 7874  p)   |.| `ViTExt
+000061b0: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+000061c0: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+000061d0: 6172 7322 2960 2020 207c 2030 2e39 3037  ars")`   | 0.907
+000061e0: 207c 2020 2020 2020 2020 2043 4152 5320   |         CARS 
+000061f0: 3139 3620 2020 2020 2020 2020 7c20 2020  196         |   
+00006200: 5b6c 696e 6b5d 2868 7474 7073 3a2f 2f64  [link](https://d
+00006210: 7269 7665 2e67 6f6f 676c 652e 636f 6d2f  rive.google.com/
+00006220: 6472 6976 652f 666f 6c64 6572 732f 3137  drive/folders/17
+00006230: 6134 5f66 6739 3464 6f78 3273 666b 586d  a4_fg94dox2sfkXm
+00006240: 772d 4b43 7469 4c42 6c78 2d75 742d 313f  w-KCtiLBlx-ut-1?
+00006250: 7573 703d 7368 6172 696e 6729 2020 2020  usp=sharing)    
+00006260: 7c20 205b 6c69 6e6b 5d28 6874 7470 733a  |  [link](https:
+00006270: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+00006280: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+00006290: 632d 6c65 6172 6e69 6e67 2f74 7265 652f  c-learning/tree/
+000062a0: 6d61 696e 2f70 6970 656c 696e 6573 2f66  main/pipelines/f
+000062b0: 6561 7475 7265 735f 6578 7472 6163 7469  eatures_extracti
+000062c0: 6f6e 2f65 7874 7261 6374 6f72 5f63 6172  on/extractor_car
+000062d0: 7329 2020 7c0a 7c20 2060 5669 5445 7874  s)  |.|  `ViTExt
+000062e0: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+000062f0: 7261 696e 6564 2822 7669 7473 3136 5f63  rained("vits16_c
+00006300: 7562 2229 6020 2020 7c20 302e 3833 3720  ub")`   | 0.837 
+00006310: 7c20 2020 2020 2020 4355 4220 3230 3020  |       CUB 200 
+00006320: 3230 3131 2020 2020 2020 207c 2020 205b  2011       |   [
+00006330: 6c69 6e6b 5d28 6874 7470 733a 2f2f 6472  link](https://dr
+00006340: 6976 652e 676f 6f67 6c65 2e63 6f6d 2f64  ive.google.com/d
+00006350: 7269 7665 2f66 6f6c 6465 7273 2f31 5450  rive/folders/1TP
+00006360: 434e 2d65 5a46 4c71 6f71 344a 4267 6e49  CN-eZFLqoq4JBgnI
+00006370: 666c 694a 6f45 4b34 3878 396f 7a62 3f75  fliJoEK48x9ozb?u
+00006380: 7370 3d73 6861 7269 6e67 2920 2020 207c  sp=sharing)    |
+00006390: 2020 5b6c 696e 6b5d 2868 7474 7073 3a2f    [link](https:/
+000063a0: 2f67 6974 6875 622e 636f 6d2f 4f4d 4c2d  /github.com/OML-
+000063b0: 5465 616d 2f6f 7065 6e2d 6d65 7472 6963  Team/open-metric
+000063c0: 2d6c 6561 726e 696e 672f 7472 6565 2f6d  -learning/tree/m
+000063d0: 6169 6e2f 7069 7065 6c69 6e65 732f 6665  ain/pipelines/fe
+000063e0: 6174 7572 6573 5f65 7874 7261 6374 696f  atures_extractio
+000063f0: 6e2f 6578 7472 6163 746f 725f 6375 6229  n/extractor_cub)
+00006400: 2020 207c 0a0a 5765 2061 6c73 6f20 7072     |..We also pr
+00006410: 6f76 6964 6520 616e 2069 6e74 6567 7261  ovide an integra
+00006420: 7469 6f6e 2077 6974 6820 7468 6520 6d6f  tion with the mo
+00006430: 6465 6c73 2070 7265 7472 6169 6e65 6420  dels pretrained 
+00006440: 6279 206f 7468 6572 2072 6573 6561 7263  by other researc
+00006450: 6865 7273 2e0a 416c 6c20 6d65 7472 6963  hers..All metric
+00006460: 7320 6265 6c6f 7720 7765 7265 206f 6274  s below were obt
+00006470: 6169 6e65 6420 6f6e 2074 6865 2069 6d61  ained on the ima
+00006480: 6765 7320 7769 7468 2074 6865 2073 697a  ges with the siz
+00006490: 6573 206f 6620 2a2a 3232 3420 7820 3232  es of **224 x 22
+000064a0: 342a 2a3a 0a0a 7c20 2020 2020 2020 2020  4**:..|         
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2020 206d 6f64 656c 2020 2020 2020 2020     model        
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 207c 2053 7461 6e66 6f72 6420       | Stanford 
+000064f0: 4f6e 6c69 6e65 2050 726f 6475 6374 7320  Online Products 
+00006500: 7c20 4465 6570 4661 7368 696f 6e20 496e  | DeepFashion In
+00006510: 5368 6f70 207c 2043 5542 2032 3030 2032  Shop | CUB 200 2
+00006520: 3031 3120 7c20 4341 5253 2031 3936 207c  011 | CARS 196 |
+00006530: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
+00006540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+00006570: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
+00006580: 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d  ----------:|:---
+00006590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a  ---------------:
+000065a0: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  |:------------:|
+000065b0: 3a2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20 2020  :--------:|.|   
+000065c0: 2060 5669 5455 6e69 636f 6d45 7874 7261   `ViTUnicomExtra
+000065d0: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+000065e0: 696e 6564 2822 7669 7462 3136 5f75 6e69  ined("vitb16_uni
+000065f0: 636f 6d22 2960 2020 2020 207c 2020 2020  com")`     |    
+00006600: 2020 2020 2020 302e 3730 3020 2020 2020        0.700     
+00006610: 2020 2020 2020 7c20 2020 2020 2020 302e        |       0.
+00006620: 3733 3420 2020 2020 2020 207c 2020 2020  734        |    
+00006630: 302e 3834 3720 2020 2020 7c20 2030 2e39  0.847     |  0.9
+00006640: 3136 2020 207c 0a7c 2020 2020 6056 6954  16   |.|    `ViT
+00006650: 556e 6963 6f6d 4578 7472 6163 746f 722e  UnicomExtractor.
+00006660: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+00006670: 2276 6974 6233 325f 756e 6963 6f6d 2229  "vitb32_unicom")
+00006680: 6020 2020 2020 7c20 2020 2020 2020 2020  `     |         
+00006690: 2030 2e36 3930 2020 2020 2020 2020 2020   0.690          
+000066a0: 207c 2020 2020 2020 2030 2e37 3232 2020   |       0.722  
+000066b0: 2020 2020 2020 7c20 2020 2030 2e37 3936        |    0.796
+000066c0: 2020 2020 207c 2020 302e 3839 3320 2020       |  0.893   
+000066d0: 7c0a 7c20 2020 2060 5669 5455 6e69 636f  |.|    `ViTUnico
+000066e0: 6d45 7874 7261 6374 6f72 2e66 726f 6d5f  mExtractor.from_
+000066f0: 7072 6574 7261 696e 6564 2822 7669 746c  pretrained("vitl
+00006700: 3134 5f75 6e69 636f 6d22 2960 2020 2020  14_unicom")`    
+00006710: 207c 2020 2020 2020 2020 2020 302e 3732   |          0.72
+00006720: 3620 2020 2020 2020 2020 2020 7c20 2020  6           |   
+00006730: 2020 2020 302e 3739 3020 2020 2020 2020      0.790       
+00006740: 207c 2020 2020 302e 3836 3820 2020 2020   |    0.868     
+00006750: 7c20 2030 2e39 3232 2020 207c 0a7c 2060  |  0.922   |.| `
+00006760: 5669 5455 6e69 636f 6d45 7874 7261 6374  ViTUnicomExtract
+00006770: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00006780: 6564 2822 7669 746c 3134 5f33 3336 7078  ed("vitl14_336px
+00006790: 5f75 6e69 636f 6d22 2960 2020 7c20 2020  _unicom")`  |   
+000067a0: 2020 2020 2020 2030 2e37 3435 2020 2020         0.745    
+000067b0: 2020 2020 2020 207c 2020 2020 2020 2030         |       0
+000067c0: 2e38 3130 2020 2020 2020 2020 7c20 2020  .810        |   
+000067d0: 2030 2e38 3735 2020 2020 207c 2020 302e   0.875     |  0.
+000067e0: 3932 3420 2020 7c0a 7c20 2020 2060 5669  924   |.|    `Vi
+000067f0: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+00006800: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00006810: 7362 6572 5f76 6974 6233 325f 3232 3422  sber_vitb32_224"
+00006820: 2960 2020 2020 207c 2020 2020 2020 2020  )`     |        
+00006830: 2020 302e 3534 3720 2020 2020 2020 2020    0.547         
+00006840: 2020 7c20 2020 2020 2020 302e 3531 3420    |       0.514 
+00006850: 2020 2020 2020 207c 2020 2020 302e 3434         |    0.44
+00006860: 3820 2020 2020 7c20 2030 2e36 3138 2020  8     |  0.618  
+00006870: 207c 0a7c 2020 2020 6056 6954 434c 4950   |.|    `ViTCLIP
+00006880: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006890: 7265 7472 6169 6e65 6428 2273 6265 725f  retrained("sber_
+000068a0: 7669 7462 3136 5f32 3234 2229 6020 2020  vitb16_224")`   
+000068b0: 2020 7c20 2020 2020 2020 2020 2030 2e35    |          0.5
+000068c0: 3635 2020 2020 2020 2020 2020 207c 2020  65           |  
+000068d0: 2020 2020 2030 2e35 3635 2020 2020 2020       0.565      
+000068e0: 2020 7c20 2020 2030 2e35 3234 2020 2020    |    0.524    
+000068f0: 207c 2020 302e 3634 3820 2020 7c0a 7c20   |  0.648   |.| 
+00006900: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00006910: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006920: 696e 6564 2822 7362 6572 5f76 6974 6c31  ined("sber_vitl1
+00006930: 345f 3232 3422 2960 2020 2020 207c 2020  4_224")`     |  
+00006940: 2020 2020 2020 2020 302e 3531 3220 2020          0.512   
+00006950: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006960: 302e 3535 3520 2020 2020 2020 207c 2020  0.555        |  
+00006970: 2020 302e 3630 3620 2020 2020 7c20 2030    0.606     |  0
+00006980: 2e37 3037 2020 207c 0a7c 2020 2060 5669  .707   |.|   `Vi
+00006990: 5443 4c49 5045 7874 7261 6374 6f72 2e66  TCLIPExtractor.f
+000069a0: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+000069b0: 6f70 656e 6169 5f76 6974 6233 325f 3232  openai_vitb32_22
+000069c0: 3422 2960 2020 2020 7c20 2020 2020 2020  4")`    |       
+000069d0: 2020 2030 2e36 3132 2020 2020 2020 2020     0.612        
+000069e0: 2020 207c 2020 2020 2020 2030 2e34 3931     |       0.491
+000069f0: 2020 2020 2020 2020 7c20 2020 2030 2e35          |    0.5
+00006a00: 3630 2020 2020 207c 2020 302e 3639 3320  60     |  0.693 
+00006a10: 2020 7c0a 7c20 2020 6056 6954 434c 4950    |.|   `ViTCLIP
+00006a20: 4578 7472 6163 746f 722e 6672 6f6d 5f70  Extractor.from_p
+00006a30: 7265 7472 6169 6e65 6428 226f 7065 6e61  retrained("opena
+00006a40: 695f 7669 7462 3136 5f32 3234 2229 6020  i_vitb16_224")` 
+00006a50: 2020 207c 2020 2020 2020 2020 2020 302e     |          0.
+00006a60: 3634 3820 2020 2020 2020 2020 2020 7c20  648           | 
+00006a70: 2020 2020 2020 302e 3630 3620 2020 2020        0.606     
+00006a80: 2020 207c 2020 2020 302e 3636 3520 2020     |    0.665   
+00006a90: 2020 7c20 2030 2e37 3637 2020 207c 0a7c    |  0.767   |.|
+00006aa0: 2020 2060 5669 5443 4c49 5045 7874 7261     `ViTCLIPExtra
+00006ab0: 6374 6f72 2e66 726f 6d5f 7072 6574 7261  ctor.from_pretra
+00006ac0: 696e 6564 2822 6f70 656e 6169 5f76 6974  ined("openai_vit
+00006ad0: 6c31 345f 3232 3422 2960 2020 2020 7c20  l14_224")`    | 
+00006ae0: 2020 2020 2020 2020 2030 2e36 3730 2020           0.670  
+00006af0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00006b00: 2030 2e36 3735 2020 2020 2020 2020 7c20   0.675        | 
+00006b10: 2020 2030 2e37 3435 2020 2020 207c 2020     0.745     |  
+00006b20: 302e 3834 3420 2020 7c0a 7c20 2020 2020  0.844   |.|     
+00006b30: 2020 2060 5669 5445 7874 7261 6374 6f72     `ViTExtractor
+00006b40: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00006b50: 2822 7669 7473 3136 5f64 696e 6f22 2960  ("vits16_dino")`
+00006b60: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00006b70: 2020 2020 302e 3634 3820 2020 2020 2020      0.648       
+00006b80: 2020 2020 7c20 2020 2020 2020 302e 3530      |       0.50
+00006b90: 3920 2020 2020 2020 207c 2020 2020 302e  9        |    0.
+00006ba0: 3632 3720 2020 2020 7c20 2030 2e32 3635  627     |  0.265
+00006bb0: 2020 207c 0a7c 2020 2020 2020 2020 2060     |.|         `
+00006bc0: 5669 5445 7874 7261 6374 6f72 2e66 726f  ViTExtractor.fro
+00006bd0: 6d5f 7072 6574 7261 696e 6564 2822 7669  m_pretrained("vi
+00006be0: 7473 385f 6469 6e6f 2229 6020 2020 2020  ts8_dino")`     
+00006bf0: 2020 2020 7c20 2020 2020 2020 2020 2030      |          0
+00006c00: 2e36 3531 2020 2020 2020 2020 2020 207c  .651           |
+00006c10: 2020 2020 2020 2030 2e35 3234 2020 2020         0.524    
+00006c20: 2020 2020 7c20 2020 2030 2e36 3631 2020      |    0.661  
+00006c30: 2020 207c 2020 302e 3331 3520 2020 7c0a     |  0.315   |.
+00006c40: 7c20 2020 2020 2020 2060 5669 5445 7874  |        `ViTExt
+00006c50: 7261 6374 6f72 2e66 726f 6d5f 7072 6574  ractor.from_pret
+00006c60: 7261 696e 6564 2822 7669 7462 3136 5f64  rained("vitb16_d
+00006c70: 696e 6f22 2960 2020 2020 2020 2020 207c  ino")`         |
+00006c80: 2020 2020 2020 2020 2020 302e 3635 3820            0.658 
+00006c90: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00006ca0: 2020 302e 3531 3420 2020 2020 2020 207c    0.514        |
+00006cb0: 2020 2020 302e 3534 3120 2020 2020 7c20      0.541     | 
+00006cc0: 2030 2e32 3838 2020 207c 0a7c 2020 2020   0.288   |.|    
+00006cd0: 2020 2020 2060 5669 5445 7874 7261 6374       `ViTExtract
+00006ce0: 6f72 2e66 726f 6d5f 7072 6574 7261 696e  or.from_pretrain
+00006cf0: 6564 2822 7669 7462 385f 6469 6e6f 2229  ed("vitb8_dino")
+00006d00: 6020 2020 2020 2020 2020 7c20 2020 2020  `         |     
+00006d10: 2020 2020 2030 2e36 3839 2020 2020 2020       0.689      
+00006d20: 2020 2020 207c 2020 2020 2020 2030 2e35       |       0.5
+00006d30: 3939 2020 2020 2020 2020 7c20 2020 2030  99        |    0
+00006d40: 2e35 3036 2020 2020 207c 2020 302e 3331  .506     |  0.31
+00006d50: 3320 2020 7c0a 7c20 2020 2060 5265 736e  3   |.|    `Resn
+00006d60: 6574 4578 7472 6163 746f 722e 6672 6f6d  etExtractor.from
+00006d70: 5f70 7265 7472 6169 6e65 6428 2272 6573  _pretrained("res
+00006d80: 6e65 7435 305f 6d6f 636f 5f76 3222 2960  net50_moco_v2")`
+00006d90: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00006da0: 302e 3439 3320 2020 2020 2020 2020 2020  0.493           
+00006db0: 7c20 2020 2020 2020 302e 3236 3720 2020  |       0.267   
+00006dc0: 2020 2020 207c 2020 2020 302e 3236 3420       |    0.264 
+00006dd0: 2020 2020 7c20 2030 2e31 3439 2020 207c      |  0.149   |
+00006de0: 0a7c 2060 5265 736e 6574 4578 7472 6163  .| `ResnetExtrac
+00006df0: 746f 722e 6672 6f6d 5f70 7265 7472 6169  tor.from_pretrai
+00006e00: 6e65 6428 2272 6573 6e65 7435 305f 696d  ned("resnet50_im
+00006e10: 6167 656e 6574 316b 5f76 3122 2960 2020  agenet1k_v1")`  
+00006e20: 7c20 2020 2020 2020 2020 2030 2e35 3135  |          0.515
+00006e30: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00006e40: 2020 2030 2e32 3834 2020 2020 2020 2020     0.284        
+00006e50: 7c20 2020 2030 2e34 3535 2020 2020 207c  |    0.455     |
+00006e60: 2020 302e 3234 3720 2020 7c0a 0a2a 2a54    0.247   |..**T
+00006e70: 6865 206d 6574 7269 6373 206d 6179 2062  he metrics may b
+00006e80: 6520 6469 6666 6572 656e 7420 6672 6f6d  e different from
+00006e90: 2074 6865 206f 6e65 7320 7265 706f 7274   the ones report
+00006ea0: 6564 2062 7920 7061 7065 7273 2c0a 6265  ed by papers,.be
+00006eb0: 6361 7573 6520 7468 6520 7665 7273 696f  cause the versio
+00006ec0: 6e20 6f66 2074 7261 696e 2f76 616c 2073  n of train/val s
+00006ed0: 706c 6974 2061 6e64 2075 7361 6765 206f  plit and usage o
+00006ee0: 6620 626f 756e 6469 6e67 2062 6f78 6573  f bounding boxes
+00006ef0: 206d 6179 2064 6966 6665 722e 0a50 6172   may differ..Par
+00006f00: 7469 6375 6c61 726c 792c 2077 6520 7573  ticularly, we us
+00006f10: 6564 2062 6f75 6e64 696e 6720 626f 7865  ed bounding boxe
+00006f20: 7320 6475 7269 6e67 2074 6865 2065 7661  s during the eva
+00006f30: 6c75 6174 696f 6e2e 2a0a 0a23 2323 2048  luation.*..### H
+00006f40: 6f77 2074 6f20 7573 6520 6d6f 6465 6c73  ow to use models
+00006f50: 2066 726f 6d20 5a6f 6f3f 0a0a 5b63 6f6d   from Zoo?..[com
+00006f60: 6d65 6e74 5d3a 7a6f 6f2d 7374 6172 740a  ment]:zoo-start.
+00006f70: 6060 6070 7974 686f 6e0a 6672 6f6d 206f  ```python.from o
+00006f80: 6d6c 2e63 6f6e 7374 2069 6d70 6f72 7420  ml.const import 
+00006f90: 434b 5054 5f53 4156 455f 524f 4f54 2061  CKPT_SAVE_ROOT a
+00006fa0: 7320 434b 5054 5f44 4952 2c20 4d4f 434b  s CKPT_DIR, MOCK
+00006fb0: 5f44 4154 4153 4554 5f50 4154 4820 6173  _DATASET_PATH as
+00006fc0: 2044 4154 415f 4449 520a 6672 6f6d 206f   DATA_DIR.from o
+00006fd0: 6d6c 2e6d 6f64 656c 7320 696d 706f 7274  ml.models import
+00006fe0: 2056 6954 4578 7472 6163 746f 720a 6672   ViTExtractor.fr
+00006ff0: 6f6d 206f 6d6c 2e72 6567 6973 7472 792e  om oml.registry.
+00007000: 7472 616e 7366 6f72 6d73 2069 6d70 6f72  transforms impor
+00007010: 7420 6765 745f 7472 616e 7366 6f72 6d73  t get_transforms
+00007020: 5f66 6f72 5f70 7265 7472 6169 6e65 640a  _for_pretrained.
+00007030: 0a6d 6f64 656c 203d 2056 6954 4578 7472  .model = ViTExtr
+00007040: 6163 746f 722e 6672 6f6d 5f70 7265 7472  actor.from_pretr
+00007050: 6169 6e65 6428 2276 6974 7331 365f 6469  ained("vits16_di
+00007060: 6e6f 2229 0a74 7261 6e73 666f 726d 732c  no").transforms,
+00007070: 2069 6d5f 7265 6164 6572 203d 2067 6574   im_reader = get
+00007080: 5f74 7261 6e73 666f 726d 735f 666f 725f  _transforms_for_
+00007090: 7072 6574 7261 696e 6564 2822 7669 7473  pretrained("vits
+000070a0: 3136 5f64 696e 6f22 290a 0a69 6d67 203d  16_dino")..img =
+000070b0: 2069 6d5f 7265 6164 6572 2844 4154 415f   im_reader(DATA_
+000070c0: 4449 5220 2f20 2269 6d61 6765 7322 202f  DIR / "images" /
+000070d0: 2022 6369 7263 6c65 5f31 2e6a 7067 2229   "circle_1.jpg")
+000070e0: 2020 2320 7075 7420 7061 7468 2074 6f20    # put path to 
+000070f0: 796f 7572 2069 6d61 6765 2068 6572 650a  your image here.
+00007100: 696d 675f 7465 6e73 6f72 203d 2074 7261  img_tensor = tra
+00007110: 6e73 666f 726d 7328 696d 6729 0a23 2069  nsforms(img).# i
+00007120: 6d67 5f74 656e 736f 7220 3d20 7472 616e  mg_tensor = tran
+00007130: 7366 6f72 6d73 2869 6d61 6765 3d69 6d67  sforms(image=img
+00007140: 295b 2269 6d61 6765 225d 2020 2320 666f  )["image"]  # fo
+00007150: 7220 7472 616e 7366 6f72 6d73 2066 726f  r transforms fro
+00007160: 6d20 416c 6275 6d65 6e74 6174 696f 6e73  m Albumentations
+00007170: 0a0a 6665 6174 7572 6573 203d 206d 6f64  ..features = mod
+00007180: 656c 2869 6d67 5f74 656e 736f 722e 756e  el(img_tensor.un
+00007190: 7371 7565 657a 6528 3029 290a 0a23 2043  squeeze(0))..# C
+000071a0: 6865 636b 206f 7468 6572 2061 7661 696c  heck other avail
+000071b0: 6162 6c65 206d 6f64 656c 733a 0a70 7269  able models:.pri
+000071c0: 6e74 286c 6973 7428 5669 5445 7874 7261  nt(list(ViTExtra
+000071d0: 6374 6f72 2e70 7265 7472 6169 6e65 645f  ctor.pretrained_
+000071e0: 6d6f 6465 6c73 2e6b 6579 7328 2929 290a  models.keys())).
+000071f0: 0a23 204c 6f61 6420 6368 6563 6b70 6f69  .# Load checkpoi
+00007200: 6e74 2073 6176 6564 206f 6e20 6120 6469  nt saved on a di
+00007210: 736b 3a0a 6d6f 6465 6c5f 203d 2056 6954  sk:.model_ = ViT
+00007220: 4578 7472 6163 746f 7228 7765 6967 6874  Extractor(weight
+00007230: 733d 434b 5054 5f44 4952 202f 2022 7669  s=CKPT_DIR / "vi
+00007240: 7473 3136 5f64 696e 6f2e 636b 7074 222c  ts16_dino.ckpt",
+00007250: 2061 7263 683d 2276 6974 7331 3622 2c20   arch="vits16", 
+00007260: 6e6f 726d 616c 6973 655f 6665 6174 7572  normalise_featur
+00007270: 6573 3d46 616c 7365 290a 6060 600a 5b63  es=False).```.[c
+00007280: 6f6d 6d65 6e74 5d3a 7a6f 6f2d 656e 640a  omment]:zoo-end.
+00007290: 0a23 2320 5b43 6f6e 7472 6962 7574 696e  .## [Contributin
+000072a0: 6720 6775 6964 655d 2868 7474 7073 3a2f  g guide](https:/
+000072b0: 2f6f 7065 6e2d 6d65 7472 6963 2d6c 6561  /open-metric-lea
+000072c0: 726e 696e 672e 7265 6164 7468 6564 6f63  rning.readthedoc
+000072d0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6f  s.io/en/latest/o
+000072e0: 6d6c 2f63 6f6e 7472 6962 7574 696e 672e  ml/contributing.
+000072f0: 6874 6d6c 290a 0a57 6520 7765 6c63 6f6d  html)..We welcom
+00007300: 6520 6e65 7720 636f 6e74 7269 6275 746f  e new contributo
+00007310: 7273 2120 506c 6561 7365 2c20 7365 6520  rs! Please, see 
+00007320: 6f75 723a 0a2a 205b 436f 6e74 7269 6275  our:.* [Contribu
+00007330: 7469 6e67 2067 7569 6465 5d28 6874 7470  ting guide](http
+00007340: 733a 2f2f 6f70 656e 2d6d 6574 7269 632d  s://open-metric-
+00007350: 6c65 6172 6e69 6e67 2e72 6561 6474 6865  learning.readthe
+00007360: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00007370: 742f 6f6d 6c2f 636f 6e74 7269 6275 7469  t/oml/contributi
+00007380: 6e67 2e68 746d 6c29 0a2a 205b 4b61 6e62  ng.html).* [Kanb
+00007390: 616e 2062 6f61 7264 5d28 6874 7470 733a  an board](https:
+000073a0: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4d4c  //github.com/OML
+000073b0: 2d54 6561 6d2f 6f70 656e 2d6d 6574 7269  -Team/open-metri
+000073c0: 632d 6c65 6172 6e69 6e67 2f70 726f 6a65  c-learning/proje
+000073d0: 6374 732f 3129 0a0a 2323 2041 636b 6e6f  cts/1)..## Ackno
+000073e0: 776c 6564 676d 656e 7473 0a0a 3c61 2068  wledgments..<a h
+000073f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00007400: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+00007410: 2d74 6561 6d2f 6361 7461 6c79 7374 2220  -team/catalyst" 
+00007420: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00007430: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00007440: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00007450: 636f 6e74 656e 742e 636f 6d2f 6361 7461  content.com/cata
+00007460: 6c79 7374 2d74 6561 6d2f 6361 7461 6c79  lyst-team/cataly
+00007470: 7374 2d70 6963 732f 6d61 7374 6572 2f70  st-pics/master/p
+00007480: 6963 732f 6361 7461 6c79 7374 5f6c 6f67  ics/catalyst_log
+00007490: 6f2e 706e 6722 2077 6964 7468 3d22 3130  o.png" width="10
+000074a0: 3022 2f3e 3c2f 613e 0a0a 5468 6520 7072  0"/></a>..The pr
+000074b0: 6f6a 6563 7420 7761 7320 7374 6172 7465  oject was starte
+000074c0: 6420 696e 2032 3032 3020 6173 2061 206d  d in 2020 as a m
+000074d0: 6f64 756c 6520 666f 7220 5b43 6174 616c  odule for [Catal
+000074e0: 7973 745d 2868 7474 7073 3a2f 2f67 6974  yst](https://git
+000074f0: 6875 622e 636f 6d2f 6361 7461 6c79 7374  hub.com/catalyst
+00007500: 2d74 6561 6d2f 6361 7461 6c79 7374 2920  -team/catalyst) 
+00007510: 6c69 6272 6172 792e 0a49 2077 616e 7420  library..I want 
+00007520: 746f 2074 6861 6e6b 2070 656f 706c 6520  to thank people 
+00007530: 7768 6f20 776f 726b 6564 2077 6974 6820  who worked with 
+00007540: 6d65 206f 6e20 7468 6174 206d 6f64 756c  me on that modul
+00007550: 653a 0a5b 4a75 6c69 6120 5368 656e 7368  e:.[Julia Shensh
+00007560: 696e 615d 2868 7474 7073 3a2f 2f67 6974  ina](https://git
+00007570: 6875 622e 636f 6d2f 6a75 6c69 612d 7368  hub.com/julia-sh
+00007580: 656e 7368 696e 6129 2c0a 5b4e 696b 6974  enshina),.[Nikit
+00007590: 6120 4261 6c61 6761 6e73 6b79 5d28 6874  a Balagansky](ht
+000075a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000075b0: 2f65 6c65 7068 616e 746d 6970 7429 2c0a  /elephantmipt),.
+000075c0: 5b53 6572 6765 7920 4b6f 6c65 736e 696b  [Sergey Kolesnik
+000075d0: 6f76 5d28 6874 7470 733a 2f2f 6769 7468  ov](https://gith
+000075e0: 7562 2e63 6f6d 2f53 6369 7461 746f 7229  ub.com/Scitator)
+000075f0: 0a61 6e64 206f 7468 6572 732e 0a0a 4920  .and others...I 
+00007600: 776f 756c 6420 6c69 6b65 2074 6f20 7468  would like to th
+00007610: 616e 6b20 7065 6f70 6c65 2077 686f 2063  ank people who c
+00007620: 6f6e 7469 6e75 6520 776f 726b 696e 6720  ontinue working 
+00007630: 6f6e 2074 6869 7320 7069 7065 6c69 6e65  on this pipeline
+00007640: 2077 6865 6e20 6974 2062 6563 616d 6520   when it became 
+00007650: 6120 7365 7061 7265 2070 726f 6a65 6374  a separe project
+00007660: 3a0a 5b4a 756c 6961 2053 6865 6e73 6869  :.[Julia Shenshi
+00007670: 6e61 5d28 6874 7470 733a 2f2f 6769 7468  na](https://gith
+00007680: 7562 2e63 6f6d 2f6a 756c 6961 2d73 6865  ub.com/julia-she
+00007690: 6e73 6869 6e61 292c 0a5b 4d69 7368 6120  nshina),.[Misha 
+000076a0: 4b69 6e64 756c 6f76 5d28 6874 7470 733a  Kindulov](https:
+000076b0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 306e  //github.com/b0n
+000076c0: 6365 292c 0a5b 416c 656b 7365 6920 5461  ce),.[Aleksei Ta
+000076d0: 7261 736f 765d 2868 7474 7073 3a2f 2f67  rasov](https://g
+000076e0: 6974 6875 622e 636f 6d2f 4461 6c6f 726f  ithub.com/Daloro
+000076f0: 4154 2920 616e 640a 5b56 6572 6b68 6f76  AT) and.[Verkhov
+00007700: 7473 6576 204c 656f 6e69 645d 2868 7474  tsev Leonid](htt
+00007710: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00007720: 6c65 6f72 6f6d 616e 6f76 6963 6829 2e0a  leoromanovich)..
+00007730: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00007740: 2f2f 7777 772e 6e65 7779 6f72 6b65 722e  //www.newyorker.
+00007750: 6465 2f22 2074 6172 6765 743d 225f 626c  de/" target="_bl
+00007760: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
+00007770: 7474 7073 3a2f 2f75 706c 6f61 642e 7769  ttps://upload.wi
+00007780: 6b69 6d65 6469 612e 6f72 672f 7769 6b69  kimedia.org/wiki
+00007790: 7065 6469 612f 636f 6d6d 6f6e 732f 7468  pedia/commons/th
+000077a0: 756d 622f 642f 6438 2f4e 6577 5f59 6f72  umb/d/d8/New_Yor
+000077b0: 6b65 722e 7376 672f 3132 3830 7078 2d4e  ker.svg/1280px-N
+000077c0: 6577 5f59 6f72 6b65 722e 7376 672e 706e  ew_Yorker.svg.pn
+000077d0: 6722 2077 6964 7468 3d22 3130 3022 2f3e  g" width="100"/>
+000077e0: 3c2f 613e 0a0a 4920 616c 736f 2077 616e  </a>..I also wan
+000077f0: 7420 746f 2074 6861 6e6b 204e 6577 596f  t to thank NewYo
+00007800: 726b 6572 2c20 7369 6e63 6520 7468 6520  rker, since the 
+00007810: 7061 7274 206f 6620 6675 6e63 7469 6f6e  part of function
+00007820: 616c 6974 7920 7761 7320 6465 7665 6c6f  ality was develo
+00007830: 7065 6420 2861 6e64 2075 7365 6429 2062  ped (and used) b
+00007840: 7920 6974 7320 636f 6d70 7574 6572 2076  y its computer v
+00007850: 6973 696f 6e20 7465 616d 206c 6564 2062  ision team led b
+00007860: 7920 6d65 2e0a                           y me..
```

### Comparing `open-metric-learning-0.4.3/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-0.4.4/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
 oml/configs/extractor/extractor_with_mlp.yaml
 oml/configs/extractor/resnet.yaml
 oml/configs/extractor/vit.yaml
 oml/configs/extractor/vit_clip.yaml
 oml/configs/extractor/vit_unicom.yaml
+oml/configs/logger/neptune.yaml
+oml/configs/logger/tensorboard.yaml
+oml/configs/logger/wandb.yaml
 oml/configs/miner/all_triplets.yaml
 oml/configs/miner/hard_cluster.yaml
 oml/configs/miner/hard_triplets.yaml
 oml/configs/miner/miner_with_bank.yaml
 oml/configs/miner/n_hard_triplets.yaml
 oml/configs/miner/triplets_with_memory.yaml
 oml/configs/optimizer/adadelta.yaml
@@ -132,14 +135,15 @@
 oml/models/vit_dino/external/vision_transformer.py
 oml/models/vit_unicom/__init__.py
 oml/models/vit_unicom/extractor.py
 oml/models/vit_unicom/external/__init__.py
 oml/models/vit_unicom/external/model.py
 oml/models/vit_unicom/external/vision_transformer.py
 oml/registry/__init__.py
+oml/registry/loggers.py
 oml/registry/losses.py
 oml/registry/miners.py
 oml/registry/models.py
 oml/registry/optimizers.py
 oml/registry/postprocessors.py
 oml/registry/samplers.py
 oml/registry/schedulers.py
```

### Comparing `open-metric-learning-0.4.3/setup.py` & `open-metric-learning-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/tests/test_build_readme.py` & `open-metric-learning-0.4.4/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/tests/test_imports.py` & `open-metric-learning-0.4.4/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-0.4.3/tests/test_outdated_docs.py` & `open-metric-learning-0.4.4/tests/test_outdated_docs.py`

 * *Files identical despite different names*

