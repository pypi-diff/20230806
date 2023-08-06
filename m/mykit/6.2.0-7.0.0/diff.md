# Comparing `tmp/mykit-6.2.0.tar.gz` & `tmp/mykit-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-ilfcgbdx/mykit-6.2.0.tar", last modified: Wed Aug  2 13:42:27 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-a21w3_xm/mykit-7.0.0.tar", last modified: Sun Aug  6 08:35:42 2023, max compression
```

## Comparing `mykit-6.2.0.tar` & `mykit-7.0.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 13:42:20.000000 mykit-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 13:42:27.000000 mykit-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 13:42:20.000000 mykit-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/pLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/rec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/rec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:20.000000 mykit-6.2.0/mykit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 13:42:27.000000 mykit-6.2.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 13:42:21.000000 mykit-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-02 13:42:27.000000 mykit-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 13:42:20.000000 mykit-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-06 08:35:35.000000 mykit-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 08:35:42.000000 mykit-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-06 08:35:35.000000 mykit-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/pLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-06 08:35:36.000000 mykit-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-06 08:35:42.000000 mykit-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 08:35:35.000000 mykit-7.0.0/setup.py
```

### Comparing `mykit-6.2.0/LICENSE` & `mykit-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/PKG-INFO` & `mykit-7.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 6.2.0
+Version: 7.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
@@ -16,30 +16,27 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- make the status easily visible -->
-[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
-
-
 # myKit
 
+[![Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- Use this link (don't use the relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
-[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
-[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
-
 
 ## Installation
 
 ```sh
 pip install mykit
 ```
 
@@ -57,15 +54,15 @@
 ```
 
 
 ## Links
 
 - [Documentation](https://nvfp.github.io/mykit)
 - [Demo](https://nvfp.github.io/mykit/demo)
-- [Supports💙](https://nvfp.github.io/mykit/supports)
+- [Supports💙](https://nvfp.github.io/many-thanks)
 - [Changelog](https://nvfp.github.io/mykit/changelog)
 - [FAQs](https://nvfp.github.io/mykit/faqs)
 
 
 ## Troubleshoot
 
 - To report bugs or ask questions, please open an issue or submit a pull request.
```

### Comparing `mykit-6.2.0/README.md` & `mykit-7.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-<!-- make the status easily visible -->
-[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
-
-
 # myKit
 
+[![Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- Use this link (don't use the relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
-[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
-[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
-
 
 ## Installation
 
 ```sh
 pip install mykit
 ```
 
@@ -35,15 +32,15 @@
 ```
 
 
 ## Links
 
 - [Documentation](https://nvfp.github.io/mykit)
 - [Demo](https://nvfp.github.io/mykit/demo)
-- [Supports💙](https://nvfp.github.io/mykit/supports)
+- [Supports💙](https://nvfp.github.io/many-thanks)
 - [Changelog](https://nvfp.github.io/mykit/changelog)
 - [FAQs](https://nvfp.github.io/mykit/faqs)
 
 
 ## Troubleshoot
 
 - To report bugs or ask questions, please open an issue or submit a pull request.
```

### Comparing `mykit-6.2.0/mykit/__init__.py` & `mykit-7.0.0/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/__main__.py` & `mykit-7.0.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/__init__.py` & `mykit-7.0.0/mykit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/architecture/eventdriven.py` & `mykit-7.0.0/mykit/app/architecture/eventdriven.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/arrow.py` & `mykit-7.0.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/button.py` & `mykit-7.0.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/complex/biplot.py` & `mykit-7.0.0/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/complex/plot.py` & `mykit-7.0.0/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/label.py` & `mykit-7.0.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/app/slider.py` & `mykit-7.0.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/color.py` & `mykit-7.0.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-7.0.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/ffmpeg.py` & `mykit-7.0.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/keycrate/__init__.py` & `mykit-7.0.0/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/math.py` & `mykit-7.0.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/neuralnet/dense.py` & `mykit-7.0.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/neuralnet/genetic.py` & `mykit-7.0.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/noise.py` & `mykit-7.0.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/pLog.py` & `mykit-7.0.0/mykit/kit/pLog.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/path.py` & `mykit-7.0.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit/kit/text.py` & `mykit-7.0.0/mykit/kit/text.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 
 def in_byte(bytes: int, /, precision: int = 2, gap: int = 1) -> str:
     """
     ## Params
     - `precision`: rounding precision
     - `gap`: gap (in spaces) between the number and the unit
 
+    ## Demo
+    >>> in_byte(100)  # 100 B
+    >>> in_byte(1300)  # 1.27 KiB
+    >>> in_byte(1300, 0, 0)  # 1KiB
+    >>> in_byte(1700, 0, 0)  # 2KiB
+
     ## Docs
     - `in_byte` is the extended version of `mykit.kit.text.byteFmt`
     """
 
     GAP = ' '*gap
 
     ## Handle 0 `bytes`
@@ -96,23 +102,31 @@
         'GiB', 'TiB', 'PiB',
         'EiB', 'ZiB', 'YiB',
     ]
 
     return sign + connum(number) + GAP + UNIT[power]
 
 
-def num_approx(num, /, precision:int=1, gap:int=1) -> str:
+def num_approx(num, /, precision:int=1, gap:int=0) -> str:
     """
     Round a number down to K (thousand), M (million), B (billion), etc.
 
     ---
 
     ## Params
     - `precision`: rounding precision
     - `gap`: gap (in spaces) between the number and the unit
+
+    ## Demo
+    >>> num_approx(999)  # 999
+    >>> num_approx(1000)  # 1K
+    >>> num_approx(1001)  # 1K
+    >>> num_approx(1_250_000)  # 1.2M
+    >>> num_approx(1_250_000, 0, 1)  # 1 M
+    >>> num_approx(1_750_000, 0, 1)  # 2 M
     """
 
     suffixes = [
         (1e3, ''),
         (1e6, 'K'),
         (1e9, 'M'),
         (1e12, 'B'),
```

### Comparing `mykit-6.2.0/mykit/kit/time.py` & `mykit-7.0.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/mykit.egg-info/PKG-INFO` & `mykit-7.0.0/mykit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 6.2.0
+Version: 7.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
@@ -16,30 +16,27 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- make the status easily visible -->
-[![🧩Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
-
-
 # myKit
 
+[![Run tests](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml/badge.svg)](https://github.com/nvfp/mykit/actions/workflows/run-tests.yml)
+[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+
 Python utility toolkit.
 
 The aim of this project is to understand how things work by building them from the ground up, while also providing a lightweight version of something that already exists out there.
 
 <!-- Use this link (don't use the relative path to the one in the repo) to be able to display the banner on PyPI -->
 ![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230619-mykit-banner-360p.png)
 
-[![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
-[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
-
 
 ## Installation
 
 ```sh
 pip install mykit
 ```
 
@@ -57,15 +54,15 @@
 ```
 
 
 ## Links
 
 - [Documentation](https://nvfp.github.io/mykit)
 - [Demo](https://nvfp.github.io/mykit/demo)
-- [Supports💙](https://nvfp.github.io/mykit/supports)
+- [Supports💙](https://nvfp.github.io/many-thanks)
 - [Changelog](https://nvfp.github.io/mykit/changelog)
 - [FAQs](https://nvfp.github.io/mykit/faqs)
 
 
 ## Troubleshoot
 
 - To report bugs or ask questions, please open an issue or submit a pull request.
```

### Comparing `mykit-6.2.0/mykit.egg-info/SOURCES.txt` & `mykit-7.0.0/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-6.2.0/pyproject.toml` & `mykit-7.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "6.2.0"
+version = "7.0.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

