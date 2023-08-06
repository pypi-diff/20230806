# Comparing `tmp/numexpr-2.8.3.tar.gz` & `tmp/numexpr-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numexpr-2.8.3.tar", last modified: Sat Jun 25 20:35:21 2022, max compression
+gzip compressed data, was "numexpr-2.8.4.tar", last modified: Wed Oct 26 02:59:27 2022, max compression
```

## Comparing `numexpr-2.8.3.tar` & `numexpr-2.8.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.620025 numexpr-2.8.3/
--rw-rw-rw-   0        0        0     2913 2022-06-25 20:25:22.000000 numexpr-2.8.3/ANNOUNCE.rst
--rw-rw-rw-   0        0        0      942 2022-06-25 20:25:22.000000 numexpr-2.8.3/AUTHORS.txt
--rw-rw-rw-   0        0        0     1214 2022-06-25 20:25:22.000000 numexpr-2.8.3/LICENSE.txt
--rw-rw-rw-   0        0        0      240 2022-06-25 20:25:22.000000 numexpr-2.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8096 2022-06-25 20:35:21.620025 numexpr-2.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     7084 2022-06-25 20:25:22.000000 numexpr-2.8.3/README.rst
--rw-rw-rw-   0        0        0    26742 2022-06-25 20:25:22.000000 numexpr-2.8.3/RELEASE_NOTES.rst
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.605028 numexpr-2.8.3/bench/
--rw-rw-rw-   0        0        0     5668 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/boolean_timing.py
--rw-rw-rw-   0        0        0      929 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/issue-36.py
--rw-rw-rw-   0        0        0      202 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/issue-47.py
--rw-rw-rw-   0        0        0     2801 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/multidim.py
--rw-rw-rw-   0        0        0     1960 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/poly.py
--rw-rw-rw-   0        0        0     4119 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/timing.py
--rw-rw-rw-   0        0        0     1489 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/unaligned-simple.py
--rw-rw-rw-   0        0        0     1679 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/varying-expr.py
--rw-rw-rw-   0        0        0     6040 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/vml_timing.py
--rw-rw-rw-   0        0        0     1526 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/vml_timing2.py
--rw-rw-rw-   0        0        0      324 2022-06-25 20:25:22.000000 numexpr-2.8.3/bench/vml_timing3.py
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.614027 numexpr-2.8.3/numexpr/
--rw-rw-rw-   0        0        0     2328 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/__init__.py
--rw-rw-rw-   0        0        0     9273 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/complex_functions.hpp
--rw-rw-rw-   0        0        0    26021 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/cpuinfo.py
--rw-rw-rw-   0        0        0    16970 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/expressions.py
--rw-rw-rw-   0        0        0     5842 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/functions.hpp
--rw-rw-rw-   0        0        0    21241 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/interp_body.cpp
--rw-rw-rw-   0        0        0    49672 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/interpreter.cpp
--rw-rw-rw-   0        0        0     2708 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/interpreter.hpp
--rw-rw-rw-   0        0        0     2052 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/missing_posix_functions.hpp
--rw-rw-rw-   0        0        0    15815 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/module.cpp
--rw-rw-rw-   0        0        0     2261 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/module.hpp
--rw-rw-rw-   0        0        0     3620 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/msvc_function_stubs.hpp
--rw-rw-rw-   0        0        0    28575 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/necompiler.py
--rw-rw-rw-   0        0        0     1177 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/numexpr_config.hpp
--rw-rw-rw-   0        0        0    15041 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/numexpr_object.cpp
--rw-rw-rw-   0        0        0     1069 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/numexpr_object.hpp
--rw-rw-rw-   0        0        0     7489 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/opcodes.hpp
--rw-rw-rw-   0        0        0    14863 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/str-two-way.hpp
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.618027 numexpr-2.8.3/numexpr/tests/
--rw-rw-rw-   0        0        0      461 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/tests/__init__.py
--rw-rw-rw-   0        0        0    46227 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/tests/test_numexpr.py
--rw-rw-rw-   0        0        0     7693 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/utils.py
--rw-rw-rw-   0        0        0      119 2022-06-25 20:35:20.000000 numexpr-2.8.3/numexpr/version.py
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.620025 numexpr-2.8.3/numexpr/win32/
--rw-rw-rw-   0        0        0     7303 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/win32/pthread.c
--rw-rw-rw-   0        0        0     3439 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/win32/pthread.h
--rw-rw-rw-   0        0        0     7565 2022-06-25 20:25:22.000000 numexpr-2.8.3/numexpr/win32/stdint.h
-drwxrwxrwx   0        0        0        0 2022-06-25 20:35:21.617026 numexpr-2.8.3/numexpr.egg-info/
--rw-rw-rw-   0        0        0     8096 2022-06-25 20:35:20.000000 numexpr-2.8.3/numexpr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1173 2022-06-25 20:35:21.000000 numexpr-2.8.3/numexpr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-25 20:35:21.000000 numexpr-2.8.3/numexpr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-25 20:26:16.000000 numexpr-2.8.3/numexpr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2022-06-25 20:35:21.000000 numexpr-2.8.3/numexpr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-25 20:35:21.000000 numexpr-2.8.3/numexpr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2022-06-25 20:25:22.000000 numexpr-2.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       26 2022-06-25 20:25:22.000000 numexpr-2.8.3/requirements.txt
--rw-rw-rw-   0        0        0      972 2022-06-25 20:35:21.621027 numexpr-2.8.3/setup.cfg
--rw-rw-rw-   0        0        0     3102 2022-06-25 20:25:22.000000 numexpr-2.8.3/setup.py
--rw-rw-rw-   0        0        0      700 2022-06-25 20:25:22.000000 numexpr-2.8.3/site.cfg.example
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.071168 numexpr-2.8.4/
+-rw-rw-rw-   0        0        0     2218 2022-10-26 02:43:06.000000 numexpr-2.8.4/ANNOUNCE.rst
+-rw-rw-rw-   0        0        0      942 2022-10-26 02:43:06.000000 numexpr-2.8.4/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1214 2022-10-26 02:43:06.000000 numexpr-2.8.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      240 2022-10-26 02:43:06.000000 numexpr-2.8.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8152 2022-10-26 02:59:27.071168 numexpr-2.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7088 2022-10-26 02:43:06.000000 numexpr-2.8.4/README.rst
+-rw-rw-rw-   0        0        0    27367 2022-10-26 02:43:06.000000 numexpr-2.8.4/RELEASE_NOTES.rst
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.055543 numexpr-2.8.4/bench/
+-rw-rw-rw-   0        0        0     5668 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/boolean_timing.py
+-rw-rw-rw-   0        0        0      929 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/issue-36.py
+-rw-rw-rw-   0        0        0      202 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/issue-47.py
+-rw-rw-rw-   0        0        0     2801 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/multidim.py
+-rw-rw-rw-   0        0        0     1960 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/poly.py
+-rw-rw-rw-   0        0        0     4119 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/timing.py
+-rw-rw-rw-   0        0        0     1489 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/unaligned-simple.py
+-rw-rw-rw-   0        0        0     1679 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/varying-expr.py
+-rw-rw-rw-   0        0        0     6040 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/vml_timing.py
+-rw-rw-rw-   0        0        0     1526 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/vml_timing2.py
+-rw-rw-rw-   0        0        0      324 2022-10-26 02:43:06.000000 numexpr-2.8.4/bench/vml_timing3.py
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.071168 numexpr-2.8.4/numexpr/
+-rw-rw-rw-   0        0        0     2328 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/__init__.py
+-rw-rw-rw-   0        0        0     9330 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/complex_functions.hpp
+-rw-rw-rw-   0        0        0    26021 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/cpuinfo.py
+-rw-rw-rw-   0        0        0    16818 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/expressions.py
+-rw-rw-rw-   0        0        0     5863 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/functions.hpp
+-rw-rw-rw-   0        0        0    21241 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/interp_body.cpp
+-rw-rw-rw-   0        0        0    49684 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/interpreter.cpp
+-rw-rw-rw-   0        0        0     2708 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/interpreter.hpp
+-rw-rw-rw-   0        0        0     2052 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/missing_posix_functions.hpp
+-rw-rw-rw-   0        0        0    15815 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/module.cpp
+-rw-rw-rw-   0        0        0     2261 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/module.hpp
+-rw-rw-rw-   0        0        0     3620 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/msvc_function_stubs.hpp
+-rw-rw-rw-   0        0        0    28891 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/necompiler.py
+-rw-rw-rw-   0        0        0     1177 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/numexpr_config.hpp
+-rw-rw-rw-   0        0        0    15041 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/numexpr_object.cpp
+-rw-rw-rw-   0        0        0     1069 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/numexpr_object.hpp
+-rw-rw-rw-   0        0        0     7489 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/opcodes.hpp
+-rw-rw-rw-   0        0        0    14863 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/str-two-way.hpp
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.071168 numexpr-2.8.4/numexpr/tests/
+-rw-rw-rw-   0        0        0      461 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/tests/__init__.py
+-rw-rw-rw-   0        0        0    46773 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/tests/test_numexpr.py
+-rw-rw-rw-   0        0        0     7693 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/utils.py
+-rw-rw-rw-   0        0        0      119 2022-10-26 02:59:26.000000 numexpr-2.8.4/numexpr/version.py
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.071168 numexpr-2.8.4/numexpr/win32/
+-rw-rw-rw-   0        0        0     7303 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/win32/pthread.c
+-rw-rw-rw-   0        0        0     3439 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/win32/pthread.h
+-rw-rw-rw-   0        0        0     7565 2022-10-26 02:43:06.000000 numexpr-2.8.4/numexpr/win32/stdint.h
+drwxrwxrwx   0        0        0        0 2022-10-26 02:59:27.071168 numexpr-2.8.4/numexpr.egg-info/
+-rw-rw-rw-   0        0        0     8152 2022-10-26 02:59:26.000000 numexpr-2.8.4/numexpr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1173 2022-10-26 02:59:27.000000 numexpr-2.8.4/numexpr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-26 02:59:26.000000 numexpr-2.8.4/numexpr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-26 02:44:17.000000 numexpr-2.8.4/numexpr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2022-10-26 02:59:26.000000 numexpr-2.8.4/numexpr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-10-26 02:59:26.000000 numexpr-2.8.4/numexpr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2022-10-26 02:43:06.000000 numexpr-2.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2022-10-26 02:43:06.000000 numexpr-2.8.4/requirements.txt
+-rw-rw-rw-   0        0        0     1013 2022-10-26 02:59:27.071168 numexpr-2.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     3138 2022-10-26 02:43:06.000000 numexpr-2.8.4/setup.py
+-rw-rw-rw-   0        0        0      700 2022-10-26 02:43:06.000000 numexpr-2.8.4/site.cfg.example
```

### Comparing `numexpr-2.8.3/ANNOUNCE.rst` & `numexpr-2.8.4/ANNOUNCE.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,33 @@
 ========================
-Announcing NumExpr 2.8.3
+Announcing NumExpr 2.8.4
 ========================
 
 Hi everyone, 
 
-Please find here another maintenance release of NumExpr. Support for Python 3.6 
-has been dropped to enable support for NumPy 1.23 (and by extension Python 3.11 
-when it is released). Wheels for ARM64 multilinux should be available again after 
-troubles with GitHub Actions and Apple Silicon wheels are also now available on 
-PyPi for download.
+This is a maintenance and bug-fix release for NumExpr. In particular, now we have 
+added Python 3.11 support. 
 
 Project documentation is available at:
 
 http://numexpr.readthedocs.io/
 
 
-Changes from 2.8.1 to 2.8.2
+Changes from 2.8.3 to 2.8.4
 ---------------------------
 
-* Support for Python 3.6 has been dropped due to the need to substitute the flag 
-  `NPY_ARRAY_WRITEBACKIFCOPY` for `NPY_ARRAY_UPDATEIFCOPY`. This flag change was 
-  initiated in NumPy 1.14 and finalized in 1.23. The only changes were made to 
-  cases where an unaligned constant was passed in with a pre-allocated output 
-  variable:
-
-```
-    x = np.empty(5, dtype=np.uint8)[1:].view(np.int32)
-    ne.evaluate('3', out=x)
-```
-
-  We think the risk of issues is very low, but if you are using NumExpr as a 
-  expression evaluation tool you may want to write a test for this edge case.
-* Thanks to Matt Einhorn (@matham) for improvements to the GitHub Actions build process to
-  add support for Apple Silicon and aarch64.
-* Thanks to Biswapriyo Nath (@biswa96) for a fix to allow `mingw` builds on Windows.
-* There have been some changes made to not import `platform.machine()` on `sparc`
-  but it is highly advised to upgrade to Python 3.9+ to avoid this issue with 
-  the Python core package `platform`.
+* Support for Python 3.11 has been added.
+* Thanks to Tobias Hangleiter for an improved accuracy complex `expm1` function.
+  While it is 25 % slower, it is significantly more accurate for the real component
+  over a range of values and matches NumPy outputs much more closely.
+* Thanks to Kirill Kouzoubov for a range of fixes to constants parsing that was 
+  resulting in duplicated constants of the same value.
+* Thanks to Mark Harfouche for noticing that we no longer need `numpy` version 
+  checks. `packaging` is no longer a requirement as a result.
+
 
 What's Numexpr?
 ---------------
 
 Numexpr is a fast numerical expression evaluator for NumPy.  With it,
 expressions that operate on arrays (like "3*a+4*b") are accelerated
 and use less memory than doing the same calculation in Python.
```

### Comparing `numexpr-2.8.3/AUTHORS.txt` & `numexpr-2.8.4/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/LICENSE.txt` & `numexpr-2.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/PKG-INFO` & `numexpr-2.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numexpr
-Version: 2.8.3
+Version: 2.8.4
 Summary: Fast numerical expression evaluator for NumPy
 Home-page: https://github.com/pydata/numexpr
 Author: David M. Cooke, Francesc Alted, and others
 Maintainer: Robert A. McLeod
 Maintainer-email: robbmcleod@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
@@ -82,17 +83,17 @@
 constants in the expression are also chunked. Chunks are distributed among 
 the available cores of the CPU, resulting in highly parallelized code 
 execution.
 
 The result is that NumExpr can get the most of your machine computing
 capabilities for array-wise computations. Common speed-ups with regard
 to NumPy are usually between 0.95x (for very simple expressions like
-:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a >
-2.5*b'`), although much higher speed-ups can be achieved for some functions 
-and complex math operations (up to 15x in some cases).
+:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a > 2.5*b'`), 
+although much higher speed-ups can be achieved for some functions  and complex 
+math operations (up to 15x in some cases).
 
 NumExpr performs best on matrices that are too large to fit in L1 CPU cache. 
 In order to get a better idea on the different speed-ups that can be achieved 
 on your platform, run the provided benchmarks.
 
 Installation
 ------------
@@ -110,25 +111,25 @@
 to use the `conda` package manager in this case::
 
     conda install numexpr
 
 From Source
 ^^^^^^^^^^^
 
-On most `Nix systems your compilers will already be present. However if you 
+On most \*nix systems your compilers will already be present. However if you 
 are using a virtual environment with a substantially newer version of Python than
 your system Python you may be prompted to install a new version of `gcc` or `clang`.
 
 For Windows, you will need to install the Microsoft Visual C++ Build Tools 
-(which are free) first.The version depends on which version of Python you have 
+(which are free) first. The version depends on which version of Python you have 
 installed:
 
 https://wiki.python.org/moin/WindowsCompilers
 
-For Python 3.6+ simply installating the latest version of MSVC build tools should 
+For Python 3.6+ simply installing the latest version of MSVC build tools should 
 be sufficient. Note that wheels found via pip do not include MKL support. Wheels 
 available via `conda` will have MKL, if the MKL backend is used for NumPy.
 
 See `requirements.txt` for the required version of NumPy.
 
 NumExpr is built in the standard Python way::
 
@@ -141,15 +142,15 @@
 Do not test NumExpr in the source directory or you will generate import errors.
 
 Enable Intel® MKL support
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 NumExpr includes support for Intel's MKL library. This may provide better 
 performance on Intel architectures, mainly when evaluating transcendental 
-functions (trigonometrical, exponential...). 
+functions (trigonometrical, exponential, ...). 
 
 If you have Intel's MKL, copy the `site.cfg.example` that comes with the 
 distribution to `site.cfg` and edit the latter file to provide correct paths to 
 the MKL libraries in your system.  After doing this, you can proceed with the 
 usual building instructions listed above.
 
 Pay attention to the messages during the building process in order to know
```

### Comparing `numexpr-2.8.3/README.rst` & `numexpr-2.8.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 constants in the expression are also chunked. Chunks are distributed among 
 the available cores of the CPU, resulting in highly parallelized code 
 execution.
 
 The result is that NumExpr can get the most of your machine computing
 capabilities for array-wise computations. Common speed-ups with regard
 to NumPy are usually between 0.95x (for very simple expressions like
-:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a >
-2.5*b'`), although much higher speed-ups can be achieved for some functions 
-and complex math operations (up to 15x in some cases).
+:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a > 2.5*b'`), 
+although much higher speed-ups can be achieved for some functions  and complex 
+math operations (up to 15x in some cases).
 
 NumExpr performs best on matrices that are too large to fit in L1 CPU cache. 
 In order to get a better idea on the different speed-ups that can be achieved 
 on your platform, run the provided benchmarks.
 
 Installation
 ------------
@@ -84,25 +84,25 @@
 to use the `conda` package manager in this case::
 
     conda install numexpr
 
 From Source
 ^^^^^^^^^^^
 
-On most `Nix systems your compilers will already be present. However if you 
+On most \*nix systems your compilers will already be present. However if you 
 are using a virtual environment with a substantially newer version of Python than
 your system Python you may be prompted to install a new version of `gcc` or `clang`.
 
 For Windows, you will need to install the Microsoft Visual C++ Build Tools 
-(which are free) first.The version depends on which version of Python you have 
+(which are free) first. The version depends on which version of Python you have 
 installed:
 
 https://wiki.python.org/moin/WindowsCompilers
 
-For Python 3.6+ simply installating the latest version of MSVC build tools should 
+For Python 3.6+ simply installing the latest version of MSVC build tools should 
 be sufficient. Note that wheels found via pip do not include MKL support. Wheels 
 available via `conda` will have MKL, if the MKL backend is used for NumPy.
 
 See `requirements.txt` for the required version of NumPy.
 
 NumExpr is built in the standard Python way::
 
@@ -115,15 +115,15 @@
 Do not test NumExpr in the source directory or you will generate import errors.
 
 Enable Intel® MKL support
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 NumExpr includes support for Intel's MKL library. This may provide better 
 performance on Intel architectures, mainly when evaluating transcendental 
-functions (trigonometrical, exponential...). 
+functions (trigonometrical, exponential, ...). 
 
 If you have Intel's MKL, copy the `site.cfg.example` that comes with the 
 distribution to `site.cfg` and edit the latter file to provide correct paths to 
 the MKL libraries in your system.  After doing this, you can proceed with the 
 usual building instructions listed above.
 
 Pay attention to the messages during the building process in order to know
```

### Comparing `numexpr-2.8.3/RELEASE_NOTES.rst` & `numexpr-2.8.4/RELEASE_NOTES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 ====================================
 Release notes for NumExpr 2.8 series
 ====================================
 
+Changes from 2.8.3 to 2.8.4
+---------------------------
+
+* Support for Python 3.11 has been added.
+* Thanks to Tobias Hangleiter for an improved accuracy complex `expm1` function.
+  While it is 25 % slower, it is significantly more accurate for the real component
+  over a range of values and matches NumPy outputs much more closely.
+* Thanks to Kirill Kouzoubov for a range of fixes to constants parsing that was 
+  resulting in duplicated constants of the same value.
+* Thanks to Mark Harfouche for noticing that we no longer need `numpy` version 
+  checks. `packaging` is no longer a requirement as a result.
+
 Changes from 2.8.1 to 2.8.3
 ---------------------------
 
 * 2.8.2 was skipped due to an error in uploading to PyPi.
 * Support for Python 3.6 has been dropped due to the need to substitute the flag 
   `NPY_ARRAY_WRITEBACKIFCOPY` for `NPY_ARRAY_UPDATEIFCOPY`. This flag change was 
   initiated in NumPy 1.14 and finalized in 1.23. The only changes were made to
```

### Comparing `numexpr-2.8.3/bench/boolean_timing.py` & `numexpr-2.8.4/bench/boolean_timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/issue-36.py` & `numexpr-2.8.4/bench/issue-36.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/multidim.py` & `numexpr-2.8.4/bench/multidim.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/poly.py` & `numexpr-2.8.4/bench/poly.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/timing.py` & `numexpr-2.8.4/bench/timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/unaligned-simple.py` & `numexpr-2.8.4/bench/unaligned-simple.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/varying-expr.py` & `numexpr-2.8.4/bench/varying-expr.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/vml_timing.py` & `numexpr-2.8.4/bench/vml_timing.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/bench/vml_timing2.py` & `numexpr-2.8.4/bench/vml_timing2.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/__init__.py` & `numexpr-2.8.4/numexpr/__init__.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/complex_functions.hpp` & `numexpr-2.8.4/numexpr/complex_functions.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,18 @@
     r->imag = a*sin(x->imag);
     return;
 }
 
 static void
 nc_expm1(npy_cdouble *x, npy_cdouble *r)
 {
-    double a = exp(x->real);
-    r->real = a*cos(x->imag) - 1.0;
-    r->imag = a*sin(x->imag);
+    double a = sin(x->imag / 2);
+    double b = exp(x->real);
+    r->real = expm1(x->real) * cos(x->imag) - 2 * a * a;
+    r->imag = b * sin(x->imag);
     return;
 }
 
 static void
 nc_pow(npy_cdouble *a, npy_cdouble *b, npy_cdouble *r)
 {
     npy_intp n;
```

### Comparing `numexpr-2.8.3/numexpr/cpuinfo.py` & `numexpr-2.8.4/numexpr/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/expressions.py` & `numexpr-2.8.4/numexpr/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 __all__ = ['E']
 
 import operator
 import sys
 import threading
 
 import numpy
-# NumPy's behavior sometimes changes with versioning, especially in regard as 
-# to when ints are cast to floats.
-from packaging.version import parse, Version
-_np_version_forbids_neg_powint = parse(numpy.__version__) > Version('1.12.0b1')
 
 # Declare a double type that does not exist in Python space
 double = numpy.double
 
 # The default kind for undeclared variables
 default_kind = 'double'
 int_ = numpy.int32
@@ -138,29 +134,31 @@
     if isinstance(x, (long_, numpy.int64)):
         return long_
     # ``double`` objects are kept as is to allow the user to force
     # promotion of results by using double constants, e.g. by operating
     # a float (32-bit) array with a double (64-bit) constant.
     if isinstance(x, double):
         return double
+    if isinstance(x, numpy.float32):
+        return float
     if isinstance(x, (int, numpy.integer)):
         # Constants needing more than 32 bits are always
         # considered ``long``, *regardless of the platform*, so we
         # can clearly tell 32- and 64-bit constants apart.
         if not (min_int32 <= x <= max_int32):
             return long_
         return int_
     # The duality of float and double in Python avoids that we have to list
     # ``double`` too.
     for converter in float, complex:
         try:
             y = converter(x)
         except Exception as err:
             continue
-        if y == x:
+        if y == x or numpy.isnan(y):
             return converter
 
 
 def getKind(x):
     converter = bestConstantType(x)
     return type_to_kind[converter]
 
@@ -269,16 +267,15 @@
 @ophelper
 def rtruediv_op(a, b):
     return truediv_op(b, a)
 
 
 @ophelper
 def pow_op(a, b):
-    if (_np_version_forbids_neg_powint and
-        b.astKind in ('int', 'long') and
+    if (b.astKind in ('int', 'long') and
         a.astKind in ('int', 'long') and
         numpy.any(b.value < 0)):
 
         raise ValueError(
             'Integers to negative integer powers are not allowed.')
 
     if allConstantNodes([a, b]):
@@ -329,14 +326,15 @@
             if x == 1:
                 return a
             if x == 2:
                 return OpNode('mul', [a, a])
     return OpNode('pow', [a, b])
 
 # The functions and the minimum and maximum types accepted
+numpy.expm1x = numpy.expm1
 functions = {
     'copy': func(numpy.copy),
     'ones_like': func(numpy.ones_like),
     'sqrt': func(numpy.sqrt, 'float'),
 
     'sin': func(numpy.sin, 'float'),
     'cos': func(numpy.cos, 'float'),
@@ -500,15 +498,15 @@
 
 class ConstantNode(LeafNode):
     astType = 'constant'
 
     def __init__(self, value=None, children=None):
         kind = getKind(value)
         # Python float constants are double precision by default
-        if kind == 'float':
+        if kind == 'float' and isinstance(value, float):
             kind = 'double'
         LeafNode.__init__(self, value=value, kind=kind)
 
     def __neg__(self):
         return ConstantNode(-self.value)
 
     def __invert__(self):
```

### Comparing `numexpr-2.8.3/numexpr/functions.hpp` & `numexpr-2.8.4/numexpr/functions.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -98,35 +98,35 @@
 #undef FUNC_DDD
 #endif
 
 #ifndef FUNC_CC
 #define ELIDE_FUNC_CC
 #define FUNC_CC(...)
 #endif
-FUNC_CC(FUNC_SQRT_CC,    "sqrt_cc",     nc_sqrt,  vzSqrt)
-FUNC_CC(FUNC_SIN_CC,     "sin_cc",      nc_sin,   vzSin)
-FUNC_CC(FUNC_COS_CC,     "cos_cc",      nc_cos,   vzCos)
-FUNC_CC(FUNC_TAN_CC,     "tan_cc",      nc_tan,   vzTan)
-FUNC_CC(FUNC_ARCSIN_CC,  "arcsin_cc",   nc_asin,  vzAsin)
-FUNC_CC(FUNC_ARCCOS_CC,  "arccos_cc",   nc_acos,  vzAcos)
-FUNC_CC(FUNC_ARCTAN_CC,  "arctan_cc",   nc_atan,  vzAtan)
-FUNC_CC(FUNC_SINH_CC,    "sinh_cc",     nc_sinh,  vzSinh)
-FUNC_CC(FUNC_COSH_CC,    "cosh_cc",     nc_cosh,  vzCosh)
-FUNC_CC(FUNC_TANH_CC,    "tanh_cc",     nc_tanh,  vzTanh)
-FUNC_CC(FUNC_ARCSINH_CC, "arcsinh_cc",  nc_asinh, vzAsinh)
-FUNC_CC(FUNC_ARCCOSH_CC, "arccosh_cc",  nc_acosh, vzAcosh)
-FUNC_CC(FUNC_ARCTANH_CC, "arctanh_cc",  nc_atanh, vzAtanh)
-FUNC_CC(FUNC_LOG_CC,     "log_cc",      nc_log,   vzLn)
-FUNC_CC(FUNC_LOG1P_CC,   "log1p_cc",    nc_log1p, vzLog1p)
-FUNC_CC(FUNC_LOG10_CC,   "log10_cc",    nc_log10, vzLog10)
-FUNC_CC(FUNC_EXP_CC,     "exp_cc",      nc_exp,   vzExp)
-FUNC_CC(FUNC_EXPM1_CC,   "expm1_cc",    nc_expm1, vzExpm1)
-FUNC_CC(FUNC_ABS_CC,     "absolute_cc", nc_abs,   vzAbs_)
-FUNC_CC(FUNC_CONJ_CC,    "conjugate_cc",nc_conj,  vzConj)
-FUNC_CC(FUNC_CC_LAST,    NULL,          NULL,     NULL)
+FUNC_CC(FUNC_SQRT_CC,    "sqrt_cc",     nc_sqrt,   vzSqrt)
+FUNC_CC(FUNC_SIN_CC,     "sin_cc",      nc_sin,    vzSin)
+FUNC_CC(FUNC_COS_CC,     "cos_cc",      nc_cos,    vzCos)
+FUNC_CC(FUNC_TAN_CC,     "tan_cc",      nc_tan,    vzTan)
+FUNC_CC(FUNC_ARCSIN_CC,  "arcsin_cc",   nc_asin,   vzAsin)
+FUNC_CC(FUNC_ARCCOS_CC,  "arccos_cc",   nc_acos,   vzAcos)
+FUNC_CC(FUNC_ARCTAN_CC,  "arctan_cc",   nc_atan,   vzAtan)
+FUNC_CC(FUNC_SINH_CC,    "sinh_cc",     nc_sinh,   vzSinh)
+FUNC_CC(FUNC_COSH_CC,    "cosh_cc",     nc_cosh,   vzCosh)
+FUNC_CC(FUNC_TANH_CC,    "tanh_cc",     nc_tanh,   vzTanh)
+FUNC_CC(FUNC_ARCSINH_CC, "arcsinh_cc",  nc_asinh,  vzAsinh)
+FUNC_CC(FUNC_ARCCOSH_CC, "arccosh_cc",  nc_acosh,  vzAcosh)
+FUNC_CC(FUNC_ARCTANH_CC, "arctanh_cc",  nc_atanh,  vzAtanh)
+FUNC_CC(FUNC_LOG_CC,     "log_cc",      nc_log,    vzLn)
+FUNC_CC(FUNC_LOG1P_CC,   "log1p_cc",    nc_log1p,  vzLog1p)
+FUNC_CC(FUNC_LOG10_CC,   "log10_cc",    nc_log10,  vzLog10)
+FUNC_CC(FUNC_EXP_CC,     "exp_cc",      nc_exp,    vzExp)
+FUNC_CC(FUNC_EXPM1_CC,   "expm1_cc",    nc_expm1,  vzExpm1)
+FUNC_CC(FUNC_ABS_CC,     "absolute_cc", nc_abs,    vzAbs_)
+FUNC_CC(FUNC_CONJ_CC,    "conjugate_cc",nc_conj,   vzConj)
+FUNC_CC(FUNC_CC_LAST,    NULL,          NULL,      NULL)
 #ifdef ELIDE_FUNC_CC
 #undef ELIDE_FUNC_CC
 #undef FUNC_CC
 #endif
 
 #ifndef FUNC_CCC
 #define ELIDE_FUNC_CCC
```

### Comparing `numexpr-2.8.3/numexpr/interp_body.cpp` & `numexpr-2.8.4/numexpr/interp_body.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/interpreter.cpp` & `numexpr-2.8.4/numexpr/interpreter.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -257,24 +257,24 @@
 #ifdef USE_VML
 /* complex expm1 not available in VML */
 static void vzExpm1(MKL_INT n, const MKL_Complex16* x1, MKL_Complex16* dest)
 {
     MKL_INT j;
     vzExp(n, x1, dest);
     for (j=0; j<n; j++) {
-    dest[j].real -= 1.0;
+        dest[j].real -= 1.0;
     };
 };
 
 static void vzLog1p(MKL_INT n, const MKL_Complex16* x1, MKL_Complex16* dest)
 {
     MKL_INT j;
     for (j=0; j<n; j++) {
-    dest[j].real = x1[j].real + 1;
-    dest[j].imag = x1[j].imag;
+        dest[j].real = x1[j].real + 1;
+        dest[j].imag = x1[j].imag;
     };
     vzLn(n, dest, dest);
 };
 
 /* Use this instead of native vzAbs in VML as it seems to work badly */
 static void vzAbs_(MKL_INT n, const MKL_Complex16* x1, MKL_Complex16* dest)
 {
```

### Comparing `numexpr-2.8.3/numexpr/interpreter.hpp` & `numexpr-2.8.4/numexpr/interpreter.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/missing_posix_functions.hpp` & `numexpr-2.8.4/numexpr/missing_posix_functions.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/module.cpp` & `numexpr-2.8.4/numexpr/module.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/module.hpp` & `numexpr-2.8.4/numexpr/module.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/msvc_function_stubs.hpp` & `numexpr-2.8.4/numexpr/msvc_function_stubs.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/necompiler.py` & `numexpr-2.8.4/numexpr/necompiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,16 @@
     RAM: implemented magic method __lt__ for ASTNode to fix issues
     #88 and #209. The following test code works now, as does the test suite.
 
         import numexpr as ne
         a = 1 + 3j; b = 5.0
         ne.evaluate('a*2 + 15j - b')
     """
-    constants_order = sorted(ast.allOf('constant'))
+    constant_registers = set([node.reg for node in ast.allOf("constant")]) 
+    constants_order = sorted([r.node for r in constant_registers])
     constants = [convertConstantToKind(a.value, a.astKind)
                  for a in constants_order]
     return constants_order, constants
 
 
 def sortNodesByOrder(nodes, order):
     order_map = {}
@@ -631,19 +632,23 @@
     """
     rev_opcodes = {}
     for op in interpreter.opcodes:
         rev_opcodes[interpreter.opcodes[op]] = op
     r_constants = 1 + len(nex.signature)
     r_temps = r_constants + len(nex.constants)
 
+    def parseOp(op):
+        name, sig = [*op.rsplit(b'_', 1), ''][:2]
+        return name, sig 
+
     def getArg(pc, offset):
-        arg = nex.program[pc + offset]
-        op = rev_opcodes.get(nex.program[pc])
+        arg = nex.program[pc + (offset if offset < 4 else offset+1)]
+        _, sig = parseOp(rev_opcodes.get(nex.program[pc]))
         try:
-            code = op.split(b'_')[1][offset - 1]
+            code = sig[offset - 1]
         except IndexError:
             return None
 
         code = bytes([code])
 
         if arg == 255:
             return None
@@ -658,18 +663,21 @@
                 return ('t%d' % (arg,)).encode('ascii')
         else:
             return arg
 
     source = []
     for pc in range(0, len(nex.program), 4):
         op = rev_opcodes.get(nex.program[pc])
-        dest = getArg(pc, 1)
-        arg1 = getArg(pc, 2)
-        arg2 = getArg(pc, 3)
-        source.append((op, dest, arg1, arg2))
+        _, sig = parseOp(op)
+        parsed = [op]
+        for i in range(len(sig)):
+            parsed.append(getArg(pc, 1 + i))
+        while len(parsed) < 4:
+            parsed.append(None)
+        source.append(parsed)
     return source
 
 
 def getType(a):
     kind = a.dtype.kind
     if kind == 'b':
         return bool
```

### Comparing `numexpr-2.8.3/numexpr/numexpr_config.hpp` & `numexpr-2.8.4/numexpr/numexpr_config.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/numexpr_object.cpp` & `numexpr-2.8.4/numexpr/numexpr_object.cpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/numexpr_object.hpp` & `numexpr-2.8.4/numexpr/numexpr_object.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/opcodes.hpp` & `numexpr-2.8.4/numexpr/opcodes.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/str-two-way.hpp` & `numexpr-2.8.4/numexpr/str-two-way.hpp`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/tests/test_numexpr.py` & `numexpr-2.8.4/numexpr/tests/test_numexpr.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,30 @@
 from numpy import (
     array, arange, empty, zeros, int32, int64, uint16, complex_, float64, rec,
     copy, ones_like, where, alltrue, linspace,
     sum, prod, sqrt, fmod, floor, ceil,
     sin, cos, tan, arcsin, arccos, arctan, arctan2,
     sinh, cosh, tanh, arcsinh, arccosh, arctanh,
     log, log1p, log10, exp, expm1, conj)
+import numpy
 from numpy.testing import (assert_equal, assert_array_equal,
                            assert_array_almost_equal, assert_allclose)
 from numpy import shape, allclose, array_equal, ravel, isnan, isinf
 
 import numexpr
 from numexpr import E, NumExpr, evaluate, re_evaluate, disassemble, use_vml
+from numexpr.expressions import ConstantNode
 
 import unittest
 
 TestCase = unittest.TestCase
 
 double = np.double
 long = int
 
-# Recommended minimum versions
-from packaging.version import Version
-minimum_numpy_version = Version('1.7.0')
-present_numpy_version = Version(np.__version__)
 
 class test_numexpr(TestCase):
     """Testing with 1 thread"""
     nthreads = 1
 
     def setUp(self):
         numexpr.set_num_threads(self.nthreads)
@@ -477,14 +475,39 @@
         try:
             evaluate("a < [0, 0, 0]")
         except TypeError:
             pass
         else:
             self.fail()
 
+    def test_disassemble(self):
+        assert_equal(disassemble(NumExpr(
+            "where(m, a, -1)", [('m', bool), ('a', float)])),
+            [[b'where_fbff', b'r0', b'r1[m]', b'r2[a]', b'c3[-1.0]'], 
+             [b'noop', None, None, None]])
+
+    def test_constant_deduplication(self):
+        assert_equal(NumExpr("(a + 1)*(a - 1)", [('a', np.int32)]).constants, (1,))
+
+    def test_nan_constant(self):
+        assert_equal(str(ConstantNode(float("nan")).value), 'nan')
+
+        # check de-duplication works for nan
+        _nan = ConstantNode(float("nan"))
+        expr = (E.a + _nan)*(E.b + _nan)
+        assert_equal(NumExpr(expr, [('a', double), ('b', double)]).constants, (float("nan"),))
+
+
+    def test_f32_constant(self):
+        assert_equal(ConstantNode(numpy.float32(1)).astKind, "float")
+        assert_equal(ConstantNode(numpy.float32("nan")).astKind, "float")
+        assert_equal(ConstantNode(numpy.float32(3)).value.dtype, numpy.dtype("float32"))
+        assert_array_equal(NumExpr(ConstantNode(numpy.float32(1))).run(), 
+                           numpy.array(1, dtype="float32"))
+
     def test_unaligned_singleton(self):
         # Test for issue #397 whether singletons outputs assigned to consts must be 
         # aligned or not.
         a = np.empty(5, dtype=np.uint8)[1:].view(np.int32)
         evaluate('3', out=a)
         assert_equal(a, 3)
 
@@ -797,22 +820,17 @@
     str_array2 = array(str_list2 * str_nloops)
     str_constant = b'doodoo'
 
     def test_null_chars(self):
         str_list = [
             b'\0\0\0', b'\0\0foo\0', b'\0\0foo\0b', b'\0\0foo\0b\0',
             b'foo\0', b'foo\0b', b'foo\0b\0', b'foo\0bar\0baz\0\0']
-        min_tobytes_version = Version('1.9.0')
         for s in str_list:
             r = evaluate('s')
-            if present_numpy_version >= min_tobytes_version:
-                self.assertEqual(s, r.tobytes())  # check *all* stored data
-            else:
-                # ndarray.tostring() is deprecated as of NumPy 1.19
-                self.assertEqual(s, r.tostring())  # check *all* stored data
+            self.assertEqual(s, r.tobytes())  # check *all* stored data
 
     def test_compare_copy(self):
         sarr = self.str_array1
         expr = 'sarr'
         res1 = eval(expr)
         res2 = evaluate(expr)
         assert_array_equal(res1, res2)
@@ -1071,18 +1089,14 @@
 
 def print_versions():
     """Print the versions of software that numexpr relies on."""
     # from pkg_resources import parse_version
     from numexpr.cpuinfo import cpu
     import platform
 
-    np_version = Version(np.__version__)
-
-    if np_version < minimum_numpy_version:
-        print('*Warning*: NumPy version is lower than recommended: %s < %s' % (np_version, minimum_numpy_version))
     print('-=' * 38)
     print('Numexpr version:   %s' % numexpr.__version__)
     print('NumPy version:     %s' % np.__version__)
     print('Python version:    %s' % sys.version)
     (sysname, nodename, release, os_version, machine, processor) = platform.uname()
     print('Platform:          %s-%s-%s' % (sys.platform, machine, os_version))
     try:
```

### Comparing `numexpr-2.8.3/numexpr/utils.py` & `numexpr-2.8.4/numexpr/utils.py`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/win32/pthread.c` & `numexpr-2.8.4/numexpr/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/win32/pthread.h` & `numexpr-2.8.4/numexpr/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr/win32/stdint.h` & `numexpr-2.8.4/numexpr/win32/stdint.h`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/numexpr.egg-info/PKG-INFO` & `numexpr-2.8.4/numexpr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numexpr
-Version: 2.8.3
+Version: 2.8.4
 Summary: Fast numerical expression evaluator for NumPy
 Home-page: https://github.com/pydata/numexpr
 Author: David M. Cooke, Francesc Alted, and others
 Maintainer: Robert A. McLeod
 Maintainer-email: robbmcleod@gmail.com
 License: MIT
 Classifier: Development Status :: 6 - Mature
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
@@ -82,17 +83,17 @@
 constants in the expression are also chunked. Chunks are distributed among 
 the available cores of the CPU, resulting in highly parallelized code 
 execution.
 
 The result is that NumExpr can get the most of your machine computing
 capabilities for array-wise computations. Common speed-ups with regard
 to NumPy are usually between 0.95x (for very simple expressions like
-:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a >
-2.5*b'`), although much higher speed-ups can be achieved for some functions 
-and complex math operations (up to 15x in some cases).
+:code:`'a + 1'`) and 4x (for relatively complex ones like :code:`'a*b-4.1*a > 2.5*b'`), 
+although much higher speed-ups can be achieved for some functions  and complex 
+math operations (up to 15x in some cases).
 
 NumExpr performs best on matrices that are too large to fit in L1 CPU cache. 
 In order to get a better idea on the different speed-ups that can be achieved 
 on your platform, run the provided benchmarks.
 
 Installation
 ------------
@@ -110,25 +111,25 @@
 to use the `conda` package manager in this case::
 
     conda install numexpr
 
 From Source
 ^^^^^^^^^^^
 
-On most `Nix systems your compilers will already be present. However if you 
+On most \*nix systems your compilers will already be present. However if you 
 are using a virtual environment with a substantially newer version of Python than
 your system Python you may be prompted to install a new version of `gcc` or `clang`.
 
 For Windows, you will need to install the Microsoft Visual C++ Build Tools 
-(which are free) first.The version depends on which version of Python you have 
+(which are free) first. The version depends on which version of Python you have 
 installed:
 
 https://wiki.python.org/moin/WindowsCompilers
 
-For Python 3.6+ simply installating the latest version of MSVC build tools should 
+For Python 3.6+ simply installing the latest version of MSVC build tools should 
 be sufficient. Note that wheels found via pip do not include MKL support. Wheels 
 available via `conda` will have MKL, if the MKL backend is used for NumPy.
 
 See `requirements.txt` for the required version of NumPy.
 
 NumExpr is built in the standard Python way::
 
@@ -141,15 +142,15 @@
 Do not test NumExpr in the source directory or you will generate import errors.
 
 Enable Intel® MKL support
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 NumExpr includes support for Intel's MKL library. This may provide better 
 performance on Intel architectures, mainly when evaluating transcendental 
-functions (trigonometrical, exponential...). 
+functions (trigonometrical, exponential, ...). 
 
 If you have Intel's MKL, copy the `site.cfg.example` that comes with the 
 distribution to `site.cfg` and edit the latter file to provide correct paths to 
 the MKL libraries in your system.  After doing this, you can proceed with the 
 usual building instructions listed above.
 
 Pay attention to the messages during the building process in order to know
```

### Comparing `numexpr-2.8.3/numexpr.egg-info/SOURCES.txt` & `numexpr-2.8.4/numexpr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numexpr-2.8.3/setup.cfg` & `numexpr-2.8.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 756d 6578 7072 0d0a 7665 7273   = numexpr..vers
-00000020: 696f 6e20 3d20 322e 382e 330d 0a64 6573  ion = 2.8.3..des
+00000020: 696f 6e20 3d20 322e 382e 340d 0a64 6573  ion = 2.8.4..des
 00000030: 6372 6970 7469 6f6e 203d 2046 6173 7420  cription = Fast 
 00000040: 6e75 6d65 7269 6361 6c20 6578 7072 6573  numerical expres
 00000050: 7369 6f6e 2065 7661 6c75 6174 6f72 2066  sion evaluator f
 00000060: 6f72 204e 756d 5079 0d0a 6175 7468 6f72  or NumPy..author
 00000070: 203d 2044 6176 6964 204d 2e20 436f 6f6b   = David M. Cook
 00000080: 652c 2046 7261 6e63 6573 6320 416c 7465  e, Francesc Alte
 00000090: 642c 2061 6e64 206f 7468 6572 730d 0a6d  d, and others..m
@@ -41,21 +41,24 @@
 00000280: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000290: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
 000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
 000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 000002c0: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
 000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002f0: 300d 0a09 4f70 6572 6174 696e 6720 5379  0...Operating Sy
-00000300: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
-00000310: 7420 3a3a 2057 696e 646f 7773 0d0a 094f  t :: Windows...O
-00000320: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000330: 3a3a 2050 4f53 4958 0d0a 094f 7065 7261  :: POSIX...Opera
-00000340: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000350: 6163 4f53 0d0a 0d0a 5b6f 7074 696f 6e73  acOS....[options
-00000360: 5d0d 0a7a 6970 5f73 6166 6520 3d20 4661  ]..zip_safe = Fa
-00000370: 6c73 650d 0a70 6163 6b61 6765 7320 3d20  lse..packages = 
-00000380: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000390: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
-000003a0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000003b0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000003c0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000002f0: 300d 0a09 5072 6f67 7261 6d6d 696e 6720  0...Programming 
+00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000310: 6f6e 203a 3a20 332e 3131 0d0a 094f 7065  on :: 3.11...Ope
+00000320: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000330: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
+00000340: 6e64 6f77 730d 0a09 4f70 6572 6174 696e  ndows...Operatin
+00000350: 6720 5379 7374 656d 203a 3a20 504f 5349  g System :: POSI
+00000360: 580d 0a09 4f70 6572 6174 696e 6720 5379  X...Operating Sy
+00000370: 7374 656d 203a 3a20 4d61 634f 530d 0a0d  stem :: MacOS...
+00000380: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
+00000390: 7361 6665 203d 2046 616c 7365 0d0a 7061  safe = False..pa
+000003a0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+000003b0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+000003c0: 3d20 3e3d 332e 370d 0a0d 0a5b 6567 675f  = >=3.7....[egg_
+000003d0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000003e0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000003f0: 300d 0a0d 0a                             0....
```

### Comparing `numexpr-2.8.3/setup.py` & `numexpr-2.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         inc_dirs.extend(
             site['mkl']['include_dirs'].split(os.pathsep))
         lib_dirs.extend(
             site['mkl']['library_dirs'].split(os.pathsep))
         libs.extend(
             site['mkl']['libraries'].split(os.pathsep))
         def_macros.append(('USE_VML', None))
+        print(f'FOUND MKL IMPORT')
         
 
 def setup_package():
 
     parse_site_cfg()
 
     numexpr_extension = Extension(
```

### Comparing `numexpr-2.8.3/site.cfg.example` & `numexpr-2.8.4/site.cfg.example`

 * *Files identical despite different names*

