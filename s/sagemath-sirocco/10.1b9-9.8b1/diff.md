# Comparing `tmp/sagemath-sirocco-10.1b9.tar.gz` & `tmp/sagemath-sirocco-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-sirocco-10.1b9.tar", last modified: Sat Aug  5 23:33:11 2023, max compression
+gzip compressed data, was "sagemath-sirocco-9.8b1.tar", last modified: Mon Nov 21 07:31:32 2022, max compression
```

## Comparing `sagemath-sirocco-10.1b9.tar` & `sagemath-sirocco-9.8b1.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:11.773709 sagemath-sirocco-10.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-05 23:33:11.773709 sagemath-sirocco-10.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-05 23:29:22.000000 sagemath-sirocco-10.1b9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:11.773709 sagemath-sirocco-10.1b9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/sage/all__sagemath_sirocco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:11.773709 sagemath-sirocco-10.1b9/sage/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/sage/libs/all__sagemath_sirocco.py
--rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/sage/libs/sirocco.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:11.773709 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-05 23:33:11.000000 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-05 23:33:11.000000 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:33:11.000000 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-05 23:33:11.000000 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 23:33:11.000000 sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-05 23:33:11.777709 sagemath-sirocco-10.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-05 23:29:06.000000 sagemath-sirocco-10.1b9/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.955325 sagemath-sirocco-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2431 2022-11-21 07:31:32.955461 sagemath-sirocco-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1351 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:42.000000 sagemath-sirocco-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.951592 sagemath-sirocco-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.953554 sagemath-sirocco-9.8b1/sage/libs/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    11139 2022-10-12 20:41:10.000000 sagemath-sirocco-9.8b1/sage/libs/sirocco.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:32.955062 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2431 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      277 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:32.000000 sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1099 2022-11-21 07:31:32.956048 sagemath-sirocco-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2061 2022-11-20 23:45:29.000000 sagemath-sirocco-9.8b1/setup.py
```

### Comparing `sagemath-sirocco-10.1b9/PKG-INFO` & `sagemath-sirocco-9.8b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-sirocco
-Version: 10.1b9
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Certified root continuation with sirocco
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
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

### Comparing `sagemath-sirocco-10.1b9/README.rst` & `sagemath-sirocco-9.8b1/README.rst`

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

### Comparing `sagemath-sirocco-10.1b9/sage/libs/sirocco.pyx` & `sagemath-sirocco-9.8b1/sage/libs/sirocco.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -288,7 +288,8 @@
     for i in range(n):
         l[i] = (rop[3*i+1], rop[3*i+2], rop[3*i+3])
     free(rop)
     free(c_values)
     free(c_otherdegrees)
     free(c_othercoefs)
     return l
+
```

### Comparing `sagemath-sirocco-10.1b9/sagemath_sirocco.egg-info/PKG-INFO` & `sagemath-sirocco-9.8b1/sagemath_sirocco.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemath-sirocco
-Version: 10.1b9
+Version: 9.8b1
 Summary: Sage: Open Source Mathematics Software: Certified root continuation with sirocco
 Home-page: https://www.sagemath.org
 Author: The Sage Developers
 Author-email: sage-support@googlegroups.com
 License: GNU General Public License (GPL) v2 or later
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Education
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

### Comparing `sagemath-sirocco-10.1b9/setup.cfg` & `sagemath-sirocco-9.8b1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
 install_requires = 
-	cypari2 >=2.1.1
-	cysignals >=1.10.2
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-sirocco-10.1b9/setup.py` & `sagemath-sirocco-9.8b1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-sirocco']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-sirocco'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-sirocco'])
 
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

