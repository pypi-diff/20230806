# Comparing `tmp/aim-4.0.0a7.tar.gz` & `tmp/aim-4.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim-4.0.0a7.tar", last modified: Mon Jun  5 20:56:04 2023, max compression
+gzip compressed data, was "aim-4.0.0a9.tar", last modified: Fri Jun 16 17:32:43 2023, max compression
```

## Comparing `aim-4.0.0a7.tar` & `aim-4.0.0a9.tar`

### file list

```diff
@@ -1,310 +1,370 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.387370 aim-4.0.0a7/
--rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0a7/LICENSE
--rw-r--r--   0 github     (503) staff       (20)      177 2023-06-02 20:14:20.000000 aim-4.0.0a7/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)    38876 2023-06-05 20:56:04.387189 aim-4.0.0a7/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    38192 2023-06-02 20:14:20.000000 aim-4.0.0a7/README.md
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.329457 aim-4.0.0a7/aim.egg-info/
--rw-r--r--   0 github     (503) staff       (20)    38876 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)     9826 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)      110 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      413 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)       21 2023-06-05 20:56:04.000000 aim-4.0.0a7/aim.egg-info/top_level.txt
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.324576 aim-4.0.0a7/pkgs/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.329558 aim-4.0.0a7/pkgs/aimstack/
--rw-r--r--   0 github     (503) staff       (20)       24 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.329807 aim-4.0.0a7/pkgs/aimstack/asp/
--rw-r--r--   0 github     (503) staff       (20)      391 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.330413 aim-4.0.0a7/pkgs/aimstack/asp/models/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.330708 aim-4.0.0a7/pkgs/aimstack/asp/models/logging/
--rw-r--r--   0 github     (503) staff       (20)     1707 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/logging/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.331652 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3239 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4220 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     5169 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/figures.py
--rw-r--r--   0 github     (503) staff       (20)     9903 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.331900 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/io/wavfile.py
--rw-r--r--   0 github     (503) staff       (20)      682 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/objects/text.py
--rw-r--r--   0 github     (503) staff       (20)     8071 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/run.py
--rw-r--r--   0 github     (503) staff       (20)     2761 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/asp/models/sequences.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.332383 aim-4.0.0a7/pkgs/aimstack/ml/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.337013 aim-4.0.0a7/pkgs/aimstack/ml/adapters/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3526 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/acme.py
--rw-r--r--   0 github     (503) staff       (20)     4652 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/catboost.py
--rw-r--r--   0 github     (503) staff       (20)     6458 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/fastai.py
--rw-r--r--   0 github     (503) staff       (20)     6608 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)     3439 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras.py
--rw-r--r--   0 github     (503) staff       (20)     1086 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras_mixins.py
--rw-r--r--   0 github     (503) staff       (20)     3715 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)     3814 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)     9019 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)     7297 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/optuna.py
--rw-r--r--   0 github     (503) staff       (20)     3573 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/paddle.py
--rw-r--r--   0 github     (503) staff       (20)     3740 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/prophet.py
--rw-r--r--   0 github     (503) staff       (20)     2346 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)     9514 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)     6870 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)     4708 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/sb3.py
--rw-r--r--   0 github     (503) staff       (20)     3460 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)     3833 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/adapters/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.337797 aim-4.0.0a7/pkgs/aimstack/ml/models/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/models/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6101 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/models/deeplake_dataset.py
--rw-r--r--   0 github     (503) staff       (20)     1963 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/models/dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     3628 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/models/hf_datasets_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1251 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/models/hub_dataset.py
--rw-r--r--   0 github     (503) staff       (20)     2204 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/ml/training_flow.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.338263 aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1273 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/run.py
--rw-r--r--   0 github     (503) staff       (20)     9323 2023-06-02 20:14:20.000000 aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/tracker.py
--rw-r--r--   0 github     (503) staff       (20)      880 2023-06-02 20:14:20.000000 aim-4.0.0a7/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)       38 2023-06-05 20:56:04.387411 aim-4.0.0a7/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     7054 2023-06-02 20:14:20.000000 aim-4.0.0a7/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.326782 aim-4.0.0a7/src/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.338530 aim-4.0.0a7/src/aimcore/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.339138 aim-4.0.0a7/src/aimcore/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      130 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1599 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      478 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/callbacks/helpers.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.339340 aim-4.0.0a7/src/aimcore/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cleanup/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.340440 aim-4.0.0a7/src/aimcore/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      872 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/cli.py
--rw-r--r--   0 github     (503) staff       (20)      166 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.340796 aim-4.0.0a7/src/aimcore/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3004 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.341498 aim-4.0.0a7/src/aimcore/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5916 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10374 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6820 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.341748 aim-4.0.0a7/src/aimcore/cli/init/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/init/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1459 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/init/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.342071 aim-4.0.0a7/src/aimcore/cli/server/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/server/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2983 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/server/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.342312 aim-4.0.0a7/src/aimcore/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4082 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.342571 aim-4.0.0a7/src/aimcore/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      304 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.343025 aim-4.0.0a7/src/aimcore/cli/up/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/up/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5195 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/up/commands.py
--rw-r--r--   0 github     (503) staff       (20)     1673 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/up/utils.py
--rw-r--r--   0 github     (503) staff       (20)      371 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.343291 aim-4.0.0a7/src/aimcore/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      149 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9963 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/cli/watcher_cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.343475 aim-4.0.0a7/src/aimcore/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31151 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/reporter/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.345995 aim-4.0.0a7/src/aimcore/transport/
--rw-r--r--   0 github     (503) staff       (20)       27 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     9268 2023-06-05 09:07:45.000000 aim-4.0.0a7/src/aimcore/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)      563 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/config.py
--rw-r--r--   0 github     (503) staff       (20)     1850 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/handlers.py
--rw-r--r--   0 github     (503) staff       (20)     5460 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/heartbeat.py
--rw-r--r--   0 github     (503) staff       (20)     3095 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/message_utils.py
--rw-r--r--   0 github     (503) staff       (20)      445 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/remote_resource.py
--rw-r--r--   0 github     (503) staff       (20)     1433 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/router.py
--rw-r--r--   0 github     (503) staff       (20)     3692 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/rpc_queue.py
--rw-r--r--   0 github     (503) staff       (20)     4326 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/server.py
--rw-r--r--   0 github     (503) staff       (20)     6086 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/transport/tracking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.346813 aim-4.0.0a7/src/aimcore/web/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.347926 aim-4.0.0a7/src/aimcore/web/api/
--rw-r--r--   0 github     (503) staff       (20)     3395 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.348744 aim-4.0.0a7/src/aimcore/web/api/boards/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/boards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1817 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/boards/models.py
--rw-r--r--   0 github     (503) staff       (20)      149 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/boards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     1147 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/boards/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.349555 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      920 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/models.py
--rw-r--r--   0 github     (503) staff       (20)      542 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      449 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2994 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.350372 aim-4.0.0a7/src/aimcore/web/api/dashboards/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      648 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboards/models.py
--rw-r--r--   0 github     (503) staff       (20)      652 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      783 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboards/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     3365 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/dashboards/views.py
--rw-r--r--   0 github     (503) staff       (20)      825 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/db.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.350941 aim-4.0.0a7/src/aimcore/web/api/projects/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/projects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      628 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/projects/project.py
--rw-r--r--   0 github     (503) staff       (20)     1272 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/projects/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     3737 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/projects/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.351187 aim-4.0.0a7/src/aimcore/web/api/queries/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/queries/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6829 2023-06-05 20:55:55.000000 aim-4.0.0a7/src/aimcore/web/api/queries/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.351714 aim-4.0.0a7/src/aimcore/web/api/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     4488 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/runs/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)    14449 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/runs/utils.py
--rw-r--r--   0 github     (503) staff       (20)    13193 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/runs/views.py
--rw-r--r--   0 github     (503) staff       (20)     3124 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/utils.py
--rw-r--r--   0 github     (503) staff       (20)     1597 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/api/views.py
--rw-r--r--   0 github     (503) staff       (20)      432 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.351968 aim-4.0.0a7/src/aimcore/web/middlewares/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/middlewares/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3654 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/middlewares/profiler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.353042 aim-4.0.0a7/src/aimcore/web/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/README
--rw-r--r--   0 github     (503) staff       (20)      800 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)      797 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2717 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/script.py.mako
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.359320 aim-4.0.0a7/src/aimcore/web/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2183 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/versions/11672b13f92c_.py
--rw-r--r--   0 github     (503) staff       (20)     1545 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/versions/517a45b2e62c_.py
--rw-r--r--   0 github     (503) staff       (20)     5592 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/versions/5ae8371b7481_.py
--rw-r--r--   0 github     (503) staff       (20)     7262 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/versions/73a3d004c227_.py
--rw-r--r--   0 github     (503) staff       (20)     1788 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py
--rw-r--r--   0 github     (503) staff       (20)       59 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/run.py
--rw-r--r--   0 github     (503) staff       (20)     3281 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/aimcore/web/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.326828 aim-4.0.0a7/src/py-sdk/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.361119 aim-4.0.0a7/src/py-sdk/aim/
--rw-r--r--   0 github     (503) staff       (20)        8 2023-06-05 20:55:55.000000 aim-4.0.0a7/src/py-sdk/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)      825 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/__about__.py
--rw-r--r--   0 github     (503) staff       (20)      622 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/__version__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.361273 aim-4.0.0a7/src/py-sdk/aim/_core/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.372931 aim-4.0.0a7/src/py-sdk/aim/_core/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   459259 2023-06-05 20:56:00.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3051 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/arrayview.py
--rw-r--r--   0 github     (503) staff       (20)   935599 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.cpp
--rw-r--r--   0 github     (503) staff       (20)      977 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.pxd
--rw-r--r--   0 github     (503) staff       (20)    12306 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.py
--rw-r--r--   0 github     (503) staff       (20)   944965 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/containertreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      337 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     6727 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/containertreeview.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.374316 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   149167 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      167 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)      107 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   380498 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7427 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   356452 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5980 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.375630 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   142042 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       97 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       56 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   206140 2023-06-05 20:56:01.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)     1083 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.375729 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   394398 2023-06-05 20:56:02.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1021 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5580 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   679035 2023-06-05 20:56:02.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      202 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4365 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     7858 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/locking.py
--rw-r--r--   0 github     (503) staff       (20)     1670 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/object.py
--rw-r--r--   0 github     (503) staff       (20)   979988 2023-06-05 20:56:02.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.cpp
--rw-r--r--   0 github     (503) staff       (20)      808 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.pxd
--rw-r--r--   0 github     (503) staff       (20)    12274 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/proxy.py
--rw-r--r--   0 github     (503) staff       (20)  1052655 2023-06-05 20:56:02.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/rockscontainer.cpp
--rw-r--r--   0 github     (503) staff       (20)    19808 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/rockscontainer.pyx
--rw-r--r--   0 github     (503) staff       (20)   706262 2023-06-05 20:56:02.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      263 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3044 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   728377 2023-06-05 20:56:03.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8419 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      713 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   528574 2023-06-05 20:56:03.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2914 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)     1363 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   817777 2023-06-05 20:56:03.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/union.cpp
--rw-r--r--   0 github     (503) staff       (20)     7943 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/union.pyx
--rw-r--r--   0 github     (503) staff       (20)   817782 2023-06-05 20:56:03.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/storage/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.376627 aim-4.0.0a7/src/py-sdk/aim/_core/utils/
--rw-r--r--   0 github     (503) staff       (20)       85 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1209 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_core/utils/deprecation.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.376872 aim-4.0.0a7/src/py-sdk/aim/_ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2021 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/exception_resistant.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.377359 aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2625 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/manager.py
--rw-r--r--   0 github     (503) staff       (20)     7169 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.379125 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      593 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1859 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      523 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1429 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1162 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      525 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1035 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      863 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.381092 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/
--rw-r--r--   0 github     (503) staff       (20)      152 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/configs.py
--rw-r--r--   0 github     (503) staff       (20)   148706 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/pynvml.py
--rw-r--r--   0 github     (503) staff       (20)     7798 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     6719 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/stat.py
--rw-r--r--   0 github     (503) staff       (20)     2225 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.381383 aim-4.0.0a7/src/py-sdk/aim/_ext/tracking/
--rw-r--r--   0 github     (503) staff       (20)     4755 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_ext/tracking/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.386439 aim-4.0.0a7/src/py-sdk/aim/_sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)       48 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/blob.py
--rw-r--r--   0 github     (503) staff       (20)     9778 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/collections.py
--rw-r--r--   0 github     (503) staff       (20)      276 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/configs.py
--rw-r--r--   0 github     (503) staff       (20)      519 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/constants.py
--rw-r--r--   0 github     (503) staff       (20)    10619 2023-06-05 09:07:45.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/container.py
--rw-r--r--   0 github     (503) staff       (20)     1837 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/context.py
--rw-r--r--   0 github     (503) staff       (20)      561 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/exceptions.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-05 20:56:04.386860 aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1224 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/container.py
--rw-r--r--   0 github     (503) staff       (20)     2196 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     2983 2023-06-05 09:07:45.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/local_storage.py
--rw-r--r--   0 github     (503) staff       (20)     6542 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/lock_manager.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/num_utils.py
--rw-r--r--   0 github     (503) staff       (20)     1681 2023-06-05 20:55:55.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/object.py
--rw-r--r--   0 github     (503) staff       (20)     2805 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/package_utils.py
--rw-r--r--   0 github     (503) staff       (20)     4221 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/query.py
--rw-r--r--   0 github     (503) staff       (20)     3046 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)    15262 2023-06-05 09:07:45.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/remote_storage.py
--rw-r--r--   0 github     (503) staff       (20)     8367 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/repo.py
--rw-r--r--   0 github     (503) staff       (20)    12647 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/sequence.py
--rw-r--r--   0 github     (503) staff       (20)      855 2023-06-05 09:07:45.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/storage_engine.py
--rw-r--r--   0 github     (503) staff       (20)     3845 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/type_utils.py
--rw-r--r--   0 github     (503) staff       (20)      165 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/types.py
--rw-r--r--   0 github     (503) staff       (20)     1479 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     1539 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/_sdk/utils.py
--rw-r--r--   0 github     (503) staff       (20)       54 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/container.py
--rw-r--r--   0 github     (503) staff       (20)       48 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/object.py
--rw-r--r--   0 github     (503) staff       (20)       44 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/repo.py
--rw-r--r--   0 github     (503) staff       (20)       52 2023-06-02 20:14:20.000000 aim-4.0.0a7/src/py-sdk/aim/sequence.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.402362 aim-4.0.0a9/
+-rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0a9/LICENSE
+-rw-r--r--   0 github     (503) staff       (20)      214 2023-06-16 17:32:34.000000 aim-4.0.0a9/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)    38876 2023-06-16 17:32:43.402162 aim-4.0.0a9/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    38192 2023-06-02 20:14:20.000000 aim-4.0.0a9/README.md
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.333442 aim-4.0.0a9/aim.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)    38876 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    11818 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)      110 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      413 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)       21 2023-06-16 17:32:43.000000 aim-4.0.0a9/aim.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.327355 aim-4.0.0a9/pkgs/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.333681 aim-4.0.0a9/pkgs/aimstack/
+-rw-r--r--   0 github     (503) staff       (20)       24 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.333942 aim-4.0.0a9/pkgs/aimstack/asp/
+-rw-r--r--   0 github     (503) staff       (20)      427 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/asp/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.334191 aim-4.0.0a9/pkgs/aimstack/asp/boards/
+-rw-r--r--   0 github     (503) staff       (20)       34 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/boards/custom-board.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.327594 aim-4.0.0a9/pkgs/aimstack/asp/boards/metrics/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.334443 aim-4.0.0a9/pkgs/aimstack/asp/boards/metrics/loss/
+-rw-r--r--   0 github     (503) staff       (20)       34 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/boards/metrics/loss/run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.334752 aim-4.0.0a9/pkgs/aimstack/asp/boards/test/
+-rw-r--r--   0 github     (503) staff       (20)      174 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/boards/test/run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.335242 aim-4.0.0a9/pkgs/aimstack/asp/models/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.336089 aim-4.0.0a9/pkgs/aimstack/asp/models/logging/
+-rw-r--r--   0 github     (503) staff       (20)     1707 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/logging/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.337391 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3240 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4220 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     5169 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/figures.py
+-rw-r--r--   0 github     (503) staff       (20)     9904 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.337755 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/io/wavfile.py
+-rw-r--r--   0 github     (503) staff       (20)      682 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/objects/text.py
+-rw-r--r--   0 github     (503) staff       (20)     8234 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/run.py
+-rw-r--r--   0 github     (503) staff       (20)     2881 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/asp/models/sequences.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.338188 aim-4.0.0a9/pkgs/aimstack/demo/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/demo/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.338787 aim-4.0.0a9/pkgs/aimstack/demo/boards/
+-rw-r--r--   0 github     (503) staff       (20)     1967 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/demo/boards/charts.py
+-rw-r--r--   0 github     (503) staff       (20)      900 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/demo/boards/data_display_elements.py
+-rw-r--r--   0 github     (503) staff       (20)     3820 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/demo/boards/input_components.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.338987 aim-4.0.0a9/pkgs/aimstack/docs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.328280 aim-4.0.0a9/pkgs/aimstack/docs/boards/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.339604 aim-4.0.0a9/pkgs/aimstack/docs/boards/sdk/
+-rw-r--r--   0 github     (503) staff       (20)     5072 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4528 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/sdk/aim_types.py
+-rw-r--r--   0 github     (503) staff       (20)     4444 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/sdk/container.py
+-rw-r--r--   0 github     (503) staff       (20)     6979 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/sdk/sequence.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.328806 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.339923 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/board/
+-rw-r--r--   0 github     (503) staff       (20)      527 2023-06-16 17:32:34.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/board/board.py
+-rw-r--r--   0 github     (503) staff       (20)      833 2023-06-16 17:32:34.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/board/board_link.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.340282 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/charts/
+-rw-r--r--   0 github     (503) staff       (20)     1547 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/charts/line_chart.py
+-rw-r--r--   0 github     (503) staff       (20)     1001 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/charts/plotly.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.341049 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/data_viz/
+-rw-r--r--   0 github     (503) staff       (20)      764 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/data_viz/dataframe.py
+-rw-r--r--   0 github     (503) staff       (20)      477 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/data_viz/html.py
+-rw-r--r--   0 github     (503) staff       (20)      713 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/data_viz/json.py
+-rw-r--r--   0 github     (503) staff       (20)      702 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/data_viz/table.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.343097 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/
+-rw-r--r--   0 github     (503) staff       (20)      728 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/checkbox.py
+-rw-r--r--   0 github     (503) staff       (20)     1207 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/multi_select.py
+-rw-r--r--   0 github     (503) staff       (20)     1153 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/number_input.py
+-rw-r--r--   0 github     (503) staff       (20)     1400 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/radio.py
+-rw-r--r--   0 github     (503) staff       (20)     1173 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/range_slider.py
+-rw-r--r--   0 github     (503) staff       (20)     1007 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/select.py
+-rw-r--r--   0 github     (503) staff       (20)     1067 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/slider.py
+-rw-r--r--   0 github     (503) staff       (20)      937 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/switch.py
+-rw-r--r--   0 github     (503) staff       (20)     1000 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/text_area.py
+-rw-r--r--   0 github     (503) staff       (20)      751 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/text_input.py
+-rw-r--r--   0 github     (503) staff       (20)     1182 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/input/toggle_button.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.343863 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/layout_containers/
+-rw-r--r--   0 github     (503) staff       (20)     1141 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/layout_containers/columns.py
+-rw-r--r--   0 github     (503) staff       (20)     1125 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/layout_containers/form.py
+-rw-r--r--   0 github     (503) staff       (20)     1023 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/layout_containers/rows.py
+-rw-r--r--   0 github     (503) staff       (20)     1452 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/layout_containers/tabs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.344375 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/sequence_viz/
+-rw-r--r--   0 github     (503) staff       (20)      414 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/sequence_viz/audios.py
+-rw-r--r--   0 github     (503) staff       (20)      422 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/sequence_viz/figures.py
+-rw-r--r--   0 github     (503) staff       (20)      414 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/sequence_viz/images.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.345262 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/
+-rw-r--r--   0 github     (503) staff       (20)      524 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/code.py
+-rw-r--r--   0 github     (503) staff       (20)      428 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/header.py
+-rw-r--r--   0 github     (503) staff       (20)      606 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/link.py
+-rw-r--r--   0 github     (503) staff       (20)      452 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/subheader.py
+-rw-r--r--   0 github     (503) staff       (20)      434 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/docs/boards/ui/text/text.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.345563 aim-4.0.0a9/pkgs/aimstack/ml/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.349818 aim-4.0.0a9/pkgs/aimstack/ml/adapters/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3526 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/acme.py
+-rw-r--r--   0 github     (503) staff       (20)     4652 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)     6458 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)     6608 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)     3439 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras.py
+-rw-r--r--   0 github     (503) staff       (20)     1086 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras_mixins.py
+-rw-r--r--   0 github     (503) staff       (20)     3715 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)     3814 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)     9019 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)     7297 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)     3573 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)     3740 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)     2298 2023-06-16 16:41:18.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)     9514 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)     6870 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)     4708 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)     3460 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     3833 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/adapters/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.350553 aim-4.0.0a9/pkgs/aimstack/ml/models/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/models/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6101 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/models/deeplake_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)     1963 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/models/dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     3628 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/models/hf_datasets_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1251 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/models/hub_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)     2204 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/ml/training_flow.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.351049 aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1273 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/run.py
+-rw-r--r--   0 github     (503) staff       (20)     9323 2023-06-02 20:14:20.000000 aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)      898 2023-06-16 16:41:18.000000 aim-4.0.0a9/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)       38 2023-06-16 17:32:43.402401 aim-4.0.0a9/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     7054 2023-06-02 20:14:20.000000 aim-4.0.0a9/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.330736 aim-4.0.0a9/src/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.351486 aim-4.0.0a9/src/aimcore/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.352459 aim-4.0.0a9/src/aimcore/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      130 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1599 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      478 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/callbacks/helpers.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.358558 aim-4.0.0a9/src/aimcore/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cleanup/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.359674 aim-4.0.0a9/src/aimcore/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      872 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/cli.py
+-rw-r--r--   0 github     (503) staff       (20)      166 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.360035 aim-4.0.0a9/src/aimcore/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3004 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.360702 aim-4.0.0a9/src/aimcore/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5916 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10374 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6820 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.360952 aim-4.0.0a9/src/aimcore/cli/init/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/init/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1459 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/init/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.361210 aim-4.0.0a9/src/aimcore/cli/server/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/server/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2983 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/server/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.361449 aim-4.0.0a9/src/aimcore/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4082 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.361765 aim-4.0.0a9/src/aimcore/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      304 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.362150 aim-4.0.0a9/src/aimcore/cli/up/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/up/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5195 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/up/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     1673 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/up/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      371 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.362392 aim-4.0.0a9/src/aimcore/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      149 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9963 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/cli/watcher_cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.362563 aim-4.0.0a9/src/aimcore/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31151 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/reporter/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.364701 aim-4.0.0a9/src/aimcore/transport/
+-rw-r--r--   0 github     (503) staff       (20)       27 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     9365 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/aimcore/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)      563 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/config.py
+-rw-r--r--   0 github     (503) staff       (20)     1850 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/handlers.py
+-rw-r--r--   0 github     (503) staff       (20)     5460 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/heartbeat.py
+-rw-r--r--   0 github     (503) staff       (20)     3095 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/message_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      445 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/remote_resource.py
+-rw-r--r--   0 github     (503) staff       (20)     1433 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/router.py
+-rw-r--r--   0 github     (503) staff       (20)     3692 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/rpc_queue.py
+-rw-r--r--   0 github     (503) staff       (20)     4326 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/server.py
+-rw-r--r--   0 github     (503) staff       (20)     6086 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/transport/tracking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.365476 aim-4.0.0a9/src/aimcore/web/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.366379 aim-4.0.0a9/src/aimcore/web/api/
+-rw-r--r--   0 github     (503) staff       (20)     3395 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.367126 aim-4.0.0a9/src/aimcore/web/api/boards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/boards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1817 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/boards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      139 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/aimcore/web/api/boards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     1147 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/boards/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.368157 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      920 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/models.py
+-rw-r--r--   0 github     (503) staff       (20)      542 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      449 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2994 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.369192 aim-4.0.0a9/src/aimcore/web/api/dashboards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      648 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      652 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      783 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboards/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     3365 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/dashboards/views.py
+-rw-r--r--   0 github     (503) staff       (20)      825 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.369925 aim-4.0.0a9/src/aimcore/web/api/projects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/projects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      628 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/projects/project.py
+-rw-r--r--   0 github     (503) staff       (20)     1272 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/projects/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     3529 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/aimcore/web/api/projects/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.370215 aim-4.0.0a9/src/aimcore/web/api/queries/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/queries/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     8757 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/aimcore/web/api/queries/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.370918 aim-4.0.0a9/src/aimcore/web/api/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     4488 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/runs/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)    14449 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/runs/utils.py
+-rw-r--r--   0 github     (503) staff       (20)    13193 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/runs/views.py
+-rw-r--r--   0 github     (503) staff       (20)     3124 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1597 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/api/views.py
+-rw-r--r--   0 github     (503) staff       (20)      432 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.371190 aim-4.0.0a9/src/aimcore/web/middlewares/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/middlewares/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3654 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/middlewares/profiler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.372169 aim-4.0.0a9/src/aimcore/web/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)      800 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)      797 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2717 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/script.py.mako
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.372988 aim-4.0.0a9/src/aimcore/web/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2183 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/versions/11672b13f92c_.py
+-rw-r--r--   0 github     (503) staff       (20)     1545 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/versions/517a45b2e62c_.py
+-rw-r--r--   0 github     (503) staff       (20)     5592 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/versions/5ae8371b7481_.py
+-rw-r--r--   0 github     (503) staff       (20)     7262 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/versions/73a3d004c227_.py
+-rw-r--r--   0 github     (503) staff       (20)     1788 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py
+-rw-r--r--   0 github     (503) staff       (20)       59 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3281 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/aimcore/web/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.330781 aim-4.0.0a9/src/py-sdk/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.374973 aim-4.0.0a9/src/py-sdk/aim/
+-rw-r--r--   0 github     (503) staff       (20)        8 2023-06-16 17:32:34.000000 aim-4.0.0a9/src/py-sdk/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)      825 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/__about__.py
+-rw-r--r--   0 github     (503) staff       (20)      622 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/__version__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.375139 aim-4.0.0a9/src/py-sdk/aim/_core/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.386644 aim-4.0.0a9/src/py-sdk/aim/_core/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   459259 2023-06-16 17:32:39.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3051 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/arrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   935063 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.cpp
+-rw-r--r--   0 github     (503) staff       (20)      977 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)    12336 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.py
+-rw-r--r--   0 github     (503) staff       (20)   944965 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/containertreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      337 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     6727 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/containertreeview.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.388104 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   149167 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      167 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)      107 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   380498 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7427 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   356452 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5980 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.389433 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   142042 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       97 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       56 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   206140 2023-06-16 17:32:40.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)     1083 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.389547 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   394398 2023-06-16 17:32:41.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1021 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5580 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   679035 2023-06-16 17:32:41.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      202 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4365 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     7858 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/locking.py
+-rw-r--r--   0 github     (503) staff       (20)     1670 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/object.py
+-rw-r--r--   0 github     (503) staff       (20)   979988 2023-06-16 17:32:41.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      808 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.pxd
+-rw-r--r--   0 github     (503) staff       (20)    12274 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)  1052655 2023-06-16 17:32:41.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/rockscontainer.cpp
+-rw-r--r--   0 github     (503) staff       (20)    19808 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/rockscontainer.pyx
+-rw-r--r--   0 github     (503) staff       (20)   706262 2023-06-16 17:32:41.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3044 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   728377 2023-06-16 17:32:42.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8419 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      713 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   528574 2023-06-16 17:32:42.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2914 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1363 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   817777 2023-06-16 17:32:42.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/union.cpp
+-rw-r--r--   0 github     (503) staff       (20)     7943 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/union.pyx
+-rw-r--r--   0 github     (503) staff       (20)   817782 2023-06-16 17:32:42.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/storage/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.390004 aim-4.0.0a9/src/py-sdk/aim/_core/utils/
+-rw-r--r--   0 github     (503) staff       (20)       85 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1209 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_core/utils/deprecation.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.390244 aim-4.0.0a9/src/py-sdk/aim/_ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2021 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/exception_resistant.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.390761 aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2625 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/manager.py
+-rw-r--r--   0 github     (503) staff       (20)     7169 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.392612 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      593 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1859 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      523 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1429 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1162 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      525 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1035 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      863 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.394560 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/
+-rw-r--r--   0 github     (503) staff       (20)      152 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/configs.py
+-rw-r--r--   0 github     (503) staff       (20)   148706 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/pynvml.py
+-rw-r--r--   0 github     (503) staff       (20)     7798 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     6719 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     2225 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.394844 aim-4.0.0a9/src/py-sdk/aim/_ext/tracking/
+-rw-r--r--   0 github     (503) staff       (20)     4755 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_ext/tracking/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.401410 aim-4.0.0a9/src/py-sdk/aim/_sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/blob.py
+-rw-r--r--   0 github     (503) staff       (20)     9778 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/collections.py
+-rw-r--r--   0 github     (503) staff       (20)      276 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      519 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/constants.py
+-rw-r--r--   0 github     (503) staff       (20)    11010 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/container.py
+-rw-r--r--   0 github     (503) staff       (20)     1837 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/context.py
+-rw-r--r--   0 github     (503) staff       (20)      561 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/exceptions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-06-16 17:32:43.401863 aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1224 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/container.py
+-rw-r--r--   0 github     (503) staff       (20)     2196 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     2983 2023-06-05 09:07:45.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/local_storage.py
+-rw-r--r--   0 github     (503) staff       (20)     6542 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/lock_manager.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/num_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1313 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/object.py
+-rw-r--r--   0 github     (503) staff       (20)     2805 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/package_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     4221 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/query.py
+-rw-r--r--   0 github     (503) staff       (20)     3046 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)    15262 2023-06-05 09:07:45.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/remote_storage.py
+-rw-r--r--   0 github     (503) staff       (20)     8888 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/repo.py
+-rw-r--r--   0 github     (503) staff       (20)    13214 2023-06-16 16:41:18.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      855 2023-06-05 09:07:45.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/storage_engine.py
+-rw-r--r--   0 github     (503) staff       (20)     3845 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/type_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      165 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/types.py
+-rw-r--r--   0 github     (503) staff       (20)     1479 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     1539 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/_sdk/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       54 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/container.py
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/object.py
+-rw-r--r--   0 github     (503) staff       (20)       44 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/repo.py
+-rw-r--r--   0 github     (503) staff       (20)       52 2023-06-02 20:14:20.000000 aim-4.0.0a9/src/py-sdk/aim/sequence.py
```

### Comparing `aim-4.0.0a7/LICENSE` & `aim-4.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/PKG-INFO` & `aim-4.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0a7
+Version: 4.0.0a9
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0a7 Summary: A super-easy way to
+Metadata-Version: 2.1 Name: aim Version: 4.0.0a9 Summary: A super-easy way to
 record, search and compare AI experiments. Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `aim-4.0.0a7/README.md` & `aim-4.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/aim.egg-info/PKG-INFO` & `aim-4.0.0a9/aim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0a7
+Version: 4.0.0a9
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0a7 Summary: A super-easy way to
+Metadata-Version: 2.1 Name: aim Version: 4.0.0a9 Summary: A super-easy way to
 record, search and compare AI experiments. Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/logging/__init__.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/audio.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
          data: file path, bytes, io.BaseIO or numpy.array (only for WAV)
          format (:obj:`str`): Format of the audio source
          rate (:obj:`int`): Rate of the audio file, for WAV defaults to 22500
          caption (:obj:`str`, optional): Optional audio caption. '' by default.
     """
 
     AIM_NAME = 'aim.Audio'
-    RESOLVE_BLOBS = True
+    RESOLVE_BLOBS = False
 
     # supported audio formats
     UNKNOWN = ''
     MP3 = 'mp3'
     WAV = 'wav'
     FLAC = 'flac'
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/distribution.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/distribution.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/figures.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/figures.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/image.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         optimize=True,
         quality=85
     """
 
     DEFAULT_IMG_FORMAT = 'png'
     FLAG_WARN_RGBA_RGB = False
     AIM_NAME = 'aim.Image'
-    RESOLVE_BLOBS = True
+    RESOLVE_BLOBS = False
 
     def __init__(self, image, caption: str = '', format=None, quality=90, optimize=False):
         super().__init__()
 
         params = {
             'format': format,
             'quality': quality,
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/io/wavfile.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/objects/text.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/objects/text.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/run.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     LogStream,
     LogRecord,
     LogRecordSequence
 )
 
 from .sequences import (
     Metric,
+    SystemMetric,
     TextSequence,
     ImageSequence,
     AudioSequence,
     DistributionSequence,
     FigureSequence,
     Figure3DSequence
 )
@@ -61,21 +62,25 @@
             }
 
             self.repo.resource_tracker.register(self)
             self.repo.resource_tracker.start()
 
     @events.on.logs_collected
     def track_terminal_logs(self, log_lines: List[Tuple[str, int]], **kwargs):
+        if self._state.get('cleanup'):
+            return
         for (line, line_num) in log_lines:
             self.logs.track(LogLine(line), step=line_num + self._prev_logs_end)
 
     @events.on.system_resource_stats_collected
     def track_system_resources(self, stats: Dict[str, Any], context: Dict, **kwargs):
+        if self._state.get('cleanup'):
+            return
         for resource_name, usage in stats.items():
-            self.sequences[resource_name, context].track(usage)
+            self.sequences.typed_sequence(SystemMetric, resource_name, context).track(usage)
 
     @property
     def name(self) -> str:
         return self._attrs_tree['name']
 
     @name.setter
     def name(self, val: str):
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/asp/models/sequences.py` & `aim-4.0.0a9/pkgs/aimstack/asp/models/sequences.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .objects.text import Text
 from .objects.image import Image
 from .objects.audio import Audio
 from .objects.distribution import Distribution
 from .objects.figures import Figure, Figure3D
 
 
-class Metric(Sequence[numbers.Number]):
+class DataframeMixin:
     def dataframe(
             self,
             include_name: bool = False,
             include_context: bool = False,
             include_axis: bool = True,
             only_last: bool = False
     ) -> 'DataFrame':
@@ -67,14 +67,22 @@
                 data[context_key] = [val] * len(indices)
 
         import pandas as pd
         df = pd.DataFrame(data)
         return df
 
 
+class Metric(Sequence[numbers.Number], DataframeMixin):
+    ...
+
+
+class SystemMetric(Sequence[numbers.Number], DataframeMixin):
+    ...
+
+
 class TextSequence(Sequence[Union[Text, List[Text]]]):
     pass
 
 
 class ImageSequence(Sequence[Union[Image, List[Image]]]):
     pass
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/acme.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/acme.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/catboost.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/catboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/fastai.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/fastai.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/hugging_face.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/hugging_face.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras_mixins.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras_mixins.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/keras_tuner.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/keras_tuner.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/lightgbm.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/lightgbm.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/mxnet.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/mxnet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/optuna.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/optuna.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/paddle.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/paddle.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/prophet.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/prophet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,40 +5,40 @@
     from aimstack.asp.models.objects.distribution import Distribution
 
     data_hist = get_model_layers(model, 'data')
 
     for name, params in data_hist.items():
         if 'weight' in params:
             run.get_distribution_sequence(name, {
-                    'type': 'data',
-                    'params': 'weights',
-                }).track(Distribution(params['weight']))
+                'type': 'data',
+                'params': 'weights',
+            }).track(Distribution(params['weight']))
         if 'bias' in params:
             run.get_distribution_sequence(name, {
-                    'type': 'data',
-                    'params': 'biases',
-                }).track(Distribution(params['bias']))
+                'type': 'data',
+                'params': 'biases',
+            }).track(Distribution(params['bias']))
 
 
 def track_gradients_dists(model, run):
     from aimstack.asp.models.objects.distribution import Distribution
 
     grad_hist = get_model_layers(model, 'grad')
 
     for name, params in grad_hist.items():
         if 'weight' in params:
             run.get_distribution_sequence(name, {
-                    'type': 'gradients',
-                    'params': 'weights',
-                }).track(Distribution(params['weight']))
+                'type': 'gradients',
+                'params': 'weights',
+            }).track(Distribution(params['weight']))
         if 'bias' in params:
             run.get_distribution_sequence(name, {
-                    'type': 'gradients',
-                    'params': 'biases',
-                }).track(Distribution(params['bias']))
+                'type': 'gradients',
+                'params': 'biases',
+            }).track(Distribution(params['bias']))
 
 
 def get_model_layers(model, dt, parent_name=None):
     layers = {}
     for name, m in model.named_children():
         layer_name = '{}__{}'.format(parent_name, name) if parent_name else name
         layer_name += '.{}'.format(type(m).__name__)
```

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch_ignite.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch_ignite.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/pytorch_lightning.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/sb3.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/sb3.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/tensorflow.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/tensorflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/adapters/xgboost.py` & `aim-4.0.0a9/pkgs/aimstack/ml/adapters/xgboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/models/deeplake_dataset.py` & `aim-4.0.0a9/pkgs/aimstack/ml/models/deeplake_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/models/dvc_metadata.py` & `aim-4.0.0a9/pkgs/aimstack/ml/models/dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/models/hf_datasets_metadata.py` & `aim-4.0.0a9/pkgs/aimstack/ml/models/hf_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/models/hub_dataset.py` & `aim-4.0.0a9/pkgs/aimstack/ml/models/hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/ml/training_flow.py` & `aim-4.0.0a9/pkgs/aimstack/ml/training_flow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/run.py` & `aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pkgs/aimstack/tensorboard_sync/tracker.py` & `aim-4.0.0a9/pkgs/aimstack/tensorboard_sync/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/pyproject.toml` & `aim-4.0.0a9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 include = ["src/aimcore/web/*", "src/py-sdk/aim/_core/*", "src/py-sdk/aim/_sdk/*"]
 omit = ["src/aimcore/web/migrations/*"]
 
 [tool.flake8]
 max-line-length = 120
 ignore = ["E712", "F405"]
 exclude = [
+    "**/build/*",
     "**/node_modules/",
     "**/migrations/",
     "**/legacy/",
     "**/_legacy_repo",
     "aimcore/web/ui",
     "**/*pb2.py",
     "**/*pb2_grpc.py"
```

### Comparing `aim-4.0.0a7/setup.py` & `aim-4.0.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/callbacks/caller.py` & `aim-4.0.0a9/src/aimcore/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/callbacks/helpers.py` & `aim-4.0.0a9/src/aimcore/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cleanup/__init__.py` & `aim-4.0.0a9/src/aimcore/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/cli.py` & `aim-4.0.0a9/src/aimcore/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/convert/commands.py` & `aim-4.0.0a9/src/aimcore/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/convert/processors/mlflow.py` & `aim-4.0.0a9/src/aimcore/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/convert/processors/tensorboard.py` & `aim-4.0.0a9/src/aimcore/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/convert/processors/wandb.py` & `aim-4.0.0a9/src/aimcore/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/init/commands.py` & `aim-4.0.0a9/src/aimcore/cli/init/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/server/commands.py` & `aim-4.0.0a9/src/aimcore/cli/server/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/storage/commands.py` & `aim-4.0.0a9/src/aimcore/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/up/commands.py` & `aim-4.0.0a9/src/aimcore/cli/up/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/up/utils.py` & `aim-4.0.0a9/src/aimcore/cli/up/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/cli/watcher_cli.py` & `aim-4.0.0a9/src/aimcore/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/reporter/__init__.py` & `aim-4.0.0a9/src/aimcore/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/client.py` & `aim-4.0.0a9/src/aimcore/transport/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import requests
 import base64
 import logging
 import os
 import threading
 import uuid
 import weakref
-from collections import defaultdict
 from copy import deepcopy
 from typing import Tuple
 from websockets.sync.client import connect
 
 from aimcore.transport.message_utils import raise_exception, pack_args, unpack_stream, unpack_args
 from aimcore.transport.rpc_queue import RpcQueueWithRetry
 from aimcore.transport.heartbeat import HeartbeatSender
@@ -223,14 +222,16 @@
         if response == b'OK':
             return
 
         response_json = decode_tree(unpack_args(response))
         raise_exception(response_json)
 
     def start_instructions_batch(self, hash_):
+        if getattr(self._thread_local, 'atomic_instructions', None) is None:
+            self._thread_local.atomic_instructions = {}
         self._thread_local.atomic_instructions[hash_] = []
 
     def flush_instructions_batch(self, hash_):
         if self._thread_local.atomic_instructions.get(hash_) is None:
             return
 
         self.get_queue().register_task(
```

### Comparing `aim-4.0.0a7/src/aimcore/transport/config.py` & `aim-4.0.0a9/src/aimcore/transport/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/handlers.py` & `aim-4.0.0a9/src/aimcore/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/heartbeat.py` & `aim-4.0.0a9/src/aimcore/transport/heartbeat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/message_utils.py` & `aim-4.0.0a9/src/aimcore/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/router.py` & `aim-4.0.0a9/src/aimcore/transport/router.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/rpc_queue.py` & `aim-4.0.0a9/src/aimcore/transport/rpc_queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/server.py` & `aim-4.0.0a9/src/aimcore/transport/server.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/transport/tracking.py` & `aim-4.0.0a9/src/aimcore/transport/tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/__init__.py` & `aim-4.0.0a9/src/aimcore/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/boards/models.py` & `aim-4.0.0a9/src/aimcore/web/api/boards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/boards/views.py` & `aim-4.0.0a9/src/aimcore/web/api/boards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/models.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/pydantic_models.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboard_apps/views.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboard_apps/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboards/models.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboards/pydantic_models.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboards/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboards/serializers.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboards/serializers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/dashboards/views.py` & `aim-4.0.0a9/src/aimcore/web/api/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/db.py` & `aim-4.0.0a9/src/aimcore/web/api/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/projects/project.py` & `aim-4.0.0a9/src/aimcore/web/api/projects/project.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/projects/pydantic_models.py` & `aim-4.0.0a9/src/aimcore/web/api/projects/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/projects/views.py` & `aim-4.0.0a9/src/aimcore/web/api/projects/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import os
 from datetime import timedelta
 from typing import Optional, Tuple
 
 from collections import Counter
 from fastapi import Depends, HTTPException, Query, Header
 from aimcore.web.api.utils import get_project_repo, \
     APIRouter  # wrapper for fastapi.APIRouter
 
-from aimcore.web.configs import AIM_PROJECT_SETTINGS_FILE
 from aimcore.web.api.projects.project import Project
 from aimcore.web.api.projects.pydantic_models import (
     ProjectActivityApiOut,
     ProjectApiOut,
-    ProjectParamsOut,
-    ProjectPinnedSequencesApiIn,
-    ProjectPinnedSequencesApiOut,
     ProjectPackagesApiOut
 )
 from aimcore.web.api.utils import object_factory
-from aim._core.storage.locking import AutoFileLock
 from aim._ext.tracking import analytics
 
 projects_router = APIRouter()
 
 
 @projects_router.get('/', response_model=ProjectApiOut)
 async def project_api():
```

### Comparing `aim-4.0.0a7/src/aimcore/web/api/queries/views.py` & `aim-4.0.0a9/src/aimcore/web/api/queries/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,108 @@
+import random
+
 from fastapi.responses import StreamingResponse
 from fastapi import HTTPException
 
 from typing import Optional, Iterable, Dict, List, Iterator, TYPE_CHECKING
 from aim._sdk.uri_service import URIService
-
+from aim._core.storage.encoding import encode_path, decode_path
 
 from aimcore.web.api.runs.pydantic_models import QuerySyntaxErrorOut
-from aimcore.web.api.utils import checked_query, collect_streamable_data, get_project_repo, \
-      APIRouter  # wrapper for fastapi.APIRouter
+from aimcore.web.api.utils import (
+    checked_query,
+    collect_streamable_data,
+    get_project_repo,
+    APIRouter  # wrapper for fastapi.APIRouter
+)
 
 from aim import Container, Sequence
 
 from aim._core.storage.treeutils import encode_tree
 
 query_router = APIRouter()
 
 if TYPE_CHECKING:
     from aim._sdk.repo import Repo
 
 
-def _process_values(repo: 'Repo', values_list: list) -> list:
+def _process_values(repo: 'Repo', values_list: list, steps_list: list, sequence: Sequence) -> list:
+    # TODO V4: Move blobs uri handling to dump
+    from aim._sdk.uri_service import URIService
+    uri_service = URIService(repo)
+
     processed_values = []
-    for val in values_list:
+    for step, val in zip(steps_list, values_list):
         if isinstance(val, list):
             processed_val = []
-            for nested_val in val:
+            for idx in range(len(val)):
+                nested_val = val[idx]
                 try:
-                    processed_nested_val = nested_val.dump(repo)
+                    processed_nested_val = nested_val.dump()
+                    if not nested_val.RESOLVE_BLOBS:
+                        khash_view = sequence._data.reservoir().container
+                        khash_step = decode_path(khash_view.to_khash(encode_path(step)))
+                        additional_path = (*khash_step, 'val', idx, 'data')
+                        resource_path = uri_service.generate_resource_path(sequence._data.container, additional_path)
+                        processed_nested_val['blobs'] = {'data': uri_service.generate_uri(resource_path)}
                 except AttributeError:
                     processed_nested_val = nested_val
                 processed_val.append(processed_nested_val)
         else:
             try:
-                processed_val = val.dump(repo)
+                processed_val = val.dump()
+                if not val.RESOLVE_BLOBS:
+                    khash_view = sequence._data.reservoir().container
+                    khash_step = decode_path(khash_view.to_khash(encode_path(step)))
+                    additional_path = (*khash_step, 'val', 'data')
+                    resource_path = uri_service.generate_resource_path(sequence._data.container, additional_path)
+                    processed_val['blobs'] = {'data': uri_service.generate_uri(resource_path)}
             except AttributeError:
                 processed_val = val
         processed_values.append(processed_val)
 
     return processed_values
 
 
 def _sequence_data(repo: 'Repo',
                    sequence: Sequence,
                    p: Optional[int],
                    start: Optional[int],
-                   stop: Optional[int]) -> Dict:
+                   stop: Optional[int],
+                   sample_seed: str) -> Dict:
     data = {
         'name': sequence.name,
         'context': sequence.context,
         'container': {
             'hash': sequence._container_hash
         },
         'item_type': sequence.type,
         'axis_names': sequence.axis_names,
-        'axis': {}
+        'range': (sequence.start, sequence.stop),
+        'axis': {},
+        'steps': [],
+        'values': [],
     }
     if p is None and start is None and stop is None:
-        data['steps'] = list(sequence.steps())
-        data['values'] = _process_values(repo, list(sequence.values()))
+        steps_list = list(sequence.steps())
+        data['steps'] = steps_list
+        data['values'] = _process_values(repo, list(sequence.values()), steps_list, sequence)
         for axis_name in sequence.axis_names:
             data['axis'][axis_name] = list(sequence.axis(axis_name))
     else:
-        steps, value_dicts = list(zip(*sequence[start:stop].sample(p)))
-        value_lists = {k: [d[k] for d in value_dicts] for k in value_dicts[0]}
-        data['steps'] = steps
-        data['values'] = _process_values(repo, value_lists.pop('val'))
-        data['axis'] = value_lists
+        random.seed(sample_seed)  # use the query API qparams as sample seed
+        try:
+            steps, value_dicts = list(zip(*sequence[start:stop].sample(p)))
+            value_lists = {k: [d[k] for d in value_dicts] for k in value_dicts[0]}
+            data['steps'] = steps
+            data['values'] = _process_values(repo, value_lists.pop('val'), steps, sequence)
+            data['axis'] = value_lists
+        except Exception:
+            pass
+
     return data
 
 
 def _container_data(container: Container) -> Dict:
     data = {
         'hash': container.hash,
         'params': container[...]
@@ -77,17 +110,18 @@
     return data
 
 
 async def sequence_search_result_streamer(repo: 'Repo',
                                           query_collection,
                                           p: Optional[int],
                                           start: Optional[int],
-                                          stop: Optional[int]):
+                                          stop: Optional[int],
+                                          sample_seed: str):
     for sequence in query_collection:
-        seq_data = {hash(sequence): _sequence_data(repo, sequence, p, start, stop)}
+        seq_data = {hash(sequence): _sequence_data(repo, sequence, p, start, stop, sample_seed)}
         encoded_tree = encode_tree(seq_data)
         yield collect_streamable_data(encoded_tree)
 
 
 async def container_search_result_streamer(query_collection: Iterable[Container]):
     for container in query_collection:
         cont_data = {container.hash: _container_data(container)}
@@ -95,19 +129,20 @@
         yield collect_streamable_data(encoded_tree)
 
 
 def sequence_query_grouped_response(repo: 'Repo',
                                     query_collection,
                                     p: Optional[int],
                                     start: Optional[int],
-                                    stop: Optional[int]):
+                                    stop: Optional[int],
+                                    sample_seed: str):
     #  TODO: V4 use repo query methods and grouping instead
     containers_data = {}
     for sequence in query_collection:
-        seq_data = _sequence_data(repo, sequence, p, start, stop)
+        seq_data = _sequence_data(repo, sequence, p, start, stop, sample_seed)
 
         cont_hash = sequence._container_hash
         if cont_hash not in containers_data:
             container = repo.get_container(cont_hash)
             cont_data = _container_data(container)
             cont_data['sequences'] = []
             containers_data[cont_hash] = cont_data
@@ -131,15 +166,16 @@
     repo = get_project_repo()
     query = checked_query(q)
     if type_ in Container.registry:
         qresult = repo.containers(query, type_)
         streamer = container_search_result_streamer(qresult)
     elif type_ in Sequence.registry:
         qresult = repo.sequences(query, type_)
-        streamer = sequence_search_result_streamer(repo, qresult, p, start, stop)
+        sample_seed = f'{query}_{p}_{start}_{stop}'
+        streamer = sequence_search_result_streamer(repo, qresult, p, start, stop, sample_seed)
     else:
         raise HTTPException(status_code=400, detail=f'Unknown type \'{type_}\'.')
     return StreamingResponse(streamer)
 
 
 @query_router.get('/grouped-sequences/')
 async def grouped_data_fetch_api(seq_type: Optional[str] = 'Sequence',
@@ -155,15 +191,16 @@
     if cont_type not in Container.registry:
         raise HTTPException(status_code=400, detail=f'\'{cont_type}\' is not a valid Container type.')
     if query:
         query = f'(container.type.startswith("{Container.registry[cont_type][0].get_full_typename()}")) and {query}'
     else:
         query = f'container.type.startswith("{Container.registry[cont_type][0].get_full_typename()}")'
     qresult = repo.sequences(query, seq_type)
-    return sequence_query_grouped_response(repo, qresult, p, start, stop)
+    sample_seed = f'{query}_{p}_{start}_{stop}'
+    return sequence_query_grouped_response(repo, qresult, p, start, stop, sample_seed)
 
 
 URIBatchIn = List[str]
 
 
 def fetch_blobs_batch(repo: 'Repo', uri_batch: List[str]) -> Iterator[bytes]:
     uri_service = URIService(repo=repo)
```

### Comparing `aim-4.0.0a7/src/aimcore/web/api/runs/pydantic_models.py` & `aim-4.0.0a9/src/aimcore/web/api/runs/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/runs/utils.py` & `aim-4.0.0a9/src/aimcore/web/api/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/runs/views.py` & `aim-4.0.0a9/src/aimcore/web/api/runs/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/utils.py` & `aim-4.0.0a9/src/aimcore/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/api/views.py` & `aim-4.0.0a9/src/aimcore/web/api/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/middlewares/profiler.py` & `aim-4.0.0a9/src/aimcore/web/middlewares/profiler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/alembic.ini` & `aim-4.0.0a9/src/aimcore/web/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/alembic_dev.ini` & `aim-4.0.0a9/src/aimcore/web/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/env.py` & `aim-4.0.0a9/src/aimcore/web/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/versions/11672b13f92c_.py` & `aim-4.0.0a9/src/aimcore/web/migrations/versions/11672b13f92c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/versions/517a45b2e62c_.py` & `aim-4.0.0a9/src/aimcore/web/migrations/versions/517a45b2e62c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/versions/5ae8371b7481_.py` & `aim-4.0.0a9/src/aimcore/web/migrations/versions/5ae8371b7481_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/versions/73a3d004c227_.py` & `aim-4.0.0a9/src/aimcore/web/migrations/versions/73a3d004c227_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py` & `aim-4.0.0a9/src/aimcore/web/migrations/versions/da08eab59790_board_and_board_templates.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/aimcore/web/utils.py` & `aim-4.0.0a9/src/aimcore/web/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/__about__.py` & `aim-4.0.0a9/src/py-sdk/aim/__about__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/__init__.py` & `aim-4.0.0a9/src/py-sdk/aim/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/arrayview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.arrayview",
         "sources": [
             "src/py-sdk/aim/_core/storage/arrayview.py"
         ]
     },
     "module_name": "aim._core.storage.arrayview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/arrayview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.container",
         "sources": [
             "src/py-sdk/aim/_core/storage/container.py"
         ]
     },
     "module_name": "aim._core.storage.container"
@@ -2513,15 +2513,15 @@
 struct __pyx_obj_3aim_5_core_7storage_9container_Container {
   PyObject_HEAD
   struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *__pyx_vtab;
   PyObject *__weakref__;
 };
 
 
-/* "aim/_core/storage/container.py":146
+/* "aim/_core/storage/container.py":150
  *         raise NotImplementedError
  * 
  *     def samples(             # <<<<<<<<<<<<<<
  *         self,
  *         begin: ContainerKey = b'',
  */
 struct __pyx_obj_3aim_5_core_7storage_9container___pyx_scope_struct__samples {
@@ -3025,15 +3025,15 @@
 
 struct __pyx_vtabstruct_3aim_5_core_7storage_5utils_BLOB {
   PyObject *(*load)(struct __pyx_obj_3aim_5_core_7storage_5utils_BLOB *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_3aim_5_core_7storage_5utils_BLOB *__pyx_vtabptr_3aim_5_core_7storage_5utils_BLOB;
 
 
-/* "aim/_core/storage/container.py":322
+/* "aim/_core/storage/container.py":326
  * 
  * 
  * class ContainerItemsIterator(interfaces.Iterator):             # <<<<<<<<<<<<<<
  *     pass
  */
 
 struct __pyx_vtabstruct_3aim_5_core_7storage_9container_ContainerItemsIterator {
@@ -7229,17 +7229,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "aim/_core/storage/container.py":116
  *         ...
  * 
- *     def items(self, begin: ContainerKey = b'', end: ContainerKey = b'') -> Iterator[Tuple[ContainerKey, ContainerValue]]:             # <<<<<<<<<<<<<<
- *         """Iterate over all the key-value records in the prefix key range.
- * 
+ *     def items(             # <<<<<<<<<<<<<<
+ *         self,
+ *         begin: ContainerKey = b'',
  */
 
 static PyObject *__pyx_pw_3aim_5_core_7storage_9container_9Container_25items(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
@@ -7321,30 +7321,30 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":144
+  /* "aim/_core/storage/container.py":148
  *                 after `end` in lexicographic order, excluding `end`.
  *         """
  *         raise NotImplementedError             # <<<<<<<<<<<<<<
  * 
  *     def samples(
  */
   __Pyx_Raise(__pyx_builtin_NotImplementedError, 0, 0, 0);
-  __PYX_ERR(0, 144, __pyx_L1_error)
+  __PYX_ERR(0, 148, __pyx_L1_error)
 
   /* "aim/_core/storage/container.py":116
  *         ...
  * 
- *     def items(self, begin: ContainerKey = b'', end: ContainerKey = b'') -> Iterator[Tuple[ContainerKey, ContainerValue]]:             # <<<<<<<<<<<<<<
- *         """Iterate over all the key-value records in the prefix key range.
- * 
+ *     def items(             # <<<<<<<<<<<<<<
+ *         self,
+ *         begin: ContainerKey = b'',
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -7442,16 +7442,16 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("items", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.items", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_begin), (&PyBytes_Type), 1, "begin", 1))) __PYX_ERR(0, 116, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), (&PyBytes_Type), 1, "end", 1))) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_begin), (&PyBytes_Type), 1, "begin", 1))) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_end), (&PyBytes_Type), 1, "end", 1))) __PYX_ERR(0, 119, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_24items(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_begin, __pyx_v_end);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7486,15 +7486,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_3aim_5_core_7storage_9container_9Container_28generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "aim/_core/storage/container.py":146
+/* "aim/_core/storage/container.py":150
  *         raise NotImplementedError
  * 
  *     def samples(             # <<<<<<<<<<<<<<
  *         self,
  *         begin: ContainerKey = b'',
  */
 
@@ -7548,27 +7548,27 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_begin);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_end);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "samples") < 0)) __PYX_ERR(0, 146, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "samples") < 0)) __PYX_ERR(0, 150, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
@@ -7577,15 +7577,15 @@
       }
     }
     __pyx_v_begin = values[0];
     __pyx_v_end = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("samples", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 146, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("samples", 0, 0, 2, __pyx_nargs); __PYX_ERR(0, 150, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.samples", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_26samples(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_begin, __pyx_v_end);
 
@@ -7602,29 +7602,29 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("samples", 0);
   __pyx_cur_scope = (struct __pyx_obj_3aim_5_core_7storage_9container___pyx_scope_struct__samples *)__pyx_tp_new_3aim_5_core_7storage_9container___pyx_scope_struct__samples(__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_3aim_5_core_7storage_9container___pyx_scope_struct__samples *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 146, __pyx_L1_error)
+    __PYX_ERR(0, 150, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_begin = __pyx_v_begin;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_begin);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_begin);
   __pyx_cur_scope->__pyx_v_end = __pyx_v_end;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_end);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_end);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3aim_5_core_7storage_9container_9Container_28generator, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_samples, __pyx_n_s_Container_samples, __pyx_n_s_aim__core_storage_container); if (unlikely(!gen)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_3aim_5_core_7storage_9container_9Container_28generator, __pyx_codeobj__2, (PyObject *) __pyx_cur_scope, __pyx_n_s_samples, __pyx_n_s_Container_samples, __pyx_n_s_aim__core_storage_container); if (unlikely(!gen)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7652,38 +7652,38 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L4_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 150, __pyx_L1_error)
 
-  /* "aim/_core/storage/container.py":166
+  /* "aim/_core/storage/container.py":170
  *                 after `end` in lexicographic order, excluding `end`.
  *         """
  *         all_samples = list(self.items(begin, end))             # <<<<<<<<<<<<<<
  *         yield all_samples
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_cur_scope->__pyx_v_begin))||((__pyx_cur_scope->__pyx_v_begin) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_cur_scope->__pyx_v_begin))) __PYX_ERR(0, 166, __pyx_L1_error)
-  if (!(likely(PyBytes_CheckExact(__pyx_cur_scope->__pyx_v_end))||((__pyx_cur_scope->__pyx_v_end) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_cur_scope->__pyx_v_end))) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_cur_scope->__pyx_v_begin))||((__pyx_cur_scope->__pyx_v_begin) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_cur_scope->__pyx_v_begin))) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_cur_scope->__pyx_v_end))||((__pyx_cur_scope->__pyx_v_end) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_cur_scope->__pyx_v_end))) __PYX_ERR(0, 170, __pyx_L1_error)
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.begin = ((PyObject*)__pyx_cur_scope->__pyx_v_begin);
   __pyx_t_2.end = ((PyObject*)__pyx_cur_scope->__pyx_v_end);
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->items(__pyx_cur_scope->__pyx_v_self, 0, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->items(__pyx_cur_scope->__pyx_v_self, 0, &__pyx_t_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_3 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_cur_scope->__pyx_v_all_samples = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "aim/_core/storage/container.py":167
+  /* "aim/_core/storage/container.py":171
  *         """
  *         all_samples = list(self.items(begin, end))
  *         yield all_samples             # <<<<<<<<<<<<<<
  * 
  *     def keys(self, prefix: ContainerKey = b'') -> Iterator[ContainerKey]:
  */
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_all_samples);
@@ -7691,18 +7691,18 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   /* return from generator, yielding value */
   __pyx_generator->resume_label = 1;
   return __pyx_r;
   __pyx_L4_resume_from_yield:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 167, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 171, __pyx_L1_error)
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "aim/_core/storage/container.py":146
+  /* "aim/_core/storage/container.py":150
  *         raise NotImplementedError
  * 
  *     def samples(             # <<<<<<<<<<<<<<
  *         self,
  *         begin: ContainerKey = b'',
  */
 
@@ -7721,15 +7721,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":169
+/* "aim/_core/storage/container.py":173
  *         yield all_samples
  * 
  *     def keys(self, prefix: ContainerKey = b'') -> Iterator[ContainerKey]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the keys in the prefix range.
  * 
  */
 
@@ -7779,34 +7779,34 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prefix);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "keys") < 0)) __PYX_ERR(0, 169, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "keys") < 0)) __PYX_ERR(0, 173, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_prefix = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("keys", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 169, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("keys", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 173, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_29keys(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_prefix);
 
@@ -7825,31 +7825,31 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("keys", 0);
 
-  /* "aim/_core/storage/container.py":187
+  /* "aim/_core/storage/container.py":191
  *             prefix (:obj:`bytes`): the prefix that defines the key range
  *         """
  *         return utils.KeysIterator(self.items(prefix))             # <<<<<<<<<<<<<<
  * 
  *     def values(self, prefix: ContainerKey = b'') -> Iterator[ContainerValue]:
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utils); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utils); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_KeysIterator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_KeysIterator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_v_prefix))||((__pyx_v_prefix) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_prefix))) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_prefix))||((__pyx_v_prefix) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_prefix))) __PYX_ERR(0, 191, __pyx_L1_error)
   __pyx_t_4.__pyx_n = 1;
   __pyx_t_4.begin = ((PyObject*)__pyx_v_prefix);
-  __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->items(__pyx_v_self, 0, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->items(__pyx_v_self, 0, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7860,23 +7860,23 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":169
+  /* "aim/_core/storage/container.py":173
  *         yield all_samples
  * 
  *     def keys(self, prefix: ContainerKey = b'') -> Iterator[ContainerKey]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the keys in the prefix range.
  * 
  */
 
@@ -7890,15 +7890,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":189
+/* "aim/_core/storage/container.py":193
  *         return utils.KeysIterator(self.items(prefix))
  * 
  *     def values(self, prefix: ContainerKey = b'') -> Iterator[ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the values in the given prefix key range.
  * 
  */
 
@@ -7948,34 +7948,34 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prefix);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "values") < 0)) __PYX_ERR(0, 189, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "values") < 0)) __PYX_ERR(0, 193, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_prefix = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("values", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 189, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("values", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 193, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.values", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_31values(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_prefix);
 
@@ -7994,31 +7994,31 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("values", 0);
 
-  /* "aim/_core/storage/container.py":207
+  /* "aim/_core/storage/container.py":211
  *             prefix (:obj:`bytes`): the prefix that defines the key range
  *         """
  *         return utils.ValuesIterator(self.items(prefix))             # <<<<<<<<<<<<<<
  * 
  *     def view(self, prefix: ContainerKey = b'') -> 'Container':
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utils); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_utils); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ValuesIterator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ValuesIterator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_v_prefix))||((__pyx_v_prefix) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_prefix))) __PYX_ERR(0, 207, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_prefix))||((__pyx_v_prefix) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_prefix))) __PYX_ERR(0, 211, __pyx_L1_error)
   __pyx_t_4.__pyx_n = 1;
   __pyx_t_4.begin = ((PyObject*)__pyx_v_prefix);
-  __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->items(__pyx_v_self, 0, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->items(__pyx_v_self, 0, &__pyx_t_4)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -8029,23 +8029,23 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":189
+  /* "aim/_core/storage/container.py":193
  *         return utils.KeysIterator(self.items(prefix))
  * 
  *     def values(self, prefix: ContainerKey = b'') -> Iterator[ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the values in the given prefix key range.
  * 
  */
 
@@ -8059,15 +8059,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":209
+/* "aim/_core/storage/container.py":213
  *         return utils.ValuesIterator(self.items(prefix))
  * 
  *     def view(self, prefix: ContainerKey = b'') -> 'Container':             # <<<<<<<<<<<<<<
  *         """Return a view (even mutable ones) that enable access to the container
  *         but with modifications.
  */
 
@@ -8117,34 +8117,34 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prefix);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 213, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "view") < 0)) __PYX_ERR(0, 209, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "view") < 0)) __PYX_ERR(0, 213, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_prefix = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("view", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 209, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("view", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 213, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.view", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_33view(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_prefix);
 
@@ -8161,15 +8161,15 @@
   /* function exit code */
   __pyx_r = ((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)Py_None); __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":234
+/* "aim/_core/storage/container.py":238
  *         ...
  * 
  *     def tree(self) -> 'TreeView':             # <<<<<<<<<<<<<<
  *         """Return a :obj:`TreeView` which enables hierarchical view and access
  *         to the container records.
  */
 
@@ -8215,15 +8215,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":253
+/* "aim/_core/storage/container.py":257
  *         ...
  * 
  *     def walk(self, prefix: ContainerKey = b''):             # <<<<<<<<<<<<<<
  *         """A bi-directional generator to walk over the collection of records on
  *         any arbitrary order. The `prefix` sent to the generator (lets call it
  */
 
@@ -8273,34 +8273,34 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_prefix);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 257, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "walk") < 0)) __PYX_ERR(0, 253, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "walk") < 0)) __PYX_ERR(0, 257, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_prefix = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("walk", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 253, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("walk", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 257, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.walk", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_37walk(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_prefix);
 
@@ -8317,15 +8317,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":269
+/* "aim/_core/storage/container.py":273
  *         ...
  * 
  *     def next_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right after the
  *         provided `key`.
  */
 
@@ -8362,15 +8362,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_40next_key)) {
@@ -8388,19 +8388,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 269, __pyx_L1_error)
+        if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 273, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8411,67 +8411,67 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":273
+  /* "aim/_core/storage/container.py":277
  *         provided `key`.
  *         """
  *         key, _ = self.next_item(key)             # <<<<<<<<<<<<<<
  *         return key
  * 
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.key = __pyx_v_key;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(__pyx_t_1 != Py_None)) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 273, __pyx_L1_error)
+      __PYX_ERR(0, 277, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 277, __pyx_L1_error)
   }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 273, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_2));
   __pyx_t_2 = 0;
   __pyx_v__ = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "aim/_core/storage/container.py":274
+  /* "aim/_core/storage/container.py":278
  *         """
  *         key, _ = self.next_item(key)
  *         return key             # <<<<<<<<<<<<<<
  * 
  *     def next_value(self, key: ContainerKey = b'') -> ContainerValue:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_key);
   __pyx_r = __pyx_v_key;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":269
+  /* "aim/_core/storage/container.py":273
  *         ...
  * 
  *     def next_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right after the
  *         provided `key`.
  */
 
@@ -8537,40 +8537,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 269, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 273, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_key") < 0)) __PYX_ERR(0, 269, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_key") < 0)) __PYX_ERR(0, 273, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("next_key", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 269, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("next_key", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 273, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.next_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 273, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_39next_key(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8586,15 +8586,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_key", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_key(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_key(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8603,15 +8603,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":276
+/* "aim/_core/storage/container.py":280
  *         return key
  * 
  *     def next_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         after the provided `key`.
  */
 
@@ -8648,15 +8648,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_42next_value)) {
@@ -8674,15 +8674,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -8696,66 +8696,66 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":280
+  /* "aim/_core/storage/container.py":284
  *         after the provided `key`.
  *         """
  *         _, value = self.next_item(key)             # <<<<<<<<<<<<<<
  *         return value
  * 
  */
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.key = __pyx_v_key;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(__pyx_t_1 != Py_None)) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 280, __pyx_L1_error)
+      __PYX_ERR(0, 284, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 280, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 284, __pyx_L1_error)
   }
   __pyx_v__ = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_value = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "aim/_core/storage/container.py":281
+  /* "aim/_core/storage/container.py":285
  *         """
  *         _, value = self.next_item(key)
  *         return value             # <<<<<<<<<<<<<<
  * 
  *     def next_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_value);
   __pyx_r = __pyx_v_value;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":276
+  /* "aim/_core/storage/container.py":280
  *         return key
  * 
  *     def next_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         after the provided `key`.
  */
 
@@ -8821,40 +8821,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 280, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_value") < 0)) __PYX_ERR(0, 276, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_value") < 0)) __PYX_ERR(0, 280, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("next_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 276, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("next_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 280, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.next_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 280, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_41next_value(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -8870,15 +8870,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_value", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8887,15 +8887,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":283
+/* "aim/_core/storage/container.py":287
  *         return value
  * 
  *     def next_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
 
@@ -8930,15 +8930,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_key_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_key_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_44next_key_value)) {
@@ -8956,19 +8956,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 283, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 287, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8979,31 +8979,31 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":287
+  /* "aim/_core/storage/container.py":291
  *         right after the provided `key`.
  *         """
  *         return self.next_item(key)             # <<<<<<<<<<<<<<
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.key = __pyx_v_key;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->next_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":283
+  /* "aim/_core/storage/container.py":287
  *         return value
  * 
  *     def next_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
 
@@ -9067,40 +9067,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_key_value") < 0)) __PYX_ERR(0, 283, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_key_value") < 0)) __PYX_ERR(0, 287, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("next_key_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 283, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("next_key_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 287, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.next_key_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 287, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_43next_key_value(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9116,15 +9116,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_key_value", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_key_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_key_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9133,15 +9133,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":289
+/* "aim/_core/storage/container.py":293
  *         return self.next_item(key)
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
 
@@ -9175,15 +9175,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_item); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_next_item); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_46next_item)) {
@@ -9201,19 +9201,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 289, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 293, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -9224,15 +9224,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":290
+  /* "aim/_core/storage/container.py":294
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  *         """Returns `(key, value)` for the key that comes (lexicographically)             # <<<<<<<<<<<<<<
  *         right after the provided `key`.
  *         """
  */
 
@@ -9248,15 +9248,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":289
+/* "aim/_core/storage/container.py":293
  *         return self.next_item(key)
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
 
@@ -9306,40 +9306,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 289, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 293, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_item") < 0)) __PYX_ERR(0, 289, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "next_item") < 0)) __PYX_ERR(0, 293, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("next_item", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 289, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("next_item", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 293, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.next_item", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 293, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_45next_item(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9355,15 +9355,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_item", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_item(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->next_item(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9372,15 +9372,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":295
+/* "aim/_core/storage/container.py":299
  *         ...
  * 
  *     def prev_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right before the
  *         provided `key`.
  */
 
@@ -9416,15 +9416,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_48prev_key)) {
@@ -9442,19 +9442,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 295, __pyx_L1_error)
+        if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 299, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -9465,65 +9465,65 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":299
+  /* "aim/_core/storage/container.py":303
  *         provided `key`.
  *         """
  *         key, _ = self.prev_item()             # <<<<<<<<<<<<<<
  *         return key
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(__pyx_t_1 != Py_None)) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 299, __pyx_L1_error)
+      __PYX_ERR(0, 303, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 299, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 303, __pyx_L1_error)
   }
-  if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 299, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_2))) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_2));
   __pyx_t_2 = 0;
   __pyx_v__ = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "aim/_core/storage/container.py":300
+  /* "aim/_core/storage/container.py":304
  *         """
  *         key, _ = self.prev_item()
  *         return key             # <<<<<<<<<<<<<<
  * 
  *     def prev_value(self, key: ContainerKey = b'') -> ContainerValue:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_key);
   __pyx_r = __pyx_v_key;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":295
+  /* "aim/_core/storage/container.py":299
  *         ...
  * 
  *     def prev_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right before the
  *         provided `key`.
  */
 
@@ -9589,40 +9589,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 295, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 299, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_key") < 0)) __PYX_ERR(0, 295, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_key") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("prev_key", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 295, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("prev_key", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 299, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.prev_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 295, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 299, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_47prev_key(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9638,15 +9638,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prev_key", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_key(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_key(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9655,15 +9655,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":302
+/* "aim/_core/storage/container.py":306
  *         return key
  * 
  *     def prev_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         before the provided `key`.
  */
 
@@ -9699,15 +9699,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_50prev_value)) {
@@ -9725,15 +9725,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
@@ -9747,64 +9747,64 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":306
+  /* "aim/_core/storage/container.py":310
  *         before the provided `key`.
  *         """
  *         _, value = self.prev_item()             # <<<<<<<<<<<<<<
  *         return value
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(__pyx_t_1 != Py_None)) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 306, __pyx_L1_error)
+      __PYX_ERR(0, 310, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 306, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 310, __pyx_L1_error)
   }
   __pyx_v__ = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_value = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "aim/_core/storage/container.py":307
+  /* "aim/_core/storage/container.py":311
  *         """
  *         _, value = self.prev_item()
  *         return value             # <<<<<<<<<<<<<<
  * 
  *     def prev_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_value);
   __pyx_r = __pyx_v_value;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":302
+  /* "aim/_core/storage/container.py":306
  *         return key
  * 
  *     def prev_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         before the provided `key`.
  */
 
@@ -9870,40 +9870,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 302, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 306, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_value") < 0)) __PYX_ERR(0, 302, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_value") < 0)) __PYX_ERR(0, 306, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("prev_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 302, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("prev_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 306, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.prev_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 306, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_49prev_value(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9919,15 +9919,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prev_value", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9936,15 +9936,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":309
+/* "aim/_core/storage/container.py":313
  *         return value
  * 
  *     def prev_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
 
@@ -9979,15 +9979,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_key_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_key_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_52prev_key_value)) {
@@ -10005,19 +10005,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 309, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 313, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -10028,31 +10028,31 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":313
+  /* "aim/_core/storage/container.py":317
  *         right before the provided `key`.
  *         """
  *         return self.prev_item(key)             # <<<<<<<<<<<<<<
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_6.__pyx_n = 1;
   __pyx_t_6.key = __pyx_v_key;
-  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_3aim_5_core_7storage_9container_Container *)__pyx_v_self->__pyx_vtab)->prev_item(__pyx_v_self, 0, &__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "aim/_core/storage/container.py":309
+  /* "aim/_core/storage/container.py":313
  *         return value
  * 
  *     def prev_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
 
@@ -10116,40 +10116,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 309, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_key_value") < 0)) __PYX_ERR(0, 309, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_key_value") < 0)) __PYX_ERR(0, 313, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("prev_key_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 309, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("prev_key_value", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 313, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.prev_key_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 309, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 313, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_51prev_key_value(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -10165,15 +10165,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prev_key_value", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_key_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_key_value(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10182,15 +10182,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":315
+/* "aim/_core/storage/container.py":319
  *         return self.prev_item(key)
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
 
@@ -10224,15 +10224,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_item); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_prev_item); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_3aim_5_core_7storage_9container_9Container_54prev_item)) {
@@ -10250,19 +10250,19 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_key};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
-        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 315, __pyx_L1_error)
+        if (!(likely(PyTuple_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_2))) __PYX_ERR(0, 319, __pyx_L1_error)
         __pyx_r = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -10273,15 +10273,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "aim/_core/storage/container.py":316
+  /* "aim/_core/storage/container.py":320
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:
  *         """Returns `(key, value)` for the key that comes (lexicographically)             # <<<<<<<<<<<<<<
  *         right before the provided `key`.
  *         """
  */
 
@@ -10297,15 +10297,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "aim/_core/storage/container.py":315
+/* "aim/_core/storage/container.py":319
  *         return self.prev_item(key)
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
 
@@ -10355,40 +10355,40 @@
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key);
           if (value) { values[0] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_item") < 0)) __PYX_ERR(0, 315, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "prev_item") < 0)) __PYX_ERR(0, 319, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_key = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("prev_item", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 315, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("prev_item", 0, 0, 1, __pyx_nargs); __PYX_ERR(0, 319, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("aim._core.storage.container.Container.prev_item", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 315, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key), (&PyBytes_Type), 1, "key", 1))) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_r = __pyx_pf_3aim_5_core_7storage_9container_9Container_53prev_item(((struct __pyx_obj_3aim_5_core_7storage_9container_Container *)__pyx_v_self), __pyx_v_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -10404,15 +10404,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("prev_item", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.key = __pyx_v_key;
-  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_item(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_3aim_5_core_7storage_9container_Container->prev_item(__pyx_v_self, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13007,15 +13007,15 @@
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {&__pyx_n_s_walk, __pyx_k_walk, sizeof(__pyx_k_walk), 0, 0, 1, 1},
   #endif
   {0, 0, 0, 0, 0, 0, 0}
 };
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 148, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -13140,188 +13140,188 @@
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
   __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_commit, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 108, __pyx_L1_error)
 
   /* "aim/_core/storage/container.py":116
  *         ...
  * 
- *     def items(self, begin: ContainerKey = b'', end: ContainerKey = b'') -> Iterator[Tuple[ContainerKey, ContainerValue]]:             # <<<<<<<<<<<<<<
- *         """Iterate over all the key-value records in the prefix key range.
- * 
+ *     def items(             # <<<<<<<<<<<<<<
+ *         self,
+ *         begin: ContainerKey = b'',
  */
   __pyx_tuple__23 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_begin, __pyx_n_s_end); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_items, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 116, __pyx_L1_error)
   __pyx_tuple__25 = PyTuple_Pack(2, __pyx_kp_b_, __pyx_kp_b_); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "aim/_core/storage/container.py":146
+  /* "aim/_core/storage/container.py":150
  *         raise NotImplementedError
  * 
  *     def samples(             # <<<<<<<<<<<<<<
  *         self,
  *         begin: ContainerKey = b'',
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_begin, __pyx_n_s_end, __pyx_n_s_all_samples); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_begin, __pyx_n_s_end, __pyx_n_s_all_samples); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_samples, 146, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_kp_b_, __pyx_kp_b_); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_GENERATOR, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_samples, 150, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_kp_b_, __pyx_kp_b_); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "aim/_core/storage/container.py":169
+  /* "aim/_core/storage/container.py":173
  *         yield all_samples
  * 
  *     def keys(self, prefix: ContainerKey = b'') -> Iterator[ContainerKey]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the keys in the prefix range.
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_prefix); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_prefix); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_keys, 169, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 169, __pyx_L1_error)
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_keys, 173, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
 
-  /* "aim/_core/storage/container.py":189
+  /* "aim/_core/storage/container.py":193
  *         return utils.KeysIterator(self.items(prefix))
  * 
  *     def values(self, prefix: ContainerKey = b'') -> Iterator[ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the values in the given prefix key range.
  * 
  */
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_values, 189, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_values, 193, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 193, __pyx_L1_error)
 
-  /* "aim/_core/storage/container.py":209
+  /* "aim/_core/storage/container.py":213
  *         return utils.ValuesIterator(self.items(prefix))
  * 
  *     def view(self, prefix: ContainerKey = b'') -> 'Container':             # <<<<<<<<<<<<<<
  *         """Return a view (even mutable ones) that enable access to the container
  *         but with modifications.
  */
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_view, 209, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_view, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 213, __pyx_L1_error)
 
-  /* "aim/_core/storage/container.py":234
+  /* "aim/_core/storage/container.py":238
  *         ...
  * 
  *     def tree(self) -> 'TreeView':             # <<<<<<<<<<<<<<
  *         """Return a :obj:`TreeView` which enables hierarchical view and access
  *         to the container records.
  */
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_tree, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_tree, 238, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 238, __pyx_L1_error)
 
-  /* "aim/_core/storage/container.py":253
+  /* "aim/_core/storage/container.py":257
  *         ...
  * 
  *     def walk(self, prefix: ContainerKey = b''):             # <<<<<<<<<<<<<<
  *         """A bi-directional generator to walk over the collection of records on
  *         any arbitrary order. The `prefix` sent to the generator (lets call it
  */
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_walk, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_walk, 257, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 257, __pyx_L1_error)
 
-  /* "aim/_core/storage/container.py":269
+  /* "aim/_core/storage/container.py":273
  *         ...
  * 
  *     def next_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right after the
  *         provided `key`.
  */
-  __pyx_tuple__35 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_key); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_key); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_key, 269, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 269, __pyx_L1_error)
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_key, 273, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
 
-  /* "aim/_core/storage/container.py":276
+  /* "aim/_core/storage/container.py":280
  *         return key
  * 
  *     def next_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         after the provided `key`.
  */
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_value, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 276, __pyx_L1_error)
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_value, 280, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
 
-  /* "aim/_core/storage/container.py":283
+  /* "aim/_core/storage/container.py":287
  *         return value
  * 
  *     def next_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_key_value, 283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 283, __pyx_L1_error)
-  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_key_value, 287, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
 
-  /* "aim/_core/storage/container.py":289
+  /* "aim/_core/storage/container.py":293
  *         return self.next_item(key)
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_item, 289, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 289, __pyx_L1_error)
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_next_item, 293, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
 
-  /* "aim/_core/storage/container.py":295
+  /* "aim/_core/storage/container.py":299
  *         ...
  * 
  *     def prev_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right before the
  *         provided `key`.
  */
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_key, 295, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 295, __pyx_L1_error)
-  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_key, 299, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
 
-  /* "aim/_core/storage/container.py":302
+  /* "aim/_core/storage/container.py":306
  *         return key
  * 
  *     def prev_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         before the provided `key`.
  */
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_value, 302, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 302, __pyx_L1_error)
-  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_value, 306, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
 
-  /* "aim/_core/storage/container.py":309
+  /* "aim/_core/storage/container.py":313
  *         return value
  * 
  *     def prev_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_key_value, 309, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 309, __pyx_L1_error)
-  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_key_value, 313, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
 
-  /* "aim/_core/storage/container.py":315
+  /* "aim/_core/storage/container.py":319
  *         return self.prev_item(key)
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_item, 315, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 315, __pyx_L1_error)
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_py_sdk_aim__core_storage_con, __pyx_n_s_prev_item, 319, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_kp_b_); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
@@ -13579,45 +13579,45 @@
   __pyx_ptype_8aimrocks_11lib_rocksdb_Iterator = __Pyx_ImportType(__pyx_t_1, "aimrocks.lib_rocksdb", "Iterator", sizeof(struct __pyx_obj_8aimrocks_11lib_rocksdb_Iterator), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_8aimrocks_11lib_rocksdb_Iterator),
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_8aimrocks_11lib_rocksdb_Iterator) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_8aimrocks_11lib_rocksdb_Iterator = (struct __pyx_vtabstruct_8aimrocks_11lib_rocksdb_Iterator*)__Pyx_GetVtable(__pyx_ptype_8aimrocks_11lib_rocksdb_Iterator); if (unlikely(!__pyx_vtabptr_8aimrocks_11lib_rocksdb_Iterator)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_3aim_5_core_7storage_9container_ContainerItemsIterator = &__pyx_vtable_3aim_5_core_7storage_9container_ContainerItemsIterator;
   __pyx_vtable_3aim_5_core_7storage_9container_ContainerItemsIterator.__pyx_base = *__pyx_vtabptr_8aimrocks_11lib_rocksdb_Iterator;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_2 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8aimrocks_11lib_rocksdb_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8aimrocks_11lib_rocksdb_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3aim_5_core_7storage_9container_ContainerItemsIterator_spec, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator)) __PYX_ERR(0, 322, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3aim_5_core_7storage_9container_ContainerItemsIterator_spec, __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator)) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3aim_5_core_7storage_9container_ContainerItemsIterator_spec, __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #else
   __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator = &__pyx_type_3aim_5_core_7storage_9container_ContainerItemsIterator;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_dealloc = __pyx_ptype_8aimrocks_11lib_rocksdb_Iterator->tp_dealloc;
   __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_base = __pyx_ptype_8aimrocks_11lib_rocksdb_Iterator;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_dictoffset && __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator, __pyx_vtabptr_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator, __pyx_vtabptr_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ContainerItemsIterator, (PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ContainerItemsIterator, (PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_ContainerItemsIterator) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   #endif
   __pyx_vtabptr_3aim_5_core_7storage_9container_Container = &__pyx_vtable_3aim_5_core_7storage_9container_Container;
   __pyx_vtable_3aim_5_core_7storage_9container_Container.close = (void (*)(struct __pyx_obj_3aim_5_core_7storage_9container_Container *, int __pyx_skip_dispatch))__pyx_f_3aim_5_core_7storage_9container_9Container_close;
   __pyx_vtable_3aim_5_core_7storage_9container_Container.preload = (void (*)(struct __pyx_obj_3aim_5_core_7storage_9container_Container *, int __pyx_skip_dispatch))__pyx_f_3aim_5_core_7storage_9container_9Container_preload;
   __pyx_vtable_3aim_5_core_7storage_9container_Container.get = (PyObject *(*)(struct __pyx_obj_3aim_5_core_7storage_9container_Container *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_3aim_5_core_7storage_9container_9Container_get *__pyx_optional_args))__pyx_f_3aim_5_core_7storage_9container_9Container_get;
   __pyx_vtable_3aim_5_core_7storage_9container_Container.set = (void (*)(struct __pyx_obj_3aim_5_core_7storage_9container_Container *, PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_3aim_5_core_7storage_9container_9Container_set *__pyx_optional_args))__pyx_f_3aim_5_core_7storage_9container_9Container_set;
   __pyx_vtable_3aim_5_core_7storage_9container_Container.delete_range = (void (*)(struct __pyx_obj_3aim_5_core_7storage_9container_Container *, PyObject *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_3aim_5_core_7storage_9container_9Container_delete_range *__pyx_optional_args))__pyx_f_3aim_5_core_7storage_9container_9Container_delete_range;
@@ -13685,23 +13685,23 @@
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Container, (PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_Container) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   if (__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_weaklistoffset == 0) __pyx_ptype_3aim_5_core_7storage_9container_Container->tp_weaklistoffset = offsetof(struct __pyx_obj_3aim_5_core_7storage_9container_Container, __weakref__);
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_3aim_5_core_7storage_9container_Container) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3aim_5_core_7storage_9container___pyx_scope_struct__samples_spec, NULL); if (unlikely(!__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples)) __PYX_ERR(0, 146, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3aim_5_core_7storage_9container___pyx_scope_struct__samples_spec, __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_3aim_5_core_7storage_9container___pyx_scope_struct__samples_spec, NULL); if (unlikely(!__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples)) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_3aim_5_core_7storage_9container___pyx_scope_struct__samples_spec, __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   #else
   __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples = &__pyx_type_3aim_5_core_7storage_9container___pyx_scope_struct__samples;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples->tp_dictoffset && __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_3aim_5_core_7storage_9container___pyx_scope_struct__samples->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -14553,298 +14553,298 @@
   if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_commit, __pyx_t_3) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
   /* "aim/_core/storage/container.py":116
  *         ...
  * 
- *     def items(self, begin: ContainerKey = b'', end: ContainerKey = b'') -> Iterator[Tuple[ContainerKey, ContainerValue]]:             # <<<<<<<<<<<<<<
- *         """Iterate over all the key-value records in the prefix key range.
- * 
+ *     def items(             # <<<<<<<<<<<<<<
+ *         self,
+ *         begin: ContainerKey = b'',
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_begin, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_end, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_25items, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_items, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__25);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_items, __pyx_t_5) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":146
+  /* "aim/_core/storage/container.py":150
  *         raise NotImplementedError
  * 
  *     def samples(             # <<<<<<<<<<<<<<
  *         self,
  *         begin: ContainerKey = b'',
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_begin, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_end, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_List_Tuple_ContainerKey_Containe) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_27samples, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_samples, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_begin, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_end, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_List_Tuple_ContainerKey_Containe) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_27samples, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_samples, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__27);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_samples, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_samples, __pyx_t_3) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":169
+  /* "aim/_core/storage/container.py":173
  *         yield all_samples
  * 
  *     def keys(self, prefix: ContainerKey = b'') -> Iterator[ContainerKey]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the keys in the prefix range.
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_Iterator_ContainerKey) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_30keys, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_keys, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_Iterator_ContainerKey) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_30keys, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_keys, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__30);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_keys, __pyx_t_5) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_keys, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":189
+  /* "aim/_core/storage/container.py":193
  *         return utils.KeysIterator(self.items(prefix))
  * 
  *     def values(self, prefix: ContainerKey = b'') -> Iterator[ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Iterate over all the values in the given prefix key range.
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_Iterator_ContainerValue) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_32values, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_values, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_Iterator_ContainerValue) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_32values, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_values, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__30);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_values, __pyx_t_3) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_values, __pyx_t_3) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":209
+  /* "aim/_core/storage/container.py":213
  *         return utils.ValuesIterator(self.items(prefix))
  * 
  *     def view(self, prefix: ContainerKey = b'') -> 'Container':             # <<<<<<<<<<<<<<
  *         """Return a view (even mutable ones) that enable access to the container
  *         but with modifications.
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_Container_2) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_34view, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_view, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_Container_2) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_34view, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_view, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__30);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_view, __pyx_t_5) < 0) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_view, __pyx_t_5) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":234
+  /* "aim/_core/storage/container.py":238
  *         ...
  * 
  *     def tree(self) -> 'TreeView':             # <<<<<<<<<<<<<<
  *         """Return a :obj:`TreeView` which enables hierarchical view and access
  *         to the container records.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_TreeView_2) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_36tree, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_tree, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_TreeView_2) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_36tree, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_tree, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_tree, __pyx_t_3) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_tree, __pyx_t_3) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":253
+  /* "aim/_core/storage/container.py":257
  *         ...
  * 
  *     def walk(self, prefix: ContainerKey = b''):             # <<<<<<<<<<<<<<
  *         """A bi-directional generator to walk over the collection of records on
  *         any arbitrary order. The `prefix` sent to the generator (lets call it
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_38walk, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_walk, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_prefix, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_38walk, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_walk, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__30);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_walk, __pyx_t_5) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_walk, __pyx_t_5) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":269
+  /* "aim/_core/storage/container.py":273
  *         ...
  * 
  *     def next_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right after the
  *         provided `key`.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_40next_key, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_key, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_40next_key, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_key, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__37);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_key, __pyx_t_3) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_key, __pyx_t_3) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":276
+  /* "aim/_core/storage/container.py":280
  *         return key
  * 
  *     def next_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         after the provided `key`.
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_42next_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_42next_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__39);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_value, __pyx_t_5) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_value, __pyx_t_5) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":283
+  /* "aim/_core/storage/container.py":287
  *         return value
  * 
  *     def next_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_44next_key_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_key_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_44next_key_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_key_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__41);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_key_value, __pyx_t_3) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_key_value, __pyx_t_3) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":289
+  /* "aim/_core/storage/container.py":293
  *         return self.next_item(key)
  * 
  *     def next_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right after the provided `key`.
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_46next_item, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_item, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_46next_item, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_next_item, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__43);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_item, __pyx_t_5) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_next_item, __pyx_t_5) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":295
+  /* "aim/_core/storage/container.py":299
  *         ...
  * 
  *     def prev_key(self, key: ContainerKey = b'') -> ContainerKey:             # <<<<<<<<<<<<<<
  *         """Returns the key that comes (lexicographically) right before the
  *         provided `key`.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_48prev_key, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_key, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_48prev_key, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_key, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__45);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_key, __pyx_t_3) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_key, __pyx_t_3) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":302
+  /* "aim/_core/storage/container.py":306
  *         return key
  * 
  *     def prev_value(self, key: ContainerKey = b'') -> ContainerValue:             # <<<<<<<<<<<<<<
  *         """Returns the value for the key that comes (lexicographically) right
  *         before the provided `key`.
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_50prev_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_50prev_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__47);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_value, __pyx_t_5) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_value, __pyx_t_5) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":309
+  /* "aim/_core/storage/container.py":313
  *         return value
  * 
  *     def prev_key_value(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_52prev_key_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_key_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 309, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_52prev_key_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_key_value, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__49);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_key_value, __pyx_t_3) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_key_value, __pyx_t_3) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
-  /* "aim/_core/storage/container.py":315
+  /* "aim/_core/storage/container.py":319
  *         return self.prev_item(key)
  * 
  *     def prev_item(self, key: ContainerKey = b'') -> Tuple[ContainerKey, ContainerValue]:             # <<<<<<<<<<<<<<
  *         """Returns `(key, value)` for the key that comes (lexicographically)
  *         right before the provided `key`.
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_54prev_item, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_item, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 315, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_n_s_ContainerKey) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_3aim_5_core_7storage_9container_9Container_54prev_item, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Container_prev_item, NULL, __pyx_n_s_aim__core_storage_container, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_tuple__51);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_item, __pyx_t_5) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_3aim_5_core_7storage_9container_Container->tp_dict, __pyx_n_s_prev_item, __pyx_t_5) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   PyType_Modified(__pyx_ptype_3aim_5_core_7storage_9container_Container);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.pxd` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/container.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,19 @@
         """Execute the accumulated write operations in the given `batch`.
 
         Depending on the :obj:`Container` implementation, this may feature
         transactions, atomic writes, etc.
         """
         ...
 
-    def items(self, begin: ContainerKey = b'', end: ContainerKey = b'') -> Iterator[Tuple[ContainerKey, ContainerValue]]:
+    def items(
+        self,
+        begin: ContainerKey = b'',
+        end: ContainerKey = b''
+    ) -> Iterator[Tuple[ContainerKey, ContainerValue]]:
         """Iterate over all the key-value records in the prefix key range.
 
         The iteration is always performed in lexiographic order w.r.t keys.
         If `begin` is provided, iterate only over those records that have key
         starting with the `begin`. If `end` is provided, iterate only over
         those records lexigraphically strictly smaller than `end`.
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/containertreeview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/containertreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.containertreeview",
         "sources": [
             "src/py-sdk/aim/_core/storage/containertreeview.py"
         ]
     },
     "module_name": "aim._core.storage.containertreeview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/containertreeview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/containertreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/__init__.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding",
         "sources": [
             "src/py-sdk/aim/_core/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.encoding"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding",
         "sources": [
             "src/py-sdk/aim/_core/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.encoding.encoding_native",
         "sources": [
             "src/py-sdk/aim/_core/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim._core.storage.encoding.encoding_native"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.pxd` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/encoding/encoding_native.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/__init__.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/py-sdk/aim/_core/storage/hashing",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing",
         "sources": [
             "src/py-sdk/aim/_core/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim._core.storage.hashing"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/c_hash.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/py-sdk/aim/_core/storage/hashing",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.c_hash",
         "sources": [
             "src/py-sdk/aim/_core/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim._core.storage.hashing.c_hash"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/c_hash.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hash/hash.h` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "src/py-sdk/aim/_core/storage/hashing",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.hashing.hashing",
         "sources": [
             "src/py-sdk/aim/_core/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim._core.storage.hashing.hashing"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.pxd` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/hashing/hashing.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/inmemorytreeview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.inmemorytreeview",
         "sources": [
             "src/py-sdk/aim/_core/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim._core.storage.inmemorytreeview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/inmemorytreeview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/locking.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/object.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/object.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.prefixview",
         "sources": [
             "src/py-sdk/aim/_core/storage/prefixview.py"
         ]
     },
     "module_name": "aim._core.storage.prefixview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.pxd` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/prefixview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/prefixview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/proxy.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/rockscontainer.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/rockscontainer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.rockscontainer",
         "sources": [
             "src/py-sdk/aim/_core/storage/rockscontainer.pyx"
         ]
     },
     "module_name": "aim._core.storage.rockscontainer"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/rockscontainer.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treearrayview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treearrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treearrayview",
         "sources": [
             "src/py-sdk/aim/_core/storage/treearrayview.py"
         ]
     },
     "module_name": "aim._core.storage.treearrayview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treearrayview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeutils",
         "sources": [
             "src/py-sdk/aim/_core/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim._core.storage.treeutils"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeutils_non_native.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeview.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.treeview",
         "sources": [
             "src/py-sdk/aim/_core/storage/treeview.py"
         ]
     },
     "module_name": "aim._core.storage.treeview"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/treeview.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/types.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/union.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/union.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.union",
         "sources": [
             "src/py-sdk/aim/_core/storage/union.pyx"
         ]
     },
     "module_name": "aim._core.storage.union"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/union.pyx` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/union.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/utils.cpp` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-r9_oaz9t/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-ykheh7_e/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim._core.storage.utils",
         "sources": [
             "src/py-sdk/aim/_core/storage/utils.py"
         ]
     },
     "module_name": "aim._core.storage.utils"
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/storage/utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_core/utils/deprecation.py` & `aim-4.0.0a9/src/py-sdk/aim/_core/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/exception_resistant.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/exception_resistant.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/manager.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notebook/notebook.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/__init__.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/config.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/logging_notifier.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/notifier.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/notifier_builder.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/slack_notifier.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/notifier/workplace_notifier.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/pynvml.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/pynvml.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/resource_tracker.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/stat.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/stat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/system_info/utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/system_info/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_ext/tracking/__init__.py` & `aim-4.0.0a9/src/py-sdk/aim/_ext/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/collections.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/collections.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/constants.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/container.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 from aim._sdk.context import Context
 
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from aim._core.storage.treeview import TreeView
     from aim._sdk.repo import Repo
-
+    from aim._sdk.collections import ContainerCollection
 
 logger = logging.getLogger(__name__)
 
 
 class ContainerAutoClean(AutoClean['Container']):
     PRIORITY = 90
 
     def __init__(self, instance: 'Container') -> None:
         super().__init__(instance)
 
         self.mode = instance.mode
         self.hash = instance.hash
 
+        self._state = instance._state
         self._tree = instance._tree
         self.storage = instance.storage
 
         self._status_reporter = instance._status_reporter
         self._lock = instance._lock
 
     def _set_end_time(self):
@@ -63,14 +64,15 @@
         """
         Close the `Run` instance resources and trigger indexing.
         """
         if self.mode == ContainerOpenMode.READONLY:
             logger.debug(f'Run {self.hash} is read-only, skipping cleanup')
             return
 
+        self._state['cleanup'] = True
         self._wait_for_empty_queue()
         self._set_end_time()
         if self._status_reporter is not None:
             self._status_reporter.close()
         if self._lock:
             self._lock.release()
 
@@ -107,14 +109,15 @@
             else:
                 raise MissingContainerError(hash_, mode)
 
         self._resources: Optional[ContainerAutoClean] = None
         self._hash = self._calc_hash()
         self._lock = None
         self._status_reporter = None
+        self._state = {}
 
         if not self._is_readonly:
             self._lock = self.storage.lock(self.hash, 0)
             self._status_reporter = self.storage.status_reporter(self.hash)
 
         if self._is_readonly:
             self._meta_tree: TreeView = repo._meta_tree
@@ -145,22 +148,27 @@
         self.storage = storage
         self.hash = hash_
 
         self._resources = None
         self._hash = self._calc_hash()
         self._lock = None
         self._status_reporter = None
+        self._state = {}
         self._meta_tree = meta_tree
 
         self.__storage_init__()
-
-        self._resources = ContainerAutoClean(self)
-
         return self
 
+    @classmethod
+    def filter(cls, expr: str = '', repo: 'Repo' = None) -> 'ContainerCollection':
+        if repo is None:
+            from aim._sdk.repo import Repo
+            repo = Repo.active_repo()
+        return repo.containers(query_=expr, type_=cls)
+
     def __storage_init__(self):
         self._tree: TreeView = self._meta_tree.subtree('chunks').subtree(self.hash)
         self._meta_attrs_tree: TreeView = self._meta_tree.subtree('attrs')
         self._attrs_tree: TreeView = self._tree.subtree('attrs')
 
         self._data_loader: Callable[[], 'TreeView'] = lambda: self._sequence_data_tree
         self.__sequence_data_tree: TreeView = None
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/context.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/context.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/exceptions.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/container.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/interfaces/sequence.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/interfaces/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/local_storage.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/local_storage.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/lock_manager.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/lock_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/num_utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/package_utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/package_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/query.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/query_utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/remote_storage.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/remote_storage.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/repo.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 from aim._ext.system_info.resource_tracker import ResourceTracker
 
 logger = logging.getLogger(__name__)
 
 
 class Repo(object):
-    _pool = WeakValueDictionary()
+    _pool: Dict[str, 'Repo'] = WeakValueDictionary()
 
     @staticmethod
     def is_remote_path(path: str) -> bool:
         return path.startswith('aim://')
 
     @classmethod
-    def default(cls):
+    def default(cls) -> 'Repo':
         return cls.from_path('aim://127.0.0.1:53800')
 
     @classmethod
-    def from_path(cls, path: str, read_only: bool = True):
+    def from_path(cls, path: str, read_only: bool = True) -> 'Repo':
         """Named constructor for Repo for given path.
 
         Arguments:
             path (:obj:`str`): Path to Aim repository.
             read_only (:obj:`bool`, optional): Flag for opening Repo in readonly mode. False by default.
             init (:obj:`bool`, optional): Flag used to initialize new Repo. False by default.
                 Recommended to use ``aim init`` command instead.
@@ -53,14 +53,24 @@
             path = clean_repo_path(path)
         repo = cls._pool.get(path)
         if repo is None:
             repo = cls(path, read_only=read_only)
             cls._pool[path] = repo
         return repo
 
+    @classmethod
+    def active_repo(cls) -> 'Repo':
+        if len(cls._pool) == 0:
+            return cls.default()
+        elif len(cls._pool) == 1:
+            path = next(cls._pool.keys())
+            return cls._pool[path]
+        else:
+            raise ValueError('Cannot determine active Repo. Please use Repo.from_path() instead.')
+
     def __init__(self, path: str, *, read_only: Optional[bool] = True):
         self.read_only = read_only
         if self.is_remote_path(path):
             self._storage_engine = RemoteStorage(path)
         else:
             self.root_path = path
             self.path = os.path.join(self.root_path, get_aim_repo_name())
@@ -211,16 +221,18 @@
 
         if issubclass(orig_type, Container):
             query_context.update({
                 KeyNames.CONTAINER_TYPES_MAP: self._meta_tree.subtree(KeyNames.CONTAINER_TYPES_MAP),
                 KeyNames.CONTAINER_TYPE: type_,
                 'required_typename': type_.get_full_typename(),
             })
-            return ContainerCollection[type_](query_context=query_context)
+            # return ContainerCollection[type_](query_context=query_context)
+            return ContainerCollection(query_context=query_context)
         if issubclass(orig_type, Sequence):
             query_context.update({
                 KeyNames.ALLOWED_VALUE_TYPES: type_utils.get_sequence_value_types(type_),
                 KeyNames.CONTAINER_TYPE: Container,
                 KeyNames.SEQUENCE_TYPE: type_,
                 'required_typename': type_.get_full_typename(),
             })
-            return SequenceCollection[type_](query_context=query_context)
+            # return SequenceCollection[type_](query_context=query_context)
+            return SequenceCollection(query_context=query_context)
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/sequence.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from aim._sdk.context import Context, cached_context
 from aim._sdk.query import RestrictedPythonQuery
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from aim._core.storage.treeview import TreeView
     from aim._sdk.container import Container
+    from aim._sdk.collections import SequenceCollection
     from aim._sdk.storage_engine import StorageEngine
+    from aim._sdk.repo import Repo
 
 _ContextInfo = Union[Dict, Context, int]
 
 logger = logging.getLogger(__name__)
 
 
 class _SequenceInfo:
@@ -110,14 +112,21 @@
 
         self._data_loader = lambda: storage.tree(hash_, 'seqs', read_only=True).subtree('chunks').subtree(hash_)
         self.__data: TreeView = None
 
         self.__storage_init__()
         return self
 
+    @classmethod
+    def filter(cls, expr: str = '', repo: 'Repo' = None) -> 'SequenceCollection':
+        if repo is None:
+            from aim._sdk.repo import Repo
+            repo = Repo.active_repo()
+        return repo.sequences(query_=expr, type_=cls)
+
     def _init_context(self, context: _ContextInfo):
         if isinstance(context, int):
             self._ctx_idx = context
             self._context = None
         elif isinstance(context, dict):
             self._context = Context(context)
             self._ctx_idx = self._context.idx
@@ -146,14 +155,24 @@
 
     @property
     def is_empty(self) -> bool:
         self._info.preload()
         return self._info.empty
 
     @property
+    def start(self) -> int:
+        self._info.preload()
+        return self._info.first_step
+
+    @property
+    def stop(self) -> int:
+        self._info.preload()
+        return self._info.last_step
+
+    @property
     def next_step(self) -> int:
         self._info.preload()
         return self._info.next_step
 
     def match(self, expr) -> bool:
         query = RestrictedPythonQuery(expr)
         query_cache = dict
```

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/storage_engine.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/storage_engine.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/type_utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/type_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/uri_service.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0a7/src/py-sdk/aim/_sdk/utils.py` & `aim-4.0.0a9/src/py-sdk/aim/_sdk/utils.py`

 * *Files identical despite different names*

