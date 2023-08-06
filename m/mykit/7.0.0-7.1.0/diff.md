# Comparing `tmp/mykit-7.0.0.tar.gz` & `tmp/mykit-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-a21w3_xm/mykit-7.0.0.tar", last modified: Sun Aug  6 08:35:42 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-k5dm1twx/mykit-7.1.0.tar", last modified: Sun Aug  6 15:09:40 2023, max compression
```

## Comparing `mykit-7.0.0.tar` & `mykit-7.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-06 08:35:35.000000 mykit-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 08:35:42.000000 mykit-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-06 08:35:35.000000 mykit-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/pLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/rec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/rec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:35.000000 mykit-7.0.0/mykit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 08:35:42.000000 mykit-7.0.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-06 08:35:36.000000 mykit-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-06 08:35:42.000000 mykit-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 08:35:35.000000 mykit-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-06 15:09:33.000000 mykit-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 15:09:40.000000 mykit-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-06 15:09:33.000000 mykit-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/pLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:33.000000 mykit-7.1.0/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 15:09:40.000000 mykit-7.1.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-06 15:09:34.000000 mykit-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-06 15:09:40.000000 mykit-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 15:09:33.000000 mykit-7.1.0/setup.py
```

### Comparing `mykit-7.0.0/LICENSE` & `mykit-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/PKG-INFO` & `mykit-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 7.0.0
+Version: 7.1.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-7.0.0/README.md` & `mykit-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/__init__.py` & `mykit-7.1.0/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/__main__.py` & `mykit-7.1.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/__init__.py` & `mykit-7.1.0/mykit/app/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/architecture/eventdriven.py` & `mykit-7.1.0/mykit/app/architecture/eventdriven.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/arrow.py` & `mykit-7.1.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/button.py` & `mykit-7.1.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/complex/biplot.py` & `mykit-7.1.0/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/complex/plot.py` & `mykit-7.1.0/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/label.py` & `mykit-7.1.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/app/slider.py` & `mykit-7.1.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/color.py` & `mykit-7.1.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-7.1.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/ffmpeg.py` & `mykit-7.1.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/keycrate/__init__.py` & `mykit-7.1.0/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/math.py` & `mykit-7.1.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/neuralnet/dense.py` & `mykit-7.1.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/neuralnet/genetic.py` & `mykit-7.1.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/noise.py` & `mykit-7.1.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/pLog.py` & `mykit-7.1.0/mykit/kit/pLog.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/path.py` & `mykit-7.1.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/text.py` & `mykit-7.1.0/mykit/kit/text.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/time.py` & `mykit-7.1.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/mykit/kit/utils.py` & `mykit-7.1.0/mykit/kit/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime as _datetime
 import keyword as _keyword
 import os as _os
 import random as _random
 import time as _time
 from typing import (
+    Dict as _Dict,
+    Hashable as _Hashable,
     Tuple as _Tuple
 )
 
 
 def randfloat(__low: float, __high: float, __prec: int = 2, /) -> float:
     """
     This function follows `random.uniform` behaviors.
@@ -240,8 +242,34 @@
     >>> reverse_dict({5: '', 1: '', 9: ''})  # {9: '', 1: '', 5: ''}
     """
     keys = list(input_dict.keys())
     keys.reverse()
     return {
         k: input_dict[k]
         for k in keys
-    }
+    }
+
+
+def merge_dicts(
+    dict1:_Dict[_Hashable, float],
+    dict2:_Dict[_Hashable, float],
+    /
+) -> _Dict[_Hashable, float]:
+    """
+    Merge two dictionaries.
+
+    ---
+
+    ## Demo
+    >>> dict1 = {'a': 1, 'b': 2}
+    >>> dict2 = {'b': 3, 'c': 4}
+    >>> merged_dict = merge_dicts(dict1, dict2)
+    >>> # merged_dict is {'a': 1, 'b': 5, 'c': 4}
+    """
+
+    for key, value in dict2.items():
+        if key in dict1:
+            dict1[key] += value
+        else:
+            dict1[key] = value
+
+    return dict1
```

### Comparing `mykit-7.0.0/mykit.egg-info/PKG-INFO` & `mykit-7.1.0/mykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 7.0.0
+Version: 7.1.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/mykit/docs
 Project-URL: Report bugs, https://github.com/nvfp/mykit/issues
```

### Comparing `mykit-7.0.0/mykit.egg-info/SOURCES.txt` & `mykit-7.1.0/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-7.0.0/pyproject.toml` & `mykit-7.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "7.0.0"
+version = "7.1.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

