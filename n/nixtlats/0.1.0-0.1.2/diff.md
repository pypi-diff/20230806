# Comparing `tmp/nixtlats-0.1.0.tar.gz` & `tmp/nixtlats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtlats-0.1.0.tar", last modified: Sat Aug  5 08:32:24 2023, max compression
+gzip compressed data, was "nixtlats-0.1.2.tar", last modified: Sun Aug  6 17:28:32 2023, max compression
```

## Comparing `nixtlats-0.1.0.tar` & `nixtlats-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.552172 nixtlats-0.1.0/
--rw-r--r--   0 fedex      (501) staff       (20)     1155 2023-08-05 06:39:47.000000 nixtlats-0.1.0/LICENSE
--rw-r--r--   0 fedex      (501) staff       (20)     3457 2023-08-05 08:32:24.552020 nixtlats-0.1.0/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)     3108 2023-08-05 06:39:47.000000 nixtlats-0.1.0/README.md
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.551029 nixtlats-0.1.0/nixtlats/
--rw-r--r--   0 fedex      (501) staff       (20)       73 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/__init__.py
--rw-r--r--   0 fedex      (501) staff       (20)     1596 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/_modidx.py
--rw-r--r--   0 fedex      (501) staff       (20)     5339 2023-08-05 08:21:15.000000 nixtlats-0.1.0/nixtlats/timegpt.py
-drwxr-xr-x   0 fedex      (501) staff       (20)        0 2023-08-05 08:32:24.551840 nixtlats-0.1.0/nixtlats.egg-info/
--rw-r--r--   0 fedex      (501) staff       (20)     3457 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/PKG-INFO
--rw-r--r--   0 fedex      (501) staff       (20)      215 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/SOURCES.txt
--rw-r--r--   0 fedex      (501) staff       (20)        1 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/dependency_links.txt
--rw-r--r--   0 fedex      (501) staff       (20)        9 2023-08-05 08:32:24.000000 nixtlats-0.1.0/nixtlats.egg-info/top_level.txt
--rw-r--r--   0 fedex      (501) staff       (20)       38 2023-08-05 08:32:24.552216 nixtlats-0.1.0/setup.cfg
--rw-r--r--   0 fedex      (501) staff       (20)      552 2023-08-05 08:32:18.000000 nixtlats-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:28:32.861900 nixtlats-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-06 17:28:19.000000 nixtlats-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-06 17:28:32.861900 nixtlats-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-06 17:28:19.000000 nixtlats-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:28:32.861900 nixtlats-0.1.2/nixtlats/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-06 17:28:19.000000 nixtlats-0.1.2/nixtlats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-06 17:28:19.000000 nixtlats-0.1.2/nixtlats/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-06 17:28:19.000000 nixtlats-0.1.2/nixtlats/timegpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:28:32.861900 nixtlats-0.1.2/nixtlats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-06 17:28:32.000000 nixtlats-0.1.2/nixtlats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-06 17:28:32.000000 nixtlats-0.1.2/nixtlats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:28:32.000000 nixtlats-0.1.2/nixtlats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 17:28:32.000000 nixtlats-0.1.2/nixtlats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 17:28:32.000000 nixtlats-0.1.2/nixtlats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:28:32.861900 nixtlats-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-06 17:28:19.000000 nixtlats-0.1.2/setup.py
```

### Comparing `nixtlats-0.1.0/LICENSE` & `nixtlats-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtlats-0.1.0/PKG-INFO` & `nixtlats-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.1.0
+Version: 0.1.2
 Summary: Nixtla SDK
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">NixtlaTS</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
-[![CI](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml)
+[![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
 [![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
-[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtlats.svg?label=docs)](https://nixtla.github.io/nixtlats/)
+[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
 [![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
     
 **NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 Certainly, adding a bit of personality and visual appeal can make your README stand out. Here's a reworked version:
 
@@ -46,21 +47,21 @@
 With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `NixtlaTS` up and running with a simple pip command:
 
 ```python
-pip install nixtlats
+pip install nixtlats>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 from nixtlats import TimeGPT
-timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'], api_url=os.environ['TIMEGPT_API_URL'])
+timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'])
 fcst_df = timegpt.forecast(df, h=24, freq='H', level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.1.0/README.md` & `nixtlats-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">NixtlaTS</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
-[![CI](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml)
+[![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
 [![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
-[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtlats.svg?label=docs)](https://nixtla.github.io/nixtlats/)
+[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
 [![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
     
 **NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 Certainly, adding a bit of personality and visual appeal can make your README stand out. Here's a reworked version:
 
@@ -34,21 +34,21 @@
 With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `NixtlaTS` up and running with a simple pip command:
 
 ```python
-pip install nixtlats
+pip install nixtlats>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 from nixtlats import TimeGPT
-timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'], api_url=os.environ['TIMEGPT_API_URL'])
+timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'])
 fcst_df = timegpt.forecast(df, h=24, freq='H', level=[80, 90])
 ```
 
-![](./nbs/img/forecast_readme.png)
+![](./nbs/img/forecast_readme.png)
```

### Comparing `nixtlats-0.1.0/nixtlats/_modidx.py` & `nixtlats-0.1.2/nixtlats/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/nixtlats/',
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/nixtla/',
                 'lib_path': 'nixtlats'},
   'syms': { 'nixtlats.timegpt': { 'nixtlats.timegpt.TimeGPT': ('timegpt.html#timegpt', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.__init__': ('timegpt.html#timegpt.__init__', 'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._infer_freq': ('timegpt.html#timegpt._infer_freq', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._input_size': ('timegpt.html#timegpt._input_size', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._multi_series': ('timegpt.html#timegpt._multi_series', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._parse_response': ( 'timegpt.html#timegpt._parse_response',
                                                                                 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT._preprocess_inputs': ( 'timegpt.html#timegpt._preprocess_inputs',
                                                                                    'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._validate_inputs': ( 'timegpt.html#timegpt._validate_inputs',
+                                                                                 'nixtlats/timegpt.py'),
+                                  'nixtlats.timegpt.TimeGPT._validate_outputs': ( 'timegpt.html#timegpt._validate_outputs',
+                                                                                  'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.forecast': ('timegpt.html#timegpt.forecast', 'nixtlats/timegpt.py'),
                                   'nixtlats.timegpt.TimeGPT.request_headers': ( 'timegpt.html#timegpt.request_headers',
                                                                                 'nixtlats/timegpt.py')}}}
```

### Comparing `nixtlats-0.1.0/nixtlats.egg-info/PKG-INFO` & `nixtlats-0.1.2/nixtlats.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: nixtlats
-Version: 0.1.0
+Version: 0.1.2
 Summary: Nixtla SDK
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Nixtla &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Statistical%20Forecasting%20Algorithms%20by%20Nixtla%20&url=https://github.com/Nixtla/statsforecast&via=nixtlainc&hashtags=StatisticalModels,TimeSeries,Forecasting) &nbsp;[![Slack](https://img.shields.io/badge/Slack-4A154B?&logo=slack&logoColor=white)](https://join.slack.com/t/nixtlacommunity/shared_invite/zt-1pmhan9j5-F54XR20edHk0UtYAPcW4KQ)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/Nixtla/neuralforecast/main/nbs/imgs_indx/logo_mid.png">
 <h1 align="center">NixtlaTS</h1>
 <h3 align="center">Forecast using TimeGPT</h3>
     
-[![CI](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtlats/actions/workflows/ci.yaml)
+[![CI](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/Nixtla/nixtla/actions/workflows/ci.yaml)
 [![Python](https://img.shields.io/pypi/pyversions/nixtlats)](https://pypi.org/project/nixtlats/)
 [![PyPi](https://img.shields.io/pypi/v/nixtlats?color=blue)](https://pypi.org/project/nixtlats/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Nixtla/nixtlats/blob/main/LICENSE)
-[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtlats.svg?label=docs)](https://nixtla.github.io/nixtlats/)
+[![docs](https://img.shields.io/website-up-down-green-red/http/nixtla.github.io/nixtla.svg?label=docs)](https://nixtla.github.io/nixtla/)
 [![Downloads](https://pepy.tech/badge/nixtlats)](https://pepy.tech/project/nixtlats)
     
 **NixtlaTS** offers a collection of classes and methods to interact with the API of TimeGPT.
 </div>
 
 Certainly, adding a bit of personality and visual appeal can make your README stand out. Here's a reworked version:
 
@@ -46,21 +47,21 @@
 With `NixtlaTS`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `NixtlaTS` up and running with a simple pip command:
 
 ```python
-pip install nixtlats
+pip install nixtlats>=0.1.0
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
 from nixtlats import TimeGPT
-timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'], api_url=os.environ['TIMEGPT_API_URL'])
+timegpt = TimeGPT(token=os.environ['TIMEGPT_TOKEN'])
 fcst_df = timegpt.forecast(df, h=24, freq='H', level=[80, 90])
 ```
 
 ![](./nbs/img/forecast_readme.png)
```

