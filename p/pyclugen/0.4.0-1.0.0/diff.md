# Comparing `tmp/pyclugen-0.4.0.tar.gz` & `tmp/pyclugen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclugen-0.4.0.tar", last modified: Tue Jun 20 18:27:34 2023, max compression
+gzip compressed data, was "pyclugen-1.0.0.tar", last modified: Sun Aug  6 18:37:14 2023, max compression
```

## Comparing `pyclugen-0.4.0.tar` & `pyclugen-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.290877 pyclugen-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 18:27:26.000000 pyclugen-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-20 18:27:34.290877 pyclugen-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-20 18:27:26.000000 pyclugen-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.286877 pyclugen-0.4.0/pyclugen/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27822 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.286877 pyclugen-0.4.0/pyclugen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:27:34.290877 pyclugen-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.290877 pyclugen-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:37:14.915016 pyclugen-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-06 18:37:06.000000 pyclugen-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-06 18:37:14.915016 pyclugen-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-06 18:37:06.000000 pyclugen-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:37:14.915016 pyclugen-1.0.0/pyclugen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27822 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyclugen/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:37:14.915016 pyclugen-1.0.0/pyclugen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-06 18:37:14.000000 pyclugen-1.0.0/pyclugen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 18:37:14.000000 pyclugen-1.0.0/pyclugen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:37:14.000000 pyclugen-1.0.0/pyclugen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-06 18:37:14.000000 pyclugen-1.0.0/pyclugen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 18:37:14.000000 pyclugen-1.0.0/pyclugen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-08-06 18:37:06.000000 pyclugen-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:37:14.915016 pyclugen-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:37:14.915016 pyclugen-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-06 18:37:06.000000 pyclugen-1.0.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-08-06 18:37:06.000000 pyclugen-1.0.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-08-06 18:37:06.000000 pyclugen-1.0.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-06 18:37:06.000000 pyclugen-1.0.0/tests/test_module.py
```

### Comparing `pyclugen-0.4.0/LICENSE.txt` & `pyclugen-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/PKG-INFO` & `pyclugen-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.4.0
+Version: 1.0.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -87,13 +87,15 @@
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
   implementation of the *clugen* algorithm.
 
 ## Reference
 
 If you use this software, please cite the following reference:
 
-* Fachada, N. & de Andrade, D. (2023). Generating Multidimensional Clusters With
-  Support Lines. <https://doi.org/10.48550/arXiv.2301.10327>.
+* Fachada, N. & de Andrade, D. (2023). Generating multidimensional clusters
+  with support lines. *Knowledge-Based Systems*, 277, 110836.
+  <https://doi.org/10.1016/j.knosys.2023.110836>
+  ([arXiv preprint](https://doi.org/10.48550/arXiv.2301.10327))
 
 ## License
 
 [MIT License](LICENSE.txt)
```

### Comparing `pyclugen-0.4.0/README.md` & `pyclugen-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -66,13 +66,15 @@
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
   implementation of the *clugen* algorithm.
 
 ## Reference
 
 If you use this software, please cite the following reference:
 
-* Fachada, N. & de Andrade, D. (2023). Generating Multidimensional Clusters With
-  Support Lines. <https://doi.org/10.48550/arXiv.2301.10327>.
+* Fachada, N. & de Andrade, D. (2023). Generating multidimensional clusters
+  with support lines. *Knowledge-Based Systems*, 277, 110836.
+  <https://doi.org/10.1016/j.knosys.2023.110836>
+  ([arXiv preprint](https://doi.org/10.48550/arXiv.2301.10327))
 
 ## License
 
 [MIT License](LICENSE.txt)
```

### Comparing `pyclugen-0.4.0/pyclugen/__init__.py` & `pyclugen-1.0.0/pyclugen/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/pyclugen/core.py` & `pyclugen-1.0.0/pyclugen/core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/pyclugen/helper.py` & `pyclugen-1.0.0/pyclugen/helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/pyclugen/main.py` & `pyclugen-1.0.0/pyclugen/main.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/pyclugen/module.py` & `pyclugen-1.0.0/pyclugen/module.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/pyclugen.egg-info/PKG-INFO` & `pyclugen-1.0.0/pyclugen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.4.0
+Version: 1.0.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -87,13 +87,15 @@
 * [MOCluGen](https://github.com/clugen/MOCluGen/), a MATLAB/Octave
   implementation of the *clugen* algorithm.
 
 ## Reference
 
 If you use this software, please cite the following reference:
 
-* Fachada, N. & de Andrade, D. (2023). Generating Multidimensional Clusters With
-  Support Lines. <https://doi.org/10.48550/arXiv.2301.10327>.
+* Fachada, N. & de Andrade, D. (2023). Generating multidimensional clusters
+  with support lines. *Knowledge-Based Systems*, 277, 110836.
+  <https://doi.org/10.1016/j.knosys.2023.110836>
+  ([arXiv preprint](https://doi.org/10.48550/arXiv.2301.10327))
 
 ## License
 
 [MIT License](LICENSE.txt)
```

### Comparing `pyclugen-0.4.0/pyproject.toml` & `pyclugen-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyclugen"
 description = "Multidimensional cluster generation in Python"
-version = "0.4.0"
+version = "1.0.0"
 authors = [ { name = "Nuno Fachada", email = "faken@fakenmc.com" } ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "multidimensional data",
     "synthetic clusters",
     "synthetic data generation",
```

### Comparing `pyclugen-0.4.0/tests/test_core.py` & `pyclugen-1.0.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/tests/test_helper.py` & `pyclugen-1.0.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/tests/test_main.py` & `pyclugen-1.0.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.4.0/tests/test_module.py` & `pyclugen-1.0.0/tests/test_module.py`

 * *Files identical despite different names*

