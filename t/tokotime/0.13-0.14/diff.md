# Comparing `tmp/tokotime-0.13.tar.gz` & `tmp/tokotime-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokotime-0.13.tar", last modified: Sun Aug  6 05:14:15 2023, max compression
+gzip compressed data, was "tokotime-0.14.tar", last modified: Sun Aug  6 06:05:49 2023, max compression
```

## Comparing `tokotime-0.13.tar` & `tokotime-0.14.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.369949 tokotime-0.13/
--rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.13/LICENSE.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:14:15.370054 tokotime-0.13/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.13/README.md
--rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 05:14:15.370367 tokotime-0.13/setup.cfg
--rw-r--r--   0 alanchn    (501) staff       (20)     1904 2023-08-06 05:10:51.000000 tokotime-0.13/setup.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.359758 tokotime-0.13/src/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 05:08:59.000000 tokotime-0.13/src/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.360041 tokotime-0.13/src/tokotime/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.362826 tokotime-0.13/src/tokotime/data_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/data_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/data_utils/utils.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.363479 tokotime-0.13/src/tokotime/experiment_design/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/experiment_design/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/experiment_design/random_sampler.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.364208 tokotime-0.13/src/tokotime/features_eng/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/features_eng/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/features_eng/base_eng.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.364590 tokotime-0.13/src/tokotime/hp_tune/
--rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/hp_tune/bayes_hp_tuner.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.367359 tokotime-0.13/src/tokotime/point_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     9853 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/evaluation_metrics.py
--rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/misc.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_mapping.py
--rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_runner.py
--rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_wrappers.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/ts_class.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/validation.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.368514 tokotime-0.13/src/tokotime/preprocess_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/preprocess_components.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6911 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/preprocessors.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.369631 tokotime-0.13/src/tokotime/probabilistic_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/probabilistic_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/probabilistic_forecasts/evaluation_metrics.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.361719 tokotime-0.13/src/tokotime.egg-info/
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:14:14.000000 tokotime-0.13/src/tokotime.egg-info/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)     1139 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/SOURCES.txt
--rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 05:14:14.000000 tokotime-0.13/src/tokotime.egg-info/dependency_links.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      146 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/requires.txt
--rw-r--r--   0 alanchn    (501) staff       (20)       18 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/top_level.txt
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.187490 tokotime-0.14/
+-rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.14/LICENSE.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 06:05:49.187612 tokotime-0.14/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.14/README.md
+-rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 06:05:49.188077 tokotime-0.14/setup.cfg
+-rw-r--r--   0 alanchn    (501) staff       (20)     1925 2023-08-06 06:05:12.000000 tokotime-0.14/setup.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.175781 tokotime-0.14/src/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 05:08:59.000000 tokotime-0.14/src/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.176126 tokotime-0.14/src/tokotime/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.179026 tokotime-0.14/src/tokotime/data_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/data_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/data_utils/utils.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.179735 tokotime-0.14/src/tokotime/experiment_design/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/experiment_design/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/experiment_design/random_sampler.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.180654 tokotime-0.14/src/tokotime/features_eng/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/features_eng/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/features_eng/base_eng.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.181102 tokotime-0.14/src/tokotime/hp_tune/
+-rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/hp_tune/bayes_hp_tuner.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.184464 tokotime-0.14/src/tokotime/point_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6457 2023-08-06 06:00:51.000000 tokotime-0.14/src/tokotime/point_forecasts/evaluation_metrics.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2048 2023-08-06 05:58:57.000000 tokotime-0.14/src/tokotime/point_forecasts/evaluator.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/misc.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/model_mapping.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/model_runner.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/model_wrappers.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/ts_class.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/point_forecasts/validation.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.185482 tokotime-0.14/src/tokotime/preprocess_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/preprocess_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/preprocess_utils/preprocess_components.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6906 2023-08-06 05:29:15.000000 tokotime-0.14/src/tokotime/preprocess_utils/preprocessors.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.186988 tokotime-0.14/src/tokotime/probabilistic_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/probabilistic_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.14/src/tokotime/probabilistic_forecasts/evaluation_metrics.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:05:49.178261 tokotime-0.14/src/tokotime.egg-info/
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 06:05:48.000000 tokotime-0.14/src/tokotime.egg-info/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)     1181 2023-08-06 06:05:49.000000 tokotime-0.14/src/tokotime.egg-info/SOURCES.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 06:05:48.000000 tokotime-0.14/src/tokotime.egg-info/dependency_links.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      157 2023-08-06 06:05:48.000000 tokotime-0.14/src/tokotime.egg-info/requires.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)       18 2023-08-06 06:05:49.000000 tokotime-0.14/src/tokotime.egg-info/top_level.txt
```

### Comparing `tokotime-0.13/LICENSE.txt` & `tokotime-0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/setup.py` & `tokotime-0.14/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from distutils.core import setup
 setup(
   name = 'tokotime',         # How you named your package folder (MyLib)
-  version = '0.13',      # Start with a small number and increase it with every change you make
+  version = '0.14',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "Tokopedia Data Science Forecasting Reusable Package",   # Give a short description about your library
   author = 'Alan Choon',                   # Type in your name
   author_email = 'alan.yu@tokopedia.com',      # Type in your E-Mail
   url = 'https://github.com/tokopedia/forecasting-platform-utils',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_013.tar.gz',
+  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_014.tar.gz',
   keywords = ['Forecasting', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
         'darts',
         'lightgbm',
         'mpire',
         'numpy',
         'optuna',
@@ -24,14 +24,15 @@
         'scikit_learn',
         'scikit_lego',
         'sklego',
         'sktime',
         'statsmodels',
         'threadpoolctl',
         'tqdm',
+        'ipywidgets'
       ],
   package_dir={"": "src"}, 
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
```

### Comparing `tokotime-0.13/src/tokotime/data_utils/utils.py` & `tokotime-0.14/src/tokotime/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/experiment_design/random_sampler.py` & `tokotime-0.14/src/tokotime/experiment_design/random_sampler.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/features_eng/base_eng.py` & `tokotime-0.14/src/tokotime/features_eng/base_eng.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/hp_tune/bayes_hp_tuner.py` & `tokotime-0.14/src/tokotime/hp_tune/bayes_hp_tuner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/evaluation_metrics.py` & `tokotime-0.14/src/tokotime/point_forecasts/evaluation_metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pandas as pd
 import numpy as np
 import functools as ft
 from typing import Tuple, Callable, List
 
 
-def calculate_mape(targets: np.array, predictions: np.array) -> float:
+def MAPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a MAPE value (Mean Absolute Percentage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
@@ -24,44 +24,44 @@
         assert any(mask) # at least 1 value in mask is True
     except AssertionError:
         return np.nan # unidentified
     else:
         mape = np.fabs((targets[mask]-predictions[mask])/targets[mask]).mean()*100
         return mape
 
-def calculate_mae(targets: np.array, predictions: np.array) -> float:
+def MAE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a MAE value (Mean Absolute Error)
     This is a measure of model performance that is unscaled
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
             mae: MAE of predictions vs targets
     '''
     residual = np.abs(targets-predictions)
     mae = np.mean(residual)
     return mae
 
-def calculate_rmse(targets: np.array, predictions: np.array) -> float:
+def RMSE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a RMSE value (Root Mean Squared Error)
     This is a measure of model performance that is unscaled
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
             rmse: RMSE of predictions vs targets
     '''
     rmse = np.sqrt(np.mean((targets-predictions)**2))
     return rmse
 
-def calculate_maape(targets: np.array, predictions: np.array) -> float:
+def MAAPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a MAAPE value (Mean Arctangent Absolute Percetage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
@@ -81,15 +81,15 @@
         forecast = predictions[mask]
         actual[actual == 0] = 1e-12
         pctg_err = (actual - forecast) / actual
         APE = abs(pctg_err)
         AAPE = np.arctan(APE)
         return np.mean(AAPE)
 
-def calculate_wape(targets: np.array, predictions: np.array) -> float:
+def WAPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a WAPE value (Weighted Average Percentage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
@@ -98,30 +98,30 @@
     resids_summed = np.sum(abs(targets-predictions))
     targets_summed = np.sum(targets)
     if targets_summed == 0:
         return np.nan
     wape = resids_summed/targets_summed
     return wape
 
-def calculate_wbpe(targets: np.array, predictions: np.array) -> float:
+def WBPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a WBPE value (Weighted Bias Percentage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
             wbpe: WBPE of predictions vs targets
     '''
     if np.sum(targets) == 0:
         return np.nan
     wbpe = np.sum(predictions-targets)/np.sum(targets)
     return wbpe
 
-def calculate_pwape(targets: np.array, predictions: np.array) -> float:
+def PWAPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a pWAPE value (positive Weighted Average Percentage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
@@ -130,15 +130,15 @@
     resids_summed = np.sum(np.clip(predictions - targets, 0, None))
     targets_summed = np.sum(targets)
     if targets_summed == 0:
         return np.nan
     pwape = resids_summed/targets_summed
     return pwape
 
-def calculate_nwape(targets: np.array, predictions: np.array) -> float:
+def NWAPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a nWAPE value (negative Weighted Average Percentage Error)
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
         Returns:
@@ -148,15 +148,15 @@
     targets_summed = np.sum(targets)
     if targets_summed == 0:
         return np.nan
 
     nwape = resids_summed/targets_summed
     return nwape
 
-def calculate_wsdpe(targets: np.array, predictions: np.array) -> float:
+def WSDPE(targets: np.array, predictions: np.array) -> float:
     '''
     Returns a WSDPE value (Weighted Standard Deviation Percentage Error)
     It measures how volatile the residuals are relative to the historical mean of the series
         Parameters:
             1. targets: A numpy array containing target values
             2. predictions: A numpy array containing forecasts
 
@@ -182,72 +182,11 @@
 
         Returns:
             results_df: Dataframe containing evaluation results
     '''
     out = []
     for col in prediction_cols:
         out.append(eval_func(df[target_col], df[col]))
+        out['prediction'] = col
 
     results_df = pd.Series(out)
-    return results_df
-
-def evaluate_by_segments(df: pd.DataFrame, prediction_cols: List[str], group_cols_lst: List[str], 
-                         target_col: str, eval_func: Callable, print_results: bool = False) -> pd.DataFrame:
-    '''
-    Returns a dataframe containing evaluation results of indicated prediction_cols vs target col
-        Parameters:
-            1. df: A pandas dataframe to apply evaluation on
-            2. prediction_cols: A list of column names containing predictions to evaluate
-            3. group_cols_lst: A list of column names to act as index to aggregate evaluation results against
-            4. target_col: Name of target col to evaluate against
-            5. eval_func: Evaluation function to apply on predictions and target col
-
-        Returns:
-            eval_df: Dataframe containing evaluation results
-    '''
-    eval_dfs_lst = []
-    
-    for group_cols in group_cols_lst:
-        eval_df = pd.DataFrame(df.groupby(group_cols).apply(lambda x : evaluate_predictions(x, prediction_cols, 
-                                                                                            target_col, 
-                                                                                            eval_func)))
-        eval_df = eval_df.reset_index().groupby(group_cols).mean().T
-        eval_df.index = prediction_cols
-        eval_dfs_lst.append(eval_df)
-        
-    eval_df = pd.concat(eval_dfs_lst, axis = 1)
-    
-    if print_results:
-        display(eval_df)
-    return eval_df
-
-def evaluate_by_segments_multiple_metrics(df: pd.DataFrame, prediction_cols: List[str], 
-                                          group_cols_lst: List[str], 
-                                          target_col: str,
-                                          eval_funcs: Tuple[Callable, ...], 
-                                          print_results: bool = False) -> pd.DataFrame:
-    '''
-    Returns a dataframe containing evaluation results of indicated prediction_cols vs target col
-        Parameters:
-            1. df: A pandas dataframe to apply evaluation on
-            2. prediction_cols: A list of column names containing predictions to evaluate
-            3. group_cols_lst: A list of column names to act as index to aggregate evaluation results against
-            4. target_col: Name of target col to evaluate against
-            5. eval_func: Evaluation function to apply on predictions and target col
-
-        Returns:
-            eval_df: Dataframe containing evaluation results
-    '''
-    eval_dfs_lst = []
-    for eval_func in eval_funcs:
-        eval_df = pd.DataFrame(df.groupby(group_cols_lst).apply(lambda x : evaluate_predictions(x, prediction_cols,
-                                                                                                target_col,
-                                                                                                eval_func))).reset_index()
-        
-        for i in range(len(prediction_cols)):
-            eval_df.rename(columns={i: f"{eval_func.__name__}_{prediction_cols[i]}"}, inplace=True)
-        eval_dfs_lst.append(eval_df)
-    eval_final_df = ft.reduce(lambda left, right: pd.merge(left, right, on=group_cols_lst), eval_dfs_lst)
-    eval_final_df.sort_values(by=group_cols_lst, inplace=True)
-    if print_results:
-        display(eval_df)
-    return eval_final_df
+    return results_df
```

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/model_mapping.py` & `tokotime-0.14/src/tokotime/point_forecasts/model_mapping.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/model_runner.py` & `tokotime-0.14/src/tokotime/point_forecasts/model_runner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/model_wrappers.py` & `tokotime-0.14/src/tokotime/point_forecasts/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/ts_class.py` & `tokotime-0.14/src/tokotime/point_forecasts/ts_class.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/point_forecasts/validation.py` & `tokotime-0.14/src/tokotime/point_forecasts/validation.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/preprocess_utils/preprocess_components.py` & `tokotime-0.14/src/tokotime/preprocess_utils/preprocess_components.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime/preprocess_utils/preprocessors.py` & `tokotime-0.14/src/tokotime/preprocess_utils/preprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,14 @@
         req_preprocess_keys = ['id_columns',  'date_column', 'forecast_column']
         for k in req_preprocess_keys:
             if k not in self.preprocess_params:
                 raise KeyError(f'{k} is a required key in preprocess_params!')
 
     
     def build_valid_params(self) -> None:
-        
-        if 'fill_missing_params' in self.preprocess_params:
-            fill_missing_params = {'fill_missing': self.preprocess_params['fill_missing_params']}
 
         self.preprocess_params = {
             ## Dataframe is mutated by the transformers and dataframe is returned
             '': {
                 'remove_leading_zero': {
                     'date_column': self.preprocess_params['date_column'],
                     'group_key': self.preprocess_params['id_columns'],
@@ -41,15 +38,17 @@
                 'generate_missing_dates': {
                     'date_column': self.preprocess_params['date_column'],
                     'group_key': self.preprocess_params['id_columns']
                 }
             },
         }
 
-        self.preprocess_params[''] = {**self.preprocess_params[''], **fill_missing_params}
+        if 'fill_missing_params' in self.preprocess_params:
+            fill_missing_params = {'fill_missing': self.preprocess_params['fill_missing_params']}
+            self.preprocess_params[''] = {**self.preprocess_params[''], **fill_missing_params}
     
     def run(self) -> pd.DataFrame:
         self.check_preprocess_params()
         self.build_valid_params()
         preprocessed_df = PreprocessFactory(self.preprocess_params).execute(self.df)
         return preprocessed_df
```

### Comparing `tokotime-0.13/src/tokotime/probabilistic_forecasts/evaluation_metrics.py` & `tokotime-0.14/src/tokotime/probabilistic_forecasts/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.13/src/tokotime.egg-info/SOURCES.txt` & `tokotime-0.14/src/tokotime.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/tokotime/experiment_design/__init__.py
 src/tokotime/experiment_design/random_sampler.py
 src/tokotime/features_eng/__init__.py
 src/tokotime/features_eng/base_eng.py
 src/tokotime/hp_tune/bayes_hp_tuner.py
 src/tokotime/point_forecasts/__init__.py
 src/tokotime/point_forecasts/evaluation_metrics.py
+src/tokotime/point_forecasts/evaluator.py
 src/tokotime/point_forecasts/misc.py
 src/tokotime/point_forecasts/model_mapping.py
 src/tokotime/point_forecasts/model_runner.py
 src/tokotime/point_forecasts/model_wrappers.py
 src/tokotime/point_forecasts/ts_class.py
 src/tokotime/point_forecasts/validation.py
 src/tokotime/preprocess_utils/__init__.py
```

