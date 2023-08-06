# Comparing `tmp/tokotime-0.141.tar.gz` & `tmp/tokotime-0.142.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokotime-0.141.tar", last modified: Sun Aug  6 06:14:07 2023, max compression
+gzip compressed data, was "tokotime-0.142.tar", last modified: Sun Aug  6 06:21:51 2023, max compression
```

## Comparing `tokotime-0.141.tar` & `tokotime-0.142.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.487479 tokotime-0.141/
--rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.141/LICENSE.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      789 2023-08-06 06:14:07.487592 tokotime-0.141/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.141/README.md
--rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 06:14:07.487975 tokotime-0.141/setup.cfg
--rw-r--r--   0 alanchn    (501) staff       (20)     1927 2023-08-06 06:13:35.000000 tokotime-0.141/setup.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.478358 tokotime-0.141/src/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 05:08:59.000000 tokotime-0.141/src/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.478645 tokotime-0.141/src/tokotime/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.480848 tokotime-0.141/src/tokotime/data_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/data_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/data_utils/utils.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.481420 tokotime-0.141/src/tokotime/experiment_design/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/experiment_design/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/experiment_design/random_sampler.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.481994 tokotime-0.141/src/tokotime/features_eng/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/features_eng/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/features_eng/base_eng.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.482599 tokotime-0.141/src/tokotime/hp_tune/
--rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/hp_tune/bayes_hp_tuner.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.485690 tokotime-0.141/src/tokotime/point_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6457 2023-08-06 06:00:51.000000 tokotime-0.141/src/tokotime/point_forecasts/evaluation_metrics.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2054 2023-08-06 06:10:08.000000 tokotime-0.141/src/tokotime/point_forecasts/evaluator.py
--rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/misc.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/model_mapping.py
--rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/model_runner.py
--rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/model_wrappers.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/ts_class.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/point_forecasts/validation.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.486631 tokotime-0.141/src/tokotime/preprocess_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/preprocess_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/preprocess_utils/preprocess_components.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6906 2023-08-06 05:29:15.000000 tokotime-0.141/src/tokotime/preprocess_utils/preprocessors.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.487223 tokotime-0.141/src/tokotime/probabilistic_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/probabilistic_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.141/src/tokotime/probabilistic_forecasts/evaluation_metrics.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:14:07.480233 tokotime-0.141/src/tokotime.egg-info/
--rw-r--r--   0 alanchn    (501) staff       (20)      789 2023-08-06 06:14:07.000000 tokotime-0.141/src/tokotime.egg-info/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)     1181 2023-08-06 06:14:07.000000 tokotime-0.141/src/tokotime.egg-info/SOURCES.txt
--rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 06:14:07.000000 tokotime-0.141/src/tokotime.egg-info/dependency_links.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      157 2023-08-06 06:14:07.000000 tokotime-0.141/src/tokotime.egg-info/requires.txt
--rw-r--r--   0 alanchn    (501) staff       (20)       18 2023-08-06 06:14:07.000000 tokotime-0.141/src/tokotime.egg-info/top_level.txt
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.665558 tokotime-0.142/
+-rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.142/LICENSE.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      789 2023-08-06 06:21:51.665664 tokotime-0.142/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.142/README.md
+-rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 06:21:51.666172 tokotime-0.142/setup.cfg
+-rw-r--r--   0 alanchn    (501) staff       (20)     1927 2023-08-06 06:21:45.000000 tokotime-0.142/setup.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.655509 tokotime-0.142/src/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 05:08:59.000000 tokotime-0.142/src/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.655874 tokotime-0.142/src/tokotime/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.658248 tokotime-0.142/src/tokotime/data_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/data_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/data_utils/utils.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.658900 tokotime-0.142/src/tokotime/experiment_design/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/experiment_design/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/experiment_design/random_sampler.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.659458 tokotime-0.142/src/tokotime/features_eng/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/features_eng/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/features_eng/base_eng.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.659808 tokotime-0.142/src/tokotime/hp_tune/
+-rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/hp_tune/bayes_hp_tuner.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.663092 tokotime-0.142/src/tokotime/point_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     5592 2023-08-06 06:17:24.000000 tokotime-0.142/src/tokotime/point_forecasts/evaluation_metrics.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     3016 2023-08-06 06:19:10.000000 tokotime-0.142/src/tokotime/point_forecasts/evaluator.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/misc.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/model_mapping.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/model_runner.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/model_wrappers.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/ts_class.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/point_forecasts/validation.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.664391 tokotime-0.142/src/tokotime/preprocess_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/preprocess_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/preprocess_utils/preprocess_components.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6906 2023-08-06 05:29:15.000000 tokotime-0.142/src/tokotime/preprocess_utils/preprocessors.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.665310 tokotime-0.142/src/tokotime/probabilistic_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/probabilistic_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.142/src/tokotime/probabilistic_forecasts/evaluation_metrics.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 06:21:51.657615 tokotime-0.142/src/tokotime.egg-info/
+-rw-r--r--   0 alanchn    (501) staff       (20)      789 2023-08-06 06:21:51.000000 tokotime-0.142/src/tokotime.egg-info/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)     1181 2023-08-06 06:21:51.000000 tokotime-0.142/src/tokotime.egg-info/SOURCES.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 06:21:51.000000 tokotime-0.142/src/tokotime.egg-info/dependency_links.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      157 2023-08-06 06:21:51.000000 tokotime-0.142/src/tokotime.egg-info/requires.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)       18 2023-08-06 06:21:51.000000 tokotime-0.142/src/tokotime.egg-info/top_level.txt
```

### Comparing `tokotime-0.141/LICENSE.txt` & `tokotime-0.142/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/PKG-INFO` & `tokotime-0.142/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.141
+Version: 0.142
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0141.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0142.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tokotime-0.141/setup.py` & `tokotime-0.142/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from distutils.core import setup
 setup(
   name = 'tokotime',         # How you named your package folder (MyLib)
-  version = '0.141',      # Start with a small number and increase it with every change you make
+  version = '0.142',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "Tokopedia Data Science Forecasting Reusable Package",   # Give a short description about your library
   author = 'Alan Choon',                   # Type in your name
   author_email = 'alan.yu@tokopedia.com',      # Type in your E-Mail
   url = 'https://github.com/tokopedia/forecasting-platform-utils',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0141.tar.gz',
+  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0142.tar.gz',
   keywords = ['Forecasting', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
         'darts',
         'lightgbm',
         'mpire',
         'numpy',
         'optuna',
```

### Comparing `tokotime-0.141/src/tokotime/data_utils/utils.py` & `tokotime-0.142/src/tokotime/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/experiment_design/random_sampler.py` & `tokotime-0.142/src/tokotime/experiment_design/random_sampler.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/features_eng/base_eng.py` & `tokotime-0.142/src/tokotime/features_eng/base_eng.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/hp_tune/bayes_hp_tuner.py` & `tokotime-0.142/src/tokotime/hp_tune/bayes_hp_tuner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/evaluation_metrics.py` & `tokotime-0.142/src/tokotime/point_forecasts/evaluation_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -164,29 +164,8 @@
             wsdpe: WSDPE of predictions vs targets
     '''
     denum = np.mean(targets)
     if denum == 0:
         return np.nan # unidentified
     else:
         wsdpe = np.sqrt(np.mean((targets-predictions)**2)) / denum
-        return wsdpe
-
-def evaluate_predictions(df: pd.DataFrame, prediction_cols: List[str], 
-                         target_col: str, eval_func: Callable) -> pd.DataFrame:
-    '''
-    Returns a dataframe containing evaluation results of indicated prediction_cols vs target col
-        Parameters:
-            1. df: A grouped pandas dataframe to apply evaluation on
-            2. prediction_cols: A list of column names containing predictions to evaluate
-            3. target_col: Name of target col to evaluate against
-            4. eval_func: Evaluation function to apply on predictions and target col
-
-        Returns:
-            results_df: Dataframe containing evaluation results
-    '''
-    out = []
-    for col in prediction_cols:
-        out.append(eval_func(df[target_col], df[col]))
-        out['prediction'] = col
-
-    results_df = pd.Series(out)
-    return results_df
+        return wsdpe
```

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/evaluator.py` & `tokotime-0.142/src/tokotime/point_forecasts/evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,47 @@
         '''
         self.df = df
         self.prediction_cols = prediction_cols
         self.group_cols_lst = group_cols_lst
         self.target_col = target_col
         self.eval_funcs = eval_funcs
 
+    @staticmethod
+    def evaluate_predictions(self, df: pd.DataFrame, prediction_cols: List[str], 
+                         target_col: str, eval_func: Callable) -> pd.DataFrame:
+        '''
+        Returns a dataframe containing evaluation results of indicated prediction_cols vs target col
+            Parameters:
+                1. df: A grouped pandas dataframe to apply evaluation on
+                2. prediction_cols: A list of column names containing predictions to evaluate
+                3. target_col: Name of target col to evaluate against
+                4. eval_func: Evaluation function to apply on predictions and target col
+
+            Returns:
+                results_df: Dataframe containing evaluation results
+        '''
+        out = []
+        for col in prediction_cols:
+            out.append(eval_func(df[target_col], df[col]))
+            out['prediction'] = col
+
+        results_df = pd.Series(out)
+        return results_df
+
 
     def evaluate(self) -> pd.DataFrame:
         '''
         Returns a dataframe containing evaluation results of indicated prediction_cols vs target col
             Returns:
                 eval_df: Dataframe containing evaluation results
         '''
         eval_dfs_lst = []
         for eval_func in self.eval_funcs:
             eval_df = pd.DataFrame(self.df.groupby(self.group_cols_lst)
-                                          .apply(lambda x : evaluate_predictions(x, self.prediction_cols,
+                                          .apply(lambda x : self.evaluate_predictions(x, self.prediction_cols,
                                                                                  self.target_col, 
                                                                                  eval_func))).reset_index()
             eval_df['eval_function'] = eval_func.__name__
             
             eval_dfs_lst.append(eval_df)
         eval_final_df = pd.concat(eval_dfs_lst)
         eval_final_df.sort_values(by=self.group_cols_lst, inplace=True)
```

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/model_mapping.py` & `tokotime-0.142/src/tokotime/point_forecasts/model_mapping.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/model_runner.py` & `tokotime-0.142/src/tokotime/point_forecasts/model_runner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/model_wrappers.py` & `tokotime-0.142/src/tokotime/point_forecasts/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/ts_class.py` & `tokotime-0.142/src/tokotime/point_forecasts/ts_class.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/point_forecasts/validation.py` & `tokotime-0.142/src/tokotime/point_forecasts/validation.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/preprocess_utils/preprocess_components.py` & `tokotime-0.142/src/tokotime/preprocess_utils/preprocess_components.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/preprocess_utils/preprocessors.py` & `tokotime-0.142/src/tokotime/preprocess_utils/preprocessors.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime/probabilistic_forecasts/evaluation_metrics.py` & `tokotime-0.142/src/tokotime/probabilistic_forecasts/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.141/src/tokotime.egg-info/PKG-INFO` & `tokotime-0.142/src/tokotime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.141
+Version: 0.142
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0141.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_0142.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tokotime-0.141/src/tokotime.egg-info/SOURCES.txt` & `tokotime-0.142/src/tokotime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

