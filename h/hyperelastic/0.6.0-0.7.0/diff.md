# Comparing `tmp/hyperelastic-0.6.0.tar.gz` & `tmp/hyperelastic-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.6.0.tar", last modified: Fri Aug  4 12:36:05 2023, max compression
+gzip compressed data, was "hyperelastic-0.7.0.tar", last modified: Sun Aug  6 20:46:57 2023, max compression
```

## Comparing `hyperelastic-0.6.0.tar` & `hyperelastic-0.7.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.994768 hyperelastic-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/lab/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_curve_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_load_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27544 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/generalized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/generalized/_stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/_generalized_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:46:57.809732 hyperelastic-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_curve_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_load_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/lab/_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27718 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/generalized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/generalized/_stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/_generalized_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.801732 hyperelastic-0.7.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 20:46:57.000000 hyperelastic-0.7.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:46:57.805732 hyperelastic-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_lab_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-06 20:46:49.000000 hyperelastic-0.7.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.6.0/LICENSE` & `hyperelastic-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/PKG-INFO` & `hyperelastic-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.6.0
+Version: 0.7.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.6.0/README.md` & `hyperelastic-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/pyproject.toml` & `hyperelastic-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/__init__.py` & `hyperelastic-0.7.0/src/hyperelastic/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/frameworks/_generalized.py` & `hyperelastic-0.7.0/src/hyperelastic/frameworks/_generalized.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.7.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.7.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/lab/_curve_fit.py` & `hyperelastic-0.7.0/src/hyperelastic/lab/_curve_fit.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/lab/_plotting.py` & `hyperelastic-0.7.0/src/hyperelastic/lab/_plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,58 @@
 import matplotlib.pyplot as plt
 
 
 class LabPlotter:
     "Class with methods for generating plots of experiments and simulations."
 
+    def __init__(self):
+        self.label = None
+
     def plot_force_displacement(
-        self, *args, xlabel=r"Displacement $d$", ylabel=r"Force $F$", ax=None, **kwargs
+        self,
+        *args,
+        xlabel=r"Displacement $d$",
+        ylabel=r"Force $F$",
+        ax=None,
+        label=None,
+        **kwargs,
     ):
         "Create a force-displacement plot."
 
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = ax.get_figure()
 
-        ax.plot(self.displacement, self.force, *args, **kwargs)
+        if label is None:
+            label = self.label
+
+        ax.plot(self.displacement, self.force, *args, label=label, **kwargs)
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
 
         return fig, ax
 
     def plot_stress_stretch(
         self,
         *args,
         ax=None,
         xlabel=r"Stretch $l/L$",
         ylabel=r"Force per undeformed area $F/A$",
+        label=None,
         **kwargs,
     ):
-        "Create a strss-stretch plot."
+        "Create a stress-stretch plot."
 
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = ax.get_figure()
 
-        ax.plot(self.stretch, self.stress(), *args, **kwargs)
+        if label is None:
+            label = self.label
+
+        ax.plot(self.stretch, self.stress(), *args, label=label, **kwargs)
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
 
         return fig, ax
```

### Comparing `hyperelastic-0.6.0/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.7.0/src/hyperelastic/math/_voigt.py`

 * *Files 1% similar despite different names*

```diff
@@ -871,14 +871,18 @@
             \boldsymbol{B} \underline{\otimes} \boldsymbol{A}
         \right)
 
         \mathbb{C}_{ijkl} &= \frac{1}{4} \left(
             A_{ik}~B_{jl} + A_{il}~B_{kj} + B_{ik}~A_{jl} + B_{il}~A_{kj}
         \right)
 
+    ..  note::
+        The technical implementation is based on an answer of Jérôme Richard (see
+        `stackoverflow <https://stackoverflow.com/questions/76640596>`_).
+
     Examples
     --------
     >>> from hyperelastic.math import asvoigt, astensor, cdya
     >>> import numpy as np
 
     >>> C = np.array([1.0, 1.3, 1.5, 1.3, 1.1, 1.4, 1.5, 1.4, 1.2]).reshape(3, 3)
     >>> D = np.array([1.0, 1.3, 1.5, 1.3, 1.1, 1.4, 1.5, 1.4, 1.2])[::-1].reshape(3, 3)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hyperelastic-0.6.0/src/hyperelastic/models/generalized/_stretch.py` & `hyperelastic-0.7.0/src/hyperelastic/models/generalized/_stretch.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.7.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/models/stretches/_generalized_invariants.py` & `hyperelastic-0.7.0/src/hyperelastic/models/stretches/_generalized_invariants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,70 @@
 import numpy as np
 
 
 class GeneralizedInvariantsModel:
     r"""Generalized-invariants isotropic hyperelastic material formulation based on the
-    principal stretches. The generalized invariants
+    principal stretches.
 
     ..  math::
 
-        I_1 &= E_1 + E_2 + E_3
+        \psi = \psi \left(
+            I_1\left( E_1(\lambda_1) \right),
+            I_2\left( E_2(\lambda_2) \right),
+            I_3\left( E_3(\lambda_3) \right) \right)
 
-        I_2 &= E_1 E_2 + E_2 E_3 + E_1 E_3
+    The three principal invariants
 
-        I_3 &= E_1 E_2 E_3
+    ..  math::
+
+        J_1 &= E_1 + E_2 + E_3
+
+        J_2 &= E_1 E_2 + E_2 E_3 + E_1 E_3
+
+        J_3 &= E_1 E_2 E_3
 
-    are related to a one-dimensional strain-stretch relation.
+    are formulated on a one-dimensional strain-stretch relation.
 
     ..  math::
 
         E_\alpha &= f(\lambda_\alpha)
 
         E'_\alpha &= f'(\lambda_\alpha) = \frac{\partial f(\lambda_\alpha)}
             {\partial \lambda_\alpha}
 
         E''_\alpha &= f''(\lambda_\alpha) = \frac{\partial^2 f(\lambda_\alpha)}
             {\partial \lambda_\alpha~\partial \lambda_\alpha}
 
+    To be consistent with linear elasticity, the invariants are scaled by deformation-
+    independent coefficients of normalization.
+
+    ..  math::
+
+        I_1 &= c_1 J_1(E_\alpha(\lambda_\alpha))
+             - I_1(E_\alpha(\lambda_\alpha=1)) (c_1 - 1)
+
+        I_2 &= c_2 J_2(E_\alpha(\lambda_\alpha))
+             - I_2(E_\alpha(\lambda_\alpha=1)) (c_2 - 1)
+
+        I_3 &= J_3
+
+    Note that they are only applied to the first and second invariant, as the third
+    invariant does not contribute to the strain energy function at the undeformed state.
+    The second partial derivative of the strain w.r.t. the stretch must be provided for
+    a reference strain (at the undeformed state).
+
+    ..  math::
+
+        c_1 &= \frac{E''_{ref}(\lambda=1) / 3}{
+            \left( E''(\lambda=1) + E'(\lambda=1) \right) / 2}
+
+        c_2 &= \frac{E''_{ref}(\lambda=1, k=2) / 3}{
+            \left( E''(\lambda=1) + E'(\lambda=1) \right) E(\lambda=1)
+            - E'^2(\lambda=1) / 2}
+
     The first partial derivatives of the strain energy function w.r.t. the invariants
 
     ..  math::
 
         \psi_{,1} &= \frac{\partial \psi}{\partial I_1}
 
         \psi_{,2} &= \frac{\partial \psi}{\partial I_2}
@@ -36,17 +72,17 @@
         \psi_{,3} &= \frac{\partial \psi}{\partial I_3}
 
     and the partial derivatives of the invariants w.r.t. the principal stretches are
     defined.
 
     ..  math::
 
-        \frac{\partial I_1}{\partial E_\alpha} &= 1
+        \frac{\partial I_1}{\partial E_\alpha} &= c_1
 
-        \frac{\partial I_2}{\partial E_\alpha} &= E_\beta + E_\gamma
+        \frac{\partial I_2}{\partial E_\alpha} &= c_2 \left( E_\beta + E_\gamma \right)
 
         \frac{\partial I_3}{\partial E_\alpha} &= E_\beta E_\gamma
 
     The first partial derivatives of the strain energy density w.r.t. the
     principal stretches are required for the principal values of the stress.
 
     ..  math::
```

### Comparing `hyperelastic-0.6.0/src/hyperelastic/models/stretches/_ogden.py` & `hyperelastic-0.7.0/src/hyperelastic/models/stretches/_ogden.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.7.0/src/hyperelastic/spaces/_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.7.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.7.0/src/hyperelastic/spaces/_distortional.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.7.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.6.0
+Version: 0.7.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.6.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.7.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,10 +31,12 @@
 src/hyperelastic/models/stretches/_ogden.py
 src/hyperelastic/spaces/__init__.py
 src/hyperelastic/spaces/_deformation.py
 src/hyperelastic/spaces/_dilatational.py
 src/hyperelastic/spaces/_distortional.py
 tests/test_generalized.py
 tests/test_lab.py
+tests/test_lab_simple.py
 tests/test_math.py
+tests/test_simulation.py
 tests/test_space.py
 tests/test_sympy.py
```

### Comparing `hyperelastic-0.6.0/tests/test_generalized.py` & `hyperelastic-0.7.0/tests/test_generalized.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/tests/test_lab.py` & `hyperelastic-0.7.0/tests/test_lab.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,66 +45,90 @@
             label="Uniaxial Tension",
             displacement=displacement,
             force=force,
             area=area,
             length=length,
         ),
         hyperelastic.lab.Experiment(
+            label="Planar Tension",
+            displacement=displacement[::2],
+            force=force[::2] * 8 / 7,
+            area=area,
+            length=length,
+        ),
+        hyperelastic.lab.Experiment(
             label="Biaxial Tension",
             displacement=displacement[::2] / 2,
             force=force[::2] * 2 / 3,
             area=area,
             length=length,
         ),
     ]
 
     ux = hyperelastic.lab.Uniaxial()
     bx = hyperelastic.lab.Biaxial()
+    ps = hyperelastic.lab.Planar()
 
     simulations = [
         hyperelastic.lab.Simulation(
             ux,
             experiments[0].stretch,
             material=material,
             labels=["C10", "C20", "C30", "k"],
         ),
         hyperelastic.lab.Simulation(
-            bx,
+            ps,
             experiments[1].stretch,
             material=material,
             labels=["C10", "C20", "C30", "k"],
         ),
+        hyperelastic.lab.Simulation(
+            bx,
+            experiments[2].stretch,
+            material=material,
+            labels=["C10", "C20", "C30", "k"],
+        ),
     ]
 
     optimize = hyperelastic.lab.Optimize(
         experiments=experiments,
         simulations=simulations,
         parameters=np.ones(4),
         mask=[  # consider only uploading path
             np.diff(experiments[0].displacement, prepend=0) >= 0,
             np.diff(experiments[1].displacement, prepend=0) >= 0,
-            # np.zeros_like(experiments[1].displacement, dtype=bool),
+            np.diff(experiments[2].displacement, prepend=0) >= 0,
+            # np.zeros_like(experiments[1].displacement, dtype=bool), # deactivate
         ],
     )
 
     parameters, pcov = optimize.curve_fit(method="lm")
 
-    print(parameters)
-
     assert np.allclose(
-        parameters, [4.92477300e-01, 9.29251248e-03, 1.08406266e-03, 1.55141229e00]
+        parameters, [5.22901342e-01, 6.60281220e-03, 1.21021751e-03, 1.54827834e00]
     )
 
     fig, ax = experiments[0].plot_force_displacement()
     fig, ax = experiments[1].plot_force_displacement(ax=ax)
+    fig, ax = experiments[2].plot_force_displacement(ax=ax)
+    ax.legend()
 
     fig, ax = experiments[0].plot_stress_stretch()
     fig, ax = experiments[1].plot_stress_stretch(ax=ax)
+    fig, ax = experiments[2].plot_stress_stretch(ax=ax)
+    ax.legend()
 
-    fig, ax = experiments[1].plot_stress_stretch(ax=ax)
+    fig, ax = simulations[0].plot_stress_stretch()
+    fig, ax = simulations[1].plot_stress_stretch(ax=ax)
+    fig, ax = simulations[2].plot_stress_stretch(ax=ax)
+    ax.legend()
+    ax.set_title("Yeoh (Generalized Invariants Framework)")
 
     fig, ax = optimize.plot(title="Yeoh (Generalized Invariants Framework)")
     ax.set_xlim(None, 1.1 * ax.get_xlim()[1])
 
+    return parameters
+
 
 if __name__ == "__main__":
-    test_lab()
+    parameters = test_lab()
+    print(parameters)
```

### Comparing `hyperelastic-0.6.0/tests/test_math.py` & `hyperelastic-0.7.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/tests/test_space.py` & `hyperelastic-0.7.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.6.0/tests/test_sympy.py` & `hyperelastic-0.7.0/tests/test_sympy.py`

 * *Files identical despite different names*

