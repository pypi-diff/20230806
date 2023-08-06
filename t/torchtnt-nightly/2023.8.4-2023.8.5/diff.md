# Comparing `tmp/torchtnt-nightly-2023.8.4.tar.gz` & `tmp/torchtnt-nightly-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt-nightly-2023.8.4.tar", last modified: Fri Aug  4 11:25:59 2023, max compression
+gzip compressed data, was "torchtnt-nightly-2023.8.5.tar", last modified: Sat Aug  5 11:24:59 2023, max compression
```

## Comparing `torchtnt-nightly-2023.8.4.tar` & `torchtnt-nightly-2023.8.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.168450 torchtnt-nightly-2023.8.4/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.172450 torchtnt-nightly-2023.8.4/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.176450 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.188450 torchtnt-nightly-2023.8.4/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.192450 torchtnt-nightly-2023.8.4/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/flops.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.192450 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/prepare_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-04 11:23:01.000000 torchtnt-nightly-2023.8.4/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:25:59.196450 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:25:59.000000 torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.725908 torchtnt-nightly-2023.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-05 11:24:59.725908 torchtnt-nightly-2023.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 11:24:59.725908 torchtnt-nightly-2023.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.693908 torchtnt-nightly-2023.8.5/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.697908 torchtnt-nightly-2023.8.5/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37488 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.705908 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.717908 torchtnt-nightly-2023.8.5/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.717908 torchtnt-nightly-2023.8.5/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.721908 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27731 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-05 11:22:01.000000 torchtnt-nightly-2023.8.5/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:59.725908 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:24:59.000000 torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.8.4/LICENSE` & `torchtnt-nightly-2023.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/PKG-INFO` & `torchtnt-nightly-2023.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.8.4
+Version: 2023.8.5
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.4 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.5 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.8.4/README.md` & `torchtnt-nightly-2023.8.5/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/setup.py` & `torchtnt-nightly-2023.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/_callback_handler.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/_callback_handler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/state.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/train.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.8.5/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/data/profile_dataloader.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/device.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/env.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/flops.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/flops.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/module_summary.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/prepare_module.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/prepare_module.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/progress.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/stateful.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/stateful.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/tqdm.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt/utils/version.py` & `torchtnt-nightly-2023.8.5/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.8.4
+Version: 2023.8.5
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.4 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.8.5 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.8.4/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.8.5/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

