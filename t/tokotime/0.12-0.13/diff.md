# Comparing `tmp/tokotime-0.12.tar.gz` & `tmp/tokotime-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokotime-0.12.tar", last modified: Sun Aug  6 05:06:30 2023, max compression
+gzip compressed data, was "tokotime-0.13.tar", last modified: Sun Aug  6 05:14:15 2023, max compression
```

## Comparing `tokotime-0.12.tar` & `tokotime-0.13.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.007334 tokotime-0.12/
--rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.12/LICENSE.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:06:30.007448 tokotime-0.12/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.12/README.md
--rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 05:06:30.007843 tokotime-0.12/setup.cfg
--rw-r--r--   0 alanchn    (501) staff       (20)     1909 2023-08-06 05:06:16.000000 tokotime-0.12/setup.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.998314 tokotime-0.12/tokotime/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.998900 tokotime-0.12/tokotime/data_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/data_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/data_utils/utils.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.999678 tokotime-0.12/tokotime/experiment_design/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/experiment_design/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/experiment_design/random_sampler.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.000468 tokotime-0.12/tokotime/features_eng/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/features_eng/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/features_eng/base_eng.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.000881 tokotime-0.12/tokotime/hp_tune/
--rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/hp_tune/bayes_hp_tuner.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.003984 tokotime-0.12/tokotime/point_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)     9853 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/evaluation_metrics.py
--rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/misc.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_mapping.py
--rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_runner.py
--rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_wrappers.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/ts_class.py
--rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/validation.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.004876 tokotime-0.12/tokotime/preprocess_utils/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/preprocess_components.py
--rw-r--r--   0 alanchn    (501) staff       (20)     6911 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/preprocessors.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.005399 tokotime-0.12/tokotime/probabilistic_forecasts/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/probabilistic_forecasts/__init__.py
--rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/probabilistic_forecasts/evaluation_metrics.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.007053 tokotime-0.12/tokotime/tokotime.egg-info/
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)     1064 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/SOURCES.txt
--rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/dependency_links.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      146 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/requires.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      116 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/top_level.txt
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.369949 tokotime-0.13/
+-rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.13/LICENSE.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:14:15.370054 tokotime-0.13/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.13/README.md
+-rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 05:14:15.370367 tokotime-0.13/setup.cfg
+-rw-r--r--   0 alanchn    (501) staff       (20)     1904 2023-08-06 05:10:51.000000 tokotime-0.13/setup.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.359758 tokotime-0.13/src/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 05:08:59.000000 tokotime-0.13/src/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.360041 tokotime-0.13/src/tokotime/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.362826 tokotime-0.13/src/tokotime/data_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/data_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/data_utils/utils.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.363479 tokotime-0.13/src/tokotime/experiment_design/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/experiment_design/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/experiment_design/random_sampler.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.364208 tokotime-0.13/src/tokotime/features_eng/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/features_eng/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/features_eng/base_eng.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.364590 tokotime-0.13/src/tokotime/hp_tune/
+-rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/hp_tune/bayes_hp_tuner.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.367359 tokotime-0.13/src/tokotime/point_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9853 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/evaluation_metrics.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/misc.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_mapping.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_runner.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/model_wrappers.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/ts_class.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/point_forecasts/validation.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.368514 tokotime-0.13/src/tokotime/preprocess_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/preprocess_components.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6911 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/preprocess_utils/preprocessors.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.369631 tokotime-0.13/src/tokotime/probabilistic_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/probabilistic_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.13/src/tokotime/probabilistic_forecasts/evaluation_metrics.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:14:15.361719 tokotime-0.13/src/tokotime.egg-info/
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:14:14.000000 tokotime-0.13/src/tokotime.egg-info/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)     1139 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/SOURCES.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 05:14:14.000000 tokotime-0.13/src/tokotime.egg-info/dependency_links.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      146 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/requires.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)       18 2023-08-06 05:14:15.000000 tokotime-0.13/src/tokotime.egg-info/top_level.txt
```

### Comparing `tokotime-0.12/LICENSE.txt` & `tokotime-0.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/PKG-INFO` & `tokotime-0.13/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.12
+Version: 0.13
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_013.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tokotime-0.12/setup.py` & `tokotime-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from distutils.core import setup
 setup(
   name = 'tokotime',         # How you named your package folder (MyLib)
-  version = '0.12',      # Start with a small number and increase it with every change you make
+  version = '0.13',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "Tokopedia Data Science Forecasting Reusable Package",   # Give a short description about your library
   author = 'Alan Choon',                   # Type in your name
   author_email = 'alan.yu@tokopedia.com',      # Type in your E-Mail
   url = 'https://github.com/tokopedia/forecasting-platform-utils',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz',
+  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_013.tar.gz',
   keywords = ['Forecasting', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
         'darts',
         'lightgbm',
         'mpire',
         'numpy',
         'optuna',
@@ -25,15 +25,15 @@
         'scikit_lego',
         'sklego',
         'sktime',
         'statsmodels',
         'threadpoolctl',
         'tqdm',
       ],
-  package_dir={"": "tokotime"}, 
+  package_dir={"": "src"}, 
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.7',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.8',
```

### Comparing `tokotime-0.12/tokotime/data_utils/utils.py` & `tokotime-0.13/src/tokotime/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/experiment_design/random_sampler.py` & `tokotime-0.13/src/tokotime/experiment_design/random_sampler.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/features_eng/base_eng.py` & `tokotime-0.13/src/tokotime/features_eng/base_eng.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/hp_tune/bayes_hp_tuner.py` & `tokotime-0.13/src/tokotime/hp_tune/bayes_hp_tuner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/evaluation_metrics.py` & `tokotime-0.13/src/tokotime/point_forecasts/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/model_mapping.py` & `tokotime-0.13/src/tokotime/point_forecasts/model_mapping.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/model_runner.py` & `tokotime-0.13/src/tokotime/point_forecasts/model_runner.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/model_wrappers.py` & `tokotime-0.13/src/tokotime/point_forecasts/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/ts_class.py` & `tokotime-0.13/src/tokotime/point_forecasts/ts_class.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/point_forecasts/validation.py` & `tokotime-0.13/src/tokotime/point_forecasts/validation.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/preprocess_utils/preprocess_components.py` & `tokotime-0.13/src/tokotime/preprocess_utils/preprocess_components.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/preprocess_utils/preprocessors.py` & `tokotime-0.13/src/tokotime/preprocess_utils/preprocessors.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/probabilistic_forecasts/evaluation_metrics.py` & `tokotime-0.13/src/tokotime/probabilistic_forecasts/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `tokotime-0.12/tokotime/tokotime.egg-info/PKG-INFO` & `tokotime-0.13/src/tokotime.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.12
+Version: 0.13
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_013.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tokotime-0.12/tokotime/tokotime.egg-info/SOURCES.txt` & `tokotime-0.13/src/tokotime.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
-tokotime/__init__.py
-tokotime/data_utils/__init__.py
-tokotime/data_utils/utils.py
-tokotime/experiment_design/__init__.py
-tokotime/experiment_design/random_sampler.py
-tokotime/features_eng/__init__.py
-tokotime/features_eng/base_eng.py
-tokotime/hp_tune/bayes_hp_tuner.py
-tokotime/point_forecasts/__init__.py
-tokotime/point_forecasts/evaluation_metrics.py
-tokotime/point_forecasts/misc.py
-tokotime/point_forecasts/model_mapping.py
-tokotime/point_forecasts/model_runner.py
-tokotime/point_forecasts/model_wrappers.py
-tokotime/point_forecasts/ts_class.py
-tokotime/point_forecasts/validation.py
-tokotime/preprocess_utils/__init__.py
-tokotime/preprocess_utils/preprocess_components.py
-tokotime/preprocess_utils/preprocessors.py
-tokotime/probabilistic_forecasts/__init__.py
-tokotime/probabilistic_forecasts/evaluation_metrics.py
-tokotime/tokotime.egg-info/PKG-INFO
-tokotime/tokotime.egg-info/SOURCES.txt
-tokotime/tokotime.egg-info/dependency_links.txt
-tokotime/tokotime.egg-info/requires.txt
-tokotime/tokotime.egg-info/top_level.txt
+src/__init__.py
+src/tokotime/__init__.py
+src/tokotime.egg-info/PKG-INFO
+src/tokotime.egg-info/SOURCES.txt
+src/tokotime.egg-info/dependency_links.txt
+src/tokotime.egg-info/requires.txt
+src/tokotime.egg-info/top_level.txt
+src/tokotime/data_utils/__init__.py
+src/tokotime/data_utils/utils.py
+src/tokotime/experiment_design/__init__.py
+src/tokotime/experiment_design/random_sampler.py
+src/tokotime/features_eng/__init__.py
+src/tokotime/features_eng/base_eng.py
+src/tokotime/hp_tune/bayes_hp_tuner.py
+src/tokotime/point_forecasts/__init__.py
+src/tokotime/point_forecasts/evaluation_metrics.py
+src/tokotime/point_forecasts/misc.py
+src/tokotime/point_forecasts/model_mapping.py
+src/tokotime/point_forecasts/model_runner.py
+src/tokotime/point_forecasts/model_wrappers.py
+src/tokotime/point_forecasts/ts_class.py
+src/tokotime/point_forecasts/validation.py
+src/tokotime/preprocess_utils/__init__.py
+src/tokotime/preprocess_utils/preprocess_components.py
+src/tokotime/preprocess_utils/preprocessors.py
+src/tokotime/probabilistic_forecasts/__init__.py
+src/tokotime/probabilistic_forecasts/evaluation_metrics.py
```

