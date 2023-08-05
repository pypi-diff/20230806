# Comparing `tmp/sagemath-mcqd-10.1b9.tar.gz` & `tmp/sagemath-mcqd-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-mcqd-10.1b9.tar", last modified: Sat Aug  5 23:33:09 2023, max compression
+gzip compressed data, was "sagemath-mcqd-9.8b1.tar", last modified: Mon Nov 21 07:31:29 2022, max compression
```

## Comparing `sagemath-mcqd-10.1b9.tar` & `sagemath-mcqd-9.8b1.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:09.205738 sagemath-mcqd-10.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-05 23:33:09.205738 sagemath-mcqd-10.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-05 23:29:22.000000 sagemath-mcqd-10.1b9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:09.201738 sagemath-mcqd-10.1b9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/sage/all__sagemath_mcqd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:09.201738 sagemath-mcqd-10.1b9/sage/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/sage/graphs/all__sagemath_mcqd.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/sage/graphs/mcqd.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/sage/graphs/mcqd.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:09.205738 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-05 23:33:08.000000 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-05 23:33:09.000000 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:33:08.000000 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-05 23:33:08.000000 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 23:33:08.000000 sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-05 23:33:09.205738 sagemath-mcqd-10.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-05 23:29:06.000000 sagemath-mcqd-10.1b9/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435581 sagemath-mcqd-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.435722 sagemath-mcqd-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1316 2022-11-20 23:46:42.000000 sagemath-mcqd-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-mcqd-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.432004 sagemath-mcqd-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.433786 sagemath-mcqd-9.8b1/sage/graphs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1677 2022-10-12 20:41:10.000000 sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:29.435257 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2388 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      261 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:29.000000 sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1091 2022-11-21 07:31:29.436316 sagemath-mcqd-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2055 2022-11-20 23:45:29.000000 sagemath-mcqd-9.8b1/setup.py
```

### Comparing `sagemath-mcqd-10.1b9/PKG-INFO` & `sagemath-mcqd-9.8b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
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

### Comparing `sagemath-mcqd-10.1b9/README.rst` & `sagemath-mcqd-9.8b1/README.rst`

 * *Files 0% similar despite different names*

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

### Comparing `sagemath-mcqd-10.1b9/sage/graphs/mcqd.pyx` & `sagemath-mcqd-9.8b1/sage/graphs/mcqd.pyx`

 * *Files identical despite different names*

### Comparing `sagemath-mcqd-10.1b9/sagemath_mcqd.egg-info/PKG-INFO` & `sagemath-mcqd-9.8b1/sagemath_mcqd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-mcqd
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Finding maximum cliques with mcqd
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with mcqd
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

### Comparing `sagemath-mcqd-10.1b9/setup.py` & `sagemath-mcqd-9.8b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-mcqd']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-mcqd'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-mcqd'])
 
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

