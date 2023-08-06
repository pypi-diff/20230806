# Comparing `tmp/matplotlib-cern-0.1.0.tar.gz` & `tmp/matplotlib-cern-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib-cern-0.1.0.tar", last modified: Sun Aug  6 09:38:58 2023, max compression
+gzip compressed data, was "matplotlib-cern-0.1.1.tar", last modified: Sun Aug  6 09:57:25 2023, max compression
```

## Comparing `matplotlib-cern-0.1.0.tar` & `matplotlib-cern-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:38:58.501852 matplotlib-cern-0.1.0/
--rw-rw-r--   0 george    (1000) george    (1000)    35149 2023-08-04 09:21:26.000000 matplotlib-cern-0.1.0/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      225 2023-08-06 09:38:58.501852 matplotlib-cern-0.1.0/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      283 2023-08-04 10:18:08.000000 matplotlib-cern-0.1.0/README.md
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:38:58.497851 matplotlib-cern-0.1.0/matplotlib_cern/
--rw-rw-r--   0 george    (1000) george    (1000)     1750 2023-08-06 09:34:31.000000 matplotlib-cern-0.1.0/matplotlib_cern/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     2809 2023-08-06 09:28:40.000000 matplotlib-cern-0.1.0/matplotlib_cern/template.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:38:58.501852 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)      225 2023-08-06 09:38:58.000000 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      276 2023-08-06 09:38:58.000000 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-08-06 09:38:58.000000 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       11 2023-08-06 09:38:58.000000 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       16 2023-08-06 09:38:58.000000 matplotlib-cern-0.1.0/matplotlib_cern.egg-info/top_level.txt
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-08-06 09:38:58.501852 matplotlib-cern-0.1.0/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)      290 2023-08-06 09:38:53.000000 matplotlib-cern-0.1.0/setup.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:57:25.773306 matplotlib-cern-0.1.1/
+-rw-rw-r--   0 george    (1000) george    (1000)    35149 2023-08-04 09:21:26.000000 matplotlib-cern-0.1.1/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      225 2023-08-06 09:57:25.773306 matplotlib-cern-0.1.1/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      283 2023-08-04 10:18:08.000000 matplotlib-cern-0.1.1/README.md
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:57:25.773306 matplotlib-cern-0.1.1/matplotlib_cern/
+-rw-rw-r--   0 george    (1000) george    (1000)     1733 2023-08-06 09:54:58.000000 matplotlib-cern-0.1.1/matplotlib_cern/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2791 2023-08-06 09:54:20.000000 matplotlib-cern-0.1.1/matplotlib_cern/template.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-08-06 09:57:25.773306 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)      225 2023-08-06 09:57:25.000000 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      276 2023-08-06 09:57:25.000000 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-08-06 09:57:25.000000 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       11 2023-08-06 09:57:25.000000 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       16 2023-08-06 09:57:25.000000 matplotlib-cern-0.1.1/matplotlib_cern.egg-info/top_level.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-08-06 09:57:25.773306 matplotlib-cern-0.1.1/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)      290 2023-08-06 09:55:54.000000 matplotlib-cern-0.1.1/setup.py
```

### Comparing `matplotlib-cern-0.1.0/LICENSE` & `matplotlib-cern-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib-cern-0.1.0/matplotlib_cern/__init__.py` & `matplotlib-cern-0.1.1/matplotlib_cern/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # matplotlibcern/__init__.py
 
 import matplotlib.pyplot as plt
 
 def set_matplotlib_cern():
     # Fonts
     plt.rcParams["text.usetex"] = True
+    plt.rcParams["text.latex.preamble"] = r"\usepackage{amsmath} \usepackage{amssymb}"
     plt.rcParams["font.size"] = 20
-    plt.rcParams["font.family"] = "serif"
-    plt.rcParams["font.serif"] = "STIXGeneral"
-    plt.rcParams["mathtext.fontset"] = "stix"
-    plt.rcParams["text.latex.preamble"] = r"\usepackage{amsmath} \usepackage{amssymb} \usepackage{sfmath}"
+    plt.rcParams["font.family"] =  "serif"
+    plt.rcParams["font.serif"] =  "STIXGeneral"
+    plt.rcParams["mathtext.fontset"] =  "stix"
 
     # Figure
     plt.rcParams["figure.figsize"] = (8, 8)
     plt.rcParams["savefig.bbox"] = "tight"
 
     # Points, Errorbars, Scatter and Lines
     plt.rcParams["errorbar.capsize"] = 3.0
```

### Comparing `matplotlib-cern-0.1.0/matplotlib_cern/template.py` & `matplotlib-cern-0.1.1/matplotlib_cern/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 from scipy.optimize import curve_fit
 
 # Fonts
 plt.rcParams["text.usetex"] = True
+plt.rcParams["text.latex.preamble"] = r"\usepackage{amsmath} \usepackage{amssymb}"
 plt.rcParams["font.size"] = 20
 plt.rcParams["font.family"] =  "serif"
 plt.rcParams["font.serif"] =  "STIXGeneral"
 plt.rcParams["mathtext.fontset"] =  "stix"
-plt.rcParams["text.latex.preamble"] = r"\usepackage{amsmath} \usepackage{amssymb} \usepackage{sfmath}"
+
 
 
 # Figure
 plt.rcParams["figure.figsize"] = (8, 8)
 plt.rcParams["savefig.bbox"] = "tight"
 
 # Points, Errorbars, Scatter and Lines
@@ -36,14 +37,15 @@
 plt.rcParams["ytick.major.left"] = True
 plt.rcParams["ytick.major.right"] = True
 plt.rcParams["ytick.minor.visible"] = True
 plt.rcParams["ytick.direction"] = "in"
 plt.rcParams["ytick.major.size"] = 8.0
 plt.rcParams["ytick.minor.size"] = 5.0
 
+
 # Axes
 plt.rcParams["xaxis.labellocation"] = "right"
 plt.rcParams["yaxis.labellocation"] = "top"
 
 # Legend
 plt.rcParams["legend.fontsize"] = 20
 plt.rcParams["legend.frameon"] = False
```

