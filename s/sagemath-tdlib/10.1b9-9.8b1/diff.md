# Comparing `tmp/sagemath-tdlib-10.1b9.tar.gz` & `tmp/sagemath-tdlib-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-tdlib-10.1b9.tar", last modified: Sat Aug  5 23:33:10 2023, max compression
+gzip compressed data, was "sagemath-tdlib-9.8b1.tar", last modified: Mon Nov 21 07:31:30 2022, max compression
```

## Comparing `sagemath-tdlib-10.1b9.tar` & `sagemath-tdlib-9.8b1.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.033729 sagemath-tdlib-10.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-05 23:33:10.033729 sagemath-tdlib-10.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-05 23:29:22.000000 sagemath-tdlib-10.1b9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.029729 sagemath-tdlib-10.1b9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/sage/all__sagemath_tdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.029729 sagemath-tdlib-10.1b9/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/sage/graphs/all__sagemath_tdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.033729 sagemath-tdlib-10.1b9/sage/graphs/graph_decompositions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/sage/graphs/graph_decompositions/all__sagemath_tdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/sage/graphs/graph_decompositions/sage_tdlib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/sage/graphs/graph_decompositions/tdlib.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.033729 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-05 23:33:09.000000 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-05 23:33:10.000000 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:33:09.000000 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 23:33:09.000000 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 23:33:09.000000 sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-05 23:33:10.033729 sagemath-tdlib-10.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-05 23:29:06.000000 sagemath-tdlib-10.1b9/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702261 sagemath-tdlib-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.702399 sagemath-tdlib-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1276 2022-11-20 23:46:42.000000 sagemath-tdlib-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-tdlib-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698530 sagemath-tdlib-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.698631 sagemath-tdlib-9.8b1/sage/graphs/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.700524 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     5663 2022-10-12 20:41:10.000000 sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:30.702002 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2350 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      288 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:30.000000 sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1093 2022-11-21 07:31:30.702993 sagemath-tdlib-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2057 2022-11-20 23:45:29.000000 sagemath-tdlib-9.8b1/setup.py
```

### Comparing `sagemath-tdlib-10.1b9/PKG-INFO` & `sagemath-tdlib-9.8b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Tree decompositions with tdlib
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -28,15 +28,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.1b9/README.rst` & `sagemath-tdlib-9.8b1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.1b9/sage/graphs/graph_decompositions/tdlib.pyx` & `sagemath-tdlib-9.8b1/sage/graphs/graph_decompositions/tdlib.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -128,20 +128,19 @@
         sage: import sage.graphs.graph_decompositions.tdlib as tdlib # optional - tdlib
         sage: G = graphs.HouseGraph()                                # optional - tdlib
         sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
         sage: T.show(vertex_size=2000)                               # optional - tdlib
 
     TESTS::
 
-        sage: # optional - tdlib
-        sage: import sage.graphs.graph_decompositions.tdlib as tdlib
-        sage: G = graphs.HouseGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
-        sage: G = graphs.PetersenGraph()
-        sage: T = tdlib.treedecomposition_exact(G)
+        sage: import sage.graphs.graph_decompositions.tdlib as tdlib # optional - tdlib
+        sage: G = graphs.HouseGraph()                                # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
+        sage: G = graphs.PetersenGraph()                             # optional - tdlib
+        sage: T = tdlib.treedecomposition_exact(G)                   # optional - tdlib
 
     """
     cdef vector[unsigned int] V_G, E_G, E_T
     cdef vector[vector[int]] V_T
 
     cdef list int_to_vertex = list(G)
     cdef dict vertex_to_int = {v: i for i, v in enumerate(G)}
```

### Comparing `sagemath-tdlib-10.1b9/sagemath_tdlib.egg-info/PKG-INFO` & `sagemath-tdlib-9.8b1/sagemath_tdlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-tdlib
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Tree decompositions with tdlib
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -28,15 +28,15 @@
 
 About SageMath
 --------------
 
    "Creating a Viable Open Source Alternative to
     Magma, Maple, Mathematica, and MATLAB"
 
-   Copyright (C) 2005-2023 The Sage Development Team
+   Copyright (C) 2005-2022 The Sage Development Team
 
    https://www.sagemath.org
 
 SageMath fully supports all major Linux distributions, recent versions of
 macOS, and Windows (using Cygwin or Windows Subsystem for Linux).
 
 The traditional and recommended way to install SageMath is from source via
```

### Comparing `sagemath-tdlib-10.1b9/setup.cfg` & `sagemath-tdlib-9.8b1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = sagemath-tdlib
 version = file: VERSION.txt
-description = Sage: Open Source Mathematics Software: Tree decompositions with tdlib
+description = Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with tdlib
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = GNU General Public License (GPL) v2 or later
 author = The Sage Developers
 author_email = sage-support@googlegroups.com
 url = https://www.sagemath.org
 classifiers = 
@@ -21,13 +21,14 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
-install_requires = cysignals >=1.10.2
+install_requires = 
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-tdlib-10.1b9/setup.py` & `sagemath-tdlib-9.8b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-tdlib']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-tdlib'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-tdlib'])
 
-log.warn('python_packages = {0}'.format(python_packages))
-log.warn('python_modules = {0}'.format(python_modules))
-log.warn('cython_modules = {0}'.format(cython_modules))
+    log.warn('python_packages = {0}'.format(python_packages))
+    log.warn('python_modules = {0}'.format(python_modules))
+    log.warn('cython_modules = {0}'.format(cython_modules))
 
 setup(
     cmdclass = cmdclass,
     packages = python_packages,
     py_modules  = python_modules,
     ext_modules = cython_modules,
 )
```

