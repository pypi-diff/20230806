# Comparing `tmp/autogluon.timeseries-0.8.3b20230804.tar.gz` & `tmp/autogluon.timeseries-0.8.3b20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.8.3b20230804.tar", last modified: Fri Aug  4 09:04:25 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.8.3b20230805.tar", last modified: Sat Aug  5 09:04:13 2023, max compression
```

## Comparing `autogluon.timeseries-0.8.3b20230804.tar` & `autogluon.timeseries-0.8.3b20230805.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.118595 autogluon.timeseries-0.8.3b20230804/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:04:25.118595 autogluon.timeseries-0.8.3b20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49176 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.114595 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-04 09:03:48.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 09:04:24.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:25.110595 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:25.000000 autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.523956 autogluon.timeseries-0.8.3b20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-08-05 09:04:13.523956 autogluon.timeseries-0.8.3b20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:04:13.523956 autogluon.timeseries-0.8.3b20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.503956 autogluon.timeseries-0.8.3b20230805/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.503956 autogluon.timeseries-0.8.3b20230805/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.515956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.515956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.515956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49176 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.519956 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-05 09:03:35.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:04:13.511956 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:04:13.000000 autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.8.3b20230804/PKG-INFO` & `autogluon.timeseries-0.8.3b20230805/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
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

### Comparing `autogluon.timeseries-0.8.3b20230804/setup.py` & `autogluon.timeseries-0.8.3b20230805/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.8.3b20230805/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
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

### Comparing `autogluon.timeseries-0.8.3b20230804/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.8.3b20230805/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

