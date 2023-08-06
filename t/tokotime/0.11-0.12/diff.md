# Comparing `tmp/tokotime-0.11.tar.gz` & `tmp/tokotime-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokotime-0.11.tar", last modified: Sun Aug  6 04:24:27 2023, max compression
+gzip compressed data, was "tokotime-0.12.tar", last modified: Sun Aug  6 05:06:30 2023, max compression
```

## Comparing `tokotime-0.11.tar` & `tokotime-0.12.tar`

### file list

```diff
@@ -1,14 +1,41 @@
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 04:24:27.596266 tokotime-0.11/
--rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.11/LICENSE.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 04:24:27.596365 tokotime-0.11/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.11/README.md
--rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 04:24:27.596717 tokotime-0.11/setup.cfg
--rw-r--r--   0 alanchn    (501) staff       (20)     1932 2023-08-06 04:23:44.000000 tokotime-0.11/setup.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 04:24:27.594249 tokotime-0.11/tokotime/
--rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.11/tokotime/__init__.py
-drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 04:24:27.596037 tokotime-0.11/tokotime.egg-info/
--rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 04:24:27.000000 tokotime-0.11/tokotime.egg-info/PKG-INFO
--rw-r--r--   0 alanchn    (501) staff       (20)      220 2023-08-06 04:24:27.000000 tokotime-0.11/tokotime.egg-info/SOURCES.txt
--rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 04:24:27.000000 tokotime-0.11/tokotime.egg-info/dependency_links.txt
--rw-r--r--   0 alanchn    (501) staff       (20)      146 2023-08-06 04:24:27.000000 tokotime-0.11/tokotime.egg-info/requires.txt
--rw-r--r--   0 alanchn    (501) staff       (20)        9 2023-08-06 04:24:27.000000 tokotime-0.11/tokotime.egg-info/top_level.txt
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.007334 tokotime-0.12/
+-rw-r--r--   0 alanchn    (501) staff       (20)     1061 2023-08-06 04:21:07.000000 tokotime-0.12/LICENSE.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:06:30.007448 tokotime-0.12/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)       39 2023-08-06 04:21:07.000000 tokotime-0.12/README.md
+-rw-r--r--   0 alanchn    (501) staff       (20)       38 2023-08-06 05:06:30.007843 tokotime-0.12/setup.cfg
+-rw-r--r--   0 alanchn    (501) staff       (20)     1909 2023-08-06 05:06:16.000000 tokotime-0.12/setup.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.998314 tokotime-0.12/tokotime/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/__init__.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.998900 tokotime-0.12/tokotime/data_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/data_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     1259 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/data_utils/utils.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:29.999678 tokotime-0.12/tokotime/experiment_design/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/experiment_design/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6749 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/experiment_design/random_sampler.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.000468 tokotime-0.12/tokotime/features_eng/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/features_eng/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     4883 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/features_eng/base_eng.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.000881 tokotime-0.12/tokotime/hp_tune/
+-rw-r--r--   0 alanchn    (501) staff       (20)     3047 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/hp_tune/bayes_hp_tuner.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.003984 tokotime-0.12/tokotime/point_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9853 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/evaluation_metrics.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      379 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/misc.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2602 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_mapping.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     9694 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_runner.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    13632 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/model_wrappers.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2378 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/ts_class.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     2145 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/point_forecasts/validation.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.004876 tokotime-0.12/tokotime/preprocess_utils/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)    35834 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/preprocess_components.py
+-rw-r--r--   0 alanchn    (501) staff       (20)     6911 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/preprocess_utils/preprocessors.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.005399 tokotime-0.12/tokotime/probabilistic_forecasts/
+-rw-r--r--   0 alanchn    (501) staff       (20)        0 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/probabilistic_forecasts/__init__.py
+-rw-r--r--   0 alanchn    (501) staff       (20)      718 2023-08-06 04:21:07.000000 tokotime-0.12/tokotime/probabilistic_forecasts/evaluation_metrics.py
+drwxr-xr-x   0 alanchn    (501) staff       (20)        0 2023-08-06 05:06:30.007053 tokotime-0.12/tokotime/tokotime.egg-info/
+-rw-r--r--   0 alanchn    (501) staff       (20)      787 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/PKG-INFO
+-rw-r--r--   0 alanchn    (501) staff       (20)     1064 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/SOURCES.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)        1 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/dependency_links.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      146 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/requires.txt
+-rw-r--r--   0 alanchn    (501) staff       (20)      116 2023-08-06 05:06:29.000000 tokotime-0.12/tokotime/tokotime.egg-info/top_level.txt
```

### Comparing `tokotime-0.11/LICENSE.txt` & `tokotime-0.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokotime-0.11/PKG-INFO` & `tokotime-0.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.11
+Version: 0.12
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_011.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tokotime-0.11/setup.py` & `tokotime-0.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 from distutils.core import setup
 setup(
   name = 'tokotime',         # How you named your package folder (MyLib)
-  packages = ['tokotime'],   # Chose the same as "name"
-  version = '0.11',      # Start with a small number and increase it with every change you make
+  version = '0.12',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "Tokopedia Data Science Forecasting Reusable Package",   # Give a short description about your library
   author = 'Alan Choon',                   # Type in your name
   author_email = 'alan.yu@tokopedia.com',      # Type in your E-Mail
   url = 'https://github.com/tokopedia/forecasting-platform-utils',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_011.tar.gz',
+  download_url = 'https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz',
   keywords = ['Forecasting', 'Machine Learning'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
         'darts',
         'lightgbm',
         'mpire',
         'numpy',
         'optuna',
@@ -26,14 +25,15 @@
         'scikit_lego',
         'sklego',
         'sktime',
         'statsmodels',
         'threadpoolctl',
         'tqdm',
       ],
+  package_dir={"": "tokotime"}, 
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.7',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.8',
```

### Comparing `tokotime-0.11/tokotime.egg-info/PKG-INFO` & `tokotime-0.12/tokotime/tokotime.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tokotime
-Version: 0.11
+Version: 0.12
 Summary: Tokopedia Data Science Forecasting Reusable Package
 Home-page: https://github.com/tokopedia/forecasting-platform-utils
-Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_011.tar.gz
+Download-URL: https://github.com/tokopedia/forecasting-platform-utils/archive/refs/tags/v_012.tar.gz
 Author: Alan Choon
 Author-email: alan.yu@tokopedia.com
 License: MIT
 Keywords: Forecasting,Machine Learning
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

