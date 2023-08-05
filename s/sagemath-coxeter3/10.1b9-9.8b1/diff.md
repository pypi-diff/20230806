# Comparing `tmp/sagemath-coxeter3-10.1b9.tar.gz` & `tmp/sagemath-coxeter3-9.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemath-coxeter3-10.1b9.tar", last modified: Sat Aug  5 23:33:10 2023, max compression
+gzip compressed data, was "sagemath-coxeter3-9.8b1.tar", last modified: Mon Nov 21 07:31:31 2022, max compression
```

## Comparing `sagemath-coxeter3-10.1b9.tar` & `sagemath-coxeter3-9.8b1.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-05 23:29:22.000000 sagemath-coxeter3-10.1b9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/sage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/all__sagemath_coxeter3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/sage/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/all__sagemath_coxeter3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/all__sagemath_coxeter3.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/coxeter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    50716 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/coxeter.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    30058 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/coxeter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/sage/libs/coxeter3/decl.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 23:33:10.889719 sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-05 23:33:10.000000 sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-05 23:33:10.000000 sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 23:33:10.000000 sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-05 23:33:10.000000 sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-05 23:33:10.893719 sagemath-coxeter3-10.1b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-05 23:29:06.000000 sagemath-coxeter3-10.1b9/setup.py
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.822778 sagemath-coxeter3-9.8b1/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      185 2022-11-20 23:45:29.000000 sagemath-coxeter3-9.8b1/MANIFEST.in
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2441 2022-11-21 07:31:31.822929 sagemath-coxeter3-9.8b1/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1361 2022-11-20 23:46:42.000000 sagemath-coxeter3-9.8b1/README.rst
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      292 2022-11-21 07:28:43.000000 sagemath-coxeter3-9.8b1/pyproject.toml
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.817720 sagemath-coxeter3-9.8b1/sage/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.817818 sagemath-coxeter3-9.8b1/sage/libs/
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.819877 sagemath-coxeter3-9.8b1/sage/libs/coxeter3/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)    50746 2022-10-12 20:41:10.000000 sagemath-coxeter3-9.8b1/sage/libs/coxeter3/coxeter.pyx
+drwxr-xr-x   0 mkoeppe    (502) staff       (20)        0 2022-11-21 07:31:31.822509 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2441 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/PKG-INFO
+-rw-r--r--   0 mkoeppe    (502) staff       (20)      291 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/SOURCES.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        1 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/dependency_links.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)       25 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/requires.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)        5 2022-11-21 07:31:31.000000 sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/top_level.txt
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     1099 2022-11-21 07:31:31.823580 sagemath-coxeter3-9.8b1/setup.cfg
+-rw-r--r--   0 mkoeppe    (502) staff       (20)     2063 2022-11-20 23:45:29.000000 sagemath-coxeter3-9.8b1/setup.py
```

### Comparing `sagemath-coxeter3-10.1b9/PKG-INFO` & `sagemath-coxeter3-9.8b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-coxeter3
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with coxeter3
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

### Comparing `sagemath-coxeter3-10.1b9/README.rst` & `sagemath-coxeter3-9.8b1/README.rst`

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

### Comparing `sagemath-coxeter3-10.1b9/sage/libs/coxeter3/coxeter.pyx` & `sagemath-coxeter3-9.8b1/sage/libs/coxeter3/coxeter.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 # distutils: language = c++
 # distutils: libraries = coxeter3
 # sage_setup: distribution = sagemath-coxeter3
 
 """
 Low level part of the interface to Fokko Ducloux's Coxeter 3 library
 
@@ -772,15 +773,15 @@
             sage: w[4]                                                                              # optional - coxeter3
             Traceback (most recent call last):
             ...
             IndexError: The index (4) is out of range.
         """
         if isinstance(i, slice):
             #Get the start, stop, and step from the slice
-            return [self[ii] for ii in range(*i.indices(len(self)))]
+            return [self[ii] for ii in xrange(*i.indices(len(self)))]
         if i < 0:
             i += len(self)
         if i >= len(self):
             raise IndexError("The index (%d) is out of range." % i)
 
         return self._parent_group.out_ordering[self.word[i]]
 
@@ -868,15 +869,15 @@
 
             sage: from sage.libs.coxeter3.coxeter import *      # optional - coxeter3
             sage: W = CoxGroup(['A',5])                         # optional - coxeter3
             sage: w = W([1,2,3])                                # optional - coxeter3
             sage: [a for a in w]                                # optional - coxeter3
             [1, 2, 3]
         """
-        return (self[i] for i in range(len(self)))
+        return (self[i] for i in xrange(len(self)))
 
     def __len__(self):
         """
         Return the length of this element.
 
         EXAMPLES::
 
@@ -975,15 +976,15 @@
         cdef c_List_CoxWord list = c_List_CoxWord(0)
         self.group.coatoms(list, self.word)
 
         coatoms = []
 
         cdef Length i = 0
         cdef CoxGroupElement res
-        for i in range(list.size()):
+        for i from 0 <= i < list.size():
             res = self._new()
             res.word = list[i]
             coatoms.append(res)
         return coatoms
 
     def normal_form(self):
         """
```

### Comparing `sagemath-coxeter3-10.1b9/sagemath_coxeter3.egg-info/PKG-INFO` & `sagemath-coxeter3-9.8b1/sagemath_coxeter3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sagemath-coxeter3
-Version: 10.1b9
-Summary: Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
+Version: 9.8b1
+Summary: Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with coxeter3
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

### Comparing `sagemath-coxeter3-10.1b9/setup.cfg` & `sagemath-coxeter3-9.8b1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = sagemath-coxeter3
 version = file: VERSION.txt
-description = Sage: Open Source Mathematics Software: Coxeter groups, Bruhat ordering, Kazhdan-Lusztig polynomials with coxeter3
+description = Sage: Open Source Mathematics Software: Graph (iso/auto)morphisms with coxeter3
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = GNU General Public License (GPL) v2 or later
 author = The Sage Developers
 author_email = sage-support@googlegroups.com
 url = https://www.sagemath.org
 classifiers = 
@@ -22,19 +22,13 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 python_requires = >=3.8, <3.12
 install_requires = 
-packages = 
-	sage.libs.coxeter3
-
-[options.package_data]
-sage.libs.coxeter3 = 
-	coxeter.pxd
-	decl.pxd
+	sagemath-standard ~= 9.8b3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sagemath-coxeter3-10.1b9/setup.py` & `sagemath-coxeter3-9.8b1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,21 +43,26 @@
     from sage_setup.command.sage_build_cython import sage_build_cython
     from sage_setup.command.sage_build_ext import sage_build_ext
     sage_build_cython.built_distributions = ['sagemath-coxeter3']
 
     cmdclass = dict(build_cython=sage_build_cython,
                     build_ext=sage_build_ext)
 
-from sage_setup.find import find_python_sources
-python_packages, python_modules, cython_modules = find_python_sources(
-    '.', ['sage'], distributions=['sagemath-coxeter3'])
+if sdist:
+    python_packages = []
+    python_modules = []
+    cython_modules = []
+else:
+    from sage_setup.find import find_python_sources
+    python_packages, python_modules, cython_modules = find_python_sources(
+        '.', ['sage'], distributions=['sagemath-coxeter3'])
 
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

