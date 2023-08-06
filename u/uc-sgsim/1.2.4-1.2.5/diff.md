# Comparing `tmp/uc_sgsim-1.2.4.tar.gz` & `tmp/uc_sgsim-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_sgsim-1.2.4.tar", last modified: Mon Jun 26 09:29:38 2023, max compression
+gzip compressed data, was "uc_sgsim-1.2.5.tar", last modified: Sun Aug  6 05:44:45 2023, max compression
```

## Comparing `uc_sgsim-1.2.4.tar` & `uc_sgsim-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.183245 uc_sgsim-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-06-26 09:29:38.183245 uc_sgsim-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-26 09:29:38.183245 uc_sgsim-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.175245 uc_sgsim-1.2.4/uc_sgsim/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.179245 uc_sgsim-1.2.4/uc_sgsim/c_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/c_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85094 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/c_core/uc_sgsim.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    37152 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/c_core/uc_sgsim.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.179245 uc_sgsim-1.2.4/uc_sgsim/cov_model/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/cov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/cov_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/cov_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.179245 uc_sgsim-1.2.4/uc_sgsim/kriging/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/kriging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/kriging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/kriging/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.179245 uc_sgsim-1.2.4/uc_sgsim/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/random_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/sgsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-26 09:29:24.000000 uc_sgsim-1.2.4/uc_sgsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:29:38.179245 uc_sgsim-1.2.4/uc_sgsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 09:29:38.000000 uc_sgsim-1.2.4/uc_sgsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 05:44:45.386345 uc_sgsim-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.378344 uc_sgsim-1.2.5/uc_sgsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/uc_sgsim/c_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/c_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84596 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/c_core/uc_sgsim.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37008 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/c_core/uc_sgsim.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/uc_sgsim/cov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/cov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/cov_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/cov_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/uc_sgsim/kriging/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/kriging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/kriging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/kriging/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.382345 uc_sgsim-1.2.5/uc_sgsim/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/plotting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/plotting/sgsim_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/random_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/sgsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-06 05:44:35.000000 uc_sgsim-1.2.5/uc_sgsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:44:45.378344 uc_sgsim-1.2.5/uc_sgsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-06 05:44:45.000000 uc_sgsim-1.2.5/uc_sgsim.egg-info/top_level.txt
```

### Comparing `uc_sgsim-1.2.4/LICENSE.md` & `uc_sgsim-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.4/PKG-INFO` & `uc_sgsim-1.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: uc_sgsim
-Version: 1.2.4
-Summary: Random Field Generation
-Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
-Author: Zncl2222
-Author-email: 3002shinning@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=c%2B%2B)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=python)
 [![ci](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml)
@@ -105,15 +84,15 @@
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
 * Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-## Example
+## Examples
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
@@ -128,14 +107,22 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
+    # You could also set z_min, z_max and max_neighbor for sgsim by key words
+    # sgsim = uc.UCSgsimDLL(x, nR, cov_model, z_min=-6, z_max=6, max_neigh=10)
+    # set z_min, z_max and max_neighbor by directly assign
+    # sgsim.z_min = -6
+    # sgsim.z_max = 6
+    # sgsim.max_neigh = 10
+
+    # Create simulation with default z_min, z_max and max_neigh params
     sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
     sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
@@ -159,14 +146,56 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
+If you would like to use pure C to run this code, you can modify the c_example.c file in this root directory. After modifying the c_example.c file, run ```sh cmake_build.sh``` on Linux or ```cmake_build.bat``` on Windows to compile and execute the code.
+
+```c
+// c_example.c
+# include <stdio.h>
+# include <stdlib.h>
+
+# include "./uc_sgsim/c_core/include/sgsim.h"
+# include "./uc_sgsim/c_core/include/cov_model.h"
+# if defined(__linux__) || defined(__unix__)
+# define PAUSE printf("Press Enter key to continue..."); fgetc(stdin);//NOLINT
+# elif _WIN32
+# define PAUSE system("PAUSE");
+# endif
+
+int main() {
+    // you can also set z_min and z_max at sgsim_t. Default value will depend on
+    // sill value in cov_model_t
+    sgsim_t sgsim_example = {
+        .x_len = 150,
+        .realization_numbers = 5,
+        .randomseed = 12345,
+        .kriging_method = 1,
+        .if_alloc_memory = 1,  // This should be equal to 1 if you want to run by c.
+    };
+
+    // you can also set max_negibor at cov_model_t. Defualt value is 4.
+    cov_model_t cov_example = {
+        .bw_l = 35,
+        .bw_s = 1,
+        .k_range = 17.32,
+        .sill = 1,
+        .nugget = 0,
+    };
+
+    sgsim_run(&sgsim_example, &cov_example, 0);
+    sgsim_t_free(&sgsim_example);
+    PAUSE
+    return 0;
+}
+```
+
 ## Future plans
 * 2D unconditional randomfield generation
 * GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
```

### Comparing `uc_sgsim-1.2.4/README.md` & `uc_sgsim-1.2.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: uc_sgsim
+Version: 1.2.5
+Summary: Random Field Generation
+Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
+Author: Zncl2222
+Author-email: 3002shinning@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 ![licence](https://img.shields.io/github/license/Zncl2222/Stochastic_UC_SGSIM)
 ![python](https://img.shields.io/pypi/pyversions/uc-sgsim)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=c%2B%2B)
 ![language](https://img.shields.io/badge/Solutions-black.svg?style=flat&logo=python)
 [![ci](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/github-pre-commit.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/cmake.yml)
 [![build](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml/badge.svg)](https://github.com/Zncl2222/Stochastic_UC_SGSIM/actions/workflows/codeql.yml)
@@ -84,15 +105,15 @@
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
 * Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-## Example
+## Examples
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
@@ -107,14 +128,22 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
+    # You could also set z_min, z_max and max_neighbor for sgsim by key words
+    # sgsim = uc.UCSgsimDLL(x, nR, cov_model, z_min=-6, z_max=6, max_neigh=10)
+    # set z_min, z_max and max_neighbor by directly assign
+    # sgsim.z_min = -6
+    # sgsim.z_max = 6
+    # sgsim.max_neigh = 10
+
+    # Create simulation with default z_min, z_max and max_neigh params
     sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
     sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
@@ -138,14 +167,56 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
+If you would like to use pure C to run this code, you can modify the c_example.c file in this root directory. After modifying the c_example.c file, run ```sh cmake_build.sh``` on Linux or ```cmake_build.bat``` on Windows to compile and execute the code.
+
+```c
+// c_example.c
+# include <stdio.h>
+# include <stdlib.h>
+
+# include "./uc_sgsim/c_core/include/sgsim.h"
+# include "./uc_sgsim/c_core/include/cov_model.h"
+# if defined(__linux__) || defined(__unix__)
+# define PAUSE printf("Press Enter key to continue..."); fgetc(stdin);//NOLINT
+# elif _WIN32
+# define PAUSE system("PAUSE");
+# endif
+
+int main() {
+    // you can also set z_min and z_max at sgsim_t. Default value will depend on
+    // sill value in cov_model_t
+    sgsim_t sgsim_example = {
+        .x_len = 150,
+        .realization_numbers = 5,
+        .randomseed = 12345,
+        .kriging_method = 1,
+        .if_alloc_memory = 1,  // This should be equal to 1 if you want to run by c.
+    };
+
+    // you can also set max_negibor at cov_model_t. Defualt value is 4.
+    cov_model_t cov_example = {
+        .bw_l = 35,
+        .bw_s = 1,
+        .k_range = 17.32,
+        .sill = 1,
+        .nugget = 0,
+    };
+
+    sgsim_run(&sgsim_example, &cov_example, 0);
+    sgsim_t_free(&sgsim_example);
+    PAUSE
+    return 0;
+}
+```
+
 ## Future plans
 * 2D unconditional randomfield generation
 * GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
```

### Comparing `uc_sgsim-1.2.4/setup.cfg` & `uc_sgsim-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uc_sgsim
-version = 1.2.4
+version = 1.2.5
 description = Random Field Generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Zncl2222/Stochastic_UC_SGSIM
 author = Zncl2222
 author_email = 3002shinning@gmail.com
 license = MIT
@@ -21,15 +21,15 @@
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
 packages = 
 	uc_sgsim
 	uc_sgsim/cov_model
 	uc_sgsim/kriging
-	uc_sgsim/plot
+	uc_sgsim/plotting
 	uc_sgsim/c_core
 install_requires = 
 	matplotlib
 	numpy
 	scipy
 python_requires = >=3.9
 include_package_data = true
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/c_core/uc_sgsim.dll` & `uc_sgsim-1.2.5/uc_sgsim/c_core/uc_sgsim.dll`

 * *Files 8% similar despite different names*

#### objdump

```diff
@@ -5,20 +5,20 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Fri Jun 23 03:06:13 2023
+Time/Date		Sat Aug  5 08:27:55 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
-SizeOfCode		0000000000007000
-SizeOfInitializedData	0000000000009e00
+SizeOfCode		0000000000006e00
+SizeOfInitializedData	0000000000009c00
 SizeOfUninitializedData	0000000000000c00
 AddressOfEntryPoint	0000000000001330
 BaseOfCode		0000000000001000
 ImageBase		00000000646c0000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	4
@@ -26,35 +26,35 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00019000
 SizeOfHeaders		00000600
-CheckSum		0001a988
+CheckSum		0001cf9a
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
-Entry 0 000000000000d000 000006ab Export Directory [.edata (or where ever we found it)]
+Entry 0 000000000000d000 000006b9 Export Directory [.edata (or where ever we found it)]
 Entry 1 000000000000e000 00000720 Import Directory [parts of .idata]
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
 Entry 3 000000000000a000 000005ac Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 0000000000011000 00000064 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
-Entry 9 00000000000092a0 00000028 Thread Storage Directory [.tls]
+Entry 9 00000000000092c0 00000028 Thread Storage Directory [.tls]
 Entry a 0000000000000000 00000000 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 000000000000e1cc 00000190 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
@@ -124,28 +124,28 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x646cd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		64950c25
+Time/Date stamp 		64ce080b
 Major/Minor 			0/0
 Name 				000000000000d29e uc_sgsim.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000003f
 	[Name Pointer/Ordinal] Table	0000003f
 Table Addresses
 	Export Address Table 		000000000000d028
 	Name Pointer Table 		000000000000d124
 	Ordinal Table 			000000000000d220
 
 Export Address Table -- Ordinal Base 1
-	[   0] +base[   1] 47a0 Export RVA
+	[   0] +base[   1] 4630 Export RVA
 	[   1] +base[   2] 1630 Export RVA
 	[   2] +base[   3] 15c0 Export RVA
 	[   3] +base[   4] 13b0 Export RVA
 	[   4] +base[   5] 1540 Export RVA
 	[   5] +base[   6] 2060 Export RVA
 	[   6] +base[   7] 2040 Export RVA
 	[   7] +base[   8] 2000 Export RVA
@@ -166,48 +166,48 @@
 	[  22] +base[  23] 1ca0 Export RVA
 	[  23] +base[  24] 1be0 Export RVA
 	[  24] +base[  25] 1c40 Export RVA
 	[  25] +base[  26] 2370 Export RVA
 	[  26] +base[  27] 2340 Export RVA
 	[  27] +base[  28] 2320 Export RVA
 	[  28] +base[  29] 2330 Export RVA
-	[  29] +base[  30] 3450 Export RVA
-	[  30] +base[  31] 3510 Export RVA
-	[  31] +base[  32] 3420 Export RVA
-	[  32] +base[  33] 4830 Export RVA
-	[  33] +base[  34] 3850 Export RVA
-	[  34] +base[  35] 3ff0 Export RVA
-	[  35] +base[  36] 3690 Export RVA
-	[  36] +base[  37] 4120 Export RVA
-	[  37] +base[  38] 43b0 Export RVA
-	[  38] +base[  39] 3e80 Export RVA
-	[  39] +base[  40] 4a50 Export RVA
-	[  40] +base[  41] 23e0 Export RVA
-	[  41] +base[  42] 2e40 Export RVA
-	[  42] +base[  43] 30d0 Export RVA
-	[  43] +base[  44] 28f0 Export RVA
-	[  44] +base[  45] 2b80 Export RVA
-	[  45] +base[  46] 2660 Export RVA
-	[  46] +base[  47] 23a0 Export RVA
-	[  47] +base[  48] 3390 Export RVA
-	[  48] +base[  49] 5110 Export RVA
-	[  49] +base[  50] 4900 Export RVA
-	[  50] +base[  51] 5220 Export RVA
-	[  51] +base[  52] 5180 Export RVA
-	[  52] +base[  53] 4cc0 Export RVA
-	[  53] +base[  54] 3610 Export RVA
-	[  54] +base[  55] 3680 Export RVA
-	[  55] +base[  56] 4b40 Export RVA
-	[  56] +base[  57] 4d10 Export RVA
-	[  57] +base[  58] 4d70 Export RVA
-	[  58] +base[  59] 50e0 Export RVA
-	[  59] +base[  60] 3b10 Export RVA
-	[  60] +base[  61] 50f0 Export RVA
-	[  61] +base[  62] 54c0 Export RVA
-	[  62] +base[  63] 52e0 Export RVA
+	[  29] +base[  30] 3460 Export RVA
+	[  30] +base[  31] 3520 Export RVA
+	[  31] +base[  32] 46c0 Export RVA
+	[  32] +base[  33] 3870 Export RVA
+	[  33] +base[  34] 4010 Export RVA
+	[  34] +base[  35] 36a0 Export RVA
+	[  35] +base[  36] 4130 Export RVA
+	[  36] +base[  37] 43c0 Export RVA
+	[  37] +base[  38] 3ea0 Export RVA
+	[  38] +base[  39] 48e0 Export RVA
+	[  39] +base[  40] 23e0 Export RVA
+	[  40] +base[  41] 2e40 Export RVA
+	[  41] +base[  42] 30d0 Export RVA
+	[  42] +base[  43] 28f0 Export RVA
+	[  43] +base[  44] 2b80 Export RVA
+	[  44] +base[  45] 2660 Export RVA
+	[  45] +base[  46] 23a0 Export RVA
+	[  46] +base[  47] 3390 Export RVA
+	[  47] +base[  48] 5050 Export RVA
+	[  48] +base[  49] 4790 Export RVA
+	[  49] +base[  50] 5160 Export RVA
+	[  50] +base[  51] 50c0 Export RVA
+	[  51] +base[  52] 4b50 Export RVA
+	[  52] +base[  53] 3620 Export RVA
+	[  53] +base[  54] 3690 Export RVA
+	[  54] +base[  55] 49d0 Export RVA
+	[  55] +base[  56] 3420 Export RVA
+	[  56] +base[  57] 4ba0 Export RVA
+	[  57] +base[  58] 4c40 Export RVA
+	[  58] +base[  59] 5020 Export RVA
+	[  59] +base[  60] 3b30 Export RVA
+	[  60] +base[  61] 5030 Export RVA
+	[  61] +base[  62] 5400 Export RVA
+	[  62] +base[  63] 5220 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] arange
 	[   1] c_array_max_double
 	[   2] c_array_max_float
 	[   3] c_array_max_int
 	[   4] c_array_max_long_long
@@ -233,40 +233,40 @@
 	[  24] c_array_var_long_long
 	[  25] cmpfunc_double
 	[  26] cmpfunc_float
 	[  27] cmpfunc_int
 	[  28] cmpfunc_long
 	[  29] cov_model
 	[  30] cov_model2d
-	[  31] cov_model_init
-	[  32] d_arange
-	[  33] find_neighbor
-	[  34] kriging_memory_free
-	[  35] kriging_param_setting
-	[  36] lu_decomposition
-	[  37] lu_inverse_solver
-	[  38] matrix_agumented
-	[  39] matrixform
-	[  40] mt19937_generate
-	[  41] mt19937_get_double
-	[  42] mt19937_get_double_range
-	[  43] mt19937_get_float
-	[  44] mt19937_get_float_range
-	[  45] mt19937_get_int32_range
-	[  46] mt19937_init
-	[  47] mt19937_random_normal
-	[  48] partition2d
-	[  49] pdist
-	[  50] quickselect2d
-	[  51] quicksort2d
-	[  52] randompath
-	[  53] sampling_state_init
-	[  54] sampling_state_update
-	[  55] save_1darray
-	[  56] sgsim_init
+	[  31] d_arange
+	[  32] find_neighbor
+	[  33] kriging_memory_free
+	[  34] kriging_param_setting
+	[  35] lu_decomposition
+	[  36] lu_inverse_solver
+	[  37] matrix_agumented
+	[  38] matrixform
+	[  39] mt19937_generate
+	[  40] mt19937_get_double
+	[  41] mt19937_get_double_range
+	[  42] mt19937_get_float
+	[  43] mt19937_get_float_range
+	[  44] mt19937_get_int32_range
+	[  45] mt19937_init
+	[  46] mt19937_random_normal
+	[  47] partition2d
+	[  48] pdist
+	[  49] quickselect2d
+	[  50] quicksort2d
+	[  51] randompath
+	[  52] sampling_state_init
+	[  53] sampling_state_update
+	[  54] save_1darray
+	[  55] set_cov_model_default
+	[  56] set_sgsim_default
 	[  57] sgsim_run
 	[  58] sgsim_t_free
 	[  59] simple_kriging
 	[  60] swaprows
 	[  61] variance
 	[  62] variogram
 
@@ -311,92 +311,92 @@
  00000000646ca1b0:	00000000646c23e0 00000000646c265a 00000000646cb0e0
  00000000646ca1bc:	00000000646c2660 00000000646c28f0 00000000646cb0ec
  00000000646ca1c8:	00000000646c28f0 00000000646c2b7d 00000000646cb0f8
  00000000646ca1d4:	00000000646c2b80 00000000646c2e37 00000000646cb104
  00000000646ca1e0:	00000000646c2e40 00000000646c30cd 00000000646cb118
  00000000646ca1ec:	00000000646c30d0 00000000646c3387 00000000646cb124
  00000000646ca1f8:	00000000646c3390 00000000646c3416 00000000646cb138
- 00000000646ca204:	00000000646c3420 00000000646c344b 00000000646cb148
- 00000000646ca210:	00000000646c3450 00000000646c3504 00000000646cb14c
- 00000000646ca21c:	00000000646c3510 00000000646c360d 00000000646cb168
- 00000000646ca228:	00000000646c3610 00000000646c3677 00000000646cb18c
- 00000000646ca234:	00000000646c3680 00000000646c368a 00000000646cb19c
- 00000000646ca240:	00000000646c3690 00000000646c3844 00000000646cb1a0
- 00000000646ca24c:	00000000646c3850 00000000646c3b04 00000000646cb1b0
- 00000000646ca258:	00000000646c3b10 00000000646c3e7c 00000000646cb1c4
- 00000000646ca264:	00000000646c3e80 00000000646c3fe7 00000000646cb1d8
- 00000000646ca270:	00000000646c3ff0 00000000646c40f0 00000000646cb1e8
- 00000000646ca27c:	00000000646c40f0 00000000646c4112 00000000646cb1f4
- 00000000646ca288:	00000000646c4120 00000000646c43a9 00000000646cb1fc
- 00000000646ca294:	00000000646c43b0 00000000646c47a0 00000000646cb210
- 00000000646ca2a0:	00000000646c47a0 00000000646c4824 00000000646cb228
- 00000000646ca2ac:	00000000646c4830 00000000646c4900 00000000646cb230
- 00000000646ca2b8:	00000000646c4900 00000000646c4a45 00000000646cb238
- 00000000646ca2c4:	00000000646c4a50 00000000646c4b3a 00000000646cb250
- 00000000646ca2d0:	00000000646c4b40 00000000646c4cbb 00000000646cb264
- 00000000646ca2dc:	00000000646c4cc0 00000000646c4d05 00000000646cb278
- 00000000646ca2e8:	00000000646c4d10 00000000646c4d6a 00000000646cb284
- 00000000646ca2f4:	00000000646c4d70 00000000646c50d4 00000000646cb28c
- 00000000646ca300:	00000000646c50e0 00000000646c50e9 00000000646cb2a4
- 00000000646ca30c:	00000000646c50f0 00000000646c510b 00000000646cb2a8
- 00000000646ca318:	00000000646c5110 00000000646c5171 00000000646cb2ac
- 00000000646ca324:	00000000646c5180 00000000646c5217 00000000646cb2b0
- 00000000646ca330:	00000000646c5220 00000000646c52d7 00000000646cb2c0
- 00000000646ca33c:	00000000646c52e0 00000000646c54b3 00000000646cb2d0
- 00000000646ca348:	00000000646c54c0 00000000646c55c8 00000000646cb2f0
- 00000000646ca354:	00000000646c55e0 00000000646c5615 00000000646cb2f4
- 00000000646ca360:	00000000646c5620 00000000646c5686 00000000646cb2fc
- 00000000646ca36c:	00000000646c5690 00000000646c56af 00000000646cb308
- 00000000646ca378:	00000000646c56b0 00000000646c5786 00000000646cb30c
- 00000000646ca384:	00000000646c5790 00000000646c5888 00000000646cb31c
- 00000000646ca390:	00000000646c5890 00000000646c58bf 00000000646cb32c
- 00000000646ca39c:	00000000646c58c0 00000000646c5933 00000000646cb334
- 00000000646ca3a8:	00000000646c5940 00000000646c5943 00000000646cb340
- 00000000646ca3b4:	00000000646c5950 00000000646c5954 00000000646cb344
- 00000000646ca3c0:	00000000646c5960 00000000646c5964 00000000646cb348
- 00000000646ca3cc:	00000000646c5970 00000000646c5b3d 00000000646cb358
- 00000000646ca3d8:	00000000646c5b40 00000000646c5dfb 00000000646cb368
- 00000000646ca3e4:	00000000646c5e00 00000000646c5fa0 00000000646cb380
- 00000000646ca3f0:	00000000646c5fa0 00000000646c608c 00000000646cb388
- 00000000646ca3fc:	00000000646c6090 00000000646c6277 00000000646cb398
- 00000000646ca408:	00000000646c6280 00000000646c62ea 00000000646cb3a0
- 00000000646ca414:	00000000646c62f0 00000000646c636f 00000000646cb3b0
- 00000000646ca420:	00000000646c6370 00000000646c6410 00000000646cb3c0
- 00000000646ca42c:	00000000646c6410 00000000646c64ea 00000000646cb3c8
- 00000000646ca438:	00000000646c64f0 00000000646c650e 00000000646cb3d0
- 00000000646ca444:	00000000646c6510 00000000646c6522 00000000646cb3d4
- 00000000646ca450:	00000000646c6530 00000000646c6574 00000000646cb3d8
- 00000000646ca45c:	00000000646c6580 00000000646c660d 00000000646cb3dc
- 00000000646ca468:	00000000646c6610 00000000646c6684 00000000646cb3e8
- 00000000646ca474:	00000000646c6690 00000000646c66ce 00000000646cb3f0
- 00000000646ca480:	00000000646c66d0 00000000646c673f 00000000646cb3f8
- 00000000646ca48c:	00000000646c6740 00000000646c6777 00000000646cb400
- 00000000646ca498:	00000000646c6780 00000000646c6811 00000000646cb408
- 00000000646ca4a4:	00000000646c6820 00000000646c68c6 00000000646cb410
- 00000000646ca4b0:	00000000646c68d0 00000000646c68d3 00000000646cb418
- 00000000646ca4bc:	00000000646c6920 00000000646c6926 00000000646cb41c
- 00000000646ca4c8:	00000000646c6930 00000000646c6936 00000000646cb420
- 00000000646ca4d4:	00000000646c6940 00000000646c6a66 00000000646cb424
- 00000000646ca4e0:	00000000646c6a70 00000000646c6a75 00000000646cb430
- 00000000646ca4ec:	00000000646c6a80 00000000646c6b74 00000000646cb434
- 00000000646ca4f8:	00000000646c6bb0 00000000646c6d94 00000000646cb440
- 00000000646ca504:	00000000646c6da0 00000000646c6ec0 00000000646cb44c
- 00000000646ca510:	00000000646c6ec0 00000000646c6f56 00000000646cb458
- 00000000646ca51c:	00000000646c6f60 00000000646c74b7 00000000646cb460
- 00000000646ca528:	00000000646c74c0 00000000646c773e 00000000646cb47c
- 00000000646ca534:	00000000646c7810 00000000646c78ce 00000000646cb488
- 00000000646ca540:	00000000646c79f0 00000000646c7a15 00000000646cb490
- 00000000646ca54c:	00000000646c7a20 00000000646c7ae8 00000000646cb494
- 00000000646ca558:	00000000646c7af0 00000000646c7b5f 00000000646cb4a4
- 00000000646ca564:	00000000646c7b60 00000000646c7b7f 00000000646cb4b0
- 00000000646ca570:	00000000646c7c50 00000000646c7c91 00000000646cb4b8
- 00000000646ca57c:	00000000646c7ca0 00000000646c7cac 00000000646cb4c0
- 00000000646ca588:	00000000646c7cb0 00000000646c7dac 00000000646cb4c4
- 00000000646ca594:	00000000646c7dc0 00000000646c7e29 00000000646cb34c
- 00000000646ca5a0:	00000000646c7e30 00000000646c7e35 00000000646cb4dc
+ 00000000646ca204:	00000000646c3420 00000000646c3459 00000000646cb148
+ 00000000646ca210:	00000000646c3460 00000000646c3514 00000000646cb14c
+ 00000000646ca21c:	00000000646c3520 00000000646c361d 00000000646cb168
+ 00000000646ca228:	00000000646c3620 00000000646c3687 00000000646cb18c
+ 00000000646ca234:	00000000646c3690 00000000646c369a 00000000646cb19c
+ 00000000646ca240:	00000000646c36a0 00000000646c386b 00000000646cb1a0
+ 00000000646ca24c:	00000000646c3870 00000000646c3b24 00000000646cb1b4
+ 00000000646ca258:	00000000646c3b30 00000000646c3e9c 00000000646cb1c8
+ 00000000646ca264:	00000000646c3ea0 00000000646c4007 00000000646cb1dc
+ 00000000646ca270:	00000000646c4010 00000000646c4100 00000000646cb1ec
+ 00000000646ca27c:	00000000646c4100 00000000646c4122 00000000646cb1f8
+ 00000000646ca288:	00000000646c4130 00000000646c43b9 00000000646cb200
+ 00000000646ca294:	00000000646c43c0 00000000646c4623 00000000646cb214
+ 00000000646ca2a0:	00000000646c4630 00000000646c46b4 00000000646cb22c
+ 00000000646ca2ac:	00000000646c46c0 00000000646c4790 00000000646cb234
+ 00000000646ca2b8:	00000000646c4790 00000000646c48d5 00000000646cb23c
+ 00000000646ca2c4:	00000000646c48e0 00000000646c49ca 00000000646cb254
+ 00000000646ca2d0:	00000000646c49d0 00000000646c4b4b 00000000646cb268
+ 00000000646ca2dc:	00000000646c4b50 00000000646c4b95 00000000646cb27c
+ 00000000646ca2e8:	00000000646c4ba0 00000000646c4c3b 00000000646cb288
+ 00000000646ca2f4:	00000000646c4c40 00000000646c501d 00000000646cb294
+ 00000000646ca300:	00000000646c5020 00000000646c5029 00000000646cb2ac
+ 00000000646ca30c:	00000000646c5030 00000000646c504b 00000000646cb2b0
+ 00000000646ca318:	00000000646c5050 00000000646c50b1 00000000646cb2b4
+ 00000000646ca324:	00000000646c50c0 00000000646c5157 00000000646cb2b8
+ 00000000646ca330:	00000000646c5160 00000000646c5217 00000000646cb2c8
+ 00000000646ca33c:	00000000646c5220 00000000646c53f3 00000000646cb2d8
+ 00000000646ca348:	00000000646c5400 00000000646c5508 00000000646cb2f8
+ 00000000646ca354:	00000000646c5520 00000000646c5555 00000000646cb2fc
+ 00000000646ca360:	00000000646c5560 00000000646c55c6 00000000646cb304
+ 00000000646ca36c:	00000000646c55d0 00000000646c55ef 00000000646cb310
+ 00000000646ca378:	00000000646c55f0 00000000646c56c6 00000000646cb314
+ 00000000646ca384:	00000000646c56d0 00000000646c57c8 00000000646cb324
+ 00000000646ca390:	00000000646c57d0 00000000646c57ff 00000000646cb334
+ 00000000646ca39c:	00000000646c5800 00000000646c5873 00000000646cb33c
+ 00000000646ca3a8:	00000000646c5880 00000000646c5883 00000000646cb348
+ 00000000646ca3b4:	00000000646c5890 00000000646c5894 00000000646cb34c
+ 00000000646ca3c0:	00000000646c58a0 00000000646c58a4 00000000646cb350
+ 00000000646ca3cc:	00000000646c58b0 00000000646c5a7d 00000000646cb360
+ 00000000646ca3d8:	00000000646c5a80 00000000646c5d3b 00000000646cb370
+ 00000000646ca3e4:	00000000646c5d40 00000000646c5ee0 00000000646cb388
+ 00000000646ca3f0:	00000000646c5ee0 00000000646c5fcc 00000000646cb390
+ 00000000646ca3fc:	00000000646c5fd0 00000000646c61b7 00000000646cb3a0
+ 00000000646ca408:	00000000646c61c0 00000000646c622a 00000000646cb3a8
+ 00000000646ca414:	00000000646c6230 00000000646c62af 00000000646cb3b8
+ 00000000646ca420:	00000000646c62b0 00000000646c6350 00000000646cb3c8
+ 00000000646ca42c:	00000000646c6350 00000000646c642a 00000000646cb3d0
+ 00000000646ca438:	00000000646c6430 00000000646c644e 00000000646cb3d8
+ 00000000646ca444:	00000000646c6450 00000000646c6462 00000000646cb3dc
+ 00000000646ca450:	00000000646c6470 00000000646c64b4 00000000646cb3e0
+ 00000000646ca45c:	00000000646c64c0 00000000646c654d 00000000646cb3e4
+ 00000000646ca468:	00000000646c6550 00000000646c65c4 00000000646cb3f0
+ 00000000646ca474:	00000000646c65d0 00000000646c660e 00000000646cb3f8
+ 00000000646ca480:	00000000646c6610 00000000646c667f 00000000646cb400
+ 00000000646ca48c:	00000000646c6680 00000000646c66b7 00000000646cb408
+ 00000000646ca498:	00000000646c66c0 00000000646c6751 00000000646cb410
+ 00000000646ca4a4:	00000000646c6760 00000000646c6806 00000000646cb418
+ 00000000646ca4b0:	00000000646c6810 00000000646c6813 00000000646cb420
+ 00000000646ca4bc:	00000000646c6860 00000000646c6866 00000000646cb424
+ 00000000646ca4c8:	00000000646c6870 00000000646c6876 00000000646cb428
+ 00000000646ca4d4:	00000000646c6880 00000000646c69a6 00000000646cb42c
+ 00000000646ca4e0:	00000000646c69b0 00000000646c69b5 00000000646cb438
+ 00000000646ca4ec:	00000000646c69c0 00000000646c6ab4 00000000646cb43c
+ 00000000646ca4f8:	00000000646c6af0 00000000646c6cd4 00000000646cb448
+ 00000000646ca504:	00000000646c6ce0 00000000646c6e00 00000000646cb454
+ 00000000646ca510:	00000000646c6e00 00000000646c6e96 00000000646cb460
+ 00000000646ca51c:	00000000646c6ea0 00000000646c73f7 00000000646cb468
+ 00000000646ca528:	00000000646c7400 00000000646c767e 00000000646cb484
+ 00000000646ca534:	00000000646c7750 00000000646c780e 00000000646cb490
+ 00000000646ca540:	00000000646c7930 00000000646c7955 00000000646cb498
+ 00000000646ca54c:	00000000646c7960 00000000646c7a28 00000000646cb49c
+ 00000000646ca558:	00000000646c7a30 00000000646c7a9f 00000000646cb4ac
+ 00000000646ca564:	00000000646c7aa0 00000000646c7abf 00000000646cb4b8
+ 00000000646ca570:	00000000646c7b90 00000000646c7bd1 00000000646cb4c0
+ 00000000646ca57c:	00000000646c7be0 00000000646c7bec 00000000646cb4c8
+ 00000000646ca588:	00000000646c7bf0 00000000646c7cec 00000000646cb4cc
+ 00000000646ca594:	00000000646c7d00 00000000646c7d69 00000000646cb354
+ 00000000646ca5a0:	00000000646c7d70 00000000646c7d75 00000000646cb4e4
 
 Dump of .xdata
  00000000646cb000 (rva: 0000b000): 00000000646c1000 - 00000000646c100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000000646cb004 (rva: 0000b004): 00000000646c1010 - 00000000646c11ff
 	Version: 1, Flags: none
@@ -566,600 +566,603 @@
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
  00000000646cb138 (rva: 0000b138): 00000000646c3390 - 00000000646c3416
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0e, Frame offset: 0x0, Frame reg: none
 	  pc+0x0e: save xmm7 at rsp + 0x30
 	  pc+0x09: save xmm6 at rsp + 0x20
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 00000000646cb148 (rva: 0000b148): 00000000646c3420 - 00000000646c344b
+ 00000000646cb148 (rva: 0000b148): 00000000646c3420 - 00000000646c3459
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb14c (rva: 0000b14c): 00000000646c3450 - 00000000646c3504
+ 00000000646cb14c (rva: 0000b14c): 00000000646c3460 - 00000000646c3514
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x18, Frame offset: 0x0, Frame reg: none
 	  pc+0x18: save xmm8 at rsp + 0x40
 	  pc+0x12: save xmm7 at rsp + 0x30
 	  pc+0x0d: save xmm6 at rsp + 0x20
 	  pc+0x08: alloc small area: rsp = rsp - 0x58
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb168 (rva: 0000b168): 00000000646c3510 - 00000000646c360d
+ 00000000646cb168 (rva: 0000b168): 00000000646c3520 - 00000000646c361d
 	Version: 1, Flags: none
 	Nbr codes: 15, Prologue size: 0x20, Frame offset: 0x0, Frame reg: none
 	  pc+0x20: save xmm8 at rsp + 0x50
 	  pc+0x1a: save xmm7 at rsp + 0x40
 	  pc+0x15: save xmm6 at rsp + 0x30
 	  pc+0x10: alloc small area: rsp = rsp - 0x68
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb18c (rva: 0000b18c): 00000000646c3610 - 00000000646c3677
+ 00000000646cb18c (rva: 0000b18c): 00000000646c3620 - 00000000646c3687
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0b, Frame offset: 0x0, Frame reg: none
 	  pc+0x0b: save xmm6 at rsp + 0x20
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb19c (rva: 0000b19c): 00000000646c3680 - 00000000646c368a
+ 00000000646cb19c (rva: 0000b19c): 00000000646c3690 - 00000000646c369a
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb1a0 (rva: 0000b1a0): 00000000646c3690 - 00000000646c3844
+ 00000000646cb1a0 (rva: 0000b1a0): 00000000646c36a0 - 00000000646c386b
 	Version: 1, Flags: none
-	Nbr codes: 6, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
-	  pc+0x0c: save xmm6 at rsp + 0x20
-	  pc+0x07: alloc small area: rsp = rsp - 0x30
-	  pc+0x03: push rbx
-	  pc+0x02: push rsi
-	  pc+0x01: push rdi
- 00000000646cb1b0 (rva: 0000b1b0): 00000000646c3850 - 00000000646c3b04
+	Nbr codes: 8, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
+	  pc+0x0f: save xmm6 at rsp + 0x20
+	  pc+0x0a: alloc small area: rsp = rsp - 0x30
+	  pc+0x06: push rbx
+	  pc+0x05: push rsi
+	  pc+0x04: push rdi
+	  pc+0x03: push rbp
+	  pc+0x02: push r12
+ 00000000646cb1b4 (rva: 0000b1b4): 00000000646c3870 - 00000000646c3b24
 	Version: 1, Flags: none
 	Nbr codes: 7, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
 	  pc+0x10: save xmm7 at rsp + 0x40
 	  pc+0x0b: save xmm6 at rsp + 0x30
 	  pc+0x06: alloc small area: rsp = rsp - 0x58
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb1c4 (rva: 0000b1c4): 00000000646c3b10 - 00000000646c3e7c
+ 00000000646cb1c8 (rva: 0000b1c8): 00000000646c3b30 - 00000000646c3e9c
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save xmm6 at rsp + 0x20
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb1d8 (rva: 0000b1d8): 00000000646c3e80 - 00000000646c3fe7
+ 00000000646cb1dc (rva: 0000b1dc): 00000000646c3ea0 - 00000000646c4007
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0d, Frame offset: 0x0, Frame reg: none
 	  pc+0x0d: save xmm7 at rsp + 0x10
 	  pc+0x08: save xmm6 at rsp + 0x0
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb1e8 (rva: 0000b1e8): 00000000646c3ff0 - 00000000646c40f0
+ 00000000646cb1ec (rva: 0000b1ec): 00000000646c4010 - 00000000646c4100
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb1f4 (rva: 0000b1f4): 00000000646c40f0 - 00000000646c4112
+ 00000000646cb1f8 (rva: 0000b1f8): 00000000646c4100 - 00000000646c4122
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
- 00000000646cb1fc (rva: 0000b1fc): 00000000646c4120 - 00000000646c43a9
+ 00000000646cb200 (rva: 0000b200): 00000000646c4130 - 00000000646c43b9
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb210 (rva: 0000b210): 00000000646c43b0 - 00000000646c47a0
+ 00000000646cb214 (rva: 0000b214): 00000000646c43c0 - 00000000646c4623
 	Version: 1, Flags: none
-	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
-	  pc+0x13: alloc large area: rsp = rsp - 0xa8
+	Nbr codes: 9, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
+	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb228 (rva: 0000b228): 00000000646c47a0 - 00000000646c4824
+ 00000000646cb22c (rva: 0000b22c): 00000000646c4630 - 00000000646c46b4
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb230 (rva: 0000b230): 00000000646c4830 - 00000000646c4900
+ 00000000646cb234 (rva: 0000b234): 00000000646c46c0 - 00000000646c4790
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb238 (rva: 0000b238): 00000000646c4900 - 00000000646c4a45
+ 00000000646cb23c (rva: 0000b23c): 00000000646c4790 - 00000000646c48d5
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
 	  pc+0x10: alloc small area: rsp = rsp - 0x28
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb250 (rva: 0000b250): 00000000646c4a50 - 00000000646c4b3a
+ 00000000646cb254 (rva: 0000b254): 00000000646c48e0 - 00000000646c49ca
 	Version: 1, Flags: none
 	Nbr codes: 7, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: push rbx
 	  pc+0x09: push rsi
 	  pc+0x08: push rdi
 	  pc+0x07: push rbp
 	  pc+0x06: push r12
 	  pc+0x04: push r13
 	  pc+0x02: push r14
- 00000000646cb264 (rva: 0000b264): 00000000646c4b40 - 00000000646c4cbb
+ 00000000646cb268 (rva: 0000b268): 00000000646c49d0 - 00000000646c4b4b
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: alloc large area: rsp = rsp - 0x1d8
 	  pc+0x08: push rbx
 	  pc+0x07: push rsi
 	  pc+0x06: push rdi
 	  pc+0x05: push rbp
 	  pc+0x04: push r12
 	  pc+0x02: push r13
- 00000000646cb278 (rva: 0000b278): 00000000646c4cc0 - 00000000646c4d05
+ 00000000646cb27c (rva: 0000b27c): 00000000646c4b50 - 00000000646c4b95
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb284 (rva: 0000b284): 00000000646c4d10 - 00000000646c4d6a
+ 00000000646cb288 (rva: 0000b288): 00000000646c4ba0 - 00000000646c4c3b
 	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: alloc small area: rsp = rsp - 0x20
-	  pc+0x01: push rbx
- 00000000646cb28c (rva: 0000b28c): 00000000646c4d70 - 00000000646c50d4
+	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
+	  pc+0x06: alloc small area: rsp = rsp - 0x28
+	  pc+0x02: push rbx
+	  pc+0x01: push rsi
+ 00000000646cb294 (rva: 0000b294): 00000000646c4c40 - 00000000646c501d
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xa08
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb2a4 (rva: 0000b2a4): 00000000646c50e0 - 00000000646c50e9
+ 00000000646cb2ac (rva: 0000b2ac): 00000000646c5020 - 00000000646c5029
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb2a8 (rva: 0000b2a8): 00000000646c50f0 - 00000000646c510b
+ 00000000646cb2b0 (rva: 0000b2b0): 00000000646c5030 - 00000000646c504b
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb2ac (rva: 0000b2ac): 00000000646c5110 - 00000000646c5171
+ 00000000646cb2b4 (rva: 0000b2b4): 00000000646c5050 - 00000000646c50b1
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb2b0 (rva: 0000b2b0): 00000000646c5180 - 00000000646c5217
+ 00000000646cb2b8 (rva: 0000b2b8): 00000000646c50c0 - 00000000646c5157
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb2c0 (rva: 0000b2c0): 00000000646c5220 - 00000000646c52d7
+ 00000000646cb2c8 (rva: 0000b2c8): 00000000646c5160 - 00000000646c5217
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb2d0 (rva: 0000b2d0): 00000000646c52e0 - 00000000646c54b3
+ 00000000646cb2d8 (rva: 0000b2d8): 00000000646c5220 - 00000000646c53f3
 	Version: 1, Flags: none
 	Nbr codes: 13, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save xmm7 at rsp + 0x50
 	  pc+0x15: save xmm6 at rsp + 0x40
 	  pc+0x10: alloc small area: rsp = rsp - 0x68
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000000646cb2f0 (rva: 0000b2f0): 00000000646c54c0 - 00000000646c55c8
+ 00000000646cb2f8 (rva: 0000b2f8): 00000000646c5400 - 00000000646c5508
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb2f4 (rva: 0000b2f4): 00000000646c55e0 - 00000000646c5615
+ 00000000646cb2fc (rva: 0000b2fc): 00000000646c5520 - 00000000646c5555
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb2fc (rva: 0000b2fc): 00000000646c5620 - 00000000646c5686
+ 00000000646cb304 (rva: 0000b304): 00000000646c5560 - 00000000646c55c6
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb308 (rva: 0000b308): 00000000646c5690 - 00000000646c56af
+ 00000000646cb310 (rva: 0000b310): 00000000646c55d0 - 00000000646c55ef
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb30c (rva: 0000b30c): 00000000646c56b0 - 00000000646c5786
+ 00000000646cb314 (rva: 0000b314): 00000000646c55f0 - 00000000646c56c6
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb31c (rva: 0000b31c): 00000000646c5790 - 00000000646c5888
+ 00000000646cb324 (rva: 0000b324): 00000000646c56d0 - 00000000646c57c8
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0a: alloc small area: rsp = rsp - 0x70
 	  pc+0x06: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
- 00000000646cb32c (rva: 0000b32c): 00000000646c5890 - 00000000646c58bf
+ 00000000646cb334 (rva: 0000b334): 00000000646c57d0 - 00000000646c57ff
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb334 (rva: 0000b334): 00000000646c58c0 - 00000000646c5933
+ 00000000646cb33c (rva: 0000b33c): 00000000646c5800 - 00000000646c5873
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb340 (rva: 0000b340): 00000000646c5940 - 00000000646c5943
+ 00000000646cb348 (rva: 0000b348): 00000000646c5880 - 00000000646c5883
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb344 (rva: 0000b344): 00000000646c5950 - 00000000646c5954
+ 00000000646cb34c (rva: 0000b34c): 00000000646c5890 - 00000000646c5894
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb348 (rva: 0000b348): 00000000646c5960 - 00000000646c5964
+ 00000000646cb350 (rva: 0000b350): 00000000646c58a0 - 00000000646c58a4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb358 (rva: 0000b358): 00000000646c5970 - 00000000646c5b3d
+ 00000000646cb360 (rva: 0000b360): 00000000646c58b0 - 00000000646c5a7d
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x50
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb368 (rva: 0000b368): 00000000646c5b40 - 00000000646c5dfb
+ 00000000646cb370 (rva: 0000b370): 00000000646c5a80 - 00000000646c5d3b
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000000646cb380 (rva: 0000b380): 00000000646c5e00 - 00000000646c5fa0
+ 00000000646cb388 (rva: 0000b388): 00000000646c5d40 - 00000000646c5ee0
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb388 (rva: 0000b388): 00000000646c5fa0 - 00000000646c608c
+ 00000000646cb390 (rva: 0000b390): 00000000646c5ee0 - 00000000646c5fcc
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb398 (rva: 0000b398): 00000000646c6090 - 00000000646c6277
+ 00000000646cb3a0 (rva: 0000b3a0): 00000000646c5fd0 - 00000000646c61b7
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3a0 (rva: 0000b3a0): 00000000646c6280 - 00000000646c62ea
+ 00000000646cb3a8 (rva: 0000b3a8): 00000000646c61c0 - 00000000646c622a
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3b0 (rva: 0000b3b0): 00000000646c62f0 - 00000000646c636f
+ 00000000646cb3b8 (rva: 0000b3b8): 00000000646c6230 - 00000000646c62af
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3c0 (rva: 0000b3c0): 00000000646c6370 - 00000000646c6410
+ 00000000646cb3c8 (rva: 0000b3c8): 00000000646c62b0 - 00000000646c6350
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3c8 (rva: 0000b3c8): 00000000646c6410 - 00000000646c64ea
+ 00000000646cb3d0 (rva: 0000b3d0): 00000000646c6350 - 00000000646c642a
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3d0 (rva: 0000b3d0): 00000000646c64f0 - 00000000646c650e
+ 00000000646cb3d8 (rva: 0000b3d8): 00000000646c6430 - 00000000646c644e
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb3d4 (rva: 0000b3d4): 00000000646c6510 - 00000000646c6522
+ 00000000646cb3dc (rva: 0000b3dc): 00000000646c6450 - 00000000646c6462
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb3d8 (rva: 0000b3d8): 00000000646c6530 - 00000000646c6574
+ 00000000646cb3e0 (rva: 0000b3e0): 00000000646c6470 - 00000000646c64b4
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb3dc (rva: 0000b3dc): 00000000646c6580 - 00000000646c660d
+ 00000000646cb3e4 (rva: 0000b3e4): 00000000646c64c0 - 00000000646c654d
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb3e8 (rva: 0000b3e8): 00000000646c6610 - 00000000646c6684
+ 00000000646cb3f0 (rva: 0000b3f0): 00000000646c6550 - 00000000646c65c4
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb3f0 (rva: 0000b3f0): 00000000646c6690 - 00000000646c66ce
+ 00000000646cb3f8 (rva: 0000b3f8): 00000000646c65d0 - 00000000646c660e
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb3f8 (rva: 0000b3f8): 00000000646c66d0 - 00000000646c673f
+ 00000000646cb400 (rva: 0000b400): 00000000646c6610 - 00000000646c667f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb400 (rva: 0000b400): 00000000646c6740 - 00000000646c6777
+ 00000000646cb408 (rva: 0000b408): 00000000646c6680 - 00000000646c66b7
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb408 (rva: 0000b408): 00000000646c6780 - 00000000646c6811
+ 00000000646cb410 (rva: 0000b410): 00000000646c66c0 - 00000000646c6751
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb410 (rva: 0000b410): 00000000646c6820 - 00000000646c68c6
+ 00000000646cb418 (rva: 0000b418): 00000000646c6760 - 00000000646c6806
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb418 (rva: 0000b418): 00000000646c68d0 - 00000000646c68d3
+ 00000000646cb420 (rva: 0000b420): 00000000646c6810 - 00000000646c6813
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb41c (rva: 0000b41c): 00000000646c6920 - 00000000646c6926
+ 00000000646cb424 (rva: 0000b424): 00000000646c6860 - 00000000646c6866
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb420 (rva: 0000b420): 00000000646c6930 - 00000000646c6936
+ 00000000646cb428 (rva: 0000b428): 00000000646c6870 - 00000000646c6876
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb424 (rva: 0000b424): 00000000646c6940 - 00000000646c6a66
+ 00000000646cb42c (rva: 0000b42c): 00000000646c6880 - 00000000646c69a6
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb430 (rva: 0000b430): 00000000646c6a70 - 00000000646c6a75
+ 00000000646cb438 (rva: 0000b438): 00000000646c69b0 - 00000000646c69b5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb434 (rva: 0000b434): 00000000646c6a80 - 00000000646c6b74
+ 00000000646cb43c (rva: 0000b43c): 00000000646c69c0 - 00000000646c6ab4
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb440 (rva: 0000b440): 00000000646c6bb0 - 00000000646c6d94
+ 00000000646cb448 (rva: 0000b448): 00000000646c6af0 - 00000000646c6cd4
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb44c (rva: 0000b44c): 00000000646c6da0 - 00000000646c6ec0
+ 00000000646cb454 (rva: 0000b454): 00000000646c6ce0 - 00000000646c6e00
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb458 (rva: 0000b458): 00000000646c6ec0 - 00000000646c6f56
+ 00000000646cb460 (rva: 0000b460): 00000000646c6e00 - 00000000646c6e96
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
- 00000000646cb460 (rva: 0000b460): 00000000646c6f60 - 00000000646c74b7
+ 00000000646cb468 (rva: 0000b468): 00000000646c6ea0 - 00000000646c73f7
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save xmm7 at rsp + 0x80
 	  pc+0x12: save xmm6 at rsp + 0x70
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb47c (rva: 0000b47c): 00000000646c74c0 - 00000000646c773e
+ 00000000646cb484 (rva: 0000b484): 00000000646c7400 - 00000000646c767e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: save xmm6 at rsp + 0x40
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb488 (rva: 0000b488): 00000000646c7810 - 00000000646c78ce
+ 00000000646cb490 (rva: 0000b490): 00000000646c7750 - 00000000646c780e
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x30
 	  pc+0x01: push rbx
- 00000000646cb490 (rva: 0000b490): 00000000646c79f0 - 00000000646c7a15
+ 00000000646cb498 (rva: 0000b498): 00000000646c7930 - 00000000646c7955
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb494 (rva: 0000b494): 00000000646c7a20 - 00000000646c7ae8
+ 00000000646cb49c (rva: 0000b49c): 00000000646c7960 - 00000000646c7a28
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb4a4 (rva: 0000b4a4): 00000000646c7af0 - 00000000646c7b5f
+ 00000000646cb4ac (rva: 0000b4ac): 00000000646c7a30 - 00000000646c7a9f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb4b0 (rva: 0000b4b0): 00000000646c7b60 - 00000000646c7b7f
+ 00000000646cb4b8 (rva: 0000b4b8): 00000000646c7aa0 - 00000000646c7abf
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb4b8 (rva: 0000b4b8): 00000000646c7c50 - 00000000646c7c91
+ 00000000646cb4c0 (rva: 0000b4c0): 00000000646c7b90 - 00000000646c7bd1
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb4c0 (rva: 0000b4c0): 00000000646c7ca0 - 00000000646c7cac
+ 00000000646cb4c8 (rva: 0000b4c8): 00000000646c7be0 - 00000000646c7bec
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb4c4 (rva: 0000b4c4): 00000000646c7cb0 - 00000000646c7dac
+ 00000000646cb4cc (rva: 0000b4cc): 00000000646c7bf0 - 00000000646c7cec
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x16, Frame offset: 0x0, Frame reg: none
 	  pc+0x16: save xmm8 at rsp + 0x60
 	  pc+0x10: save xmm7 at rsp + 0x50
 	  pc+0x0b: save xmm6 at rsp + 0x40
 	  pc+0x06: alloc small area: rsp = rsp - 0x78
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb34c (rva: 0000b34c): 00000000646c7dc0 - 00000000646c7e29
+ 00000000646cb354 (rva: 0000b354): 00000000646c7d00 - 00000000646c7d69
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb4dc (rva: 0000b4dc): 00000000646c7e30 - 00000000646c7e35
+ 00000000646cb4e4 (rva: 0000b4e4): 00000000646c7d70 - 00000000646c7d75
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00007000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  e48 [7e48] DIR64
+	reloc    0 offset  d88 [7d88] DIR64
 	reloc    1 offset    0 [7000] ABSOLUTE
 
 Virtual Address: 00008000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset    0 [8000] DIR64
 	reloc    1 offset   50 [8050] DIR64
 	reloc    2 offset   58 [8058] DIR64
 	reloc    3 offset   60 [8060] DIR64
 	reloc    4 offset   70 [8070] DIR64
 	reloc    5 offset    0 [8000] ABSOLUTE
 
 Virtual Address: 00009000 Chunk size 52 (0x34) Number of fixups 22
-	reloc    0 offset  270 [9270] DIR64
-	reloc    1 offset  278 [9278] DIR64
-	reloc    2 offset  280 [9280] DIR64
-	reloc    3 offset  2a0 [92a0] DIR64
-	reloc    4 offset  2a8 [92a8] DIR64
-	reloc    5 offset  2b0 [92b0] DIR64
-	reloc    6 offset  2b8 [92b8] DIR64
-	reloc    7 offset  6b0 [96b0] DIR64
-	reloc    8 offset  6c0 [96c0] DIR64
-	reloc    9 offset  6d0 [96d0] DIR64
-	reloc   10 offset  6e0 [96e0] DIR64
-	reloc   11 offset  6f0 [96f0] DIR64
-	reloc   12 offset  700 [9700] DIR64
-	reloc   13 offset  710 [9710] DIR64
-	reloc   14 offset  720 [9720] DIR64
-	reloc   15 offset  730 [9730] DIR64
-	reloc   16 offset  740 [9740] DIR64
-	reloc   17 offset  750 [9750] DIR64
-	reloc   18 offset  760 [9760] DIR64
-	reloc   19 offset  770 [9770] DIR64
-	reloc   20 offset  780 [9780] DIR64
+	reloc    0 offset  290 [9290] DIR64
+	reloc    1 offset  298 [9298] DIR64
+	reloc    2 offset  2a0 [92a0] DIR64
+	reloc    3 offset  2c0 [92c0] DIR64
+	reloc    4 offset  2c8 [92c8] DIR64
+	reloc    5 offset  2d0 [92d0] DIR64
+	reloc    6 offset  2d8 [92d8] DIR64
+	reloc    7 offset  6d0 [96d0] DIR64
+	reloc    8 offset  6e0 [96e0] DIR64
+	reloc    9 offset  6f0 [96f0] DIR64
+	reloc   10 offset  700 [9700] DIR64
+	reloc   11 offset  710 [9710] DIR64
+	reloc   12 offset  720 [9720] DIR64
+	reloc   13 offset  730 [9730] DIR64
+	reloc   14 offset  740 [9740] DIR64
+	reloc   15 offset  750 [9750] DIR64
+	reloc   16 offset  760 [9760] DIR64
+	reloc   17 offset  770 [9770] DIR64
+	reloc   18 offset  780 [9780] DIR64
+	reloc   19 offset  790 [9790] DIR64
+	reloc   20 offset  7a0 [97a0] DIR64
 	reloc   21 offset    0 [9000] ABSOLUTE
 
 Virtual Address: 0000f000 Chunk size 16 (0x10) Number of fixups 4
 	reloc    0 offset   18 [f018] DIR64
 	reloc    1 offset   30 [f030] DIR64
 	reloc    2 offset   38 [f038] DIR64
 	reloc    3 offset    0 [f000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00006e68  00000000646c1000  00000000646c1000  00000600  2**4
+  0 .text         00006da8  00000000646c1000  00000000646c1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
-  1 .data         000000a0  00000000646c8000  00000000646c8000  00007600  2**4
+  1 .data         000000a0  00000000646c8000  00000000646c8000  00007400  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  2 .rdata        000009d0  00000000646c9000  00000000646c9000  00007800  2**5
+  2 .rdata        000009f0  00000000646c9000  00000000646c9000  00007600  2**5
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  3 .pdata        000005ac  00000000646ca000  00000000646ca000  00008200  2**2
+  3 .pdata        000005ac  00000000646ca000  00000000646ca000  00008000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        000004e0  00000000646cb000  00000000646cb000  00008800  2**2
+  4 .xdata        000004e8  00000000646cb000  00000000646cb000  00008600  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  5 .bss          00000b50  00000000646cc000  00000000646cc000  00000000  2**5
+  5 .bss          00000b30  00000000646cc000  00000000646cc000  00000000  2**5
                   ALLOC
-  6 .edata        000006ab  00000000646cd000  00000000646cd000  00008e00  2**2
+  6 .edata        000006b9  00000000646cd000  00000000646cd000  00008c00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000720  00000000646ce000  00000000646ce000  00009600  2**2
+  7 .idata        00000720  00000000646ce000  00000000646ce000  00009400  2**2
                   CONTENTS, ALLOC, LOAD, DATA
-  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009e00  2**3
+  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009c00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
-  9 .tls          00000010  00000000646d0000  00000000646d0000  0000a000  2**3
+  9 .tls          00000010  00000000646d0000  00000000646d0000  00009e00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
- 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a200  2**2
+ 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
- 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a400  2**4
+ 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a200  2**4
                   CONTENTS, READONLY, DEBUGGING
- 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a600  2**0
+ 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a400  2**0
                   CONTENTS, READONLY, DEBUGGING
- 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c600  2**0
+ 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c400  2**0
                   CONTENTS, READONLY, DEBUGGING
- 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c800  2**0
+ 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c600  2**0
                   CONTENTS, READONLY, DEBUGGING
- 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000cc00  2**3
+ 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000ca00  2**3
                   CONTENTS, READONLY, DEBUGGING
- 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000ce00  2**0
+ 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000cc00  2**0
                   CONTENTS, READONLY, DEBUGGING
 SYMBOL TABLE:
 [  0](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000028 crtdll.c
 File 
 [  2](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000000 pre_c_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [  4](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 atexit_table
 [  5](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000010 _CRT_INIT
 [  6](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000018 __proc_attached
-[  7](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000720 .rdata$.refptr.__native_startup_lock
+[  7](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .rdata$.refptr.__native_startup_lock
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[  9](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000730 .rdata$.refptr.__native_startup_state
+[  9](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000750 .rdata$.refptr.__native_startup_state
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 11](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006f0 .rdata$.refptr.__dyn_tls_init_callback
+[ 11](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000710 .rdata$.refptr.__dyn_tls_init_callback
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 13](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000770 .rdata$.refptr.__xi_z
+[ 13](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000790 .rdata$.refptr.__xi_z
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 15](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000760 .rdata$.refptr.__xi_a
+[ 15](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000780 .rdata$.refptr.__xi_a
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 17](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000750 .rdata$.refptr.__xc_z
+[ 17](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000770 .rdata$.refptr.__xc_z
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 19](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .rdata$.refptr.__xc_a
+[ 19](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000760 .rdata$.refptr.__xc_a
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 21](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000000200 __DllMainCRTStartup
-[ 22](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000710 .rdata$.refptr.__native_dllmain_reason
+[ 22](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000730 .rdata$.refptr.__native_dllmain_reason
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 24](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000330 DllMainCRTStartup
-[ 25](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000780 .rdata$.refptr.mingw_app_type
+[ 25](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007a0 .rdata$.refptr.mingw_app_type
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 27](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000380 atexit
 [ 28](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .text
 AUX scnlen 0x38f nreloc 39 nlnno 0
 [ 30](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 32](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .bss
@@ -1224,15 +1227,15 @@
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 92](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .xdata
 AUX scnlen 0xa0 nreloc 0 nlnno 0
 [ 94](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000054 .pdata
 AUX scnlen 0x150 nreloc 84 nlnno 0
 [ 96](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .rdata
 AUX scnlen 0x50 nreloc 0 nlnno 0
-[ 98](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000790 .rdata$zzz
+[ 98](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007b0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [100](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000007d c_array_mt.c
 File 
 [102](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000013a0 mt19937_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000013e0 mt19937_generate
 [105](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001660 mt19937_get_int32_range
@@ -1249,1321 +1252,1320 @@
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [117](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000dc .xdata
 AUX scnlen 0x6c nreloc 0 nlnno 0
 [119](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001a4 .pdata
 AUX scnlen 0x60 nreloc 24 nlnno 0
 [121](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .rdata
 AUX scnlen 0x50 nreloc 0 nlnno 0
-[123](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007d0 .rdata$zzz
+[123](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007f0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [125](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000091 cov_model.c
 File 
-[127](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002420 cov_model_init
+[127](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002420 set_cov_model_default
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[129](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002450 cov_model
-[130](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002510 cov_model2d
+[129](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002460 cov_model
+[130](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002520 cov_model2d
 [131](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002420 .text
-AUX scnlen 0x1ed nreloc 6 nlnno 0
+AUX scnlen 0x1fd nreloc 8 nlnno 0
 [133](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [135](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [137](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000148 .xdata
 AUX scnlen 0x44 nreloc 0 nlnno 0
 [139](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000204 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [141](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000a0 .rdata
-AUX scnlen 0x10 nreloc 0 nlnno 0
-[143](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000810 .rdata$zzz
+AUX scnlen 0x18 nreloc 0 nlnno 0
+[143](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[145](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000b6 kriging.c
+[145](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000b5 kriging.c
 File 
-[147](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002610 sampling_state_init
+[147](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000002620 sampling_state_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[149](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002680 sampling_state_update
-[150](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002690 kriging_param_setting
-[151](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 location
-[152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000148 k_range
-[153](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000150 model
-[154](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000100 loc_cov
-[155](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 loc_cov2
+[149](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002690 sampling_state_update
+[150](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000026a0 kriging_param_setting
+[151](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000128 k_range
+[152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000130 model
+[153](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000100 location
+[154](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 location_cov
+[155](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c0 location_cov2d
 [156](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 weights
 [157](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a0 flatten_temp
-[158](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e0 data_temp
-[159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 pdist_temp
-[160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 datacov
-[161](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000060 array2d_temp
-[162](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002850 find_neighbor
-[163](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002b10 simple_kriging
-[164](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 estimation
-[165](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000138 kriging_var
-[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002e80 matrix_agumented
-[167](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002ff0 kriging_memory_free
-[168](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002610 .text
-AUX scnlen 0xae0 nreloc 120 nlnno 0
-[170](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
-AUX scnlen 0x0 nreloc 0 nlnno 0
-[172](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
-AUX scnlen 0x138 nreloc 0 nlnno 0
-[174](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .xdata
-AUX scnlen 0x68 nreloc 0 nlnno 0
-[176](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
+[158](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 pdist_temp
+[159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 data_cov
+[160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000060 distance_mat
+[161](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002870 find_neighbor
+[162](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002b30 simple_kriging
+[163](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000120 estimation
+[164](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000118 kriging_var
+[165](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002ea0 matrix_agumented
+[166](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003010 kriging_memory_free
+[167](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002620 .text
+AUX scnlen 0xae0 nreloc 116 nlnno 0
+[169](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+AUX scnlen 0x0 nreloc 0 nlnno 0
+[171](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
+AUX scnlen 0x118 nreloc 0 nlnno 0
+[173](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000018c .xdata
+AUX scnlen 0x6c nreloc 0 nlnno 0
+[175](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
 AUX scnlen 0x54 nreloc 21 nlnno 0
-[178](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000b0 .rdata
-AUX scnlen 0xa0 nreloc 0 nlnno 0
-[180](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000850 .rdata$zzz
+[177](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000c0 .rdata
+AUX scnlen 0x80 nreloc 0 nlnno 0
+[179](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000870 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[182](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000cf matrix_tools.c
+[181](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000ce matrix_tools.c
 File 
-[184](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000030f0 snprintf.constprop.0
+[183](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000003100 snprintf.constprop.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[186](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003120 lu_decomposition
-[187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000033b0 lu_inverse_solver
-[188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000037a0 arange
-[189](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003830 d_arange
-[190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003900 pdist
-[191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003a50 matrixform
-[192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003b40 save_1darray
-[193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000030f0 .text
-AUX scnlen 0xbcb nreloc 38 nlnno 0
-[195](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[185](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003130 lu_decomposition
+[186](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000033c0 lu_inverse_solver
+[187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003630 arange
+[188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000036c0 d_arange
+[189](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003790 pdist
+[190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000038e0 matrixform
+[191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000039d0 save_1darray
+[192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003100 .text
+AUX scnlen 0xa4b nreloc 42 nlnno 0
+[194](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[197](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000160 .bss
+[196](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000140 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[199](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001f4 .xdata
+[198](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001f8 .xdata
 AUX scnlen 0x84 nreloc 0 nlnno 0
-[201](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .pdata
+[200](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .pdata
 AUX scnlen 0x60 nreloc 24 nlnno 0
-[203](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000150 .rdata
+[202](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000140 .rdata
 AUX scnlen 0xb8 nreloc 0 nlnno 0
-[205](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000890 .rdata$zzz
+[204](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008b0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[207](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000df random_tools.c
+[206](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000de random_tools.c
 File 
-[209](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003cc0 randompath
+[208](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003b50 randompath
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[211](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003cc0 .text
+[210](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003b50 .text
 AUX scnlen 0x45 nreloc 1 nlnno 0
-[213](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[212](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000160 .bss
+[214](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000140 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[217](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000278 .xdata
+[216](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[219](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002dc .pdata
+[218](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002dc .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[221](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008d0 .rdata$zzz
+[220](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008f0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[223](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000f9 sgsim.c
+[222](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000f8 sgsim.c
 File 
-[225](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003d10 sgsim_init
+[224](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003ba0 set_sgsim_default
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[227](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003d70 sgsim_run
-[228](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 _sampling
-[229](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f0 variogram_array
-[230](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 sgsim_array
-[231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 count
-[232](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000210 x_grid
-[233](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 flag
-[234](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040e0 sgsim_t_free
-[235](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003d10 .text
-AUX scnlen 0x3d9 nreloc 64 nlnno 0
-[237](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[226](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003c40 sgsim_run
+[227](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000160 _sampling
+[228](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d0 variogram_array
+[229](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b0 sgsim_array
+[230](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000140 count
+[231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f0 x_grid
+[232](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 flag
+[233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004020 sgsim_t_free
+[234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003ba0 .text
+AUX scnlen 0x489 nreloc 74 nlnno 0
+[236](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[239](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000160 .bss
+[238](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000140 .bss
 AUX scnlen 0xc8 nreloc 0 nlnno 0
-[241](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000284 .xdata
-AUX scnlen 0x24 nreloc 0 nlnno 0
-[243](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002e8 .pdata
+[240](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000288 .xdata
+AUX scnlen 0x28 nreloc 0 nlnno 0
+[242](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002e8 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[245](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000210 .rdata
-AUX scnlen 0x4e nreloc 0 nlnno 0
-[247](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000910 .rdata$zzz
+[244](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .rdata
+AUX scnlen 0x80 nreloc 0 nlnno 0
+[246](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000930 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[249](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010c sort_tools.c
+[248](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010b sort_tools.c
 File 
-[251](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000040f0 swaprows
+[250](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004030 swaprows
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[253](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004110 partition2d
-[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004180 quicksort2d
-[255](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004220 quickselect2d
-[256](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000040f0 .text
+[252](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004050 partition2d
+[253](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040c0 quicksort2d
+[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004160 quickselect2d
+[255](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004030 .text
 AUX scnlen 0x1e7 nreloc 0 nlnno 0
-[258](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[257](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[260](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
+[259](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[262](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a8 .xdata
+[261](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b0 .xdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[264](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
+[263](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
-[266](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000950 .rdata$zzz
+[265](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000970 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[268](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000126 variogram.c
+[267](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000125 variogram.c
 File 
-[270](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000042e0 variogram
+[269](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004220 variogram
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000044c0 variance
-[273](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000042e0 .text
+[271](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004400 variance
+[272](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004220 .text
 AUX scnlen 0x2e8 nreloc 9 nlnno 0
-[275](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[274](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[277](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
+[276](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[279](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002d0 .xdata
+[278](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002d8 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
-[281](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000033c .pdata
+[280](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000033c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[283](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000260 .rdata
+[282](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[285](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000990 .rdata$zzz
+[284](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000009b0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[287](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000045d0 .text
-[288](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
-[289](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000240 .bss
-[290](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
-[291](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
-[292](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
-[293](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
-[294](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000134 fake
+[286](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000004510 .text
+[287](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
+[288](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 .bss
+[289](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
+[290](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
+[291](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
+[292](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
+[293](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000133 fake
 File 
-[296](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
-[297](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
-[298](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045e0 .text
+[295](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
+[296](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
+[297](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[300](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[299](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[302](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
+[301](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[304](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
+[303](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[306](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
-[307](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
-[308](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000142 fake
+[305](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
+[306](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
+[307](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000141 fake
 File 
-[310](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045e0 .text
+[309](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[312](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[311](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[314](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
+[313](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[316](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
+[315](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[318](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
+[317](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[320](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
+[319](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
-[322](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000156 gccmain.c
+[321](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000155 gccmain.c
 File 
-[324](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000045e0 __do_global_dtors
+[323](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004520 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[326](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
-[327](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004620 __do_global_ctors
-[328](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006c0 .rdata$.refptr.__CTOR_LIST__
+[325](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
+[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004560 __do_global_ctors
+[327](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[330](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004690 __main
-[331](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000240 initialized
-[332](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045e0 .text
+[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000045d0 __main
+[330](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 initialized
+[331](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
-[334](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
+[333](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[336](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
+[335](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000220 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[338](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f4 .xdata
+[337](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002fc .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[340](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .pdata
+[339](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[342](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000015e natstart.c
+[341](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000015d natstart.c
 File 
-[344](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000046b0 .text
+[343](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[346](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
+[345](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[348](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000250 .bss
+[347](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000230 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[350](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000176 gs_support.c
+[349](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000175 gs_support.c
 File 
-[352](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000046b0 __security_init_cookie
+[351](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000045f0 __security_init_cookie
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[354](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
+[353](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[356](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
+[355](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[358](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004790 __report_gsfailure
-[359](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000260 GS_ContextRecord
-[360](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000740 GS_ExceptionRecord
-[361](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000270 GS_ExceptionPointers
-[362](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000046b0 .text
+[357](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000046d0 __report_gsfailure
+[358](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000240 GS_ContextRecord
+[359](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000720 GS_ExceptionRecord
+[360](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000290 GS_ExceptionPointers
+[361](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000045f0 .text
 AUX scnlen 0x1d8 nreloc 29 nlnno 0
-[364](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[363](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[366](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000260 .bss
+[365](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000240 .bss
 AUX scnlen 0x578 nreloc 0 nlnno 0
-[368](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .xdata
+[367](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000314 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[370](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000378 .pdata
+[369](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000378 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[372](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000270 .rdata
+[371](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .rdata
 AUX scnlen 0x10 nreloc 2 nlnno 0
-[374](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019c tlssup.c
+[373](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019b tlssup.c
 File 
-[376](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004890 __dyn_tls_dtor
+[375](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000047d0 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[378](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000048c0 __dyn_tls_init
-[379](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006b0 .rdata$.refptr._CRT_MT
+[377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004800 __dyn_tls_init
+[378](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006d0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[381](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
-[382](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[383](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004940 __tlregdtor
-[384](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004890 .text
+[380](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
+[381](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
+[382](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004880 __tlregdtor
+[383](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000047d0 .text
 AUX scnlen 0xb3 nreloc 5 nlnno 0
-[386](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[385](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[388](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007e0 .bss
+[387](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[390](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000032c .xdata
+[389](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000334 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[392](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000390 .pdata
+[391](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000390 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[394](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
+[393](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[396](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
+[395](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[398](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .rdata
+[397](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .rdata
 AUX scnlen 0x48 nreloc 5 nlnno 0
-[400](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .CRT$XDZ
+[399](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .CRT$XDZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[402](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000048 .CRT$XDA
+[401](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000048 .CRT$XDA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[404](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .CRT$XLZ
+[403](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .CRT$XLZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[406](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .CRT$XLA
+[405](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000028 .CRT$XLA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[408](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
+[407](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[410](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
+[409](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[412](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ac cinitexe.c
+[411](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ab cinitexe.c
 File 
-[414](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004950 .text
+[413](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004890 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[416](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[415](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[418](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007f0 .bss
+[417](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007d0 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[420](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
+[419](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[422](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .CRT$XCA
+[421](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .CRT$XCA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[424](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
+[423](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[426](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
+[425](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[428](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001bb mingw_helpers.c
+[427](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ba mingw_helpers.c
 File 
-[430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004950 _decode_pointer
+[429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004890 _decode_pointer
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004960 _encode_pointer
-[433](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004950 .text
+[431](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000048a0 _encode_pointer
+[432](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004890 .text
 AUX scnlen 0x14 nreloc 0 nlnno 0
-[435](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[434](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[437](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007f0 .bss
+[436](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007d0 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[439](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000344 .xdata
+[438](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000034c .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[441](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003b4 .pdata
+[440](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003b4 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[443](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001dc pseudo-reloc.c
+[442](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001db pseudo-reloc.c
 File 
-[445](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006dc0 __report_error
+[444](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006d00 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000004970 __write_memory.part.0
-[448](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000804 maxSections
-[449](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000808 the_secs
-[450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004b40 _pei386_runtime_relocator
-[451](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000800 was_init.95174
-[452](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006d0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[446](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x00000000000048b0 __write_memory.part.0
+[447](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e4 maxSections
+[448](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e8 the_secs
+[449](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004a80 _pei386_runtime_relocator
+[450](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000007e0 was_init.95174
+[451](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006f0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[454](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[453](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000700 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[456](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000700 .rdata$.refptr.__image_base__
+[455](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000720 .rdata$.refptr.__image_base__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[458](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004970 .text
+[457](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000048b0 .text
 AUX scnlen 0x48b nreloc 36 nlnno 0
-[460](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[459](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[462](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000800 .bss
+[461](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007e0 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[464](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002e0 .rdata
+[463](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000300 .rdata
 AUX scnlen 0x102 nreloc 0 nlnno 0
-[466](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text.unlikely
+[465](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d00 .text.unlikely
 AUX scnlen 0x69 nreloc 6 nlnno 0
-[468](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000034c .xdata.unlikely
+[467](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .xdata.unlikely
 AUX scnlen 0xc nreloc 0 nlnno 0
-[470](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata.unlikely
+[469](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata.unlikely
 AUX scnlen 0xc nreloc 3 nlnno 0
-[472](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000358 .xdata
+[471](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000360 .xdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[474](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d8 .pdata
+[473](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d8 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[476](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f1 crt_handler.c
+[475](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f0 crt_handler.c
 File 
-[478](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004e00 __mingw_SEH_error_handler
+[477](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004d40 __mingw_SEH_error_handler
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004fa0 __mingw_init_ehandler
-[481](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000828 was_here.95013
-[482](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000940 emu_pdata
-[483](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 emu_xdata
-[484](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005090 _gnu_exception_handler
-[485](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004e00 .text
+[479](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004ee0 __mingw_init_ehandler
+[480](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000808 was_here.95013
+[481](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000920 emu_pdata
+[482](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000820 emu_xdata
+[483](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004fd0 _gnu_exception_handler
+[484](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004d40 .text
 AUX scnlen 0x477 nreloc 29 nlnno 0
-[487](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[486](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[489](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .bss
+[488](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000800 .bss
 AUX scnlen 0x2a0 nreloc 0 nlnno 0
-[491](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .xdata
+[490](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000388 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[493](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003f0 .pdata
+[492](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003f0 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[495](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003f0 .rdata
+[494](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000410 .rdata
 AUX scnlen 0x7 nreloc 0 nlnno 0
-[497](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000205 tlsthrd.c
+[496](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000204 tlsthrd.c
 File 
-[499](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005280 __mingwthr_run_key_dtors.part.0
+[498](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000051c0 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[501](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000ae0 __mingwthr_cs
-[502](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000ac0 key_dtor_list
-[503](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052f0 ___w64_mingwthr_add_key_dtor
-[504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000ac8 __mingwthr_cs_init
-[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005370 ___w64_mingwthr_remove_key_dtor
-[506](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005410 __mingw_TLScallback
-[507](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005280 .text
+[500](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000ac0 __mingwthr_cs
+[501](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000aa0 key_dtor_list
+[502](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005230 ___w64_mingwthr_add_key_dtor
+[503](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000aa8 __mingwthr_cs_init
+[504](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052b0 ___w64_mingwthr_remove_key_dtor
+[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005350 __mingw_TLScallback
+[506](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000051c0 .text
 AUX scnlen 0x26a nreloc 39 nlnno 0
-[509](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[508](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[511](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000ac0 .bss
+[510](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000aa0 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[513](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .xdata
+[512](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
-[515](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000414 .pdata
+[514](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000414 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
-[517](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020d tlsmcrt.c
+[516](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020c tlsmcrt.c
 File 
-[519](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
+[518](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005430 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[521](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
+[520](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[523](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b20 .bss
+[522](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[525](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000215 pseudo-reloc-list.c
+[524](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000214 pseudo-reloc-list.c
 File 
-[527](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
+[526](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005430 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[529](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[528](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[531](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b20 .bss
+[530](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
-[533](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022c pesect.c
+[532](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022b pesect.c
 File 
-[535](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000054f0 _ValidateImageBase.part.0
+[534](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005430 _ValidateImageBase.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[537](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005510 _ValidateImageBase
-[538](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005530 _FindPESection
-[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005580 _FindPESectionByName
-[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005610 __mingw_GetSectionForAddress
-[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005690 __mingw_GetSectionCount
-[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000056d0 _FindPESectionExec
-[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005740 _GetPEImageBase
-[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005780 _IsNonwritableInCurrentImage
-[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005820 __mingw_enum_import_library_names
-[546](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
+[536](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005450 _ValidateImageBase
+[537](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005470 _FindPESection
+[538](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054c0 _FindPESectionByName
+[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005550 __mingw_GetSectionForAddress
+[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000055d0 __mingw_GetSectionCount
+[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005610 _FindPESectionExec
+[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005680 _GetPEImageBase
+[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000056c0 _IsNonwritableInCurrentImage
+[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005760 __mingw_enum_import_library_names
+[545](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005430 .text
 AUX scnlen 0x3d6 nreloc 9 nlnno 0
-[548](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[547](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[550](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[549](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[552](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d0 .xdata
+[551](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003d8 .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
-[554](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000444 .pdata
+[553](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000444 .pdata
 AUX scnlen 0x78 nreloc 30 nlnno 0
-[556](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023b CRT_fp10.c
+[555](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023a CRT_fp10.c
 File 
-[558](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000058d0 _fpreset
+[557](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005810 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000058d0 fpreset
-[561](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000058d0 .text
+[559](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005810 fpreset
+[560](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005810 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
-[563](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[562](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[565](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[564](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[567](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000418 .xdata
+[566](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[569](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
+[568](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[571](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000024f fake
+[570](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000024e fake
 File 
-[573](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
+[572](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
 AUX scnlen 0x2e nreloc 7 nlnno 0
-[575](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
+[574](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
 AUX scnlen 0x14 nreloc 0 nlnno 0
-[577](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
+[576](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
 AUX scnlen 0x7b nreloc 1 nlnno 0
-[579](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000058e0 .text
+[578](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005820 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
-[581](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[580](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[583](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[582](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[585](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
+[584](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
-[587](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
+[586](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
 AUX scnlen 0x9b nreloc 0 nlnno 0
-[589](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
+[588](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
 AUX scnlen 0x48 nreloc 2 nlnno 0
-[591](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000025f libgcc2.c
+[590](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000025e libgcc2.c
 File 
-[593](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005920 .text
+[592](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005860 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[595](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[594](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[597](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[596](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[599](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
+[598](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
 AUX scnlen 0x1eda nreloc 4 nlnno 0
-[601](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .debug_abbrev
+[600](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .debug_abbrev
 AUX scnlen 0x135 nreloc 0 nlnno 0
-[603](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
+[602](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
 AUX scnlen 0x20 nreloc 1 nlnno 0
-[605](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
+[604](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
 AUX scnlen 0x1a7 nreloc 0 nlnno 0
-[607](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000026d dllentry.c
+[606](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000026c dllentry.c
 File 
-[609](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005920 DllEntryPoint
+[608](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005860 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[611](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005920 .text
+[610](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005860 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
-[613](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[612](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[615](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[614](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[617](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000041c .xdata
+[616](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000424 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[619](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
+[618](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[621](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027b dllmain.c
+[620](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027a dllmain.c
 File 
-[623](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005930 DllMain
+[622](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005870 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[625](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005930 .text
+[624](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005870 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
-[627](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[626](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[629](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[628](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[631](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .xdata
+[630](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000428 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[633](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
+[632](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[635](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028b sqrt.c
+[634](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028a sqrt.c
 File 
-[637](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005940 sqrt
+[636](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005880 sqrt
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[639](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005940 .text
+[638](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005880 .text
 AUX scnlen 0x126 nreloc 10 nlnno 0
-[641](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[640](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[643](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[642](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[645](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000400 .rdata
+[644](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[647](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000424 .xdata
+[646](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000042c .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[649](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
+[648](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[651](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000299 vsnprintf.c
+[650](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000298 vsnprintf.c
 File 
-[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005a70 __ms_vsnprintf
+[652](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000059b0 __ms_vsnprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005a70 .text
+[654](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000059b0 .text
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[657](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[656](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[659](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[658](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[661](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000430 .xdata
+[660](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000438 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[663](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
+[662](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[665](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a9 cos.c
+[664](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a8 cos.c
 File 
-[667](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005a80 cos
+[666](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000059c0 cos
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[669](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005a80 .text
+[668](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000059c0 .text
 AUX scnlen 0xf4 nreloc 8 nlnno 0
-[671](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[670](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[673](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[672](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[675](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000430 .rdata
+[674](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000450 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[677](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000434 .xdata
+[676](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000043c .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[679](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
+[678](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[681](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002b3 cosl_internal.S
+[680](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002b2 cosl_internal.S
 File 
-[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005b80 __cosl_internal
+[682](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005ac0 __cosl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[685](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005b80 .text
+[684](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ac0 .text
 AUX scnlen 0x30 nreloc 0 nlnno 0
-[687](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[686](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[689](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[688](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[691](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c5 exp.c
+[690](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c4 exp.c
 File 
-[693](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005bb0 exp
+[692](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005af0 exp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[695](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
-[696](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
-[697](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005bb0 .text
+[694](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
+[695](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
+[696](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005af0 .text
 AUX scnlen 0x1e4 nreloc 17 nlnno 0
-[699](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
+[698](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[701](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[700](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[703](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .rdata
+[702](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[705](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .xdata
+[704](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000448 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[707](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
+[706](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[709](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d5 log.c
+[708](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d4 log.c
 File 
-[711](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005da0 log
+[710](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005ce0 log
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[713](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005da0 .text
+[712](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ce0 .text
 AUX scnlen 0x120 nreloc 11 nlnno 0
-[715](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[714](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[717](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[716](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[719](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000470 .rdata
+[718](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .rdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[721](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000044c .xdata
+[720](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000454 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[723](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
+[722](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[725](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002e6 pow.c
+[724](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002e5 pow.c
 File 
-[727](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005ec0 internal_modf
+[726](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005e00 internal_modf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[729](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005f60 pow
-[730](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ec0 .text
+[728](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005ea0 pow
+[729](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005e00 .text
 AUX scnlen 0x5f7 nreloc 31 nlnno 0
-[732](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[731](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[734](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[733](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[736](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000458 .xdata
+[735](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
-[738](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
+[737](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[740](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .rdata
+[739](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b0 .rdata
 AUX scnlen 0x80 nreloc 0 nlnno 0
-[742](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f6 powi.c
+[741](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002f5 powi.c
 File 
-[744](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064c0 __powi
+[743](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006400 __powi
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[746](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064c0 .text
+[745](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006400 .text
 AUX scnlen 0x27e nreloc 15 nlnno 0
-[748](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[747](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[750](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[749](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[752](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .rdata
+[751](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000530 .rdata
 AUX scnlen 0x60 nreloc 0 nlnno 0
-[754](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000047c .xdata
+[753](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000484 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
-[756](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000534 .pdata
+[755](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000534 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[758](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000300 exp2l.S
+[757](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ff exp2l.S
 File 
-[760](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006740 exp2l
+[759](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006680 exp2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[762](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006740 .text
+[761](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006680 .text
 AUX scnlen 0x68 nreloc 0 nlnno 0
-[764](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[763](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[766](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[765](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[768](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000030c internal_logl.S
+[767](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000030b internal_logl.S
 File 
-[770](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b0 one
-[771](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b8 limit
-[772](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000067c0 __logl_internal
+[769](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000066f0 one
+[770](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000066f8 limit
+[771](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006700 __logl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[774](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000067b0 .text
+[773](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000066f0 .text
 AUX scnlen 0x51 nreloc 0 nlnno 0
-[776](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[775](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[778](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[777](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[780](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000031a ldexp.c
+[779](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000319 ldexp.c
 File 
-[782](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006810 ldexp
+[781](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006750 ldexp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[784](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006810 .text
+[783](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006750 .text
 AUX scnlen 0xbe nreloc 1 nlnno 0
-[786](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[785](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[788](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[787](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[790](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000488 .xdata
+[789](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[792](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000540 .pdata
+[791](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000540 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[794](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003b9 log2l.S
+[793](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003b8 log2l.S
 File 
-[796](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d0 one
-[797](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d8 limit
-[798](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000068e0 log2l
+[795](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006810 one
+[796](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000006818 limit
+[797](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006820 log2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[800](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068d0 .text
+[799](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006810 .text
 AUX scnlen 0x6c nreloc 0 nlnno 0
-[802](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[801](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[804](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[803](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[806](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
-[807](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[808](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[809](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
-[810](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
-[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
-[812](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
-[813](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
-[814](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[815](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[816](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
-[817](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
-[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
-[819](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
-[820](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
-[821](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[822](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[823](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
-[824](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
-[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
-[826](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
-[827](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006958 .text
-[828](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[829](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[830](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
-[831](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
-[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
-[833](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
-[834](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006960 .text
-[835](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[836](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[837](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
-[838](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
-[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
-[840](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
-[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006968 .text
-[842](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[843](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[844](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
-[845](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
-[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
-[847](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
-[848](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006970 .text
-[849](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[850](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
-[852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
-[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
-[854](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
-[855](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006978 .text
-[856](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[857](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
-[859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
-[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
-[861](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
-[862](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006980 .text
-[863](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[864](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
-[866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
-[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
-[868](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
-[869](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006988 .text
-[870](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[871](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
-[873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
-[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
-[875](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
-[876](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006990 .text
-[877](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[878](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
-[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
-[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
-[882](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
-[883](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006998 .text
-[884](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[885](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
-[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
-[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
-[889](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
-[890](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a0 .text
-[891](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[892](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
-[894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
-[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
-[896](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
-[897](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a8 .text
-[898](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[899](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
-[901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
-[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
-[903](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
-[904](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b0 .text
-[905](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[906](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
-[908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
-[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
-[910](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
-[911](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b8 .text
-[912](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[913](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
-[915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
-[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
-[917](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
-[918](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c0 .text
-[919](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[920](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
-[922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
-[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
-[924](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
-[925](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c8 .text
-[926](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[927](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
-[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
-[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
-[931](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
-[932](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d0 .text
-[933](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[934](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
-[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
-[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
-[938](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
-[939](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d8 .text
-[940](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[941](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
-[943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
-[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
-[945](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
-[946](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069e0 .text
-[947](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
-[948](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
-[950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
-[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
-[952](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
-[953](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003c9 onexit_table.c
+[805](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006880 .text
+[806](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[807](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[808](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
+[809](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
+[810](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
+[811](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
+[812](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006888 .text
+[813](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[814](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[815](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
+[816](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
+[817](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
+[818](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
+[819](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006890 .text
+[820](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[821](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[822](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
+[823](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
+[824](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
+[825](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
+[826](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006898 .text
+[827](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[828](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[829](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
+[830](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
+[831](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
+[832](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
+[833](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a0 .text
+[834](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[835](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[836](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
+[837](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
+[838](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
+[839](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
+[840](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a8 .text
+[841](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[842](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[843](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
+[844](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
+[845](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
+[846](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
+[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b0 .text
+[848](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[849](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[850](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
+[851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
+[852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
+[853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
+[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b8 .text
+[855](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[856](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[857](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
+[858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
+[859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
+[860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
+[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c0 .text
+[862](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[863](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[864](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
+[865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
+[866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
+[867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
+[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c8 .text
+[869](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[870](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[871](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
+[872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
+[873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
+[874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
+[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d0 .text
+[876](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[877](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[878](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
+[879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
+[880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
+[881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
+[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d8 .text
+[883](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[884](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[885](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
+[886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
+[887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
+[888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
+[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e0 .text
+[890](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[891](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[892](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
+[893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
+[894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
+[895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
+[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e8 .text
+[897](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[899](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
+[900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
+[901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
+[902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
+[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f0 .text
+[904](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[906](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
+[907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
+[908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
+[909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
+[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f8 .text
+[911](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[912](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[913](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
+[914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
+[915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
+[916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
+[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006900 .text
+[918](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[919](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[920](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
+[921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
+[922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
+[923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
+[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006908 .text
+[925](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[926](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[927](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
+[928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
+[929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
+[930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
+[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006910 .text
+[932](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[933](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[934](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
+[935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
+[936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
+[937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
+[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006918 .text
+[939](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[940](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[941](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
+[942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
+[943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
+[944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
+[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006920 .text
+[946](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
+[947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[948](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
+[949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
+[950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
+[951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
+[952](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003c8 onexit_table.c
 File 
-[955](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000069f0 _initialize_onexit_table
+[954](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006930 _initialize_onexit_table
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[957](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a20 _register_onexit_function
-[958](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006af0 _execute_onexit_table
-[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000069f0 .text
+[956](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006960 _register_onexit_function
+[957](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a30 _execute_onexit_table
+[958](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006930 .text
 AUX scnlen 0x16f nreloc 8 nlnno 0
-[961](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
+[960](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x18 nreloc 3 nlnno 0
-[963](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[962](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[965](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
+[964](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000498 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[967](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
+[966](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[969](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d7 acrt_iob_func.c
+[968](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003d6 acrt_iob_func.c
 File 
-[971](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006b60 __acrt_iob_func
+[970](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006aa0 __acrt_iob_func
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b60 .text
+[972](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006aa0 .text
 AUX scnlen 0x1f nreloc 1 nlnno 0
-[975](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
+[974](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[977](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[976](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[979](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b0 .xdata
+[978](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b8 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[981](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .pdata
+[980](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[983](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000401 fake
+[982](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000400 fake
 File 
-[985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
-[986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
-[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b80 .text
+[984](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
+[985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
+[986](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ac0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[989](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[988](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[991](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[990](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
+[992](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
-[995](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
-[996](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[997](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b80 .text
-[998](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[999](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
-[1001](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
-[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
-[1003](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
-[1004](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b88 .text
-[1005](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1006](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
-[1008](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
-[1009](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
-[1010](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
-[1011](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b90 .text
-[1012](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1013](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
-[1015](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
-[1016](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
-[1017](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
-[1018](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b98 .text
-[1019](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1020](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1021](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
-[1022](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[1023](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
-[1024](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
-[1025](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004a2 fake
+[994](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
+[995](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
+[996](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ac0 .text
+[997](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[998](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[999](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
+[1000](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
+[1001](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
+[1002](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
+[1003](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ac8 .text
+[1004](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1005](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1006](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
+[1007](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
+[1008](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
+[1009](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
+[1010](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ad0 .text
+[1011](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1012](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1013](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
+[1014](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
+[1015](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
+[1016](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
+[1017](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ad8 .text
+[1018](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1019](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1020](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
+[1021](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
+[1022](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
+[1023](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
+[1024](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004a1 fake
 File 
-[1027](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ba0 .text
+[1026](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ae0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1029](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1028](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1031](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[1030](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1033](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
+[1032](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1035](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
+[1034](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
+[1036](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
 AUX scnlen 0xb nreloc 0 nlnno 0
-[1039](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba0 .text
-[1040](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1041](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
-[1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
-[1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
-[1045](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
-[1046](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba8 .text
-[1047](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1048](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
-[1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
-[1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
-[1052](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
-[1053](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb0 .text
-[1054](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1055](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
-[1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
-[1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
-[1059](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
-[1060](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb8 .text
-[1061](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1062](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
-[1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
-[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
-[1066](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
-[1067](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc0 .text
-[1068](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1069](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1070](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
-[1071](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
-[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
-[1073](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
-[1074](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc8 .text
-[1075](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1076](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1077](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
-[1078](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
-[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
-[1080](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
-[1081](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd0 .text
-[1082](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1083](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
-[1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
-[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
-[1087](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
-[1088](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd8 .text
-[1089](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1090](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
-[1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
-[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
-[1094](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
-[1095](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be0 .text
-[1096](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1097](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
-[1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
-[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
-[1101](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
-[1102](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be8 .text
-[1103](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1104](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
-[1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
-[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
-[1108](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
-[1109](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf0 .text
-[1110](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1111](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
-[1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
-[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
-[1115](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
-[1116](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf8 .text
-[1117](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1118](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
-[1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
-[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
-[1122](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
-[1123](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c00 .text
-[1124](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1125](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
-[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
-[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
-[1129](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
-[1130](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c08 .text
-[1131](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1132](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
-[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
-[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
-[1136](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
-[1137](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c10 .text
-[1138](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1139](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
-[1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
-[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
-[1143](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
-[1144](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c18 .text
-[1145](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1146](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
-[1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
-[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
-[1150](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
-[1151](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c20 .text
-[1152](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1153](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
-[1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
-[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
-[1157](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
-[1158](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c28 .text
-[1159](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1160](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
-[1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
-[1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
-[1164](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
-[1165](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c30 .text
-[1166](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1167](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
-[1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
-[1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
-[1171](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
-[1172](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c38 .text
-[1173](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1174](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
-[1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
-[1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
-[1178](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
-[1179](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c40 .text
-[1180](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1181](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 .bss
-[1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
-[1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
-[1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
-[1185](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
-[1186](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004bc merr.c
+[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ae0 .text
+[1039](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1041](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
+[1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
+[1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
+[1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
+[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ae8 .text
+[1046](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1048](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
+[1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
+[1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
+[1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
+[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006af0 .text
+[1053](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1054](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1055](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
+[1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
+[1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
+[1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
+[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006af8 .text
+[1060](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1061](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1062](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
+[1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
+[1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
+[1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
+[1066](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b00 .text
+[1067](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1068](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1069](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
+[1070](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
+[1071](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
+[1072](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
+[1073](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b08 .text
+[1074](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1075](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1076](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
+[1077](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
+[1078](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
+[1079](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
+[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b10 .text
+[1081](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1082](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1083](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
+[1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
+[1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
+[1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
+[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b18 .text
+[1088](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1089](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1090](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
+[1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
+[1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
+[1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
+[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b20 .text
+[1095](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1096](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1097](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
+[1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
+[1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
+[1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
+[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b28 .text
+[1102](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1103](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1104](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
+[1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
+[1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
+[1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
+[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b30 .text
+[1109](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1111](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
+[1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
+[1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
+[1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
+[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b38 .text
+[1116](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1117](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1118](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
+[1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
+[1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
+[1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
+[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b40 .text
+[1123](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1124](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1125](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
+[1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
+[1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
+[1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
+[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b48 .text
+[1130](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1131](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1132](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
+[1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
+[1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
+[1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
+[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b50 .text
+[1137](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1139](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
+[1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
+[1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
+[1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
+[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b58 .text
+[1144](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1146](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
+[1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
+[1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
+[1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
+[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b60 .text
+[1151](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1153](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
+[1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
+[1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
+[1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
+[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b68 .text
+[1158](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1160](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
+[1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
+[1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
+[1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
+[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b70 .text
+[1165](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1166](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1167](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
+[1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
+[1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
+[1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
+[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b78 .text
+[1172](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1173](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1174](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
+[1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
+[1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
+[1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
+[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b80 .text
+[1179](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1180](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 .bss
+[1181](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
+[1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
+[1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
+[1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
+[1185](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004bb merr.c
 File 
-[1188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006c50 __mingw_raise_matherr
+[1187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006b90 __mingw_raise_matherr
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1190](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b30 stUserMathErr
-[1191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ca0 __mingw_setusermatherr
-[1192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006cb0 _matherr
-[1193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006c50 .text
+[1189](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b10 stUserMathErr
+[1190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006be0 __mingw_setusermatherr
+[1191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006bf0 _matherr
+[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b90 .text
 AUX scnlen 0x15c nreloc 14 nlnno 0
-[1195](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1194](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1197](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b30 .bss
+[1196](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b10 .bss
 AUX scnlen 0x8 nreloc 0 nlnno 0
-[1199](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004b8 .xdata
+[1198](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
-[1201](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000057c .pdata
+[1200](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000057c .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[1203](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000570 .rdata
+[1202](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000590 .rdata
 AUX scnlen 0x140 nreloc 7 nlnno 0
-[1205](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006db0 .text
-[1206](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
-[1207](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b40 .bss
-[1208](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
-[1209](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
-[1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
-[1211](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
-[1212](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004ce cygming-crtend.c
+[1204](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006cf0 .text
+[1205](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
+[1206](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b20 .bss
+[1207](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
+[1208](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
+[1209](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
+[1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
+[1211](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004cd cygming-crtend.c
 File 
-[1214](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006e30 register_frame_ctor
+[1213](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006d70 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1216](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text
+[1215](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d00 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1218](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
+[1217](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1220](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b40 .bss
+[1219](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b20 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1222](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e30 .text.startup
+[1221](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d70 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
-[1224](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004dc .xdata.startup
+[1223](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e4 .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
-[1226](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .pdata.startup
+[1225](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005a0 .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1228](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e48 .ctors.65535
+[1227](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006d88 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[1230](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
-[1231](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 ___RUNTIME_PSEUDO_RELOC_LIST__
-[1232](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
-[1233](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
-[1234](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
-[1235](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1236](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 ___DTOR_LIST__
-[1237](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
-[1238](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006960 printf
-[1239](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
-[1240](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
-[1241](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc8 SetUnhandledExceptionFilter
-[1242](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c0 _vsnprintf
-[1243](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
-[1244](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b90 _lock
-[1245](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c8 _mkdir
-[1246](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
-[1247](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000730 .refptr.__native_startup_state
-[1248](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
-[1249](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1250](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c18 GetLastError
-[1251](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c10 GetSystemTimeAsFileTime
-[1252](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007e0 mingw_initltssuo_force
-[1253](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 __rt_psrelocs_start
-[1254](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
-[1255](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b98 __iob_func
-[1257](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
-[1258](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
-[1259](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
-[1260](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
-[1261](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
-[1262](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
-[1263](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006c0 .refptr.__CTOR_LIST__
-[1264](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba0 VirtualQuery
-[1265](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
-[1266](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
-[1267](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
-[1268](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
-[1269](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1270](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006968 perror
-[1271](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
-[1272](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000820 __mingw_oldexcpt_handler
-[1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
-[1274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006970 malloc
-[1275](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c28 GetCurrentProcessId
-[1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
-[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb8 TlsGetValue
-[1278](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc0 TerminateProcess
-[1279](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
-[1280](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1281](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd8 RtlLookupFunctionEntry
-[1282](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
-[1283](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
-[1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
-[1285](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
-[1286](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba8 VirtualProtect
-[1287](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007f0 mingw_app_type
-[1288](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
-[1289](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
-[1290](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
-[1291](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b8 abort
-[1292](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
-[1293](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
-[1294](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
-[1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
-[1296](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
-[1297](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c38 EnterCriticalSection
-[1298](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000760 .refptr.__xi_a
-[1299](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
-[1300](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006b0 .refptr._CRT_MT
-[1301](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be0 RtlCaptureContext
-[1302](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
-[1303](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
-[1304](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b0 calloc
-[1305](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 _tls_used
-[1306](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb0 UnhandledExceptionFilter
-[1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
-[1308](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 __RUNTIME_PSEUDO_RELOC_LIST__
-[1309](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006990 fprintf
-[1310](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
-[1311](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000045d0 Sleep
-[1312](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
-[1313](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
-[1314](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 __CTOR_LIST__
-[1315](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
-[1316](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b50 __bss_end__
-[1317](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c08 GetTickCount
-[1319](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
-[1320](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
-[1321](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be8 RtlAddFunctionTable
-[1323](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000720 .refptr.__native_startup_lock
-[1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
-[1325](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007ec _tls_index
-[1326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006958 signal
-[1327](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b40 __native_startup_state
-[1328](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
-[1329](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
-[1330](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006948 strncmp
-[1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
-[1332](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
-[1333](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 ___CTOR_LIST__
-[1334](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006f0 .refptr.__dyn_tls_init_callback
-[1335](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
-[1336](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006978 log10
-[1337](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
-[1338](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b80 realloc
-[1339](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
-[1340](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
-[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
-[1342](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
-[1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
-[1344](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
-[1345](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
-[1346](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c00 InitializeCriticalSection
-[1347](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
-[1348](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006998 fopen
-[1349](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
-[1350](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1351](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a0 fclose
-[1352](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
-[1353](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
-[1354](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
-[1355](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
-[1356](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
-[1357](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000780 .refptr.mingw_app_type
-[1358](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
-[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 __DTOR_LIST__
-[1360](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd0 RtlVirtualUnwind
-[1361](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
-[1362](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
-[1363](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
-[1364](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf8 LeaveCriticalSection
-[1365](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
-[1366](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
-[1367](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
-[1368](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
-[1369](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1370](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069e0 _amsg_exit
-[1371](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
-[1372](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
-[1373](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c30 GetCurrentProcess
-[1374](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
-[1375](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006db0 __setusermatherr
-[1376](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
-[1377](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
-[1378](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
-[1379](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1380](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf0 QueryPerformanceCounter
-[1381](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
-[1382](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
-[1383](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007e4 mingw_initltsdyn_force
-[1384](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
-[1385](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
-[1386](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000280 __dyn_tls_init_callback
-[1387](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000700 .refptr.__image_base__
-[1388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d0 _initterm
-[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006980 fwrite
-[1390](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
-[1391](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
-[1392](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
-[1393](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
-[1394](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1395](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000058e0 ___chkstk_ms
-[1396](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b48 __native_startup_lock
-[1397](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000710 .refptr.__native_dllmain_reason
-[1398](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
-[1399](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c20 GetCurrentThreadId
-[1400](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 __rt_psrelocs_end
-[1401](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a8 exit
-[1402](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
-[1403](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
-[1404](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
-[1405](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d8 _errno
-[1406](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007e8 mingw_initltsdrot_force
-[1407](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
-[1408](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000740 .refptr.__xc_a
-[1409](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006950 strlen
-[1410](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000770 .refptr.__xi_z
-[1411](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c40 DeleteCriticalSection
-[1412](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
-[1413](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009d0 __RUNTIME_PSEUDO_RELOC_LIST_END__
-[1414](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
-[1415](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b88 _unlock
-[1416](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
-[1417](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000750 .refptr.__xc_z
-[1418](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1419](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006940 vfprintf
-[1420](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006988 free
-[1421](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
+[1229](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
+[1230](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 ___RUNTIME_PSEUDO_RELOC_LIST__
+[1231](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
+[1232](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
+[1233](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
+[1234](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
+[1235](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006d98 ___DTOR_LIST__
+[1236](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
+[1237](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a0 printf
+[1238](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
+[1239](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
+[1240](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b08 SetUnhandledExceptionFilter
+[1241](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006900 _vsnprintf
+[1242](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
+[1243](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ad0 _lock
+[1244](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006908 _mkdir
+[1245](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
+[1246](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000750 .refptr.__native_startup_state
+[1247](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
+[1248](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
+[1249](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b58 GetLastError
+[1250](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 GetSystemTimeAsFileTime
+[1251](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007c0 mingw_initltssuo_force
+[1252](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 __rt_psrelocs_start
+[1253](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
+[1254](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
+[1255](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ad8 __iob_func
+[1256](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
+[1257](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
+[1258](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
+[1259](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
+[1260](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
+[1261](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
+[1262](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006e0 .refptr.__CTOR_LIST__
+[1263](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ae0 VirtualQuery
+[1264](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
+[1265](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
+[1266](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
+[1267](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
+[1268](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
+[1269](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a8 perror
+[1270](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000700 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[1271](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000800 __mingw_oldexcpt_handler
+[1272](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
+[1273](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068b0 malloc
+[1274](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 GetCurrentProcessId
+[1275](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
+[1276](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006af8 TlsGetValue
+[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b00 TerminateProcess
+[1278](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
+[1279](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
+[1280](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b18 RtlLookupFunctionEntry
+[1281](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
+[1282](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
+[1283](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
+[1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
+[1285](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ae8 VirtualProtect
+[1286](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007d0 mingw_app_type
+[1287](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
+[1288](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
+[1289](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
+[1290](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068f8 abort
+[1291](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006f0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[1292](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
+[1293](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
+[1294](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
+[1295](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
+[1296](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b78 EnterCriticalSection
+[1297](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000780 .refptr.__xi_a
+[1298](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
+[1299](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006d0 .refptr._CRT_MT
+[1300](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b20 RtlCaptureContext
+[1301](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
+[1302](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
+[1303](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068f0 calloc
+[1304](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c0 _tls_used
+[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006af0 UnhandledExceptionFilter
+[1306](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
+[1307](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 __RUNTIME_PSEUDO_RELOC_LIST__
+[1308](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068d0 fprintf
+[1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
+[1310](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000004510 Sleep
+[1311](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
+[1312](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
+[1313](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006d80 __CTOR_LIST__
+[1314](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
+[1315](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b30 __bss_end__
+[1316](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
+[1317](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b48 GetTickCount
+[1318](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
+[1319](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
+[1320](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
+[1321](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b28 RtlAddFunctionTable
+[1322](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000740 .refptr.__native_startup_lock
+[1323](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
+[1324](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007cc _tls_index
+[1325](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006898 signal
+[1326](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b20 __native_startup_state
+[1327](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
+[1328](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
+[1329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006888 strncmp
+[1330](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
+[1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
+[1332](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006d80 ___CTOR_LIST__
+[1333](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000710 .refptr.__dyn_tls_init_callback
+[1334](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
+[1335](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068b8 log10
+[1336](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
+[1337](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ac0 realloc
+[1338](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
+[1339](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
+[1340](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
+[1341](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
+[1342](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
+[1343](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
+[1344](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
+[1345](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b40 InitializeCriticalSection
+[1346](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
+[1347](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068d8 fopen
+[1348](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
+[1349](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
+[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068e0 fclose
+[1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
+[1352](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
+[1353](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
+[1354](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
+[1355](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
+[1356](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007a0 .refptr.mingw_app_type
+[1357](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
+[1358](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006d98 __DTOR_LIST__
+[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b10 RtlVirtualUnwind
+[1360](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
+[1361](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
+[1362](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
+[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b38 LeaveCriticalSection
+[1364](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
+[1365](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
+[1366](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
+[1367](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
+[1368](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
+[1369](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006920 _amsg_exit
+[1370](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
+[1371](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
+[1372](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b70 GetCurrentProcess
+[1373](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
+[1374](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006cf0 __setusermatherr
+[1375](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
+[1376](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
+[1377](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
+[1378](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
+[1379](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b30 QueryPerformanceCounter
+[1380](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
+[1381](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
+[1382](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007c4 mingw_initltsdyn_force
+[1383](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
+[1384](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
+[1385](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a0 __dyn_tls_init_callback
+[1386](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000720 .refptr.__image_base__
+[1387](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006910 _initterm
+[1388](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068c0 fwrite
+[1389](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
+[1390](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
+[1391](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
+[1392](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
+[1393](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
+[1394](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000005820 ___chkstk_ms
+[1395](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b28 __native_startup_lock
+[1396](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000730 .refptr.__native_dllmain_reason
+[1397](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
+[1398](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b60 GetCurrentThreadId
+[1399](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 __rt_psrelocs_end
+[1400](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068e8 exit
+[1401](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
+[1402](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
+[1403](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
+[1404](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006918 _errno
+[1405](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000007c8 mingw_initltsdrot_force
+[1406](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
+[1407](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000760 .refptr.__xc_a
+[1408](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006890 strlen
+[1409](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000790 .refptr.__xi_z
+[1410](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b80 DeleteCriticalSection
+[1411](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
+[1412](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000009f0 __RUNTIME_PSEUDO_RELOC_LIST_END__
+[1413](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
+[1414](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ac8 _unlock
+[1415](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
+[1416](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000770 .refptr.__xc_z
+[1417](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
+[1418](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006880 vfprintf
+[1419](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068c8 free
+[1420](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
 
 
 
 Disassembly of section .text:
 
 00000000646c1000 <pre_c_init>:
     646c1000:	lea    0xaff9(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c1007:	jmp    646c79f0 <_initialize_onexit_table>
+    646c1007:	jmp    646c7930 <_initialize_onexit_table>
     646c100c:	nopl   0x0(%rax)
 
 00000000646c1010 <_CRT_INIT>:
     646c1010:	push   %r13
     646c1012:	push   %r12
     646c1014:	push   %rbp
     646c1015:	push   %rdi
@@ -2575,74 +2577,74 @@
     646c1021:	mov    %r8,%r13
     646c1024:	jne    646c10a0 <_CRT_INIT+0x90>
     646c1026:	mov    0xafec(%rip),%edx        # 646cc018 <__proc_attached>
     646c102c:	xor    %eax,%eax
     646c102e:	test   %edx,%edx
     646c1030:	jle    646c108b <_CRT_INIT+0x7b>
     646c1032:	sub    $0x1,%edx
-    646c1035:	mov    0x86e4(%rip),%rbx        # 646c9720 <.refptr.__native_startup_lock>
+    646c1035:	mov    0x8704(%rip),%rbx        # 646c9740 <.refptr.__native_startup_lock>
     646c103c:	xor    %ebp,%ebp
     646c103e:	mov    $0x1,%edi
     646c1043:	mov    %edx,0xafcf(%rip)        # 646cc018 <__proc_attached>
     646c1049:	mov    0xd1fc(%rip),%r12        # 646ce24c <__imp_Sleep>
     646c1050:	jmp    646c105a <_CRT_INIT+0x4a>
     646c1052:	mov    $0x3e8,%ecx
     646c1057:	call   *%r12
     646c105a:	mov    %rbp,%rax
     646c105d:	lock cmpxchg %rdi,(%rbx)
     646c1062:	test   %rax,%rax
     646c1065:	mov    %rax,%rsi
     646c1068:	jne    646c1052 <_CRT_INIT+0x42>
-    646c106a:	mov    0x86bf(%rip),%rdi        # 646c9730 <.refptr.__native_startup_state>
+    646c106a:	mov    0x86df(%rip),%rdi        # 646c9750 <.refptr.__native_startup_state>
     646c1071:	mov    (%rdi),%eax
     646c1073:	cmp    $0x2,%eax
     646c1076:	je     646c1165 <_CRT_INIT+0x155>
     646c107c:	mov    $0x1f,%ecx
-    646c1081:	call   646c79e0 <_amsg_exit>
+    646c1081:	call   646c7920 <_amsg_exit>
     646c1086:	mov    $0x1,%eax
     646c108b:	add    $0x28,%rsp
     646c108f:	pop    %rbx
     646c1090:	pop    %rsi
     646c1091:	pop    %rdi
     646c1092:	pop    %rbp
     646c1093:	pop    %r12
     646c1095:	pop    %r13
     646c1097:	ret
     646c1098:	nopl   0x0(%rax,%rax,1)
     646c10a0:	cmp    $0x1,%edx
     646c10a3:	jne    646c1153 <_CRT_INIT+0x143>
     646c10a9:	mov    %gs:0x30,%rax
-    646c10b2:	mov    0x8667(%rip),%rbx        # 646c9720 <.refptr.__native_startup_lock>
+    646c10b2:	mov    0x8687(%rip),%rbx        # 646c9740 <.refptr.__native_startup_lock>
     646c10b9:	xor    %edi,%edi
     646c10bb:	mov    0x8(%rax),%rsi
     646c10bf:	mov    0xd186(%rip),%rbp        # 646ce24c <__imp_Sleep>
     646c10c6:	jmp    646c10e0 <_CRT_INIT+0xd0>
     646c10c8:	nopl   0x0(%rax,%rax,1)
     646c10d0:	cmp    %rax,%rsi
     646c10d3:	je     646c1190 <_CRT_INIT+0x180>
     646c10d9:	mov    $0x3e8,%ecx
     646c10de:	call   *%rbp
     646c10e0:	mov    %rdi,%rax
     646c10e3:	lock cmpxchg %rsi,(%rbx)
     646c10e8:	test   %rax,%rax
     646c10eb:	jne    646c10d0 <_CRT_INIT+0xc0>
     646c10ed:	xor    %edi,%edi
-    646c10ef:	mov    0x863a(%rip),%rsi        # 646c9730 <.refptr.__native_startup_state>
+    646c10ef:	mov    0x865a(%rip),%rsi        # 646c9750 <.refptr.__native_startup_state>
     646c10f6:	mov    (%rsi),%eax
     646c10f8:	cmp    $0x1,%eax
     646c10fb:	je     646c11f0 <_CRT_INIT+0x1e0>
     646c1101:	mov    (%rsi),%eax
     646c1103:	test   %eax,%eax
     646c1105:	je     646c11b0 <_CRT_INIT+0x1a0>
     646c110b:	mov    (%rsi),%eax
     646c110d:	cmp    $0x1,%eax
     646c1110:	je     646c11d0 <_CRT_INIT+0x1c0>
     646c1116:	test   %edi,%edi
     646c1118:	je     646c11a0 <_CRT_INIT+0x190>
-    646c111e:	mov    0x85cb(%rip),%rax        # 646c96f0 <.refptr.__dyn_tls_init_callback>
+    646c111e:	mov    0x85eb(%rip),%rax        # 646c9710 <.refptr.__dyn_tls_init_callback>
     646c1125:	mov    (%rax),%rax
     646c1128:	test   %rax,%rax
     646c112b:	je     646c113a <_CRT_INIT+0x12a>
     646c112d:	mov    %r13,%r8
     646c1130:	mov    $0x2,%edx
     646c1135:	mov    %r12,%rcx
     646c1138:	call   *%rax
@@ -2662,15 +2664,15 @@
     646c115d:	pop    %rsi
     646c115e:	pop    %rdi
     646c115f:	pop    %rbp
     646c1160:	pop    %r12
     646c1162:	pop    %r13
     646c1164:	ret
     646c1165:	lea    0xae94(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c116c:	call   646c7af0 <_execute_onexit_table>
+    646c116c:	call   646c7a30 <_execute_onexit_table>
     646c1171:	movl   $0x0,(%rdi)
     646c1177:	xchg   %rsi,(%rbx)
     646c117a:	mov    $0x1,%eax
     646c117f:	add    $0x28,%rsp
     646c1183:	pop    %rbx
     646c1184:	pop    %rsi
     646c1185:	pop    %rdi
@@ -2682,57 +2684,57 @@
     646c1190:	mov    $0x1,%edi
     646c1195:	jmp    646c10ef <_CRT_INIT+0xdf>
     646c119a:	nopw   0x0(%rax,%rax,1)
     646c11a0:	xor    %eax,%eax
     646c11a2:	xchg   %rax,(%rbx)
     646c11a5:	jmp    646c111e <_CRT_INIT+0x10e>
     646c11aa:	nopw   0x0(%rax,%rax,1)
-    646c11b0:	mov    0x85b9(%rip),%rdx        # 646c9770 <.refptr.__xi_z>
+    646c11b0:	mov    0x85d9(%rip),%rdx        # 646c9790 <.refptr.__xi_z>
     646c11b7:	movl   $0x1,(%rsi)
-    646c11bd:	mov    0x859c(%rip),%rcx        # 646c9760 <.refptr.__xi_a>
-    646c11c4:	call   646c79d0 <_initterm>
+    646c11bd:	mov    0x85bc(%rip),%rcx        # 646c9780 <.refptr.__xi_a>
+    646c11c4:	call   646c7910 <_initterm>
     646c11c9:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ce:	xchg   %ax,%ax
-    646c11d0:	mov    0x8579(%rip),%rdx        # 646c9750 <.refptr.__xc_z>
-    646c11d7:	mov    0x8562(%rip),%rcx        # 646c9740 <.refptr.__xc_a>
-    646c11de:	call   646c79d0 <_initterm>
+    646c11d0:	mov    0x8599(%rip),%rdx        # 646c9770 <.refptr.__xc_z>
+    646c11d7:	mov    0x8582(%rip),%rcx        # 646c9760 <.refptr.__xc_a>
+    646c11de:	call   646c7910 <_initterm>
     646c11e3:	movl   $0x2,(%rsi)
     646c11e9:	jmp    646c1116 <_CRT_INIT+0x106>
     646c11ee:	xchg   %ax,%ax
     646c11f0:	mov    $0x1f,%ecx
-    646c11f5:	call   646c79e0 <_amsg_exit>
+    646c11f5:	call   646c7920 <_amsg_exit>
     646c11fa:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ff:	nop
 
 00000000646c1200 <__DllMainCRTStartup>:
     646c1200:	push   %r12
     646c1202:	push   %rbp
     646c1203:	push   %rdi
     646c1204:	push   %rsi
     646c1205:	push   %rbx
     646c1206:	sub    $0x20,%rsp
-    646c120a:	mov    0x84ff(%rip),%rsi        # 646c9710 <.refptr.__native_dllmain_reason>
+    646c120a:	mov    0x851f(%rip),%rsi        # 646c9730 <.refptr.__native_dllmain_reason>
     646c1211:	test   %edx,%edx
     646c1213:	mov    %rcx,%rdi
     646c1216:	mov    %edx,%ebx
     646c1218:	mov    %edx,(%rsi)
     646c121a:	mov    %r8,%rbp
     646c121d:	jne    646c1273 <__DllMainCRTStartup+0x73>
     646c121f:	mov    0xadf3(%rip),%eax        # 646cc018 <__proc_attached>
     646c1225:	test   %eax,%eax
     646c1227:	je     646c125c <__DllMainCRTStartup+0x5c>
-    646c1229:	call   646c5b40 <_pei386_runtime_relocator>
+    646c1229:	call   646c5a80 <_pei386_runtime_relocator>
     646c122e:	mov    %rbp,%r8
     646c1231:	xor    %edx,%edx
     646c1233:	mov    %rdi,%rcx
-    646c1236:	call   646c6930 <DllMain>
+    646c1236:	call   646c6870 <DllMain>
     646c123b:	mov    %rbp,%r8
     646c123e:	mov    %ebx,%edx
     646c1240:	mov    %rdi,%rcx
-    646c1243:	call   646c6920 <DllEntryPoint>
+    646c1243:	call   646c6860 <DllEntryPoint>
     646c1248:	mov    %rbp,%r8
     646c124b:	mov    %ebx,%edx
     646c124d:	mov    %rdi,%rcx
     646c1250:	mov    %eax,%r12d
     646c1253:	call   646c1010 <_CRT_INIT>
     646c1258:	test   %eax,%eax
     646c125a:	jne    646c125f <__DllMainCRTStartup+0x5f>
@@ -2742,94 +2744,94 @@
     646c1268:	add    $0x20,%rsp
     646c126c:	pop    %rbx
     646c126d:	pop    %rsi
     646c126e:	pop    %rdi
     646c126f:	pop    %rbp
     646c1270:	pop    %r12
     646c1272:	ret
-    646c1273:	call   646c5b40 <_pei386_runtime_relocator>
+    646c1273:	call   646c5a80 <_pei386_runtime_relocator>
     646c1278:	lea    -0x1(%rbx),%eax
     646c127b:	cmp    $0x1,%eax
     646c127e:	jbe    646c12a0 <__DllMainCRTStartup+0xa0>
     646c1280:	mov    %rbp,%r8
     646c1283:	mov    %ebx,%edx
     646c1285:	mov    %rdi,%rcx
-    646c1288:	call   646c6930 <DllMain>
+    646c1288:	call   646c6870 <DllMain>
     646c128d:	cmp    $0x3,%ebx
     646c1290:	mov    %eax,%r12d
     646c1293:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c1295:	jmp    646c123b <__DllMainCRTStartup+0x3b>
     646c1297:	nopw   0x0(%rax,%rax,1)
     646c12a0:	mov    %rbp,%r8
     646c12a3:	mov    %ebx,%edx
     646c12a5:	mov    %rdi,%rcx
     646c12a8:	call   646c1010 <_CRT_INIT>
     646c12ad:	test   %eax,%eax
     646c12af:	je     646c125c <__DllMainCRTStartup+0x5c>
     646c12b1:	mov    %rbp,%r8
     646c12b4:	mov    %ebx,%edx
     646c12b6:	mov    %rdi,%rcx
-    646c12b9:	call   646c6920 <DllEntryPoint>
+    646c12b9:	call   646c6860 <DllEntryPoint>
     646c12be:	test   %eax,%eax
     646c12c0:	mov    %eax,%r12d
     646c12c3:	je     646c1320 <__DllMainCRTStartup+0x120>
     646c12c5:	cmp    $0x1,%ebx
     646c12c8:	jne    646c1280 <__DllMainCRTStartup+0x80>
-    646c12ca:	call   646c5690 <__main>
+    646c12ca:	call   646c55d0 <__main>
     646c12cf:	mov    %rbp,%r8
     646c12d2:	mov    $0x1,%edx
     646c12d7:	mov    %rdi,%rcx
-    646c12da:	call   646c6930 <DllMain>
+    646c12da:	call   646c6870 <DllMain>
     646c12df:	test   %eax,%eax
     646c12e1:	mov    %eax,%r12d
     646c12e4:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c12ea:	mov    %rbp,%r8
     646c12ed:	xor    %edx,%edx
     646c12ef:	mov    %rdi,%rcx
-    646c12f2:	call   646c6930 <DllMain>
+    646c12f2:	call   646c6870 <DllMain>
     646c12f7:	mov    %rbp,%r8
     646c12fa:	xor    %edx,%edx
     646c12fc:	mov    %rdi,%rcx
-    646c12ff:	call   646c6920 <DllEntryPoint>
+    646c12ff:	call   646c6860 <DllEntryPoint>
     646c1304:	mov    %rbp,%r8
     646c1307:	xor    %edx,%edx
     646c1309:	mov    %rdi,%rcx
     646c130c:	call   646c1010 <_CRT_INIT>
     646c1311:	jmp    646c125f <__DllMainCRTStartup+0x5f>
     646c1316:	cs nopw 0x0(%rax,%rax,1)
     646c1320:	cmp    $0x1,%ebx
     646c1323:	jne    646c125c <__DllMainCRTStartup+0x5c>
     646c1329:	jmp    646c1304 <__DllMainCRTStartup+0x104>
     646c132b:	nopl   0x0(%rax,%rax,1)
 
 00000000646c1330 <DllMainCRTStartup>:
     646c1330:	sub    $0x48,%rsp
-    646c1334:	mov    0x8445(%rip),%rax        # 646c9780 <.refptr.mingw_app_type>
+    646c1334:	mov    0x8465(%rip),%rax        # 646c97a0 <.refptr.mingw_app_type>
     646c133b:	movl   $0x0,(%rax)
     646c1341:	cmp    $0x1,%edx
     646c1344:	je     646c1350 <DllMainCRTStartup+0x20>
     646c1346:	add    $0x48,%rsp
     646c134a:	jmp    646c1200 <__DllMainCRTStartup>
     646c134f:	nop
     646c1350:	mov    %r8,0x38(%rsp)
     646c1355:	mov    %edx,0x34(%rsp)
     646c1359:	mov    %rcx,0x28(%rsp)
-    646c135e:	call   646c56b0 <__security_init_cookie>
-    646c1363:	call   646c5fa0 <__mingw_init_ehandler>
+    646c135e:	call   646c55f0 <__security_init_cookie>
+    646c1363:	call   646c5ee0 <__mingw_init_ehandler>
     646c1368:	mov    0x38(%rsp),%r8
     646c136d:	mov    0x34(%rsp),%edx
     646c1371:	mov    0x28(%rsp),%rcx
     646c1376:	add    $0x48,%rsp
     646c137a:	jmp    646c1200 <__DllMainCRTStartup>
     646c137f:	nop
 
 00000000646c1380 <atexit>:
     646c1380:	mov    %rcx,%rdx
     646c1383:	lea    0xac76(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c138a:	jmp    646c7a20 <_register_onexit_function>
+    646c138a:	jmp    646c7960 <_register_onexit_function>
     646c138f:	nop
 
 00000000646c1390 <__gcc_register_frame>:
     646c1390:	lea    0x9(%rip),%rcx        # 646c13a0 <__gcc_deregister_frame>
     646c1397:	jmp    646c1380 <atexit>
     646c139c:	nopl   0x0(%rax)
 
@@ -3559,15 +3561,15 @@
     646c1e03:	movapd %xmm6,%xmm0
     646c1e07:	movaps 0x20(%rsp),%xmm6
     646c1e0c:	add    $0x38,%rsp
     646c1e10:	ret
     646c1e11:	pxor   %xmm3,%xmm3
     646c1e15:	pxor   %xmm0,%xmm0
     646c1e19:	jmp    646c1ded <c_array_std_int+0x3d>
-    646c1e1b:	call   646c6940 <sqrt>
+    646c1e1b:	call   646c6880 <sqrt>
     646c1e20:	jmp    646c1e03 <c_array_std_int+0x53>
     646c1e22:	nopl   0x0(%rax)
     646c1e26:	cs nopw 0x0(%rax,%rax,1)
 
 00000000646c1e30 <c_array_std_long_long>:
     646c1e30:	sub    $0x38,%rsp
     646c1e34:	movaps %xmm6,0x20(%rsp)
@@ -3595,15 +3597,15 @@
     646c1e84:	movapd %xmm6,%xmm0
     646c1e88:	movaps 0x20(%rsp),%xmm6
     646c1e8d:	add    $0x38,%rsp
     646c1e91:	ret
     646c1e92:	pxor   %xmm3,%xmm3
     646c1e96:	pxor   %xmm0,%xmm0
     646c1e9a:	jmp    646c1e6e <c_array_std_long_long+0x3e>
-    646c1e9c:	call   646c6940 <sqrt>
+    646c1e9c:	call   646c6880 <sqrt>
     646c1ea1:	jmp    646c1e84 <c_array_std_long_long+0x54>
     646c1ea3:	nopl   (%rax)
     646c1ea6:	cs nopw 0x0(%rax,%rax,1)
 
 00000000646c1eb0 <c_array_std_float>:
     646c1eb0:	sub    $0x38,%rsp
     646c1eb4:	movaps %xmm6,0x20(%rsp)
@@ -3631,15 +3633,15 @@
     646c1f03:	movapd %xmm6,%xmm0
     646c1f07:	movaps 0x20(%rsp),%xmm6
     646c1f0c:	add    $0x38,%rsp
     646c1f10:	ret
     646c1f11:	pxor   %xmm3,%xmm3
     646c1f15:	pxor   %xmm0,%xmm0
     646c1f19:	jmp    646c1eed <c_array_std_float+0x3d>
-    646c1f1b:	call   646c6940 <sqrt>
+    646c1f1b:	call   646c6880 <sqrt>
     646c1f20:	jmp    646c1f03 <c_array_std_float+0x53>
     646c1f22:	nopl   0x0(%rax)
     646c1f26:	cs nopw 0x0(%rax,%rax,1)
 
 00000000646c1f30 <c_array_std_double>:
     646c1f30:	sub    $0x38,%rsp
     646c1f34:	movaps %xmm6,0x20(%rsp)
@@ -3692,15 +3694,15 @@
     646c1fe0:	pxor   %xmm5,%xmm5
     646c1fe4:	pxor   %xmm0,%xmm0
     646c1fe8:	jmp    646c1fba <c_array_std_double+0x8a>
     646c1fea:	xor    %eax,%eax
     646c1fec:	pxor   %xmm5,%xmm5
     646c1ff0:	pxor   %xmm0,%xmm0
     646c1ff4:	jmp    646c1fa7 <c_array_std_double+0x77>
-    646c1ff6:	call   646c6940 <sqrt>
+    646c1ff6:	call   646c6880 <sqrt>
     646c1ffb:	jmp    646c1fd0 <c_array_std_double+0xa0>
     646c1ffd:	nopl   (%rax)
 
 00000000646c2000 <c_array_mean_int>:
     646c2000:	pxor   %xmm0,%xmm0
     646c2004:	pxor   %xmm1,%xmm1
     646c2008:	cvtsi2sd %r8d,%xmm0
@@ -4951,5506 +4953,5481 @@
     646c33af:	pxor   %xmm0,%xmm0
     646c33b3:	movsd  0x5ccd(%rip),%xmm1        # 646c9088 <.rdata+0x38>
     646c33bb:	cvtsi2sd %r9,%xmm0
     646c33c0:	mov    %eax,%eax
     646c33c2:	cvtsi2sd %rax,%xmm6
     646c33c7:	mulsd  %xmm1,%xmm0
     646c33cb:	mulsd  %xmm1,%xmm6
-    646c33cf:	call   646c6da0 <log>
+    646c33cf:	call   646c6ce0 <log>
     646c33d4:	mulsd  0x5cb4(%rip),%xmm0        # 646c9090 <.rdata+0x40>
     646c33dc:	pxor   %xmm1,%xmm1
     646c33e0:	ucomisd %xmm0,%xmm1
     646c33e4:	sqrtsd %xmm0,%xmm7
     646c33e8:	ja     646c340f <mt19937_random_normal+0x7f>
     646c33ea:	mulsd  0x5ca6(%rip),%xmm6        # 646c9098 <.rdata+0x48>
     646c33f2:	movapd %xmm6,%xmm0
-    646c33f6:	call   646c6a80 <cos>
+    646c33f6:	call   646c69c0 <cos>
     646c33fb:	nop
     646c33fc:	movaps 0x20(%rsp),%xmm6
     646c3401:	mulsd  %xmm7,%xmm0
     646c3405:	movaps 0x30(%rsp),%xmm7
     646c340a:	add    $0x48,%rsp
     646c340e:	ret
-    646c340f:	call   646c6940 <sqrt>
+    646c340f:	call   646c6880 <sqrt>
     646c3414:	jmp    646c33ea <mt19937_random_normal+0x5a>
     646c3416:	nop
     646c3417:	nop
     646c3418:	nop
     646c3419:	nop
     646c341a:	nop
     646c341b:	nop
     646c341c:	nop
     646c341d:	nop
     646c341e:	nop
     646c341f:	nop
 
-00000000646c3420 <cov_model_init>:
-    646c3420:	movsd  0x28(%rsp),%xmm0
-    646c3426:	mov    %edx,%eax
-    646c3428:	mov    %edx,(%rcx)
-    646c342a:	cltd
-    646c342b:	movsd  %xmm0,0x18(%rcx)
-    646c3430:	movsd  0x30(%rsp),%xmm0
-    646c3436:	idiv   %r8d
-    646c3439:	mov    %r8d,0x4(%rcx)
-    646c343d:	movsd  %xmm3,0x10(%rcx)
-    646c3442:	movsd  %xmm0,0x20(%rcx)
-    646c3447:	mov    %eax,0x8(%rcx)
-    646c344a:	ret
-    646c344b:	nopl   0x0(%rax,%rax,1)
-
-00000000646c3450 <cov_model>:
-    646c3450:	push   %rbp
-    646c3451:	push   %rdi
-    646c3452:	push   %rsi
-    646c3453:	push   %rbx
-    646c3454:	sub    $0x58,%rsp
-    646c3458:	movaps %xmm6,0x20(%rsp)
-    646c345d:	movaps %xmm7,0x30(%rsp)
-    646c3462:	movaps %xmm8,0x40(%rsp)
-    646c3468:	movsd  0x18(%r9),%xmm6
-    646c346e:	subsd  0x20(%r9),%xmm6
-    646c3474:	test   %r8d,%r8d
-    646c3477:	mov    %r9,%rsi
-    646c347a:	jle    646c34eb <cov_model+0x9b>
-    646c347c:	lea    -0x1(%r8),%eax
-    646c3480:	movsd  0x5c20(%rip),%xmm7        # 646c90a8 <.rdata+0x8>
-    646c3488:	mov    %rcx,%rbx
-    646c348b:	mov    %rdx,%rdi
-    646c348e:	movsd  0x5c09(%rip),%xmm8        # 646c90a0 <.rdata>
-    646c3497:	lea    0x8(%rcx,%rax,8),%rbp
-    646c349c:	nopl   0x0(%rax)
-    646c34a0:	movsd  (%rbx),%xmm0
-    646c34a4:	add    $0x8,%rbx
-    646c34a8:	add    $0x8,%rdi
-    646c34ac:	movsd  0x10(%rsi),%xmm1
-    646c34b1:	mulsd  %xmm0,%xmm0
-    646c34b5:	mulsd  %xmm1,%xmm1
-    646c34b9:	mulsd  %xmm8,%xmm0
-    646c34be:	divsd  %xmm1,%xmm0
-    646c34c2:	call   646c6bb0 <exp>
-    646c34c7:	movapd %xmm7,%xmm1
-    646c34cb:	subsd  %xmm0,%xmm1
-    646c34cf:	movsd  0x18(%rsi),%xmm0
-    646c34d4:	mulsd  %xmm6,%xmm1
-    646c34d8:	subsd  %xmm1,%xmm0
-    646c34dc:	addsd  0x20(%rsi),%xmm0
-    646c34e1:	movsd  %xmm0,-0x8(%rdi)
-    646c34e6:	cmp    %rbx,%rbp
-    646c34e9:	jne    646c34a0 <cov_model+0x50>
-    646c34eb:	movaps 0x20(%rsp),%xmm6
-    646c34f0:	movaps 0x30(%rsp),%xmm7
-    646c34f5:	movaps 0x40(%rsp),%xmm8
-    646c34fb:	add    $0x58,%rsp
-    646c34ff:	pop    %rbx
-    646c3500:	pop    %rsi
-    646c3501:	pop    %rdi
-    646c3502:	pop    %rbp
-    646c3503:	ret
-    646c3504:	xchg   %ax,%ax
-    646c3506:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c3510 <cov_model2d>:
-    646c3510:	push   %r15
-    646c3512:	push   %r14
-    646c3514:	push   %r13
-    646c3516:	push   %r12
-    646c3518:	push   %rbp
-    646c3519:	push   %rdi
-    646c351a:	push   %rsi
-    646c351b:	push   %rbx
-    646c351c:	sub    $0x68,%rsp
-    646c3520:	movaps %xmm6,0x30(%rsp)
-    646c3525:	movaps %xmm7,0x40(%rsp)
-    646c352a:	movaps %xmm8,0x50(%rsp)
-    646c3530:	movsd  0x18(%r9),%xmm6
-    646c3536:	subsd  0x20(%r9),%xmm6
-    646c353c:	test   %r8d,%r8d
-    646c353f:	mov    %rdx,%r14
-    646c3542:	mov    %r8d,%r13d
-    646c3545:	mov    %r9,%r15
-    646c3548:	jle    646c35ec <cov_model2d+0xdc>
-    646c354e:	lea    -0x1(%r8),%eax
-    646c3552:	movsd  0x5b4e(%rip),%xmm7        # 646c90a8 <.rdata+0x8>
-    646c355a:	mov    %rcx,%rsi
-    646c355d:	xor    %r12d,%r12d
-    646c3560:	movsd  0x5b37(%rip),%xmm8        # 646c90a0 <.rdata>
-    646c3569:	lea    0x8(%rcx,%rax,8),%rdx
-    646c356e:	mov    %rdx,0x28(%rsp)
-    646c3573:	lea    0x8(,%rax,8),%rbp
-    646c357b:	nopl   0x0(%rax,%rax,1)
-    646c3580:	movslq %r12d,%rax
-    646c3583:	xor    %ebx,%ebx
-    646c3585:	lea    (%r14,%rax,8),%rdi
-    646c3589:	nopl   0x0(%rax)
-    646c3590:	mov    (%rsi),%rax
-    646c3593:	movsd  0x10(%r15),%xmm1
-    646c3599:	mulsd  %xmm1,%xmm1
-    646c359d:	movsd  (%rax,%rbx,1),%xmm0
-    646c35a2:	mulsd  %xmm0,%xmm0
-    646c35a6:	mulsd  %xmm8,%xmm0
-    646c35ab:	divsd  %xmm1,%xmm0
-    646c35af:	call   646c6bb0 <exp>
-    646c35b4:	movapd %xmm7,%xmm1
-    646c35b8:	subsd  %xmm0,%xmm1
-    646c35bc:	movsd  0x18(%r15),%xmm0
-    646c35c2:	mulsd  %xmm6,%xmm1
-    646c35c6:	subsd  %xmm1,%xmm0
-    646c35ca:	addsd  0x20(%r15),%xmm0
-    646c35d0:	movsd  %xmm0,(%rdi,%rbx,1)
-    646c35d5:	add    $0x8,%rbx
-    646c35d9:	cmp    %rbx,%rbp
-    646c35dc:	jne    646c3590 <cov_model2d+0x80>
-    646c35de:	add    %r13d,%r12d
-    646c35e1:	add    $0x8,%rsi
-    646c35e5:	cmp    %rsi,0x28(%rsp)
-    646c35ea:	jne    646c3580 <cov_model2d+0x70>
-    646c35ec:	movaps 0x30(%rsp),%xmm6
-    646c35f1:	movaps 0x40(%rsp),%xmm7
-    646c35f6:	movaps 0x50(%rsp),%xmm8
-    646c35fc:	add    $0x68,%rsp
-    646c3600:	pop    %rbx
-    646c3601:	pop    %rsi
-    646c3602:	pop    %rdi
-    646c3603:	pop    %rbp
-    646c3604:	pop    %r12
-    646c3606:	pop    %r13
-    646c3608:	pop    %r14
-    646c360a:	pop    %r15
-    646c360c:	ret
-    646c360d:	nop
-    646c360e:	nop
-    646c360f:	nop
-
-00000000646c3610 <sampling_state_init>:
-    646c3610:	push   %rsi
-    646c3611:	push   %rbx
-    646c3612:	sub    $0x38,%rsp
-    646c3616:	movaps %xmm6,0x20(%rsp)
-    646c361b:	movslq %edx,%rsi
-    646c361e:	mov    %rcx,%rbx
-    646c3621:	movq   $0x0,(%rcx)
-    646c3628:	mov    $0x8,%edx
-    646c362d:	movq   %rsi,%xmm6
-    646c3632:	movl   $0x0,0x8(%rcx)
-    646c3639:	punpcklqdq %xmm6,%xmm6
-    646c363d:	movq   $0x0,0x10(%rcx)
-    646c3645:	movups %xmm6,0x20(%rcx)
-    646c3649:	mov    %rsi,%rcx
-    646c364c:	call   646c79b0 <calloc>
-    646c3651:	movups %xmm6,0x38(%rbx)
-    646c3655:	mov    $0x8,%edx
-    646c365a:	mov    %rsi,%rcx
-    646c365d:	mov    %rax,0x18(%rbx)
-    646c3661:	call   646c79b0 <calloc>
-    646c3666:	nop
-    646c3667:	movaps 0x20(%rsp),%xmm6
-    646c366c:	mov    %rax,0x30(%rbx)
-    646c3670:	add    $0x38,%rsp
-    646c3674:	pop    %rbx
-    646c3675:	pop    %rsi
-    646c3676:	ret
-    646c3677:	nopw   0x0(%rax,%rax,1)
-
-00000000646c3680 <sampling_state_update>:
-    646c3680:	movsd  %xmm1,0x10(%rcx)
-    646c3685:	mov    %r8d,0x8(%rcx)
-    646c3689:	ret
-    646c368a:	nopw   0x0(%rax,%rax,1)
-
-00000000646c3690 <kriging_param_setting>:
-    646c3690:	push   %rdi
-    646c3691:	push   %rsi
-    646c3692:	push   %rbx
-    646c3693:	sub    $0x30,%rsp
-    646c3697:	movaps %xmm6,0x20(%rsp)
-    646c369c:	movdqa 0x5a0c(%rip),%xmm6        # 646c90b0 <.rdata>
-    646c36a4:	movsd  0x10(%rdx),%xmm0
-    646c36a9:	movups %xmm6,0x8a78(%rip)        # 646cc128 <location+0x8>
-    646c36b0:	movsd  %xmm0,0x8a90(%rip)        # 646cc148 <k_range>
-    646c36b8:	mov    %rdx,0x8a91(%rip)        # 646cc150 <model>
-    646c36bf:	mov    %ecx,%esi
-    646c36c1:	mov    $0x8,%edx
-    646c36c6:	mov    $0xa,%ecx
-    646c36cb:	call   646c79b0 <calloc>
-    646c36d0:	mov    $0x8,%edx
-    646c36d5:	mov    $0xa,%ecx
-    646c36da:	movups %xmm6,0x8a27(%rip)        # 646cc108 <loc_cov+0x8>
-    646c36e1:	mov    %rax,0x8a38(%rip)        # 646cc120 <location>
-    646c36e8:	call   646c79b0 <calloc>
-    646c36ed:	mov    $0x8,%edx
-    646c36f2:	mov    $0xa,%ecx
-    646c36f7:	movups %xmm6,0x89ca(%rip)        # 646cc0c8 <loc_cov2+0x8>
-    646c36fe:	mov    %rax,0x89fb(%rip)        # 646cc100 <loc_cov>
-    646c3705:	call   646c79b0 <calloc>
-    646c370a:	mov    $0x8,%edx
-    646c370f:	mov    $0xa,%ecx
-    646c3714:	movups %xmm6,0x896d(%rip)        # 646cc088 <weights+0x8>
-    646c371b:	mov    %rax,0x899e(%rip)        # 646cc0c0 <loc_cov2>
-    646c3722:	call   646c79b0 <calloc>
-    646c3727:	mov    $0x8,%edx
-    646c372c:	mov    $0x64,%ecx
-    646c3731:	movdqa 0x5987(%rip),%xmm0        # 646c90c0 <.rdata+0x10>
-    646c3739:	mov    %rax,0x8940(%rip)        # 646cc080 <weights>
-    646c3740:	movups %xmm0,0x8961(%rip)        # 646cc0a8 <flatten_temp+0x8>
-    646c3747:	call   646c79b0 <calloc>
-    646c374c:	mov    $0x8,%edx
-    646c3751:	mov    $0xa,%ecx
-    646c3756:	movups %xmm6,0x898b(%rip)        # 646cc0e8 <data_temp+0x8>
-    646c375d:	mov    %rax,0x893c(%rip)        # 646cc0a0 <flatten_temp>
-    646c3764:	call   646c79b0 <calloc>
-    646c3769:	mov    $0x50,%ecx
-    646c376e:	movups %xmm6,0x88d3(%rip)        # 646cc048 <pdist_temp+0x8>
-    646c3775:	mov    %rax,0x8964(%rip)        # 646cc0e0 <data_temp>
-    646c377c:	call   646c7970 <malloc>
+00000000646c3420 <set_cov_model_default>:
+    646c3420:	mov    $0x4,%edx
+    646c3425:	mov    0xc(%rcx),%eax
+    646c3428:	test   %eax,%eax
+    646c342a:	cmove  %edx,%eax
+    646c342d:	mov    %eax,0xc(%rcx)
+    646c3430:	mov    0x18(%rcx),%rax
+    646c3434:	movq   %rax,%xmm0
+    646c3439:	ucomisd 0x5c67(%rip),%xmm0        # 646c90a8 <.rdata+0x8>
+    646c3441:	jp     646c344b <set_cov_model_default+0x2b>
+    646c3443:	cmove  0x5c55(%rip),%rax        # 646c90a0 <.rdata>
+    646c344b:	mov    %rax,0x18(%rcx)
+    646c344f:	mov    (%rcx),%eax
+    646c3451:	cltd
+    646c3452:	idivl  0x4(%rcx)
+    646c3455:	mov    %eax,0x8(%rcx)
+    646c3458:	ret
+    646c3459:	nopl   0x0(%rax)
+
+00000000646c3460 <cov_model>:
+    646c3460:	push   %rbp
+    646c3461:	push   %rdi
+    646c3462:	push   %rsi
+    646c3463:	push   %rbx
+    646c3464:	sub    $0x58,%rsp
+    646c3468:	movaps %xmm6,0x20(%rsp)
+    646c346d:	movaps %xmm7,0x30(%rsp)
+    646c3472:	movaps %xmm8,0x40(%rsp)
+    646c3478:	movsd  0x18(%r9),%xmm6
+    646c347e:	subsd  0x20(%r9),%xmm6
+    646c3484:	test   %r8d,%r8d
+    646c3487:	mov    %r9,%rsi
+    646c348a:	jle    646c34fb <cov_model+0x9b>
+    646c348c:	lea    -0x1(%r8),%eax
+    646c3490:	movsd  0x5c08(%rip),%xmm7        # 646c90a0 <.rdata>
+    646c3498:	mov    %rcx,%rbx
+    646c349b:	mov    %rdx,%rdi
+    646c349e:	movsd  0x5c09(%rip),%xmm8        # 646c90b0 <.rdata+0x10>
+    646c34a7:	lea    0x8(%rcx,%rax,8),%rbp
+    646c34ac:	nopl   0x0(%rax)
+    646c34b0:	movsd  (%rbx),%xmm0
+    646c34b4:	add    $0x8,%rbx
+    646c34b8:	add    $0x8,%rdi
+    646c34bc:	movsd  0x10(%rsi),%xmm1
+    646c34c1:	mulsd  %xmm0,%xmm0
+    646c34c5:	mulsd  %xmm1,%xmm1
+    646c34c9:	mulsd  %xmm8,%xmm0
+    646c34ce:	divsd  %xmm1,%xmm0
+    646c34d2:	call   646c6af0 <exp>
+    646c34d7:	movapd %xmm7,%xmm1
+    646c34db:	subsd  %xmm0,%xmm1
+    646c34df:	movsd  0x18(%rsi),%xmm0
+    646c34e4:	mulsd  %xmm6,%xmm1
+    646c34e8:	subsd  %xmm1,%xmm0
+    646c34ec:	addsd  0x20(%rsi),%xmm0
+    646c34f1:	movsd  %xmm0,-0x8(%rdi)
+    646c34f6:	cmp    %rbx,%rbp
+    646c34f9:	jne    646c34b0 <cov_model+0x50>
+    646c34fb:	movaps 0x20(%rsp),%xmm6
+    646c3500:	movaps 0x30(%rsp),%xmm7
+    646c3505:	movaps 0x40(%rsp),%xmm8
+    646c350b:	add    $0x58,%rsp
+    646c350f:	pop    %rbx
+    646c3510:	pop    %rsi
+    646c3511:	pop    %rdi
+    646c3512:	pop    %rbp
+    646c3513:	ret
+    646c3514:	xchg   %ax,%ax
+    646c3516:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c3520 <cov_model2d>:
+    646c3520:	push   %r15
+    646c3522:	push   %r14
+    646c3524:	push   %r13
+    646c3526:	push   %r12
+    646c3528:	push   %rbp
+    646c3529:	push   %rdi
+    646c352a:	push   %rsi
+    646c352b:	push   %rbx
+    646c352c:	sub    $0x68,%rsp
+    646c3530:	movaps %xmm6,0x30(%rsp)
+    646c3535:	movaps %xmm7,0x40(%rsp)
+    646c353a:	movaps %xmm8,0x50(%rsp)
+    646c3540:	movsd  0x18(%r9),%xmm6
+    646c3546:	subsd  0x20(%r9),%xmm6
+    646c354c:	test   %r8d,%r8d
+    646c354f:	mov    %rdx,%r14
+    646c3552:	mov    %r8d,%r13d
+    646c3555:	mov    %r9,%r15
+    646c3558:	jle    646c35fc <cov_model2d+0xdc>
+    646c355e:	lea    -0x1(%r8),%eax
+    646c3562:	movsd  0x5b36(%rip),%xmm7        # 646c90a0 <.rdata>
+    646c356a:	mov    %rcx,%rsi
+    646c356d:	xor    %r12d,%r12d
+    646c3570:	movsd  0x5b37(%rip),%xmm8        # 646c90b0 <.rdata+0x10>
+    646c3579:	lea    0x8(%rcx,%rax,8),%rdx
+    646c357e:	mov    %rdx,0x28(%rsp)
+    646c3583:	lea    0x8(,%rax,8),%rbp
+    646c358b:	nopl   0x0(%rax,%rax,1)
+    646c3590:	movslq %r12d,%rax
+    646c3593:	xor    %ebx,%ebx
+    646c3595:	lea    (%r14,%rax,8),%rdi
+    646c3599:	nopl   0x0(%rax)
+    646c35a0:	mov    (%rsi),%rax
+    646c35a3:	movsd  0x10(%r15),%xmm1
+    646c35a9:	mulsd  %xmm1,%xmm1
+    646c35ad:	movsd  (%rax,%rbx,1),%xmm0
+    646c35b2:	mulsd  %xmm0,%xmm0
+    646c35b6:	mulsd  %xmm8,%xmm0
+    646c35bb:	divsd  %xmm1,%xmm0
+    646c35bf:	call   646c6af0 <exp>
+    646c35c4:	movapd %xmm7,%xmm1
+    646c35c8:	subsd  %xmm0,%xmm1
+    646c35cc:	movsd  0x18(%r15),%xmm0
+    646c35d2:	mulsd  %xmm6,%xmm1
+    646c35d6:	subsd  %xmm1,%xmm0
+    646c35da:	addsd  0x20(%r15),%xmm0
+    646c35e0:	movsd  %xmm0,(%rdi,%rbx,1)
+    646c35e5:	add    $0x8,%rbx
+    646c35e9:	cmp    %rbx,%rbp
+    646c35ec:	jne    646c35a0 <cov_model2d+0x80>
+    646c35ee:	add    %r13d,%r12d
+    646c35f1:	add    $0x8,%rsi
+    646c35f5:	cmp    %rsi,0x28(%rsp)
+    646c35fa:	jne    646c3590 <cov_model2d+0x70>
+    646c35fc:	movaps 0x30(%rsp),%xmm6
+    646c3601:	movaps 0x40(%rsp),%xmm7
+    646c3606:	movaps 0x50(%rsp),%xmm8
+    646c360c:	add    $0x68,%rsp
+    646c3610:	pop    %rbx
+    646c3611:	pop    %rsi
+    646c3612:	pop    %rdi
+    646c3613:	pop    %rbp
+    646c3614:	pop    %r12
+    646c3616:	pop    %r13
+    646c3618:	pop    %r14
+    646c361a:	pop    %r15
+    646c361c:	ret
+    646c361d:	nop
+    646c361e:	nop
+    646c361f:	nop
+
+00000000646c3620 <sampling_state_init>:
+    646c3620:	push   %rsi
+    646c3621:	push   %rbx
+    646c3622:	sub    $0x38,%rsp
+    646c3626:	movaps %xmm6,0x20(%rsp)
+    646c362b:	movslq %edx,%rsi
+    646c362e:	mov    %rcx,%rbx
+    646c3631:	movq   $0x0,(%rcx)
+    646c3638:	mov    $0x8,%edx
+    646c363d:	movq   %rsi,%xmm6
+    646c3642:	movl   $0x0,0x8(%rcx)
+    646c3649:	punpcklqdq %xmm6,%xmm6
+    646c364d:	movq   $0x0,0x10(%rcx)
+    646c3655:	movups %xmm6,0x20(%rcx)
+    646c3659:	mov    %rsi,%rcx
+    646c365c:	call   646c78f0 <calloc>
+    646c3661:	movups %xmm6,0x38(%rbx)
+    646c3665:	mov    $0x8,%edx
+    646c366a:	mov    %rsi,%rcx
+    646c366d:	mov    %rax,0x18(%rbx)
+    646c3671:	call   646c78f0 <calloc>
+    646c3676:	nop
+    646c3677:	movaps 0x20(%rsp),%xmm6
+    646c367c:	mov    %rax,0x30(%rbx)
+    646c3680:	add    $0x38,%rsp
+    646c3684:	pop    %rbx
+    646c3685:	pop    %rsi
+    646c3686:	ret
+    646c3687:	nopw   0x0(%rax,%rax,1)
+
+00000000646c3690 <sampling_state_update>:
+    646c3690:	movsd  %xmm1,0x10(%rcx)
+    646c3695:	mov    %r8d,0x8(%rcx)
+    646c3699:	ret
+    646c369a:	nopw   0x0(%rax,%rax,1)
+
+00000000646c36a0 <kriging_param_setting>:
+    646c36a0:	push   %r12
+    646c36a2:	push   %rbp
+    646c36a3:	push   %rdi
+    646c36a4:	push   %rsi
+    646c36a5:	push   %rbx
+    646c36a6:	sub    $0x30,%rsp
+    646c36aa:	movaps %xmm6,0x20(%rsp)
+    646c36af:	mov    0xc(%rdx),%ebp
+    646c36b2:	movsd  0x10(%rdx),%xmm0
+    646c36b7:	movsd  %xmm0,0x8a69(%rip)        # 646cc128 <k_range>
+    646c36bf:	lea    0x2(%rbp),%ebx
+    646c36c2:	mov    %rdx,0x8a67(%rip)        # 646cc130 <model>
+    646c36c9:	mov    %ecx,%edi
+    646c36cb:	mov    $0x8,%edx
+    646c36d0:	movslq %ebx,%rsi
+    646c36d3:	mov    %rsi,%rcx
+    646c36d6:	movq   %rsi,%xmm6
+    646c36db:	punpcklqdq %xmm6,%xmm6
+    646c36df:	movups %xmm6,0x8a22(%rip)        # 646cc108 <location+0x8>
+    646c36e6:	call   646c78f0 <calloc>
+    646c36eb:	mov    %rsi,%rcx
+    646c36ee:	mov    $0x8,%edx
+    646c36f3:	movups %xmm6,0x89ee(%rip)        # 646cc0e8 <location_cov+0x8>
+    646c36fa:	mov    %rax,0x89ff(%rip)        # 646cc100 <location>
+    646c3701:	call   646c78f0 <calloc>
+    646c3706:	mov    %rsi,%rcx
+    646c3709:	mov    $0x8,%edx
+    646c370e:	movups %xmm6,0x89b3(%rip)        # 646cc0c8 <location_cov2d+0x8>
+    646c3715:	mov    %rax,0x89c4(%rip)        # 646cc0e0 <location_cov>
+    646c371c:	call   646c78f0 <calloc>
+    646c3721:	mov    %rsi,%rcx
+    646c3724:	shl    $0x3,%rsi
+    646c3728:	mov    $0x8,%edx
+    646c372d:	mov    %rax,0x898c(%rip)        # 646cc0c0 <location_cov2d>
+    646c3734:	movups %xmm6,0x894d(%rip)        # 646cc088 <weights+0x8>
+    646c373b:	call   646c78f0 <calloc>
+    646c3740:	mov    %ebx,%ecx
+    646c3742:	mov    $0x8,%edx
+    646c3747:	imul   %ebx,%ecx
+    646c374a:	mov    %rax,0x892f(%rip)        # 646cc080 <weights>
+    646c3751:	movslq %ecx,%rcx
+    646c3754:	movq   %rcx,%xmm0
+    646c3759:	punpcklqdq %xmm0,%xmm0
+    646c375d:	movups %xmm0,0x8944(%rip)        # 646cc0a8 <flatten_temp+0x8>
+    646c3764:	call   646c78f0 <calloc>
+    646c3769:	mov    %rsi,%rcx
+    646c376c:	movups %xmm6,0x88d5(%rip)        # 646cc048 <pdist_temp+0x8>
+    646c3773:	mov    %rax,0x8926(%rip)        # 646cc0a0 <flatten_temp>
+    646c377a:	call   646c78b0 <malloc>
+    646c377f:	test   %ebx,%ebx
     646c3781:	mov    %rax,0x88b8(%rip)        # 646cc040 <pdist_temp>
-    646c3788:	lea    0x50(%rax),%rdi
-    646c378c:	mov    %rax,%rbx
-    646c378f:	nop
-    646c3790:	mov    $0x50,%ecx
-    646c3795:	add    $0x8,%rbx
-    646c3799:	call   646c7970 <malloc>
-    646c379e:	mov    %rax,-0x8(%rbx)
-    646c37a2:	cmp    %rdi,%rbx
-    646c37a5:	jne    646c3790 <kriging_param_setting+0x100>
-    646c37a7:	mov    $0x50,%ecx
-    646c37ac:	movups %xmm6,0x8875(%rip)        # 646cc028 <datacov+0x8>
-    646c37b3:	call   646c7970 <malloc>
-    646c37b8:	mov    %rax,0x8861(%rip)        # 646cc020 <datacov>
-    646c37bf:	lea    0x50(%rax),%rdi
-    646c37c3:	mov    %rax,%rbx
-    646c37c6:	cs nopw 0x0(%rax,%rax,1)
-    646c37d0:	mov    $0x50,%ecx
-    646c37d5:	add    $0x8,%rbx
-    646c37d9:	call   646c7970 <malloc>
-    646c37de:	mov    %rax,-0x8(%rbx)
-    646c37e2:	cmp    %rdi,%rbx
-    646c37e5:	jne    646c37d0 <kriging_param_setting+0x140>
-    646c37e7:	movq   $0x3,0x887e(%rip)        # 646cc070 <array2d_temp+0x10>
-    646c37f2:	movslq %esi,%rcx
-    646c37f5:	mov    %rcx,0x886c(%rip)        # 646cc068 <array2d_temp+0x8>
-    646c37fc:	shl    $0x3,%rcx
-    646c3800:	call   646c7970 <malloc>
-    646c3805:	test   %esi,%esi
-    646c3807:	mov    %rax,0x8852(%rip)        # 646cc060 <array2d_temp>
-    646c380e:	jle    646c3837 <kriging_param_setting+0x1a7>
-    646c3810:	mov    %rax,%rbx
-    646c3813:	lea    -0x1(%rsi),%eax
-    646c3816:	lea    0x8(%rbx,%rax,8),%rsi
-    646c381b:	nopl   0x0(%rax,%rax,1)
+    646c3788:	jle    646c3850 <kriging_param_setting+0x1b0>
+    646c378e:	mov    %rax,%rbx
+    646c3791:	lea    0x1(%rbp),%eax
+    646c3794:	lea    0x8(,%rax,8),%rbp
+    646c379c:	lea    (%rbx,%rbp,1),%r12
+    646c37a0:	mov    %rsi,%rcx
+    646c37a3:	add    $0x8,%rbx
+    646c37a7:	call   646c78b0 <malloc>
+    646c37ac:	mov    %rax,-0x8(%rbx)
+    646c37b0:	cmp    %r12,%rbx
+    646c37b3:	jne    646c37a0 <kriging_param_setting+0x100>
+    646c37b5:	mov    %rsi,%rcx
+    646c37b8:	movups %xmm6,0x8869(%rip)        # 646cc028 <data_cov+0x8>
+    646c37bf:	call   646c78b0 <malloc>
+    646c37c4:	mov    %rax,0x8855(%rip)        # 646cc020 <data_cov>
+    646c37cb:	mov    %rax,%rbx
+    646c37ce:	add    %rax,%rbp
+    646c37d1:	mov    %rsi,%rcx
+    646c37d4:	add    $0x8,%rbx
+    646c37d8:	call   646c78b0 <malloc>
+    646c37dd:	mov    %rax,-0x8(%rbx)
+    646c37e1:	cmp    %rbp,%rbx
+    646c37e4:	jne    646c37d1 <kriging_param_setting+0x131>
+    646c37e6:	movq   $0x3,0x887f(%rip)        # 646cc070 <distance_mat+0x10>
+    646c37f1:	movslq %edi,%rcx
+    646c37f4:	mov    %rcx,0x886d(%rip)        # 646cc068 <distance_mat+0x8>
+    646c37fb:	shl    $0x3,%rcx
+    646c37ff:	call   646c78b0 <malloc>
+    646c3804:	test   %edi,%edi
+    646c3806:	mov    %rax,0x8853(%rip)        # 646cc060 <distance_mat>
+    646c380d:	jle    646c3837 <kriging_param_setting+0x197>
+    646c380f:	mov    %rax,%rbx
+    646c3812:	lea    -0x1(%rdi),%eax
+    646c3815:	lea    0x8(%rbx,%rax,8),%rsi
+    646c381a:	nopw   0x0(%rax,%rax,1)
     646c3820:	mov    $0x18,%ecx
     646c3825:	add    $0x8,%rbx
-    646c3829:	call   646c7970 <malloc>
+    646c3829:	call   646c78b0 <malloc>
     646c382e:	mov    %rax,-0x8(%rbx)
     646c3832:	cmp    %rbx,%rsi
-    646c3835:	jne    646c3820 <kriging_param_setting+0x190>
+    646c3835:	jne    646c3820 <kriging_param_setting+0x180>
     646c3837:	movaps 0x20(%rsp),%xmm6
     646c383c:	add    $0x30,%rsp
     646c3840:	pop    %rbx
     646c3841:	pop    %rsi
     646c3842:	pop    %rdi
-    646c3843:	ret
-    646c3844:	xchg   %ax,%ax
-    646c3846:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c3850 <find_neighbor>:
-    646c3850:	push   %rsi
-    646c3851:	push   %rbx
-    646c3852:	sub    $0x58,%rsp
-    646c3856:	movaps %xmm6,0x30(%rsp)
-    646c385b:	movaps %xmm7,0x40(%rsp)
-    646c3860:	mov    (%rdx),%eax
-    646c3862:	test   %eax,%eax
-    646c3864:	mov    %rcx,%rsi
-    646c3867:	mov    %rdx,%rbx
-    646c386a:	je     646c3a40 <find_neighbor+0x1f0>
-    646c3870:	mov    0x4(%rdx),%r11d
-    646c3874:	test   %r11d,%r11d
-    646c3877:	jle    646c3a80 <find_neighbor+0x230>
-    646c387d:	mov    0x30(%rdx),%r9
-    646c3881:	lea    -0x1(%r11),%eax
-    646c3885:	mov    0x18(%rdx),%r10
-    646c3889:	movslq %r11d,%rdx
-    646c388c:	movsd  0x583c(%rip),%xmm7        # 646c90d0 <.rdata+0x20>
-    646c3894:	mulsd  0x88ac(%rip),%xmm7        # 646cc148 <k_range>
-    646c389c:	lea    (%r9,%rdx,8),%rcx
-    646c38a0:	lea    0x10(%rbx),%rdx
-    646c38a4:	cmp    %rdx,%rcx
-    646c38a7:	lea    0x18(%rbx),%rdx
-    646c38ab:	setbe  %cl
-    646c38ae:	cmp    %rdx,%r9
-    646c38b1:	setae  %dl
-    646c38b4:	or     %dl,%cl
-    646c38b6:	je     646c3ac0 <find_neighbor+0x270>
-    646c38bc:	lea    0x20(%r10),%rdx
-    646c38c0:	lea    0x20(%r9),%rcx
-    646c38c4:	cmp    %rdx,%r9
-    646c38c7:	setae  %dl
-    646c38ca:	cmp    %rcx,%r10
-    646c38cd:	setae  %cl
-    646c38d0:	or     %ecx,%edx
-    646c38d2:	cmp    $0x4,%eax
-    646c38d5:	seta   %cl
-    646c38d8:	test   %cl,%dl
-    646c38da:	je     646c3ac0 <find_neighbor+0x270>
-    646c38e0:	mov    %r11d,%edx
-    646c38e3:	movapd 0x57f5(%rip),%xmm4        # 646c90e0 <.rdata+0x30>
-    646c38eb:	xor    %eax,%eax
-    646c38ed:	movddup 0x10(%rbx),%xmm6
-    646c38f2:	shr    $0x2,%edx
-    646c38f5:	movdqa 0x57f3(%rip),%xmm3        # 646c90f0 <.rdata+0x40>
-    646c38fd:	movddup %xmm7,%xmm5
-    646c3901:	pxor   %xmm2,%xmm2
-    646c3905:	shl    $0x5,%rdx
-    646c3909:	nopl   0x0(%rax)
-    646c3910:	movq   (%r10,%rax,1),%xmm0
-    646c3916:	movq   0x10(%r10,%rax,1),%xmm1
-    646c391d:	movhpd 0x8(%r10,%rax,1),%xmm0
-    646c3924:	movhpd 0x18(%r10,%rax,1),%xmm1
-    646c392b:	subpd  %xmm6,%xmm0
-    646c392f:	subpd  %xmm6,%xmm1
-    646c3933:	andpd  %xmm4,%xmm0
-    646c3937:	movlpd %xmm0,(%r9,%rax,1)
-    646c393d:	andpd  %xmm4,%xmm1
-    646c3941:	movhpd %xmm0,0x8(%r9,%rax,1)
-    646c3948:	cmpltpd %xmm5,%xmm0
-    646c394d:	movlpd %xmm1,0x10(%r9,%rax,1)
-    646c3954:	movhpd %xmm1,0x18(%r9,%rax,1)
-    646c395b:	cmpltpd %xmm5,%xmm1
-    646c3960:	add    $0x20,%rax
-    646c3964:	cmp    %rdx,%rax
-    646c3967:	pand   %xmm3,%xmm0
-    646c396b:	pand   %xmm3,%xmm1
-    646c396f:	shufps $0x88,%xmm1,%xmm0
-    646c3973:	paddd  %xmm0,%xmm2
-    646c3977:	jne    646c3910 <find_neighbor+0xc0>
-    646c3979:	movdqa %xmm2,%xmm0
-    646c397d:	mov    %r11d,%edx
-    646c3980:	psrldq $0x8,%xmm0
-    646c3985:	and    $0xfffffffc,%edx
-    646c3988:	paddd  %xmm0,%xmm2
-    646c398c:	cmp    %edx,%r11d
-    646c398f:	movdqa %xmm2,%xmm0
-    646c3993:	psrldq $0x4,%xmm0
-    646c3998:	paddd  %xmm0,%xmm2
-    646c399c:	movd   %xmm2,%eax
-    646c39a0:	je     646c3a26 <find_neighbor+0x1d6>
-    646c39a6:	mov    %edx,%ecx
-    646c39a8:	movq   0x5750(%rip),%xmm1        # 646c9100 <.rdata+0x50>
-    646c39b0:	movsd  (%r10,%rcx,8),%xmm0
-    646c39b6:	subsd  0x10(%rbx),%xmm0
-    646c39bb:	andpd  %xmm1,%xmm0
-    646c39bf:	movsd  %xmm0,(%r9,%rcx,8)
-    646c39c5:	xor    %ecx,%ecx
-    646c39c7:	comisd %xmm0,%xmm7
-    646c39cb:	seta   %cl
-    646c39ce:	add    %ecx,%eax
-    646c39d0:	lea    0x1(%rdx),%ecx
-    646c39d3:	cmp    %r11d,%ecx
-    646c39d6:	jge    646c3a26 <find_neighbor+0x1d6>
-    646c39d8:	movslq %ecx,%rcx
-    646c39db:	movsd  (%r10,%rcx,8),%xmm0
-    646c39e1:	subsd  0x10(%rbx),%xmm0
-    646c39e6:	andpd  %xmm1,%xmm0
-    646c39ea:	movsd  %xmm0,(%r9,%rcx,8)
-    646c39f0:	xor    %ecx,%ecx
-    646c39f2:	comisd %xmm0,%xmm7
-    646c39f6:	seta   %cl
-    646c39f9:	add    $0x2,%edx
-    646c39fc:	add    %ecx,%eax
-    646c39fe:	cmp    %r11d,%edx
-    646c3a01:	jge    646c3a26 <find_neighbor+0x1d6>
-    646c3a03:	movslq %edx,%rdx
-    646c3a06:	movsd  (%r10,%rdx,8),%xmm0
-    646c3a0c:	subsd  0x10(%rbx),%xmm0
-    646c3a11:	andpd  %xmm0,%xmm1
-    646c3a15:	movsd  %xmm1,(%r9,%rdx,8)
-    646c3a1b:	xor    %edx,%edx
-    646c3a1d:	comisd %xmm1,%xmm7
-    646c3a21:	seta   %dl
-    646c3a24:	add    %edx,%eax
-    646c3a26:	test   %eax,%eax
-    646c3a28:	je     646c3a80 <find_neighbor+0x230>
-    646c3a2a:	mov    $0x1,%eax
-    646c3a2f:	movaps 0x30(%rsp),%xmm6
-    646c3a34:	movaps 0x40(%rsp),%xmm7
-    646c3a39:	add    $0x58,%rsp
-    646c3a3d:	pop    %rbx
-    646c3a3e:	pop    %rsi
-    646c3a3f:	ret
-    646c3a40:	mov    %r8,%rcx
-    646c3a43:	mov    %eax,0x2c(%rsp)
-    646c3a47:	call   646c3390 <mt19937_random_normal>
-    646c3a4c:	mov    0x86fd(%rip),%rcx        # 646cc150 <model>
-    646c3a53:	cvttsd2si 0x10(%rbx),%edx
-    646c3a58:	mov    0x2c(%rsp),%eax
-    646c3a5c:	mulsd  0x18(%rcx),%xmm0
-    646c3a61:	movslq %edx,%rdx
-    646c3a64:	movslq 0x8(%rbx),%rcx
-    646c3a68:	movsd  %xmm0,(%rsi,%rdx,8)
-    646c3a6d:	mov    0x18(%rbx),%rdx
-    646c3a71:	movsd  0x10(%rbx),%xmm0
-    646c3a76:	movsd  %xmm0,(%rdx,%rcx,8)
-    646c3a7b:	jmp    646c3a2f <find_neighbor+0x1df>
-    646c3a7d:	nopl   (%rax)
-    646c3a80:	mov    %r8,%rcx
-    646c3a83:	call   646c3390 <mt19937_random_normal>
-    646c3a88:	mov    0x86c1(%rip),%rdx        # 646cc150 <model>
-    646c3a8f:	cvttsd2si 0x10(%rbx),%eax
-    646c3a94:	mulsd  0x18(%rdx),%xmm0
-    646c3a99:	cltq
-    646c3a9b:	movslq 0x8(%rbx),%rdx
-    646c3a9f:	movsd  %xmm0,(%rsi,%rax,8)
-    646c3aa4:	mov    0x18(%rbx),%rax
-    646c3aa8:	movsd  0x10(%rbx),%xmm0
-    646c3aad:	movsd  %xmm0,(%rax,%rdx,8)
-    646c3ab2:	xor    %eax,%eax
-    646c3ab4:	jmp    646c3a2f <find_neighbor+0x1df>
-    646c3ab9:	nopl   0x0(%rax)
-    646c3ac0:	mov    %eax,%ecx
-    646c3ac2:	xor    %edx,%edx
-    646c3ac4:	xor    %eax,%eax
-    646c3ac6:	movq   0x5632(%rip),%xmm1        # 646c9100 <.rdata+0x50>
-    646c3ace:	jmp    646c3ad3 <find_neighbor+0x283>
-    646c3ad0:	mov    %r11,%rdx
-    646c3ad3:	movsd  (%r10,%rdx,8),%xmm0
-    646c3ad9:	xor    %r11d,%r11d
-    646c3adc:	subsd  0x10(%rbx),%xmm0
-    646c3ae1:	andpd  %xmm1,%xmm0
-    646c3ae5:	comisd %xmm0,%xmm7
-    646c3ae9:	movsd  %xmm0,(%r9,%rdx,8)
-    646c3aef:	seta   %r11b
-    646c3af3:	add    %r11d,%eax
-    646c3af6:	cmp    %rcx,%rdx
-    646c3af9:	lea    0x1(%rdx),%r11
-    646c3afd:	jne    646c3ad0 <find_neighbor+0x280>
-    646c3aff:	jmp    646c3a26 <find_neighbor+0x1d6>
-    646c3b04:	xchg   %ax,%ax
-    646c3b06:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c3b10 <simple_kriging>:
-    646c3b10:	push   %r12
-    646c3b12:	push   %rbp
-    646c3b13:	push   %rdi
-    646c3b14:	push   %rsi
-    646c3b15:	push   %rbx
-    646c3b16:	sub    $0x30,%rsp
-    646c3b1a:	movaps %xmm6,0x20(%rsp)
-    646c3b1f:	mov    %rcx,%rbp
-    646c3b22:	mov    %rdx,%rbx
-    646c3b25:	mov    %r8,%rsi
-    646c3b28:	mov    %r9d,%edi
-    646c3b2b:	call   646c3850 <find_neighbor>
-    646c3b30:	test   %eax,%eax
-    646c3b32:	je     646c3d77 <simple_kriging+0x267>
-    646c3b38:	mov    0x4(%rbx),%r12d
-    646c3b3c:	test   %r12d,%r12d
-    646c3b3f:	jle    646c3b96 <simple_kriging+0x86>
-    646c3b41:	mov    0x18(%rbx),%r11
-    646c3b45:	lea    -0x1(%r12),%r8d
-    646c3b4a:	xor    %edx,%edx
-    646c3b4c:	mov    0x850d(%rip),%r10        # 646cc060 <array2d_temp>
-    646c3b53:	mov    0x30(%rbx),%r9
-    646c3b57:	jmp    646c3b63 <simple_kriging+0x53>
-    646c3b59:	nopl   0x0(%rax)
-    646c3b60:	mov    %rax,%rdx
-    646c3b63:	movsd  (%r11,%rdx,8),%xmm0
-    646c3b69:	cmp    %rdx,%r8
-    646c3b6c:	mov    (%r10,%rdx,8),%rcx
-    646c3b70:	cvttsd2si %xmm0,%eax
-    646c3b74:	movsd  %xmm0,(%rcx)
-    646c3b78:	cltq
-    646c3b7a:	movsd  0x0(%rbp,%rax,8),%xmm0
-    646c3b80:	lea    0x1(%rdx),%rax
-    646c3b84:	movsd  %xmm0,0x8(%rcx)
-    646c3b89:	movsd  (%r9,%rdx,8),%xmm0
-    646c3b8f:	movsd  %xmm0,0x10(%rcx)
-    646c3b94:	jne    646c3b60 <simple_kriging+0x50>
-    646c3b96:	mov    (%rbx),%r8d
-    646c3b99:	cmp    $0x1,%r8d
-    646c3b9d:	jg     646c3d90 <simple_kriging+0x280>
-    646c3ba3:	test   %r8d,%r8d
-    646c3ba6:	mov    0x8573(%rip),%rcx        # 646cc120 <location>
-    646c3bad:	jle    646c3be9 <simple_kriging+0xd9>
-    646c3baf:	mov    0x84aa(%rip),%r12        # 646cc060 <array2d_temp>
-    646c3bb6:	lea    -0x1(%r8),%r10d
-    646c3bba:	xor    %eax,%eax
-    646c3bbc:	mov    0x84fd(%rip),%r11        # 646cc0c0 <loc_cov2>
-    646c3bc3:	jmp    646c3bc8 <simple_kriging+0xb8>
-    646c3bc5:	mov    %rdx,%rax
-    646c3bc8:	mov    (%r12,%rax,8),%rdx
-    646c3bcc:	cmp    %rax,%r10
-    646c3bcf:	movsd  (%rdx),%xmm0
-    646c3bd3:	movsd  %xmm0,(%rcx,%rax,8)
-    646c3bd8:	movsd  0x10(%rdx),%xmm0
-    646c3bdd:	lea    0x1(%rax),%rdx
-    646c3be1:	movsd  %xmm0,(%r11,%rax,8)
-    646c3be7:	jne    646c3bc5 <simple_kriging+0xb5>
-    646c3be9:	mov    0x8450(%rip),%rdx        # 646cc040 <pdist_temp>
-    646c3bf0:	call   646c4900 <pdist>
-    646c3bf5:	mov    0x8554(%rip),%r9        # 646cc150 <model>
-    646c3bfc:	mov    (%rbx),%r8d
-    646c3bff:	mov    0x849a(%rip),%rdx        # 646cc0a0 <flatten_temp>
-    646c3c06:	mov    0x8433(%rip),%rcx        # 646cc040 <pdist_temp>
-    646c3c0d:	call   646c3510 <cov_model2d>
-    646c3c12:	mov    (%rbx),%r8d
-    646c3c15:	mov    0x8404(%rip),%rdx        # 646cc020 <datacov>
-    646c3c1c:	mov    0x847d(%rip),%rcx        # 646cc0a0 <flatten_temp>
-    646c3c23:	call   646c4a50 <matrixform>
-    646c3c28:	mov    0x8521(%rip),%r9        # 646cc150 <model>
-    646c3c2f:	mov    (%rbx),%r8d
-    646c3c32:	mov    0x84c7(%rip),%rdx        # 646cc100 <loc_cov>
-    646c3c39:	mov    0x8480(%rip),%rcx        # 646cc0c0 <loc_cov2>
-    646c3c40:	call   646c3450 <cov_model>
-    646c3c45:	cmp    $0x1,%edi
-    646c3c48:	je     646c3dc0 <simple_kriging+0x2b0>
-    646c3c4e:	mov    (%rbx),%r9d
-    646c3c51:	mov    %r9d,%eax
-    646c3c54:	test   %eax,%eax
-    646c3c56:	jg     646c3c80 <simple_kriging+0x170>
-    646c3c58:	pxor   %xmm4,%xmm4
-    646c3c5c:	pxor   %xmm1,%xmm1
-    646c3c60:	movq   $0x0,0x84d5(%rip)        # 646cc140 <estimation>
-    646c3c6b:	movq   $0x0,0x84c2(%rip)        # 646cc138 <kriging_var>
-    646c3c76:	jmp    646c3d1f <simple_kriging+0x20f>
-    646c3c7b:	nopl   0x0(%rax,%rax,1)
-    646c3c80:	mov    0x83f9(%rip),%r8        # 646cc080 <weights>
-    646c3c87:	mov    0x8472(%rip),%rdx        # 646cc100 <loc_cov>
-    646c3c8e:	mov    0x838b(%rip),%rcx        # 646cc020 <datacov>
-    646c3c95:	call   646c43b0 <lu_inverse_solver>
-    646c3c9a:	mov    (%rbx),%eax
-    646c3c9c:	pxor   %xmm4,%xmm4
-    646c3ca0:	movq   $0x0,0x8495(%rip)        # 646cc140 <estimation>
-    646c3cab:	movq   $0x0,0x8482(%rip)        # 646cc138 <kriging_var>
-    646c3cb6:	test   %eax,%eax
-    646c3cb8:	jle    646c3e73 <simple_kriging+0x363>
-    646c3cbe:	lea    -0x1(%rax),%ecx
-    646c3cc1:	mov    0x8398(%rip),%r10        # 646cc060 <array2d_temp>
-    646c3cc8:	xor    %eax,%eax
-    646c3cca:	pxor   %xmm1,%xmm1
-    646c3cce:	mov    0x83ab(%rip),%r9        # 646cc080 <weights>
-    646c3cd5:	pxor   %xmm2,%xmm2
-    646c3cd9:	mov    0x8420(%rip),%r8        # 646cc100 <loc_cov>
-    646c3ce0:	jmp    646c3ce5 <simple_kriging+0x1d5>
-    646c3ce2:	mov    %rdx,%rax
-    646c3ce5:	mov    (%r10,%rax,8),%rdx
-    646c3ce9:	cmp    %rcx,%rax
-    646c3cec:	movsd  (%r9,%rax,8),%xmm0
-    646c3cf2:	movsd  0x8(%rdx),%xmm3
-    646c3cf7:	lea    0x1(%rax),%rdx
-    646c3cfb:	mulsd  %xmm0,%xmm3
-    646c3cff:	mulsd  (%r8,%rax,8),%xmm0
-    646c3d05:	addsd  %xmm3,%xmm2
-    646c3d09:	addsd  %xmm0,%xmm1
-    646c3d0d:	jne    646c3ce2 <simple_kriging+0x1d2>
-    646c3d0f:	movsd  %xmm2,0x8429(%rip)        # 646cc140 <estimation>
-    646c3d17:	movsd  %xmm1,0x8419(%rip)        # 646cc138 <kriging_var>
-    646c3d1f:	mov    0x842a(%rip),%rax        # 646cc150 <model>
-    646c3d26:	movsd  0x18(%rax),%xmm0
-    646c3d2b:	subsd  %xmm1,%xmm0
-    646c3d2f:	comisd %xmm0,%xmm4
-    646c3d33:	ja     646c3db0 <simple_kriging+0x2a0>
-    646c3d35:	movsd  %xmm0,0x83fb(%rip)        # 646cc138 <kriging_var>
-    646c3d3d:	mov    %rsi,%rcx
-    646c3d40:	call   646c3390 <mt19937_random_normal>
-    646c3d45:	movsd  0x53cb(%rip),%xmm1        # 646c9118 <.rdata+0x68>
-    646c3d4d:	movapd %xmm0,%xmm6
-    646c3d51:	movsd  0x83df(%rip),%xmm0        # 646cc138 <kriging_var>
-    646c3d59:	call   646c6f60 <pow>
-    646c3d5e:	cvttsd2si 0x10(%rbx),%eax
-    646c3d63:	mulsd  %xmm0,%xmm6
-    646c3d67:	addsd  0x83d1(%rip),%xmm6        # 646cc140 <estimation>
-    646c3d6f:	cltq
-    646c3d71:	movsd  %xmm6,0x0(%rbp,%rax,8)
-    646c3d77:	movaps 0x20(%rsp),%xmm6
-    646c3d7c:	add    $0x30,%rsp
-    646c3d80:	pop    %rbx
-    646c3d81:	pop    %rsi
-    646c3d82:	pop    %rdi
-    646c3d83:	pop    %rbp
-    646c3d84:	pop    %r12
-    646c3d86:	ret
-    646c3d87:	nopw   0x0(%rax,%rax,1)
-    646c3d90:	mov    0x82c9(%rip),%rcx        # 646cc060 <array2d_temp>
-    646c3d97:	mov    %r8d,%r9d
-    646c3d9a:	xor    %edx,%edx
-    646c3d9c:	lea    -0x1(%r12),%r8d
-    646c3da1:	call   646c5220 <quickselect2d>
-    646c3da6:	mov    (%rbx),%r8d
-    646c3da9:	jmp    646c3ba3 <simple_kriging+0x93>
-    646c3dae:	xchg   %ax,%ax
-    646c3db0:	movq   $0x0,0x837d(%rip)        # 646cc138 <kriging_var>
-    646c3dbb:	jmp    646c3d3d <simple_kriging+0x22d>
-    646c3dbd:	nopl   (%rax)
-    646c3dc0:	movslq (%rbx),%rdx
-    646c3dc3:	mov    0x8256(%rip),%r10        # 646cc020 <datacov>
-    646c3dca:	mov    %rdx,%r9
-    646c3dcd:	mov    %edx,%eax
-    646c3dcf:	shl    $0x3,%rdx
-    646c3dd3:	test   %r9d,%r9d
-    646c3dd6:	jle    646c3e67 <simple_kriging+0x357>
-    646c3ddc:	lea    -0x1(%r9),%ecx
-    646c3de0:	movsd  0x5328(%rip),%xmm0        # 646c9110 <.rdata+0x60>
-    646c3de8:	mov    %r10,%rax
-    646c3deb:	lea    0x8(%r10,%rcx,8),%r8
-    646c3df0:	mov    (%rax),%rcx
-    646c3df3:	add    $0x8,%rax
-    646c3df7:	cmp    %rax,%r8
-    646c3dfa:	movsd  %xmm0,(%rcx,%rdx,1)
-    646c3dff:	jne    646c3df0 <simple_kriging+0x2e0>
-    646c3e01:	add    %r10,%rdx
-    646c3e04:	xor    %eax,%eax
-    646c3e06:	cs nopw 0x0(%rax,%rax,1)
-    646c3e10:	cmp    %eax,%r9d
-    646c3e13:	je     646c3e50 <simple_kriging+0x340>
-    646c3e15:	mov    (%rdx),%rcx
-    646c3e18:	movsd  %xmm0,(%rcx,%rax,8)
-    646c3e1d:	add    $0x1,%rax
-    646c3e21:	cmp    %eax,%r9d
-    646c3e24:	jge    646c3e10 <simple_kriging+0x300>
-    646c3e26:	movslq %r9d,%rdx
-    646c3e29:	mov    %r9d,%eax
-    646c3e2c:	shl    $0x3,%rdx
-    646c3e30:	mov    0x82c9(%rip),%rcx        # 646cc100 <loc_cov>
-    646c3e37:	add    $0x1,%r9d
-    646c3e3b:	test   %eax,%eax
-    646c3e3d:	movsd  %xmm0,(%rcx,%rdx,1)
-    646c3e42:	jle    646c3c58 <simple_kriging+0x148>
-    646c3e48:	jmp    646c3c80 <simple_kriging+0x170>
-    646c3e4d:	nopl   (%rax)
-    646c3e50:	mov    (%r10,%rax,8),%rcx
-    646c3e54:	movq   $0x0,(%rcx,%rax,8)
-    646c3e5c:	add    $0x1,%rax
-    646c3e60:	cmp    %eax,%r9d
-    646c3e63:	jge    646c3e10 <simple_kriging+0x300>
-    646c3e65:	jmp    646c3e26 <simple_kriging+0x316>
-    646c3e67:	movsd  0x52a1(%rip),%xmm0        # 646c9110 <.rdata+0x60>
-    646c3e6f:	jne    646c3e30 <simple_kriging+0x320>
-    646c3e71:	jmp    646c3e01 <simple_kriging+0x2f1>
-    646c3e73:	pxor   %xmm1,%xmm1
-    646c3e77:	jmp    646c3d1f <simple_kriging+0x20f>
-    646c3e7c:	nopl   0x0(%rax)
-
-00000000646c3e80 <matrix_agumented>:
-    646c3e80:	sub    $0x28,%rsp
-    646c3e84:	movaps %xmm6,(%rsp)
-    646c3e88:	movaps %xmm7,0x10(%rsp)
-    646c3e8d:	test   %edx,%edx
-    646c3e8f:	jle    646c3fd0 <matrix_agumented+0x150>
-    646c3e95:	movslq %edx,%r11
-    646c3e98:	movsd  0x5270(%rip),%xmm0        # 646c9110 <.rdata+0x60>
-    646c3ea0:	mov    %rcx,%rax
-    646c3ea3:	lea    -0x1(%rdx),%r8d
-    646c3ea7:	lea    0x0(,%r11,8),%r10
-    646c3eaf:	lea    0x8(%rcx,%r8,8),%r9
-    646c3eb4:	mov    (%rax),%r8
-    646c3eb7:	add    $0x8,%rax
-    646c3ebb:	cmp    %r9,%rax
-    646c3ebe:	movsd  %xmm0,(%r8,%r10,1)
-    646c3ec4:	jne    646c3eb4 <matrix_agumented+0x34>
-    646c3ec6:	mov    (%rcx,%r11,8),%r8
-    646c3eca:	lea    0x1(%rdx),%r9d
-    646c3ece:	cmp    $0x2,%edx
-    646c3ed1:	jle    646c3fe0 <matrix_agumented+0x160>
-    646c3ed7:	mov    %r9d,%ecx
-    646c3eda:	movd   %edx,%xmm5
-    646c3ede:	mov    %r8,%rax
-    646c3ee1:	movdqa 0x5237(%rip),%xmm2        # 646c9120 <.rdata+0x70>
-    646c3ee9:	shr    $0x2,%ecx
-    646c3eec:	movdqa 0x523c(%rip),%xmm6        # 646c9130 <.rdata+0x80>
-    646c3ef4:	pshufd $0x0,%xmm5,%xmm7
-    646c3ef9:	pxor   %xmm5,%xmm5
-    646c3efd:	shl    $0x5,%rcx
-    646c3f01:	movapd 0x5237(%rip),%xmm4        # 646c9140 <.rdata+0x90>
-    646c3f09:	add    %r8,%rcx
-    646c3f0c:	nopl   0x0(%rax)
-    646c3f10:	movdqa %xmm2,%xmm0
-    646c3f14:	movdqa %xmm5,%xmm3
-    646c3f18:	add    $0x20,%rax
-    646c3f1c:	pcmpeqd %xmm7,%xmm0
-    646c3f20:	paddd  %xmm6,%xmm2
-    646c3f24:	pcmpgtd %xmm0,%xmm3
-    646c3f28:	movdqa %xmm0,%xmm1
-    646c3f2c:	punpckldq %xmm3,%xmm1
-    646c3f30:	punpckhdq %xmm3,%xmm0
-    646c3f34:	andnpd %xmm4,%xmm1
-    646c3f38:	andnpd %xmm4,%xmm0
-    646c3f3c:	movlpd %xmm1,-0x20(%rax)
-    646c3f41:	movhpd %xmm1,-0x18(%rax)
-    646c3f46:	movlpd %xmm0,-0x10(%rax)
-    646c3f4b:	movhpd %xmm0,-0x8(%rax)
-    646c3f50:	cmp    %rax,%rcx
-    646c3f53:	jne    646c3f10 <matrix_agumented+0x90>
-    646c3f55:	mov    %r9d,%eax
-    646c3f58:	and    $0xfffffffc,%eax
-    646c3f5b:	cmp    %eax,%r9d
-    646c3f5e:	je     646c3fa0 <matrix_agumented+0x120>
-    646c3f60:	movslq %eax,%rcx
-    646c3f63:	cmp    %eax,%edx
-    646c3f65:	movsd  0x51a3(%rip),%xmm0        # 646c9110 <.rdata+0x60>
-    646c3f6d:	lea    (%r8,%rcx,8),%rcx
-    646c3f71:	je     646c3fb0 <matrix_agumented+0x130>
-    646c3f73:	movsd  %xmm0,(%rcx)
-    646c3f77:	lea    0x1(%rax),%ecx
-    646c3f7a:	cmp    %edx,%ecx
-    646c3f7c:	jg     646c3fa0 <matrix_agumented+0x120>
-    646c3f7e:	movslq %ecx,%r9
-    646c3f81:	lea    (%r8,%r9,8),%r9
-    646c3f85:	je     646c3fc5 <matrix_agumented+0x145>
-    646c3f87:	movsd  %xmm0,(%r9)
-    646c3f8c:	add    $0x2,%eax
-    646c3f8f:	cmp    %eax,%edx
-    646c3f91:	jl     646c3fa0 <matrix_agumented+0x120>
-    646c3f93:	movslq %eax,%rcx
-    646c3f96:	lea    (%r8,%rcx,8),%rcx
-    646c3f9a:	je     646c3fb0 <matrix_agumented+0x130>
-    646c3f9c:	movsd  %xmm0,(%rcx)
-    646c3fa0:	movaps (%rsp),%xmm6
-    646c3fa4:	movaps 0x10(%rsp),%xmm7
-    646c3fa9:	add    $0x28,%rsp
-    646c3fad:	ret
-    646c3fae:	xchg   %ax,%ax
-    646c3fb0:	movq   $0x0,(%rcx)
-    646c3fb7:	movaps (%rsp),%xmm6
-    646c3fbb:	movaps 0x10(%rsp),%xmm7
-    646c3fc0:	add    $0x28,%rsp
-    646c3fc4:	ret
-    646c3fc5:	movq   $0x0,(%r9)
-    646c3fcc:	jmp    646c3f8c <matrix_agumented+0x10c>
+    646c3843:	pop    %rbp
+    646c3844:	pop    %r12
+    646c3846:	ret
+    646c3847:	nopw   0x0(%rax,%rax,1)
+    646c3850:	mov    %rsi,%rcx
+    646c3853:	movups %xmm6,0x87ce(%rip)        # 646cc028 <data_cov+0x8>
+    646c385a:	call   646c78b0 <malloc>
+    646c385f:	mov    %rax,0x87ba(%rip)        # 646cc020 <data_cov>
+    646c3866:	jmp    646c37e6 <kriging_param_setting+0x146>
+    646c386b:	nopl   0x0(%rax,%rax,1)
+
+00000000646c3870 <find_neighbor>:
+    646c3870:	push   %rsi
+    646c3871:	push   %rbx
+    646c3872:	sub    $0x58,%rsp
+    646c3876:	movaps %xmm6,0x30(%rsp)
+    646c387b:	movaps %xmm7,0x40(%rsp)
+    646c3880:	mov    (%rdx),%eax
+    646c3882:	test   %eax,%eax
+    646c3884:	mov    %rcx,%rsi
+    646c3887:	mov    %rdx,%rbx
+    646c388a:	je     646c3a60 <find_neighbor+0x1f0>
+    646c3890:	mov    0x4(%rdx),%r11d
+    646c3894:	test   %r11d,%r11d
+    646c3897:	jle    646c3aa0 <find_neighbor+0x230>
+    646c389d:	mov    0x30(%rdx),%r9
+    646c38a1:	lea    -0x1(%r11),%eax
+    646c38a5:	mov    0x18(%rdx),%r10
+    646c38a9:	movslq %r11d,%rdx
+    646c38ac:	movsd  0x580c(%rip),%xmm7        # 646c90c0 <.rdata>
+    646c38b4:	mulsd  0x886c(%rip),%xmm7        # 646cc128 <k_range>
+    646c38bc:	lea    (%r9,%rdx,8),%rcx
+    646c38c0:	lea    0x10(%rbx),%rdx
+    646c38c4:	cmp    %rdx,%rcx
+    646c38c7:	lea    0x18(%rbx),%rdx
+    646c38cb:	setbe  %cl
+    646c38ce:	cmp    %rdx,%r9
+    646c38d1:	setae  %dl
+    646c38d4:	or     %dl,%cl
+    646c38d6:	je     646c3ae0 <find_neighbor+0x270>
+    646c38dc:	lea    0x20(%r10),%rdx
+    646c38e0:	lea    0x20(%r9),%rcx
+    646c38e4:	cmp    %rdx,%r9
+    646c38e7:	setae  %dl
+    646c38ea:	cmp    %rcx,%r10
+    646c38ed:	setae  %cl
+    646c38f0:	or     %ecx,%edx
+    646c38f2:	cmp    $0x4,%eax
+    646c38f5:	seta   %cl
+    646c38f8:	test   %cl,%dl
+    646c38fa:	je     646c3ae0 <find_neighbor+0x270>
+    646c3900:	mov    %r11d,%edx
+    646c3903:	movapd 0x57c5(%rip),%xmm4        # 646c90d0 <.rdata+0x10>
+    646c390b:	xor    %eax,%eax
+    646c390d:	movddup 0x10(%rbx),%xmm6
+    646c3912:	shr    $0x2,%edx
+    646c3915:	movdqa 0x57c3(%rip),%xmm3        # 646c90e0 <.rdata+0x20>
+    646c391d:	movddup %xmm7,%xmm5
+    646c3921:	pxor   %xmm2,%xmm2
+    646c3925:	shl    $0x5,%rdx
+    646c3929:	nopl   0x0(%rax)
+    646c3930:	movq   (%r10,%rax,1),%xmm0
+    646c3936:	movq   0x10(%r10,%rax,1),%xmm1
+    646c393d:	movhpd 0x8(%r10,%rax,1),%xmm0
+    646c3944:	movhpd 0x18(%r10,%rax,1),%xmm1
+    646c394b:	subpd  %xmm6,%xmm0
+    646c394f:	subpd  %xmm6,%xmm1
+    646c3953:	andpd  %xmm4,%xmm0
+    646c3957:	movlpd %xmm0,(%r9,%rax,1)
+    646c395d:	andpd  %xmm4,%xmm1
+    646c3961:	movhpd %xmm0,0x8(%r9,%rax,1)
+    646c3968:	cmpltpd %xmm5,%xmm0
+    646c396d:	movlpd %xmm1,0x10(%r9,%rax,1)
+    646c3974:	movhpd %xmm1,0x18(%r9,%rax,1)
+    646c397b:	cmpltpd %xmm5,%xmm1
+    646c3980:	add    $0x20,%rax
+    646c3984:	cmp    %rdx,%rax
+    646c3987:	pand   %xmm3,%xmm0
+    646c398b:	pand   %xmm3,%xmm1
+    646c398f:	shufps $0x88,%xmm1,%xmm0
+    646c3993:	paddd  %xmm0,%xmm2
+    646c3997:	jne    646c3930 <find_neighbor+0xc0>
+    646c3999:	movdqa %xmm2,%xmm0
+    646c399d:	mov    %r11d,%edx
+    646c39a0:	psrldq $0x8,%xmm0
+    646c39a5:	and    $0xfffffffc,%edx
+    646c39a8:	paddd  %xmm0,%xmm2
+    646c39ac:	cmp    %edx,%r11d
+    646c39af:	movdqa %xmm2,%xmm0
+    646c39b3:	psrldq $0x4,%xmm0
+    646c39b8:	paddd  %xmm0,%xmm2
+    646c39bc:	movd   %xmm2,%eax
+    646c39c0:	je     646c3a46 <find_neighbor+0x1d6>
+    646c39c6:	mov    %edx,%ecx
+    646c39c8:	movq   0x5720(%rip),%xmm1        # 646c90f0 <.rdata+0x30>
+    646c39d0:	movsd  (%r10,%rcx,8),%xmm0
+    646c39d6:	subsd  0x10(%rbx),%xmm0
+    646c39db:	andpd  %xmm1,%xmm0
+    646c39df:	movsd  %xmm0,(%r9,%rcx,8)
+    646c39e5:	xor    %ecx,%ecx
+    646c39e7:	comisd %xmm0,%xmm7
+    646c39eb:	seta   %cl
+    646c39ee:	add    %ecx,%eax
+    646c39f0:	lea    0x1(%rdx),%ecx
+    646c39f3:	cmp    %r11d,%ecx
+    646c39f6:	jge    646c3a46 <find_neighbor+0x1d6>
+    646c39f8:	movslq %ecx,%rcx
+    646c39fb:	movsd  (%r10,%rcx,8),%xmm0
+    646c3a01:	subsd  0x10(%rbx),%xmm0
+    646c3a06:	andpd  %xmm1,%xmm0
+    646c3a0a:	movsd  %xmm0,(%r9,%rcx,8)
+    646c3a10:	xor    %ecx,%ecx
+    646c3a12:	comisd %xmm0,%xmm7
+    646c3a16:	seta   %cl
+    646c3a19:	add    $0x2,%edx
+    646c3a1c:	add    %ecx,%eax
+    646c3a1e:	cmp    %r11d,%edx
+    646c3a21:	jge    646c3a46 <find_neighbor+0x1d6>
+    646c3a23:	movslq %edx,%rdx
+    646c3a26:	movsd  (%r10,%rdx,8),%xmm0
+    646c3a2c:	subsd  0x10(%rbx),%xmm0
+    646c3a31:	andpd  %xmm0,%xmm1
+    646c3a35:	movsd  %xmm1,(%r9,%rdx,8)
+    646c3a3b:	xor    %edx,%edx
+    646c3a3d:	comisd %xmm1,%xmm7
+    646c3a41:	seta   %dl
+    646c3a44:	add    %edx,%eax
+    646c3a46:	test   %eax,%eax
+    646c3a48:	je     646c3aa0 <find_neighbor+0x230>
+    646c3a4a:	mov    $0x1,%eax
+    646c3a4f:	movaps 0x30(%rsp),%xmm6
+    646c3a54:	movaps 0x40(%rsp),%xmm7
+    646c3a59:	add    $0x58,%rsp
+    646c3a5d:	pop    %rbx
+    646c3a5e:	pop    %rsi
+    646c3a5f:	ret
+    646c3a60:	mov    %r8,%rcx
+    646c3a63:	mov    %eax,0x2c(%rsp)
+    646c3a67:	call   646c3390 <mt19937_random_normal>
+    646c3a6c:	mov    0x86bd(%rip),%rcx        # 646cc130 <model>
+    646c3a73:	cvttsd2si 0x10(%rbx),%edx
+    646c3a78:	mov    0x2c(%rsp),%eax
+    646c3a7c:	mulsd  0x18(%rcx),%xmm0
+    646c3a81:	movslq %edx,%rdx
+    646c3a84:	movslq 0x8(%rbx),%rcx
+    646c3a88:	movsd  %xmm0,(%rsi,%rdx,8)
+    646c3a8d:	mov    0x18(%rbx),%rdx
+    646c3a91:	movsd  0x10(%rbx),%xmm0
+    646c3a96:	movsd  %xmm0,(%rdx,%rcx,8)
+    646c3a9b:	jmp    646c3a4f <find_neighbor+0x1df>
+    646c3a9d:	nopl   (%rax)
+    646c3aa0:	mov    %r8,%rcx
+    646c3aa3:	call   646c3390 <mt19937_random_normal>
+    646c3aa8:	mov    0x8681(%rip),%rdx        # 646cc130 <model>
+    646c3aaf:	cvttsd2si 0x10(%rbx),%eax
+    646c3ab4:	mulsd  0x18(%rdx),%xmm0
+    646c3ab9:	cltq
+    646c3abb:	movslq 0x8(%rbx),%rdx
+    646c3abf:	movsd  %xmm0,(%rsi,%rax,8)
+    646c3ac4:	mov    0x18(%rbx),%rax
+    646c3ac8:	movsd  0x10(%rbx),%xmm0
+    646c3acd:	movsd  %xmm0,(%rax,%rdx,8)
+    646c3ad2:	xor    %eax,%eax
+    646c3ad4:	jmp    646c3a4f <find_neighbor+0x1df>
+    646c3ad9:	nopl   0x0(%rax)
+    646c3ae0:	mov    %eax,%ecx
+    646c3ae2:	xor    %edx,%edx
+    646c3ae4:	xor    %eax,%eax
+    646c3ae6:	movq   0x5602(%rip),%xmm1        # 646c90f0 <.rdata+0x30>
+    646c3aee:	jmp    646c3af3 <find_neighbor+0x283>
+    646c3af0:	mov    %r11,%rdx
+    646c3af3:	movsd  (%r10,%rdx,8),%xmm0
+    646c3af9:	xor    %r11d,%r11d
+    646c3afc:	subsd  0x10(%rbx),%xmm0
+    646c3b01:	andpd  %xmm1,%xmm0
+    646c3b05:	comisd %xmm0,%xmm7
+    646c3b09:	movsd  %xmm0,(%r9,%rdx,8)
+    646c3b0f:	seta   %r11b
+    646c3b13:	add    %r11d,%eax
+    646c3b16:	cmp    %rcx,%rdx
+    646c3b19:	lea    0x1(%rdx),%r11
+    646c3b1d:	jne    646c3af0 <find_neighbor+0x280>
+    646c3b1f:	jmp    646c3a46 <find_neighbor+0x1d6>
+    646c3b24:	xchg   %ax,%ax
+    646c3b26:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c3b30 <simple_kriging>:
+    646c3b30:	push   %r12
+    646c3b32:	push   %rbp
+    646c3b33:	push   %rdi
+    646c3b34:	push   %rsi
+    646c3b35:	push   %rbx
+    646c3b36:	sub    $0x30,%rsp
+    646c3b3a:	movaps %xmm6,0x20(%rsp)
+    646c3b3f:	mov    %rcx,%rbp
+    646c3b42:	mov    %rdx,%rbx
+    646c3b45:	mov    %r8,%rsi
+    646c3b48:	mov    %r9d,%edi
+    646c3b4b:	call   646c3870 <find_neighbor>
+    646c3b50:	test   %eax,%eax
+    646c3b52:	je     646c3d97 <simple_kriging+0x267>
+    646c3b58:	mov    0x4(%rbx),%r12d
+    646c3b5c:	test   %r12d,%r12d
+    646c3b5f:	jle    646c3bb6 <simple_kriging+0x86>
+    646c3b61:	mov    0x18(%rbx),%r11
+    646c3b65:	lea    -0x1(%r12),%r8d
+    646c3b6a:	xor    %edx,%edx
+    646c3b6c:	mov    0x84ed(%rip),%r10        # 646cc060 <distance_mat>
+    646c3b73:	mov    0x30(%rbx),%r9
+    646c3b77:	jmp    646c3b83 <simple_kriging+0x53>
+    646c3b79:	nopl   0x0(%rax)
+    646c3b80:	mov    %rax,%rdx
+    646c3b83:	movsd  (%r11,%rdx,8),%xmm0
+    646c3b89:	cmp    %rdx,%r8
+    646c3b8c:	mov    (%r10,%rdx,8),%rcx
+    646c3b90:	cvttsd2si %xmm0,%eax
+    646c3b94:	movsd  %xmm0,(%rcx)
+    646c3b98:	cltq
+    646c3b9a:	movsd  0x0(%rbp,%rax,8),%xmm0
+    646c3ba0:	lea    0x1(%rdx),%rax
+    646c3ba4:	movsd  %xmm0,0x8(%rcx)
+    646c3ba9:	movsd  (%r9,%rdx,8),%xmm0
+    646c3baf:	movsd  %xmm0,0x10(%rcx)
+    646c3bb4:	jne    646c3b80 <simple_kriging+0x50>
+    646c3bb6:	mov    (%rbx),%r8d
+    646c3bb9:	cmp    $0x1,%r8d
+    646c3bbd:	jg     646c3db0 <simple_kriging+0x280>
+    646c3bc3:	test   %r8d,%r8d
+    646c3bc6:	mov    0x8533(%rip),%rcx        # 646cc100 <location>
+    646c3bcd:	jle    646c3c09 <simple_kriging+0xd9>
+    646c3bcf:	mov    0x848a(%rip),%r12        # 646cc060 <distance_mat>
+    646c3bd6:	lea    -0x1(%r8),%r10d
+    646c3bda:	xor    %eax,%eax
+    646c3bdc:	mov    0x84dd(%rip),%r11        # 646cc0c0 <location_cov2d>
+    646c3be3:	jmp    646c3be8 <simple_kriging+0xb8>
+    646c3be5:	mov    %rdx,%rax
+    646c3be8:	mov    (%r12,%rax,8),%rdx
+    646c3bec:	cmp    %rax,%r10
+    646c3bef:	movsd  (%rdx),%xmm0
+    646c3bf3:	movsd  %xmm0,(%rcx,%rax,8)
+    646c3bf8:	movsd  0x10(%rdx),%xmm0
+    646c3bfd:	lea    0x1(%rax),%rdx
+    646c3c01:	movsd  %xmm0,(%r11,%rax,8)
+    646c3c07:	jne    646c3be5 <simple_kriging+0xb5>
+    646c3c09:	mov    0x8430(%rip),%rdx        # 646cc040 <pdist_temp>
+    646c3c10:	call   646c4790 <pdist>
+    646c3c15:	mov    0x8514(%rip),%r9        # 646cc130 <model>
+    646c3c1c:	mov    (%rbx),%r8d
+    646c3c1f:	mov    0x847a(%rip),%rdx        # 646cc0a0 <flatten_temp>
+    646c3c26:	mov    0x8413(%rip),%rcx        # 646cc040 <pdist_temp>
+    646c3c2d:	call   646c3520 <cov_model2d>
+    646c3c32:	mov    (%rbx),%r8d
+    646c3c35:	mov    0x83e4(%rip),%rdx        # 646cc020 <data_cov>
+    646c3c3c:	mov    0x845d(%rip),%rcx        # 646cc0a0 <flatten_temp>
+    646c3c43:	call   646c48e0 <matrixform>
+    646c3c48:	mov    0x84e1(%rip),%r9        # 646cc130 <model>
+    646c3c4f:	mov    (%rbx),%r8d
+    646c3c52:	mov    0x8487(%rip),%rdx        # 646cc0e0 <location_cov>
+    646c3c59:	mov    0x8460(%rip),%rcx        # 646cc0c0 <location_cov2d>
+    646c3c60:	call   646c3460 <cov_model>
+    646c3c65:	cmp    $0x1,%edi
+    646c3c68:	je     646c3de0 <simple_kriging+0x2b0>
+    646c3c6e:	mov    (%rbx),%r9d
+    646c3c71:	mov    %r9d,%eax
+    646c3c74:	test   %eax,%eax
+    646c3c76:	jg     646c3ca0 <simple_kriging+0x170>
+    646c3c78:	pxor   %xmm4,%xmm4
+    646c3c7c:	pxor   %xmm1,%xmm1
+    646c3c80:	movq   $0x0,0x8495(%rip)        # 646cc120 <estimation>
+    646c3c8b:	movq   $0x0,0x8482(%rip)        # 646cc118 <kriging_var>
+    646c3c96:	jmp    646c3d3f <simple_kriging+0x20f>
+    646c3c9b:	nopl   0x0(%rax,%rax,1)
+    646c3ca0:	mov    0x83d9(%rip),%r8        # 646cc080 <weights>
+    646c3ca7:	mov    0x8432(%rip),%rdx        # 646cc0e0 <location_cov>
+    646c3cae:	mov    0x836b(%rip),%rcx        # 646cc020 <data_cov>
+    646c3cb5:	call   646c43c0 <lu_inverse_solver>
+    646c3cba:	mov    (%rbx),%eax
+    646c3cbc:	pxor   %xmm4,%xmm4
+    646c3cc0:	movq   $0x0,0x8455(%rip)        # 646cc120 <estimation>
+    646c3ccb:	movq   $0x0,0x8442(%rip)        # 646cc118 <kriging_var>
+    646c3cd6:	test   %eax,%eax
+    646c3cd8:	jle    646c3e93 <simple_kriging+0x363>
+    646c3cde:	lea    -0x1(%rax),%ecx
+    646c3ce1:	mov    0x8378(%rip),%r10        # 646cc060 <distance_mat>
+    646c3ce8:	xor    %eax,%eax
+    646c3cea:	pxor   %xmm1,%xmm1
+    646c3cee:	mov    0x838b(%rip),%r9        # 646cc080 <weights>
+    646c3cf5:	pxor   %xmm2,%xmm2
+    646c3cf9:	mov    0x83e0(%rip),%r8        # 646cc0e0 <location_cov>
+    646c3d00:	jmp    646c3d05 <simple_kriging+0x1d5>
+    646c3d02:	mov    %rdx,%rax
+    646c3d05:	mov    (%r10,%rax,8),%rdx
+    646c3d09:	cmp    %rcx,%rax
+    646c3d0c:	movsd  (%r9,%rax,8),%xmm0
+    646c3d12:	movsd  0x8(%rdx),%xmm3
+    646c3d17:	lea    0x1(%rax),%rdx
+    646c3d1b:	mulsd  %xmm0,%xmm3
+    646c3d1f:	mulsd  (%r8,%rax,8),%xmm0
+    646c3d25:	addsd  %xmm3,%xmm2
+    646c3d29:	addsd  %xmm0,%xmm1
+    646c3d2d:	jne    646c3d02 <simple_kriging+0x1d2>
+    646c3d2f:	movsd  %xmm2,0x83e9(%rip)        # 646cc120 <estimation>
+    646c3d37:	movsd  %xmm1,0x83d9(%rip)        # 646cc118 <kriging_var>
+    646c3d3f:	mov    0x83ea(%rip),%rax        # 646cc130 <model>
+    646c3d46:	movsd  0x18(%rax),%xmm0
+    646c3d4b:	subsd  %xmm1,%xmm0
+    646c3d4f:	comisd %xmm0,%xmm4
+    646c3d53:	ja     646c3dd0 <simple_kriging+0x2a0>
+    646c3d55:	movsd  %xmm0,0x83bb(%rip)        # 646cc118 <kriging_var>
+    646c3d5d:	mov    %rsi,%rcx
+    646c3d60:	call   646c3390 <mt19937_random_normal>
+    646c3d65:	movsd  0x539b(%rip),%xmm1        # 646c9108 <.rdata+0x48>
+    646c3d6d:	movapd %xmm0,%xmm6
+    646c3d71:	movsd  0x839f(%rip),%xmm0        # 646cc118 <kriging_var>
+    646c3d79:	call   646c6ea0 <pow>
+    646c3d7e:	cvttsd2si 0x10(%rbx),%eax
+    646c3d83:	mulsd  %xmm0,%xmm6
+    646c3d87:	addsd  0x8391(%rip),%xmm6        # 646cc120 <estimation>
+    646c3d8f:	cltq
+    646c3d91:	movsd  %xmm6,0x0(%rbp,%rax,8)
+    646c3d97:	movaps 0x20(%rsp),%xmm6
+    646c3d9c:	add    $0x30,%rsp
+    646c3da0:	pop    %rbx
+    646c3da1:	pop    %rsi
+    646c3da2:	pop    %rdi
+    646c3da3:	pop    %rbp
+    646c3da4:	pop    %r12
+    646c3da6:	ret
+    646c3da7:	nopw   0x0(%rax,%rax,1)
+    646c3db0:	mov    0x82a9(%rip),%rcx        # 646cc060 <distance_mat>
+    646c3db7:	mov    %r8d,%r9d
+    646c3dba:	xor    %edx,%edx
+    646c3dbc:	lea    -0x1(%r12),%r8d
+    646c3dc1:	call   646c5160 <quickselect2d>
+    646c3dc6:	mov    (%rbx),%r8d
+    646c3dc9:	jmp    646c3bc3 <simple_kriging+0x93>
+    646c3dce:	xchg   %ax,%ax
+    646c3dd0:	movq   $0x0,0x833d(%rip)        # 646cc118 <kriging_var>
+    646c3ddb:	jmp    646c3d5d <simple_kriging+0x22d>
+    646c3ddd:	nopl   (%rax)
+    646c3de0:	movslq (%rbx),%rdx
+    646c3de3:	mov    0x8236(%rip),%r10        # 646cc020 <data_cov>
+    646c3dea:	mov    %rdx,%r9
+    646c3ded:	mov    %edx,%eax
+    646c3def:	shl    $0x3,%rdx
+    646c3df3:	test   %r9d,%r9d
+    646c3df6:	jle    646c3e87 <simple_kriging+0x357>
+    646c3dfc:	lea    -0x1(%r9),%ecx
+    646c3e00:	movsd  0x52f8(%rip),%xmm0        # 646c9100 <.rdata+0x40>
+    646c3e08:	mov    %r10,%rax
+    646c3e0b:	lea    0x8(%r10,%rcx,8),%r8
+    646c3e10:	mov    (%rax),%rcx
+    646c3e13:	add    $0x8,%rax
+    646c3e17:	cmp    %rax,%r8
+    646c3e1a:	movsd  %xmm0,(%rcx,%rdx,1)
+    646c3e1f:	jne    646c3e10 <simple_kriging+0x2e0>
+    646c3e21:	add    %r10,%rdx
+    646c3e24:	xor    %eax,%eax
+    646c3e26:	cs nopw 0x0(%rax,%rax,1)
+    646c3e30:	cmp    %eax,%r9d
+    646c3e33:	je     646c3e70 <simple_kriging+0x340>
+    646c3e35:	mov    (%rdx),%rcx
+    646c3e38:	movsd  %xmm0,(%rcx,%rax,8)
+    646c3e3d:	add    $0x1,%rax
+    646c3e41:	cmp    %eax,%r9d
+    646c3e44:	jge    646c3e30 <simple_kriging+0x300>
+    646c3e46:	movslq %r9d,%rdx
+    646c3e49:	mov    %r9d,%eax
+    646c3e4c:	shl    $0x3,%rdx
+    646c3e50:	mov    0x8289(%rip),%rcx        # 646cc0e0 <location_cov>
+    646c3e57:	add    $0x1,%r9d
+    646c3e5b:	test   %eax,%eax
+    646c3e5d:	movsd  %xmm0,(%rcx,%rdx,1)
+    646c3e62:	jle    646c3c78 <simple_kriging+0x148>
+    646c3e68:	jmp    646c3ca0 <simple_kriging+0x170>
+    646c3e6d:	nopl   (%rax)
+    646c3e70:	mov    (%r10,%rax,8),%rcx
+    646c3e74:	movq   $0x0,(%rcx,%rax,8)
+    646c3e7c:	add    $0x1,%rax
+    646c3e80:	cmp    %eax,%r9d
+    646c3e83:	jge    646c3e30 <simple_kriging+0x300>
+    646c3e85:	jmp    646c3e46 <simple_kriging+0x316>
+    646c3e87:	movsd  0x5271(%rip),%xmm0        # 646c9100 <.rdata+0x40>
+    646c3e8f:	jne    646c3e50 <simple_kriging+0x320>
+    646c3e91:	jmp    646c3e21 <simple_kriging+0x2f1>
+    646c3e93:	pxor   %xmm1,%xmm1
+    646c3e97:	jmp    646c3d3f <simple_kriging+0x20f>
+    646c3e9c:	nopl   0x0(%rax)
+
+00000000646c3ea0 <matrix_agumented>:
+    646c3ea0:	sub    $0x28,%rsp
+    646c3ea4:	movaps %xmm6,(%rsp)
+    646c3ea8:	movaps %xmm7,0x10(%rsp)
+    646c3ead:	test   %edx,%edx
+    646c3eaf:	jle    646c3ff0 <matrix_agumented+0x150>
+    646c3eb5:	movslq %edx,%r11
+    646c3eb8:	movsd  0x5240(%rip),%xmm0        # 646c9100 <.rdata+0x40>
+    646c3ec0:	mov    %rcx,%rax
+    646c3ec3:	lea    -0x1(%rdx),%r8d
+    646c3ec7:	lea    0x0(,%r11,8),%r10
+    646c3ecf:	lea    0x8(%rcx,%r8,8),%r9
+    646c3ed4:	mov    (%rax),%r8
+    646c3ed7:	add    $0x8,%rax
+    646c3edb:	cmp    %r9,%rax
+    646c3ede:	movsd  %xmm0,(%r8,%r10,1)
+    646c3ee4:	jne    646c3ed4 <matrix_agumented+0x34>
+    646c3ee6:	mov    (%rcx,%r11,8),%r8
+    646c3eea:	lea    0x1(%rdx),%r9d
+    646c3eee:	cmp    $0x2,%edx
+    646c3ef1:	jle    646c4000 <matrix_agumented+0x160>
+    646c3ef7:	mov    %r9d,%ecx
+    646c3efa:	movd   %edx,%xmm5
+    646c3efe:	mov    %r8,%rax
+    646c3f01:	movdqa 0x5207(%rip),%xmm2        # 646c9110 <.rdata+0x50>
+    646c3f09:	shr    $0x2,%ecx
+    646c3f0c:	movdqa 0x520c(%rip),%xmm6        # 646c9120 <.rdata+0x60>
+    646c3f14:	pshufd $0x0,%xmm5,%xmm7
+    646c3f19:	pxor   %xmm5,%xmm5
+    646c3f1d:	shl    $0x5,%rcx
+    646c3f21:	movapd 0x5207(%rip),%xmm4        # 646c9130 <.rdata+0x70>
+    646c3f29:	add    %r8,%rcx
+    646c3f2c:	nopl   0x0(%rax)
+    646c3f30:	movdqa %xmm2,%xmm0
+    646c3f34:	movdqa %xmm5,%xmm3
+    646c3f38:	add    $0x20,%rax
+    646c3f3c:	pcmpeqd %xmm7,%xmm0
+    646c3f40:	paddd  %xmm6,%xmm2
+    646c3f44:	pcmpgtd %xmm0,%xmm3
+    646c3f48:	movdqa %xmm0,%xmm1
+    646c3f4c:	punpckldq %xmm3,%xmm1
+    646c3f50:	punpckhdq %xmm3,%xmm0
+    646c3f54:	andnpd %xmm4,%xmm1
+    646c3f58:	andnpd %xmm4,%xmm0
+    646c3f5c:	movlpd %xmm1,-0x20(%rax)
+    646c3f61:	movhpd %xmm1,-0x18(%rax)
+    646c3f66:	movlpd %xmm0,-0x10(%rax)
+    646c3f6b:	movhpd %xmm0,-0x8(%rax)
+    646c3f70:	cmp    %rax,%rcx
+    646c3f73:	jne    646c3f30 <matrix_agumented+0x90>
+    646c3f75:	mov    %r9d,%eax
+    646c3f78:	and    $0xfffffffc,%eax
+    646c3f7b:	cmp    %eax,%r9d
+    646c3f7e:	je     646c3fc0 <matrix_agumented+0x120>
+    646c3f80:	movslq %eax,%rcx
+    646c3f83:	cmp    %eax,%edx
+    646c3f85:	movsd  0x5173(%rip),%xmm0        # 646c9100 <.rdata+0x40>
+    646c3f8d:	lea    (%r8,%rcx,8),%rcx
+    646c3f91:	je     646c3fd0 <matrix_agumented+0x130>
+    646c3f93:	movsd  %xmm0,(%rcx)
+    646c3f97:	lea    0x1(%rax),%ecx
+    646c3f9a:	cmp    %edx,%ecx
+    646c3f9c:	jg     646c3fc0 <matrix_agumented+0x120>
+    646c3f9e:	movslq %ecx,%r9
+    646c3fa1:	lea    (%r8,%r9,8),%r9
+    646c3fa5:	je     646c3fe5 <matrix_agumented+0x145>
+    646c3fa7:	movsd  %xmm0,(%r9)
+    646c3fac:	add    $0x2,%eax
+    646c3faf:	cmp    %eax,%edx
+    646c3fb1:	jl     646c3fc0 <matrix_agumented+0x120>
+    646c3fb3:	movslq %eax,%rcx
+    646c3fb6:	lea    (%r8,%rcx,8),%rcx
+    646c3fba:	je     646c3fd0 <matrix_agumented+0x130>
+    646c3fbc:	movsd  %xmm0,(%rcx)
+    646c3fc0:	movaps (%rsp),%xmm6
+    646c3fc4:	movaps 0x10(%rsp),%xmm7
+    646c3fc9:	add    $0x28,%rsp
+    646c3fcd:	ret
     646c3fce:	xchg   %ax,%ax
-    646c3fd0:	jne    646c3fa0 <matrix_agumented+0x120>
-    646c3fd2:	mov    (%rcx),%r8
-    646c3fd5:	xor    %eax,%eax
-    646c3fd7:	jmp    646c3f60 <matrix_agumented+0xe0>
-    646c3fd9:	nopl   0x0(%rax)
-    646c3fe0:	mov    %r8,%rcx
-    646c3fe3:	xor    %eax,%eax
-    646c3fe5:	jmp    646c3f73 <matrix_agumented+0xf3>
-    646c3fe7:	nopw   0x0(%rax,%rax,1)
-
-00000000646c3ff0 <kriging_memory_free>:
-    646c3ff0:	push   %rdi
-    646c3ff1:	push   %rsi
-    646c3ff2:	push   %rbx
-    646c3ff3:	sub    $0x20,%rsp
-    646c3ff7:	mov    0x8122(%rip),%rcx        # 646cc120 <location>
-    646c3ffe:	call   646c7988 <free>
-    646c4003:	mov    0x80f6(%rip),%rcx        # 646cc100 <loc_cov>
-    646c400a:	call   646c7988 <free>
-    646c400f:	mov    0x80ca(%rip),%rcx        # 646cc0e0 <data_temp>
-    646c4016:	call   646c7988 <free>
-    646c401b:	mov    0x809e(%rip),%rcx        # 646cc0c0 <loc_cov2>
-    646c4022:	call   646c7988 <free>
-    646c4027:	mov    0x8072(%rip),%rcx        # 646cc0a0 <flatten_temp>
-    646c402e:	call   646c7988 <free>
-    646c4033:	mov    0x8046(%rip),%rcx        # 646cc080 <weights>
-    646c403a:	call   646c7988 <free>
-    646c403f:	mov    0x8022(%rip),%rax        # 646cc068 <array2d_temp+0x8>
-    646c4046:	mov    0x8013(%rip),%rdi        # 646cc060 <array2d_temp>
-    646c404d:	test   %rax,%rax
-    646c4050:	lea    (%rdi,%rax,8),%rsi
-    646c4054:	mov    %rdi,%rbx
-    646c4057:	je     646c4071 <kriging_memory_free+0x81>
-    646c4059:	nopl   0x0(%rax)
-    646c4060:	mov    (%rbx),%rcx
-    646c4063:	add    $0x8,%rbx
-    646c4067:	call   646c7988 <free>
-    646c406c:	cmp    %rbx,%rsi
-    646c406f:	jne    646c4060 <kriging_memory_free+0x70>
-    646c4071:	mov    %rdi,%rcx
-    646c4074:	call   646c7988 <free>
-    646c4079:	mov    0x7fc8(%rip),%rax        # 646cc048 <pdist_temp+0x8>
-    646c4080:	mov    0x7fb9(%rip),%rdi        # 646cc040 <pdist_temp>
-    646c4087:	test   %rax,%rax
-    646c408a:	lea    (%rdi,%rax,8),%rsi
-    646c408e:	mov    %rdi,%rbx
-    646c4091:	je     646c40a4 <kriging_memory_free+0xb4>
-    646c4093:	mov    (%rbx),%rcx
-    646c4096:	add    $0x8,%rbx
-    646c409a:	call   646c7988 <free>
-    646c409f:	cmp    %rbx,%rsi
-    646c40a2:	jne    646c4093 <kriging_memory_free+0xa3>
-    646c40a4:	mov    %rdi,%rcx
-    646c40a7:	call   646c7988 <free>
-    646c40ac:	mov    0x7f75(%rip),%rax        # 646cc028 <datacov+0x8>
-    646c40b3:	mov    0x7f66(%rip),%rdi        # 646cc020 <datacov>
-    646c40ba:	test   %rax,%rax
-    646c40bd:	lea    (%rdi,%rax,8),%rsi
-    646c40c1:	mov    %rdi,%rbx
-    646c40c4:	je     646c40e1 <kriging_memory_free+0xf1>
-    646c40c6:	cs nopw 0x0(%rax,%rax,1)
-    646c40d0:	mov    (%rbx),%rcx
-    646c40d3:	add    $0x8,%rbx
-    646c40d7:	call   646c7988 <free>
-    646c40dc:	cmp    %rbx,%rsi
-    646c40df:	jne    646c40d0 <kriging_memory_free+0xe0>
-    646c40e1:	mov    %rdi,%rcx
-    646c40e4:	add    $0x20,%rsp
-    646c40e8:	pop    %rbx
-    646c40e9:	pop    %rsi
-    646c40ea:	pop    %rdi
-    646c40eb:	jmp    646c7988 <free>
-
-00000000646c40f0 <snprintf.constprop.0>:
-    646c40f0:	sub    $0x38,%rsp
-    646c40f4:	mov    $0xc8,%edx
-    646c40f9:	mov    %r9,0x58(%rsp)
-    646c40fe:	lea    0x58(%rsp),%r9
-    646c4103:	mov    %r9,0x28(%rsp)
-    646c4108:	call   646c6a70 <__ms_vsnprintf>
-    646c410d:	add    $0x38,%rsp
-    646c4111:	ret
-    646c4112:	nopl   0x0(%rax)
-    646c4116:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c4120 <lu_decomposition>:
-    646c4120:	push   %r15
-    646c4122:	push   %r14
-    646c4124:	push   %r13
-    646c4126:	push   %r12
-    646c4128:	push   %rbp
-    646c4129:	push   %rdi
-    646c412a:	push   %rsi
-    646c412b:	push   %rbx
-    646c412c:	xor    %r11d,%r11d
-    646c412f:	xor    %esi,%esi
-    646c4131:	mov    $0xffffffff,%r14d
-    646c4137:	test   %r9d,%r9d
-    646c413a:	jle    646c4259 <lu_decomposition+0x139>
-    646c4140:	movsd  0x5088(%rip),%xmm4        # 646c91d0 <.rdata+0x80>
-    646c4148:	movdqa 0x5050(%rip),%xmm5        # 646c91a0 <.rdata+0x50>
-    646c4150:	movdqa 0x5058(%rip),%xmm3        # 646c91b0 <.rdata+0x60>
-    646c4158:	movdqa 0x5060(%rip),%xmm2        # 646c91c0 <.rdata+0x70>
-    646c4160:	test   %esi,%esi
-    646c4162:	jg     646c4285 <lu_decomposition+0x165>
-    646c4168:	xor    %r10d,%r10d
-    646c416b:	movslq %r10d,%r10
-    646c416e:	mov    %r14d,%r12d
-    646c4171:	mov    (%rcx,%r10,8),%rax
-    646c4175:	mov    (%rdx,%r10,8),%rbp
-    646c4179:	movsd  (%rax,%r11,1),%xmm1
-    646c417f:	xor    %eax,%eax
-    646c4181:	test   %esi,%esi
-    646c4183:	lea    0x0(%rbp,%r11,1),%rdi
-    646c4188:	movsd  %xmm1,(%rdi)
-    646c418c:	jne    646c4193 <lu_decomposition+0x73>
-    646c418e:	jmp    646c41b4 <lu_decomposition+0x94>
-    646c4190:	mov    %rbx,%rax
-    646c4193:	mov    (%r8,%rax,8),%rbx
-    646c4197:	cmp    %r12,%rax
-    646c419a:	movsd  (%rbx,%r11,1),%xmm0
-    646c41a0:	lea    0x1(%rax),%rbx
-    646c41a4:	mulsd  0x0(%rbp,%rax,8),%xmm0
-    646c41aa:	subsd  %xmm0,%xmm1
-    646c41ae:	movsd  %xmm1,(%rdi)
-    646c41b2:	jne    646c4190 <lu_decomposition+0x70>
-    646c41b4:	add    $0x1,%r10
-    646c41b8:	cmp    %r10d,%r9d
-    646c41bb:	jg     646c4171 <lu_decomposition+0x51>
-    646c41bd:	test   %esi,%esi
-    646c41bf:	mov    (%r8,%r11,1),%rdi
-    646c41c3:	jg     646c42c0 <lu_decomposition+0x1a0>
-    646c41c9:	xor    %r10d,%r10d
-    646c41cc:	movslq %r10d,%r10
-    646c41cf:	mov    %r14d,%r15d
-    646c41d2:	lea    0x0(,%r10,8),%rbp
-    646c41da:	cmp    %r10d,%esi
-    646c41dd:	je     646c4270 <lu_decomposition+0x150>
-    646c41e3:	mov    (%rdx,%r11,1),%r13
-    646c41e7:	test   %esi,%esi
-    646c41e9:	mov    (%rcx,%r11,1),%rax
-    646c41ed:	lea    0x0(%r13,%r11,1),%r12
-    646c41f2:	movsd  (%rax,%r10,8),%xmm1
-    646c41f8:	divsd  (%r12),%xmm1
-    646c41fe:	movsd  %xmm1,(%rdi,%r10,8)
-    646c4204:	jle    646c423c <lu_decomposition+0x11c>
-    646c4206:	xor    %eax,%eax
-    646c4208:	jmp    646c4213 <lu_decomposition+0xf3>
-    646c420a:	nopw   0x0(%rax,%rax,1)
-    646c4210:	mov    %rbx,%rax
-    646c4213:	mov    (%r8,%rax,8),%rbx
-    646c4217:	cmp    %rax,%r15
-    646c421a:	movsd  (%rbx,%rbp,1),%xmm0
-    646c421f:	lea    0x1(%rax),%rbx
-    646c4223:	mulsd  0x0(%r13,%rax,8),%xmm0
-    646c422a:	divsd  (%r12),%xmm0
-    646c4230:	subsd  %xmm0,%xmm1
-    646c4234:	movsd  %xmm1,(%rdi,%r10,8)
-    646c423a:	jne    646c4210 <lu_decomposition+0xf0>
-    646c423c:	add    $0x1,%r10
-    646c4240:	cmp    %r10d,%r9d
-    646c4243:	jg     646c41d2 <lu_decomposition+0xb2>
-    646c4245:	add    $0x1,%esi
-    646c4248:	add    $0x8,%r11
-    646c424c:	add    $0x1,%r14d
-    646c4250:	cmp    %esi,%r9d
-    646c4253:	jne    646c4160 <lu_decomposition+0x40>
-    646c4259:	pop    %rbx
-    646c425a:	pop    %rsi
-    646c425b:	pop    %rdi
-    646c425c:	pop    %rbp
-    646c425d:	pop    %r12
-    646c425f:	pop    %r13
-    646c4261:	pop    %r14
-    646c4263:	pop    %r15
-    646c4265:	ret
-    646c4266:	cs nopw 0x0(%rax,%rax,1)
-    646c4270:	movsd  %xmm4,(%rdi,%r10,8)
-    646c4276:	add    $0x1,%r10
-    646c427a:	cmp    %r10d,%r9d
-    646c427d:	jg     646c41d2 <lu_decomposition+0xb2>
-    646c4283:	jmp    646c4245 <lu_decomposition+0x125>
-    646c4285:	cmp    %esi,%r9d
-    646c4288:	mov    %esi,%edi
-    646c428a:	mov    %rdx,%rax
-    646c428d:	cmovle %r9d,%edi
-    646c4291:	xor    %r10d,%r10d
-    646c4294:	mov    (%rax),%rbx
-    646c4297:	add    $0x1,%r10d
-    646c429b:	add    $0x8,%rax
-    646c429f:	cmp    %edi,%r10d
-    646c42a2:	movq   $0x0,(%rbx,%r11,1)
-    646c42aa:	jl     646c4294 <lu_decomposition+0x174>
-    646c42ac:	cmp    %r10d,%r9d
-    646c42af:	jg     646c416b <lu_decomposition+0x4b>
-    646c42b5:	mov    (%r8,%r11,1),%rdi
-    646c42b9:	nopl   0x0(%rax)
-    646c42c0:	cmp    %esi,%r9d
-    646c42c3:	mov    %esi,%ebx
-    646c42c5:	mov    $0x1,%ebp
-    646c42ca:	cmovle %r9d,%ebx
-    646c42ce:	test   %ebx,%ebx
-    646c42d0:	cmovg  %ebx,%ebp
-    646c42d3:	cmp    $0x4,%ebx
-    646c42d6:	jle    646c43a5 <lu_decomposition+0x285>
-    646c42dc:	mov    %ebp,%r10d
-    646c42df:	mov    %rdi,%rax
-    646c42e2:	movdqa %xmm5,%xmm1
-    646c42e6:	shr    $0x2,%r10d
-    646c42ea:	shl    $0x5,%r10
-    646c42ee:	add    %rdi,%r10
-    646c42f1:	movq   $0x0,(%rax)
-    646c42f8:	add    $0x20,%rax
-    646c42fc:	movdqa %xmm1,%xmm0
-    646c4300:	paddd  %xmm3,%xmm1
-    646c4304:	movq   $0x0,-0x18(%rax)
-    646c430c:	paddd  %xmm2,%xmm0
-    646c4310:	movq   $0x0,-0x10(%rax)
-    646c4318:	movq   $0x0,-0x8(%rax)
-    646c4320:	cmp    %rax,%r10
-    646c4323:	jne    646c42f1 <lu_decomposition+0x1d1>
-    646c4325:	mov    %ebp,%eax
-    646c4327:	pshufd $0xff,%xmm0,%xmm0
-    646c432c:	movd   %xmm0,%r10d
-    646c4331:	and    $0xfffffffc,%eax
-    646c4334:	cmp    %ebp,%eax
-    646c4336:	je     646c4383 <lu_decomposition+0x263>
-    646c4338:	movslq %eax,%r10
-    646c433b:	movq   $0x0,(%rdi,%r10,8)
-    646c4343:	lea    0x1(%rax),%r10d
-    646c4347:	cmp    %ebx,%r10d
-    646c434a:	jge    646c4383 <lu_decomposition+0x263>
-    646c434c:	movslq %r10d,%r10
-    646c434f:	movq   $0x0,(%rdi,%r10,8)
-    646c4357:	lea    0x2(%rax),%r10d
-    646c435b:	cmp    %ebx,%r10d
-    646c435e:	jge    646c4383 <lu_decomposition+0x263>
-    646c4360:	movslq %r10d,%r10
-    646c4363:	movq   $0x0,(%rdi,%r10,8)
-    646c436b:	lea    0x3(%rax),%r10d
-    646c436f:	cmp    %ebx,%r10d
-    646c4372:	jge    646c4383 <lu_decomposition+0x263>
-    646c4374:	movslq %r10d,%r10
-    646c4377:	movq   $0x0,(%rdi,%r10,8)
-    646c437f:	lea    0x4(%rax),%r10d
-    646c4383:	cmp    %r9d,%r10d
-    646c4386:	jl     646c41cc <lu_decomposition+0xac>
-    646c438c:	add    $0x1,%esi
-    646c438f:	add    $0x8,%r11
-    646c4393:	add    $0x1,%r14d
-    646c4397:	cmp    %esi,%r9d
-    646c439a:	jne    646c4160 <lu_decomposition+0x40>
-    646c43a0:	jmp    646c4259 <lu_decomposition+0x139>
-    646c43a5:	xor    %eax,%eax
-    646c43a7:	jmp    646c4338 <lu_decomposition+0x218>
-    646c43a9:	nopl   0x0(%rax)
-
-00000000646c43b0 <lu_inverse_solver>:
-    646c43b0:	push   %r15
-    646c43b2:	push   %r14
-    646c43b4:	push   %r13
-    646c43b6:	push   %r12
-    646c43b8:	push   %rbp
-    646c43b9:	push   %rdi
-    646c43ba:	push   %rsi
-    646c43bb:	push   %rbx
-    646c43bc:	sub    $0xa8,%rsp
-    646c43c3:	mov    %rcx,0x38(%rsp)
-    646c43c8:	mov    $0x50,%ecx
-    646c43cd:	mov    %rdx,%r14
-    646c43d0:	mov    %r8,%r15
-    646c43d3:	mov    %r9d,%ebx
-    646c43d6:	call   646c7970 <malloc>
-    646c43db:	mov    %rax,0x30(%rsp)
-    646c43e0:	lea    0x50(%rax),%r12
-    646c43e4:	mov    %rax,%rdi
-    646c43e7:	mov    %rax,%rsi
-    646c43ea:	nopw   0x0(%rax,%rax,1)
-    646c43f0:	mov    $0x50,%ecx
-    646c43f5:	add    $0x8,%rdi
-    646c43f9:	call   646c7970 <malloc>
-    646c43fe:	mov    %rax,-0x8(%rdi)
-    646c4402:	cmp    %r12,%rdi
-    646c4405:	jne    646c43f0 <lu_inverse_solver+0x40>
-    646c4407:	mov    $0x50,%ecx
-    646c440c:	call   646c7970 <malloc>
-    646c4411:	mov    %rax,0x28(%rsp)
-    646c4416:	lea    0x50(%rax),%rbp
-    646c441a:	mov    %rax,%r13
-    646c441d:	mov    %rax,%rdi
-    646c4420:	mov    $0x50,%ecx
-    646c4425:	add    $0x8,%r13
-    646c4429:	call   646c7970 <malloc>
-    646c442e:	mov    %rax,-0x8(%r13)
-    646c4432:	cmp    %rbp,%r13
-    646c4435:	jne    646c4420 <lu_inverse_solver+0x70>
-    646c4437:	mov    0x30(%rsp),%r13
-    646c443c:	mov    %ebx,%r9d
-    646c443f:	mov    0x28(%rsp),%r8
-    646c4444:	mov    0x38(%rsp),%rcx
-    646c4449:	mov    %r13,%rdx
-    646c444c:	call   646c4120 <lu_decomposition>
-    646c4451:	mov    0x0(%r13),%rax
-    646c4455:	movslq %ebx,%r10
-    646c4458:	movsd  (%r14),%xmm0
-    646c445d:	divsd  (%rax),%xmm0
-    646c4461:	lea    0x0(,%r10,8),%rax
-    646c4469:	movsd  %xmm0,0x50(%rsp)
-    646c446f:	mov    %rax,0x48(%rsp)
-    646c4474:	add    %r15,%rax
-    646c4477:	cmp    $0x1,%ebx
-    646c447a:	mov    %rax,0x38(%rsp)
-    646c447f:	lea    -0x1(%rbx),%eax
-    646c4482:	mov    %eax,0x44(%rsp)
-    646c4486:	jle    646c477e <lu_inverse_solver+0x3ce>
-    646c448c:	lea    0x50(%rsp),%r11
-    646c4491:	mov    $0x1,%edx
-    646c4496:	lea    0x8(%r11),%rax
-    646c449a:	nopw   0x0(%rax,%rax,1)
-    646c44a0:	mov    0x0(%r13,%rdx,8),%rcx
-    646c44a5:	cmp    $0x1,%rdx
-    646c44a9:	movsd  (%r14,%rdx,8),%xmm0
-    646c44af:	lea    0x0(,%rdx,8),%r9
-    646c44b7:	movsd  %xmm0,(%rax)
-    646c44bb:	movsd  (%rcx),%xmm1
-    646c44bf:	mulsd  0x50(%rsp),%xmm1
-    646c44c5:	subsd  %xmm1,%xmm0
-    646c44c9:	movsd  %xmm0,(%rax)
-    646c44cd:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c44d3:	movsd  0x8(%rcx),%xmm1
-    646c44d8:	cmp    $0x2,%edx
-    646c44db:	mulsd  0x58(%rsp),%xmm1
-    646c44e1:	subsd  %xmm1,%xmm0
-    646c44e5:	movsd  %xmm0,(%rax)
-    646c44e9:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c44ef:	movsd  0x10(%rcx),%xmm1
-    646c44f4:	cmp    $0x3,%edx
-    646c44f7:	mulsd  0x60(%rsp),%xmm1
-    646c44fd:	subsd  %xmm1,%xmm0
-    646c4501:	movsd  %xmm0,(%rax)
-    646c4505:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c450b:	movsd  0x18(%rcx),%xmm1
-    646c4510:	cmp    $0x4,%edx
-    646c4513:	mulsd  0x68(%rsp),%xmm1
-    646c4519:	subsd  %xmm1,%xmm0
-    646c451d:	movsd  %xmm0,(%rax)
-    646c4521:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c4523:	movsd  0x20(%rcx),%xmm1
-    646c4528:	cmp    $0x5,%edx
-    646c452b:	mulsd  0x70(%rsp),%xmm1
-    646c4531:	subsd  %xmm1,%xmm0
-    646c4535:	movsd  %xmm0,(%rax)
-    646c4539:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c453b:	movsd  0x28(%rcx),%xmm1
-    646c4540:	cmp    $0x6,%edx
-    646c4543:	mulsd  0x78(%rsp),%xmm1
-    646c4549:	subsd  %xmm1,%xmm0
-    646c454d:	movsd  %xmm0,(%rax)
-    646c4551:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c4553:	movsd  0x30(%rcx),%xmm1
-    646c4558:	cmp    $0x7,%edx
-    646c455b:	mulsd  0x80(%rsp),%xmm1
-    646c4564:	subsd  %xmm1,%xmm0
-    646c4568:	movsd  %xmm0,(%rax)
-    646c456c:	je     646c459b <lu_inverse_solver+0x1eb>
-    646c456e:	movsd  0x38(%rcx),%xmm1
-    646c4573:	cmp    $0x9,%edx
-    646c4576:	mulsd  0x88(%rsp),%xmm1
-    646c457f:	subsd  %xmm1,%xmm0
-    646c4583:	movsd  %xmm0,(%rax)
-    646c4587:	jne    646c459b <lu_inverse_solver+0x1eb>
-    646c4589:	movsd  0x40(%rcx),%xmm1
-    646c458e:	mulsd  0x90(%rsp),%xmm1
-    646c4597:	subsd  %xmm1,%xmm0
-    646c459b:	add    $0x1,%rdx
-    646c459f:	divsd  (%rcx,%r9,1),%xmm0
-    646c45a5:	add    $0x8,%rax
-    646c45a9:	movsd  %xmm0,-0x8(%rax)
-    646c45ae:	cmp    %edx,%ebx
-    646c45b0:	jg     646c44a0 <lu_inverse_solver+0xf0>
-    646c45b6:	mov    0x38(%rsp),%rax
-    646c45bb:	movsd  0x50(%rsp,%r10,8),%xmm0
-    646c45c2:	movsd  %xmm0,(%rax)
-    646c45c6:	mov    0x48(%rsp),%rax
-    646c45cb:	movslq 0x44(%rsp),%rdx
-    646c45d0:	mov    0x28(%rsp),%r10
-    646c45d5:	lea    -0x8(%r15,%rax,1),%rax
-    646c45da:	nopw   0x0(%rax,%rax,1)
-    646c45e0:	movsd  (%r11,%rdx,8),%xmm0
-    646c45e6:	lea    0x1(%rdx),%r8d
-    646c45ea:	mov    %edx,%ecx
-    646c45ec:	cmp    %r8d,%ebx
-    646c45ef:	movsd  %xmm0,(%rax)
-    646c45f3:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c45f9:	mov    (%r10,%rdx,8),%r8
-    646c45fd:	lea    0x2(%rdx),%r9d
-    646c4601:	cmp    %r9d,%ebx
-    646c4604:	movsd  0x8(%r8,%rdx,8),%xmm1
-    646c460b:	mulsd  0x8(%rax),%xmm1
-    646c4610:	subsd  %xmm1,%xmm0
-    646c4614:	movsd  %xmm0,(%rax)
-    646c4618:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c461e:	movslq %r9d,%r9
-    646c4621:	movsd  (%r15,%r9,8),%xmm1
-    646c4627:	mulsd  (%r8,%r9,8),%xmm1
-    646c462d:	lea    0x3(%rdx),%r9d
-    646c4631:	cmp    %r9d,%ebx
-    646c4634:	subsd  %xmm1,%xmm0
-    646c4638:	movsd  %xmm0,(%rax)
-    646c463c:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c4642:	movslq %r9d,%r9
-    646c4645:	movsd  (%r15,%r9,8),%xmm1
-    646c464b:	mulsd  (%r8,%r9,8),%xmm1
-    646c4651:	lea    0x4(%rdx),%r9d
-    646c4655:	cmp    %r9d,%ebx
-    646c4658:	subsd  %xmm1,%xmm0
-    646c465c:	movsd  %xmm0,(%rax)
-    646c4660:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c4666:	movslq %r9d,%r9
-    646c4669:	movsd  (%r15,%r9,8),%xmm1
-    646c466f:	mulsd  (%r8,%r9,8),%xmm1
-    646c4675:	lea    0x5(%rdx),%r9d
-    646c4679:	cmp    %r9d,%ebx
-    646c467c:	subsd  %xmm1,%xmm0
-    646c4680:	movsd  %xmm0,(%rax)
-    646c4684:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c468a:	movslq %r9d,%r9
-    646c468d:	movsd  (%r15,%r9,8),%xmm1
-    646c4693:	mulsd  (%r8,%r9,8),%xmm1
-    646c4699:	lea    0x6(%rdx),%r9d
-    646c469d:	cmp    %r9d,%ebx
-    646c46a0:	subsd  %xmm1,%xmm0
-    646c46a4:	movsd  %xmm0,(%rax)
-    646c46a8:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c46aa:	movslq %r9d,%r9
-    646c46ad:	movsd  (%r15,%r9,8),%xmm1
-    646c46b3:	mulsd  (%r8,%r9,8),%xmm1
-    646c46b9:	lea    0x7(%rdx),%r9d
-    646c46bd:	cmp    %r9d,%ebx
-    646c46c0:	subsd  %xmm1,%xmm0
-    646c46c4:	movsd  %xmm0,(%rax)
-    646c46c8:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c46ca:	movslq %r9d,%r9
-    646c46cd:	movsd  (%r15,%r9,8),%xmm1
-    646c46d3:	mulsd  (%r8,%r9,8),%xmm1
-    646c46d9:	lea    0x8(%rdx),%r9d
-    646c46dd:	cmp    %r9d,%ebx
-    646c46e0:	subsd  %xmm1,%xmm0
-    646c46e4:	movsd  %xmm0,(%rax)
-    646c46e8:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c46ea:	movslq %r9d,%r9
-    646c46ed:	add    $0x9,%ecx
-    646c46f0:	movsd  (%r8,%r9,8),%xmm1
-    646c46f6:	cmp    %ecx,%ebx
-    646c46f8:	mulsd  (%r15,%r9,8),%xmm1
-    646c46fe:	subsd  %xmm1,%xmm0
-    646c4702:	movsd  %xmm0,(%rax)
-    646c4706:	jle    646c471f <lu_inverse_solver+0x36f>
-    646c4708:	movslq %ecx,%rcx
-    646c470b:	movsd  (%r8,%rcx,8),%xmm1
-    646c4711:	mulsd  (%r15,%rcx,8),%xmm1
-    646c4717:	subsd  %xmm1,%xmm0
-    646c471b:	movsd  %xmm0,(%rax)
-    646c471f:	sub    $0x1,%rdx
-    646c4723:	sub    $0x8,%rax
-    646c4727:	test   %edx,%edx
-    646c4729:	jns    646c45e0 <lu_inverse_solver+0x230>
-    646c472f:	nop
-    646c4730:	mov    (%rsi),%rcx
-    646c4733:	add    $0x8,%rsi
-    646c4737:	call   646c7988 <free>
-    646c473c:	cmp    %r12,%rsi
-    646c473f:	jne    646c4730 <lu_inverse_solver+0x380>
-    646c4741:	mov    0x30(%rsp),%rcx
-    646c4746:	call   646c7988 <free>
-    646c474b:	nopl   0x0(%rax,%rax,1)
-    646c4750:	mov    (%rdi),%rcx
-    646c4753:	add    $0x8,%rdi
-    646c4757:	call   646c7988 <free>
-    646c475c:	cmp    %rbp,%rdi
-    646c475f:	jne    646c4750 <lu_inverse_solver+0x3a0>
-    646c4761:	mov    0x28(%rsp),%rcx
-    646c4766:	add    $0xa8,%rsp
-    646c476d:	pop    %rbx
-    646c476e:	pop    %rsi
-    646c476f:	pop    %rdi
-    646c4770:	pop    %rbp
-    646c4771:	pop    %r12
-    646c4773:	pop    %r13
-    646c4775:	pop    %r14
-    646c4777:	pop    %r15
-    646c4779:	jmp    646c7988 <free>
-    646c477e:	mov    0x38(%rsp),%rax
-    646c4783:	movsd  0x50(%rsp,%r10,8),%xmm0
-    646c478a:	movsd  %xmm0,(%rax)
-    646c478e:	mov    0x44(%rsp),%eax
-    646c4792:	test   %eax,%eax
-    646c4794:	js     646c4730 <lu_inverse_solver+0x380>
-    646c4796:	lea    0x50(%rsp),%r11
-    646c479b:	jmp    646c45c6 <lu_inverse_solver+0x216>
-
-00000000646c47a0 <arange>:
-    646c47a0:	push   %rbx
-    646c47a1:	sub    $0x20,%rsp
-    646c47a5:	movslq %ecx,%rcx
-    646c47a8:	mov    %rcx,%rbx
-    646c47ab:	shl    $0x2,%rcx
-    646c47af:	call   646c7970 <malloc>
-    646c47b4:	test   %ebx,%ebx
-    646c47b6:	jle    646c481a <arange+0x7a>
-    646c47b8:	lea    -0x1(%rbx),%edx
-    646c47bb:	cmp    $0x2,%edx
-    646c47be:	jbe    646c4820 <arange+0x80>
-    646c47c0:	mov    %ebx,%ecx
-    646c47c2:	movdqa 0x49d6(%rip),%xmm0        # 646c91a0 <.rdata+0x50>
-    646c47ca:	mov    %rax,%rdx
-    646c47cd:	shr    $0x2,%ecx
-    646c47d0:	movdqa 0x49d8(%rip),%xmm1        # 646c91b0 <.rdata+0x60>
-    646c47d8:	shl    $0x4,%rcx
-    646c47dc:	add    %rax,%rcx
-    646c47df:	nop
-    646c47e0:	movups %xmm0,(%rdx)
-    646c47e3:	add    $0x10,%rdx
-    646c47e7:	paddd  %xmm1,%xmm0
-    646c47eb:	cmp    %rcx,%rdx
-    646c47ee:	jne    646c47e0 <arange+0x40>
-    646c47f0:	mov    %ebx,%edx
-    646c47f2:	and    $0xfffffffc,%edx
-    646c47f5:	cmp    %edx,%ebx
-    646c47f7:	je     646c481a <arange+0x7a>
-    646c47f9:	movslq %edx,%rcx
-    646c47fc:	mov    %edx,(%rax,%rcx,4)
-    646c47ff:	lea    0x1(%rdx),%ecx
-    646c4802:	cmp    %ecx,%ebx
-    646c4804:	jle    646c481a <arange+0x7a>
-    646c4806:	add    $0x2,%edx
-    646c4809:	movslq %ecx,%r8
-    646c480c:	cmp    %edx,%ebx
-    646c480e:	mov    %ecx,(%rax,%r8,4)
-    646c4812:	jle    646c481a <arange+0x7a>
-    646c4814:	movslq %edx,%rcx
-    646c4817:	mov    %edx,(%rax,%rcx,4)
-    646c481a:	add    $0x20,%rsp
-    646c481e:	pop    %rbx
-    646c481f:	ret
-    646c4820:	xor    %edx,%edx
-    646c4822:	jmp    646c47f9 <arange+0x59>
-    646c4824:	xchg   %ax,%ax
-    646c4826:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c4830 <d_arange>:
-    646c4830:	push   %rbx
-    646c4831:	sub    $0x20,%rsp
-    646c4835:	movslq %ecx,%rcx
-    646c4838:	mov    %rcx,%rbx
-    646c483b:	shl    $0x3,%rcx
-    646c483f:	call   646c7970 <malloc>
-    646c4844:	test   %ebx,%ebx
-    646c4846:	jle    646c48f6 <d_arange+0xc6>
-    646c484c:	lea    -0x1(%rbx),%edx
-    646c484f:	cmp    $0x2,%edx
-    646c4852:	jbe    646c48fc <d_arange+0xcc>
-    646c4858:	mov    %ebx,%ecx
-    646c485a:	movdqa 0x493e(%rip),%xmm1        # 646c91a0 <.rdata+0x50>
-    646c4862:	mov    %rax,%rdx
-    646c4865:	shr    $0x2,%ecx
-    646c4868:	movdqa 0x4940(%rip),%xmm2        # 646c91b0 <.rdata+0x60>
-    646c4870:	shl    $0x5,%rcx
-    646c4874:	add    %rax,%rcx
-    646c4877:	nopw   0x0(%rax,%rax,1)
-    646c4880:	cvtdq2pd %xmm1,%xmm0
-    646c4884:	add    $0x20,%rdx
-    646c4888:	movlpd %xmm0,-0x20(%rdx)
-    646c488d:	movhpd %xmm0,-0x18(%rdx)
-    646c4892:	pshufd $0xee,%xmm1,%xmm0
-    646c4897:	cvtdq2pd %xmm0,%xmm0
-    646c489b:	paddd  %xmm2,%xmm1
-    646c489f:	movlpd %xmm0,-0x10(%rdx)
-    646c48a4:	movhpd %xmm0,-0x8(%rdx)
-    646c48a9:	cmp    %rcx,%rdx
-    646c48ac:	jne    646c4880 <d_arange+0x50>
-    646c48ae:	mov    %ebx,%edx
-    646c48b0:	and    $0xfffffffc,%edx
-    646c48b3:	cmp    %edx,%ebx
-    646c48b5:	je     646c48f6 <d_arange+0xc6>
-    646c48b7:	pxor   %xmm0,%xmm0
-    646c48bb:	cvtsi2sd %edx,%xmm0
-    646c48bf:	movslq %edx,%rcx
-    646c48c2:	movsd  %xmm0,(%rax,%rcx,8)
-    646c48c7:	lea    0x1(%rdx),%ecx
-    646c48ca:	cmp    %ecx,%ebx
-    646c48cc:	jle    646c48f6 <d_arange+0xc6>
-    646c48ce:	pxor   %xmm0,%xmm0
-    646c48d2:	cvtsi2sd %ecx,%xmm0
-    646c48d6:	add    $0x2,%edx
-    646c48d9:	movslq %ecx,%r8
-    646c48dc:	cmp    %edx,%ebx
-    646c48de:	movsd  %xmm0,(%rax,%r8,8)
-    646c48e4:	jle    646c48f6 <d_arange+0xc6>
-    646c48e6:	pxor   %xmm0,%xmm0
-    646c48ea:	cvtsi2sd %edx,%xmm0
-    646c48ee:	movslq %edx,%rcx
-    646c48f1:	movsd  %xmm0,(%rax,%rcx,8)
-    646c48f6:	add    $0x20,%rsp
-    646c48fa:	pop    %rbx
-    646c48fb:	ret
-    646c48fc:	xor    %edx,%edx
-    646c48fe:	jmp    646c48b7 <d_arange+0x87>
-
-00000000646c4900 <pdist>:
-    646c4900:	push   %r15
-    646c4902:	push   %r14
-    646c4904:	push   %r13
-    646c4906:	push   %r12
-    646c4908:	push   %rbp
-    646c4909:	push   %rdi
-    646c490a:	push   %rsi
-    646c490b:	push   %rbx
-    646c490c:	sub    $0x28,%rsp
-    646c4910:	test   %r8d,%r8d
-    646c4913:	jle    646c4a08 <pdist+0x108>
-    646c4919:	lea    -0x1(%r8),%r13d
-    646c491d:	mov    %r8d,%r10d
-    646c4920:	movslq %r8d,%r14
-    646c4923:	movq   0x48b5(%rip),%xmm4        # 646c91e0 <.rdata+0x90>
-    646c492b:	lea    0x8(%rcx,%r13,8),%rax
-    646c4930:	shr    %r10d
-    646c4933:	movapd 0x48b5(%rip),%xmm2        # 646c91f0 <.rdata+0xa0>
-    646c493b:	mov    %rdx,%rdi
-    646c493e:	mov    %rax,0x8(%rsp)
-    646c4943:	mov    %r8d,%eax
-    646c4946:	mov    %rcx,%r9
-    646c4949:	mov    %r13,%r15
-    646c494c:	and    $0xfffffffe,%eax
-    646c494f:	shl    $0x3,%r14
-    646c4953:	movapd %xmm4,%xmm3
-    646c4957:	mov    %eax,%r11d
-    646c495a:	mov    %eax,0x1c(%rsp)
-    646c495e:	shl    $0x4,%r10
-    646c4962:	lea    0x10(%rcx),%rax
-    646c4966:	shl    $0x3,%r11
-    646c496a:	lea    (%rcx,%r11,1),%rdx
-    646c496e:	mov    %rax,0x10(%rsp)
-    646c4973:	mov    (%rdi),%rax
-    646c4976:	lea    0x8(%r9),%rbp
-    646c497a:	lea    0x10(%rax),%rbx
-    646c497e:	cmp    %rbx,%rcx
-    646c4981:	setae  %sil
-    646c4985:	cmp    0x10(%rsp),%rax
-    646c498a:	setae  %bl
-    646c498d:	or     %ebx,%esi
-    646c498f:	lea    (%rax,%r14,1),%rbx
-    646c4993:	cmp    %rbx,%r9
-    646c4996:	setae  %bl
-    646c4999:	cmp    %rbp,%rax
-    646c499c:	setae  %r12b
-    646c49a0:	or     %r12d,%ebx
-    646c49a3:	test   %bl,%sil
-    646c49a6:	je     646c4a20 <pdist+0x120>
-    646c49a8:	cmp    $0x2,%r15d
-    646c49ac:	jbe    646c4a20 <pdist+0x120>
-    646c49ae:	xor    %ebx,%ebx
-    646c49b0:	movddup (%r9),%xmm1
-    646c49b5:	movq   (%rcx,%rbx,1),%xmm0
-    646c49ba:	movhpd 0x8(%rcx,%rbx,1),%xmm0
-    646c49c0:	subpd  %xmm1,%xmm0
-    646c49c4:	andpd  %xmm2,%xmm0
-    646c49c8:	movlpd %xmm0,(%rax,%rbx,1)
-    646c49cd:	movhpd %xmm0,0x8(%rax,%rbx,1)
-    646c49d3:	add    $0x10,%rbx
-    646c49d7:	cmp    %r10,%rbx
-    646c49da:	jne    646c49b5 <pdist+0xb5>
-    646c49dc:	cmp    %r8d,0x1c(%rsp)
-    646c49e1:	je     646c49f6 <pdist+0xf6>
-    646c49e3:	movsd  (%rdx),%xmm0
-    646c49e7:	subsd  (%r9),%xmm0
-    646c49ec:	andpd  %xmm3,%xmm0
-    646c49f0:	movsd  %xmm0,(%rax,%r11,1)
-    646c49f6:	add    $0x8,%rdi
-    646c49fa:	cmp    0x8(%rsp),%rbp
-    646c49ff:	mov    %rbp,%r9
-    646c4a02:	jne    646c4973 <pdist+0x73>
-    646c4a08:	add    $0x28,%rsp
-    646c4a0c:	pop    %rbx
-    646c4a0d:	pop    %rsi
-    646c4a0e:	pop    %rdi
-    646c4a0f:	pop    %rbp
-    646c4a10:	pop    %r12
-    646c4a12:	pop    %r13
-    646c4a14:	pop    %r14
-    646c4a16:	pop    %r15
-    646c4a18:	ret
-    646c4a19:	nopl   0x0(%rax)
-    646c4a20:	xor    %ebx,%ebx
-    646c4a22:	jmp    646c4a27 <pdist+0x127>
-    646c4a24:	mov    %rsi,%rbx
-    646c4a27:	movsd  (%rcx,%rbx,8),%xmm0
-    646c4a2c:	lea    0x1(%rbx),%rsi
-    646c4a30:	cmp    %r13,%rbx
-    646c4a33:	subsd  (%r9),%xmm0
-    646c4a38:	andpd  %xmm4,%xmm0
-    646c4a3c:	movsd  %xmm0,(%rax,%rbx,8)
-    646c4a41:	jne    646c4a24 <pdist+0x124>
-    646c4a43:	jmp    646c49f6 <pdist+0xf6>
-    646c4a45:	nop
-    646c4a46:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c4a50 <matrixform>:
-    646c4a50:	push   %r14
-    646c4a52:	push   %r13
-    646c4a54:	push   %r12
-    646c4a56:	push   %rbp
-    646c4a57:	push   %rdi
-    646c4a58:	push   %rsi
-    646c4a59:	push   %rbx
-    646c4a5a:	test   %r8d,%r8d
-    646c4a5d:	jle    646c4b08 <matrixform+0xb8>
-    646c4a63:	mov    %r8d,%r11d
-    646c4a66:	mov    %r8d,%ebp
-    646c4a69:	xor    %esi,%esi
-    646c4a6b:	lea    -0x1(%r8),%edi
-    646c4a6f:	shr    %r11d
-    646c4a72:	and    $0xfffffffe,%ebp
-    646c4a75:	mov    %rdi,%r12
-    646c4a78:	shl    $0x4,%r11
-    646c4a7c:	mov    %ebp,%ebx
-    646c4a7e:	lea    0x8(%rdx,%rdi,8),%r13
-    646c4a83:	mov    (%rdx),%r9
-    646c4a86:	movslq %esi,%rax
-    646c4a89:	lea    0x10(,%rax,8),%rax
-    646c4a91:	lea    -0x10(%rcx,%rax,1),%r10
-    646c4a96:	add    %rcx,%rax
-    646c4a99:	cmp    %rax,%r9
-    646c4a9c:	lea    0x10(%r9),%rax
-    646c4aa0:	setae  %r14b
-    646c4aa4:	cmp    %rax,%r10
-    646c4aa7:	setae  %al
-    646c4aaa:	or     %al,%r14b
-    646c4aad:	je     646c4b13 <matrixform+0xc3>
-    646c4aaf:	xor    %eax,%eax
-    646c4ab1:	cmp    $0x3,%r12d
-    646c4ab5:	jbe    646c4b13 <matrixform+0xc3>
-    646c4ab7:	nopw   0x0(%rax,%rax,1)
-    646c4ac0:	movq   (%r10,%rax,1),%xmm0
-    646c4ac6:	movhpd 0x8(%r10,%rax,1),%xmm0
-    646c4acd:	movlpd %xmm0,(%r9,%rax,1)
-    646c4ad3:	movhpd %xmm0,0x8(%r9,%rax,1)
-    646c4ada:	add    $0x10,%rax
-    646c4ade:	cmp    %r11,%rax
-    646c4ae1:	jne    646c4ac0 <matrixform+0x70>
-    646c4ae3:	lea    (%rsi,%rbp,1),%eax
-    646c4ae6:	cmp    %r8d,%ebp
-    646c4ae9:	je     646c4af8 <matrixform+0xa8>
-    646c4aeb:	cltq
-    646c4aed:	movsd  (%rcx,%rax,8),%xmm0
-    646c4af2:	movsd  %xmm0,(%r9,%rbx,8)
-    646c4af8:	add    $0x8,%rdx
-    646c4afc:	add    %r8d,%esi
-    646c4aff:	cmp    %r13,%rdx
-    646c4b02:	jne    646c4a83 <matrixform+0x33>
-    646c4b08:	pop    %rbx
-    646c4b09:	pop    %rsi
-    646c4b0a:	pop    %rdi
-    646c4b0b:	pop    %rbp
-    646c4b0c:	pop    %r12
-    646c4b0e:	pop    %r13
-    646c4b10:	pop    %r14
-    646c4b12:	ret
-    646c4b13:	xor    %eax,%eax
-    646c4b15:	jmp    646c4b23 <matrixform+0xd3>
-    646c4b17:	nopw   0x0(%rax,%rax,1)
-    646c4b20:	mov    %r14,%rax
-    646c4b23:	movsd  (%r10,%rax,8),%xmm0
-    646c4b29:	lea    0x1(%rax),%r14
-    646c4b2d:	cmp    %rdi,%rax
-    646c4b30:	movsd  %xmm0,(%r9,%rax,8)
-    646c4b36:	jne    646c4b20 <matrixform+0xd0>
-    646c4b38:	jmp    646c4af8 <matrixform+0xa8>
-    646c4b3a:	nopw   0x0(%rax,%rax,1)
-
-00000000646c4b40 <save_1darray>:
-    646c4b40:	push   %r13
-    646c4b42:	push   %r12
-    646c4b44:	push   %rbp
-    646c4b45:	push   %rdi
-    646c4b46:	push   %rsi
-    646c4b47:	push   %rbx
-    646c4b48:	sub    $0x1d8,%rsp
-    646c4b4f:	pxor   %xmm0,%xmm0
-    646c4b53:	mov    %rcx,%r12
-    646c4b56:	mov    %edx,%r13d
-    646c4b59:	mov    %r8,%rdi
-    646c4b5c:	cvtsi2sdl 0x230(%rsp),%xmm0
-    646c4b65:	mov    %r9,%rbx
-    646c4b68:	call   646c7978 <log10>
-    646c4b6d:	movsd  0x466b(%rip),%xmm3        # 646c91e0 <.rdata+0x90>
-    646c4b75:	movsd  0x4683(%rip),%xmm4        # 646c9200 <.rdata+0xb0>
-    646c4b7d:	movapd %xmm0,%xmm2
-    646c4b81:	movapd %xmm0,%xmm1
-    646c4b85:	andpd  %xmm3,%xmm2
-    646c4b89:	ucomisd %xmm2,%xmm4
-    646c4b8d:	jbe    646c4bba <save_1darray+0x7a>
-    646c4b8f:	cvttsd2si %xmm0,%rax
-    646c4b94:	pxor   %xmm2,%xmm2
-    646c4b98:	movsd  0x4630(%rip),%xmm4        # 646c91d0 <.rdata+0x80>
-    646c4ba0:	andnpd %xmm0,%xmm3
-    646c4ba4:	cvtsi2sd %rax,%xmm2
-    646c4ba9:	cmpnlesd %xmm2,%xmm1
-    646c4bae:	andpd  %xmm4,%xmm1
-    646c4bb2:	addsd  %xmm2,%xmm1
-    646c4bb6:	orpd   %xmm3,%xmm1
-    646c4bba:	cvttsd2si %xmm1,%eax
-    646c4bbe:	mov    %rbx,%r9
-    646c4bc1:	mov    %rdi,0x20(%rsp)
-    646c4bc6:	lea    0x30(%rsp),%rsi
-    646c4bcb:	mov    $0xc8,%edx
-    646c4bd0:	lea    0x4579(%rip),%r8        # 646c9150 <.rdata>
-    646c4bd7:	mov    %rsi,%rcx
-    646c4bda:	add    $0x1,%eax
-    646c4bdd:	mov    %eax,0x28(%rsp)
-    646c4be1:	call   646c40f0 <snprintf.constprop.0>
-    646c4be6:	mov    %rbx,%rcx
-    646c4be9:	call   646c79c8 <_mkdir>
-    646c4bee:	cmp    $0xffffffff,%eax
-    646c4bf1:	je     646c4c84 <save_1darray+0x144>
-    646c4bf7:	mov    0x238(%rsp),%r9d
-    646c4bff:	lea    0x100(%rsp),%rbx
-    646c4c07:	mov    %rsi,%r8
-    646c4c0a:	mov    $0xc8,%edx
-    646c4c0f:	mov    %rbx,%rcx
-    646c4c12:	call   646c40f0 <snprintf.constprop.0>
-    646c4c17:	lea    0x4557(%rip),%rdx        # 646c9175 <.rdata+0x25>
-    646c4c1e:	mov    %rbx,%rcx
-    646c4c21:	call   646c7998 <fopen>
-    646c4c26:	test   %rax,%rax
-    646c4c29:	mov    %rax,%rsi
-    646c4c2c:	je     646c4ca4 <save_1darray+0x164>
-    646c4c2e:	lea    -0x1(%r13),%ebp
-    646c4c32:	xor    %ebx,%ebx
-    646c4c34:	test   %r13d,%r13d
-    646c4c37:	lea    0x4551(%rip),%rdi        # 646c918f <.rdata+0x3f>
-    646c4c3e:	jg     646c4c45 <save_1darray+0x105>
-    646c4c40:	jmp    646c4c6b <save_1darray+0x12b>
-    646c4c42:	mov    %rax,%rbx
-    646c4c45:	movsd  (%r12,%rbx,8),%xmm0
-    646c4c4b:	mov    %ebx,%r8d
-    646c4c4e:	mov    %rdi,%rdx
-    646c4c51:	mov    %rsi,%rcx
-    646c4c54:	movapd %xmm0,%xmm3
-    646c4c58:	movq   %xmm0,%r9
-    646c4c5d:	call   646c7990 <fprintf>
-    646c4c62:	lea    0x1(%rbx),%rax
-    646c4c66:	cmp    %rbp,%rbx
-    646c4c69:	jne    646c4c42 <save_1darray+0x102>
-    646c4c6b:	mov    %rsi,%rcx
-    646c4c6e:	call   646c79a0 <fclose>
-    646c4c73:	nop
-    646c4c74:	add    $0x1d8,%rsp
-    646c4c7b:	pop    %rbx
-    646c4c7c:	pop    %rsi
-    646c4c7d:	pop    %rdi
-    646c4c7e:	pop    %rbp
-    646c4c7f:	pop    %r12
-    646c4c81:	pop    %r13
-    646c4c83:	ret
-    646c4c84:	call   *0x9612(%rip)        # 646ce29c <__imp__errno>
-    646c4c8a:	cmpl   $0x11,(%rax)
-    646c4c8d:	je     646c4bf7 <save_1darray+0xb7>
-    646c4c93:	lea    0x44c5(%rip),%rcx        # 646c915f <.rdata+0xf>
-    646c4c9a:	call   646c7960 <printf>
-    646c4c9f:	jmp    646c4bf7 <save_1darray+0xb7>
-    646c4ca4:	lea    0x44cc(%rip),%rcx        # 646c9177 <.rdata+0x27>
-    646c4cab:	call   646c7968 <perror>
-    646c4cb0:	mov    $0x1,%ecx
-    646c4cb5:	call   646c79a8 <exit>
-    646c4cba:	nop
-    646c4cbb:	nop
-    646c4cbc:	nop
-    646c4cbd:	nop
-    646c4cbe:	nop
-    646c4cbf:	nop
-
-00000000646c4cc0 <randompath>:
-    646c4cc0:	push   %rdi
-    646c4cc1:	push   %rsi
-    646c4cc2:	push   %rbx
-    646c4cc3:	sub    $0x20,%rsp
-    646c4cc7:	sub    $0x1,%edx
-    646c4cca:	mov    %rcx,%rdi
-    646c4ccd:	mov    %r8,%rsi
-    646c4cd0:	je     646c4cfa <randompath+0x3a>
-    646c4cd2:	movslq %edx,%rbx
-    646c4cd5:	mov    %rsi,%rcx
-    646c4cd8:	call   646c23e0 <mt19937_generate>
-    646c4cdd:	xor    %edx,%edx
-    646c4cdf:	mov    (%rdi,%rbx,4),%ecx
-    646c4ce2:	div    %ebx
-    646c4ce4:	movslq %edx,%rdx
-    646c4ce7:	lea    (%rdi,%rdx,4),%rax
-    646c4ceb:	mov    (%rax),%edx
-    646c4ced:	mov    %ecx,(%rax)
-    646c4cef:	mov    %edx,(%rdi,%rbx,4)
-    646c4cf2:	sub    $0x1,%rbx
-    646c4cf6:	test   %ebx,%ebx
-    646c4cf8:	jne    646c4cd5 <randompath+0x15>
-    646c4cfa:	mov    %rdi,%rax
-    646c4cfd:	add    $0x20,%rsp
-    646c4d01:	pop    %rbx
-    646c4d02:	pop    %rsi
-    646c4d03:	pop    %rdi
-    646c4d04:	ret
-    646c4d05:	nop
-    646c4d06:	nop
-    646c4d07:	nop
-    646c4d08:	nop
-    646c4d09:	nop
-    646c4d0a:	nop
-    646c4d0b:	nop
-    646c4d0c:	nop
-    646c4d0d:	nop
-    646c4d0e:	nop
-    646c4d0f:	nop
-
-00000000646c4d10 <sgsim_init>:
-    646c4d10:	push   %rbx
-    646c4d11:	sub    $0x20,%rsp
-    646c4d15:	cmpl   $0x1,0x58(%rsp)
-    646c4d1a:	movd   0x50(%rsp),%xmm2
-    646c4d20:	movd   %r9d,%xmm1
-    646c4d25:	movd   %edx,%xmm0
-    646c4d29:	mov    %rcx,%rbx
-    646c4d2c:	mov    %r8d,0x40(%rsp)
-    646c4d31:	movd   %r8d,%xmm3
-    646c4d36:	punpckldq %xmm2,%xmm1
-    646c4d3a:	punpckldq %xmm3,%xmm0
-    646c4d3e:	punpcklqdq %xmm1,%xmm0
-    646c4d42:	movups %xmm0,(%rcx)
-    646c4d45:	je     646c4d50 <sgsim_init+0x40>
-    646c4d47:	add    $0x20,%rsp
-    646c4d4b:	pop    %rbx
-    646c4d4c:	ret
-    646c4d4d:	nopl   (%rax)
-    646c4d50:	mov    %edx,%ecx
-    646c4d52:	mov    $0x8,%edx
-    646c4d57:	imul   %r8d,%ecx
-    646c4d5b:	call   646c79b0 <calloc>
-    646c4d60:	mov    %rax,0x18(%rbx)
-    646c4d64:	add    $0x20,%rsp
-    646c4d68:	pop    %rbx
-    646c4d69:	ret
-    646c4d6a:	nopw   0x0(%rax,%rax,1)
-
-00000000646c4d70 <sgsim_run>:
-    646c4d70:	push   %r15
-    646c4d72:	push   %r14
-    646c4d74:	push   %r13
-    646c4d76:	push   %r12
-    646c4d78:	push   %rbp
-    646c4d79:	push   %rdi
-    646c4d7a:	push   %rsi
-    646c4d7b:	push   %rbx
-    646c4d7c:	sub    $0xa08,%rsp
-    646c4d83:	mov    %rdx,0xa58(%rsp)
-    646c4d8b:	mov    0x8(%rcx),%edx
-    646c4d8e:	lea    0x30(%rsp),%r13
-    646c4d93:	mov    %rcx,%rsi
-    646c4d96:	mov    %r13,%rcx
-    646c4d99:	mov    %r8d,0xa60(%rsp)
-    646c4da1:	call   646c23a0 <mt19937_init>
-    646c4da6:	mov    (%rsi),%edx
-    646c4da8:	lea    0x73d1(%rip),%rcx        # 646cc180 <_sampling>
-    646c4daf:	call   646c3610 <sampling_state_init>
-    646c4db4:	mov    0xa58(%rsp),%rax
-    646c4dbc:	mov    $0x8,%edx
-    646c4dc1:	movslq 0x8(%rax),%rcx
-    646c4dc5:	movq   %rcx,%xmm0
-    646c4dca:	punpcklqdq %xmm0,%xmm0
-    646c4dce:	movups %xmm0,0x7423(%rip)        # 646cc1f8 <variogram_array+0x8>
-    646c4dd5:	call   646c79b0 <calloc>
-    646c4dda:	movslq (%rsi),%rcx
-    646c4ddd:	mov    $0x8,%edx
-    646c4de2:	mov    %rax,0x7407(%rip)        # 646cc1f0 <variogram_array>
-    646c4de9:	movq   %rcx,%xmm0
-    646c4dee:	mov    %rcx,%rbx
-    646c4df1:	punpcklqdq %xmm0,%xmm0
-    646c4df5:	movups %xmm0,0x73dc(%rip)        # 646cc1d8 <sgsim_array+0x8>
-    646c4dfc:	call   646c79b0 <calloc>
-    646c4e01:	mov    0xa58(%rsp),%rdx
-    646c4e09:	mov    %ebx,%ecx
-    646c4e0b:	mov    %rax,0x73be(%rip)        # 646cc1d0 <sgsim_array>
-    646c4e12:	call   646c3690 <kriging_param_setting>
-    646c4e17:	mov    (%rsi),%ecx
-    646c4e19:	call   646c47a0 <arange>
-    646c4e1e:	xor    %edx,%edx
-    646c4e20:	movl   $0x0,0x7336(%rip)        # 646cc160 <count>
-    646c4e2a:	mov    %rax,0x73df(%rip)        # 646cc210 <x_grid>
-    646c4e31:	cmp    %edx,0x4(%rsi)
-    646c4e34:	jle    646c4fd9 <sgsim_run+0x269>
-    646c4e3a:	lea    0x43cf(%rip),%rcx        # 646c9210 <.rdata>
-    646c4e41:	call   646c7960 <printf>
-    646c4e46:	mov    0x73c3(%rip),%rcx        # 646cc210 <x_grid>
-    646c4e4d:	mov    %r13,%r8
-    646c4e50:	movq   $0x0,0x7325(%rip)        # 646cc180 <_sampling>
-    646c4e5b:	mov    (%rsi),%edx
-    646c4e5d:	lea    0x73ac(%rip),%r14        # 646cc210 <x_grid>
-    646c4e64:	movl   $0x0,0x72f6(%rip)        # 646cc164 <flag>
-    646c4e6e:	call   646c4cc0 <randompath>
-    646c4e73:	mov    (%rsi),%r8d
-    646c4e76:	mov    %rax,0x7393(%rip)        # 646cc210 <x_grid>
-    646c4e7d:	test   %r8d,%r8d
-    646c4e80:	jle    646c4f78 <sgsim_run+0x208>
-    646c4e86:	lea    0x72f3(%rip),%r12        # 646cc180 <_sampling>
-    646c4e8d:	xor    %ebx,%ebx
-    646c4e8f:	lea    0x733a(%rip),%rbp        # 646cc1d0 <sgsim_array>
-    646c4e96:	mov    %r12,%rdi
-    646c4e99:	nopl   0x0(%rax)
-    646c4ea0:	pxor   %xmm1,%xmm1
-    646c4ea4:	cvtsi2sdl (%rax,%rbx,4),%xmm1
-    646c4ea9:	mov    %ebx,%r8d
-    646c4eac:	lea    0x0(,%rbx,4),%r15
-    646c4eb4:	mov    %rdi,%rcx
-    646c4eb7:	call   646c3680 <sampling_state_update>
-    646c4ebc:	mov    0xc(%rsi),%r9d
-    646c4ec0:	mov    %r13,%r8
-    646c4ec3:	mov    %rdi,%rdx
-    646c4ec6:	mov    0x0(%rbp),%rcx
-    646c4eca:	call   646c3b10 <simple_kriging>
-    646c4ecf:	mov    (%r14),%rax
-    646c4ed2:	mov    0x0(%rbp),%r9
-    646c4ed6:	mov    (%rsi),%r8d
-    646c4ed9:	mov    0x18(%rsi),%r10
-    646c4edd:	add    %rax,%r15
-    646c4ee0:	movslq (%r15),%rcx
-    646c4ee3:	mov    %rcx,%rdx
-    646c4ee6:	movsd  (%r9,%rcx,8),%xmm0
-    646c4eec:	mov    0x726e(%rip),%ecx        # 646cc160 <count>
-    646c4ef2:	imul   %r8d,%ecx
-    646c4ef6:	add    %edx,%ecx
-    646c4ef8:	movslq %ecx,%rcx
-    646c4efb:	movsd  %xmm0,(%r10,%rcx,8)
-    646c4f01:	mov    (%r12),%ecx
-    646c4f05:	cmp    $0x7,%ecx
-    646c4f08:	jg     646c4f14 <sgsim_run+0x1a4>
-    646c4f0a:	add    $0x1,%ecx
-    646c4f0d:	mov    %ecx,(%r12)
-    646c4f11:	mov    (%r15),%edx
-    646c4f14:	pxor   %xmm0,%xmm0
-    646c4f18:	cvtsi2sd %edx,%xmm0
-    646c4f1c:	mov    0x7275(%rip),%rdx        # 646cc198 <_sampling+0x18>
-    646c4f23:	movsd  %xmm0,(%rdx,%rbx,8)
-    646c4f28:	addl   $0x1,0x7255(%rip)        # 646cc184 <_sampling+0x4>
-    646c4f2f:	movslq (%r15),%rdx
-    646c4f32:	mov    (%r9,%rdx,8),%rcx
-    646c4f36:	mov    %rcx,%rdx
-    646c4f39:	shr    $0x20,%rdx
-    646c4f3d:	mov    %edx,%r9d
-    646c4f40:	and    $0x7fffffff,%r9d
-    646c4f47:	or     %ecx,%r9d
-    646c4f4a:	sete   %r9b
-    646c4f4e:	and    $0x7ff00000,%edx
-    646c4f54:	sete   %cl
-    646c4f57:	or     %cl,%r9b
-    646c4f5a:	jne    646c4f6b <sgsim_run+0x1fb>
-    646c4f5c:	cmp    $0x7ff00000,%edx
-    646c4f62:	jne    646c4f6b <sgsim_run+0x1fb>
-    646c4f64:	addl   $0x1,0x71f9(%rip)        # 646cc164 <flag>
-    646c4f6b:	add    $0x1,%rbx
-    646c4f6f:	cmp    %ebx,%r8d
-    646c4f72:	jg     646c4ea0 <sgsim_run+0x130>
-    646c4f78:	cmpl   $0x1,0xa60(%rsp)
-    646c4f80:	je     646c5030 <sgsim_run+0x2c0>
-    646c4f86:	mov    0x71d8(%rip),%eax        # 646cc164 <flag>
-    646c4f8c:	mov    0x71ce(%rip),%edx        # 646cc160 <count>
-    646c4f92:	test   %eax,%eax
-    646c4f94:	jne    646c4e31 <sgsim_run+0xc1>
-    646c4f9a:	mov    0x4(%rsi),%eax
-    646c4f9d:	mov    %edx,0x28(%rsp)
-    646c4fa1:	lea    0x4275(%rip),%r9        # 646c921d <.rdata+0xd>
-    646c4fa8:	mov    (%rsi),%edx
-    646c4faa:	lea    0x427c(%rip),%r8        # 646c922d <.rdata+0x1d>
-    646c4fb1:	mov    0x7218(%rip),%rcx        # 646cc1d0 <sgsim_array>
-    646c4fb8:	mov    %eax,0x20(%rsp)
-    646c4fbc:	call   646c4b40 <save_1darray>
-    646c4fc1:	mov    0x7199(%rip),%eax        # 646cc160 <count>
-    646c4fc7:	lea    0x1(%rax),%edx
-    646c4fca:	cmp    %edx,0x4(%rsi)
-    646c4fcd:	mov    %edx,0x718d(%rip)        # 646cc160 <count>
-    646c4fd3:	jg     646c4e3a <sgsim_run+0xca>
-    646c4fd9:	call   646c3ff0 <kriging_memory_free>
-    646c4fde:	mov    0x71b3(%rip),%rcx        # 646cc198 <_sampling+0x18>
-    646c4fe5:	call   646c7988 <free>
-    646c4fea:	mov    0x71bf(%rip),%rcx        # 646cc1b0 <_sampling+0x30>
-    646c4ff1:	call   646c7988 <free>
-    646c4ff6:	mov    0x71d3(%rip),%rcx        # 646cc1d0 <sgsim_array>
-    646c4ffd:	call   646c7988 <free>
-    646c5002:	mov    0x7207(%rip),%rcx        # 646cc210 <x_grid>
-    646c5009:	call   646c7988 <free>
-    646c500e:	mov    0x71db(%rip),%rcx        # 646cc1f0 <variogram_array>
-    646c5015:	call   646c7988 <free>
-    646c501a:	nop
-    646c501b:	add    $0xa08,%rsp
-    646c5022:	pop    %rbx
-    646c5023:	pop    %rsi
-    646c5024:	pop    %rdi
-    646c5025:	pop    %rbp
-    646c5026:	pop    %r12
-    646c5028:	pop    %r13
-    646c502a:	pop    %r14
-    646c502c:	pop    %r15
-    646c502e:	ret
+    646c3fd0:	movq   $0x0,(%rcx)
+    646c3fd7:	movaps (%rsp),%xmm6
+    646c3fdb:	movaps 0x10(%rsp),%xmm7
+    646c3fe0:	add    $0x28,%rsp
+    646c3fe4:	ret
+    646c3fe5:	movq   $0x0,(%r9)
+    646c3fec:	jmp    646c3fac <matrix_agumented+0x10c>
+    646c3fee:	xchg   %ax,%ax
+    646c3ff0:	jne    646c3fc0 <matrix_agumented+0x120>
+    646c3ff2:	mov    (%rcx),%r8
+    646c3ff5:	xor    %eax,%eax
+    646c3ff7:	jmp    646c3f80 <matrix_agumented+0xe0>
+    646c3ff9:	nopl   0x0(%rax)
+    646c4000:	mov    %r8,%rcx
+    646c4003:	xor    %eax,%eax
+    646c4005:	jmp    646c3f93 <matrix_agumented+0xf3>
+    646c4007:	nopw   0x0(%rax,%rax,1)
+
+00000000646c4010 <kriging_memory_free>:
+    646c4010:	push   %rdi
+    646c4011:	push   %rsi
+    646c4012:	push   %rbx
+    646c4013:	sub    $0x20,%rsp
+    646c4017:	mov    0x80e2(%rip),%rcx        # 646cc100 <location>
+    646c401e:	call   646c78c8 <free>
+    646c4023:	mov    0x80b6(%rip),%rcx        # 646cc0e0 <location_cov>
+    646c402a:	call   646c78c8 <free>
+    646c402f:	mov    0x808a(%rip),%rcx        # 646cc0c0 <location_cov2d>
+    646c4036:	call   646c78c8 <free>
+    646c403b:	mov    0x805e(%rip),%rcx        # 646cc0a0 <flatten_temp>
+    646c4042:	call   646c78c8 <free>
+    646c4047:	mov    0x8032(%rip),%rcx        # 646cc080 <weights>
+    646c404e:	call   646c78c8 <free>
+    646c4053:	mov    0x800e(%rip),%rax        # 646cc068 <distance_mat+0x8>
+    646c405a:	mov    0x7fff(%rip),%rdi        # 646cc060 <distance_mat>
+    646c4061:	test   %rax,%rax
+    646c4064:	lea    (%rdi,%rax,8),%rsi
+    646c4068:	mov    %rdi,%rbx
+    646c406b:	je     646c4081 <kriging_memory_free+0x71>
+    646c406d:	nopl   (%rax)
+    646c4070:	mov    (%rbx),%rcx
+    646c4073:	add    $0x8,%rbx
+    646c4077:	call   646c78c8 <free>
+    646c407c:	cmp    %rbx,%rsi
+    646c407f:	jne    646c4070 <kriging_memory_free+0x60>
+    646c4081:	mov    %rdi,%rcx
+    646c4084:	call   646c78c8 <free>
+    646c4089:	mov    0x7fb8(%rip),%rax        # 646cc048 <pdist_temp+0x8>
+    646c4090:	mov    0x7fa9(%rip),%rdi        # 646cc040 <pdist_temp>
+    646c4097:	test   %rax,%rax
+    646c409a:	lea    (%rdi,%rax,8),%rsi
+    646c409e:	mov    %rdi,%rbx
+    646c40a1:	je     646c40b4 <kriging_memory_free+0xa4>
+    646c40a3:	mov    (%rbx),%rcx
+    646c40a6:	add    $0x8,%rbx
+    646c40aa:	call   646c78c8 <free>
+    646c40af:	cmp    %rbx,%rsi
+    646c40b2:	jne    646c40a3 <kriging_memory_free+0x93>
+    646c40b4:	mov    %rdi,%rcx
+    646c40b7:	call   646c78c8 <free>
+    646c40bc:	mov    0x7f65(%rip),%rax        # 646cc028 <data_cov+0x8>
+    646c40c3:	mov    0x7f56(%rip),%rdi        # 646cc020 <data_cov>
+    646c40ca:	test   %rax,%rax
+    646c40cd:	lea    (%rdi,%rax,8),%rsi
+    646c40d1:	mov    %rdi,%rbx
+    646c40d4:	je     646c40f1 <kriging_memory_free+0xe1>
+    646c40d6:	cs nopw 0x0(%rax,%rax,1)
+    646c40e0:	mov    (%rbx),%rcx
+    646c40e3:	add    $0x8,%rbx
+    646c40e7:	call   646c78c8 <free>
+    646c40ec:	cmp    %rbx,%rsi
+    646c40ef:	jne    646c40e0 <kriging_memory_free+0xd0>
+    646c40f1:	mov    %rdi,%rcx
+    646c40f4:	add    $0x20,%rsp
+    646c40f8:	pop    %rbx
+    646c40f9:	pop    %rsi
+    646c40fa:	pop    %rdi
+    646c40fb:	jmp    646c78c8 <free>
+
+00000000646c4100 <snprintf.constprop.0>:
+    646c4100:	sub    $0x38,%rsp
+    646c4104:	mov    $0xc8,%edx
+    646c4109:	mov    %r9,0x58(%rsp)
+    646c410e:	lea    0x58(%rsp),%r9
+    646c4113:	mov    %r9,0x28(%rsp)
+    646c4118:	call   646c69b0 <__ms_vsnprintf>
+    646c411d:	add    $0x38,%rsp
+    646c4121:	ret
+    646c4122:	nopl   0x0(%rax)
+    646c4126:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c4130 <lu_decomposition>:
+    646c4130:	push   %r15
+    646c4132:	push   %r14
+    646c4134:	push   %r13
+    646c4136:	push   %r12
+    646c4138:	push   %rbp
+    646c4139:	push   %rdi
+    646c413a:	push   %rsi
+    646c413b:	push   %rbx
+    646c413c:	xor    %r11d,%r11d
+    646c413f:	xor    %esi,%esi
+    646c4141:	mov    $0xffffffff,%r14d
+    646c4147:	test   %r9d,%r9d
+    646c414a:	jle    646c4269 <lu_decomposition+0x139>
+    646c4150:	movsd  0x5068(%rip),%xmm4        # 646c91c0 <.rdata+0x80>
+    646c4158:	movdqa 0x5030(%rip),%xmm5        # 646c9190 <.rdata+0x50>
+    646c4160:	movdqa 0x5038(%rip),%xmm3        # 646c91a0 <.rdata+0x60>
+    646c4168:	movdqa 0x5040(%rip),%xmm2        # 646c91b0 <.rdata+0x70>
+    646c4170:	test   %esi,%esi
+    646c4172:	jg     646c4295 <lu_decomposition+0x165>
+    646c4178:	xor    %r10d,%r10d
+    646c417b:	movslq %r10d,%r10
+    646c417e:	mov    %r14d,%r12d
+    646c4181:	mov    (%rcx,%r10,8),%rax
+    646c4185:	mov    (%rdx,%r10,8),%rbp
+    646c4189:	movsd  (%rax,%r11,1),%xmm1
+    646c418f:	xor    %eax,%eax
+    646c4191:	test   %esi,%esi
+    646c4193:	lea    0x0(%rbp,%r11,1),%rdi
+    646c4198:	movsd  %xmm1,(%rdi)
+    646c419c:	jne    646c41a3 <lu_decomposition+0x73>
+    646c419e:	jmp    646c41c4 <lu_decomposition+0x94>
+    646c41a0:	mov    %rbx,%rax
+    646c41a3:	mov    (%r8,%rax,8),%rbx
+    646c41a7:	cmp    %r12,%rax
+    646c41aa:	movsd  (%rbx,%r11,1),%xmm0
+    646c41b0:	lea    0x1(%rax),%rbx
+    646c41b4:	mulsd  0x0(%rbp,%rax,8),%xmm0
+    646c41ba:	subsd  %xmm0,%xmm1
+    646c41be:	movsd  %xmm1,(%rdi)
+    646c41c2:	jne    646c41a0 <lu_decomposition+0x70>
+    646c41c4:	add    $0x1,%r10
+    646c41c8:	cmp    %r10d,%r9d
+    646c41cb:	jg     646c4181 <lu_decomposition+0x51>
+    646c41cd:	test   %esi,%esi
+    646c41cf:	mov    (%r8,%r11,1),%rdi
+    646c41d3:	jg     646c42d0 <lu_decomposition+0x1a0>
+    646c41d9:	xor    %r10d,%r10d
+    646c41dc:	movslq %r10d,%r10
+    646c41df:	mov    %r14d,%r15d
+    646c41e2:	lea    0x0(,%r10,8),%rbp
+    646c41ea:	cmp    %r10d,%esi
+    646c41ed:	je     646c4280 <lu_decomposition+0x150>
+    646c41f3:	mov    (%rdx,%r11,1),%r13
+    646c41f7:	test   %esi,%esi
+    646c41f9:	mov    (%rcx,%r11,1),%rax
+    646c41fd:	lea    0x0(%r13,%r11,1),%r12
+    646c4202:	movsd  (%rax,%r10,8),%xmm1
+    646c4208:	divsd  (%r12),%xmm1
+    646c420e:	movsd  %xmm1,(%rdi,%r10,8)
+    646c4214:	jle    646c424c <lu_decomposition+0x11c>
+    646c4216:	xor    %eax,%eax
+    646c4218:	jmp    646c4223 <lu_decomposition+0xf3>
+    646c421a:	nopw   0x0(%rax,%rax,1)
+    646c4220:	mov    %rbx,%rax
+    646c4223:	mov    (%r8,%rax,8),%rbx
+    646c4227:	cmp    %rax,%r15
+    646c422a:	movsd  (%rbx,%rbp,1),%xmm0
+    646c422f:	lea    0x1(%rax),%rbx
+    646c4233:	mulsd  0x0(%r13,%rax,8),%xmm0
+    646c423a:	divsd  (%r12),%xmm0
+    646c4240:	subsd  %xmm0,%xmm1
+    646c4244:	movsd  %xmm1,(%rdi,%r10,8)
+    646c424a:	jne    646c4220 <lu_decomposition+0xf0>
+    646c424c:	add    $0x1,%r10
+    646c4250:	cmp    %r10d,%r9d
+    646c4253:	jg     646c41e2 <lu_decomposition+0xb2>
+    646c4255:	add    $0x1,%esi
+    646c4258:	add    $0x8,%r11
+    646c425c:	add    $0x1,%r14d
+    646c4260:	cmp    %esi,%r9d
+    646c4263:	jne    646c4170 <lu_decomposition+0x40>
+    646c4269:	pop    %rbx
+    646c426a:	pop    %rsi
+    646c426b:	pop    %rdi
+    646c426c:	pop    %rbp
+    646c426d:	pop    %r12
+    646c426f:	pop    %r13
+    646c4271:	pop    %r14
+    646c4273:	pop    %r15
+    646c4275:	ret
+    646c4276:	cs nopw 0x0(%rax,%rax,1)
+    646c4280:	movsd  %xmm4,(%rdi,%r10,8)
+    646c4286:	add    $0x1,%r10
+    646c428a:	cmp    %r10d,%r9d
+    646c428d:	jg     646c41e2 <lu_decomposition+0xb2>
+    646c4293:	jmp    646c4255 <lu_decomposition+0x125>
+    646c4295:	cmp    %esi,%r9d
+    646c4298:	mov    %esi,%edi
+    646c429a:	mov    %rdx,%rax
+    646c429d:	cmovle %r9d,%edi
+    646c42a1:	xor    %r10d,%r10d
+    646c42a4:	mov    (%rax),%rbx
+    646c42a7:	add    $0x1,%r10d
+    646c42ab:	add    $0x8,%rax
+    646c42af:	cmp    %edi,%r10d
+    646c42b2:	movq   $0x0,(%rbx,%r11,1)
+    646c42ba:	jl     646c42a4 <lu_decomposition+0x174>
+    646c42bc:	cmp    %r10d,%r9d
+    646c42bf:	jg     646c417b <lu_decomposition+0x4b>
+    646c42c5:	mov    (%r8,%r11,1),%rdi
+    646c42c9:	nopl   0x0(%rax)
+    646c42d0:	cmp    %esi,%r9d
+    646c42d3:	mov    %esi,%ebx
+    646c42d5:	mov    $0x1,%ebp
+    646c42da:	cmovle %r9d,%ebx
+    646c42de:	test   %ebx,%ebx
+    646c42e0:	cmovg  %ebx,%ebp
+    646c42e3:	cmp    $0x4,%ebx
+    646c42e6:	jle    646c43b5 <lu_decomposition+0x285>
+    646c42ec:	mov    %ebp,%r10d
+    646c42ef:	mov    %rdi,%rax
+    646c42f2:	movdqa %xmm5,%xmm1
+    646c42f6:	shr    $0x2,%r10d
+    646c42fa:	shl    $0x5,%r10
+    646c42fe:	add    %rdi,%r10
+    646c4301:	movq   $0x0,(%rax)
+    646c4308:	add    $0x20,%rax
+    646c430c:	movdqa %xmm1,%xmm0
+    646c4310:	paddd  %xmm3,%xmm1
+    646c4314:	movq   $0x0,-0x18(%rax)
+    646c431c:	paddd  %xmm2,%xmm0
+    646c4320:	movq   $0x0,-0x10(%rax)
+    646c4328:	movq   $0x0,-0x8(%rax)
+    646c4330:	cmp    %rax,%r10
+    646c4333:	jne    646c4301 <lu_decomposition+0x1d1>
+    646c4335:	mov    %ebp,%eax
+    646c4337:	pshufd $0xff,%xmm0,%xmm0
+    646c433c:	movd   %xmm0,%r10d
+    646c4341:	and    $0xfffffffc,%eax
+    646c4344:	cmp    %ebp,%eax
+    646c4346:	je     646c4393 <lu_decomposition+0x263>
+    646c4348:	movslq %eax,%r10
+    646c434b:	movq   $0x0,(%rdi,%r10,8)
+    646c4353:	lea    0x1(%rax),%r10d
+    646c4357:	cmp    %ebx,%r10d
+    646c435a:	jge    646c4393 <lu_decomposition+0x263>
+    646c435c:	movslq %r10d,%r10
+    646c435f:	movq   $0x0,(%rdi,%r10,8)
+    646c4367:	lea    0x2(%rax),%r10d
+    646c436b:	cmp    %ebx,%r10d
+    646c436e:	jge    646c4393 <lu_decomposition+0x263>
+    646c4370:	movslq %r10d,%r10
+    646c4373:	movq   $0x0,(%rdi,%r10,8)
+    646c437b:	lea    0x3(%rax),%r10d
+    646c437f:	cmp    %ebx,%r10d
+    646c4382:	jge    646c4393 <lu_decomposition+0x263>
+    646c4384:	movslq %r10d,%r10
+    646c4387:	movq   $0x0,(%rdi,%r10,8)
+    646c438f:	lea    0x4(%rax),%r10d
+    646c4393:	cmp    %r9d,%r10d
+    646c4396:	jl     646c41dc <lu_decomposition+0xac>
+    646c439c:	add    $0x1,%esi
+    646c439f:	add    $0x8,%r11
+    646c43a3:	add    $0x1,%r14d
+    646c43a7:	cmp    %esi,%r9d
+    646c43aa:	jne    646c4170 <lu_decomposition+0x40>
+    646c43b0:	jmp    646c4269 <lu_decomposition+0x139>
+    646c43b5:	xor    %eax,%eax
+    646c43b7:	jmp    646c4348 <lu_decomposition+0x218>
+    646c43b9:	nopl   0x0(%rax)
+
+00000000646c43c0 <lu_inverse_solver>:
+    646c43c0:	push   %r15
+    646c43c2:	push   %r14
+    646c43c4:	push   %r13
+    646c43c6:	push   %r12
+    646c43c8:	push   %rbp
+    646c43c9:	push   %rdi
+    646c43ca:	push   %rsi
+    646c43cb:	push   %rbx
+    646c43cc:	sub    $0x38,%rsp
+    646c43d0:	lea    0x1(%r9),%ebp
+    646c43d4:	mov    %rcx,0x28(%rsp)
+    646c43d9:	mov    %rdx,%r13
+    646c43dc:	mov    %r8,%r14
+    646c43df:	movslq %ebp,%rax
+    646c43e2:	mov    %r9d,%ebx
+    646c43e5:	lea    0x0(,%rax,8),%rsi
+    646c43ed:	mov    %rax,0x20(%rsp)
+    646c43f2:	mov    %rsi,%rcx
+    646c43f5:	call   646c78b0 <malloc>
+    646c43fa:	test   %ebp,%ebp
+    646c43fc:	mov    %rax,%rdi
+    646c43ff:	jle    646c45e1 <lu_inverse_solver+0x221>
+    646c4405:	mov    %rax,%r15
+    646c4408:	mov    %ebx,%eax
+    646c440a:	lea    0x8(,%rax,8),%r12
+    646c4412:	lea    (%r12,%rdi,1),%rbp
+    646c4416:	cs nopw 0x0(%rax,%rax,1)
+    646c4420:	mov    %rsi,%rcx
+    646c4423:	add    $0x8,%r15
+    646c4427:	call   646c78b0 <malloc>
+    646c442c:	mov    %rax,-0x8(%r15)
+    646c4430:	cmp    %r15,%rbp
+    646c4433:	jne    646c4420 <lu_inverse_solver+0x60>
+    646c4435:	mov    %rsi,%rcx
+    646c4438:	call   646c78b0 <malloc>
+    646c443d:	mov    %rax,%rbp
+    646c4440:	mov    %rax,%r15
+    646c4443:	add    %rax,%r12
+    646c4446:	cs nopw 0x0(%rax,%rax,1)
+    646c4450:	mov    %rsi,%rcx
+    646c4453:	add    $0x8,%r15
+    646c4457:	call   646c78b0 <malloc>
+    646c445c:	mov    %rax,-0x8(%r15)
+    646c4460:	cmp    %r15,%r12
+    646c4463:	jne    646c4450 <lu_inverse_solver+0x90>
+    646c4465:	mov    0x20(%rsp),%rcx
+    646c446a:	lea    -0x8(%r14,%rsi,1),%r15
+    646c446f:	mov    $0x8,%edx
+    646c4474:	call   646c78f0 <calloc>
+    646c4479:	mov    0x28(%rsp),%rcx
+    646c447e:	mov    %ebx,%r9d
+    646c4481:	mov    %rbp,%r8
+    646c4484:	mov    %rdi,%rdx
+    646c4487:	mov    %rax,%r12
+    646c448a:	call   646c4130 <lu_decomposition>
+    646c448f:	mov    (%rdi),%rax
+    646c4492:	lea    -0x1(%rbx),%r10d
+    646c4496:	cmp    $0x1,%ebx
+    646c4499:	movsd  0x0(%r13),%xmm0
+    646c449f:	divsd  (%rax),%xmm0
+    646c44a3:	movsd  %xmm0,(%r12)
+    646c44a9:	jle    646c45f1 <lu_inverse_solver+0x231>
+    646c44af:	lea    -0x2(%rbx),%r11d
+    646c44b3:	mov    $0x1,%ecx
+    646c44b8:	lea    0x8(%r12),%rax
+    646c44bd:	add    $0x2,%r11
+    646c44c1:	mov    (%rdi,%rcx,8),%r8
+    646c44c5:	lea    0x0(,%rcx,8),%r9
+    646c44cd:	xor    %edx,%edx
+    646c44cf:	movsd  0x0(%r13,%rcx,8),%xmm1
+    646c44d6:	movsd  %xmm1,(%rax)
+    646c44da:	nopw   0x0(%rax,%rax,1)
+    646c44e0:	movsd  (%r8,%rdx,8),%xmm0
+    646c44e6:	mulsd  (%r12,%rdx,8),%xmm0
+    646c44ec:	add    $0x1,%rdx
+    646c44f0:	cmp    %rdx,%rcx
+    646c44f3:	subsd  %xmm0,%xmm1
+    646c44f7:	movsd  %xmm1,(%rax)
+    646c44fb:	jne    646c44e0 <lu_inverse_solver+0x120>
+    646c44fd:	add    $0x1,%rcx
+    646c4501:	divsd  (%r8,%r9,1),%xmm1
+    646c4507:	add    $0x8,%rax
+    646c450b:	movsd  %xmm1,-0x8(%rax)
+    646c4510:	cmp    %rcx,%r11
+    646c4513:	jne    646c44c1 <lu_inverse_solver+0x101>
+    646c4515:	movsd  -0x8(%r12,%rsi,1),%xmm0
+    646c451c:	movsd  %xmm0,(%r15)
+    646c4521:	lea    -0x10(%r14,%rsi,1),%rdx
+    646c4526:	movslq %r10d,%r8
+    646c4529:	nopl   0x0(%rax)
+    646c4530:	movsd  (%r12,%r8,8),%xmm1
+    646c4536:	lea    0x1(%r8),%eax
+    646c453a:	cmp    %eax,%ebx
+    646c453c:	movsd  %xmm1,(%rdx)
+    646c4540:	jle    646c456b <lu_inverse_solver+0x1ab>
+    646c4542:	mov    0x0(%rbp,%r8,8),%rcx
+    646c4547:	cltq
+    646c4549:	nopl   0x0(%rax)
+    646c4550:	movsd  (%rcx,%rax,8),%xmm0
+    646c4555:	mulsd  (%r14,%rax,8),%xmm0
+    646c455b:	add    $0x1,%rax
+    646c455f:	cmp    %eax,%ebx
+    646c4561:	subsd  %xmm0,%xmm1
+    646c4565:	movsd  %xmm1,(%rdx)
+    646c4569:	jg     646c4550 <lu_inverse_solver+0x190>
+    646c456b:	sub    $0x1,%r8
+    646c456f:	sub    $0x8,%rdx
+    646c4573:	test   %r8d,%r8d
+    646c4576:	jns    646c4530 <lu_inverse_solver+0x170>
+    646c4578:	cmpq   $0x0,0x20(%rsp)
+    646c457e:	lea    (%rsi,%rdi,1),%r13
+    646c4582:	mov    %rdi,%rbx
+    646c4585:	je     646c4619 <lu_inverse_solver+0x259>
+    646c458b:	nopl   0x0(%rax,%rax,1)
+    646c4590:	mov    (%rbx),%rcx
+    646c4593:	add    $0x8,%rbx
+    646c4597:	call   646c78c8 <free>
+    646c459c:	cmp    %rbx,%r13
+    646c459f:	jne    646c4590 <lu_inverse_solver+0x1d0>
+    646c45a1:	mov    %rdi,%rcx
+    646c45a4:	mov    %rbp,%rbx
+    646c45a7:	add    %rbp,%rsi
+    646c45aa:	call   646c78c8 <free>
+    646c45af:	nop
+    646c45b0:	mov    (%rbx),%rcx
+    646c45b3:	add    $0x8,%rbx
+    646c45b7:	call   646c78c8 <free>
+    646c45bc:	cmp    %rbx,%rsi
+    646c45bf:	jne    646c45b0 <lu_inverse_solver+0x1f0>
+    646c45c1:	mov    %rbp,%rcx
+    646c45c4:	call   646c78c8 <free>
+    646c45c9:	mov    %r12,%rcx
+    646c45cc:	add    $0x38,%rsp
+    646c45d0:	pop    %rbx
+    646c45d1:	pop    %rsi
+    646c45d2:	pop    %rdi
+    646c45d3:	pop    %rbp
+    646c45d4:	pop    %r12
+    646c45d6:	pop    %r13
+    646c45d8:	pop    %r14
+    646c45da:	pop    %r15
+    646c45dc:	jmp    646c78c8 <free>
+    646c45e1:	mov    %rsi,%rcx
+    646c45e4:	call   646c78b0 <malloc>
+    646c45e9:	mov    %rax,%rbp
+    646c45ec:	jmp    646c4465 <lu_inverse_solver+0xa5>
+    646c45f1:	movsd  -0x8(%r12,%rsi,1),%xmm0
+    646c45f8:	test   %r10d,%r10d
+    646c45fb:	movsd  %xmm0,(%r15)
+    646c4600:	jns    646c4521 <lu_inverse_solver+0x161>
+    646c4606:	cmpq   $0x0,0x20(%rsp)
+    646c460c:	lea    (%rsi,%rdi,1),%r13
+    646c4610:	mov    %rdi,%rbx
+    646c4613:	jne    646c4590 <lu_inverse_solver+0x1d0>
+    646c4619:	mov    %rdi,%rcx
+    646c461c:	call   646c78c8 <free>
+    646c4621:	jmp    646c45c1 <lu_inverse_solver+0x201>
+    646c4623:	nopl   (%rax)
+    646c4626:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c4630 <arange>:
+    646c4630:	push   %rbx
+    646c4631:	sub    $0x20,%rsp
+    646c4635:	movslq %ecx,%rcx
+    646c4638:	mov    %rcx,%rbx
+    646c463b:	shl    $0x2,%rcx
+    646c463f:	call   646c78b0 <malloc>
+    646c4644:	test   %ebx,%ebx
+    646c4646:	jle    646c46aa <arange+0x7a>
+    646c4648:	lea    -0x1(%rbx),%edx
+    646c464b:	cmp    $0x2,%edx
+    646c464e:	jbe    646c46b0 <arange+0x80>
+    646c4650:	mov    %ebx,%ecx
+    646c4652:	movdqa 0x4b36(%rip),%xmm0        # 646c9190 <.rdata+0x50>
+    646c465a:	mov    %rax,%rdx
+    646c465d:	shr    $0x2,%ecx
+    646c4660:	movdqa 0x4b38(%rip),%xmm1        # 646c91a0 <.rdata+0x60>
+    646c4668:	shl    $0x4,%rcx
+    646c466c:	add    %rax,%rcx
+    646c466f:	nop
+    646c4670:	movups %xmm0,(%rdx)
+    646c4673:	add    $0x10,%rdx
+    646c4677:	paddd  %xmm1,%xmm0
+    646c467b:	cmp    %rcx,%rdx
+    646c467e:	jne    646c4670 <arange+0x40>
+    646c4680:	mov    %ebx,%edx
+    646c4682:	and    $0xfffffffc,%edx
+    646c4685:	cmp    %edx,%ebx
+    646c4687:	je     646c46aa <arange+0x7a>
+    646c4689:	movslq %edx,%rcx
+    646c468c:	mov    %edx,(%rax,%rcx,4)
+    646c468f:	lea    0x1(%rdx),%ecx
+    646c4692:	cmp    %ecx,%ebx
+    646c4694:	jle    646c46aa <arange+0x7a>
+    646c4696:	add    $0x2,%edx
+    646c4699:	movslq %ecx,%r8
+    646c469c:	cmp    %edx,%ebx
+    646c469e:	mov    %ecx,(%rax,%r8,4)
+    646c46a2:	jle    646c46aa <arange+0x7a>
+    646c46a4:	movslq %edx,%rcx
+    646c46a7:	mov    %edx,(%rax,%rcx,4)
+    646c46aa:	add    $0x20,%rsp
+    646c46ae:	pop    %rbx
+    646c46af:	ret
+    646c46b0:	xor    %edx,%edx
+    646c46b2:	jmp    646c4689 <arange+0x59>
+    646c46b4:	xchg   %ax,%ax
+    646c46b6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c46c0 <d_arange>:
+    646c46c0:	push   %rbx
+    646c46c1:	sub    $0x20,%rsp
+    646c46c5:	movslq %ecx,%rcx
+    646c46c8:	mov    %rcx,%rbx
+    646c46cb:	shl    $0x3,%rcx
+    646c46cf:	call   646c78b0 <malloc>
+    646c46d4:	test   %ebx,%ebx
+    646c46d6:	jle    646c4786 <d_arange+0xc6>
+    646c46dc:	lea    -0x1(%rbx),%edx
+    646c46df:	cmp    $0x2,%edx
+    646c46e2:	jbe    646c478c <d_arange+0xcc>
+    646c46e8:	mov    %ebx,%ecx
+    646c46ea:	movdqa 0x4a9e(%rip),%xmm1        # 646c9190 <.rdata+0x50>
+    646c46f2:	mov    %rax,%rdx
+    646c46f5:	shr    $0x2,%ecx
+    646c46f8:	movdqa 0x4aa0(%rip),%xmm2        # 646c91a0 <.rdata+0x60>
+    646c4700:	shl    $0x5,%rcx
+    646c4704:	add    %rax,%rcx
+    646c4707:	nopw   0x0(%rax,%rax,1)
+    646c4710:	cvtdq2pd %xmm1,%xmm0
+    646c4714:	add    $0x20,%rdx
+    646c4718:	movlpd %xmm0,-0x20(%rdx)
+    646c471d:	movhpd %xmm0,-0x18(%rdx)
+    646c4722:	pshufd $0xee,%xmm1,%xmm0
+    646c4727:	cvtdq2pd %xmm0,%xmm0
+    646c472b:	paddd  %xmm2,%xmm1
+    646c472f:	movlpd %xmm0,-0x10(%rdx)
+    646c4734:	movhpd %xmm0,-0x8(%rdx)
+    646c4739:	cmp    %rcx,%rdx
+    646c473c:	jne    646c4710 <d_arange+0x50>
+    646c473e:	mov    %ebx,%edx
+    646c4740:	and    $0xfffffffc,%edx
+    646c4743:	cmp    %edx,%ebx
+    646c4745:	je     646c4786 <d_arange+0xc6>
+    646c4747:	pxor   %xmm0,%xmm0
+    646c474b:	cvtsi2sd %edx,%xmm0
+    646c474f:	movslq %edx,%rcx
+    646c4752:	movsd  %xmm0,(%rax,%rcx,8)
+    646c4757:	lea    0x1(%rdx),%ecx
+    646c475a:	cmp    %ecx,%ebx
+    646c475c:	jle    646c4786 <d_arange+0xc6>
+    646c475e:	pxor   %xmm0,%xmm0
+    646c4762:	cvtsi2sd %ecx,%xmm0
+    646c4766:	add    $0x2,%edx
+    646c4769:	movslq %ecx,%r8
+    646c476c:	cmp    %edx,%ebx
+    646c476e:	movsd  %xmm0,(%rax,%r8,8)
+    646c4774:	jle    646c4786 <d_arange+0xc6>
+    646c4776:	pxor   %xmm0,%xmm0
+    646c477a:	cvtsi2sd %edx,%xmm0
+    646c477e:	movslq %edx,%rcx
+    646c4781:	movsd  %xmm0,(%rax,%rcx,8)
+    646c4786:	add    $0x20,%rsp
+    646c478a:	pop    %rbx
+    646c478b:	ret
+    646c478c:	xor    %edx,%edx
+    646c478e:	jmp    646c4747 <d_arange+0x87>
+
+00000000646c4790 <pdist>:
+    646c4790:	push   %r15
+    646c4792:	push   %r14
+    646c4794:	push   %r13
+    646c4796:	push   %r12
+    646c4798:	push   %rbp
+    646c4799:	push   %rdi
+    646c479a:	push   %rsi
+    646c479b:	push   %rbx
+    646c479c:	sub    $0x28,%rsp
+    646c47a0:	test   %r8d,%r8d
+    646c47a3:	jle    646c4898 <pdist+0x108>
+    646c47a9:	lea    -0x1(%r8),%r13d
+    646c47ad:	mov    %r8d,%r10d
+    646c47b0:	movslq %r8d,%r14
+    646c47b3:	movq   0x4a15(%rip),%xmm4        # 646c91d0 <.rdata+0x90>
+    646c47bb:	lea    0x8(%rcx,%r13,8),%rax
+    646c47c0:	shr    %r10d
+    646c47c3:	movapd 0x4a15(%rip),%xmm2        # 646c91e0 <.rdata+0xa0>
+    646c47cb:	mov    %rdx,%rdi
+    646c47ce:	mov    %rax,0x8(%rsp)
+    646c47d3:	mov    %r8d,%eax
+    646c47d6:	mov    %rcx,%r9
+    646c47d9:	mov    %r13,%r15
+    646c47dc:	and    $0xfffffffe,%eax
+    646c47df:	shl    $0x3,%r14
+    646c47e3:	movapd %xmm4,%xmm3
+    646c47e7:	mov    %eax,%r11d
+    646c47ea:	mov    %eax,0x1c(%rsp)
+    646c47ee:	shl    $0x4,%r10
+    646c47f2:	lea    0x10(%rcx),%rax
+    646c47f6:	shl    $0x3,%r11
+    646c47fa:	lea    (%rcx,%r11,1),%rdx
+    646c47fe:	mov    %rax,0x10(%rsp)
+    646c4803:	mov    (%rdi),%rax
+    646c4806:	lea    0x8(%r9),%rbp
+    646c480a:	lea    0x10(%rax),%rbx
+    646c480e:	cmp    %rbx,%rcx
+    646c4811:	setae  %sil
+    646c4815:	cmp    0x10(%rsp),%rax
+    646c481a:	setae  %bl
+    646c481d:	or     %ebx,%esi
+    646c481f:	lea    (%rax,%r14,1),%rbx
+    646c4823:	cmp    %rbx,%r9
+    646c4826:	setae  %bl
+    646c4829:	cmp    %rbp,%rax
+    646c482c:	setae  %r12b
+    646c4830:	or     %r12d,%ebx
+    646c4833:	test   %bl,%sil
+    646c4836:	je     646c48b0 <pdist+0x120>
+    646c4838:	cmp    $0x2,%r15d
+    646c483c:	jbe    646c48b0 <pdist+0x120>
+    646c483e:	xor    %ebx,%ebx
+    646c4840:	movddup (%r9),%xmm1
+    646c4845:	movq   (%rcx,%rbx,1),%xmm0
+    646c484a:	movhpd 0x8(%rcx,%rbx,1),%xmm0
+    646c4850:	subpd  %xmm1,%xmm0
+    646c4854:	andpd  %xmm2,%xmm0
+    646c4858:	movlpd %xmm0,(%rax,%rbx,1)
+    646c485d:	movhpd %xmm0,0x8(%rax,%rbx,1)
+    646c4863:	add    $0x10,%rbx
+    646c4867:	cmp    %r10,%rbx
+    646c486a:	jne    646c4845 <pdist+0xb5>
+    646c486c:	cmp    %r8d,0x1c(%rsp)
+    646c4871:	je     646c4886 <pdist+0xf6>
+    646c4873:	movsd  (%rdx),%xmm0
+    646c4877:	subsd  (%r9),%xmm0
+    646c487c:	andpd  %xmm3,%xmm0
+    646c4880:	movsd  %xmm0,(%rax,%r11,1)
+    646c4886:	add    $0x8,%rdi
+    646c488a:	cmp    0x8(%rsp),%rbp
+    646c488f:	mov    %rbp,%r9
+    646c4892:	jne    646c4803 <pdist+0x73>
+    646c4898:	add    $0x28,%rsp
+    646c489c:	pop    %rbx
+    646c489d:	pop    %rsi
+    646c489e:	pop    %rdi
+    646c489f:	pop    %rbp
+    646c48a0:	pop    %r12
+    646c48a2:	pop    %r13
+    646c48a4:	pop    %r14
+    646c48a6:	pop    %r15
+    646c48a8:	ret
+    646c48a9:	nopl   0x0(%rax)
+    646c48b0:	xor    %ebx,%ebx
+    646c48b2:	jmp    646c48b7 <pdist+0x127>
+    646c48b4:	mov    %rsi,%rbx
+    646c48b7:	movsd  (%rcx,%rbx,8),%xmm0
+    646c48bc:	lea    0x1(%rbx),%rsi
+    646c48c0:	cmp    %r13,%rbx
+    646c48c3:	subsd  (%r9),%xmm0
+    646c48c8:	andpd  %xmm4,%xmm0
+    646c48cc:	movsd  %xmm0,(%rax,%rbx,8)
+    646c48d1:	jne    646c48b4 <pdist+0x124>
+    646c48d3:	jmp    646c4886 <pdist+0xf6>
+    646c48d5:	nop
+    646c48d6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c48e0 <matrixform>:
+    646c48e0:	push   %r14
+    646c48e2:	push   %r13
+    646c48e4:	push   %r12
+    646c48e6:	push   %rbp
+    646c48e7:	push   %rdi
+    646c48e8:	push   %rsi
+    646c48e9:	push   %rbx
+    646c48ea:	test   %r8d,%r8d
+    646c48ed:	jle    646c4998 <matrixform+0xb8>
+    646c48f3:	mov    %r8d,%r11d
+    646c48f6:	mov    %r8d,%ebp
+    646c48f9:	xor    %esi,%esi
+    646c48fb:	lea    -0x1(%r8),%edi
+    646c48ff:	shr    %r11d
+    646c4902:	and    $0xfffffffe,%ebp
+    646c4905:	mov    %rdi,%r12
+    646c4908:	shl    $0x4,%r11
+    646c490c:	mov    %ebp,%ebx
+    646c490e:	lea    0x8(%rdx,%rdi,8),%r13
+    646c4913:	mov    (%rdx),%r9
+    646c4916:	movslq %esi,%rax
+    646c4919:	lea    0x10(,%rax,8),%rax
+    646c4921:	lea    -0x10(%rcx,%rax,1),%r10
+    646c4926:	add    %rcx,%rax
+    646c4929:	cmp    %rax,%r9
+    646c492c:	lea    0x10(%r9),%rax
+    646c4930:	setae  %r14b
+    646c4934:	cmp    %rax,%r10
+    646c4937:	setae  %al
+    646c493a:	or     %al,%r14b
+    646c493d:	je     646c49a3 <matrixform+0xc3>
+    646c493f:	xor    %eax,%eax
+    646c4941:	cmp    $0x3,%r12d
+    646c4945:	jbe    646c49a3 <matrixform+0xc3>
+    646c4947:	nopw   0x0(%rax,%rax,1)
+    646c4950:	movq   (%r10,%rax,1),%xmm0
+    646c4956:	movhpd 0x8(%r10,%rax,1),%xmm0
+    646c495d:	movlpd %xmm0,(%r9,%rax,1)
+    646c4963:	movhpd %xmm0,0x8(%r9,%rax,1)
+    646c496a:	add    $0x10,%rax
+    646c496e:	cmp    %r11,%rax
+    646c4971:	jne    646c4950 <matrixform+0x70>
+    646c4973:	lea    (%rsi,%rbp,1),%eax
+    646c4976:	cmp    %r8d,%ebp
+    646c4979:	je     646c4988 <matrixform+0xa8>
+    646c497b:	cltq
+    646c497d:	movsd  (%rcx,%rax,8),%xmm0
+    646c4982:	movsd  %xmm0,(%r9,%rbx,8)
+    646c4988:	add    $0x8,%rdx
+    646c498c:	add    %r8d,%esi
+    646c498f:	cmp    %r13,%rdx
+    646c4992:	jne    646c4913 <matrixform+0x33>
+    646c4998:	pop    %rbx
+    646c4999:	pop    %rsi
+    646c499a:	pop    %rdi
+    646c499b:	pop    %rbp
+    646c499c:	pop    %r12
+    646c499e:	pop    %r13
+    646c49a0:	pop    %r14
+    646c49a2:	ret
+    646c49a3:	xor    %eax,%eax
+    646c49a5:	jmp    646c49b3 <matrixform+0xd3>
+    646c49a7:	nopw   0x0(%rax,%rax,1)
+    646c49b0:	mov    %r14,%rax
+    646c49b3:	movsd  (%r10,%rax,8),%xmm0
+    646c49b9:	lea    0x1(%rax),%r14
+    646c49bd:	cmp    %rdi,%rax
+    646c49c0:	movsd  %xmm0,(%r9,%rax,8)
+    646c49c6:	jne    646c49b0 <matrixform+0xd0>
+    646c49c8:	jmp    646c4988 <matrixform+0xa8>
+    646c49ca:	nopw   0x0(%rax,%rax,1)
+
+00000000646c49d0 <save_1darray>:
+    646c49d0:	push   %r13
+    646c49d2:	push   %r12
+    646c49d4:	push   %rbp
+    646c49d5:	push   %rdi
+    646c49d6:	push   %rsi
+    646c49d7:	push   %rbx
+    646c49d8:	sub    $0x1d8,%rsp
+    646c49df:	pxor   %xmm0,%xmm0
+    646c49e3:	mov    %rcx,%r12
+    646c49e6:	mov    %edx,%r13d
+    646c49e9:	mov    %r8,%rdi
+    646c49ec:	cvtsi2sdl 0x230(%rsp),%xmm0
+    646c49f5:	mov    %r9,%rbx
+    646c49f8:	call   646c78b8 <log10>
+    646c49fd:	movsd  0x47cb(%rip),%xmm3        # 646c91d0 <.rdata+0x90>
+    646c4a05:	movsd  0x47e3(%rip),%xmm4        # 646c91f0 <.rdata+0xb0>
+    646c4a0d:	movapd %xmm0,%xmm2
+    646c4a11:	movapd %xmm0,%xmm1
+    646c4a15:	andpd  %xmm3,%xmm2
+    646c4a19:	ucomisd %xmm2,%xmm4
+    646c4a1d:	jbe    646c4a4a <save_1darray+0x7a>
+    646c4a1f:	cvttsd2si %xmm0,%rax
+    646c4a24:	pxor   %xmm2,%xmm2
+    646c4a28:	movsd  0x4790(%rip),%xmm4        # 646c91c0 <.rdata+0x80>
+    646c4a30:	andnpd %xmm0,%xmm3
+    646c4a34:	cvtsi2sd %rax,%xmm2
+    646c4a39:	cmpnlesd %xmm2,%xmm1
+    646c4a3e:	andpd  %xmm4,%xmm1
+    646c4a42:	addsd  %xmm2,%xmm1
+    646c4a46:	orpd   %xmm3,%xmm1
+    646c4a4a:	cvttsd2si %xmm1,%eax
+    646c4a4e:	mov    %rbx,%r9
+    646c4a51:	mov    %rdi,0x20(%rsp)
+    646c4a56:	lea    0x30(%rsp),%rsi
+    646c4a5b:	mov    $0xc8,%edx
+    646c4a60:	lea    0x46d9(%rip),%r8        # 646c9140 <.rdata>
+    646c4a67:	mov    %rsi,%rcx
+    646c4a6a:	add    $0x1,%eax
+    646c4a6d:	mov    %eax,0x28(%rsp)
+    646c4a71:	call   646c4100 <snprintf.constprop.0>
+    646c4a76:	mov    %rbx,%rcx
+    646c4a79:	call   646c7908 <_mkdir>
+    646c4a7e:	cmp    $0xffffffff,%eax
+    646c4a81:	je     646c4b14 <save_1darray+0x144>
+    646c4a87:	mov    0x238(%rsp),%r9d
+    646c4a8f:	lea    0x100(%rsp),%rbx
+    646c4a97:	mov    %rsi,%r8
+    646c4a9a:	mov    $0xc8,%edx
+    646c4a9f:	mov    %rbx,%rcx
+    646c4aa2:	call   646c4100 <snprintf.constprop.0>
+    646c4aa7:	lea    0x46b7(%rip),%rdx        # 646c9165 <.rdata+0x25>
+    646c4aae:	mov    %rbx,%rcx
+    646c4ab1:	call   646c78d8 <fopen>
+    646c4ab6:	test   %rax,%rax
+    646c4ab9:	mov    %rax,%rsi
+    646c4abc:	je     646c4b34 <save_1darray+0x164>
+    646c4abe:	lea    -0x1(%r13),%ebp
+    646c4ac2:	xor    %ebx,%ebx
+    646c4ac4:	test   %r13d,%r13d
+    646c4ac7:	lea    0x46b1(%rip),%rdi        # 646c917f <.rdata+0x3f>
+    646c4ace:	jg     646c4ad5 <save_1darray+0x105>
+    646c4ad0:	jmp    646c4afb <save_1darray+0x12b>
+    646c4ad2:	mov    %rax,%rbx
+    646c4ad5:	movsd  (%r12,%rbx,8),%xmm0
+    646c4adb:	mov    %ebx,%r8d
+    646c4ade:	mov    %rdi,%rdx
+    646c4ae1:	mov    %rsi,%rcx
+    646c4ae4:	movapd %xmm0,%xmm3
+    646c4ae8:	movq   %xmm0,%r9
+    646c4aed:	call   646c78d0 <fprintf>
+    646c4af2:	lea    0x1(%rbx),%rax
+    646c4af6:	cmp    %rbp,%rbx
+    646c4af9:	jne    646c4ad2 <save_1darray+0x102>
+    646c4afb:	mov    %rsi,%rcx
+    646c4afe:	call   646c78e0 <fclose>
+    646c4b03:	nop
+    646c4b04:	add    $0x1d8,%rsp
+    646c4b0b:	pop    %rbx
+    646c4b0c:	pop    %rsi
+    646c4b0d:	pop    %rdi
+    646c4b0e:	pop    %rbp
+    646c4b0f:	pop    %r12
+    646c4b11:	pop    %r13
+    646c4b13:	ret
+    646c4b14:	call   *0x9782(%rip)        # 646ce29c <__imp__errno>
+    646c4b1a:	cmpl   $0x11,(%rax)
+    646c4b1d:	je     646c4a87 <save_1darray+0xb7>
+    646c4b23:	lea    0x4625(%rip),%rcx        # 646c914f <.rdata+0xf>
+    646c4b2a:	call   646c78a0 <printf>
+    646c4b2f:	jmp    646c4a87 <save_1darray+0xb7>
+    646c4b34:	lea    0x462c(%rip),%rcx        # 646c9167 <.rdata+0x27>
+    646c4b3b:	call   646c78a8 <perror>
+    646c4b40:	mov    $0x1,%ecx
+    646c4b45:	call   646c78e8 <exit>
+    646c4b4a:	nop
+    646c4b4b:	nop
+    646c4b4c:	nop
+    646c4b4d:	nop
+    646c4b4e:	nop
+    646c4b4f:	nop
+
+00000000646c4b50 <randompath>:
+    646c4b50:	push   %rdi
+    646c4b51:	push   %rsi
+    646c4b52:	push   %rbx
+    646c4b53:	sub    $0x20,%rsp
+    646c4b57:	sub    $0x1,%edx
+    646c4b5a:	mov    %rcx,%rdi
+    646c4b5d:	mov    %r8,%rsi
+    646c4b60:	je     646c4b8a <randompath+0x3a>
+    646c4b62:	movslq %edx,%rbx
+    646c4b65:	mov    %rsi,%rcx
+    646c4b68:	call   646c23e0 <mt19937_generate>
+    646c4b6d:	xor    %edx,%edx
+    646c4b6f:	mov    (%rdi,%rbx,4),%ecx
+    646c4b72:	div    %ebx
+    646c4b74:	movslq %edx,%rdx
+    646c4b77:	lea    (%rdi,%rdx,4),%rax
+    646c4b7b:	mov    (%rax),%edx
+    646c4b7d:	mov    %ecx,(%rax)
+    646c4b7f:	mov    %edx,(%rdi,%rbx,4)
+    646c4b82:	sub    $0x1,%rbx
+    646c4b86:	test   %ebx,%ebx
+    646c4b88:	jne    646c4b65 <randompath+0x15>
+    646c4b8a:	mov    %rdi,%rax
+    646c4b8d:	add    $0x20,%rsp
+    646c4b91:	pop    %rbx
+    646c4b92:	pop    %rsi
+    646c4b93:	pop    %rdi
+    646c4b94:	ret
+    646c4b95:	nop
+    646c4b96:	nop
+    646c4b97:	nop
+    646c4b98:	nop
+    646c4b99:	nop
+    646c4b9a:	nop
+    646c4b9b:	nop
+    646c4b9c:	nop
+    646c4b9d:	nop
+    646c4b9e:	nop
+    646c4b9f:	nop
+
+00000000646c4ba0 <set_sgsim_default>:
+    646c4ba0:	push   %rsi
+    646c4ba1:	push   %rbx
+    646c4ba2:	sub    $0x28,%rsp
+    646c4ba6:	mov    %rdx,%rsi
+    646c4ba9:	mov    %rcx,%rbx
+    646c4bac:	mov    %rdx,%rcx
+    646c4baf:	call   646c3420 <set_cov_model_default>
+    646c4bb4:	movsd  0x4694(%rip),%xmm1        # 646c9250 <.rdata+0x50>
+    646c4bbc:	movsd  0x18(%rsi),%xmm0
+    646c4bc1:	call   646c6ea0 <pow>
+    646c4bc6:	movsd  0x20(%rbx),%xmm1
+    646c4bcb:	movsd  0x468d(%rip),%xmm3        # 646c9260 <.rdata+0x60>
+    646c4bd3:	mulsd  0x467d(%rip),%xmm0        # 646c9258 <.rdata+0x58>
+    646c4bdb:	comisd %xmm1,%xmm3
+    646c4bdf:	jbe    646c4bed <set_sgsim_default+0x4d>
+    646c4be1:	movapd %xmm0,%xmm1
+    646c4be5:	xorpd  0x4683(%rip),%xmm1        # 646c9270 <.rdata+0x70>
+    646c4bed:	movsd  0x28(%rbx),%xmm2
+    646c4bf2:	movsd  %xmm1,0x20(%rbx)
+    646c4bf7:	cmpl   $0x1,0x10(%rbx)
+    646c4bfb:	movapd %xmm2,%xmm1
+    646c4bff:	cmpltsd %xmm3,%xmm1
+    646c4c04:	andpd  %xmm1,%xmm0
+    646c4c08:	andnpd %xmm2,%xmm1
+    646c4c0c:	orpd   %xmm1,%xmm0
+    646c4c10:	movsd  %xmm0,0x28(%rbx)
+    646c4c15:	je     646c4c20 <set_sgsim_default+0x80>
+    646c4c17:	add    $0x28,%rsp
+    646c4c1b:	pop    %rbx
+    646c4c1c:	pop    %rsi
+    646c4c1d:	ret
+    646c4c1e:	xchg   %ax,%ax
+    646c4c20:	mov    (%rbx),%ecx
+    646c4c22:	mov    $0x8,%edx
+    646c4c27:	imul   0x4(%rbx),%ecx
+    646c4c2b:	call   646c78f0 <calloc>
+    646c4c30:	mov    %rax,0x18(%rbx)
+    646c4c34:	add    $0x28,%rsp
+    646c4c38:	pop    %rbx
+    646c4c39:	pop    %rsi
+    646c4c3a:	ret
+    646c4c3b:	nopl   0x0(%rax,%rax,1)
+
+00000000646c4c40 <sgsim_run>:
+    646c4c40:	push   %r15
+    646c4c42:	push   %r14
+    646c4c44:	push   %r13
+    646c4c46:	push   %r12
+    646c4c48:	push   %rbp
+    646c4c49:	push   %rdi
+    646c4c4a:	push   %rsi
+    646c4c4b:	push   %rbx
+    646c4c4c:	sub    $0xa08,%rsp
+    646c4c53:	mov    %rdx,%r13
+    646c4c56:	mov    0x8(%rcx),%edx
+    646c4c59:	mov    %rcx,%r14
+    646c4c5c:	mov    %r8d,0xa60(%rsp)
+    646c4c64:	lea    0x30(%rsp),%rbp
+    646c4c69:	mov    %rbp,%rcx
+    646c4c6c:	call   646c23a0 <mt19937_init>
+    646c4c71:	mov    %r13,%rcx
+    646c4c74:	call   646c3420 <set_cov_model_default>
+    646c4c79:	movsd  0x45cf(%rip),%xmm1        # 646c9250 <.rdata+0x50>
+    646c4c81:	movsd  0x18(%r13),%xmm0
+    646c4c87:	call   646c6ea0 <pow>
+    646c4c8c:	movsd  0x20(%r14),%xmm1
+    646c4c92:	movsd  0x45c6(%rip),%xmm3        # 646c9260 <.rdata+0x60>
+    646c4c9a:	mulsd  0x45b6(%rip),%xmm0        # 646c9258 <.rdata+0x58>
+    646c4ca2:	comisd %xmm1,%xmm3
+    646c4ca6:	jbe    646c4cb4 <sgsim_run+0x74>
+    646c4ca8:	movapd %xmm0,%xmm1
+    646c4cac:	xorpd  0x45bc(%rip),%xmm1        # 646c9270 <.rdata+0x70>
+    646c4cb4:	movsd  0x28(%r14),%xmm2
+    646c4cba:	movsd  %xmm1,0x20(%r14)
+    646c4cc0:	cmpl   $0x1,0x10(%r14)
+    646c4cc5:	movapd %xmm2,%xmm1
+    646c4cc9:	mov    (%r14),%ebx
+    646c4ccc:	cmpltsd %xmm3,%xmm1
+    646c4cd1:	andpd  %xmm1,%xmm0
+    646c4cd5:	andnpd %xmm2,%xmm1
+    646c4cd9:	orpd   %xmm1,%xmm0
+    646c4cdd:	movsd  %xmm0,0x28(%r14)
+    646c4ce3:	je     646c4fac <sgsim_run+0x36c>
+    646c4ce9:	lea    0x7470(%rip),%rcx        # 646cc160 <_sampling>
+    646c4cf0:	mov    %ebx,%edx
+    646c4cf2:	call   646c3620 <sampling_state_init>
+    646c4cf7:	movslq 0x8(%r13),%rcx
+    646c4cfb:	mov    $0x8,%edx
+    646c4d00:	lea    0x7459(%rip),%rsi        # 646cc160 <_sampling>
+    646c4d07:	movq   %rcx,%xmm0
+    646c4d0c:	punpcklqdq %xmm0,%xmm0
+    646c4d10:	movups %xmm0,0x74c1(%rip)        # 646cc1d8 <variogram_array+0x8>
+    646c4d17:	call   646c78f0 <calloc>
+    646c4d1c:	movslq (%r14),%rcx
+    646c4d1f:	mov    $0x8,%edx
+    646c4d24:	mov    %rax,0x74a5(%rip)        # 646cc1d0 <variogram_array>
+    646c4d2b:	movq   %rcx,%xmm0
+    646c4d30:	mov    %rcx,%rbx
+    646c4d33:	punpcklqdq %xmm0,%xmm0
+    646c4d37:	movups %xmm0,0x747a(%rip)        # 646cc1b8 <sgsim_array+0x8>
+    646c4d3e:	call   646c78f0 <calloc>
+    646c4d43:	mov    %r13,%rdx
+    646c4d46:	mov    %ebx,%ecx
+    646c4d48:	mov    %rax,0x7461(%rip)        # 646cc1b0 <sgsim_array>
+    646c4d4f:	call   646c36a0 <kriging_param_setting>
+    646c4d54:	mov    (%r14),%ecx
+    646c4d57:	call   646c4630 <arange>
+    646c4d5c:	xor    %edx,%edx
+    646c4d5e:	movl   $0x0,0x73d8(%rip)        # 646cc140 <count>
+    646c4d68:	mov    %rax,0x7481(%rip)        # 646cc1f0 <x_grid>
+    646c4d6f:	nop
+    646c4d70:	cmp    %edx,0x4(%r14)
+    646c4d74:	jle    646c4f34 <sgsim_run+0x2f4>
+    646c4d7a:	lea    0x447f(%rip),%rcx        # 646c9200 <.rdata>
+    646c4d81:	call   646c78a0 <printf>
+    646c4d86:	mov    0x7463(%rip),%rcx        # 646cc1f0 <x_grid>
+    646c4d8d:	mov    %rbp,%r8
+    646c4d90:	movq   $0x0,0x73c5(%rip)        # 646cc160 <_sampling>
+    646c4d9b:	mov    (%r14),%edx
+    646c4d9e:	lea    0x744b(%rip),%r12        # 646cc1f0 <x_grid>
+    646c4da5:	movl   $0x0,0x7395(%rip)        # 646cc144 <flag>
+    646c4daf:	call   646c4b50 <randompath>
+    646c4db4:	mov    (%r14),%edx
+    646c4db7:	mov    %rax,0x7432(%rip)        # 646cc1f0 <x_grid>
+    646c4dbe:	test   %edx,%edx
+    646c4dc0:	jle    646c4f9b <sgsim_run+0x35b>
+    646c4dc6:	lea    0x73e3(%rip),%rdi        # 646cc1b0 <sgsim_array>
+    646c4dcd:	xor    %ebx,%ebx
+    646c4dcf:	jmp    646c4e76 <sgsim_run+0x236>
+    646c4dd4:	movsd  0x20(%r14),%xmm1
+    646c4dda:	comisd %xmm0,%xmm1
+    646c4dde:	jae    646c4ecd <sgsim_run+0x28d>
+    646c4de4:	mov    (%r14),%r11d
+    646c4de7:	mov    0x18(%r14),%r15
+    646c4deb:	mov    %r11d,%r8d
+    646c4dee:	imul   %edx,%r8d
+    646c4df2:	add    %ecx,%r8d
+    646c4df5:	movslq %r8d,%r8
+    646c4df8:	movsd  %xmm0,(%r15,%r8,8)
+    646c4dfe:	mov    (%rsi),%r8d
+    646c4e01:	cmp    0xc(%r13),%r8d
+    646c4e05:	jge    646c4e11 <sgsim_run+0x1d1>
+    646c4e07:	add    $0x1,%r8d
+    646c4e0b:	mov    %r8d,(%rsi)
+    646c4e0e:	mov    (%r9),%ecx
+    646c4e11:	pxor   %xmm0,%xmm0
+    646c4e15:	cvtsi2sd %ecx,%xmm0
+    646c4e19:	mov    0x7358(%rip),%rcx        # 646cc178 <_sampling+0x18>
+    646c4e20:	movsd  %xmm0,(%rcx,%rbx,8)
+    646c4e25:	addl   $0x1,0x7338(%rip)        # 646cc164 <_sampling+0x4>
+    646c4e2c:	movslq (%r9),%rcx
+    646c4e2f:	mov    (%r10,%rcx,8),%r8
+    646c4e33:	mov    %r8,%rcx
+    646c4e36:	shr    $0x20,%rcx
+    646c4e3a:	mov    %ecx,%r9d
+    646c4e3d:	and    $0x7fffffff,%r9d
+    646c4e44:	or     %r8d,%r9d
+    646c4e47:	sete   %r9b
+    646c4e4b:	and    $0x7ff00000,%ecx
+    646c4e51:	sete   %r8b
+    646c4e55:	or     %r8b,%r9b
+    646c4e58:	jne    646c4e69 <sgsim_run+0x229>
+    646c4e5a:	cmp    $0x7ff00000,%ecx
+    646c4e60:	jne    646c4e69 <sgsim_run+0x229>
+    646c4e62:	addl   $0x1,0x72db(%rip)        # 646cc144 <flag>
+    646c4e69:	add    $0x1,%rbx
+    646c4e6d:	cmp    %ebx,%r11d
+    646c4e70:	jle    646c4f90 <sgsim_run+0x350>
+    646c4e76:	pxor   %xmm1,%xmm1
+    646c4e7a:	cvtsi2sdl (%rax,%rbx,4),%xmm1
+    646c4e7f:	mov    %ebx,%r8d
+    646c4e82:	lea    0x0(,%rbx,4),%r15
+    646c4e8a:	mov    %rsi,%rcx
+    646c4e8d:	call   646c3690 <sampling_state_update>
+    646c4e92:	mov    0xc(%r14),%r9d
+    646c4e96:	mov    %rsi,%rdx
+    646c4e99:	mov    %rbp,%r8
+    646c4e9c:	mov    (%rdi),%rcx
+    646c4e9f:	call   646c3b30 <simple_kriging>
+    646c4ea4:	mov    (%r12),%rax
+    646c4ea8:	mov    (%rdi),%r10
+    646c4eab:	lea    (%rax,%r15,1),%r9
+    646c4eaf:	movslq (%r9),%rdx
+    646c4eb2:	movsd  (%r10,%rdx,8),%xmm0
+    646c4eb8:	mov    %rdx,%rcx
+    646c4ebb:	comisd 0x28(%r14),%xmm0
+    646c4ec1:	mov    0x7279(%rip),%edx        # 646cc140 <count>
+    646c4ec7:	jb     646c4dd4 <sgsim_run+0x194>
+    646c4ecd:	mov    0x7271(%rip),%eax        # 646cc144 <flag>
+    646c4ed3:	add    $0x1,%eax
+    646c4ed6:	mov    %eax,0x7268(%rip)        # 646cc144 <flag>
+    646c4edc:	test   %eax,%eax
+    646c4ede:	jne    646c4d70 <sgsim_run+0x130>
+    646c4ee4:	mov    0x4(%r14),%eax
+    646c4ee8:	mov    %edx,0x28(%rsp)
+    646c4eec:	lea    0x431a(%rip),%r9        # 646c920d <.rdata+0xd>
+    646c4ef3:	mov    (%r14),%edx
+    646c4ef6:	lea    0x4320(%rip),%r8        # 646c921d <.rdata+0x1d>
+    646c4efd:	mov    0x72ac(%rip),%rcx        # 646cc1b0 <sgsim_array>
+    646c4f04:	mov    %eax,0x20(%rsp)
+    646c4f08:	call   646c49d0 <save_1darray>
+    646c4f0d:	cmpl   $0x1,0xa60(%rsp)
+    646c4f15:	je     646c4fc6 <sgsim_run+0x386>
+    646c4f1b:	mov    0x721f(%rip),%eax        # 646cc140 <count>
+    646c4f21:	lea    0x1(%rax),%edx
+    646c4f24:	cmp    %edx,0x4(%r14)
+    646c4f28:	mov    %edx,0x7212(%rip)        # 646cc140 <count>
+    646c4f2e:	jg     646c4d7a <sgsim_run+0x13a>
+    646c4f34:	call   646c4010 <kriging_memory_free>
+    646c4f39:	mov    0x7238(%rip),%rcx        # 646cc178 <_sampling+0x18>
+    646c4f40:	call   646c78c8 <free>
+    646c4f45:	mov    0x7244(%rip),%rcx        # 646cc190 <_sampling+0x30>
+    646c4f4c:	call   646c78c8 <free>
+    646c4f51:	mov    0x7258(%rip),%rcx        # 646cc1b0 <sgsim_array>
+    646c4f58:	call   646c78c8 <free>
+    646c4f5d:	mov    0x728c(%rip),%rcx        # 646cc1f0 <x_grid>
+    646c4f64:	call   646c78c8 <free>
+    646c4f69:	mov    0x7260(%rip),%rcx        # 646cc1d0 <variogram_array>
+    646c4f70:	call   646c78c8 <free>
+    646c4f75:	nop
+    646c4f76:	add    $0xa08,%rsp
+    646c4f7d:	pop    %rbx
+    646c4f7e:	pop    %rsi
+    646c4f7f:	pop    %rdi
+    646c4f80:	pop    %rbp
+    646c4f81:	pop    %r12
+    646c4f83:	pop    %r13
+    646c4f85:	pop    %r14
+    646c4f87:	pop    %r15
+    646c4f89:	ret
+    646c4f8a:	nopw   0x0(%rax,%rax,1)
+    646c4f90:	mov    0x71ae(%rip),%eax        # 646cc144 <flag>
+    646c4f96:	jmp    646c4edc <sgsim_run+0x29c>
+    646c4f9b:	mov    0x71a3(%rip),%eax        # 646cc144 <flag>
+    646c4fa1:	mov    0x7199(%rip),%edx        # 646cc140 <count>
+    646c4fa7:	jmp    646c4edc <sgsim_run+0x29c>
+    646c4fac:	mov    %ebx,%ecx
+    646c4fae:	mov    $0x8,%edx
+    646c4fb3:	imul   0x4(%r14),%ecx
+    646c4fb8:	call   646c78f0 <calloc>
+    646c4fbd:	mov    %rax,0x18(%r14)
+    646c4fc1:	jmp    646c4ce9 <sgsim_run+0xa9>
+    646c4fc6:	mov    0x4(%r13),%eax
+    646c4fca:	mov    0x8(%r13),%r9d
+    646c4fce:	mov    (%r14),%r8d
+    646c4fd1:	mov    0x71f8(%rip),%rdx        # 646cc1d0 <variogram_array>
+    646c4fd8:	mov    0x71d1(%rip),%rcx        # 646cc1b0 <sgsim_array>
+    646c4fdf:	mov    %eax,0x20(%rsp)
+    646c4fe3:	call   646c5220 <variogram>
+    646c4fe8:	mov    0x8(%r13),%edx
+    646c4fec:	lea    0x4237(%rip),%r9        # 646c922a <.rdata+0x2a>
+    646c4ff3:	mov    0x7147(%rip),%eax        # 646cc140 <count>
+    646c4ff9:	lea    0x4244(%rip),%r8        # 646c9244 <.rdata+0x44>
+    646c5000:	mov    0x71c9(%rip),%rcx        # 646cc1d0 <variogram_array>
+    646c5007:	mov    %eax,0x28(%rsp)
+    646c500b:	mov    0x4(%r14),%eax
+    646c500f:	mov    %eax,0x20(%rsp)
+    646c5013:	call   646c49d0 <save_1darray>
+    646c5018:	jmp    646c4f1b <sgsim_run+0x2db>
+    646c501d:	nopl   (%rax)
+
+00000000646c5020 <sgsim_t_free>:
+    646c5020:	mov    0x18(%rcx),%rcx
+    646c5024:	jmp    646c78c8 <free>
+    646c5029:	nop
+    646c502a:	nop
+    646c502b:	nop
+    646c502c:	nop
+    646c502d:	nop
+    646c502e:	nop
     646c502f:	nop
-    646c5030:	mov    0xa58(%rsp),%rax
-    646c5038:	mov    0x71b1(%rip),%rdx        # 646cc1f0 <variogram_array>
-    646c503f:	mov    0x718a(%rip),%rcx        # 646cc1d0 <sgsim_array>
-    646c5046:	mov    0x4(%rax),%eax
-    646c5049:	mov    %eax,0x20(%rsp)
-    646c504d:	mov    0xa58(%rsp),%rax
-    646c5055:	mov    0x8(%rax),%r9d
-    646c5059:	call   646c52e0 <variogram>
-    646c505e:	mov    0x7100(%rip),%ecx        # 646cc164 <flag>
-    646c5064:	mov    0x70f6(%rip),%edx        # 646cc160 <count>
-    646c506a:	test   %ecx,%ecx
-    646c506c:	jne    646c4e31 <sgsim_run+0xc1>
-    646c5072:	mov    0x4(%rsi),%eax
-    646c5075:	mov    %edx,0x28(%rsp)
-    646c5079:	lea    0x419d(%rip),%r9        # 646c921d <.rdata+0xd>
-    646c5080:	mov    (%rsi),%edx
-    646c5082:	lea    0x41a4(%rip),%r8        # 646c922d <.rdata+0x1d>
-    646c5089:	mov    0x7140(%rip),%rcx        # 646cc1d0 <sgsim_array>
-    646c5090:	mov    %eax,0x20(%rsp)
-    646c5094:	call   646c4b40 <save_1darray>
-    646c5099:	mov    0xa58(%rsp),%rax
-    646c50a1:	lea    0x4192(%rip),%r9        # 646c923a <.rdata+0x2a>
-    646c50a8:	mov    0x7141(%rip),%rcx        # 646cc1f0 <variogram_array>
-    646c50af:	lea    0x419e(%rip),%r8        # 646c9254 <.rdata+0x44>
-    646c50b6:	mov    0x8(%rax),%edx
-    646c50b9:	mov    0x70a1(%rip),%eax        # 646cc160 <count>
-    646c50bf:	mov    %eax,0x28(%rsp)
-    646c50c3:	mov    0x4(%rsi),%eax
-    646c50c6:	mov    %eax,0x20(%rsp)
-    646c50ca:	call   646c4b40 <save_1darray>
-    646c50cf:	jmp    646c4fc1 <sgsim_run+0x251>
-    646c50d4:	xchg   %ax,%ax
-    646c50d6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c50e0 <sgsim_t_free>:
-    646c50e0:	mov    0x18(%rcx),%rcx
-    646c50e4:	jmp    646c7988 <free>
-    646c50e9:	nop
-    646c50ea:	nop
-    646c50eb:	nop
-    646c50ec:	nop
-    646c50ed:	nop
-    646c50ee:	nop
-    646c50ef:	nop
-
-00000000646c50f0 <swaprows>:
-    646c50f0:	movslq %edx,%rdx
-    646c50f3:	movslq %r8d,%r8
-    646c50f6:	lea    (%rcx,%r8,8),%r8
-    646c50fa:	lea    (%rcx,%rdx,8),%rax
-    646c50fe:	mov    (%r8),%r9
-    646c5101:	mov    (%rax),%rdx
-    646c5104:	mov    %rdx,(%r8)
-    646c5107:	mov    %r9,(%rax)
-    646c510a:	ret
-    646c510b:	nopl   0x0(%rax,%rax,1)
-
-00000000646c5110 <partition2d>:
-    646c5110:	movslq %edx,%r10
-    646c5113:	mov    (%rcx,%r10,8),%rax
-    646c5117:	movsd  0x10(%rax),%xmm1
-    646c511c:	lea    0x1(%r8),%eax
-    646c5120:	movapd %xmm1,%xmm0
-    646c5124:	comisd %xmm0,%xmm1
-    646c5128:	ja     646c515b <partition2d+0x4b>
-    646c512a:	movslq %eax,%rdx
-    646c512d:	lea    -0x8(%rcx,%rdx,8),%rdx
-    646c5132:	mov    (%rdx),%r8
-    646c5135:	sub    $0x1,%eax
-    646c5138:	mov    %rdx,%r9
-    646c513b:	sub    $0x8,%rdx
-    646c513f:	movsd  0x10(%r8),%xmm0
-    646c5145:	comisd %xmm1,%xmm0
-    646c5149:	ja     646c5132 <partition2d+0x22>
-    646c514b:	cmp    %r10d,%eax
-    646c514e:	jle    646c5170 <partition2d+0x60>
-    646c5150:	mov    (%rcx,%r10,8),%rdx
-    646c5154:	mov    %rdx,(%r9)
-    646c5157:	mov    %r8,(%rcx,%r10,8)
-    646c515b:	mov    0x8(%rcx,%r10,8),%rdx
-    646c5160:	add    $0x1,%r10
-    646c5164:	movsd  0x10(%rdx),%xmm0
-    646c5169:	jmp    646c5124 <partition2d+0x14>
-    646c516b:	nopl   0x0(%rax,%rax,1)
-    646c5170:	ret
-    646c5171:	nopl   0x0(%rax,%rax,1)
-    646c5176:	cs nopw 0x0(%rax,%rax,1)
 
-00000000646c5180 <quicksort2d>:
-    646c5180:	push   %rbp
-    646c5181:	push   %rdi
-    646c5182:	push   %rsi
-    646c5183:	push   %rbx
-    646c5184:	sub    $0x28,%rsp
-    646c5188:	cmp    %r8d,%edx
-    646c518b:	mov    %rcx,%rbx
-    646c518e:	mov    %r8d,%esi
-    646c5191:	jge    646c520e <quicksort2d+0x8e>
-    646c5193:	lea    0x1(%r8),%edi
-    646c5197:	movslq %edx,%rax
-    646c519a:	mov    %edi,%r8d
-    646c519d:	mov    (%rbx,%rax,8),%rcx
-    646c51a1:	movsd  0x10(%rcx),%xmm0
-    646c51a6:	movapd %xmm0,%xmm1
-    646c51aa:	nopw   0x0(%rax,%rax,1)
-    646c51b0:	comisd %xmm1,%xmm0
-    646c51b4:	ja     646c51f0 <quicksort2d+0x70>
-    646c51b6:	movslq %r8d,%rcx
-    646c51b9:	mov    %r8d,%ebp
-    646c51bc:	lea    -0x8(%rbx,%rcx,8),%rcx
-    646c51c1:	jmp    646c51c6 <quicksort2d+0x46>
-    646c51c3:	mov    %r8d,%ebp
-    646c51c6:	mov    (%rcx),%r9
-    646c51c9:	sub    $0x1,%r8d
-    646c51cd:	mov    %rcx,%r10
-    646c51d0:	sub    $0x8,%rcx
-    646c51d4:	movsd  0x10(%r9),%xmm1
-    646c51da:	comisd %xmm0,%xmm1
-    646c51de:	ja     646c51c3 <quicksort2d+0x43>
-    646c51e0:	cmp    %eax,%r8d
-    646c51e3:	jle    646c5200 <quicksort2d+0x80>
-    646c51e5:	mov    (%rbx,%rax,8),%rcx
-    646c51e9:	mov    %rcx,(%r10)
-    646c51ec:	mov    %r9,(%rbx,%rax,8)
-    646c51f0:	mov    0x8(%rbx,%rax,8),%rcx
-    646c51f5:	add    $0x1,%rax
-    646c51f9:	movsd  0x10(%rcx),%xmm1
-    646c51fe:	jmp    646c51b0 <quicksort2d+0x30>
-    646c5200:	mov    %rbx,%rcx
-    646c5203:	call   646c5180 <quicksort2d>
-    646c5208:	cmp    %ebp,%esi
-    646c520a:	mov    %ebp,%edx
-    646c520c:	jg     646c5197 <quicksort2d+0x17>
-    646c520e:	add    $0x28,%rsp
-    646c5212:	pop    %rbx
-    646c5213:	pop    %rsi
-    646c5214:	pop    %rdi
-    646c5215:	pop    %rbp
+00000000646c5030 <swaprows>:
+    646c5030:	movslq %edx,%rdx
+    646c5033:	movslq %r8d,%r8
+    646c5036:	lea    (%rcx,%r8,8),%r8
+    646c503a:	lea    (%rcx,%rdx,8),%rax
+    646c503e:	mov    (%r8),%r9
+    646c5041:	mov    (%rax),%rdx
+    646c5044:	mov    %rdx,(%r8)
+    646c5047:	mov    %r9,(%rax)
+    646c504a:	ret
+    646c504b:	nopl   0x0(%rax,%rax,1)
+
+00000000646c5050 <partition2d>:
+    646c5050:	movslq %edx,%r10
+    646c5053:	mov    (%rcx,%r10,8),%rax
+    646c5057:	movsd  0x10(%rax),%xmm1
+    646c505c:	lea    0x1(%r8),%eax
+    646c5060:	movapd %xmm1,%xmm0
+    646c5064:	comisd %xmm0,%xmm1
+    646c5068:	ja     646c509b <partition2d+0x4b>
+    646c506a:	movslq %eax,%rdx
+    646c506d:	lea    -0x8(%rcx,%rdx,8),%rdx
+    646c5072:	mov    (%rdx),%r8
+    646c5075:	sub    $0x1,%eax
+    646c5078:	mov    %rdx,%r9
+    646c507b:	sub    $0x8,%rdx
+    646c507f:	movsd  0x10(%r8),%xmm0
+    646c5085:	comisd %xmm1,%xmm0
+    646c5089:	ja     646c5072 <partition2d+0x22>
+    646c508b:	cmp    %r10d,%eax
+    646c508e:	jle    646c50b0 <partition2d+0x60>
+    646c5090:	mov    (%rcx,%r10,8),%rdx
+    646c5094:	mov    %rdx,(%r9)
+    646c5097:	mov    %r8,(%rcx,%r10,8)
+    646c509b:	mov    0x8(%rcx,%r10,8),%rdx
+    646c50a0:	add    $0x1,%r10
+    646c50a4:	movsd  0x10(%rdx),%xmm0
+    646c50a9:	jmp    646c5064 <partition2d+0x14>
+    646c50ab:	nopl   0x0(%rax,%rax,1)
+    646c50b0:	ret
+    646c50b1:	nopl   0x0(%rax,%rax,1)
+    646c50b6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c50c0 <quicksort2d>:
+    646c50c0:	push   %rbp
+    646c50c1:	push   %rdi
+    646c50c2:	push   %rsi
+    646c50c3:	push   %rbx
+    646c50c4:	sub    $0x28,%rsp
+    646c50c8:	cmp    %r8d,%edx
+    646c50cb:	mov    %rcx,%rbx
+    646c50ce:	mov    %r8d,%esi
+    646c50d1:	jge    646c514e <quicksort2d+0x8e>
+    646c50d3:	lea    0x1(%r8),%edi
+    646c50d7:	movslq %edx,%rax
+    646c50da:	mov    %edi,%r8d
+    646c50dd:	mov    (%rbx,%rax,8),%rcx
+    646c50e1:	movsd  0x10(%rcx),%xmm0
+    646c50e6:	movapd %xmm0,%xmm1
+    646c50ea:	nopw   0x0(%rax,%rax,1)
+    646c50f0:	comisd %xmm1,%xmm0
+    646c50f4:	ja     646c5130 <quicksort2d+0x70>
+    646c50f6:	movslq %r8d,%rcx
+    646c50f9:	mov    %r8d,%ebp
+    646c50fc:	lea    -0x8(%rbx,%rcx,8),%rcx
+    646c5101:	jmp    646c5106 <quicksort2d+0x46>
+    646c5103:	mov    %r8d,%ebp
+    646c5106:	mov    (%rcx),%r9
+    646c5109:	sub    $0x1,%r8d
+    646c510d:	mov    %rcx,%r10
+    646c5110:	sub    $0x8,%rcx
+    646c5114:	movsd  0x10(%r9),%xmm1
+    646c511a:	comisd %xmm0,%xmm1
+    646c511e:	ja     646c5103 <quicksort2d+0x43>
+    646c5120:	cmp    %eax,%r8d
+    646c5123:	jle    646c5140 <quicksort2d+0x80>
+    646c5125:	mov    (%rbx,%rax,8),%rcx
+    646c5129:	mov    %rcx,(%r10)
+    646c512c:	mov    %r9,(%rbx,%rax,8)
+    646c5130:	mov    0x8(%rbx,%rax,8),%rcx
+    646c5135:	add    $0x1,%rax
+    646c5139:	movsd  0x10(%rcx),%xmm1
+    646c513e:	jmp    646c50f0 <quicksort2d+0x30>
+    646c5140:	mov    %rbx,%rcx
+    646c5143:	call   646c50c0 <quicksort2d>
+    646c5148:	cmp    %ebp,%esi
+    646c514a:	mov    %ebp,%edx
+    646c514c:	jg     646c50d7 <quicksort2d+0x17>
+    646c514e:	add    $0x28,%rsp
+    646c5152:	pop    %rbx
+    646c5153:	pop    %rsi
+    646c5154:	pop    %rdi
+    646c5155:	pop    %rbp
+    646c5156:	ret
+    646c5157:	nopw   0x0(%rax,%rax,1)
+
+00000000646c5160 <quickselect2d>:
+    646c5160:	push   %r12
+    646c5162:	push   %rbp
+    646c5163:	push   %rdi
+    646c5164:	push   %rsi
+    646c5165:	push   %rbx
+    646c5166:	lea    0x1(%r8),%r12d
+    646c516a:	cmp    %r8d,%edx
+    646c516d:	movslq %edx,%rdi
+    646c5170:	jge    646c5210 <quickselect2d+0xb0>
+    646c5176:	cs nopw 0x0(%rax,%rax,1)
+    646c5180:	mov    (%rcx,%rdi,8),%rax
+    646c5184:	mov    %rdi,%r10
+    646c5187:	movsd  0x10(%rax),%xmm0
+    646c518c:	mov    %r12d,%eax
+    646c518f:	movapd %xmm0,%xmm1
+    646c5193:	comisd %xmm1,%xmm0
+    646c5197:	ja     646c51d0 <quickselect2d+0x70>
+    646c5199:	movslq %eax,%r11
+    646c519c:	mov    %eax,%ebx
+    646c519e:	lea    -0x8(%rcx,%r11,8),%r11
+    646c51a3:	jmp    646c51a7 <quickselect2d+0x47>
+    646c51a5:	mov    %eax,%ebx
+    646c51a7:	mov    (%r11),%rsi
+    646c51aa:	sub    $0x1,%eax
+    646c51ad:	mov    %r11,%rbp
+    646c51b0:	sub    $0x8,%r11
+    646c51b4:	movsd  0x10(%rsi),%xmm1
+    646c51b9:	comisd %xmm0,%xmm1
+    646c51bd:	ja     646c51a5 <quickselect2d+0x45>
+    646c51bf:	cmp    %r10d,%eax
+    646c51c2:	jle    646c51e1 <quickselect2d+0x81>
+    646c51c4:	mov    (%rcx,%r10,8),%r11
+    646c51c8:	mov    %r11,0x0(%rbp)
+    646c51cc:	mov    %rsi,(%rcx,%r10,8)
+    646c51d0:	mov    0x8(%rcx,%r10,8),%r11
+    646c51d5:	add    $0x1,%r10
+    646c51d9:	movsd  0x10(%r11),%xmm1
+    646c51df:	jmp    646c5193 <quickselect2d+0x33>
+    646c51e1:	cmp    %ebx,%r9d
+    646c51e4:	je     646c5210 <quickselect2d+0xb0>
+    646c51e6:	cmp    %eax,%r9d
+    646c51e9:	jle    646c5200 <quickselect2d+0xa0>
+    646c51eb:	cmp    %r8d,%ebx
+    646c51ee:	jge    646c5210 <quickselect2d+0xb0>
+    646c51f0:	movslq %ebx,%rdi
+    646c51f3:	mov    %rdi,%rdx
+    646c51f6:	jmp    646c5180 <quickselect2d+0x20>
+    646c51f8:	nopl   0x0(%rax,%rax,1)
+    646c5200:	cmp    %edx,%eax
+    646c5202:	jle    646c5210 <quickselect2d+0xb0>
+    646c5204:	lea    0x1(%rax),%r12d
+    646c5208:	mov    %eax,%r8d
+    646c520b:	jmp    646c5180 <quickselect2d+0x20>
+    646c5210:	pop    %rbx
+    646c5211:	pop    %rsi
+    646c5212:	pop    %rdi
+    646c5213:	pop    %rbp
+    646c5214:	pop    %r12
     646c5216:	ret
-    646c5217:	nopw   0x0(%rax,%rax,1)
-
-00000000646c5220 <quickselect2d>:
-    646c5220:	push   %r12
-    646c5222:	push   %rbp
-    646c5223:	push   %rdi
-    646c5224:	push   %rsi
-    646c5225:	push   %rbx
-    646c5226:	lea    0x1(%r8),%r12d
-    646c522a:	cmp    %r8d,%edx
-    646c522d:	movslq %edx,%rdi
-    646c5230:	jge    646c52d0 <quickselect2d+0xb0>
-    646c5236:	cs nopw 0x0(%rax,%rax,1)
-    646c5240:	mov    (%rcx,%rdi,8),%rax
-    646c5244:	mov    %rdi,%r10
-    646c5247:	movsd  0x10(%rax),%xmm0
-    646c524c:	mov    %r12d,%eax
-    646c524f:	movapd %xmm0,%xmm1
-    646c5253:	comisd %xmm1,%xmm0
-    646c5257:	ja     646c5290 <quickselect2d+0x70>
-    646c5259:	movslq %eax,%r11
-    646c525c:	mov    %eax,%ebx
-    646c525e:	lea    -0x8(%rcx,%r11,8),%r11
-    646c5263:	jmp    646c5267 <quickselect2d+0x47>
-    646c5265:	mov    %eax,%ebx
-    646c5267:	mov    (%r11),%rsi
-    646c526a:	sub    $0x1,%eax
-    646c526d:	mov    %r11,%rbp
-    646c5270:	sub    $0x8,%r11
-    646c5274:	movsd  0x10(%rsi),%xmm1
-    646c5279:	comisd %xmm0,%xmm1
-    646c527d:	ja     646c5265 <quickselect2d+0x45>
-    646c527f:	cmp    %r10d,%eax
-    646c5282:	jle    646c52a1 <quickselect2d+0x81>
-    646c5284:	mov    (%rcx,%r10,8),%r11
-    646c5288:	mov    %r11,0x0(%rbp)
-    646c528c:	mov    %rsi,(%rcx,%r10,8)
-    646c5290:	mov    0x8(%rcx,%r10,8),%r11
-    646c5295:	add    $0x1,%r10
-    646c5299:	movsd  0x10(%r11),%xmm1
-    646c529f:	jmp    646c5253 <quickselect2d+0x33>
-    646c52a1:	cmp    %ebx,%r9d
-    646c52a4:	je     646c52d0 <quickselect2d+0xb0>
-    646c52a6:	cmp    %eax,%r9d
-    646c52a9:	jle    646c52c0 <quickselect2d+0xa0>
-    646c52ab:	cmp    %r8d,%ebx
-    646c52ae:	jge    646c52d0 <quickselect2d+0xb0>
-    646c52b0:	movslq %ebx,%rdi
-    646c52b3:	mov    %rdi,%rdx
-    646c52b6:	jmp    646c5240 <quickselect2d+0x20>
-    646c52b8:	nopl   0x0(%rax,%rax,1)
-    646c52c0:	cmp    %edx,%eax
-    646c52c2:	jle    646c52d0 <quickselect2d+0xb0>
-    646c52c4:	lea    0x1(%rax),%r12d
-    646c52c8:	mov    %eax,%r8d
-    646c52cb:	jmp    646c5240 <quickselect2d+0x20>
-    646c52d0:	pop    %rbx
-    646c52d1:	pop    %rsi
-    646c52d2:	pop    %rdi
-    646c52d3:	pop    %rbp
-    646c52d4:	pop    %r12
-    646c52d6:	ret
-    646c52d7:	nop
-    646c52d8:	nop
-    646c52d9:	nop
-    646c52da:	nop
-    646c52db:	nop
-    646c52dc:	nop
-    646c52dd:	nop
-    646c52de:	nop
-    646c52df:	nop
-
-00000000646c52e0 <variogram>:
-    646c52e0:	push   %r15
-    646c52e2:	push   %r14
-    646c52e4:	push   %r13
-    646c52e6:	push   %r12
-    646c52e8:	push   %rbp
-    646c52e9:	push   %rdi
-    646c52ea:	push   %rsi
-    646c52eb:	push   %rbx
-    646c52ec:	sub    $0x68,%rsp
-    646c52f0:	movaps %xmm6,0x40(%rsp)
-    646c52f5:	movaps %xmm7,0x50(%rsp)
-    646c52fa:	mov    0xd0(%rsp),%edi
-    646c5301:	movslq %r8d,%rax
-    646c5304:	mov    %rcx,%r12
-    646c5307:	mov    %rdx,0x38(%rsp)
-    646c530c:	mov    %r9d,%ebp
-    646c530f:	lea    0x0(,%rax,8),%rsi
-    646c5317:	mov    %rax,%rbx
-    646c531a:	mov    %rax,0x28(%rsp)
-    646c531f:	mov    %rsi,%rcx
-    646c5322:	call   646c7970 <malloc>
-    646c5327:	test   %ebx,%ebx
-    646c5329:	mov    %rax,%r13
-    646c532c:	jle    646c5355 <variogram+0x75>
-    646c532e:	mov    %rax,%r14
-    646c5331:	lea    -0x1(%rbx),%eax
-    646c5334:	lea    0x8(%r13,%rax,8),%r15
-    646c5339:	nopl   0x0(%rax)
-    646c5340:	mov    %rsi,%rcx
-    646c5343:	add    $0x8,%r14
-    646c5347:	call   646c7970 <malloc>
-    646c534c:	mov    %rax,-0x8(%r14)
-    646c5350:	cmp    %r15,%r14
-    646c5353:	jne    646c5340 <variogram+0x60>
-    646c5355:	mov    %ebx,%ecx
-    646c5357:	call   646c4830 <d_arange>
-    646c535c:	mov    %ebx,%r8d
-    646c535f:	mov    %r13,%rdx
-    646c5362:	mov    %rax,%rcx
-    646c5365:	mov    %rax,0x30(%rsp)
-    646c536a:	call   646c4900 <pdist>
-    646c536f:	test   %ebp,%ebp
-    646c5371:	jle    646c5463 <variogram+0x183>
-    646c5377:	movslq %edi,%rax
-    646c537a:	mov    %edi,%r15d
-    646c537d:	mov    0x38(%rsp),%rdx
-    646c5382:	xor    %r14d,%r14d
-    646c5385:	lea    -0x2(%rbx),%r11d
-    646c5389:	shl    $0x3,%rax
-    646c538d:	mov    %rsi,0x38(%rsp)
-    646c5392:	neg    %r15d
-    646c5395:	movsd  0x3ec3(%rip),%xmm6        # 646c9260 <.rdata>
-    646c539d:	add    $0x2,%r11
-    646c53a1:	mov    %rax,%rsi
-    646c53a4:	movsd  0x3ebc(%rip),%xmm7        # 646c9268 <.rdata+0x8>
-    646c53ac:	nopl   0x0(%rax)
-    646c53b0:	add    %edi,%r14d
-    646c53b3:	test   %ebx,%ebx
-    646c53b5:	pxor   %xmm1,%xmm1
-    646c53b9:	pxor   %xmm4,%xmm4
-    646c53bd:	cvtsi2sd %r15d,%xmm1
-    646c53c2:	cvtsi2sd %r14d,%xmm4
-    646c53c7:	jle    646c544f <variogram+0x16f>
-    646c53cd:	cmp    $0x1,%ebx
-    646c53d0:	je     646c544f <variogram+0x16f>
-    646c53d2:	mov    $0x1,%r9d
-    646c53d8:	xor    %eax,%eax
-    646c53da:	pxor   %xmm2,%xmm2
-    646c53de:	pxor   %xmm3,%xmm3
-    646c53e2:	mov    0x0(%r13,%r9,8),%r8
-    646c53e7:	lea    0x8(,%rax,8),%rcx
-    646c53ef:	mov    %r9d,%r10d
-    646c53f2:	xor    %eax,%eax
-    646c53f4:	movsd  (%r12,%r9,8),%xmm5
-    646c53fa:	nopw   0x0(%rax,%rax,1)
-    646c5400:	movsd  (%r8,%rax,1),%xmm0
-    646c5406:	comisd %xmm1,%xmm0
-    646c540a:	jb     646c5428 <variogram+0x148>
-    646c540c:	comisd %xmm0,%xmm4
-    646c5410:	jb     646c5428 <variogram+0x148>
-    646c5412:	movapd %xmm5,%xmm0
-    646c5416:	subsd  (%r12,%rax,1),%xmm0
-    646c541c:	addsd  %xmm6,%xmm2
-    646c5420:	mulsd  %xmm0,%xmm0
-    646c5424:	addsd  %xmm0,%xmm3
-    646c5428:	add    $0x8,%rax
-    646c542c:	cmp    %rax,%rcx
-    646c542f:	jne    646c5400 <variogram+0x120>
-    646c5431:	add    $0x1,%r9
-    646c5435:	movslq %r10d,%rax
-    646c5438:	cmp    %r11,%r9
-    646c543b:	jne    646c53e2 <variogram+0x102>
-    646c543d:	comisd %xmm7,%xmm3
-    646c5441:	jb     646c544f <variogram+0x16f>
-    646c5443:	addsd  %xmm2,%xmm2
-    646c5447:	divsd  %xmm2,%xmm3
-    646c544b:	movsd  %xmm3,(%rdx)
-    646c544f:	add    %edi,%r15d
-    646c5452:	add    %rsi,%rdx
-    646c5455:	cmp    %ebp,%r14d
-    646c5458:	jl     646c53b0 <variogram+0xd0>
-    646c545e:	mov    0x38(%rsp),%rsi
-    646c5463:	mov    0x30(%rsp),%rcx
-    646c5468:	call   646c7988 <free>
-    646c546d:	cmpq   $0x0,0x28(%rsp)
-    646c5473:	je     646c5491 <variogram+0x1b1>
-    646c5475:	mov    %r13,%rbx
-    646c5478:	add    %r13,%rsi
-    646c547b:	nopl   0x0(%rax,%rax,1)
-    646c5480:	mov    (%rbx),%rcx
-    646c5483:	add    $0x8,%rbx
-    646c5487:	call   646c7988 <free>
-    646c548c:	cmp    %rbx,%rsi
-    646c548f:	jne    646c5480 <variogram+0x1a0>
-    646c5491:	movaps 0x40(%rsp),%xmm6
-    646c5496:	mov    %r13,%rcx
-    646c5499:	movaps 0x50(%rsp),%xmm7
-    646c549e:	add    $0x68,%rsp
-    646c54a2:	pop    %rbx
-    646c54a3:	pop    %rsi
-    646c54a4:	pop    %rdi
-    646c54a5:	pop    %rbp
-    646c54a6:	pop    %r12
-    646c54a8:	pop    %r13
-    646c54aa:	pop    %r14
-    646c54ac:	pop    %r15
-    646c54ae:	jmp    646c7988 <free>
-    646c54b3:	nopl   (%rax)
-    646c54b6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c54c0 <variance>:
-    646c54c0:	pxor   %xmm4,%xmm4
-    646c54c4:	cvtsi2sd %edx,%xmm4
-    646c54c8:	test   %edx,%edx
-    646c54ca:	jle    646c55b0 <variance+0xf0>
-    646c54d0:	cmp    $0x1,%edx
-    646c54d3:	je     646c55b9 <variance+0xf9>
-    646c54d9:	mov    %edx,%r8d
-    646c54dc:	mov    %rcx,%rax
-    646c54df:	pxor   %xmm0,%xmm0
-    646c54e3:	pxor   %xmm2,%xmm2
-    646c54e7:	shr    %r8d
-    646c54ea:	shl    $0x4,%r8
-    646c54ee:	add    %rcx,%r8
-    646c54f1:	movq   (%rax),%xmm1
-    646c54f5:	add    $0x10,%rax
-    646c54f9:	movhpd -0x8(%rax),%xmm1
-    646c54fe:	cmp    %r8,%rax
-    646c5501:	addsd  %xmm1,%xmm2
-    646c5505:	unpckhpd %xmm1,%xmm1
-    646c5509:	addsd  %xmm1,%xmm2
-    646c550d:	jne    646c54f1 <variance+0x31>
-    646c550f:	mov    %edx,%eax
-    646c5511:	and    $0xfffffffe,%eax
-    646c5514:	cmp    %eax,%edx
-    646c5516:	je     646c55a0 <variance+0xe0>
-    646c551c:	cltq
-    646c551e:	cmp    $0x1,%edx
-    646c5521:	addsd  (%rcx,%rax,8),%xmm2
-    646c5526:	divsd  %xmm4,%xmm2
-    646c552a:	je     646c5593 <variance+0xd3>
-    646c552c:	mov    %edx,%r8d
-    646c552f:	mov    %rcx,%rax
-    646c5532:	movddup %xmm2,%xmm5
-    646c5536:	shr    %r8d
-    646c5539:	shl    $0x4,%r8
-    646c553d:	add    %rcx,%r8
-    646c5540:	movq   (%rax),%xmm1
-    646c5544:	add    $0x10,%rax
-    646c5548:	movhpd -0x8(%rax),%xmm1
-    646c554d:	cmp    %rax,%r8
-    646c5550:	subpd  %xmm5,%xmm1
-    646c5554:	mulpd  %xmm1,%xmm1
-    646c5558:	movapd %xmm1,%xmm3
-    646c555c:	unpckhpd %xmm1,%xmm1
-    646c5560:	addsd  %xmm0,%xmm3
-    646c5564:	movapd %xmm1,%xmm0
-    646c5568:	addsd  %xmm3,%xmm0
-    646c556c:	jne    646c5540 <variance+0x80>
-    646c556e:	mov    %edx,%eax
-    646c5570:	and    $0xfffffffe,%eax
-    646c5573:	cmp    %edx,%eax
-    646c5575:	je     646c558e <variance+0xce>
-    646c5577:	cltq
-    646c5579:	movsd  (%rcx,%rax,8),%xmm3
-    646c557e:	subsd  %xmm2,%xmm3
-    646c5582:	movapd %xmm3,%xmm2
-    646c5586:	mulsd  %xmm3,%xmm2
-    646c558a:	addsd  %xmm2,%xmm0
-    646c558e:	divsd  %xmm4,%xmm0
-    646c5592:	ret
-    646c5593:	xor    %eax,%eax
-    646c5595:	jmp    646c5577 <variance+0xb7>
-    646c5597:	nopw   0x0(%rax,%rax,1)
-    646c55a0:	divsd  %xmm4,%xmm2
-    646c55a4:	jmp    646c552c <variance+0x6c>
-    646c55a6:	cs nopw 0x0(%rax,%rax,1)
-    646c55b0:	pxor   %xmm0,%xmm0
-    646c55b4:	divsd  %xmm4,%xmm0
-    646c55b8:	ret
-    646c55b9:	xor    %eax,%eax
-    646c55bb:	pxor   %xmm0,%xmm0
-    646c55bf:	pxor   %xmm2,%xmm2
-    646c55c3:	jmp    646c551c <variance+0x5c>
-    646c55c8:	nop
-    646c55c9:	nop
-    646c55ca:	nop
-    646c55cb:	nop
-    646c55cc:	nop
-    646c55cd:	nop
-    646c55ce:	nop
-    646c55cf:	nop
-
-00000000646c55d0 <Sleep>:
-    646c55d0:	jmp    *0x8c76(%rip)        # 646ce24c <__imp_Sleep>
-    646c55d6:	nop
-    646c55d7:	nop
-    646c55d8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c55e0 <__do_global_dtors>:
-    646c55e0:	sub    $0x28,%rsp
-    646c55e4:	mov    0x2a15(%rip),%rax        # 646c8000 <__data_start__>
-    646c55eb:	mov    (%rax),%rax
-    646c55ee:	test   %rax,%rax
-    646c55f1:	je     646c5610 <__do_global_dtors+0x30>
-    646c55f3:	call   *%rax
-    646c55f5:	mov    0x2a04(%rip),%rax        # 646c8000 <__data_start__>
-    646c55fc:	lea    0x8(%rax),%rdx
-    646c5600:	mov    0x8(%rax),%rax
-    646c5604:	mov    %rdx,0x29f5(%rip)        # 646c8000 <__data_start__>
-    646c560b:	test   %rax,%rax
-    646c560e:	jne    646c55f3 <__do_global_dtors+0x13>
-    646c5610:	add    $0x28,%rsp
-    646c5614:	ret
-    646c5615:	nop
-    646c5616:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5620 <__do_global_ctors>:
-    646c5620:	push   %rsi
-    646c5621:	push   %rbx
-    646c5622:	sub    $0x28,%rsp
-    646c5626:	mov    0x4093(%rip),%rcx        # 646c96c0 <.refptr.__CTOR_LIST__>
-    646c562d:	mov    (%rcx),%rdx
-    646c5630:	cmp    $0xffffffff,%edx
-    646c5633:	mov    %edx,%eax
-    646c5635:	je     646c5670 <__do_global_ctors+0x50>
-    646c5637:	test   %eax,%eax
-    646c5639:	je     646c565b <__do_global_ctors+0x3b>
-    646c563b:	mov    %eax,%edx
-    646c563d:	sub    $0x1,%eax
-    646c5640:	lea    (%rcx,%rdx,8),%rbx
-    646c5644:	sub    %rax,%rdx
-    646c5647:	lea    -0x8(%rcx,%rdx,8),%rsi
-    646c564c:	nopl   0x0(%rax)
-    646c5650:	call   *(%rbx)
-    646c5652:	sub    $0x8,%rbx
-    646c5656:	cmp    %rsi,%rbx
-    646c5659:	jne    646c5650 <__do_global_ctors+0x30>
-    646c565b:	lea    -0x82(%rip),%rcx        # 646c55e0 <__do_global_dtors>
-    646c5662:	add    $0x28,%rsp
-    646c5666:	pop    %rbx
-    646c5667:	pop    %rsi
-    646c5668:	jmp    646c1380 <atexit>
-    646c566d:	nopl   (%rax)
-    646c5670:	xor    %eax,%eax
-    646c5672:	jmp    646c5676 <__do_global_ctors+0x56>
-    646c5674:	mov    %edx,%eax
-    646c5676:	lea    0x1(%rax),%r8d
-    646c567a:	cmpq   $0x0,(%rcx,%r8,8)
-    646c567f:	mov    %r8,%rdx
-    646c5682:	jne    646c5674 <__do_global_ctors+0x54>
-    646c5684:	jmp    646c5637 <__do_global_ctors+0x17>
-    646c5686:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5690 <__main>:
-    646c5690:	mov    0x6baa(%rip),%eax        # 646cc240 <initialized>
-    646c5696:	test   %eax,%eax
-    646c5698:	je     646c56a0 <__main+0x10>
-    646c569a:	ret
-    646c569b:	nopl   0x0(%rax,%rax,1)
-    646c56a0:	movl   $0x1,0x6b96(%rip)        # 646cc240 <initialized>
-    646c56aa:	jmp    646c5620 <__do_global_ctors>
-    646c56af:	nop
-
-00000000646c56b0 <__security_init_cookie>:
-    646c56b0:	push   %r12
-    646c56b2:	push   %rbp
-    646c56b3:	push   %rdi
-    646c56b4:	push   %rsi
-    646c56b5:	push   %rbx
-    646c56b6:	sub    $0x30,%rsp
-    646c56ba:	mov    0x29bf(%rip),%rbx        # 646c8080 <__security_cookie>
-    646c56c1:	movabs $0x2b992ddfa232,%rax
-    646c56cb:	cmp    %rax,%rbx
-    646c56ce:	movq   $0x0,0x20(%rsp)
-    646c56d7:	je     646c56f0 <__security_init_cookie+0x40>
-    646c56d9:	not    %rbx
-    646c56dc:	mov    %rbx,0x29ad(%rip)        # 646c8090 <__security_cookie_complement>
-    646c56e3:	add    $0x30,%rsp
-    646c56e7:	pop    %rbx
-    646c56e8:	pop    %rsi
-    646c56e9:	pop    %rdi
-    646c56ea:	pop    %rbp
-    646c56eb:	pop    %r12
-    646c56ed:	ret
-    646c56ee:	xchg   %ax,%ax
-    646c56f0:	lea    0x20(%rsp),%rcx
-    646c56f5:	call   *0x8b01(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c56fb:	mov    0x20(%rsp),%rsi
-    646c5700:	call   *0x8ade(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c5706:	mov    %eax,%r12d
-    646c5709:	call   *0x8add(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c570f:	mov    %eax,%ebp
-    646c5711:	call   *0x8aed(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c5717:	lea    0x28(%rsp),%rcx
-    646c571c:	mov    %eax,%edi
-    646c571e:	call   *0x8af8(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c5724:	xor    0x28(%rsp),%rsi
-    646c5729:	mov    %r12d,%eax
-    646c572c:	movabs $0xffffffffffff,%rdx
-    646c5736:	xor    %rsi,%rax
-    646c5739:	mov    %ebp,%esi
-    646c573b:	xor    %rax,%rsi
-    646c573e:	mov    %edi,%eax
-    646c5740:	xor    %rsi,%rax
-    646c5743:	and    %rdx,%rax
-    646c5746:	cmp    %rbx,%rax
-    646c5749:	je     646c5770 <__security_init_cookie+0xc0>
-    646c574b:	mov    %rax,%rdx
-    646c574e:	not    %rdx
-    646c5751:	mov    %rax,0x2928(%rip)        # 646c8080 <__security_cookie>
-    646c5758:	mov    %rdx,0x2931(%rip)        # 646c8090 <__security_cookie_complement>
-    646c575f:	add    $0x30,%rsp
-    646c5763:	pop    %rbx
-    646c5764:	pop    %rsi
-    646c5765:	pop    %rdi
-    646c5766:	pop    %rbp
-    646c5767:	pop    %r12
-    646c5769:	ret
-    646c576a:	nopw   0x0(%rax,%rax,1)
-    646c5770:	movabs $0xffffd466d2205dcc,%rdx
-    646c577a:	movabs $0x2b992ddfa233,%rax
-    646c5784:	jmp    646c5751 <__security_init_cookie+0xa1>
-    646c5786:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5790 <__report_gsfailure>:
-    646c5790:	push   %rbp
-    646c5791:	push   %rsi
-    646c5792:	push   %rbx
-    646c5793:	mov    %rsp,%rbp
-    646c5796:	sub    $0x70,%rsp
-    646c579a:	mov    %rcx,%rsi
-    646c579d:	lea    0x6abc(%rip),%rcx        # 646cc260 <GS_ContextRecord>
-    646c57a4:	call   *0x8a82(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c57aa:	mov    0x6ba7(%rip),%rbx        # 646cc358 <GS_ContextRecord+0xf8>
-    646c57b1:	lea    -0x28(%rbp),%rdx
-    646c57b5:	xor    %r8d,%r8d
-    646c57b8:	mov    %rbx,%rcx
-    646c57bb:	call   *0x8a73(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c57c1:	test   %rax,%rax
-    646c57c4:	je     646c586d <__report_gsfailure+0xdd>
-    646c57ca:	lea    -0x20(%rbp),%rdx
-    646c57ce:	mov    %rax,%r9
-    646c57d1:	mov    %rbx,%r8
-    646c57d4:	movq   $0x0,0x38(%rsp)
-    646c57dd:	lea    0x6a7c(%rip),%rcx        # 646cc260 <GS_ContextRecord>
-    646c57e4:	mov    %rdx,0x30(%rsp)
-    646c57e9:	lea    -0x18(%rbp),%rdx
-    646c57ed:	mov    %rcx,0x20(%rsp)
-    646c57f2:	xor    %ecx,%ecx
-    646c57f4:	mov    %rdx,0x28(%rsp)
-    646c57f9:	mov    -0x28(%rbp),%rdx
-    646c57fd:	call   *0x8a39(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c5803:	mov    0x6b4e(%rip),%rax        # 646cc358 <GS_ContextRecord+0xf8>
-    646c580a:	xor    %ecx,%ecx
-    646c580c:	mov    %rsi,0x6acd(%rip)        # 646cc2e0 <GS_ContextRecord+0x80>
-    646c5813:	mov    %rax,0x6f36(%rip)        # 646cc750 <GS_ExceptionRecord+0x10>
-    646c581a:	movabs $0x1c0000409,%rax
-    646c5824:	mov    %rax,0x6f15(%rip)        # 646cc740 <GS_ExceptionRecord>
-    646c582b:	mov    0x284e(%rip),%rax        # 646c8080 <__security_cookie>
-    646c5832:	mov    %rax,-0x10(%rbp)
-    646c5836:	mov    0x2853(%rip),%rax        # 646c8090 <__security_cookie_complement>
-    646c583d:	mov    %rax,-0x8(%rbp)
-    646c5841:	call   *0x89fd(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c5847:	lea    0x3a22(%rip),%rcx        # 646c9270 <GS_ExceptionPointers>
-    646c584e:	call   *0x8a10(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c5854:	call   *0x8982(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c585a:	mov    $0xc0000409,%edx
-    646c585f:	mov    %rax,%rcx
-    646c5862:	call   *0x89ec(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c5868:	call   646c79b8 <abort>
-    646c586d:	mov    0x18(%rbp),%rax
-    646c5871:	mov    %rax,0x6ae0(%rip)        # 646cc358 <GS_ContextRecord+0xf8>
-    646c5878:	lea    0x8(%rbp),%rax
-    646c587c:	mov    %rax,0x6a75(%rip)        # 646cc2f8 <GS_ContextRecord+0x98>
-    646c5883:	jmp    646c5803 <__report_gsfailure+0x73>
+    646c5217:	nop
+    646c5218:	nop
+    646c5219:	nop
+    646c521a:	nop
+    646c521b:	nop
+    646c521c:	nop
+    646c521d:	nop
+    646c521e:	nop
+    646c521f:	nop
+
+00000000646c5220 <variogram>:
+    646c5220:	push   %r15
+    646c5222:	push   %r14
+    646c5224:	push   %r13
+    646c5226:	push   %r12
+    646c5228:	push   %rbp
+    646c5229:	push   %rdi
+    646c522a:	push   %rsi
+    646c522b:	push   %rbx
+    646c522c:	sub    $0x68,%rsp
+    646c5230:	movaps %xmm6,0x40(%rsp)
+    646c5235:	movaps %xmm7,0x50(%rsp)
+    646c523a:	mov    0xd0(%rsp),%edi
+    646c5241:	movslq %r8d,%rax
+    646c5244:	mov    %rcx,%r12
+    646c5247:	mov    %rdx,0x38(%rsp)
+    646c524c:	mov    %r9d,%ebp
+    646c524f:	lea    0x0(,%rax,8),%rsi
+    646c5257:	mov    %rax,%rbx
+    646c525a:	mov    %rax,0x28(%rsp)
+    646c525f:	mov    %rsi,%rcx
+    646c5262:	call   646c78b0 <malloc>
+    646c5267:	test   %ebx,%ebx
+    646c5269:	mov    %rax,%r13
+    646c526c:	jle    646c5295 <variogram+0x75>
+    646c526e:	mov    %rax,%r14
+    646c5271:	lea    -0x1(%rbx),%eax
+    646c5274:	lea    0x8(%r13,%rax,8),%r15
+    646c5279:	nopl   0x0(%rax)
+    646c5280:	mov    %rsi,%rcx
+    646c5283:	add    $0x8,%r14
+    646c5287:	call   646c78b0 <malloc>
+    646c528c:	mov    %rax,-0x8(%r14)
+    646c5290:	cmp    %r15,%r14
+    646c5293:	jne    646c5280 <variogram+0x60>
+    646c5295:	mov    %ebx,%ecx
+    646c5297:	call   646c46c0 <d_arange>
+    646c529c:	mov    %ebx,%r8d
+    646c529f:	mov    %r13,%rdx
+    646c52a2:	mov    %rax,%rcx
+    646c52a5:	mov    %rax,0x30(%rsp)
+    646c52aa:	call   646c4790 <pdist>
+    646c52af:	test   %ebp,%ebp
+    646c52b1:	jle    646c53a3 <variogram+0x183>
+    646c52b7:	movslq %edi,%rax
+    646c52ba:	mov    %edi,%r15d
+    646c52bd:	mov    0x38(%rsp),%rdx
+    646c52c2:	xor    %r14d,%r14d
+    646c52c5:	lea    -0x2(%rbx),%r11d
+    646c52c9:	shl    $0x3,%rax
+    646c52cd:	mov    %rsi,0x38(%rsp)
+    646c52d2:	neg    %r15d
+    646c52d5:	movsd  0x3fa3(%rip),%xmm6        # 646c9280 <.rdata>
+    646c52dd:	add    $0x2,%r11
+    646c52e1:	mov    %rax,%rsi
+    646c52e4:	movsd  0x3f9c(%rip),%xmm7        # 646c9288 <.rdata+0x8>
+    646c52ec:	nopl   0x0(%rax)
+    646c52f0:	add    %edi,%r14d
+    646c52f3:	test   %ebx,%ebx
+    646c52f5:	pxor   %xmm1,%xmm1
+    646c52f9:	pxor   %xmm4,%xmm4
+    646c52fd:	cvtsi2sd %r15d,%xmm1
+    646c5302:	cvtsi2sd %r14d,%xmm4
+    646c5307:	jle    646c538f <variogram+0x16f>
+    646c530d:	cmp    $0x1,%ebx
+    646c5310:	je     646c538f <variogram+0x16f>
+    646c5312:	mov    $0x1,%r9d
+    646c5318:	xor    %eax,%eax
+    646c531a:	pxor   %xmm2,%xmm2
+    646c531e:	pxor   %xmm3,%xmm3
+    646c5322:	mov    0x0(%r13,%r9,8),%r8
+    646c5327:	lea    0x8(,%rax,8),%rcx
+    646c532f:	mov    %r9d,%r10d
+    646c5332:	xor    %eax,%eax
+    646c5334:	movsd  (%r12,%r9,8),%xmm5
+    646c533a:	nopw   0x0(%rax,%rax,1)
+    646c5340:	movsd  (%r8,%rax,1),%xmm0
+    646c5346:	comisd %xmm1,%xmm0
+    646c534a:	jb     646c5368 <variogram+0x148>
+    646c534c:	comisd %xmm0,%xmm4
+    646c5350:	jb     646c5368 <variogram+0x148>
+    646c5352:	movapd %xmm5,%xmm0
+    646c5356:	subsd  (%r12,%rax,1),%xmm0
+    646c535c:	addsd  %xmm6,%xmm2
+    646c5360:	mulsd  %xmm0,%xmm0
+    646c5364:	addsd  %xmm0,%xmm3
+    646c5368:	add    $0x8,%rax
+    646c536c:	cmp    %rax,%rcx
+    646c536f:	jne    646c5340 <variogram+0x120>
+    646c5371:	add    $0x1,%r9
+    646c5375:	movslq %r10d,%rax
+    646c5378:	cmp    %r11,%r9
+    646c537b:	jne    646c5322 <variogram+0x102>
+    646c537d:	comisd %xmm7,%xmm3
+    646c5381:	jb     646c538f <variogram+0x16f>
+    646c5383:	addsd  %xmm2,%xmm2
+    646c5387:	divsd  %xmm2,%xmm3
+    646c538b:	movsd  %xmm3,(%rdx)
+    646c538f:	add    %edi,%r15d
+    646c5392:	add    %rsi,%rdx
+    646c5395:	cmp    %ebp,%r14d
+    646c5398:	jl     646c52f0 <variogram+0xd0>
+    646c539e:	mov    0x38(%rsp),%rsi
+    646c53a3:	mov    0x30(%rsp),%rcx
+    646c53a8:	call   646c78c8 <free>
+    646c53ad:	cmpq   $0x0,0x28(%rsp)
+    646c53b3:	je     646c53d1 <variogram+0x1b1>
+    646c53b5:	mov    %r13,%rbx
+    646c53b8:	add    %r13,%rsi
+    646c53bb:	nopl   0x0(%rax,%rax,1)
+    646c53c0:	mov    (%rbx),%rcx
+    646c53c3:	add    $0x8,%rbx
+    646c53c7:	call   646c78c8 <free>
+    646c53cc:	cmp    %rbx,%rsi
+    646c53cf:	jne    646c53c0 <variogram+0x1a0>
+    646c53d1:	movaps 0x40(%rsp),%xmm6
+    646c53d6:	mov    %r13,%rcx
+    646c53d9:	movaps 0x50(%rsp),%xmm7
+    646c53de:	add    $0x68,%rsp
+    646c53e2:	pop    %rbx
+    646c53e3:	pop    %rsi
+    646c53e4:	pop    %rdi
+    646c53e5:	pop    %rbp
+    646c53e6:	pop    %r12
+    646c53e8:	pop    %r13
+    646c53ea:	pop    %r14
+    646c53ec:	pop    %r15
+    646c53ee:	jmp    646c78c8 <free>
+    646c53f3:	nopl   (%rax)
+    646c53f6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5400 <variance>:
+    646c5400:	pxor   %xmm4,%xmm4
+    646c5404:	cvtsi2sd %edx,%xmm4
+    646c5408:	test   %edx,%edx
+    646c540a:	jle    646c54f0 <variance+0xf0>
+    646c5410:	cmp    $0x1,%edx
+    646c5413:	je     646c54f9 <variance+0xf9>
+    646c5419:	mov    %edx,%r8d
+    646c541c:	mov    %rcx,%rax
+    646c541f:	pxor   %xmm0,%xmm0
+    646c5423:	pxor   %xmm2,%xmm2
+    646c5427:	shr    %r8d
+    646c542a:	shl    $0x4,%r8
+    646c542e:	add    %rcx,%r8
+    646c5431:	movq   (%rax),%xmm1
+    646c5435:	add    $0x10,%rax
+    646c5439:	movhpd -0x8(%rax),%xmm1
+    646c543e:	cmp    %r8,%rax
+    646c5441:	addsd  %xmm1,%xmm2
+    646c5445:	unpckhpd %xmm1,%xmm1
+    646c5449:	addsd  %xmm1,%xmm2
+    646c544d:	jne    646c5431 <variance+0x31>
+    646c544f:	mov    %edx,%eax
+    646c5451:	and    $0xfffffffe,%eax
+    646c5454:	cmp    %eax,%edx
+    646c5456:	je     646c54e0 <variance+0xe0>
+    646c545c:	cltq
+    646c545e:	cmp    $0x1,%edx
+    646c5461:	addsd  (%rcx,%rax,8),%xmm2
+    646c5466:	divsd  %xmm4,%xmm2
+    646c546a:	je     646c54d3 <variance+0xd3>
+    646c546c:	mov    %edx,%r8d
+    646c546f:	mov    %rcx,%rax
+    646c5472:	movddup %xmm2,%xmm5
+    646c5476:	shr    %r8d
+    646c5479:	shl    $0x4,%r8
+    646c547d:	add    %rcx,%r8
+    646c5480:	movq   (%rax),%xmm1
+    646c5484:	add    $0x10,%rax
+    646c5488:	movhpd -0x8(%rax),%xmm1
+    646c548d:	cmp    %rax,%r8
+    646c5490:	subpd  %xmm5,%xmm1
+    646c5494:	mulpd  %xmm1,%xmm1
+    646c5498:	movapd %xmm1,%xmm3
+    646c549c:	unpckhpd %xmm1,%xmm1
+    646c54a0:	addsd  %xmm0,%xmm3
+    646c54a4:	movapd %xmm1,%xmm0
+    646c54a8:	addsd  %xmm3,%xmm0
+    646c54ac:	jne    646c5480 <variance+0x80>
+    646c54ae:	mov    %edx,%eax
+    646c54b0:	and    $0xfffffffe,%eax
+    646c54b3:	cmp    %edx,%eax
+    646c54b5:	je     646c54ce <variance+0xce>
+    646c54b7:	cltq
+    646c54b9:	movsd  (%rcx,%rax,8),%xmm3
+    646c54be:	subsd  %xmm2,%xmm3
+    646c54c2:	movapd %xmm3,%xmm2
+    646c54c6:	mulsd  %xmm3,%xmm2
+    646c54ca:	addsd  %xmm2,%xmm0
+    646c54ce:	divsd  %xmm4,%xmm0
+    646c54d2:	ret
+    646c54d3:	xor    %eax,%eax
+    646c54d5:	jmp    646c54b7 <variance+0xb7>
+    646c54d7:	nopw   0x0(%rax,%rax,1)
+    646c54e0:	divsd  %xmm4,%xmm2
+    646c54e4:	jmp    646c546c <variance+0x6c>
+    646c54e6:	cs nopw 0x0(%rax,%rax,1)
+    646c54f0:	pxor   %xmm0,%xmm0
+    646c54f4:	divsd  %xmm4,%xmm0
+    646c54f8:	ret
+    646c54f9:	xor    %eax,%eax
+    646c54fb:	pxor   %xmm0,%xmm0
+    646c54ff:	pxor   %xmm2,%xmm2
+    646c5503:	jmp    646c545c <variance+0x5c>
+    646c5508:	nop
+    646c5509:	nop
+    646c550a:	nop
+    646c550b:	nop
+    646c550c:	nop
+    646c550d:	nop
+    646c550e:	nop
+    646c550f:	nop
+
+00000000646c5510 <Sleep>:
+    646c5510:	jmp    *0x8d36(%rip)        # 646ce24c <__imp_Sleep>
+    646c5516:	nop
+    646c5517:	nop
+    646c5518:	nopl   0x0(%rax,%rax,1)
+
+00000000646c5520 <__do_global_dtors>:
+    646c5520:	sub    $0x28,%rsp
+    646c5524:	mov    0x2ad5(%rip),%rax        # 646c8000 <__data_start__>
+    646c552b:	mov    (%rax),%rax
+    646c552e:	test   %rax,%rax
+    646c5531:	je     646c5550 <__do_global_dtors+0x30>
+    646c5533:	call   *%rax
+    646c5535:	mov    0x2ac4(%rip),%rax        # 646c8000 <__data_start__>
+    646c553c:	lea    0x8(%rax),%rdx
+    646c5540:	mov    0x8(%rax),%rax
+    646c5544:	mov    %rdx,0x2ab5(%rip)        # 646c8000 <__data_start__>
+    646c554b:	test   %rax,%rax
+    646c554e:	jne    646c5533 <__do_global_dtors+0x13>
+    646c5550:	add    $0x28,%rsp
+    646c5554:	ret
+    646c5555:	nop
+    646c5556:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5560 <__do_global_ctors>:
+    646c5560:	push   %rsi
+    646c5561:	push   %rbx
+    646c5562:	sub    $0x28,%rsp
+    646c5566:	mov    0x4173(%rip),%rcx        # 646c96e0 <.refptr.__CTOR_LIST__>
+    646c556d:	mov    (%rcx),%rdx
+    646c5570:	cmp    $0xffffffff,%edx
+    646c5573:	mov    %edx,%eax
+    646c5575:	je     646c55b0 <__do_global_ctors+0x50>
+    646c5577:	test   %eax,%eax
+    646c5579:	je     646c559b <__do_global_ctors+0x3b>
+    646c557b:	mov    %eax,%edx
+    646c557d:	sub    $0x1,%eax
+    646c5580:	lea    (%rcx,%rdx,8),%rbx
+    646c5584:	sub    %rax,%rdx
+    646c5587:	lea    -0x8(%rcx,%rdx,8),%rsi
+    646c558c:	nopl   0x0(%rax)
+    646c5590:	call   *(%rbx)
+    646c5592:	sub    $0x8,%rbx
+    646c5596:	cmp    %rsi,%rbx
+    646c5599:	jne    646c5590 <__do_global_ctors+0x30>
+    646c559b:	lea    -0x82(%rip),%rcx        # 646c5520 <__do_global_dtors>
+    646c55a2:	add    $0x28,%rsp
+    646c55a6:	pop    %rbx
+    646c55a7:	pop    %rsi
+    646c55a8:	jmp    646c1380 <atexit>
+    646c55ad:	nopl   (%rax)
+    646c55b0:	xor    %eax,%eax
+    646c55b2:	jmp    646c55b6 <__do_global_ctors+0x56>
+    646c55b4:	mov    %edx,%eax
+    646c55b6:	lea    0x1(%rax),%r8d
+    646c55ba:	cmpq   $0x0,(%rcx,%r8,8)
+    646c55bf:	mov    %r8,%rdx
+    646c55c2:	jne    646c55b4 <__do_global_ctors+0x54>
+    646c55c4:	jmp    646c5577 <__do_global_ctors+0x17>
+    646c55c6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c55d0 <__main>:
+    646c55d0:	mov    0x6c4a(%rip),%eax        # 646cc220 <initialized>
+    646c55d6:	test   %eax,%eax
+    646c55d8:	je     646c55e0 <__main+0x10>
+    646c55da:	ret
+    646c55db:	nopl   0x0(%rax,%rax,1)
+    646c55e0:	movl   $0x1,0x6c36(%rip)        # 646cc220 <initialized>
+    646c55ea:	jmp    646c5560 <__do_global_ctors>
+    646c55ef:	nop
+
+00000000646c55f0 <__security_init_cookie>:
+    646c55f0:	push   %r12
+    646c55f2:	push   %rbp
+    646c55f3:	push   %rdi
+    646c55f4:	push   %rsi
+    646c55f5:	push   %rbx
+    646c55f6:	sub    $0x30,%rsp
+    646c55fa:	mov    0x2a7f(%rip),%rbx        # 646c8080 <__security_cookie>
+    646c5601:	movabs $0x2b992ddfa232,%rax
+    646c560b:	cmp    %rax,%rbx
+    646c560e:	movq   $0x0,0x20(%rsp)
+    646c5617:	je     646c5630 <__security_init_cookie+0x40>
+    646c5619:	not    %rbx
+    646c561c:	mov    %rbx,0x2a6d(%rip)        # 646c8090 <__security_cookie_complement>
+    646c5623:	add    $0x30,%rsp
+    646c5627:	pop    %rbx
+    646c5628:	pop    %rsi
+    646c5629:	pop    %rdi
+    646c562a:	pop    %rbp
+    646c562b:	pop    %r12
+    646c562d:	ret
+    646c562e:	xchg   %ax,%ax
+    646c5630:	lea    0x20(%rsp),%rcx
+    646c5635:	call   *0x8bc1(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c563b:	mov    0x20(%rsp),%rsi
+    646c5640:	call   *0x8b9e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c5646:	mov    %eax,%r12d
+    646c5649:	call   *0x8b9d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c564f:	mov    %eax,%ebp
+    646c5651:	call   *0x8bad(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c5657:	lea    0x28(%rsp),%rcx
+    646c565c:	mov    %eax,%edi
+    646c565e:	call   *0x8bb8(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c5664:	xor    0x28(%rsp),%rsi
+    646c5669:	mov    %r12d,%eax
+    646c566c:	movabs $0xffffffffffff,%rdx
+    646c5676:	xor    %rsi,%rax
+    646c5679:	mov    %ebp,%esi
+    646c567b:	xor    %rax,%rsi
+    646c567e:	mov    %edi,%eax
+    646c5680:	xor    %rsi,%rax
+    646c5683:	and    %rdx,%rax
+    646c5686:	cmp    %rbx,%rax
+    646c5689:	je     646c56b0 <__security_init_cookie+0xc0>
+    646c568b:	mov    %rax,%rdx
+    646c568e:	not    %rdx
+    646c5691:	mov    %rax,0x29e8(%rip)        # 646c8080 <__security_cookie>
+    646c5698:	mov    %rdx,0x29f1(%rip)        # 646c8090 <__security_cookie_complement>
+    646c569f:	add    $0x30,%rsp
+    646c56a3:	pop    %rbx
+    646c56a4:	pop    %rsi
+    646c56a5:	pop    %rdi
+    646c56a6:	pop    %rbp
+    646c56a7:	pop    %r12
+    646c56a9:	ret
+    646c56aa:	nopw   0x0(%rax,%rax,1)
+    646c56b0:	movabs $0xffffd466d2205dcc,%rdx
+    646c56ba:	movabs $0x2b992ddfa233,%rax
+    646c56c4:	jmp    646c5691 <__security_init_cookie+0xa1>
+    646c56c6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c56d0 <__report_gsfailure>:
+    646c56d0:	push   %rbp
+    646c56d1:	push   %rsi
+    646c56d2:	push   %rbx
+    646c56d3:	mov    %rsp,%rbp
+    646c56d6:	sub    $0x70,%rsp
+    646c56da:	mov    %rcx,%rsi
+    646c56dd:	lea    0x6b5c(%rip),%rcx        # 646cc240 <GS_ContextRecord>
+    646c56e4:	call   *0x8b42(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c56ea:	mov    0x6c47(%rip),%rbx        # 646cc338 <GS_ContextRecord+0xf8>
+    646c56f1:	lea    -0x28(%rbp),%rdx
+    646c56f5:	xor    %r8d,%r8d
+    646c56f8:	mov    %rbx,%rcx
+    646c56fb:	call   *0x8b33(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c5701:	test   %rax,%rax
+    646c5704:	je     646c57ad <__report_gsfailure+0xdd>
+    646c570a:	lea    -0x20(%rbp),%rdx
+    646c570e:	mov    %rax,%r9
+    646c5711:	mov    %rbx,%r8
+    646c5714:	movq   $0x0,0x38(%rsp)
+    646c571d:	lea    0x6b1c(%rip),%rcx        # 646cc240 <GS_ContextRecord>
+    646c5724:	mov    %rdx,0x30(%rsp)
+    646c5729:	lea    -0x18(%rbp),%rdx
+    646c572d:	mov    %rcx,0x20(%rsp)
+    646c5732:	xor    %ecx,%ecx
+    646c5734:	mov    %rdx,0x28(%rsp)
+    646c5739:	mov    -0x28(%rbp),%rdx
+    646c573d:	call   *0x8af9(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c5743:	mov    0x6bee(%rip),%rax        # 646cc338 <GS_ContextRecord+0xf8>
+    646c574a:	xor    %ecx,%ecx
+    646c574c:	mov    %rsi,0x6b6d(%rip)        # 646cc2c0 <GS_ContextRecord+0x80>
+    646c5753:	mov    %rax,0x6fd6(%rip)        # 646cc730 <GS_ExceptionRecord+0x10>
+    646c575a:	movabs $0x1c0000409,%rax
+    646c5764:	mov    %rax,0x6fb5(%rip)        # 646cc720 <GS_ExceptionRecord>
+    646c576b:	mov    0x290e(%rip),%rax        # 646c8080 <__security_cookie>
+    646c5772:	mov    %rax,-0x10(%rbp)
+    646c5776:	mov    0x2913(%rip),%rax        # 646c8090 <__security_cookie_complement>
+    646c577d:	mov    %rax,-0x8(%rbp)
+    646c5781:	call   *0x8abd(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c5787:	lea    0x3b02(%rip),%rcx        # 646c9290 <GS_ExceptionPointers>
+    646c578e:	call   *0x8ad0(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c5794:	call   *0x8a42(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c579a:	mov    $0xc0000409,%edx
+    646c579f:	mov    %rax,%rcx
+    646c57a2:	call   *0x8aac(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c57a8:	call   646c78f8 <abort>
+    646c57ad:	mov    0x18(%rbp),%rax
+    646c57b1:	mov    %rax,0x6b80(%rip)        # 646cc338 <GS_ContextRecord+0xf8>
+    646c57b8:	lea    0x8(%rbp),%rax
+    646c57bc:	mov    %rax,0x6b15(%rip)        # 646cc2d8 <GS_ContextRecord+0x98>
+    646c57c3:	jmp    646c5743 <__report_gsfailure+0x73>
+    646c57c8:	nop
+    646c57c9:	nop
+    646c57ca:	nop
+    646c57cb:	nop
+    646c57cc:	nop
+    646c57cd:	nop
+    646c57ce:	nop
+    646c57cf:	nop
+
+00000000646c57d0 <__dyn_tls_dtor>:
+    646c57d0:	sub    $0x28,%rsp
+    646c57d4:	cmp    $0x3,%edx
+    646c57d7:	je     646c57f0 <__dyn_tls_dtor+0x20>
+    646c57d9:	test   %edx,%edx
+    646c57db:	je     646c57f0 <__dyn_tls_dtor+0x20>
+    646c57dd:	mov    $0x1,%eax
+    646c57e2:	add    $0x28,%rsp
+    646c57e6:	ret
+    646c57e7:	nopw   0x0(%rax,%rax,1)
+    646c57f0:	call   646c6350 <__mingw_TLScallback>
+    646c57f5:	mov    $0x1,%eax
+    646c57fa:	add    $0x28,%rsp
+    646c57fe:	ret
+    646c57ff:	nop
+
+00000000646c5800 <__dyn_tls_init>:
+    646c5800:	push   %rsi
+    646c5801:	push   %rbx
+    646c5802:	sub    $0x28,%rsp
+    646c5806:	mov    0x3ec3(%rip),%rax        # 646c96d0 <.refptr._CRT_MT>
+    646c580d:	cmpl   $0x2,(%rax)
+    646c5810:	je     646c5818 <__dyn_tls_init+0x18>
+    646c5812:	movl   $0x2,(%rax)
+    646c5818:	cmp    $0x2,%edx
+    646c581b:	je     646c5830 <__dyn_tls_init+0x30>
+    646c581d:	cmp    $0x1,%edx
+    646c5820:	je     646c5862 <__dyn_tls_init+0x62>
+    646c5822:	mov    $0x1,%eax
+    646c5827:	add    $0x28,%rsp
+    646c582b:	pop    %rbx
+    646c582c:	pop    %rsi
+    646c582d:	ret
+    646c582e:	xchg   %ax,%ax
+    646c5830:	lea    0x9819(%rip),%rbx        # 646cf050 <__xd_z>
+    646c5837:	lea    0x9812(%rip),%rsi        # 646cf050 <__xd_z>
+    646c583e:	cmp    %rbx,%rsi
+    646c5841:	je     646c5822 <__dyn_tls_init+0x22>
+    646c5843:	mov    (%rbx),%rax
+    646c5846:	test   %rax,%rax
+    646c5849:	je     646c584d <__dyn_tls_init+0x4d>
+    646c584b:	call   *%rax
+    646c584d:	add    $0x8,%rbx
+    646c5851:	cmp    %rbx,%rsi
+    646c5854:	jne    646c5843 <__dyn_tls_init+0x43>
+    646c5856:	mov    $0x1,%eax
+    646c585b:	add    $0x28,%rsp
+    646c585f:	pop    %rbx
+    646c5860:	pop    %rsi
+    646c5861:	ret
+    646c5862:	call   646c6350 <__mingw_TLScallback>
+    646c5867:	mov    $0x1,%eax
+    646c586c:	add    $0x28,%rsp
+    646c5870:	pop    %rbx
+    646c5871:	pop    %rsi
+    646c5872:	ret
+    646c5873:	nopl   (%rax)
+    646c5876:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5880 <__tlregdtor>:
+    646c5880:	xor    %eax,%eax
+    646c5882:	ret
+    646c5883:	nop
+    646c5884:	nop
+    646c5885:	nop
+    646c5886:	nop
+    646c5887:	nop
     646c5888:	nop
     646c5889:	nop
     646c588a:	nop
     646c588b:	nop
     646c588c:	nop
     646c588d:	nop
     646c588e:	nop
     646c588f:	nop
 
-00000000646c5890 <__dyn_tls_dtor>:
-    646c5890:	sub    $0x28,%rsp
-    646c5894:	cmp    $0x3,%edx
-    646c5897:	je     646c58b0 <__dyn_tls_dtor+0x20>
-    646c5899:	test   %edx,%edx
-    646c589b:	je     646c58b0 <__dyn_tls_dtor+0x20>
-    646c589d:	mov    $0x1,%eax
-    646c58a2:	add    $0x28,%rsp
-    646c58a6:	ret
-    646c58a7:	nopw   0x0(%rax,%rax,1)
-    646c58b0:	call   646c6410 <__mingw_TLScallback>
-    646c58b5:	mov    $0x1,%eax
-    646c58ba:	add    $0x28,%rsp
-    646c58be:	ret
-    646c58bf:	nop
-
-00000000646c58c0 <__dyn_tls_init>:
-    646c58c0:	push   %rsi
-    646c58c1:	push   %rbx
-    646c58c2:	sub    $0x28,%rsp
-    646c58c6:	mov    0x3de3(%rip),%rax        # 646c96b0 <.refptr._CRT_MT>
-    646c58cd:	cmpl   $0x2,(%rax)
-    646c58d0:	je     646c58d8 <__dyn_tls_init+0x18>
-    646c58d2:	movl   $0x2,(%rax)
-    646c58d8:	cmp    $0x2,%edx
-    646c58db:	je     646c58f0 <__dyn_tls_init+0x30>
-    646c58dd:	cmp    $0x1,%edx
-    646c58e0:	je     646c5922 <__dyn_tls_init+0x62>
-    646c58e2:	mov    $0x1,%eax
-    646c58e7:	add    $0x28,%rsp
-    646c58eb:	pop    %rbx
-    646c58ec:	pop    %rsi
-    646c58ed:	ret
-    646c58ee:	xchg   %ax,%ax
-    646c58f0:	lea    0x9759(%rip),%rbx        # 646cf050 <__xd_z>
-    646c58f7:	lea    0x9752(%rip),%rsi        # 646cf050 <__xd_z>
-    646c58fe:	cmp    %rbx,%rsi
-    646c5901:	je     646c58e2 <__dyn_tls_init+0x22>
-    646c5903:	mov    (%rbx),%rax
-    646c5906:	test   %rax,%rax
-    646c5909:	je     646c590d <__dyn_tls_init+0x4d>
-    646c590b:	call   *%rax
-    646c590d:	add    $0x8,%rbx
-    646c5911:	cmp    %rbx,%rsi
-    646c5914:	jne    646c5903 <__dyn_tls_init+0x43>
-    646c5916:	mov    $0x1,%eax
-    646c591b:	add    $0x28,%rsp
-    646c591f:	pop    %rbx
-    646c5920:	pop    %rsi
-    646c5921:	ret
-    646c5922:	call   646c6410 <__mingw_TLScallback>
-    646c5927:	mov    $0x1,%eax
-    646c592c:	add    $0x28,%rsp
-    646c5930:	pop    %rbx
-    646c5931:	pop    %rsi
-    646c5932:	ret
-    646c5933:	nopl   (%rax)
-    646c5936:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5940 <__tlregdtor>:
-    646c5940:	xor    %eax,%eax
-    646c5942:	ret
-    646c5943:	nop
-    646c5944:	nop
-    646c5945:	nop
-    646c5946:	nop
-    646c5947:	nop
-    646c5948:	nop
-    646c5949:	nop
-    646c594a:	nop
-    646c594b:	nop
-    646c594c:	nop
-    646c594d:	nop
-    646c594e:	nop
-    646c594f:	nop
-
-00000000646c5950 <_decode_pointer>:
-    646c5950:	mov    %rcx,%rax
-    646c5953:	ret
-    646c5954:	xchg   %ax,%ax
-    646c5956:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5960 <_encode_pointer>:
-    646c5960:	mov    %rcx,%rax
-    646c5963:	ret
-    646c5964:	nop
-    646c5965:	nop
-    646c5966:	nop
-    646c5967:	nop
-    646c5968:	nop
-    646c5969:	nop
-    646c596a:	nop
-    646c596b:	nop
-    646c596c:	nop
-    646c596d:	nop
-    646c596e:	nop
-    646c596f:	nop
-
-00000000646c5970 <__write_memory.part.0>:
-    646c5970:	push   %r12
-    646c5972:	push   %rbp
-    646c5973:	push   %rdi
-    646c5974:	push   %rsi
-    646c5975:	push   %rbx
-    646c5976:	sub    $0x50,%rsp
-    646c597a:	movslq 0x6e83(%rip),%rsi        # 646cc804 <maxSections>
-    646c5981:	test   %esi,%esi
-    646c5983:	mov    %rcx,%rbx
-    646c5986:	mov    %rdx,%rbp
-    646c5989:	mov    %r8,%rdi
-    646c598c:	jle    646c5af8 <__write_memory.part.0+0x188>
-    646c5992:	mov    0x6e6f(%rip),%rax        # 646cc808 <the_secs>
-    646c5999:	xor    %ecx,%ecx
-    646c599b:	add    $0x18,%rax
-    646c599f:	nop
-    646c59a0:	mov    (%rax),%rdx
-    646c59a3:	cmp    %rdx,%rbx
-    646c59a6:	jb     646c59bc <__write_memory.part.0+0x4c>
-    646c59a8:	mov    0x8(%rax),%r8
-    646c59ac:	mov    0x8(%r8),%r8d
-    646c59b0:	add    %r8,%rdx
-    646c59b3:	cmp    %rdx,%rbx
-    646c59b6:	jb     646c5a45 <__write_memory.part.0+0xd5>
-    646c59bc:	add    $0x1,%ecx
-    646c59bf:	add    $0x28,%rax
-    646c59c3:	cmp    %esi,%ecx
-    646c59c5:	jne    646c59a0 <__write_memory.part.0+0x30>
-    646c59c7:	mov    %rbx,%rcx
-    646c59ca:	call   646c6610 <__mingw_GetSectionForAddress>
-    646c59cf:	test   %rax,%rax
-    646c59d2:	mov    %rax,%r12
-    646c59d5:	je     646c5b2d <__write_memory.part.0+0x1bd>
-    646c59db:	mov    0x6e26(%rip),%rax        # 646cc808 <the_secs>
-    646c59e2:	lea    (%rsi,%rsi,4),%rsi
-    646c59e6:	shl    $0x3,%rsi
-    646c59ea:	add    %rsi,%rax
-    646c59ed:	mov    %r12,0x20(%rax)
-    646c59f1:	movl   $0x0,(%rax)
-    646c59f7:	call   646c6740 <_GetPEImageBase>
-    646c59fc:	mov    0xc(%r12),%ecx
-    646c5a01:	lea    0x20(%rsp),%rdx
-    646c5a06:	mov    $0x30,%r8d
-    646c5a0c:	add    %rax,%rcx
-    646c5a0f:	mov    0x6df2(%rip),%rax        # 646cc808 <the_secs>
-    646c5a16:	mov    %rcx,0x18(%rax,%rsi,1)
-    646c5a1b:	call   *0x8853(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c5a21:	test   %rax,%rax
-    646c5a24:	je     646c5b10 <__write_memory.part.0+0x1a0>
-    646c5a2a:	mov    0x44(%rsp),%eax
-    646c5a2e:	lea    -0x4(%rax),%edx
-    646c5a31:	and    $0xfffffffb,%edx
-    646c5a34:	je     646c5a3e <__write_memory.part.0+0xce>
-    646c5a36:	sub    $0x40,%eax
-    646c5a39:	and    $0xffffffbf,%eax
-    646c5a3c:	jne    646c5aa0 <__write_memory.part.0+0x130>
-    646c5a3e:	addl   $0x1,0x6dbf(%rip)        # 646cc804 <maxSections>
-    646c5a45:	cmp    $0x8,%edi
-    646c5a48:	jae    646c5a73 <__write_memory.part.0+0x103>
-    646c5a4a:	test   $0x4,%dil
-    646c5a4e:	jne    646c5ae4 <__write_memory.part.0+0x174>
-    646c5a54:	test   %edi,%edi
-    646c5a56:	je     646c5a68 <__write_memory.part.0+0xf8>
-    646c5a58:	movzbl 0x0(%rbp),%eax
-    646c5a5c:	test   $0x2,%dil
-    646c5a60:	mov    %al,(%rbx)
-    646c5a62:	jne    646c5aff <__write_memory.part.0+0x18f>
-    646c5a68:	add    $0x50,%rsp
-    646c5a6c:	pop    %rbx
-    646c5a6d:	pop    %rsi
-    646c5a6e:	pop    %rdi
-    646c5a6f:	pop    %rbp
-    646c5a70:	pop    %r12
-    646c5a72:	ret
-    646c5a73:	mov    %edi,%eax
-    646c5a75:	sub    $0x1,%edi
-    646c5a78:	mov    -0x8(%rbp,%rax,1),%rdx
-    646c5a7d:	cmp    $0x8,%edi
-    646c5a80:	mov    %rdx,-0x8(%rbx,%rax,1)
-    646c5a85:	jb     646c5a68 <__write_memory.part.0+0xf8>
-    646c5a87:	and    $0xfffffff8,%edi
-    646c5a8a:	xor    %eax,%eax
-    646c5a8c:	mov    %eax,%edx
-    646c5a8e:	add    $0x8,%eax
-    646c5a91:	mov    0x0(%rbp,%rdx,1),%rcx
-    646c5a96:	cmp    %edi,%eax
-    646c5a98:	mov    %rcx,(%rbx,%rdx,1)
-    646c5a9c:	jb     646c5a8c <__write_memory.part.0+0x11c>
-    646c5a9e:	jmp    646c5a68 <__write_memory.part.0+0xf8>
-    646c5aa0:	add    0x6d61(%rip),%rsi        # 646cc808 <the_secs>
-    646c5aa7:	mov    $0x40,%r8d
-    646c5aad:	mov    0x20(%rsp),%rcx
-    646c5ab2:	mov    0x38(%rsp),%rdx
-    646c5ab7:	mov    %rsi,%r9
-    646c5aba:	mov    %rcx,0x8(%rsi)
-    646c5abe:	mov    %rdx,0x10(%rsi)
-    646c5ac2:	call   *0x87a4(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c5ac8:	test   %eax,%eax
-    646c5aca:	jne    646c5a3e <__write_memory.part.0+0xce>
-    646c5ad0:	call   *0x871e(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c5ad6:	lea    0x387b(%rip),%rcx        # 646c9358 <.rdata+0x78>
-    646c5add:	mov    %eax,%edx
-    646c5adf:	call   646c7dc0 <__report_error>
-    646c5ae4:	mov    0x0(%rbp),%eax
-    646c5ae7:	mov    %edi,%edi
-    646c5ae9:	mov    %eax,(%rbx)
-    646c5aeb:	mov    -0x4(%rbp,%rdi,1),%eax
-    646c5aef:	mov    %eax,-0x4(%rbx,%rdi,1)
-    646c5af3:	jmp    646c5a68 <__write_memory.part.0+0xf8>
-    646c5af8:	xor    %esi,%esi
-    646c5afa:	jmp    646c59c7 <__write_memory.part.0+0x57>
-    646c5aff:	mov    %edi,%edi
-    646c5b01:	movzwl -0x2(%rbp,%rdi,1),%eax
-    646c5b06:	mov    %ax,-0x2(%rbx,%rdi,1)
-    646c5b0b:	jmp    646c5a68 <__write_memory.part.0+0xf8>
-    646c5b10:	mov    0x6cf1(%rip),%rax        # 646cc808 <the_secs>
-    646c5b17:	lea    0x3802(%rip),%rcx        # 646c9320 <.rdata+0x40>
-    646c5b1e:	mov    0x8(%r12),%edx
-    646c5b23:	mov    0x18(%rax,%rsi,1),%r8
-    646c5b28:	call   646c7dc0 <__report_error>
-    646c5b2d:	lea    0x37cc(%rip),%rcx        # 646c9300 <.rdata+0x20>
-    646c5b34:	mov    %rbx,%rdx
-    646c5b37:	call   646c7dc0 <__report_error>
-    646c5b3c:	nop
-    646c5b3d:	nopl   (%rax)
-
-00000000646c5b40 <_pei386_runtime_relocator>:
-    646c5b40:	push   %rbp
-    646c5b41:	push   %r15
-    646c5b43:	push   %r14
-    646c5b45:	push   %r13
-    646c5b47:	push   %r12
-    646c5b49:	push   %rdi
-    646c5b4a:	push   %rsi
-    646c5b4b:	push   %rbx
-    646c5b4c:	sub    $0x38,%rsp
-    646c5b50:	lea    0x80(%rsp),%rbp
-    646c5b58:	mov    0x6ca2(%rip),%ebx        # 646cc800 <was_init.95174>
-    646c5b5e:	test   %ebx,%ebx
-    646c5b60:	je     646c5b73 <_pei386_runtime_relocator+0x33>
-    646c5b62:	lea    -0x48(%rbp),%rsp
-    646c5b66:	pop    %rbx
-    646c5b67:	pop    %rsi
-    646c5b68:	pop    %rdi
-    646c5b69:	pop    %r12
-    646c5b6b:	pop    %r13
-    646c5b6d:	pop    %r14
-    646c5b6f:	pop    %r15
-    646c5b71:	pop    %rbp
-    646c5b72:	ret
-    646c5b73:	movl   $0x1,0x6c83(%rip)        # 646cc800 <was_init.95174>
-    646c5b7d:	call   646c6690 <__mingw_GetSectionCount>
-    646c5b82:	cltq
-    646c5b84:	lea    (%rax,%rax,4),%rax
-    646c5b88:	lea    0x1e(,%rax,8),%rax
-    646c5b90:	and    $0xfffffffffffffff0,%rax
-    646c5b94:	call   646c68e0 <___chkstk_ms>
-    646c5b99:	mov    0x3b30(%rip),%r12        # 646c96d0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-    646c5ba0:	movl   $0x0,0x6c5a(%rip)        # 646cc804 <maxSections>
-    646c5baa:	mov    0x3b2f(%rip),%rsi        # 646c96e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
-    646c5bb1:	sub    %rax,%rsp
-    646c5bb4:	lea    0x20(%rsp),%rax
-    646c5bb9:	mov    %rax,0x6c48(%rip)        # 646cc808 <the_secs>
-    646c5bc0:	mov    %r12,%rax
-    646c5bc3:	sub    %rsi,%rax
-    646c5bc6:	cmp    $0x7,%rax
-    646c5bca:	jle    646c5b62 <_pei386_runtime_relocator+0x22>
-    646c5bcc:	cmp    $0xb,%rax
-    646c5bd0:	mov    (%rsi),%edx
-    646c5bd2:	jle    646c5ca0 <_pei386_runtime_relocator+0x160>
-    646c5bd8:	test   %edx,%edx
-    646c5bda:	je     646c5c84 <_pei386_runtime_relocator+0x144>
-    646c5be0:	cmp    %r12,%rsi
-    646c5be3:	jae    646c5b62 <_pei386_runtime_relocator+0x22>
-    646c5be9:	lea    0x8(%rsi),%r14
-    646c5bed:	add    $0x7,%r12
-    646c5bf1:	mov    0x3b08(%rip),%r13        # 646c9700 <.refptr.__image_base__>
-    646c5bf8:	lea    -0x58(%rbp),%rdi
-    646c5bfc:	sub    %r14,%r12
-    646c5bff:	shr    $0x3,%r12
-    646c5c03:	lea    0x8(%rsi,%r12,8),%r12
-    646c5c08:	jmp    646c5c14 <_pei386_runtime_relocator+0xd4>
-    646c5c0a:	nopw   0x0(%rax,%rax,1)
-    646c5c10:	add    $0x8,%r14
-    646c5c14:	mov    0x4(%rsi),%ecx
-    646c5c17:	mov    $0x4,%r8d
-    646c5c1d:	mov    %rdi,%rdx
-    646c5c20:	mov    (%rsi),%eax
-    646c5c22:	mov    %r14,%rsi
-    646c5c25:	add    %r13,%rcx
-    646c5c28:	add    (%rcx),%eax
-    646c5c2a:	mov    %eax,-0x58(%rbp)
-    646c5c2d:	call   646c5970 <__write_memory.part.0>
-    646c5c32:	cmp    %r12,%r14
-    646c5c35:	jne    646c5c10 <_pei386_runtime_relocator+0xd0>
-    646c5c37:	mov    0x6bc7(%rip),%eax        # 646cc804 <maxSections>
-    646c5c3d:	xor    %esi,%esi
-    646c5c3f:	mov    0x8626(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
-    646c5c46:	test   %eax,%eax
-    646c5c48:	jle    646c5b62 <_pei386_runtime_relocator+0x22>
-    646c5c4e:	xchg   %ax,%ax
-    646c5c50:	mov    0x6bb1(%rip),%rax        # 646cc808 <the_secs>
-    646c5c57:	add    %rsi,%rax
-    646c5c5a:	mov    (%rax),%r8d
-    646c5c5d:	test   %r8d,%r8d
-    646c5c60:	je     646c5c70 <_pei386_runtime_relocator+0x130>
-    646c5c62:	mov    0x10(%rax),%rdx
-    646c5c66:	mov    %rdi,%r9
-    646c5c69:	mov    0x8(%rax),%rcx
-    646c5c6d:	call   *%r12
-    646c5c70:	add    $0x1,%ebx
-    646c5c73:	add    $0x28,%rsi
-    646c5c77:	cmp    0x6b87(%rip),%ebx        # 646cc804 <maxSections>
-    646c5c7d:	jl     646c5c50 <_pei386_runtime_relocator+0x110>
-    646c5c7f:	jmp    646c5b62 <_pei386_runtime_relocator+0x22>
-    646c5c84:	mov    0x4(%rsi),%ecx
-    646c5c87:	test   %ecx,%ecx
-    646c5c89:	jne    646c5be0 <_pei386_runtime_relocator+0xa0>
-    646c5c8f:	mov    0x8(%rsi),%edx
-    646c5c92:	test   %edx,%edx
-    646c5c94:	jne    646c5cb3 <_pei386_runtime_relocator+0x173>
-    646c5c96:	mov    0xc(%rsi),%edx
-    646c5c99:	add    $0xc,%rsi
-    646c5c9d:	nopl   (%rax)
-    646c5ca0:	test   %edx,%edx
-    646c5ca2:	jne    646c5be0 <_pei386_runtime_relocator+0xa0>
-    646c5ca8:	mov    0x4(%rsi),%eax
-    646c5cab:	test   %eax,%eax
-    646c5cad:	jne    646c5be0 <_pei386_runtime_relocator+0xa0>
-    646c5cb3:	mov    0x8(%rsi),%edx
-    646c5cb6:	cmp    $0x1,%edx
-    646c5cb9:	jne    646c5dee <_pei386_runtime_relocator+0x2ae>
-    646c5cbf:	mov    0x3a3a(%rip),%r13        # 646c9700 <.refptr.__image_base__>
-    646c5cc6:	add    $0xc,%rsi
-    646c5cca:	movabs $0xffffffff00000000,%r15
-    646c5cd4:	lea    -0x58(%rbp),%r14
-    646c5cd8:	cmp    %r12,%rsi
-    646c5cdb:	jb     646c5d25 <_pei386_runtime_relocator+0x1e5>
-    646c5cdd:	jmp    646c5b62 <_pei386_runtime_relocator+0x22>
-    646c5ce2:	jbe    646c5da0 <_pei386_runtime_relocator+0x260>
-    646c5ce8:	cmp    $0x20,%edx
-    646c5ceb:	je     646c5d70 <_pei386_runtime_relocator+0x230>
-    646c5cf1:	cmp    $0x40,%edx
-    646c5cf4:	jne    646c5dda <_pei386_runtime_relocator+0x29a>
-    646c5cfa:	mov    (%rcx),%rdx
-    646c5cfd:	mov    $0x8,%r8d
-    646c5d03:	mov    %r14,%rdi
-    646c5d06:	sub    %rax,%rdx
-    646c5d09:	add    %r9,%rdx
-    646c5d0c:	mov    %rdx,-0x58(%rbp)
-    646c5d10:	mov    %r14,%rdx
-    646c5d13:	call   646c5970 <__write_memory.part.0>
-    646c5d18:	add    $0xc,%rsi
-    646c5d1c:	cmp    %r12,%rsi
-    646c5d1f:	jae    646c5c37 <_pei386_runtime_relocator+0xf7>
-    646c5d25:	mov    0x4(%rsi),%ecx
-    646c5d28:	mov    (%rsi),%eax
-    646c5d2a:	movzbl 0x8(%rsi),%edx
-    646c5d2e:	add    %r13,%rcx
-    646c5d31:	add    %r13,%rax
-    646c5d34:	cmp    $0x10,%edx
-    646c5d37:	mov    (%rax),%r9
-    646c5d3a:	jne    646c5ce2 <_pei386_runtime_relocator+0x1a2>
-    646c5d3c:	movzwl (%rcx),%r8d
-    646c5d40:	mov    %r14,%rdx
-    646c5d43:	mov    %r14,%rdi
-    646c5d46:	mov    %r8,%r10
-    646c5d49:	or     $0xffffffffffff0000,%r10
-    646c5d50:	test   %r8w,%r8w
-    646c5d54:	cmovs  %r10,%r8
-    646c5d58:	sub    %rax,%r8
-    646c5d5b:	add    %r9,%r8
-    646c5d5e:	mov    %r8,-0x58(%rbp)
-    646c5d62:	mov    $0x2,%r8d
-    646c5d68:	call   646c5970 <__write_memory.part.0>
-    646c5d6d:	jmp    646c5d18 <_pei386_runtime_relocator+0x1d8>
-    646c5d6f:	nop
-    646c5d70:	mov    (%rcx),%edx
-    646c5d72:	mov    %r14,%rdi
-    646c5d75:	mov    %rdx,%r8
-    646c5d78:	or     %r15,%rdx
-    646c5d7b:	test   %r8d,%r8d
-    646c5d7e:	cmovns %r8,%rdx
-    646c5d82:	mov    $0x4,%r8d
-    646c5d88:	sub    %rax,%rdx
-    646c5d8b:	add    %r9,%rdx
-    646c5d8e:	mov    %rdx,-0x58(%rbp)
-    646c5d92:	mov    %r14,%rdx
-    646c5d95:	call   646c5970 <__write_memory.part.0>
-    646c5d9a:	jmp    646c5d18 <_pei386_runtime_relocator+0x1d8>
-    646c5d9f:	nop
-    646c5da0:	cmp    $0x8,%edx
-    646c5da3:	jne    646c5dda <_pei386_runtime_relocator+0x29a>
-    646c5da5:	movzbl (%rcx),%r8d
-    646c5da9:	mov    %r14,%rdx
-    646c5dac:	mov    %r14,%rdi
-    646c5daf:	mov    %r8,%r10
-    646c5db2:	or     $0xffffffffffffff00,%r10
-    646c5db9:	test   %r8b,%r8b
-    646c5dbc:	cmovs  %r10,%r8
-    646c5dc0:	sub    %rax,%r8
-    646c5dc3:	add    %r9,%r8
-    646c5dc6:	mov    %r8,-0x58(%rbp)
-    646c5dca:	mov    $0x1,%r8d
-    646c5dd0:	call   646c5970 <__write_memory.part.0>
-    646c5dd5:	jmp    646c5d18 <_pei386_runtime_relocator+0x1d8>
-    646c5dda:	lea    0x35d7(%rip),%rcx        # 646c93b8 <.rdata+0xd8>
-    646c5de1:	movq   $0x0,-0x58(%rbp)
-    646c5de9:	call   646c7dc0 <__report_error>
-    646c5dee:	lea    0x358b(%rip),%rcx        # 646c9380 <.rdata+0xa0>
-    646c5df5:	call   646c7dc0 <__report_error>
-    646c5dfa:	nop
-    646c5dfb:	nop
-    646c5dfc:	nop
-    646c5dfd:	nop
-    646c5dfe:	nop
-    646c5dff:	nop
-
-00000000646c5e00 <__mingw_SEH_error_handler>:
-    646c5e00:	sub    $0x28,%rsp
-    646c5e04:	mov    (%rcx),%eax
-    646c5e06:	cmp    $0xc0000091,%eax
-    646c5e0b:	ja     646c5e70 <__mingw_SEH_error_handler+0x70>
-    646c5e0d:	cmp    $0xc000008d,%eax
-    646c5e12:	jae    646c5e8f <__mingw_SEH_error_handler+0x8f>
-    646c5e14:	cmp    $0xc0000008,%eax
-    646c5e19:	je     646c5f24 <__mingw_SEH_error_handler+0x124>
-    646c5e1f:	ja     646c5ef0 <__mingw_SEH_error_handler+0xf0>
-    646c5e25:	cmp    $0x80000002,%eax
-    646c5e2a:	je     646c5f24 <__mingw_SEH_error_handler+0x124>
-    646c5e30:	cmp    $0xc0000005,%eax
-    646c5e35:	jne    646c5efe <__mingw_SEH_error_handler+0xfe>
-    646c5e3b:	xor    %edx,%edx
-    646c5e3d:	mov    $0xb,%ecx
-    646c5e42:	call   646c7958 <signal>
-    646c5e47:	cmp    $0x1,%rax
-    646c5e4b:	je     646c5f80 <__mingw_SEH_error_handler+0x180>
-    646c5e51:	test   %rax,%rax
-    646c5e54:	je     646c5f96 <__mingw_SEH_error_handler+0x196>
-    646c5e5a:	mov    $0xb,%ecx
-    646c5e5f:	call   *%rax
-    646c5e61:	xor    %eax,%eax
-    646c5e63:	add    $0x28,%rsp
-    646c5e67:	ret
-    646c5e68:	nopl   0x0(%rax,%rax,1)
-    646c5e70:	cmp    $0xc0000094,%eax
-    646c5e75:	je     646c5f30 <__mingw_SEH_error_handler+0x130>
-    646c5e7b:	ja     646c5eb4 <__mingw_SEH_error_handler+0xb4>
-    646c5e7d:	cmp    $0xc0000092,%eax
-    646c5e82:	je     646c5f24 <__mingw_SEH_error_handler+0x124>
-    646c5e88:	cmp    $0xc0000093,%eax
-    646c5e8d:	jne    646c5efe <__mingw_SEH_error_handler+0xfe>
-    646c5e8f:	xor    %edx,%edx
-    646c5e91:	mov    $0x8,%ecx
-    646c5e96:	call   646c7958 <signal>
-    646c5e9b:	cmp    $0x1,%rax
-    646c5e9f:	je     646c5f10 <__mingw_SEH_error_handler+0x110>
-    646c5ea1:	test   %rax,%rax
-    646c5ea4:	je     646c5efe <__mingw_SEH_error_handler+0xfe>
-    646c5ea6:	mov    $0x8,%ecx
-    646c5eab:	call   *%rax
-    646c5ead:	xor    %eax,%eax
-    646c5eaf:	add    $0x28,%rsp
-    646c5eb3:	ret
-    646c5eb4:	cmp    $0xc0000095,%eax
-    646c5eb9:	je     646c5f24 <__mingw_SEH_error_handler+0x124>
-    646c5ebb:	cmp    $0xc0000096,%eax
-    646c5ec0:	jne    646c5efe <__mingw_SEH_error_handler+0xfe>
-    646c5ec2:	xor    %edx,%edx
-    646c5ec4:	mov    $0x4,%ecx
-    646c5ec9:	call   646c7958 <signal>
-    646c5ece:	cmp    $0x1,%rax
-    646c5ed2:	je     646c5f60 <__mingw_SEH_error_handler+0x160>
-    646c5ed8:	test   %rax,%rax
-    646c5edb:	je     646c5f96 <__mingw_SEH_error_handler+0x196>
-    646c5ee1:	mov    $0x4,%ecx
-    646c5ee6:	call   *%rax
-    646c5ee8:	xor    %eax,%eax
-    646c5eea:	add    $0x28,%rsp
-    646c5eee:	ret
-    646c5eef:	nop
-    646c5ef0:	cmp    $0xc000001d,%eax
-    646c5ef5:	je     646c5ec2 <__mingw_SEH_error_handler+0xc2>
-    646c5ef7:	cmp    $0xc000008c,%eax
-    646c5efc:	je     646c5f24 <__mingw_SEH_error_handler+0x124>
-    646c5efe:	mov    $0x1,%eax
-    646c5f03:	add    $0x28,%rsp
-    646c5f07:	ret
-    646c5f08:	nopl   0x0(%rax,%rax,1)
-    646c5f10:	mov    $0x1,%edx
-    646c5f15:	mov    $0x8,%ecx
-    646c5f1a:	call   646c7958 <signal>
-    646c5f1f:	call   646c68d0 <_fpreset>
-    646c5f24:	xor    %eax,%eax
-    646c5f26:	add    $0x28,%rsp
-    646c5f2a:	ret
-    646c5f2b:	nopl   0x0(%rax,%rax,1)
-    646c5f30:	xor    %edx,%edx
-    646c5f32:	mov    $0x8,%ecx
-    646c5f37:	call   646c7958 <signal>
-    646c5f3c:	cmp    $0x1,%rax
-    646c5f40:	jne    646c5ea1 <__mingw_SEH_error_handler+0xa1>
-    646c5f46:	mov    $0x1,%edx
-    646c5f4b:	mov    $0x8,%ecx
-    646c5f50:	call   646c7958 <signal>
-    646c5f55:	xor    %eax,%eax
-    646c5f57:	jmp    646c5e63 <__mingw_SEH_error_handler+0x63>
-    646c5f5c:	nopl   0x0(%rax)
-    646c5f60:	mov    $0x1,%edx
-    646c5f65:	mov    $0x4,%ecx
-    646c5f6a:	call   646c7958 <signal>
-    646c5f6f:	xor    %eax,%eax
-    646c5f71:	jmp    646c5e63 <__mingw_SEH_error_handler+0x63>
-    646c5f76:	cs nopw 0x0(%rax,%rax,1)
-    646c5f80:	mov    $0x1,%edx
-    646c5f85:	mov    $0xb,%ecx
-    646c5f8a:	call   646c7958 <signal>
-    646c5f8f:	xor    %eax,%eax
-    646c5f91:	jmp    646c5e63 <__mingw_SEH_error_handler+0x63>
-    646c5f96:	mov    $0x4,%eax
-    646c5f9b:	jmp    646c5e63 <__mingw_SEH_error_handler+0x63>
-
-00000000646c5fa0 <__mingw_init_ehandler>:
-    646c5fa0:	push   %r12
-    646c5fa2:	push   %rbp
-    646c5fa3:	push   %rdi
-    646c5fa4:	push   %rsi
-    646c5fa5:	push   %rbx
-    646c5fa6:	sub    $0x20,%rsp
-    646c5faa:	call   646c6740 <_GetPEImageBase>
-    646c5faf:	mov    %rax,%rbp
-    646c5fb2:	mov    0x6870(%rip),%eax        # 646cc828 <was_here.95013>
-    646c5fb8:	test   %eax,%eax
-    646c5fba:	jne    646c5fe1 <__mingw_init_ehandler+0x41>
-    646c5fbc:	test   %rbp,%rbp
-    646c5fbf:	je     646c5fe1 <__mingw_init_ehandler+0x41>
-    646c5fc1:	lea    0x3428(%rip),%rcx        # 646c93f0 <.rdata>
-    646c5fc8:	movl   $0x1,0x6856(%rip)        # 646cc828 <was_here.95013>
-    646c5fd2:	call   646c6580 <_FindPESectionByName>
-    646c5fd7:	test   %rax,%rax
-    646c5fda:	je     646c5ff0 <__mingw_init_ehandler+0x50>
-    646c5fdc:	mov    $0x1,%eax
-    646c5fe1:	add    $0x20,%rsp
-    646c5fe5:	pop    %rbx
-    646c5fe6:	pop    %rsi
-    646c5fe7:	pop    %rdi
-    646c5fe8:	pop    %rbp
-    646c5fe9:	pop    %r12
-    646c5feb:	ret
-    646c5fec:	nopl   0x0(%rax)
-    646c5ff0:	lea    0x6949(%rip),%rbx        # 646cc940 <emu_pdata>
-    646c5ff7:	mov    $0x30,%ecx
-    646c5ffc:	xor    %esi,%esi
-    646c5ffe:	lea    0x683b(%rip),%rdx        # 646cc840 <emu_xdata>
-    646c6005:	mov    %rbx,%rdi
-    646c6008:	rep stos %rax,%es:(%rdi)
-    646c600b:	lea    -0x212(%rip),%r12        # 646c5e00 <__mingw_SEH_error_handler>
-    646c6012:	mov    $0x20,%ecx
-    646c6017:	mov    %rdx,%rdi
-    646c601a:	rep stos %rax,%es:(%rdi)
-    646c601d:	sub    %rbp,%r12
-    646c6020:	mov    %rdx,%rdi
-    646c6023:	jmp    646c6053 <__mingw_init_ehandler+0xb3>
-    646c6025:	movb   $0x9,(%rdi)
-    646c6028:	add    $0x1,%rsi
-    646c602c:	add    $0xc,%rbx
-    646c6030:	mov    %r12d,0x4(%rdi)
-    646c6034:	mov    0xc(%rax),%ecx
-    646c6037:	mov    %ecx,-0xc(%rbx)
-    646c603a:	add    0x8(%rax),%ecx
-    646c603d:	mov    %rdi,%rax
-    646c6040:	add    $0x8,%rdi
-    646c6044:	sub    %rbp,%rax
-    646c6047:	mov    %eax,-0x4(%rbx)
-    646c604a:	mov    %ecx,-0x8(%rbx)
-    646c604d:	cmp    $0x20,%rsi
-    646c6051:	je     646c6085 <__mingw_init_ehandler+0xe5>
-    646c6053:	mov    %rsi,%rcx
-    646c6056:	call   646c66d0 <_FindPESectionExec>
-    646c605b:	test   %rax,%rax
-    646c605e:	jne    646c6025 <__mingw_init_ehandler+0x85>
-    646c6060:	test   %rsi,%rsi
-    646c6063:	mov    %esi,%edx
-    646c6065:	je     646c5fdc <__mingw_init_ehandler+0x3c>
-    646c606b:	nopl   0x0(%rax,%rax,1)
-    646c6070:	lea    0x68c9(%rip),%rcx        # 646cc940 <emu_pdata>
-    646c6077:	mov    %rbp,%r8
-    646c607a:	call   *0x81a4(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c6080:	jmp    646c5fdc <__mingw_init_ehandler+0x3c>
-    646c6085:	mov    $0x20,%edx
-    646c608a:	jmp    646c6070 <__mingw_init_ehandler+0xd0>
-    646c608c:	nopl   0x0(%rax)
-
-00000000646c6090 <_gnu_exception_handler>:
-    646c6090:	push   %rbx
-    646c6091:	sub    $0x20,%rsp
-    646c6095:	mov    (%rcx),%rdx
-    646c6098:	mov    (%rdx),%eax
-    646c609a:	mov    %rcx,%rbx
-    646c609d:	mov    %eax,%ecx
-    646c609f:	and    $0x20ffffff,%ecx
-    646c60a5:	cmp    $0x20474343,%ecx
-    646c60ab:	je     646c6170 <_gnu_exception_handler+0xe0>
-    646c60b1:	cmp    $0xc0000091,%eax
-    646c60b6:	ja     646c6120 <_gnu_exception_handler+0x90>
-    646c60b8:	cmp    $0xc000008d,%eax
-    646c60bd:	jae    646c613b <_gnu_exception_handler+0xab>
-    646c60bf:	cmp    $0xc0000008,%eax
-    646c60c4:	je     646c617a <_gnu_exception_handler+0xea>
-    646c60ca:	ja     646c61c4 <_gnu_exception_handler+0x134>
-    646c60d0:	cmp    $0x80000002,%eax
-    646c60d5:	je     646c617a <_gnu_exception_handler+0xea>
-    646c60db:	cmp    $0xc0000005,%eax
-    646c60e0:	jne    646c6101 <_gnu_exception_handler+0x71>
-    646c60e2:	xor    %edx,%edx
-    646c60e4:	mov    $0xb,%ecx
-    646c60e9:	call   646c7958 <signal>
-    646c60ee:	cmp    $0x1,%rax
-    646c60f2:	je     646c6249 <_gnu_exception_handler+0x1b9>
-    646c60f8:	test   %rax,%rax
-    646c60fb:	jne    646c6210 <_gnu_exception_handler+0x180>
-    646c6101:	mov    0x6718(%rip),%rax        # 646cc820 <__mingw_oldexcpt_handler>
-    646c6108:	test   %rax,%rax
-    646c610b:	je     646c6221 <_gnu_exception_handler+0x191>
-    646c6111:	mov    %rbx,%rcx
-    646c6114:	add    $0x20,%rsp
-    646c6118:	pop    %rbx
-    646c6119:	rex.W jmp *%rax
-    646c611c:	nopl   0x0(%rax)
-    646c6120:	cmp    $0xc0000094,%eax
-    646c6125:	je     646c61e0 <_gnu_exception_handler+0x150>
-    646c612b:	ja     646c6185 <_gnu_exception_handler+0xf5>
-    646c612d:	cmp    $0xc0000092,%eax
-    646c6132:	je     646c617a <_gnu_exception_handler+0xea>
-    646c6134:	cmp    $0xc0000093,%eax
-    646c6139:	jne    646c6101 <_gnu_exception_handler+0x71>
-    646c613b:	xor    %edx,%edx
-    646c613d:	mov    $0x8,%ecx
-    646c6142:	call   646c7958 <signal>
-    646c6147:	cmp    $0x1,%rax
-    646c614b:	je     646c6230 <_gnu_exception_handler+0x1a0>
-    646c6151:	test   %rax,%rax
-    646c6154:	je     646c6101 <_gnu_exception_handler+0x71>
-    646c6156:	mov    $0x8,%ecx
-    646c615b:	call   *%rax
-    646c615d:	mov    $0xffffffff,%eax
-    646c6162:	add    $0x20,%rsp
-    646c6166:	pop    %rbx
-    646c6167:	ret
+00000000646c5890 <_decode_pointer>:
+    646c5890:	mov    %rcx,%rax
+    646c5893:	ret
+    646c5894:	xchg   %ax,%ax
+    646c5896:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c58a0 <_encode_pointer>:
+    646c58a0:	mov    %rcx,%rax
+    646c58a3:	ret
+    646c58a4:	nop
+    646c58a5:	nop
+    646c58a6:	nop
+    646c58a7:	nop
+    646c58a8:	nop
+    646c58a9:	nop
+    646c58aa:	nop
+    646c58ab:	nop
+    646c58ac:	nop
+    646c58ad:	nop
+    646c58ae:	nop
+    646c58af:	nop
+
+00000000646c58b0 <__write_memory.part.0>:
+    646c58b0:	push   %r12
+    646c58b2:	push   %rbp
+    646c58b3:	push   %rdi
+    646c58b4:	push   %rsi
+    646c58b5:	push   %rbx
+    646c58b6:	sub    $0x50,%rsp
+    646c58ba:	movslq 0x6f23(%rip),%rsi        # 646cc7e4 <maxSections>
+    646c58c1:	test   %esi,%esi
+    646c58c3:	mov    %rcx,%rbx
+    646c58c6:	mov    %rdx,%rbp
+    646c58c9:	mov    %r8,%rdi
+    646c58cc:	jle    646c5a38 <__write_memory.part.0+0x188>
+    646c58d2:	mov    0x6f0f(%rip),%rax        # 646cc7e8 <the_secs>
+    646c58d9:	xor    %ecx,%ecx
+    646c58db:	add    $0x18,%rax
+    646c58df:	nop
+    646c58e0:	mov    (%rax),%rdx
+    646c58e3:	cmp    %rdx,%rbx
+    646c58e6:	jb     646c58fc <__write_memory.part.0+0x4c>
+    646c58e8:	mov    0x8(%rax),%r8
+    646c58ec:	mov    0x8(%r8),%r8d
+    646c58f0:	add    %r8,%rdx
+    646c58f3:	cmp    %rdx,%rbx
+    646c58f6:	jb     646c5985 <__write_memory.part.0+0xd5>
+    646c58fc:	add    $0x1,%ecx
+    646c58ff:	add    $0x28,%rax
+    646c5903:	cmp    %esi,%ecx
+    646c5905:	jne    646c58e0 <__write_memory.part.0+0x30>
+    646c5907:	mov    %rbx,%rcx
+    646c590a:	call   646c6550 <__mingw_GetSectionForAddress>
+    646c590f:	test   %rax,%rax
+    646c5912:	mov    %rax,%r12
+    646c5915:	je     646c5a6d <__write_memory.part.0+0x1bd>
+    646c591b:	mov    0x6ec6(%rip),%rax        # 646cc7e8 <the_secs>
+    646c5922:	lea    (%rsi,%rsi,4),%rsi
+    646c5926:	shl    $0x3,%rsi
+    646c592a:	add    %rsi,%rax
+    646c592d:	mov    %r12,0x20(%rax)
+    646c5931:	movl   $0x0,(%rax)
+    646c5937:	call   646c6680 <_GetPEImageBase>
+    646c593c:	mov    0xc(%r12),%ecx
+    646c5941:	lea    0x20(%rsp),%rdx
+    646c5946:	mov    $0x30,%r8d
+    646c594c:	add    %rax,%rcx
+    646c594f:	mov    0x6e92(%rip),%rax        # 646cc7e8 <the_secs>
+    646c5956:	mov    %rcx,0x18(%rax,%rsi,1)
+    646c595b:	call   *0x8913(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c5961:	test   %rax,%rax
+    646c5964:	je     646c5a50 <__write_memory.part.0+0x1a0>
+    646c596a:	mov    0x44(%rsp),%eax
+    646c596e:	lea    -0x4(%rax),%edx
+    646c5971:	and    $0xfffffffb,%edx
+    646c5974:	je     646c597e <__write_memory.part.0+0xce>
+    646c5976:	sub    $0x40,%eax
+    646c5979:	and    $0xffffffbf,%eax
+    646c597c:	jne    646c59e0 <__write_memory.part.0+0x130>
+    646c597e:	addl   $0x1,0x6e5f(%rip)        # 646cc7e4 <maxSections>
+    646c5985:	cmp    $0x8,%edi
+    646c5988:	jae    646c59b3 <__write_memory.part.0+0x103>
+    646c598a:	test   $0x4,%dil
+    646c598e:	jne    646c5a24 <__write_memory.part.0+0x174>
+    646c5994:	test   %edi,%edi
+    646c5996:	je     646c59a8 <__write_memory.part.0+0xf8>
+    646c5998:	movzbl 0x0(%rbp),%eax
+    646c599c:	test   $0x2,%dil
+    646c59a0:	mov    %al,(%rbx)
+    646c59a2:	jne    646c5a3f <__write_memory.part.0+0x18f>
+    646c59a8:	add    $0x50,%rsp
+    646c59ac:	pop    %rbx
+    646c59ad:	pop    %rsi
+    646c59ae:	pop    %rdi
+    646c59af:	pop    %rbp
+    646c59b0:	pop    %r12
+    646c59b2:	ret
+    646c59b3:	mov    %edi,%eax
+    646c59b5:	sub    $0x1,%edi
+    646c59b8:	mov    -0x8(%rbp,%rax,1),%rdx
+    646c59bd:	cmp    $0x8,%edi
+    646c59c0:	mov    %rdx,-0x8(%rbx,%rax,1)
+    646c59c5:	jb     646c59a8 <__write_memory.part.0+0xf8>
+    646c59c7:	and    $0xfffffff8,%edi
+    646c59ca:	xor    %eax,%eax
+    646c59cc:	mov    %eax,%edx
+    646c59ce:	add    $0x8,%eax
+    646c59d1:	mov    0x0(%rbp,%rdx,1),%rcx
+    646c59d6:	cmp    %edi,%eax
+    646c59d8:	mov    %rcx,(%rbx,%rdx,1)
+    646c59dc:	jb     646c59cc <__write_memory.part.0+0x11c>
+    646c59de:	jmp    646c59a8 <__write_memory.part.0+0xf8>
+    646c59e0:	add    0x6e01(%rip),%rsi        # 646cc7e8 <the_secs>
+    646c59e7:	mov    $0x40,%r8d
+    646c59ed:	mov    0x20(%rsp),%rcx
+    646c59f2:	mov    0x38(%rsp),%rdx
+    646c59f7:	mov    %rsi,%r9
+    646c59fa:	mov    %rcx,0x8(%rsi)
+    646c59fe:	mov    %rdx,0x10(%rsi)
+    646c5a02:	call   *0x8864(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c5a08:	test   %eax,%eax
+    646c5a0a:	jne    646c597e <__write_memory.part.0+0xce>
+    646c5a10:	call   *0x87de(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c5a16:	lea    0x395b(%rip),%rcx        # 646c9378 <.rdata+0x78>
+    646c5a1d:	mov    %eax,%edx
+    646c5a1f:	call   646c7d00 <__report_error>
+    646c5a24:	mov    0x0(%rbp),%eax
+    646c5a27:	mov    %edi,%edi
+    646c5a29:	mov    %eax,(%rbx)
+    646c5a2b:	mov    -0x4(%rbp,%rdi,1),%eax
+    646c5a2f:	mov    %eax,-0x4(%rbx,%rdi,1)
+    646c5a33:	jmp    646c59a8 <__write_memory.part.0+0xf8>
+    646c5a38:	xor    %esi,%esi
+    646c5a3a:	jmp    646c5907 <__write_memory.part.0+0x57>
+    646c5a3f:	mov    %edi,%edi
+    646c5a41:	movzwl -0x2(%rbp,%rdi,1),%eax
+    646c5a46:	mov    %ax,-0x2(%rbx,%rdi,1)
+    646c5a4b:	jmp    646c59a8 <__write_memory.part.0+0xf8>
+    646c5a50:	mov    0x6d91(%rip),%rax        # 646cc7e8 <the_secs>
+    646c5a57:	lea    0x38e2(%rip),%rcx        # 646c9340 <.rdata+0x40>
+    646c5a5e:	mov    0x8(%r12),%edx
+    646c5a63:	mov    0x18(%rax,%rsi,1),%r8
+    646c5a68:	call   646c7d00 <__report_error>
+    646c5a6d:	lea    0x38ac(%rip),%rcx        # 646c9320 <.rdata+0x20>
+    646c5a74:	mov    %rbx,%rdx
+    646c5a77:	call   646c7d00 <__report_error>
+    646c5a7c:	nop
+    646c5a7d:	nopl   (%rax)
+
+00000000646c5a80 <_pei386_runtime_relocator>:
+    646c5a80:	push   %rbp
+    646c5a81:	push   %r15
+    646c5a83:	push   %r14
+    646c5a85:	push   %r13
+    646c5a87:	push   %r12
+    646c5a89:	push   %rdi
+    646c5a8a:	push   %rsi
+    646c5a8b:	push   %rbx
+    646c5a8c:	sub    $0x38,%rsp
+    646c5a90:	lea    0x80(%rsp),%rbp
+    646c5a98:	mov    0x6d42(%rip),%ebx        # 646cc7e0 <was_init.95174>
+    646c5a9e:	test   %ebx,%ebx
+    646c5aa0:	je     646c5ab3 <_pei386_runtime_relocator+0x33>
+    646c5aa2:	lea    -0x48(%rbp),%rsp
+    646c5aa6:	pop    %rbx
+    646c5aa7:	pop    %rsi
+    646c5aa8:	pop    %rdi
+    646c5aa9:	pop    %r12
+    646c5aab:	pop    %r13
+    646c5aad:	pop    %r14
+    646c5aaf:	pop    %r15
+    646c5ab1:	pop    %rbp
+    646c5ab2:	ret
+    646c5ab3:	movl   $0x1,0x6d23(%rip)        # 646cc7e0 <was_init.95174>
+    646c5abd:	call   646c65d0 <__mingw_GetSectionCount>
+    646c5ac2:	cltq
+    646c5ac4:	lea    (%rax,%rax,4),%rax
+    646c5ac8:	lea    0x1e(,%rax,8),%rax
+    646c5ad0:	and    $0xfffffffffffffff0,%rax
+    646c5ad4:	call   646c6820 <___chkstk_ms>
+    646c5ad9:	mov    0x3c10(%rip),%r12        # 646c96f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+    646c5ae0:	movl   $0x0,0x6cfa(%rip)        # 646cc7e4 <maxSections>
+    646c5aea:	mov    0x3c0f(%rip),%rsi        # 646c9700 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+    646c5af1:	sub    %rax,%rsp
+    646c5af4:	lea    0x20(%rsp),%rax
+    646c5af9:	mov    %rax,0x6ce8(%rip)        # 646cc7e8 <the_secs>
+    646c5b00:	mov    %r12,%rax
+    646c5b03:	sub    %rsi,%rax
+    646c5b06:	cmp    $0x7,%rax
+    646c5b0a:	jle    646c5aa2 <_pei386_runtime_relocator+0x22>
+    646c5b0c:	cmp    $0xb,%rax
+    646c5b10:	mov    (%rsi),%edx
+    646c5b12:	jle    646c5be0 <_pei386_runtime_relocator+0x160>
+    646c5b18:	test   %edx,%edx
+    646c5b1a:	je     646c5bc4 <_pei386_runtime_relocator+0x144>
+    646c5b20:	cmp    %r12,%rsi
+    646c5b23:	jae    646c5aa2 <_pei386_runtime_relocator+0x22>
+    646c5b29:	lea    0x8(%rsi),%r14
+    646c5b2d:	add    $0x7,%r12
+    646c5b31:	mov    0x3be8(%rip),%r13        # 646c9720 <.refptr.__image_base__>
+    646c5b38:	lea    -0x58(%rbp),%rdi
+    646c5b3c:	sub    %r14,%r12
+    646c5b3f:	shr    $0x3,%r12
+    646c5b43:	lea    0x8(%rsi,%r12,8),%r12
+    646c5b48:	jmp    646c5b54 <_pei386_runtime_relocator+0xd4>
+    646c5b4a:	nopw   0x0(%rax,%rax,1)
+    646c5b50:	add    $0x8,%r14
+    646c5b54:	mov    0x4(%rsi),%ecx
+    646c5b57:	mov    $0x4,%r8d
+    646c5b5d:	mov    %rdi,%rdx
+    646c5b60:	mov    (%rsi),%eax
+    646c5b62:	mov    %r14,%rsi
+    646c5b65:	add    %r13,%rcx
+    646c5b68:	add    (%rcx),%eax
+    646c5b6a:	mov    %eax,-0x58(%rbp)
+    646c5b6d:	call   646c58b0 <__write_memory.part.0>
+    646c5b72:	cmp    %r12,%r14
+    646c5b75:	jne    646c5b50 <_pei386_runtime_relocator+0xd0>
+    646c5b77:	mov    0x6c67(%rip),%eax        # 646cc7e4 <maxSections>
+    646c5b7d:	xor    %esi,%esi
+    646c5b7f:	mov    0x86e6(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
+    646c5b86:	test   %eax,%eax
+    646c5b88:	jle    646c5aa2 <_pei386_runtime_relocator+0x22>
+    646c5b8e:	xchg   %ax,%ax
+    646c5b90:	mov    0x6c51(%rip),%rax        # 646cc7e8 <the_secs>
+    646c5b97:	add    %rsi,%rax
+    646c5b9a:	mov    (%rax),%r8d
+    646c5b9d:	test   %r8d,%r8d
+    646c5ba0:	je     646c5bb0 <_pei386_runtime_relocator+0x130>
+    646c5ba2:	mov    0x10(%rax),%rdx
+    646c5ba6:	mov    %rdi,%r9
+    646c5ba9:	mov    0x8(%rax),%rcx
+    646c5bad:	call   *%r12
+    646c5bb0:	add    $0x1,%ebx
+    646c5bb3:	add    $0x28,%rsi
+    646c5bb7:	cmp    0x6c27(%rip),%ebx        # 646cc7e4 <maxSections>
+    646c5bbd:	jl     646c5b90 <_pei386_runtime_relocator+0x110>
+    646c5bbf:	jmp    646c5aa2 <_pei386_runtime_relocator+0x22>
+    646c5bc4:	mov    0x4(%rsi),%ecx
+    646c5bc7:	test   %ecx,%ecx
+    646c5bc9:	jne    646c5b20 <_pei386_runtime_relocator+0xa0>
+    646c5bcf:	mov    0x8(%rsi),%edx
+    646c5bd2:	test   %edx,%edx
+    646c5bd4:	jne    646c5bf3 <_pei386_runtime_relocator+0x173>
+    646c5bd6:	mov    0xc(%rsi),%edx
+    646c5bd9:	add    $0xc,%rsi
+    646c5bdd:	nopl   (%rax)
+    646c5be0:	test   %edx,%edx
+    646c5be2:	jne    646c5b20 <_pei386_runtime_relocator+0xa0>
+    646c5be8:	mov    0x4(%rsi),%eax
+    646c5beb:	test   %eax,%eax
+    646c5bed:	jne    646c5b20 <_pei386_runtime_relocator+0xa0>
+    646c5bf3:	mov    0x8(%rsi),%edx
+    646c5bf6:	cmp    $0x1,%edx
+    646c5bf9:	jne    646c5d2e <_pei386_runtime_relocator+0x2ae>
+    646c5bff:	mov    0x3b1a(%rip),%r13        # 646c9720 <.refptr.__image_base__>
+    646c5c06:	add    $0xc,%rsi
+    646c5c0a:	movabs $0xffffffff00000000,%r15
+    646c5c14:	lea    -0x58(%rbp),%r14
+    646c5c18:	cmp    %r12,%rsi
+    646c5c1b:	jb     646c5c65 <_pei386_runtime_relocator+0x1e5>
+    646c5c1d:	jmp    646c5aa2 <_pei386_runtime_relocator+0x22>
+    646c5c22:	jbe    646c5ce0 <_pei386_runtime_relocator+0x260>
+    646c5c28:	cmp    $0x20,%edx
+    646c5c2b:	je     646c5cb0 <_pei386_runtime_relocator+0x230>
+    646c5c31:	cmp    $0x40,%edx
+    646c5c34:	jne    646c5d1a <_pei386_runtime_relocator+0x29a>
+    646c5c3a:	mov    (%rcx),%rdx
+    646c5c3d:	mov    $0x8,%r8d
+    646c5c43:	mov    %r14,%rdi
+    646c5c46:	sub    %rax,%rdx
+    646c5c49:	add    %r9,%rdx
+    646c5c4c:	mov    %rdx,-0x58(%rbp)
+    646c5c50:	mov    %r14,%rdx
+    646c5c53:	call   646c58b0 <__write_memory.part.0>
+    646c5c58:	add    $0xc,%rsi
+    646c5c5c:	cmp    %r12,%rsi
+    646c5c5f:	jae    646c5b77 <_pei386_runtime_relocator+0xf7>
+    646c5c65:	mov    0x4(%rsi),%ecx
+    646c5c68:	mov    (%rsi),%eax
+    646c5c6a:	movzbl 0x8(%rsi),%edx
+    646c5c6e:	add    %r13,%rcx
+    646c5c71:	add    %r13,%rax
+    646c5c74:	cmp    $0x10,%edx
+    646c5c77:	mov    (%rax),%r9
+    646c5c7a:	jne    646c5c22 <_pei386_runtime_relocator+0x1a2>
+    646c5c7c:	movzwl (%rcx),%r8d
+    646c5c80:	mov    %r14,%rdx
+    646c5c83:	mov    %r14,%rdi
+    646c5c86:	mov    %r8,%r10
+    646c5c89:	or     $0xffffffffffff0000,%r10
+    646c5c90:	test   %r8w,%r8w
+    646c5c94:	cmovs  %r10,%r8
+    646c5c98:	sub    %rax,%r8
+    646c5c9b:	add    %r9,%r8
+    646c5c9e:	mov    %r8,-0x58(%rbp)
+    646c5ca2:	mov    $0x2,%r8d
+    646c5ca8:	call   646c58b0 <__write_memory.part.0>
+    646c5cad:	jmp    646c5c58 <_pei386_runtime_relocator+0x1d8>
+    646c5caf:	nop
+    646c5cb0:	mov    (%rcx),%edx
+    646c5cb2:	mov    %r14,%rdi
+    646c5cb5:	mov    %rdx,%r8
+    646c5cb8:	or     %r15,%rdx
+    646c5cbb:	test   %r8d,%r8d
+    646c5cbe:	cmovns %r8,%rdx
+    646c5cc2:	mov    $0x4,%r8d
+    646c5cc8:	sub    %rax,%rdx
+    646c5ccb:	add    %r9,%rdx
+    646c5cce:	mov    %rdx,-0x58(%rbp)
+    646c5cd2:	mov    %r14,%rdx
+    646c5cd5:	call   646c58b0 <__write_memory.part.0>
+    646c5cda:	jmp    646c5c58 <_pei386_runtime_relocator+0x1d8>
+    646c5cdf:	nop
+    646c5ce0:	cmp    $0x8,%edx
+    646c5ce3:	jne    646c5d1a <_pei386_runtime_relocator+0x29a>
+    646c5ce5:	movzbl (%rcx),%r8d
+    646c5ce9:	mov    %r14,%rdx
+    646c5cec:	mov    %r14,%rdi
+    646c5cef:	mov    %r8,%r10
+    646c5cf2:	or     $0xffffffffffffff00,%r10
+    646c5cf9:	test   %r8b,%r8b
+    646c5cfc:	cmovs  %r10,%r8
+    646c5d00:	sub    %rax,%r8
+    646c5d03:	add    %r9,%r8
+    646c5d06:	mov    %r8,-0x58(%rbp)
+    646c5d0a:	mov    $0x1,%r8d
+    646c5d10:	call   646c58b0 <__write_memory.part.0>
+    646c5d15:	jmp    646c5c58 <_pei386_runtime_relocator+0x1d8>
+    646c5d1a:	lea    0x36b7(%rip),%rcx        # 646c93d8 <.rdata+0xd8>
+    646c5d21:	movq   $0x0,-0x58(%rbp)
+    646c5d29:	call   646c7d00 <__report_error>
+    646c5d2e:	lea    0x366b(%rip),%rcx        # 646c93a0 <.rdata+0xa0>
+    646c5d35:	call   646c7d00 <__report_error>
+    646c5d3a:	nop
+    646c5d3b:	nop
+    646c5d3c:	nop
+    646c5d3d:	nop
+    646c5d3e:	nop
+    646c5d3f:	nop
+
+00000000646c5d40 <__mingw_SEH_error_handler>:
+    646c5d40:	sub    $0x28,%rsp
+    646c5d44:	mov    (%rcx),%eax
+    646c5d46:	cmp    $0xc0000091,%eax
+    646c5d4b:	ja     646c5db0 <__mingw_SEH_error_handler+0x70>
+    646c5d4d:	cmp    $0xc000008d,%eax
+    646c5d52:	jae    646c5dcf <__mingw_SEH_error_handler+0x8f>
+    646c5d54:	cmp    $0xc0000008,%eax
+    646c5d59:	je     646c5e64 <__mingw_SEH_error_handler+0x124>
+    646c5d5f:	ja     646c5e30 <__mingw_SEH_error_handler+0xf0>
+    646c5d65:	cmp    $0x80000002,%eax
+    646c5d6a:	je     646c5e64 <__mingw_SEH_error_handler+0x124>
+    646c5d70:	cmp    $0xc0000005,%eax
+    646c5d75:	jne    646c5e3e <__mingw_SEH_error_handler+0xfe>
+    646c5d7b:	xor    %edx,%edx
+    646c5d7d:	mov    $0xb,%ecx
+    646c5d82:	call   646c7898 <signal>
+    646c5d87:	cmp    $0x1,%rax
+    646c5d8b:	je     646c5ec0 <__mingw_SEH_error_handler+0x180>
+    646c5d91:	test   %rax,%rax
+    646c5d94:	je     646c5ed6 <__mingw_SEH_error_handler+0x196>
+    646c5d9a:	mov    $0xb,%ecx
+    646c5d9f:	call   *%rax
+    646c5da1:	xor    %eax,%eax
+    646c5da3:	add    $0x28,%rsp
+    646c5da7:	ret
+    646c5da8:	nopl   0x0(%rax,%rax,1)
+    646c5db0:	cmp    $0xc0000094,%eax
+    646c5db5:	je     646c5e70 <__mingw_SEH_error_handler+0x130>
+    646c5dbb:	ja     646c5df4 <__mingw_SEH_error_handler+0xb4>
+    646c5dbd:	cmp    $0xc0000092,%eax
+    646c5dc2:	je     646c5e64 <__mingw_SEH_error_handler+0x124>
+    646c5dc8:	cmp    $0xc0000093,%eax
+    646c5dcd:	jne    646c5e3e <__mingw_SEH_error_handler+0xfe>
+    646c5dcf:	xor    %edx,%edx
+    646c5dd1:	mov    $0x8,%ecx
+    646c5dd6:	call   646c7898 <signal>
+    646c5ddb:	cmp    $0x1,%rax
+    646c5ddf:	je     646c5e50 <__mingw_SEH_error_handler+0x110>
+    646c5de1:	test   %rax,%rax
+    646c5de4:	je     646c5e3e <__mingw_SEH_error_handler+0xfe>
+    646c5de6:	mov    $0x8,%ecx
+    646c5deb:	call   *%rax
+    646c5ded:	xor    %eax,%eax
+    646c5def:	add    $0x28,%rsp
+    646c5df3:	ret
+    646c5df4:	cmp    $0xc0000095,%eax
+    646c5df9:	je     646c5e64 <__mingw_SEH_error_handler+0x124>
+    646c5dfb:	cmp    $0xc0000096,%eax
+    646c5e00:	jne    646c5e3e <__mingw_SEH_error_handler+0xfe>
+    646c5e02:	xor    %edx,%edx
+    646c5e04:	mov    $0x4,%ecx
+    646c5e09:	call   646c7898 <signal>
+    646c5e0e:	cmp    $0x1,%rax
+    646c5e12:	je     646c5ea0 <__mingw_SEH_error_handler+0x160>
+    646c5e18:	test   %rax,%rax
+    646c5e1b:	je     646c5ed6 <__mingw_SEH_error_handler+0x196>
+    646c5e21:	mov    $0x4,%ecx
+    646c5e26:	call   *%rax
+    646c5e28:	xor    %eax,%eax
+    646c5e2a:	add    $0x28,%rsp
+    646c5e2e:	ret
+    646c5e2f:	nop
+    646c5e30:	cmp    $0xc000001d,%eax
+    646c5e35:	je     646c5e02 <__mingw_SEH_error_handler+0xc2>
+    646c5e37:	cmp    $0xc000008c,%eax
+    646c5e3c:	je     646c5e64 <__mingw_SEH_error_handler+0x124>
+    646c5e3e:	mov    $0x1,%eax
+    646c5e43:	add    $0x28,%rsp
+    646c5e47:	ret
+    646c5e48:	nopl   0x0(%rax,%rax,1)
+    646c5e50:	mov    $0x1,%edx
+    646c5e55:	mov    $0x8,%ecx
+    646c5e5a:	call   646c7898 <signal>
+    646c5e5f:	call   646c6810 <_fpreset>
+    646c5e64:	xor    %eax,%eax
+    646c5e66:	add    $0x28,%rsp
+    646c5e6a:	ret
+    646c5e6b:	nopl   0x0(%rax,%rax,1)
+    646c5e70:	xor    %edx,%edx
+    646c5e72:	mov    $0x8,%ecx
+    646c5e77:	call   646c7898 <signal>
+    646c5e7c:	cmp    $0x1,%rax
+    646c5e80:	jne    646c5de1 <__mingw_SEH_error_handler+0xa1>
+    646c5e86:	mov    $0x1,%edx
+    646c5e8b:	mov    $0x8,%ecx
+    646c5e90:	call   646c7898 <signal>
+    646c5e95:	xor    %eax,%eax
+    646c5e97:	jmp    646c5da3 <__mingw_SEH_error_handler+0x63>
+    646c5e9c:	nopl   0x0(%rax)
+    646c5ea0:	mov    $0x1,%edx
+    646c5ea5:	mov    $0x4,%ecx
+    646c5eaa:	call   646c7898 <signal>
+    646c5eaf:	xor    %eax,%eax
+    646c5eb1:	jmp    646c5da3 <__mingw_SEH_error_handler+0x63>
+    646c5eb6:	cs nopw 0x0(%rax,%rax,1)
+    646c5ec0:	mov    $0x1,%edx
+    646c5ec5:	mov    $0xb,%ecx
+    646c5eca:	call   646c7898 <signal>
+    646c5ecf:	xor    %eax,%eax
+    646c5ed1:	jmp    646c5da3 <__mingw_SEH_error_handler+0x63>
+    646c5ed6:	mov    $0x4,%eax
+    646c5edb:	jmp    646c5da3 <__mingw_SEH_error_handler+0x63>
+
+00000000646c5ee0 <__mingw_init_ehandler>:
+    646c5ee0:	push   %r12
+    646c5ee2:	push   %rbp
+    646c5ee3:	push   %rdi
+    646c5ee4:	push   %rsi
+    646c5ee5:	push   %rbx
+    646c5ee6:	sub    $0x20,%rsp
+    646c5eea:	call   646c6680 <_GetPEImageBase>
+    646c5eef:	mov    %rax,%rbp
+    646c5ef2:	mov    0x6910(%rip),%eax        # 646cc808 <was_here.95013>
+    646c5ef8:	test   %eax,%eax
+    646c5efa:	jne    646c5f21 <__mingw_init_ehandler+0x41>
+    646c5efc:	test   %rbp,%rbp
+    646c5eff:	je     646c5f21 <__mingw_init_ehandler+0x41>
+    646c5f01:	lea    0x3508(%rip),%rcx        # 646c9410 <.rdata>
+    646c5f08:	movl   $0x1,0x68f6(%rip)        # 646cc808 <was_here.95013>
+    646c5f12:	call   646c64c0 <_FindPESectionByName>
+    646c5f17:	test   %rax,%rax
+    646c5f1a:	je     646c5f30 <__mingw_init_ehandler+0x50>
+    646c5f1c:	mov    $0x1,%eax
+    646c5f21:	add    $0x20,%rsp
+    646c5f25:	pop    %rbx
+    646c5f26:	pop    %rsi
+    646c5f27:	pop    %rdi
+    646c5f28:	pop    %rbp
+    646c5f29:	pop    %r12
+    646c5f2b:	ret
+    646c5f2c:	nopl   0x0(%rax)
+    646c5f30:	lea    0x69e9(%rip),%rbx        # 646cc920 <emu_pdata>
+    646c5f37:	mov    $0x30,%ecx
+    646c5f3c:	xor    %esi,%esi
+    646c5f3e:	lea    0x68db(%rip),%rdx        # 646cc820 <emu_xdata>
+    646c5f45:	mov    %rbx,%rdi
+    646c5f48:	rep stos %rax,%es:(%rdi)
+    646c5f4b:	lea    -0x212(%rip),%r12        # 646c5d40 <__mingw_SEH_error_handler>
+    646c5f52:	mov    $0x20,%ecx
+    646c5f57:	mov    %rdx,%rdi
+    646c5f5a:	rep stos %rax,%es:(%rdi)
+    646c5f5d:	sub    %rbp,%r12
+    646c5f60:	mov    %rdx,%rdi
+    646c5f63:	jmp    646c5f93 <__mingw_init_ehandler+0xb3>
+    646c5f65:	movb   $0x9,(%rdi)
+    646c5f68:	add    $0x1,%rsi
+    646c5f6c:	add    $0xc,%rbx
+    646c5f70:	mov    %r12d,0x4(%rdi)
+    646c5f74:	mov    0xc(%rax),%ecx
+    646c5f77:	mov    %ecx,-0xc(%rbx)
+    646c5f7a:	add    0x8(%rax),%ecx
+    646c5f7d:	mov    %rdi,%rax
+    646c5f80:	add    $0x8,%rdi
+    646c5f84:	sub    %rbp,%rax
+    646c5f87:	mov    %eax,-0x4(%rbx)
+    646c5f8a:	mov    %ecx,-0x8(%rbx)
+    646c5f8d:	cmp    $0x20,%rsi
+    646c5f91:	je     646c5fc5 <__mingw_init_ehandler+0xe5>
+    646c5f93:	mov    %rsi,%rcx
+    646c5f96:	call   646c6610 <_FindPESectionExec>
+    646c5f9b:	test   %rax,%rax
+    646c5f9e:	jne    646c5f65 <__mingw_init_ehandler+0x85>
+    646c5fa0:	test   %rsi,%rsi
+    646c5fa3:	mov    %esi,%edx
+    646c5fa5:	je     646c5f1c <__mingw_init_ehandler+0x3c>
+    646c5fab:	nopl   0x0(%rax,%rax,1)
+    646c5fb0:	lea    0x6969(%rip),%rcx        # 646cc920 <emu_pdata>
+    646c5fb7:	mov    %rbp,%r8
+    646c5fba:	call   *0x8264(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c5fc0:	jmp    646c5f1c <__mingw_init_ehandler+0x3c>
+    646c5fc5:	mov    $0x20,%edx
+    646c5fca:	jmp    646c5fb0 <__mingw_init_ehandler+0xd0>
+    646c5fcc:	nopl   0x0(%rax)
+
+00000000646c5fd0 <_gnu_exception_handler>:
+    646c5fd0:	push   %rbx
+    646c5fd1:	sub    $0x20,%rsp
+    646c5fd5:	mov    (%rcx),%rdx
+    646c5fd8:	mov    (%rdx),%eax
+    646c5fda:	mov    %rcx,%rbx
+    646c5fdd:	mov    %eax,%ecx
+    646c5fdf:	and    $0x20ffffff,%ecx
+    646c5fe5:	cmp    $0x20474343,%ecx
+    646c5feb:	je     646c60b0 <_gnu_exception_handler+0xe0>
+    646c5ff1:	cmp    $0xc0000091,%eax
+    646c5ff6:	ja     646c6060 <_gnu_exception_handler+0x90>
+    646c5ff8:	cmp    $0xc000008d,%eax
+    646c5ffd:	jae    646c607b <_gnu_exception_handler+0xab>
+    646c5fff:	cmp    $0xc0000008,%eax
+    646c6004:	je     646c60ba <_gnu_exception_handler+0xea>
+    646c600a:	ja     646c6104 <_gnu_exception_handler+0x134>
+    646c6010:	cmp    $0x80000002,%eax
+    646c6015:	je     646c60ba <_gnu_exception_handler+0xea>
+    646c601b:	cmp    $0xc0000005,%eax
+    646c6020:	jne    646c6041 <_gnu_exception_handler+0x71>
+    646c6022:	xor    %edx,%edx
+    646c6024:	mov    $0xb,%ecx
+    646c6029:	call   646c7898 <signal>
+    646c602e:	cmp    $0x1,%rax
+    646c6032:	je     646c6189 <_gnu_exception_handler+0x1b9>
+    646c6038:	test   %rax,%rax
+    646c603b:	jne    646c6150 <_gnu_exception_handler+0x180>
+    646c6041:	mov    0x67b8(%rip),%rax        # 646cc800 <__mingw_oldexcpt_handler>
+    646c6048:	test   %rax,%rax
+    646c604b:	je     646c6161 <_gnu_exception_handler+0x191>
+    646c6051:	mov    %rbx,%rcx
+    646c6054:	add    $0x20,%rsp
+    646c6058:	pop    %rbx
+    646c6059:	rex.W jmp *%rax
+    646c605c:	nopl   0x0(%rax)
+    646c6060:	cmp    $0xc0000094,%eax
+    646c6065:	je     646c6120 <_gnu_exception_handler+0x150>
+    646c606b:	ja     646c60c5 <_gnu_exception_handler+0xf5>
+    646c606d:	cmp    $0xc0000092,%eax
+    646c6072:	je     646c60ba <_gnu_exception_handler+0xea>
+    646c6074:	cmp    $0xc0000093,%eax
+    646c6079:	jne    646c6041 <_gnu_exception_handler+0x71>
+    646c607b:	xor    %edx,%edx
+    646c607d:	mov    $0x8,%ecx
+    646c6082:	call   646c7898 <signal>
+    646c6087:	cmp    $0x1,%rax
+    646c608b:	je     646c6170 <_gnu_exception_handler+0x1a0>
+    646c6091:	test   %rax,%rax
+    646c6094:	je     646c6041 <_gnu_exception_handler+0x71>
+    646c6096:	mov    $0x8,%ecx
+    646c609b:	call   *%rax
+    646c609d:	mov    $0xffffffff,%eax
+    646c60a2:	add    $0x20,%rsp
+    646c60a6:	pop    %rbx
+    646c60a7:	ret
+    646c60a8:	nopl   0x0(%rax,%rax,1)
+    646c60b0:	testb  $0x1,0x4(%rdx)
+    646c60b4:	jne    646c5ff1 <_gnu_exception_handler+0x21>
+    646c60ba:	mov    $0xffffffff,%eax
+    646c60bf:	add    $0x20,%rsp
+    646c60c3:	pop    %rbx
+    646c60c4:	ret
+    646c60c5:	cmp    $0xc0000095,%eax
+    646c60ca:	je     646c60ba <_gnu_exception_handler+0xea>
+    646c60cc:	cmp    $0xc0000096,%eax
+    646c60d1:	jne    646c6041 <_gnu_exception_handler+0x71>
+    646c60d7:	xor    %edx,%edx
+    646c60d9:	mov    $0x4,%ecx
+    646c60de:	call   646c7898 <signal>
+    646c60e3:	cmp    $0x1,%rax
+    646c60e7:	je     646c61a0 <_gnu_exception_handler+0x1d0>
+    646c60ed:	test   %rax,%rax
+    646c60f0:	je     646c6041 <_gnu_exception_handler+0x71>
+    646c60f6:	mov    $0x4,%ecx
+    646c60fb:	call   *%rax
+    646c60fd:	mov    $0xffffffff,%eax
+    646c6102:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
+    646c6104:	cmp    $0xc000001d,%eax
+    646c6109:	je     646c60d7 <_gnu_exception_handler+0x107>
+    646c610b:	cmp    $0xc000008c,%eax
+    646c6110:	jne    646c6041 <_gnu_exception_handler+0x71>
+    646c6116:	jmp    646c60ba <_gnu_exception_handler+0xea>
+    646c6118:	nopl   0x0(%rax,%rax,1)
+    646c6120:	xor    %edx,%edx
+    646c6122:	mov    $0x8,%ecx
+    646c6127:	call   646c7898 <signal>
+    646c612c:	cmp    $0x1,%rax
+    646c6130:	jne    646c6091 <_gnu_exception_handler+0xc1>
+    646c6136:	mov    $0x1,%edx
+    646c613b:	mov    $0x8,%ecx
+    646c6140:	call   646c7898 <signal>
+    646c6145:	mov    $0xffffffff,%eax
+    646c614a:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
+    646c614f:	nop
+    646c6150:	mov    $0xb,%ecx
+    646c6155:	call   *%rax
+    646c6157:	mov    $0xffffffff,%eax
+    646c615c:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
+    646c6161:	xor    %eax,%eax
+    646c6163:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
     646c6168:	nopl   0x0(%rax,%rax,1)
-    646c6170:	testb  $0x1,0x4(%rdx)
-    646c6174:	jne    646c60b1 <_gnu_exception_handler+0x21>
-    646c617a:	mov    $0xffffffff,%eax
-    646c617f:	add    $0x20,%rsp
-    646c6183:	pop    %rbx
-    646c6184:	ret
-    646c6185:	cmp    $0xc0000095,%eax
-    646c618a:	je     646c617a <_gnu_exception_handler+0xea>
-    646c618c:	cmp    $0xc0000096,%eax
-    646c6191:	jne    646c6101 <_gnu_exception_handler+0x71>
-    646c6197:	xor    %edx,%edx
-    646c6199:	mov    $0x4,%ecx
-    646c619e:	call   646c7958 <signal>
-    646c61a3:	cmp    $0x1,%rax
-    646c61a7:	je     646c6260 <_gnu_exception_handler+0x1d0>
-    646c61ad:	test   %rax,%rax
-    646c61b0:	je     646c6101 <_gnu_exception_handler+0x71>
-    646c61b6:	mov    $0x4,%ecx
-    646c61bb:	call   *%rax
-    646c61bd:	mov    $0xffffffff,%eax
-    646c61c2:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c61c4:	cmp    $0xc000001d,%eax
-    646c61c9:	je     646c6197 <_gnu_exception_handler+0x107>
-    646c61cb:	cmp    $0xc000008c,%eax
-    646c61d0:	jne    646c6101 <_gnu_exception_handler+0x71>
-    646c61d6:	jmp    646c617a <_gnu_exception_handler+0xea>
-    646c61d8:	nopl   0x0(%rax,%rax,1)
-    646c61e0:	xor    %edx,%edx
-    646c61e2:	mov    $0x8,%ecx
-    646c61e7:	call   646c7958 <signal>
-    646c61ec:	cmp    $0x1,%rax
-    646c61f0:	jne    646c6151 <_gnu_exception_handler+0xc1>
-    646c61f6:	mov    $0x1,%edx
-    646c61fb:	mov    $0x8,%ecx
-    646c6200:	call   646c7958 <signal>
-    646c6205:	mov    $0xffffffff,%eax
-    646c620a:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c620f:	nop
-    646c6210:	mov    $0xb,%ecx
-    646c6215:	call   *%rax
-    646c6217:	mov    $0xffffffff,%eax
-    646c621c:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c6221:	xor    %eax,%eax
-    646c6223:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c6228:	nopl   0x0(%rax,%rax,1)
-    646c6230:	mov    $0x1,%edx
-    646c6235:	mov    $0x8,%ecx
-    646c623a:	call   646c7958 <signal>
-    646c623f:	call   646c68d0 <_fpreset>
-    646c6244:	jmp    646c617a <_gnu_exception_handler+0xea>
-    646c6249:	mov    $0x1,%edx
-    646c624e:	mov    $0xb,%ecx
-    646c6253:	call   646c7958 <signal>
-    646c6258:	or     $0xffffffff,%eax
-    646c625b:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c6260:	mov    $0x1,%edx
-    646c6265:	mov    $0x4,%ecx
-    646c626a:	call   646c7958 <signal>
-    646c626f:	or     $0xffffffff,%eax
-    646c6272:	jmp    646c6162 <_gnu_exception_handler+0xd2>
-    646c6277:	nop
-    646c6278:	nop
-    646c6279:	nop
-    646c627a:	nop
-    646c627b:	nop
-    646c627c:	nop
-    646c627d:	nop
-    646c627e:	nop
-    646c627f:	nop
-
-00000000646c6280 <__mingwthr_run_key_dtors.part.0>:
-    646c6280:	push   %rbp
-    646c6281:	push   %rdi
-    646c6282:	push   %rsi
-    646c6283:	push   %rbx
-    646c6284:	sub    $0x28,%rsp
-    646c6288:	lea    0x6851(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c628f:	call   *0x7f3f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c6295:	mov    0x6824(%rip),%rbx        # 646ccac0 <key_dtor_list>
-    646c629c:	test   %rbx,%rbx
-    646c629f:	je     646c62d4 <__mingwthr_run_key_dtors.part.0+0x54>
-    646c62a1:	mov    0x7fb4(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
-    646c62a8:	mov    0x7f45(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
+    646c6170:	mov    $0x1,%edx
+    646c6175:	mov    $0x8,%ecx
+    646c617a:	call   646c7898 <signal>
+    646c617f:	call   646c6810 <_fpreset>
+    646c6184:	jmp    646c60ba <_gnu_exception_handler+0xea>
+    646c6189:	mov    $0x1,%edx
+    646c618e:	mov    $0xb,%ecx
+    646c6193:	call   646c7898 <signal>
+    646c6198:	or     $0xffffffff,%eax
+    646c619b:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
+    646c61a0:	mov    $0x1,%edx
+    646c61a5:	mov    $0x4,%ecx
+    646c61aa:	call   646c7898 <signal>
+    646c61af:	or     $0xffffffff,%eax
+    646c61b2:	jmp    646c60a2 <_gnu_exception_handler+0xd2>
+    646c61b7:	nop
+    646c61b8:	nop
+    646c61b9:	nop
+    646c61ba:	nop
+    646c61bb:	nop
+    646c61bc:	nop
+    646c61bd:	nop
+    646c61be:	nop
+    646c61bf:	nop
+
+00000000646c61c0 <__mingwthr_run_key_dtors.part.0>:
+    646c61c0:	push   %rbp
+    646c61c1:	push   %rdi
+    646c61c2:	push   %rsi
+    646c61c3:	push   %rbx
+    646c61c4:	sub    $0x28,%rsp
+    646c61c8:	lea    0x68f1(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c61cf:	call   *0x7fff(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c61d5:	mov    0x68c4(%rip),%rbx        # 646ccaa0 <key_dtor_list>
+    646c61dc:	test   %rbx,%rbx
+    646c61df:	je     646c6214 <__mingwthr_run_key_dtors.part.0+0x54>
+    646c61e1:	mov    0x8074(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
+    646c61e8:	mov    0x8005(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
+    646c61ef:	nop
+    646c61f0:	mov    (%rbx),%ecx
+    646c61f2:	call   *%rbp
+    646c61f4:	mov    %rax,%rsi
+    646c61f7:	call   *%rdi
+    646c61f9:	test   %eax,%eax
+    646c61fb:	jne    646c620b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c61fd:	test   %rsi,%rsi
+    646c6200:	je     646c620b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c6202:	mov    0x8(%rbx),%rax
+    646c6206:	mov    %rsi,%rcx
+    646c6209:	call   *%rax
+    646c620b:	mov    0x10(%rbx),%rbx
+    646c620f:	test   %rbx,%rbx
+    646c6212:	jne    646c61f0 <__mingwthr_run_key_dtors.part.0+0x30>
+    646c6214:	lea    0x68a5(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c621b:	add    $0x28,%rsp
+    646c621f:	pop    %rbx
+    646c6220:	pop    %rsi
+    646c6221:	pop    %rdi
+    646c6222:	pop    %rbp
+    646c6223:	rex.W jmp *0x7fea(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c622a:	nopw   0x0(%rax,%rax,1)
+
+00000000646c6230 <___w64_mingwthr_add_key_dtor>:
+    646c6230:	push   %rbp
+    646c6231:	push   %rdi
+    646c6232:	push   %rsi
+    646c6233:	push   %rbx
+    646c6234:	sub    $0x28,%rsp
+    646c6238:	mov    0x686a(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c623e:	xor    %esi,%esi
+    646c6240:	test   %eax,%eax
+    646c6242:	mov    %ecx,%ebp
+    646c6244:	mov    %rdx,%rdi
+    646c6247:	jne    646c6254 <___w64_mingwthr_add_key_dtor+0x24>
+    646c6249:	mov    %esi,%eax
+    646c624b:	add    $0x28,%rsp
+    646c624f:	pop    %rbx
+    646c6250:	pop    %rsi
+    646c6251:	pop    %rdi
+    646c6252:	pop    %rbp
+    646c6253:	ret
+    646c6254:	mov    $0x18,%edx
+    646c6259:	mov    $0x1,%ecx
+    646c625e:	call   646c78f0 <calloc>
+    646c6263:	test   %rax,%rax
+    646c6266:	mov    %rax,%rbx
+    646c6269:	je     646c62a8 <___w64_mingwthr_add_key_dtor+0x78>
+    646c626b:	mov    %ebp,(%rax)
+    646c626d:	lea    0x684c(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c6274:	mov    %rdi,0x8(%rax)
+    646c6278:	call   *0x7f56(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c627e:	mov    0x681b(%rip),%rax        # 646ccaa0 <key_dtor_list>
+    646c6285:	lea    0x6834(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c628c:	mov    %rbx,0x680d(%rip)        # 646ccaa0 <key_dtor_list>
+    646c6293:	mov    %rax,0x10(%rbx)
+    646c6297:	call   *0x7f77(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c629d:	mov    %esi,%eax
+    646c629f:	add    $0x28,%rsp
+    646c62a3:	pop    %rbx
+    646c62a4:	pop    %rsi
+    646c62a5:	pop    %rdi
+    646c62a6:	pop    %rbp
+    646c62a7:	ret
+    646c62a8:	mov    $0xffffffff,%esi
+    646c62ad:	jmp    646c6249 <___w64_mingwthr_add_key_dtor+0x19>
     646c62af:	nop
-    646c62b0:	mov    (%rbx),%ecx
-    646c62b2:	call   *%rbp
-    646c62b4:	mov    %rax,%rsi
-    646c62b7:	call   *%rdi
-    646c62b9:	test   %eax,%eax
-    646c62bb:	jne    646c62cb <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c62bd:	test   %rsi,%rsi
-    646c62c0:	je     646c62cb <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c62c2:	mov    0x8(%rbx),%rax
-    646c62c6:	mov    %rsi,%rcx
-    646c62c9:	call   *%rax
-    646c62cb:	mov    0x10(%rbx),%rbx
-    646c62cf:	test   %rbx,%rbx
-    646c62d2:	jne    646c62b0 <__mingwthr_run_key_dtors.part.0+0x30>
-    646c62d4:	lea    0x6805(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c62db:	add    $0x28,%rsp
-    646c62df:	pop    %rbx
-    646c62e0:	pop    %rsi
-    646c62e1:	pop    %rdi
-    646c62e2:	pop    %rbp
-    646c62e3:	rex.W jmp *0x7f2a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c62ea:	nopw   0x0(%rax,%rax,1)
-
-00000000646c62f0 <___w64_mingwthr_add_key_dtor>:
-    646c62f0:	push   %rbp
-    646c62f1:	push   %rdi
-    646c62f2:	push   %rsi
-    646c62f3:	push   %rbx
-    646c62f4:	sub    $0x28,%rsp
-    646c62f8:	mov    0x67ca(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c62fe:	xor    %esi,%esi
-    646c6300:	test   %eax,%eax
-    646c6302:	mov    %ecx,%ebp
-    646c6304:	mov    %rdx,%rdi
-    646c6307:	jne    646c6314 <___w64_mingwthr_add_key_dtor+0x24>
-    646c6309:	mov    %esi,%eax
-    646c630b:	add    $0x28,%rsp
-    646c630f:	pop    %rbx
-    646c6310:	pop    %rsi
-    646c6311:	pop    %rdi
-    646c6312:	pop    %rbp
-    646c6313:	ret
-    646c6314:	mov    $0x18,%edx
-    646c6319:	mov    $0x1,%ecx
-    646c631e:	call   646c79b0 <calloc>
-    646c6323:	test   %rax,%rax
-    646c6326:	mov    %rax,%rbx
-    646c6329:	je     646c6368 <___w64_mingwthr_add_key_dtor+0x78>
-    646c632b:	mov    %ebp,(%rax)
-    646c632d:	lea    0x67ac(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c6334:	mov    %rdi,0x8(%rax)
-    646c6338:	call   *0x7e96(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c633e:	mov    0x677b(%rip),%rax        # 646ccac0 <key_dtor_list>
-    646c6345:	lea    0x6794(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c634c:	mov    %rbx,0x676d(%rip)        # 646ccac0 <key_dtor_list>
-    646c6353:	mov    %rax,0x10(%rbx)
-    646c6357:	call   *0x7eb7(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c635d:	mov    %esi,%eax
-    646c635f:	add    $0x28,%rsp
-    646c6363:	pop    %rbx
-    646c6364:	pop    %rsi
-    646c6365:	pop    %rdi
-    646c6366:	pop    %rbp
-    646c6367:	ret
-    646c6368:	mov    $0xffffffff,%esi
-    646c636d:	jmp    646c6309 <___w64_mingwthr_add_key_dtor+0x19>
-    646c636f:	nop
-
-00000000646c6370 <___w64_mingwthr_remove_key_dtor>:
-    646c6370:	push   %rbx
-    646c6371:	sub    $0x20,%rsp
-    646c6375:	mov    0x674d(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c637b:	test   %eax,%eax
-    646c637d:	mov    %ecx,%ebx
-    646c637f:	jne    646c6390 <___w64_mingwthr_remove_key_dtor+0x20>
-    646c6381:	xor    %eax,%eax
-    646c6383:	add    $0x20,%rsp
-    646c6387:	pop    %rbx
-    646c6388:	ret
-    646c6389:	nopl   0x0(%rax)
-    646c6390:	lea    0x6749(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c6397:	call   *0x7e37(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c639d:	mov    0x671c(%rip),%rax        # 646ccac0 <key_dtor_list>
-    646c63a4:	test   %rax,%rax
-    646c63a7:	je     646c63c3 <___w64_mingwthr_remove_key_dtor+0x53>
-    646c63a9:	mov    (%rax),%edx
-    646c63ab:	cmp    %edx,%ebx
-    646c63ad:	jne    646c63ba <___w64_mingwthr_remove_key_dtor+0x4a>
-    646c63af:	jmp    646c6400 <___w64_mingwthr_remove_key_dtor+0x90>
-    646c63b1:	mov    (%rcx),%edx
-    646c63b3:	cmp    %ebx,%edx
-    646c63b5:	je     646c63e0 <___w64_mingwthr_remove_key_dtor+0x70>
-    646c63b7:	mov    %rcx,%rax
-    646c63ba:	mov    0x10(%rax),%rcx
-    646c63be:	test   %rcx,%rcx
-    646c63c1:	jne    646c63b1 <___w64_mingwthr_remove_key_dtor+0x41>
-    646c63c3:	lea    0x6716(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c63ca:	call   *0x7e44(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c63d0:	xor    %eax,%eax
-    646c63d2:	add    $0x20,%rsp
-    646c63d6:	pop    %rbx
-    646c63d7:	ret
-    646c63d8:	nopl   0x0(%rax,%rax,1)
-    646c63e0:	mov    0x10(%rcx),%rdx
-    646c63e4:	mov    %rdx,0x10(%rax)
-    646c63e8:	call   646c7988 <free>
-    646c63ed:	lea    0x66ec(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c63f4:	call   *0x7e1a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c63fa:	jmp    646c63d0 <___w64_mingwthr_remove_key_dtor+0x60>
-    646c63fc:	nopl   0x0(%rax)
-    646c6400:	mov    0x10(%rax),%rdx
-    646c6404:	mov    %rax,%rcx
-    646c6407:	mov    %rdx,0x66b2(%rip)        # 646ccac0 <key_dtor_list>
-    646c640e:	jmp    646c63e8 <___w64_mingwthr_remove_key_dtor+0x78>
-
-00000000646c6410 <__mingw_TLScallback>:
-    646c6410:	push   %rbx
-    646c6411:	sub    $0x20,%rsp
-    646c6415:	cmp    $0x1,%edx
-    646c6418:	je     646c64b0 <__mingw_TLScallback+0xa0>
-    646c641e:	jb     646c6450 <__mingw_TLScallback+0x40>
-    646c6420:	cmp    $0x2,%edx
-    646c6423:	je     646c6440 <__mingw_TLScallback+0x30>
-    646c6425:	cmp    $0x3,%edx
-    646c6428:	jne    646c6445 <__mingw_TLScallback+0x35>
-    646c642a:	mov    0x6698(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c6430:	test   %eax,%eax
-    646c6432:	je     646c6445 <__mingw_TLScallback+0x35>
-    646c6434:	call   646c6280 <__mingwthr_run_key_dtors.part.0>
-    646c6439:	jmp    646c6445 <__mingw_TLScallback+0x35>
-    646c643b:	nopl   0x0(%rax,%rax,1)
-    646c6440:	call   646c68d0 <_fpreset>
-    646c6445:	mov    $0x1,%eax
-    646c644a:	add    $0x20,%rsp
-    646c644e:	pop    %rbx
-    646c644f:	ret
-    646c6450:	mov    0x6672(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c6456:	test   %eax,%eax
-    646c6458:	jne    646c64e0 <__mingw_TLScallback+0xd0>
-    646c645e:	mov    0x6664(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c6464:	cmp    $0x1,%eax
-    646c6467:	jne    646c6445 <__mingw_TLScallback+0x35>
-    646c6469:	mov    0x6650(%rip),%rcx        # 646ccac0 <key_dtor_list>
-    646c6470:	test   %rcx,%rcx
-    646c6473:	je     646c6486 <__mingw_TLScallback+0x76>
-    646c6475:	mov    0x10(%rcx),%rbx
-    646c6479:	call   646c7988 <free>
-    646c647e:	test   %rbx,%rbx
-    646c6481:	mov    %rbx,%rcx
-    646c6484:	jne    646c6475 <__mingw_TLScallback+0x65>
-    646c6486:	lea    0x6653(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c648d:	movq   $0x0,0x6628(%rip)        # 646ccac0 <key_dtor_list>
-    646c6498:	movl   $0x0,0x6626(%rip)        # 646ccac8 <__mingwthr_cs_init>
-    646c64a2:	call   *0x7d24(%rip)        # 646ce1cc <__IAT_start__>
-    646c64a8:	jmp    646c6445 <__mingw_TLScallback+0x35>
-    646c64aa:	nopw   0x0(%rax,%rax,1)
-    646c64b0:	mov    0x6612(%rip),%eax        # 646ccac8 <__mingwthr_cs_init>
-    646c64b6:	test   %eax,%eax
-    646c64b8:	je     646c64d0 <__mingw_TLScallback+0xc0>
-    646c64ba:	movl   $0x1,0x6604(%rip)        # 646ccac8 <__mingwthr_cs_init>
-    646c64c4:	mov    $0x1,%eax
-    646c64c9:	add    $0x20,%rsp
-    646c64cd:	pop    %rbx
-    646c64ce:	ret
-    646c64cf:	nop
-    646c64d0:	lea    0x6609(%rip),%rcx        # 646ccae0 <__mingwthr_cs>
-    646c64d7:	call   *0x7d2f(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c64dd:	jmp    646c64ba <__mingw_TLScallback+0xaa>
-    646c64df:	nop
-    646c64e0:	call   646c6280 <__mingwthr_run_key_dtors.part.0>
-    646c64e5:	jmp    646c645e <__mingw_TLScallback+0x4e>
-    646c64ea:	nop
-    646c64eb:	nop
-    646c64ec:	nop
-    646c64ed:	nop
-    646c64ee:	nop
-    646c64ef:	nop
-
-00000000646c64f0 <_ValidateImageBase.part.0>:
-    646c64f0:	movslq 0x3c(%rcx),%rax
-    646c64f4:	add    %rax,%rcx
-    646c64f7:	xor    %eax,%eax
-    646c64f9:	cmpl   $0x4550,(%rcx)
-    646c64ff:	je     646c6502 <_ValidateImageBase.part.0+0x12>
-    646c6501:	ret
-    646c6502:	xor    %eax,%eax
-    646c6504:	cmpw   $0x20b,0x18(%rcx)
-    646c650a:	sete   %al
-    646c650d:	ret
-    646c650e:	xchg   %ax,%ax
-
-00000000646c6510 <_ValidateImageBase>:
-    646c6510:	cmpw   $0x5a4d,(%rcx)
-    646c6515:	je     646c6520 <_ValidateImageBase+0x10>
-    646c6517:	xor    %eax,%eax
-    646c6519:	ret
-    646c651a:	nopw   0x0(%rax,%rax,1)
-    646c6520:	jmp    646c64f0 <_ValidateImageBase.part.0>
-    646c6522:	nopl   0x0(%rax)
-    646c6526:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6530 <_FindPESection>:
-    646c6530:	movslq 0x3c(%rcx),%rax
-    646c6534:	add    %rax,%rcx
-    646c6537:	movzwl 0x14(%rcx),%eax
-    646c653b:	lea    0x18(%rcx,%rax,1),%rax
-    646c6540:	movzwl 0x6(%rcx),%ecx
-    646c6544:	test   %ecx,%ecx
-    646c6546:	je     646c6571 <_FindPESection+0x41>
-    646c6548:	sub    $0x1,%ecx
-    646c654b:	lea    (%rcx,%rcx,4),%rcx
-    646c654f:	lea    0x28(%rax,%rcx,8),%r9
-    646c6554:	mov    0xc(%rax),%r8d
-    646c6558:	cmp    %rdx,%r8
-    646c655b:	mov    %r8,%rcx
-    646c655e:	ja     646c6568 <_FindPESection+0x38>
-    646c6560:	add    0x8(%rax),%ecx
-    646c6563:	cmp    %rdx,%rcx
-    646c6566:	ja     646c6573 <_FindPESection+0x43>
-    646c6568:	add    $0x28,%rax
-    646c656c:	cmp    %r9,%rax
-    646c656f:	jne    646c6554 <_FindPESection+0x24>
-    646c6571:	xor    %eax,%eax
-    646c6573:	ret
-    646c6574:	xchg   %ax,%ax
-    646c6576:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6580 <_FindPESectionByName>:
-    646c6580:	push   %rdi
-    646c6581:	push   %rsi
-    646c6582:	push   %rbx
-    646c6583:	sub    $0x20,%rsp
-    646c6587:	mov    %rcx,%rsi
-    646c658a:	call   646c7950 <strlen>
-    646c658f:	cmp    $0x8,%rax
-    646c6593:	ja     646c6600 <_FindPESectionByName+0x80>
-    646c6595:	mov    0x3164(%rip),%rdx        # 646c9700 <.refptr.__image_base__>
-    646c659c:	cmpw   $0x5a4d,(%rdx)
-    646c65a1:	jne    646c6600 <_FindPESectionByName+0x80>
-    646c65a3:	mov    %rdx,%rcx
-    646c65a6:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c65ab:	test   %eax,%eax
-    646c65ad:	je     646c6600 <_FindPESectionByName+0x80>
-    646c65af:	movslq 0x3c(%rdx),%rcx
-    646c65b3:	add    %rdx,%rcx
-    646c65b6:	movzwl 0x14(%rcx),%eax
-    646c65ba:	lea    0x18(%rcx,%rax,1),%rbx
-    646c65bf:	movzwl 0x6(%rcx),%eax
-    646c65c3:	test   %eax,%eax
-    646c65c5:	je     646c6600 <_FindPESectionByName+0x80>
-    646c65c7:	sub    $0x1,%eax
-    646c65ca:	lea    (%rax,%rax,4),%rax
-    646c65ce:	lea    0x28(%rbx,%rax,8),%rdi
-    646c65d3:	jmp    646c65de <_FindPESectionByName+0x5e>
-    646c65d5:	add    $0x28,%rbx
-    646c65d9:	cmp    %rdi,%rbx
-    646c65dc:	je     646c6600 <_FindPESectionByName+0x80>
-    646c65de:	mov    $0x8,%r8d
-    646c65e4:	mov    %rsi,%rdx
-    646c65e7:	mov    %rbx,%rcx
-    646c65ea:	call   646c7948 <strncmp>
-    646c65ef:	test   %eax,%eax
-    646c65f1:	jne    646c65d5 <_FindPESectionByName+0x55>
-    646c65f3:	mov    %rbx,%rax
-    646c65f6:	add    $0x20,%rsp
-    646c65fa:	pop    %rbx
-    646c65fb:	pop    %rsi
-    646c65fc:	pop    %rdi
-    646c65fd:	ret
-    646c65fe:	xchg   %ax,%ax
-    646c6600:	xor    %ebx,%ebx
-    646c6602:	mov    %rbx,%rax
-    646c6605:	add    $0x20,%rsp
-    646c6609:	pop    %rbx
-    646c660a:	pop    %rsi
-    646c660b:	pop    %rdi
-    646c660c:	ret
-    646c660d:	nopl   (%rax)
 
-00000000646c6610 <__mingw_GetSectionForAddress>:
+00000000646c62b0 <___w64_mingwthr_remove_key_dtor>:
+    646c62b0:	push   %rbx
+    646c62b1:	sub    $0x20,%rsp
+    646c62b5:	mov    0x67ed(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c62bb:	test   %eax,%eax
+    646c62bd:	mov    %ecx,%ebx
+    646c62bf:	jne    646c62d0 <___w64_mingwthr_remove_key_dtor+0x20>
+    646c62c1:	xor    %eax,%eax
+    646c62c3:	add    $0x20,%rsp
+    646c62c7:	pop    %rbx
+    646c62c8:	ret
+    646c62c9:	nopl   0x0(%rax)
+    646c62d0:	lea    0x67e9(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c62d7:	call   *0x7ef7(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c62dd:	mov    0x67bc(%rip),%rax        # 646ccaa0 <key_dtor_list>
+    646c62e4:	test   %rax,%rax
+    646c62e7:	je     646c6303 <___w64_mingwthr_remove_key_dtor+0x53>
+    646c62e9:	mov    (%rax),%edx
+    646c62eb:	cmp    %edx,%ebx
+    646c62ed:	jne    646c62fa <___w64_mingwthr_remove_key_dtor+0x4a>
+    646c62ef:	jmp    646c6340 <___w64_mingwthr_remove_key_dtor+0x90>
+    646c62f1:	mov    (%rcx),%edx
+    646c62f3:	cmp    %ebx,%edx
+    646c62f5:	je     646c6320 <___w64_mingwthr_remove_key_dtor+0x70>
+    646c62f7:	mov    %rcx,%rax
+    646c62fa:	mov    0x10(%rax),%rcx
+    646c62fe:	test   %rcx,%rcx
+    646c6301:	jne    646c62f1 <___w64_mingwthr_remove_key_dtor+0x41>
+    646c6303:	lea    0x67b6(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c630a:	call   *0x7f04(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c6310:	xor    %eax,%eax
+    646c6312:	add    $0x20,%rsp
+    646c6316:	pop    %rbx
+    646c6317:	ret
+    646c6318:	nopl   0x0(%rax,%rax,1)
+    646c6320:	mov    0x10(%rcx),%rdx
+    646c6324:	mov    %rdx,0x10(%rax)
+    646c6328:	call   646c78c8 <free>
+    646c632d:	lea    0x678c(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c6334:	call   *0x7eda(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c633a:	jmp    646c6310 <___w64_mingwthr_remove_key_dtor+0x60>
+    646c633c:	nopl   0x0(%rax)
+    646c6340:	mov    0x10(%rax),%rdx
+    646c6344:	mov    %rax,%rcx
+    646c6347:	mov    %rdx,0x6752(%rip)        # 646ccaa0 <key_dtor_list>
+    646c634e:	jmp    646c6328 <___w64_mingwthr_remove_key_dtor+0x78>
+
+00000000646c6350 <__mingw_TLScallback>:
+    646c6350:	push   %rbx
+    646c6351:	sub    $0x20,%rsp
+    646c6355:	cmp    $0x1,%edx
+    646c6358:	je     646c63f0 <__mingw_TLScallback+0xa0>
+    646c635e:	jb     646c6390 <__mingw_TLScallback+0x40>
+    646c6360:	cmp    $0x2,%edx
+    646c6363:	je     646c6380 <__mingw_TLScallback+0x30>
+    646c6365:	cmp    $0x3,%edx
+    646c6368:	jne    646c6385 <__mingw_TLScallback+0x35>
+    646c636a:	mov    0x6738(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c6370:	test   %eax,%eax
+    646c6372:	je     646c6385 <__mingw_TLScallback+0x35>
+    646c6374:	call   646c61c0 <__mingwthr_run_key_dtors.part.0>
+    646c6379:	jmp    646c6385 <__mingw_TLScallback+0x35>
+    646c637b:	nopl   0x0(%rax,%rax,1)
+    646c6380:	call   646c6810 <_fpreset>
+    646c6385:	mov    $0x1,%eax
+    646c638a:	add    $0x20,%rsp
+    646c638e:	pop    %rbx
+    646c638f:	ret
+    646c6390:	mov    0x6712(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c6396:	test   %eax,%eax
+    646c6398:	jne    646c6420 <__mingw_TLScallback+0xd0>
+    646c639e:	mov    0x6704(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c63a4:	cmp    $0x1,%eax
+    646c63a7:	jne    646c6385 <__mingw_TLScallback+0x35>
+    646c63a9:	mov    0x66f0(%rip),%rcx        # 646ccaa0 <key_dtor_list>
+    646c63b0:	test   %rcx,%rcx
+    646c63b3:	je     646c63c6 <__mingw_TLScallback+0x76>
+    646c63b5:	mov    0x10(%rcx),%rbx
+    646c63b9:	call   646c78c8 <free>
+    646c63be:	test   %rbx,%rbx
+    646c63c1:	mov    %rbx,%rcx
+    646c63c4:	jne    646c63b5 <__mingw_TLScallback+0x65>
+    646c63c6:	lea    0x66f3(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c63cd:	movq   $0x0,0x66c8(%rip)        # 646ccaa0 <key_dtor_list>
+    646c63d8:	movl   $0x0,0x66c6(%rip)        # 646ccaa8 <__mingwthr_cs_init>
+    646c63e2:	call   *0x7de4(%rip)        # 646ce1cc <__IAT_start__>
+    646c63e8:	jmp    646c6385 <__mingw_TLScallback+0x35>
+    646c63ea:	nopw   0x0(%rax,%rax,1)
+    646c63f0:	mov    0x66b2(%rip),%eax        # 646ccaa8 <__mingwthr_cs_init>
+    646c63f6:	test   %eax,%eax
+    646c63f8:	je     646c6410 <__mingw_TLScallback+0xc0>
+    646c63fa:	movl   $0x1,0x66a4(%rip)        # 646ccaa8 <__mingwthr_cs_init>
+    646c6404:	mov    $0x1,%eax
+    646c6409:	add    $0x20,%rsp
+    646c640d:	pop    %rbx
+    646c640e:	ret
+    646c640f:	nop
+    646c6410:	lea    0x66a9(%rip),%rcx        # 646ccac0 <__mingwthr_cs>
+    646c6417:	call   *0x7def(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c641d:	jmp    646c63fa <__mingw_TLScallback+0xaa>
+    646c641f:	nop
+    646c6420:	call   646c61c0 <__mingwthr_run_key_dtors.part.0>
+    646c6425:	jmp    646c639e <__mingw_TLScallback+0x4e>
+    646c642a:	nop
+    646c642b:	nop
+    646c642c:	nop
+    646c642d:	nop
+    646c642e:	nop
+    646c642f:	nop
+
+00000000646c6430 <_ValidateImageBase.part.0>:
+    646c6430:	movslq 0x3c(%rcx),%rax
+    646c6434:	add    %rax,%rcx
+    646c6437:	xor    %eax,%eax
+    646c6439:	cmpl   $0x4550,(%rcx)
+    646c643f:	je     646c6442 <_ValidateImageBase.part.0+0x12>
+    646c6441:	ret
+    646c6442:	xor    %eax,%eax
+    646c6444:	cmpw   $0x20b,0x18(%rcx)
+    646c644a:	sete   %al
+    646c644d:	ret
+    646c644e:	xchg   %ax,%ax
+
+00000000646c6450 <_ValidateImageBase>:
+    646c6450:	cmpw   $0x5a4d,(%rcx)
+    646c6455:	je     646c6460 <_ValidateImageBase+0x10>
+    646c6457:	xor    %eax,%eax
+    646c6459:	ret
+    646c645a:	nopw   0x0(%rax,%rax,1)
+    646c6460:	jmp    646c6430 <_ValidateImageBase.part.0>
+    646c6462:	nopl   0x0(%rax)
+    646c6466:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6470 <_FindPESection>:
+    646c6470:	movslq 0x3c(%rcx),%rax
+    646c6474:	add    %rax,%rcx
+    646c6477:	movzwl 0x14(%rcx),%eax
+    646c647b:	lea    0x18(%rcx,%rax,1),%rax
+    646c6480:	movzwl 0x6(%rcx),%ecx
+    646c6484:	test   %ecx,%ecx
+    646c6486:	je     646c64b1 <_FindPESection+0x41>
+    646c6488:	sub    $0x1,%ecx
+    646c648b:	lea    (%rcx,%rcx,4),%rcx
+    646c648f:	lea    0x28(%rax,%rcx,8),%r9
+    646c6494:	mov    0xc(%rax),%r8d
+    646c6498:	cmp    %rdx,%r8
+    646c649b:	mov    %r8,%rcx
+    646c649e:	ja     646c64a8 <_FindPESection+0x38>
+    646c64a0:	add    0x8(%rax),%ecx
+    646c64a3:	cmp    %rdx,%rcx
+    646c64a6:	ja     646c64b3 <_FindPESection+0x43>
+    646c64a8:	add    $0x28,%rax
+    646c64ac:	cmp    %r9,%rax
+    646c64af:	jne    646c6494 <_FindPESection+0x24>
+    646c64b1:	xor    %eax,%eax
+    646c64b3:	ret
+    646c64b4:	xchg   %ax,%ax
+    646c64b6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c64c0 <_FindPESectionByName>:
+    646c64c0:	push   %rdi
+    646c64c1:	push   %rsi
+    646c64c2:	push   %rbx
+    646c64c3:	sub    $0x20,%rsp
+    646c64c7:	mov    %rcx,%rsi
+    646c64ca:	call   646c7890 <strlen>
+    646c64cf:	cmp    $0x8,%rax
+    646c64d3:	ja     646c6540 <_FindPESectionByName+0x80>
+    646c64d5:	mov    0x3244(%rip),%rdx        # 646c9720 <.refptr.__image_base__>
+    646c64dc:	cmpw   $0x5a4d,(%rdx)
+    646c64e1:	jne    646c6540 <_FindPESectionByName+0x80>
+    646c64e3:	mov    %rdx,%rcx
+    646c64e6:	call   646c6430 <_ValidateImageBase.part.0>
+    646c64eb:	test   %eax,%eax
+    646c64ed:	je     646c6540 <_FindPESectionByName+0x80>
+    646c64ef:	movslq 0x3c(%rdx),%rcx
+    646c64f3:	add    %rdx,%rcx
+    646c64f6:	movzwl 0x14(%rcx),%eax
+    646c64fa:	lea    0x18(%rcx,%rax,1),%rbx
+    646c64ff:	movzwl 0x6(%rcx),%eax
+    646c6503:	test   %eax,%eax
+    646c6505:	je     646c6540 <_FindPESectionByName+0x80>
+    646c6507:	sub    $0x1,%eax
+    646c650a:	lea    (%rax,%rax,4),%rax
+    646c650e:	lea    0x28(%rbx,%rax,8),%rdi
+    646c6513:	jmp    646c651e <_FindPESectionByName+0x5e>
+    646c6515:	add    $0x28,%rbx
+    646c6519:	cmp    %rdi,%rbx
+    646c651c:	je     646c6540 <_FindPESectionByName+0x80>
+    646c651e:	mov    $0x8,%r8d
+    646c6524:	mov    %rsi,%rdx
+    646c6527:	mov    %rbx,%rcx
+    646c652a:	call   646c7888 <strncmp>
+    646c652f:	test   %eax,%eax
+    646c6531:	jne    646c6515 <_FindPESectionByName+0x55>
+    646c6533:	mov    %rbx,%rax
+    646c6536:	add    $0x20,%rsp
+    646c653a:	pop    %rbx
+    646c653b:	pop    %rsi
+    646c653c:	pop    %rdi
+    646c653d:	ret
+    646c653e:	xchg   %ax,%ax
+    646c6540:	xor    %ebx,%ebx
+    646c6542:	mov    %rbx,%rax
+    646c6545:	add    $0x20,%rsp
+    646c6549:	pop    %rbx
+    646c654a:	pop    %rsi
+    646c654b:	pop    %rdi
+    646c654c:	ret
+    646c654d:	nopl   (%rax)
+
+00000000646c6550 <__mingw_GetSectionForAddress>:
+    646c6550:	sub    $0x28,%rsp
+    646c6554:	mov    0x31c5(%rip),%r8        # 646c9720 <.refptr.__image_base__>
+    646c655b:	cmpw   $0x5a4d,(%r8)
+    646c6561:	mov    %rcx,%rdx
+    646c6564:	jne    646c65bd <__mingw_GetSectionForAddress+0x6d>
+    646c6566:	mov    %r8,%rcx
+    646c6569:	call   646c6430 <_ValidateImageBase.part.0>
+    646c656e:	test   %eax,%eax
+    646c6570:	je     646c65bd <__mingw_GetSectionForAddress+0x6d>
+    646c6572:	movslq 0x3c(%r8),%rax
+    646c6576:	mov    %rdx,%rcx
+    646c6579:	sub    %r8,%rcx
+    646c657c:	add    %rax,%r8
+    646c657f:	movzwl 0x6(%r8),%edx
+    646c6584:	movzwl 0x14(%r8),%eax
+    646c6589:	test   %edx,%edx
+    646c658b:	lea    0x18(%r8,%rax,1),%rax
+    646c6590:	je     646c65bd <__mingw_GetSectionForAddress+0x6d>
+    646c6592:	sub    $0x1,%edx
+    646c6595:	lea    (%rdx,%rdx,4),%rdx
+    646c6599:	lea    0x28(%rax,%rdx,8),%r9
+    646c659e:	xchg   %ax,%ax
+    646c65a0:	mov    0xc(%rax),%r8d
+    646c65a4:	cmp    %r8,%rcx
+    646c65a7:	mov    %r8,%rdx
+    646c65aa:	jb     646c65b4 <__mingw_GetSectionForAddress+0x64>
+    646c65ac:	add    0x8(%rax),%edx
+    646c65af:	cmp    %rdx,%rcx
+    646c65b2:	jb     646c65bf <__mingw_GetSectionForAddress+0x6f>
+    646c65b4:	add    $0x28,%rax
+    646c65b8:	cmp    %r9,%rax
+    646c65bb:	jne    646c65a0 <__mingw_GetSectionForAddress+0x50>
+    646c65bd:	xor    %eax,%eax
+    646c65bf:	add    $0x28,%rsp
+    646c65c3:	ret
+    646c65c4:	xchg   %ax,%ax
+    646c65c6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c65d0 <__mingw_GetSectionCount>:
+    646c65d0:	sub    $0x28,%rsp
+    646c65d4:	mov    0x3145(%rip),%rdx        # 646c9720 <.refptr.__image_base__>
+    646c65db:	xor    %r8d,%r8d
+    646c65de:	cmpw   $0x5a4d,(%rdx)
+    646c65e3:	je     646c65f0 <__mingw_GetSectionCount+0x20>
+    646c65e5:	mov    %r8d,%eax
+    646c65e8:	add    $0x28,%rsp
+    646c65ec:	ret
+    646c65ed:	nopl   (%rax)
+    646c65f0:	mov    %rdx,%rcx
+    646c65f3:	call   646c6430 <_ValidateImageBase.part.0>
+    646c65f8:	test   %eax,%eax
+    646c65fa:	je     646c65e5 <__mingw_GetSectionCount+0x15>
+    646c65fc:	movslq 0x3c(%rdx),%rax
+    646c6600:	movzwl 0x6(%rax,%rdx,1),%r8d
+    646c6606:	mov    %r8d,%eax
+    646c6609:	add    $0x28,%rsp
+    646c660d:	ret
+    646c660e:	xchg   %ax,%ax
+
+00000000646c6610 <_FindPESectionExec>:
     646c6610:	sub    $0x28,%rsp
-    646c6614:	mov    0x30e5(%rip),%r8        # 646c9700 <.refptr.__image_base__>
+    646c6614:	mov    0x3105(%rip),%r8        # 646c9720 <.refptr.__image_base__>
     646c661b:	cmpw   $0x5a4d,(%r8)
     646c6621:	mov    %rcx,%rdx
-    646c6624:	jne    646c667d <__mingw_GetSectionForAddress+0x6d>
+    646c6624:	jne    646c6678 <_FindPESectionExec+0x68>
     646c6626:	mov    %r8,%rcx
-    646c6629:	call   646c64f0 <_ValidateImageBase.part.0>
+    646c6629:	call   646c6430 <_ValidateImageBase.part.0>
     646c662e:	test   %eax,%eax
-    646c6630:	je     646c667d <__mingw_GetSectionForAddress+0x6d>
-    646c6632:	movslq 0x3c(%r8),%rax
-    646c6636:	mov    %rdx,%rcx
-    646c6639:	sub    %r8,%rcx
-    646c663c:	add    %rax,%r8
-    646c663f:	movzwl 0x6(%r8),%edx
-    646c6644:	movzwl 0x14(%r8),%eax
-    646c6649:	test   %edx,%edx
-    646c664b:	lea    0x18(%r8,%rax,1),%rax
-    646c6650:	je     646c667d <__mingw_GetSectionForAddress+0x6d>
-    646c6652:	sub    $0x1,%edx
-    646c6655:	lea    (%rdx,%rdx,4),%rdx
-    646c6659:	lea    0x28(%rax,%rdx,8),%r9
-    646c665e:	xchg   %ax,%ax
-    646c6660:	mov    0xc(%rax),%r8d
-    646c6664:	cmp    %r8,%rcx
-    646c6667:	mov    %r8,%rdx
-    646c666a:	jb     646c6674 <__mingw_GetSectionForAddress+0x64>
-    646c666c:	add    0x8(%rax),%edx
-    646c666f:	cmp    %rdx,%rcx
-    646c6672:	jb     646c667f <__mingw_GetSectionForAddress+0x6f>
-    646c6674:	add    $0x28,%rax
-    646c6678:	cmp    %r9,%rax
-    646c667b:	jne    646c6660 <__mingw_GetSectionForAddress+0x50>
-    646c667d:	xor    %eax,%eax
-    646c667f:	add    $0x28,%rsp
-    646c6683:	ret
-    646c6684:	xchg   %ax,%ax
-    646c6686:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6690 <__mingw_GetSectionCount>:
-    646c6690:	sub    $0x28,%rsp
-    646c6694:	mov    0x3065(%rip),%rdx        # 646c9700 <.refptr.__image_base__>
-    646c669b:	xor    %r8d,%r8d
-    646c669e:	cmpw   $0x5a4d,(%rdx)
-    646c66a3:	je     646c66b0 <__mingw_GetSectionCount+0x20>
-    646c66a5:	mov    %r8d,%eax
-    646c66a8:	add    $0x28,%rsp
-    646c66ac:	ret
-    646c66ad:	nopl   (%rax)
-    646c66b0:	mov    %rdx,%rcx
-    646c66b3:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c66b8:	test   %eax,%eax
-    646c66ba:	je     646c66a5 <__mingw_GetSectionCount+0x15>
-    646c66bc:	movslq 0x3c(%rdx),%rax
-    646c66c0:	movzwl 0x6(%rax,%rdx,1),%r8d
-    646c66c6:	mov    %r8d,%eax
-    646c66c9:	add    $0x28,%rsp
-    646c66cd:	ret
-    646c66ce:	xchg   %ax,%ax
-
-00000000646c66d0 <_FindPESectionExec>:
-    646c66d0:	sub    $0x28,%rsp
-    646c66d4:	mov    0x3025(%rip),%r8        # 646c9700 <.refptr.__image_base__>
-    646c66db:	cmpw   $0x5a4d,(%r8)
-    646c66e1:	mov    %rcx,%rdx
-    646c66e4:	jne    646c6738 <_FindPESectionExec+0x68>
-    646c66e6:	mov    %r8,%rcx
-    646c66e9:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c66ee:	test   %eax,%eax
-    646c66f0:	je     646c6738 <_FindPESectionExec+0x68>
-    646c66f2:	movslq 0x3c(%r8),%rcx
-    646c66f6:	add    %r8,%rcx
-    646c66f9:	movzwl 0x14(%rcx),%eax
-    646c66fd:	lea    0x18(%rcx,%rax,1),%rax
-    646c6702:	movzwl 0x6(%rcx),%ecx
-    646c6706:	test   %ecx,%ecx
-    646c6708:	je     646c6738 <_FindPESectionExec+0x68>
-    646c670a:	sub    $0x1,%ecx
-    646c670d:	lea    (%rcx,%rcx,4),%rcx
-    646c6711:	lea    0x28(%rax,%rcx,8),%rcx
-    646c6716:	cs nopw 0x0(%rax,%rax,1)
-    646c6720:	testb  $0x20,0x27(%rax)
-    646c6724:	je     646c672f <_FindPESectionExec+0x5f>
-    646c6726:	test   %rdx,%rdx
-    646c6729:	je     646c673a <_FindPESectionExec+0x6a>
-    646c672b:	sub    $0x1,%rdx
-    646c672f:	add    $0x28,%rax
-    646c6733:	cmp    %rcx,%rax
-    646c6736:	jne    646c6720 <_FindPESectionExec+0x50>
-    646c6738:	xor    %eax,%eax
-    646c673a:	add    $0x28,%rsp
-    646c673e:	ret
-    646c673f:	nop
-
-00000000646c6740 <_GetPEImageBase>:
-    646c6740:	sub    $0x28,%rsp
-    646c6744:	mov    0x2fb5(%rip),%rdx        # 646c9700 <.refptr.__image_base__>
-    646c674b:	cmpw   $0x5a4d,(%rdx)
-    646c6750:	jne    646c6770 <_GetPEImageBase+0x30>
-    646c6752:	mov    %rdx,%rcx
-    646c6755:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c675a:	test   %eax,%eax
-    646c675c:	mov    $0x0,%eax
-    646c6761:	cmovne %rdx,%rax
-    646c6765:	add    $0x28,%rsp
-    646c6769:	ret
-    646c676a:	nopw   0x0(%rax,%rax,1)
-    646c6770:	xor    %eax,%eax
-    646c6772:	add    $0x28,%rsp
-    646c6776:	ret
-    646c6777:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6780 <_IsNonwritableInCurrentImage>:
-    646c6780:	sub    $0x28,%rsp
-    646c6784:	mov    0x2f75(%rip),%r8        # 646c9700 <.refptr.__image_base__>
-    646c678b:	xor    %eax,%eax
-    646c678d:	cmpw   $0x5a4d,(%r8)
-    646c6793:	mov    %rcx,%rdx
-    646c6796:	je     646c67a0 <_IsNonwritableInCurrentImage+0x20>
-    646c6798:	add    $0x28,%rsp
-    646c679c:	ret
-    646c679d:	nopl   (%rax)
-    646c67a0:	mov    %r8,%rcx
-    646c67a3:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c67a8:	test   %eax,%eax
-    646c67aa:	je     646c6798 <_IsNonwritableInCurrentImage+0x18>
-    646c67ac:	movslq 0x3c(%r8),%rax
-    646c67b0:	mov    %rdx,%rcx
-    646c67b3:	sub    %r8,%rcx
-    646c67b6:	add    %rax,%r8
-    646c67b9:	movzwl 0x6(%r8),%edx
-    646c67be:	movzwl 0x14(%r8),%eax
-    646c67c3:	test   %edx,%edx
-    646c67c5:	lea    0x18(%r8,%rax,1),%rax
-    646c67ca:	je     646c67fd <_IsNonwritableInCurrentImage+0x7d>
-    646c67cc:	sub    $0x1,%edx
-    646c67cf:	lea    (%rdx,%rdx,4),%rdx
-    646c67d3:	lea    0x28(%rax,%rdx,8),%r9
-    646c67d8:	nopl   0x0(%rax,%rax,1)
-    646c67e0:	mov    0xc(%rax),%r8d
-    646c67e4:	cmp    %r8,%rcx
-    646c67e7:	mov    %r8,%rdx
-    646c67ea:	jb     646c67f4 <_IsNonwritableInCurrentImage+0x74>
-    646c67ec:	add    0x8(%rax),%edx
-    646c67ef:	cmp    %rdx,%rcx
-    646c67f2:	jb     646c6804 <_IsNonwritableInCurrentImage+0x84>
-    646c67f4:	add    $0x28,%rax
-    646c67f8:	cmp    %r9,%rax
-    646c67fb:	jne    646c67e0 <_IsNonwritableInCurrentImage+0x60>
-    646c67fd:	xor    %eax,%eax
-    646c67ff:	add    $0x28,%rsp
-    646c6803:	ret
-    646c6804:	mov    0x24(%rax),%eax
-    646c6807:	not    %eax
-    646c6809:	shr    $0x1f,%eax
-    646c680c:	add    $0x28,%rsp
-    646c6810:	ret
-    646c6811:	nopl   0x0(%rax,%rax,1)
-    646c6816:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6820 <__mingw_enum_import_library_names>:
-    646c6820:	sub    $0x28,%rsp
-    646c6824:	mov    0x2ed5(%rip),%r11        # 646c9700 <.refptr.__image_base__>
-    646c682b:	cmpw   $0x5a4d,(%r11)
-    646c6831:	mov    %ecx,%r9d
-    646c6834:	jne    646c688e <__mingw_enum_import_library_names+0x6e>
-    646c6836:	mov    %r11,%rcx
-    646c6839:	call   646c64f0 <_ValidateImageBase.part.0>
-    646c683e:	test   %eax,%eax
-    646c6840:	je     646c688e <__mingw_enum_import_library_names+0x6e>
-    646c6842:	movslq 0x3c(%r11),%rax
-    646c6846:	add    %r11,%rax
-    646c6849:	mov    0x90(%rax),%edx
-    646c684f:	test   %edx,%edx
-    646c6851:	je     646c688e <__mingw_enum_import_library_names+0x6e>
-    646c6853:	movzwl 0x14(%rax),%ecx
-    646c6857:	lea    0x18(%rax,%rcx,1),%rcx
-    646c685c:	movzwl 0x6(%rax),%eax
-    646c6860:	test   %eax,%eax
-    646c6862:	je     646c688e <__mingw_enum_import_library_names+0x6e>
-    646c6864:	sub    $0x1,%eax
-    646c6867:	lea    (%rax,%rax,4),%rax
-    646c686b:	lea    0x28(%rcx,%rax,8),%rax
-    646c6870:	mov    0xc(%rcx),%r10d
-    646c6874:	cmp    %r10,%rdx
-    646c6877:	mov    %r10,%r8
-    646c687a:	jb     646c6885 <__mingw_enum_import_library_names+0x65>
-    646c687c:	add    0x8(%rcx),%r8d
-    646c6880:	cmp    %r8,%rdx
-    646c6883:	jb     646c6895 <__mingw_enum_import_library_names+0x75>
-    646c6885:	add    $0x28,%rcx
-    646c6889:	cmp    %rax,%rcx
-    646c688c:	jne    646c6870 <__mingw_enum_import_library_names+0x50>
-    646c688e:	xor    %eax,%eax
-    646c6890:	add    $0x28,%rsp
-    646c6894:	ret
-    646c6895:	add    %r11,%rdx
-    646c6898:	jne    646c68a8 <__mingw_enum_import_library_names+0x88>
-    646c689a:	jmp    646c688e <__mingw_enum_import_library_names+0x6e>
-    646c689c:	nopl   0x0(%rax)
-    646c68a0:	sub    $0x1,%r9d
-    646c68a4:	add    $0x14,%rdx
-    646c68a8:	mov    0x4(%rdx),%ecx
-    646c68ab:	test   %ecx,%ecx
-    646c68ad:	jne    646c68b6 <__mingw_enum_import_library_names+0x96>
-    646c68af:	mov    0xc(%rdx),%eax
-    646c68b2:	test   %eax,%eax
-    646c68b4:	je     646c688e <__mingw_enum_import_library_names+0x6e>
-    646c68b6:	test   %r9d,%r9d
-    646c68b9:	jg     646c68a0 <__mingw_enum_import_library_names+0x80>
-    646c68bb:	mov    0xc(%rdx),%eax
-    646c68be:	add    %r11,%rax
-    646c68c1:	add    $0x28,%rsp
-    646c68c5:	ret
-    646c68c6:	nop
-    646c68c7:	nop
-    646c68c8:	nop
-    646c68c9:	nop
-    646c68ca:	nop
-    646c68cb:	nop
-    646c68cc:	nop
-    646c68cd:	nop
-    646c68ce:	nop
-    646c68cf:	nop
-
-00000000646c68d0 <_fpreset>:
-    646c68d0:	fninit
-    646c68d2:	ret
-    646c68d3:	nop
-    646c68d4:	nop
-    646c68d5:	nop
-    646c68d6:	nop
-    646c68d7:	nop
-    646c68d8:	nop
-    646c68d9:	nop
-    646c68da:	nop
-    646c68db:	nop
-    646c68dc:	nop
-    646c68dd:	nop
-    646c68de:	nop
-    646c68df:	nop
+    646c6630:	je     646c6678 <_FindPESectionExec+0x68>
+    646c6632:	movslq 0x3c(%r8),%rcx
+    646c6636:	add    %r8,%rcx
+    646c6639:	movzwl 0x14(%rcx),%eax
+    646c663d:	lea    0x18(%rcx,%rax,1),%rax
+    646c6642:	movzwl 0x6(%rcx),%ecx
+    646c6646:	test   %ecx,%ecx
+    646c6648:	je     646c6678 <_FindPESectionExec+0x68>
+    646c664a:	sub    $0x1,%ecx
+    646c664d:	lea    (%rcx,%rcx,4),%rcx
+    646c6651:	lea    0x28(%rax,%rcx,8),%rcx
+    646c6656:	cs nopw 0x0(%rax,%rax,1)
+    646c6660:	testb  $0x20,0x27(%rax)
+    646c6664:	je     646c666f <_FindPESectionExec+0x5f>
+    646c6666:	test   %rdx,%rdx
+    646c6669:	je     646c667a <_FindPESectionExec+0x6a>
+    646c666b:	sub    $0x1,%rdx
+    646c666f:	add    $0x28,%rax
+    646c6673:	cmp    %rcx,%rax
+    646c6676:	jne    646c6660 <_FindPESectionExec+0x50>
+    646c6678:	xor    %eax,%eax
+    646c667a:	add    $0x28,%rsp
+    646c667e:	ret
+    646c667f:	nop
+
+00000000646c6680 <_GetPEImageBase>:
+    646c6680:	sub    $0x28,%rsp
+    646c6684:	mov    0x3095(%rip),%rdx        # 646c9720 <.refptr.__image_base__>
+    646c668b:	cmpw   $0x5a4d,(%rdx)
+    646c6690:	jne    646c66b0 <_GetPEImageBase+0x30>
+    646c6692:	mov    %rdx,%rcx
+    646c6695:	call   646c6430 <_ValidateImageBase.part.0>
+    646c669a:	test   %eax,%eax
+    646c669c:	mov    $0x0,%eax
+    646c66a1:	cmovne %rdx,%rax
+    646c66a5:	add    $0x28,%rsp
+    646c66a9:	ret
+    646c66aa:	nopw   0x0(%rax,%rax,1)
+    646c66b0:	xor    %eax,%eax
+    646c66b2:	add    $0x28,%rsp
+    646c66b6:	ret
+    646c66b7:	nopw   0x0(%rax,%rax,1)
+
+00000000646c66c0 <_IsNonwritableInCurrentImage>:
+    646c66c0:	sub    $0x28,%rsp
+    646c66c4:	mov    0x3055(%rip),%r8        # 646c9720 <.refptr.__image_base__>
+    646c66cb:	xor    %eax,%eax
+    646c66cd:	cmpw   $0x5a4d,(%r8)
+    646c66d3:	mov    %rcx,%rdx
+    646c66d6:	je     646c66e0 <_IsNonwritableInCurrentImage+0x20>
+    646c66d8:	add    $0x28,%rsp
+    646c66dc:	ret
+    646c66dd:	nopl   (%rax)
+    646c66e0:	mov    %r8,%rcx
+    646c66e3:	call   646c6430 <_ValidateImageBase.part.0>
+    646c66e8:	test   %eax,%eax
+    646c66ea:	je     646c66d8 <_IsNonwritableInCurrentImage+0x18>
+    646c66ec:	movslq 0x3c(%r8),%rax
+    646c66f0:	mov    %rdx,%rcx
+    646c66f3:	sub    %r8,%rcx
+    646c66f6:	add    %rax,%r8
+    646c66f9:	movzwl 0x6(%r8),%edx
+    646c66fe:	movzwl 0x14(%r8),%eax
+    646c6703:	test   %edx,%edx
+    646c6705:	lea    0x18(%r8,%rax,1),%rax
+    646c670a:	je     646c673d <_IsNonwritableInCurrentImage+0x7d>
+    646c670c:	sub    $0x1,%edx
+    646c670f:	lea    (%rdx,%rdx,4),%rdx
+    646c6713:	lea    0x28(%rax,%rdx,8),%r9
+    646c6718:	nopl   0x0(%rax,%rax,1)
+    646c6720:	mov    0xc(%rax),%r8d
+    646c6724:	cmp    %r8,%rcx
+    646c6727:	mov    %r8,%rdx
+    646c672a:	jb     646c6734 <_IsNonwritableInCurrentImage+0x74>
+    646c672c:	add    0x8(%rax),%edx
+    646c672f:	cmp    %rdx,%rcx
+    646c6732:	jb     646c6744 <_IsNonwritableInCurrentImage+0x84>
+    646c6734:	add    $0x28,%rax
+    646c6738:	cmp    %r9,%rax
+    646c673b:	jne    646c6720 <_IsNonwritableInCurrentImage+0x60>
+    646c673d:	xor    %eax,%eax
+    646c673f:	add    $0x28,%rsp
+    646c6743:	ret
+    646c6744:	mov    0x24(%rax),%eax
+    646c6747:	not    %eax
+    646c6749:	shr    $0x1f,%eax
+    646c674c:	add    $0x28,%rsp
+    646c6750:	ret
+    646c6751:	nopl   0x0(%rax,%rax,1)
+    646c6756:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6760 <__mingw_enum_import_library_names>:
+    646c6760:	sub    $0x28,%rsp
+    646c6764:	mov    0x2fb5(%rip),%r11        # 646c9720 <.refptr.__image_base__>
+    646c676b:	cmpw   $0x5a4d,(%r11)
+    646c6771:	mov    %ecx,%r9d
+    646c6774:	jne    646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c6776:	mov    %r11,%rcx
+    646c6779:	call   646c6430 <_ValidateImageBase.part.0>
+    646c677e:	test   %eax,%eax
+    646c6780:	je     646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c6782:	movslq 0x3c(%r11),%rax
+    646c6786:	add    %r11,%rax
+    646c6789:	mov    0x90(%rax),%edx
+    646c678f:	test   %edx,%edx
+    646c6791:	je     646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c6793:	movzwl 0x14(%rax),%ecx
+    646c6797:	lea    0x18(%rax,%rcx,1),%rcx
+    646c679c:	movzwl 0x6(%rax),%eax
+    646c67a0:	test   %eax,%eax
+    646c67a2:	je     646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c67a4:	sub    $0x1,%eax
+    646c67a7:	lea    (%rax,%rax,4),%rax
+    646c67ab:	lea    0x28(%rcx,%rax,8),%rax
+    646c67b0:	mov    0xc(%rcx),%r10d
+    646c67b4:	cmp    %r10,%rdx
+    646c67b7:	mov    %r10,%r8
+    646c67ba:	jb     646c67c5 <__mingw_enum_import_library_names+0x65>
+    646c67bc:	add    0x8(%rcx),%r8d
+    646c67c0:	cmp    %r8,%rdx
+    646c67c3:	jb     646c67d5 <__mingw_enum_import_library_names+0x75>
+    646c67c5:	add    $0x28,%rcx
+    646c67c9:	cmp    %rax,%rcx
+    646c67cc:	jne    646c67b0 <__mingw_enum_import_library_names+0x50>
+    646c67ce:	xor    %eax,%eax
+    646c67d0:	add    $0x28,%rsp
+    646c67d4:	ret
+    646c67d5:	add    %r11,%rdx
+    646c67d8:	jne    646c67e8 <__mingw_enum_import_library_names+0x88>
+    646c67da:	jmp    646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c67dc:	nopl   0x0(%rax)
+    646c67e0:	sub    $0x1,%r9d
+    646c67e4:	add    $0x14,%rdx
+    646c67e8:	mov    0x4(%rdx),%ecx
+    646c67eb:	test   %ecx,%ecx
+    646c67ed:	jne    646c67f6 <__mingw_enum_import_library_names+0x96>
+    646c67ef:	mov    0xc(%rdx),%eax
+    646c67f2:	test   %eax,%eax
+    646c67f4:	je     646c67ce <__mingw_enum_import_library_names+0x6e>
+    646c67f6:	test   %r9d,%r9d
+    646c67f9:	jg     646c67e0 <__mingw_enum_import_library_names+0x80>
+    646c67fb:	mov    0xc(%rdx),%eax
+    646c67fe:	add    %r11,%rax
+    646c6801:	add    $0x28,%rsp
+    646c6805:	ret
+    646c6806:	nop
+    646c6807:	nop
+    646c6808:	nop
+    646c6809:	nop
+    646c680a:	nop
+    646c680b:	nop
+    646c680c:	nop
+    646c680d:	nop
+    646c680e:	nop
+    646c680f:	nop
+
+00000000646c6810 <_fpreset>:
+    646c6810:	fninit
+    646c6812:	ret
+    646c6813:	nop
+    646c6814:	nop
+    646c6815:	nop
+    646c6816:	nop
+    646c6817:	nop
+    646c6818:	nop
+    646c6819:	nop
+    646c681a:	nop
+    646c681b:	nop
+    646c681c:	nop
+    646c681d:	nop
+    646c681e:	nop
+    646c681f:	nop
 
-00000000646c68e0 <___chkstk_ms>:
+00000000646c6820 <___chkstk_ms>:
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:117
-    646c68e0:	push   %rcx
+    646c6820:	push   %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:119
-    646c68e1:	push   %rax
+    646c6821:	push   %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:121
-    646c68e2:	cmp    $0x1000,%rax
+    646c6822:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:122
-    646c68e8:	lea    0x18(%rsp),%rcx
+    646c6828:	lea    0x18(%rsp),%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:123
-    646c68ed:	jb     646c6908 <___chkstk_ms+0x28>
+    646c682d:	jb     646c6848 <___chkstk_ms+0x28>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:125
-    646c68ef:	sub    $0x1000,%rcx
+    646c682f:	sub    $0x1000,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:126
-    646c68f6:	orq    $0x0,(%rcx)
+    646c6836:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:127
-    646c68fa:	sub    $0x1000,%rax
+    646c683a:	sub    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:128
-    646c6900:	cmp    $0x1000,%rax
+    646c6840:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:129
-    646c6906:	ja     646c68ef <___chkstk_ms+0xf>
+    646c6846:	ja     646c682f <___chkstk_ms+0xf>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:131
-    646c6908:	sub    %rax,%rcx
+    646c6848:	sub    %rax,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:132
-    646c690b:	orq    $0x0,(%rcx)
+    646c684b:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:134
-    646c690f:	pop    %rax
+    646c684f:	pop    %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:136
-    646c6910:	pop    %rcx
+    646c6850:	pop    %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:138
-    646c6911:	ret
-    646c6912:	nop
-    646c6913:	nop
-    646c6914:	nop
-    646c6915:	nop
-    646c6916:	nop
-    646c6917:	nop
-    646c6918:	nop
-    646c6919:	nop
-    646c691a:	nop
-    646c691b:	nop
-    646c691c:	nop
-    646c691d:	nop
-    646c691e:	nop
-    646c691f:	nop
-
-00000000646c6920 <DllEntryPoint>:
-    646c6920:	mov    $0x1,%eax
-    646c6925:	ret
-    646c6926:	nop
-    646c6927:	nop
-    646c6928:	nop
-    646c6929:	nop
-    646c692a:	nop
-    646c692b:	nop
-    646c692c:	nop
-    646c692d:	nop
-    646c692e:	nop
-    646c692f:	nop
-
-00000000646c6930 <DllMain>:
-    646c6930:	mov    $0x1,%eax
-    646c6935:	ret
-    646c6936:	nop
-    646c6937:	nop
-    646c6938:	nop
-    646c6939:	nop
-    646c693a:	nop
-    646c693b:	nop
-    646c693c:	nop
-    646c693d:	nop
-    646c693e:	nop
-    646c693f:	nop
-
-00000000646c6940 <sqrt>:
-    646c6940:	push   %rbx
-    646c6941:	sub    $0x50,%rsp
-    646c6945:	movaps %xmm6,0x40(%rsp)
-    646c694a:	movq   %xmm0,%rdx
-    646c694f:	movq   %xmm0,%rbx
-    646c6954:	shr    $0x20,%rdx
-    646c6958:	mov    %edx,%eax
-    646c695a:	mov    %edx,%ecx
-    646c695c:	and    $0xfffff,%eax
-    646c6961:	and    $0x7ff00000,%ecx
-    646c6967:	or     %ebx,%eax
-    646c6969:	mov    %eax,%r8d
-    646c696c:	or     %ecx,%r8d
-    646c696f:	je     646c69b0 <sqrt+0x70>
-    646c6971:	test   %ecx,%ecx
-    646c6973:	jne    646c69d0 <sqrt+0x90>
-    646c6975:	test   %edx,%edx
-    646c6977:	js     646c69f0 <sqrt+0xb0>
-    646c6979:	movsd  0x2a9f(%rip),%xmm0        # 646c9420 <.rdata+0x20>
-    646c6981:	movq   %rbx,%xmm1
-    646c6986:	ucomisd %xmm0,%xmm1
-    646c698a:	jp     646c698e <sqrt+0x4e>
-    646c698c:	je     646c69a3 <sqrt+0x63>
-    646c698e:	mov    %rbx,0x38(%rsp)
-    646c6993:	fldl   0x38(%rsp)
-    646c6997:	fsqrt
-    646c6999:	fstpl  0x38(%rsp)
-    646c699d:	movsd  0x38(%rsp),%xmm0
-    646c69a3:	movaps 0x40(%rsp),%xmm6
-    646c69a8:	add    $0x50,%rsp
-    646c69ac:	pop    %rbx
-    646c69ad:	ret
-    646c69ae:	xchg   %ax,%ax
-    646c69b0:	test   %edx,%edx
-    646c69b2:	pxor   %xmm0,%xmm0
-    646c69b6:	jns    646c69a3 <sqrt+0x63>
-    646c69b8:	movsd  0x2a48(%rip),%xmm0        # 646c9408 <.rdata+0x8>
-    646c69c0:	movaps 0x40(%rsp),%xmm6
-    646c69c5:	add    $0x50,%rsp
-    646c69c9:	pop    %rbx
-    646c69ca:	ret
-    646c69cb:	nopl   0x0(%rax,%rax,1)
-    646c69d0:	cmp    $0x7ff00000,%ecx
-    646c69d6:	jne    646c6975 <sqrt+0x35>
-    646c69d8:	test   %eax,%eax
-    646c69da:	jne    646c6a32 <sqrt+0xf2>
-    646c69dc:	test   %edx,%edx
-    646c69de:	js     646c69f0 <sqrt+0xb0>
-    646c69e0:	movsd  0x2a30(%rip),%xmm0        # 646c9418 <.rdata+0x18>
-    646c69e8:	jmp    646c69a3 <sqrt+0x63>
-    646c69ea:	nopw   0x0(%rax,%rax,1)
-    646c69f0:	call   646c79d8 <_errno>
-    646c69f5:	movq   %rbx,%xmm2
-    646c69fa:	mov    $0x1,%ecx
-    646c69ff:	movsd  0x2a09(%rip),%xmm6        # 646c9410 <.rdata+0x10>
-    646c6a07:	movl   $0x21,(%rax)
-    646c6a0d:	lea    0x29ec(%rip),%rdx        # 646c9400 <.rdata>
-    646c6a14:	pxor   %xmm3,%xmm3
-    646c6a18:	movsd  %xmm6,0x20(%rsp)
-    646c6a1e:	call   646c7c50 <__mingw_raise_matherr>
-    646c6a23:	movapd %xmm6,%xmm0
-    646c6a27:	movaps 0x40(%rsp),%xmm6
-    646c6a2c:	add    $0x50,%rsp
-    646c6a30:	pop    %rbx
-    646c6a31:	ret
-    646c6a32:	call   646c79d8 <_errno>
-    646c6a37:	movq   %rbx,%xmm2
-    646c6a3c:	mov    $0x1,%ecx
-    646c6a41:	pxor   %xmm3,%xmm3
-    646c6a45:	movl   $0x21,(%rax)
-    646c6a4b:	lea    0x29ae(%rip),%rdx        # 646c9400 <.rdata>
-    646c6a52:	mov    %rbx,0x20(%rsp)
-    646c6a57:	call   646c7c50 <__mingw_raise_matherr>
-    646c6a5c:	movq   %rbx,%xmm0
-    646c6a61:	jmp    646c69a3 <sqrt+0x63>
-    646c6a66:	nop
-    646c6a67:	nop
-    646c6a68:	nop
-    646c6a69:	nop
-    646c6a6a:	nop
-    646c6a6b:	nop
-    646c6a6c:	nop
-    646c6a6d:	nop
-    646c6a6e:	nop
-    646c6a6f:	nop
-
-00000000646c6a70 <__ms_vsnprintf>:
-    646c6a70:	jmp    646c79c0 <_vsnprintf>
-    646c6a75:	nop
-    646c6a76:	nop
-    646c6a77:	nop
-    646c6a78:	nop
-    646c6a79:	nop
-    646c6a7a:	nop
-    646c6a7b:	nop
-    646c6a7c:	nop
-    646c6a7d:	nop
-    646c6a7e:	nop
-    646c6a7f:	nop
-
-00000000646c6a80 <cos>:
-    646c6a80:	push   %rbx
-    646c6a81:	sub    $0x70,%rsp
-    646c6a85:	movaps %xmm6,0x60(%rsp)
-    646c6a8a:	movq   %xmm0,%rax
-    646c6a8f:	movq   %xmm0,%rbx
-    646c6a94:	shr    $0x20,%rax
-    646c6a98:	mov    %eax,%edx
-    646c6a9a:	and    $0x7ff00000,%eax
-    646c6a9f:	and    $0xfffff,%edx
-    646c6aa5:	or     %ebx,%edx
-    646c6aa7:	mov    %edx,%ecx
-    646c6aa9:	or     %eax,%ecx
-    646c6aab:	sete   %r8b
-    646c6aaf:	test   %eax,%eax
-    646c6ab1:	sete   %cl
-    646c6ab4:	or     %cl,%r8b
-    646c6ab7:	jne    646c6ac0 <cos+0x40>
-    646c6ab9:	cmp    $0x7ff00000,%eax
-    646c6abe:	je     646c6af5 <cos+0x75>
-    646c6ac0:	mov    %rbx,0x30(%rsp)
-    646c6ac5:	lea    0x50(%rsp),%rcx
-    646c6aca:	fldl   0x30(%rsp)
-    646c6ace:	fstpt  0x40(%rsp)
-    646c6ad2:	lea    0x40(%rsp),%rdx
-    646c6ad7:	call   646c6b80 <__cosl_internal>
-    646c6adc:	fldt   0x50(%rsp)
-    646c6ae0:	fstpl  0x38(%rsp)
-    646c6ae4:	movsd  0x38(%rsp),%xmm0
-    646c6aea:	movaps 0x60(%rsp),%xmm6
-    646c6aef:	add    $0x70,%rsp
-    646c6af3:	pop    %rbx
-    646c6af4:	ret
-    646c6af5:	test   %edx,%edx
-    646c6af7:	jne    646c6b40 <cos+0xc0>
-    646c6af9:	call   646c79d8 <_errno>
-    646c6afe:	movq   %rbx,%xmm2
-    646c6b03:	mov    $0x1,%ecx
-    646c6b08:	movsd  0x2928(%rip),%xmm6        # 646c9438 <.rdata+0x8>
-    646c6b10:	movl   $0x21,(%rax)
-    646c6b16:	lea    0x2913(%rip),%rdx        # 646c9430 <.rdata>
-    646c6b1d:	pxor   %xmm3,%xmm3
-    646c6b21:	movsd  %xmm6,0x20(%rsp)
-    646c6b27:	call   646c7c50 <__mingw_raise_matherr>
-    646c6b2c:	movapd %xmm6,%xmm0
-    646c6b30:	movaps 0x60(%rsp),%xmm6
-    646c6b35:	add    $0x70,%rsp
-    646c6b39:	pop    %rbx
-    646c6b3a:	ret
-    646c6b3b:	nopl   0x0(%rax,%rax,1)
-    646c6b40:	call   646c79d8 <_errno>
-    646c6b45:	movq   %rbx,%xmm2
-    646c6b4a:	mov    $0x1,%ecx
-    646c6b4f:	pxor   %xmm3,%xmm3
-    646c6b53:	movl   $0x21,(%rax)
-    646c6b59:	lea    0x28d0(%rip),%rdx        # 646c9430 <.rdata>
-    646c6b60:	mov    %rbx,0x20(%rsp)
-    646c6b65:	call   646c7c50 <__mingw_raise_matherr>
-    646c6b6a:	movq   %rbx,%xmm0
-    646c6b6f:	jmp    646c6aea <cos+0x6a>
-    646c6b74:	nop
-    646c6b75:	nop
-    646c6b76:	nop
-    646c6b77:	nop
-    646c6b78:	nop
-    646c6b79:	nop
-    646c6b7a:	nop
-    646c6b7b:	nop
-    646c6b7c:	nop
-    646c6b7d:	nop
-    646c6b7e:	nop
-    646c6b7f:	nop
-
-00000000646c6b80 <__cosl_internal>:
-    646c6b80:	fldt   (%rdx)
-    646c6b82:	fcos
-    646c6b84:	fnstsw %ax
-    646c6b86:	test   $0x400,%eax
-    646c6b8b:	je     646c6ba2 <__cosl_internal+0x22>
-    646c6b8d:	fldpi
-    646c6b8f:	fadd   %st(0),%st
-    646c6b91:	fxch   %st(1)
-    646c6b93:	fprem1
-    646c6b95:	fnstsw %ax
-    646c6b97:	test   $0x400,%eax
-    646c6b9c:	jne    646c6b93 <__cosl_internal+0x13>
-    646c6b9e:	fstp   %st(1)
-    646c6ba0:	fcos
-    646c6ba2:	mov    %rcx,%rax
-    646c6ba5:	movq   $0x0,0x8(%rcx)
-    646c6bad:	fstpt  (%rcx)
-    646c6baf:	ret
-
-00000000646c6bb0 <exp>:
-    646c6bb0:	push   %rbx
-    646c6bb1:	sub    $0x50,%rsp
-    646c6bb5:	movaps %xmm6,0x40(%rsp)
-    646c6bba:	movsd  0x288e(%rip),%xmm6        # 646c9450 <.rdata+0x10>
-    646c6bc2:	movq   %xmm0,%rdx
-    646c6bc7:	movq   %xmm0,%rbx
-    646c6bcc:	shr    $0x20,%rdx
-    646c6bd0:	mov    %edx,%eax
-    646c6bd2:	mov    %edx,%ecx
-    646c6bd4:	and    $0xfffff,%eax
-    646c6bd9:	and    $0x7ff00000,%ecx
-    646c6bdf:	or     %ebx,%eax
-    646c6be1:	mov    %eax,%r8d
-    646c6be4:	or     %ecx,%r8d
-    646c6be7:	je     646c6c19 <exp+0x69>
-    646c6be9:	cmp    $0x7ff00000,%ecx
-    646c6bef:	je     646c6cb0 <exp+0x100>
-    646c6bf5:	ucomisd 0x285b(%rip),%xmm0        # 646c9458 <.rdata+0x18>
-    646c6bfd:	movapd %xmm0,%xmm1
-    646c6c01:	ja     646c6d02 <exp+0x152>
-    646c6c07:	movsd  0x2851(%rip),%xmm0        # 646c9460 <.rdata+0x20>
-    646c6c0f:	pxor   %xmm6,%xmm6
-    646c6c13:	ucomisd %xmm1,%xmm0
-    646c6c17:	jbe    646c6c30 <exp+0x80>
-    646c6c19:	movapd %xmm6,%xmm0
-    646c6c1d:	movaps 0x40(%rsp),%xmm6
-    646c6c22:	add    $0x50,%rsp
-    646c6c26:	pop    %rbx
-    646c6c27:	ret
-    646c6c28:	nopl   0x0(%rax,%rax,1)
-    646c6c30:	mov    %rbx,0x30(%rsp)
-    646c6c35:	fldl   0x30(%rsp)
-    646c6c39:	fldl2e
-    646c6c3b:	fmul   %st(1),%st
-    646c6c3d:	sub    $0x8,%rsp
-    646c6c41:	fnstcw 0x4(%rsp)
-    646c6c45:	movzwl 0x4(%rsp),%eax
-    646c6c4a:	or     $0xc,%ah
-    646c6c4d:	mov    %ax,(%rsp)
-    646c6c51:	fldcw  (%rsp)
-    646c6c54:	frndint
-    646c6c56:	fld    %st(1)
-    646c6c58:	frndint
-    646c6c5a:	fldcw  0x4(%rsp)
-    646c6c5e:	add    $0x8,%rsp
-    646c6c62:	fld    %st(1)
-    646c6c64:	fldt   0x13d6(%rip)        # 646c8040 <c0>
-    646c6c6a:	fld    %st(2)
-    646c6c6c:	fmul   %st(1),%st
-    646c6c6e:	fsubp  %st,%st(2)
-    646c6c70:	fld    %st(4)
-    646c6c72:	fsub   %st(3),%st
-    646c6c74:	fmulp  %st,%st(1)
-    646c6c76:	faddp  %st,%st(1)
-    646c6c78:	fldt   0x13b2(%rip)        # 646c8030 <c1>
-    646c6c7e:	fmul   %st(4),%st
-    646c6c80:	faddp  %st,%st(1)
-    646c6c82:	f2xm1
-    646c6c84:	fld1
-    646c6c86:	faddp  %st,%st(1)
-    646c6c88:	fstp   %st(1)
-    646c6c8a:	fscale
-    646c6c8c:	fstp   %st(1)
-    646c6c8e:	fstp   %st(1)
-    646c6c90:	fstpl  0x38(%rsp)
-    646c6c94:	movsd  0x38(%rsp),%xmm6
-    646c6c9a:	movapd %xmm6,%xmm0
-    646c6c9e:	movaps 0x40(%rsp),%xmm6
-    646c6ca3:	add    $0x50,%rsp
-    646c6ca7:	pop    %rbx
-    646c6ca8:	ret
-    646c6ca9:	nopl   0x0(%rax)
-    646c6cb0:	test   %eax,%eax
-    646c6cb2:	jne    646c6d60 <exp+0x1b0>
-    646c6cb8:	test   %edx,%edx
-    646c6cba:	js     646c6d44 <exp+0x194>
-    646c6cc0:	call   646c79d8 <_errno>
-    646c6cc5:	movsd  0x277b(%rip),%xmm6        # 646c9448 <.rdata+0x8>
-    646c6ccd:	mov    $0x4,%ecx
-    646c6cd2:	movl   $0x22,(%rax)
-    646c6cd8:	movsd  %xmm6,0x20(%rsp)
-    646c6cde:	movq   %rbx,%xmm2
-    646c6ce3:	pxor   %xmm3,%xmm3
-    646c6ce7:	lea    0x2752(%rip),%rdx        # 646c9440 <.rdata>
-    646c6cee:	call   646c7c50 <__mingw_raise_matherr>
-    646c6cf3:	movapd %xmm6,%xmm0
-    646c6cf7:	movaps 0x40(%rsp),%xmm6
-    646c6cfc:	add    $0x50,%rsp
-    646c6d00:	pop    %rbx
-    646c6d01:	ret
-    646c6d02:	call   646c79d8 <_errno>
-    646c6d07:	movq   %rbx,%xmm2
-    646c6d0c:	mov    $0x3,%ecx
-    646c6d11:	movsd  0x272f(%rip),%xmm6        # 646c9448 <.rdata+0x8>
-    646c6d19:	movl   $0x22,(%rax)
-    646c6d1f:	lea    0x271a(%rip),%rdx        # 646c9440 <.rdata>
-    646c6d26:	pxor   %xmm3,%xmm3
-    646c6d2a:	movsd  %xmm6,0x20(%rsp)
-    646c6d30:	call   646c7c50 <__mingw_raise_matherr>
-    646c6d35:	movapd %xmm6,%xmm0
-    646c6d39:	movaps 0x40(%rsp),%xmm6
-    646c6d3e:	add    $0x50,%rsp
-    646c6d42:	pop    %rbx
-    646c6d43:	ret
-    646c6d44:	call   646c79d8 <_errno>
-    646c6d49:	pxor   %xmm6,%xmm6
-    646c6d4d:	mov    $0x3,%ecx
-    646c6d52:	movl   $0x22,(%rax)
-    646c6d58:	jmp    646c6cd8 <exp+0x128>
-    646c6d5d:	nopl   (%rax)
-    646c6d60:	call   646c79d8 <_errno>
-    646c6d65:	movq   %rbx,%xmm2
-    646c6d6a:	mov    $0x1,%ecx
-    646c6d6f:	pxor   %xmm3,%xmm3
-    646c6d73:	movl   $0x21,(%rax)
-    646c6d79:	lea    0x26c0(%rip),%rdx        # 646c9440 <.rdata>
-    646c6d80:	movq   %rbx,%xmm6
-    646c6d85:	mov    %rbx,0x20(%rsp)
-    646c6d8a:	call   646c7c50 <__mingw_raise_matherr>
-    646c6d8f:	jmp    646c6c19 <exp+0x69>
-    646c6d94:	nop
-    646c6d95:	nop
-    646c6d96:	nop
-    646c6d97:	nop
-    646c6d98:	nop
-    646c6d99:	nop
-    646c6d9a:	nop
-    646c6d9b:	nop
-    646c6d9c:	nop
-    646c6d9d:	nop
-    646c6d9e:	nop
-    646c6d9f:	nop
-
-00000000646c6da0 <log>:
-    646c6da0:	push   %rbx
-    646c6da1:	sub    $0x70,%rsp
-    646c6da5:	movaps %xmm6,0x60(%rsp)
-    646c6daa:	movq   %xmm0,%rdx
-    646c6daf:	movq   %xmm0,%rbx
-    646c6db4:	shr    $0x20,%rdx
-    646c6db8:	mov    %edx,%eax
-    646c6dba:	mov    %edx,%ecx
-    646c6dbc:	and    $0xfffff,%eax
-    646c6dc1:	and    $0x7ff00000,%ecx
-    646c6dc7:	or     %ebx,%eax
-    646c6dc9:	mov    %eax,%r8d
-    646c6dcc:	or     %ecx,%r8d
-    646c6dcf:	je     646c6e30 <log+0x90>
-    646c6dd1:	test   %ecx,%ecx
-    646c6dd3:	jne    646c6e12 <log+0x72>
-    646c6dd5:	test   %edx,%edx
-    646c6dd7:	js     646c6e7e <log+0xde>
-    646c6ddd:	mov    %rbx,0x30(%rsp)
-    646c6de2:	lea    0x50(%rsp),%rcx
-    646c6de7:	fldl   0x30(%rsp)
-    646c6deb:	fstpt  0x40(%rsp)
-    646c6def:	lea    0x40(%rsp),%rdx
-    646c6df4:	call   646c77c0 <__logl_internal>
-    646c6df9:	fldt   0x50(%rsp)
-    646c6dfd:	fstpl  0x38(%rsp)
-    646c6e01:	movsd  0x38(%rsp),%xmm0
-    646c6e07:	movaps 0x60(%rsp),%xmm6
-    646c6e0c:	add    $0x70,%rsp
-    646c6e10:	pop    %rbx
-    646c6e11:	ret
-    646c6e12:	cmp    $0x7ff00000,%ecx
-    646c6e18:	jne    646c6dd5 <log+0x35>
-    646c6e1a:	test   %eax,%eax
-    646c6e1c:	je     646c6e72 <log+0xd2>
-    646c6e1e:	test   %edx,%edx
-    646c6e20:	js     646c6e7e <log+0xde>
-    646c6e22:	movsd  0x2656(%rip),%xmm0        # 646c9480 <.rdata+0x10>
-    646c6e2a:	jmp    646c6e07 <log+0x67>
-    646c6e2c:	nopl   0x0(%rax)
-    646c6e30:	call   646c79d8 <_errno>
-    646c6e35:	movq   %rbx,%xmm2
-    646c6e3a:	mov    $0x3,%ecx
-    646c6e3f:	movsd  0x2631(%rip),%xmm6        # 646c9478 <.rdata+0x8>
-    646c6e47:	movl   $0x22,(%rax)
-    646c6e4d:	lea    0x261c(%rip),%rdx        # 646c9470 <.rdata>
-    646c6e54:	pxor   %xmm3,%xmm3
-    646c6e58:	movsd  %xmm6,0x20(%rsp)
-    646c6e5e:	call   646c7c50 <__mingw_raise_matherr>
-    646c6e63:	movapd %xmm6,%xmm0
-    646c6e67:	movaps 0x60(%rsp),%xmm6
-    646c6e6c:	add    $0x70,%rsp
-    646c6e70:	pop    %rbx
-    646c6e71:	ret
-    646c6e72:	test   %edx,%edx
-    646c6e74:	movsd  0x260c(%rip),%xmm0        # 646c9488 <.rdata+0x18>
-    646c6e7c:	jns    646c6e07 <log+0x67>
-    646c6e7e:	call   646c79d8 <_errno>
-    646c6e83:	movq   %rbx,%xmm2
-    646c6e88:	mov    $0x1,%ecx
-    646c6e8d:	movsd  0x25eb(%rip),%xmm6        # 646c9480 <.rdata+0x10>
-    646c6e95:	movl   $0x21,(%rax)
-    646c6e9b:	lea    0x25ce(%rip),%rdx        # 646c9470 <.rdata>
-    646c6ea2:	pxor   %xmm3,%xmm3
-    646c6ea6:	movsd  %xmm6,0x20(%rsp)
-    646c6eac:	call   646c7c50 <__mingw_raise_matherr>
-    646c6eb1:	movapd %xmm6,%xmm0
-    646c6eb5:	movaps 0x60(%rsp),%xmm6
-    646c6eba:	add    $0x70,%rsp
-    646c6ebe:	pop    %rbx
-    646c6ebf:	ret
-
-00000000646c6ec0 <internal_modf>:
-    646c6ec0:	sub    $0x18,%rsp
-    646c6ec4:	movsd  %xmm0,0x8(%rsp)
-    646c6eca:	fldl   0x8(%rsp)
-    646c6ece:	push   %rax
-    646c6ecf:	sub    $0x8,%rsp
-    646c6ed3:	fnstcw 0x4(%rsp)
-    646c6ed7:	movzwl 0x4(%rsp),%eax
-    646c6edc:	or     $0xc,%ah
-    646c6edf:	mov    %ax,(%rsp)
-    646c6ee3:	fldcw  (%rsp)
-    646c6ee6:	frndint
-    646c6ee8:	fldcw  0x4(%rsp)
-    646c6eec:	add    $0x8,%rsp
-    646c6ef0:	pop    %rax
-    646c6ef1:	movq   %xmm0,%rax
-    646c6ef6:	fstpl  0x8(%rsp)
-    646c6efa:	movsd  0x8(%rsp),%xmm1
-    646c6f00:	shr    $0x20,%rax
-    646c6f04:	mov    %eax,%ecx
-    646c6f06:	movsd  %xmm1,(%rdx)
-    646c6f0a:	movq   %xmm0,%rdx
-    646c6f0f:	and    $0x7ff00000,%eax
-    646c6f14:	and    $0xfffff,%ecx
-    646c6f1a:	or     %edx,%ecx
-    646c6f1c:	mov    %ecx,%edx
-    646c6f1e:	or     %eax,%edx
-    646c6f20:	sete   %dl
-    646c6f23:	test   %eax,%eax
-    646c6f25:	sete   %r8b
-    646c6f29:	or     %r8d,%edx
-    646c6f2c:	xor    $0x1,%edx
-    646c6f2f:	cmp    $0x7ff00000,%eax
-    646c6f34:	sete   %al
-    646c6f37:	test   %al,%dl
-    646c6f39:	je     646c6f3f <internal_modf+0x7f>
-    646c6f3b:	test   %ecx,%ecx
-    646c6f3d:	je     646c6f50 <internal_modf+0x90>
-    646c6f3f:	subsd  0x8(%rsp),%xmm0
-    646c6f45:	add    $0x18,%rsp
-    646c6f49:	ret
-    646c6f4a:	nopw   0x0(%rax,%rax,1)
-    646c6f50:	pxor   %xmm0,%xmm0
-    646c6f54:	jmp    646c6f45 <internal_modf+0x85>
-    646c6f56:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6f60 <pow>:
-    646c6f60:	push   %r12
-    646c6f62:	push   %rbp
-    646c6f63:	push   %rdi
-    646c6f64:	push   %rsi
-    646c6f65:	push   %rbx
-    646c6f66:	sub    $0x90,%rsp
-    646c6f6d:	movaps %xmm6,0x70(%rsp)
-    646c6f72:	movaps %xmm7,0x80(%rsp)
-    646c6f7a:	mov    $0x4000,%edx
-    646c6f7f:	movq   %xmm0,%rbx
-    646c6f84:	movq   %xmm0,%rdi
-    646c6f89:	movq   %xmm1,%rbp
-    646c6f8e:	shr    $0x20,%rbx
-    646c6f92:	mov    %ebx,%eax
-    646c6f94:	mov    %ebx,%ecx
-    646c6f96:	and    $0xfffff,%eax
-    646c6f9b:	and    $0x7ff00000,%ecx
-    646c6fa1:	or     %edi,%eax
-    646c6fa3:	mov    %ecx,%esi
-    646c6fa5:	or     %eax,%esi
-    646c6fa7:	je     646c6fb6 <pow+0x56>
-    646c6fa9:	test   %ecx,%ecx
-    646c6fab:	mov    $0x4400,%edx
-    646c6fb0:	jne    646c7101 <pow+0x1a1>
-    646c6fb6:	mov    %rbp,%rsi
-    646c6fb9:	movsd  0x24ff(%rip),%xmm6        # 646c94c0 <.rdata+0x30>
-    646c6fc1:	shr    $0x20,%rsi
-    646c6fc5:	mov    %esi,%eax
-    646c6fc7:	mov    %esi,%ecx
-    646c6fc9:	and    $0xfffff,%eax
-    646c6fce:	and    $0x7ff00000,%ecx
-    646c6fd4:	or     %ebp,%eax
-    646c6fd6:	mov    %ecx,%r9d
-    646c6fd9:	or     %eax,%r9d
-    646c6fdc:	je     646c706b <pow+0x10b>
-    646c6fe2:	test   %ecx,%ecx
-    646c6fe4:	jne    646c7090 <pow+0x130>
-    646c6fea:	mov    $0x4400,%r8d
-    646c6ff0:	movsd  0x24c8(%rip),%xmm2        # 646c94c0 <.rdata+0x30>
-    646c6ff8:	movq   %rdi,%xmm4
-    646c6ffd:	ucomisd %xmm2,%xmm4
-    646c7001:	jp     646c7009 <pow+0xa9>
-    646c7003:	je     646c7458 <pow+0x4f8>
-    646c7009:	cmp    $0x100,%edx
-    646c700f:	je     646c70c0 <pow+0x160>
-    646c7015:	cmp    $0x4000,%edx
-    646c701b:	je     646c7130 <pow+0x1d0>
-    646c7021:	cmp    $0x500,%r8d
-    646c7028:	je     646c7180 <pow+0x220>
-    646c702e:	cmp    $0x500,%edx
-    646c7034:	jne    646c71a5 <pow+0x245>
-    646c703a:	test   %ebx,%ebx
-    646c703c:	js     646c7341 <pow+0x3e1>
-    646c7042:	mov    $0xffffffff,%edx
-    646c7047:	movq   %rbp,%xmm0
-    646c704c:	call   646c7810 <ldexp>
-    646c7051:	lea    0x68(%rsp),%rdx
-    646c7056:	call   646c6ec0 <internal_modf>
-    646c705b:	test   %esi,%esi
-    646c705d:	js     646c7162 <pow+0x202>
-    646c7063:	movsd  0x244d(%rip),%xmm6        # 646c94b8 <.rdata+0x28>
-    646c706b:	movapd %xmm6,%xmm0
-    646c706f:	movaps 0x80(%rsp),%xmm7
-    646c7077:	movaps 0x70(%rsp),%xmm6
-    646c707c:	add    $0x90,%rsp
-    646c7083:	pop    %rbx
-    646c7084:	pop    %rsi
-    646c7085:	pop    %rdi
-    646c7086:	pop    %rbp
-    646c7087:	pop    %r12
-    646c7089:	ret
-    646c708a:	nopw   0x0(%rax,%rax,1)
-    646c7090:	cmp    $0x7ff00000,%ecx
-    646c7096:	mov    $0x400,%r8d
-    646c709c:	jne    646c6ff0 <pow+0x90>
-    646c70a2:	test   %eax,%eax
-    646c70a4:	mov    $0x500,%r8d
-    646c70aa:	je     646c6ff0 <pow+0x90>
-    646c70b0:	movq   %rdi,%xmm5
-    646c70b5:	ucomisd %xmm6,%xmm5
-    646c70b9:	jp     646c70c0 <pow+0x160>
-    646c70bb:	je     646c706b <pow+0x10b>
+    646c6851:	ret
+    646c6852:	nop
+    646c6853:	nop
+    646c6854:	nop
+    646c6855:	nop
+    646c6856:	nop
+    646c6857:	nop
+    646c6858:	nop
+    646c6859:	nop
+    646c685a:	nop
+    646c685b:	nop
+    646c685c:	nop
+    646c685d:	nop
+    646c685e:	nop
+    646c685f:	nop
+
+00000000646c6860 <DllEntryPoint>:
+    646c6860:	mov    $0x1,%eax
+    646c6865:	ret
+    646c6866:	nop
+    646c6867:	nop
+    646c6868:	nop
+    646c6869:	nop
+    646c686a:	nop
+    646c686b:	nop
+    646c686c:	nop
+    646c686d:	nop
+    646c686e:	nop
+    646c686f:	nop
+
+00000000646c6870 <DllMain>:
+    646c6870:	mov    $0x1,%eax
+    646c6875:	ret
+    646c6876:	nop
+    646c6877:	nop
+    646c6878:	nop
+    646c6879:	nop
+    646c687a:	nop
+    646c687b:	nop
+    646c687c:	nop
+    646c687d:	nop
+    646c687e:	nop
+    646c687f:	nop
+
+00000000646c6880 <sqrt>:
+    646c6880:	push   %rbx
+    646c6881:	sub    $0x50,%rsp
+    646c6885:	movaps %xmm6,0x40(%rsp)
+    646c688a:	movq   %xmm0,%rdx
+    646c688f:	movq   %xmm0,%rbx
+    646c6894:	shr    $0x20,%rdx
+    646c6898:	mov    %edx,%eax
+    646c689a:	mov    %edx,%ecx
+    646c689c:	and    $0xfffff,%eax
+    646c68a1:	and    $0x7ff00000,%ecx
+    646c68a7:	or     %ebx,%eax
+    646c68a9:	mov    %eax,%r8d
+    646c68ac:	or     %ecx,%r8d
+    646c68af:	je     646c68f0 <sqrt+0x70>
+    646c68b1:	test   %ecx,%ecx
+    646c68b3:	jne    646c6910 <sqrt+0x90>
+    646c68b5:	test   %edx,%edx
+    646c68b7:	js     646c6930 <sqrt+0xb0>
+    646c68b9:	movsd  0x2b7f(%rip),%xmm0        # 646c9440 <.rdata+0x20>
+    646c68c1:	movq   %rbx,%xmm1
+    646c68c6:	ucomisd %xmm0,%xmm1
+    646c68ca:	jp     646c68ce <sqrt+0x4e>
+    646c68cc:	je     646c68e3 <sqrt+0x63>
+    646c68ce:	mov    %rbx,0x38(%rsp)
+    646c68d3:	fldl   0x38(%rsp)
+    646c68d7:	fsqrt
+    646c68d9:	fstpl  0x38(%rsp)
+    646c68dd:	movsd  0x38(%rsp),%xmm0
+    646c68e3:	movaps 0x40(%rsp),%xmm6
+    646c68e8:	add    $0x50,%rsp
+    646c68ec:	pop    %rbx
+    646c68ed:	ret
+    646c68ee:	xchg   %ax,%ax
+    646c68f0:	test   %edx,%edx
+    646c68f2:	pxor   %xmm0,%xmm0
+    646c68f6:	jns    646c68e3 <sqrt+0x63>
+    646c68f8:	movsd  0x2b28(%rip),%xmm0        # 646c9428 <.rdata+0x8>
+    646c6900:	movaps 0x40(%rsp),%xmm6
+    646c6905:	add    $0x50,%rsp
+    646c6909:	pop    %rbx
+    646c690a:	ret
+    646c690b:	nopl   0x0(%rax,%rax,1)
+    646c6910:	cmp    $0x7ff00000,%ecx
+    646c6916:	jne    646c68b5 <sqrt+0x35>
+    646c6918:	test   %eax,%eax
+    646c691a:	jne    646c6972 <sqrt+0xf2>
+    646c691c:	test   %edx,%edx
+    646c691e:	js     646c6930 <sqrt+0xb0>
+    646c6920:	movsd  0x2b10(%rip),%xmm0        # 646c9438 <.rdata+0x18>
+    646c6928:	jmp    646c68e3 <sqrt+0x63>
+    646c692a:	nopw   0x0(%rax,%rax,1)
+    646c6930:	call   646c7918 <_errno>
+    646c6935:	movq   %rbx,%xmm2
+    646c693a:	mov    $0x1,%ecx
+    646c693f:	movsd  0x2ae9(%rip),%xmm6        # 646c9430 <.rdata+0x10>
+    646c6947:	movl   $0x21,(%rax)
+    646c694d:	lea    0x2acc(%rip),%rdx        # 646c9420 <.rdata>
+    646c6954:	pxor   %xmm3,%xmm3
+    646c6958:	movsd  %xmm6,0x20(%rsp)
+    646c695e:	call   646c7b90 <__mingw_raise_matherr>
+    646c6963:	movapd %xmm6,%xmm0
+    646c6967:	movaps 0x40(%rsp),%xmm6
+    646c696c:	add    $0x50,%rsp
+    646c6970:	pop    %rbx
+    646c6971:	ret
+    646c6972:	call   646c7918 <_errno>
+    646c6977:	movq   %rbx,%xmm2
+    646c697c:	mov    $0x1,%ecx
+    646c6981:	pxor   %xmm3,%xmm3
+    646c6985:	movl   $0x21,(%rax)
+    646c698b:	lea    0x2a8e(%rip),%rdx        # 646c9420 <.rdata>
+    646c6992:	mov    %rbx,0x20(%rsp)
+    646c6997:	call   646c7b90 <__mingw_raise_matherr>
+    646c699c:	movq   %rbx,%xmm0
+    646c69a1:	jmp    646c68e3 <sqrt+0x63>
+    646c69a6:	nop
+    646c69a7:	nop
+    646c69a8:	nop
+    646c69a9:	nop
+    646c69aa:	nop
+    646c69ab:	nop
+    646c69ac:	nop
+    646c69ad:	nop
+    646c69ae:	nop
+    646c69af:	nop
+
+00000000646c69b0 <__ms_vsnprintf>:
+    646c69b0:	jmp    646c7900 <_vsnprintf>
+    646c69b5:	nop
+    646c69b6:	nop
+    646c69b7:	nop
+    646c69b8:	nop
+    646c69b9:	nop
+    646c69ba:	nop
+    646c69bb:	nop
+    646c69bc:	nop
+    646c69bd:	nop
+    646c69be:	nop
+    646c69bf:	nop
+
+00000000646c69c0 <cos>:
+    646c69c0:	push   %rbx
+    646c69c1:	sub    $0x70,%rsp
+    646c69c5:	movaps %xmm6,0x60(%rsp)
+    646c69ca:	movq   %xmm0,%rax
+    646c69cf:	movq   %xmm0,%rbx
+    646c69d4:	shr    $0x20,%rax
+    646c69d8:	mov    %eax,%edx
+    646c69da:	and    $0x7ff00000,%eax
+    646c69df:	and    $0xfffff,%edx
+    646c69e5:	or     %ebx,%edx
+    646c69e7:	mov    %edx,%ecx
+    646c69e9:	or     %eax,%ecx
+    646c69eb:	sete   %r8b
+    646c69ef:	test   %eax,%eax
+    646c69f1:	sete   %cl
+    646c69f4:	or     %cl,%r8b
+    646c69f7:	jne    646c6a00 <cos+0x40>
+    646c69f9:	cmp    $0x7ff00000,%eax
+    646c69fe:	je     646c6a35 <cos+0x75>
+    646c6a00:	mov    %rbx,0x30(%rsp)
+    646c6a05:	lea    0x50(%rsp),%rcx
+    646c6a0a:	fldl   0x30(%rsp)
+    646c6a0e:	fstpt  0x40(%rsp)
+    646c6a12:	lea    0x40(%rsp),%rdx
+    646c6a17:	call   646c6ac0 <__cosl_internal>
+    646c6a1c:	fldt   0x50(%rsp)
+    646c6a20:	fstpl  0x38(%rsp)
+    646c6a24:	movsd  0x38(%rsp),%xmm0
+    646c6a2a:	movaps 0x60(%rsp),%xmm6
+    646c6a2f:	add    $0x70,%rsp
+    646c6a33:	pop    %rbx
+    646c6a34:	ret
+    646c6a35:	test   %edx,%edx
+    646c6a37:	jne    646c6a80 <cos+0xc0>
+    646c6a39:	call   646c7918 <_errno>
+    646c6a3e:	movq   %rbx,%xmm2
+    646c6a43:	mov    $0x1,%ecx
+    646c6a48:	movsd  0x2a08(%rip),%xmm6        # 646c9458 <.rdata+0x8>
+    646c6a50:	movl   $0x21,(%rax)
+    646c6a56:	lea    0x29f3(%rip),%rdx        # 646c9450 <.rdata>
+    646c6a5d:	pxor   %xmm3,%xmm3
+    646c6a61:	movsd  %xmm6,0x20(%rsp)
+    646c6a67:	call   646c7b90 <__mingw_raise_matherr>
+    646c6a6c:	movapd %xmm6,%xmm0
+    646c6a70:	movaps 0x60(%rsp),%xmm6
+    646c6a75:	add    $0x70,%rsp
+    646c6a79:	pop    %rbx
+    646c6a7a:	ret
+    646c6a7b:	nopl   0x0(%rax,%rax,1)
+    646c6a80:	call   646c7918 <_errno>
+    646c6a85:	movq   %rbx,%xmm2
+    646c6a8a:	mov    $0x1,%ecx
+    646c6a8f:	pxor   %xmm3,%xmm3
+    646c6a93:	movl   $0x21,(%rax)
+    646c6a99:	lea    0x29b0(%rip),%rdx        # 646c9450 <.rdata>
+    646c6aa0:	mov    %rbx,0x20(%rsp)
+    646c6aa5:	call   646c7b90 <__mingw_raise_matherr>
+    646c6aaa:	movq   %rbx,%xmm0
+    646c6aaf:	jmp    646c6a2a <cos+0x6a>
+    646c6ab4:	nop
+    646c6ab5:	nop
+    646c6ab6:	nop
+    646c6ab7:	nop
+    646c6ab8:	nop
+    646c6ab9:	nop
+    646c6aba:	nop
+    646c6abb:	nop
+    646c6abc:	nop
+    646c6abd:	nop
+    646c6abe:	nop
+    646c6abf:	nop
+
+00000000646c6ac0 <__cosl_internal>:
+    646c6ac0:	fldt   (%rdx)
+    646c6ac2:	fcos
+    646c6ac4:	fnstsw %ax
+    646c6ac6:	test   $0x400,%eax
+    646c6acb:	je     646c6ae2 <__cosl_internal+0x22>
+    646c6acd:	fldpi
+    646c6acf:	fadd   %st(0),%st
+    646c6ad1:	fxch   %st(1)
+    646c6ad3:	fprem1
+    646c6ad5:	fnstsw %ax
+    646c6ad7:	test   $0x400,%eax
+    646c6adc:	jne    646c6ad3 <__cosl_internal+0x13>
+    646c6ade:	fstp   %st(1)
+    646c6ae0:	fcos
+    646c6ae2:	mov    %rcx,%rax
+    646c6ae5:	movq   $0x0,0x8(%rcx)
+    646c6aed:	fstpt  (%rcx)
+    646c6aef:	ret
+
+00000000646c6af0 <exp>:
+    646c6af0:	push   %rbx
+    646c6af1:	sub    $0x50,%rsp
+    646c6af5:	movaps %xmm6,0x40(%rsp)
+    646c6afa:	movsd  0x296e(%rip),%xmm6        # 646c9470 <.rdata+0x10>
+    646c6b02:	movq   %xmm0,%rdx
+    646c6b07:	movq   %xmm0,%rbx
+    646c6b0c:	shr    $0x20,%rdx
+    646c6b10:	mov    %edx,%eax
+    646c6b12:	mov    %edx,%ecx
+    646c6b14:	and    $0xfffff,%eax
+    646c6b19:	and    $0x7ff00000,%ecx
+    646c6b1f:	or     %ebx,%eax
+    646c6b21:	mov    %eax,%r8d
+    646c6b24:	or     %ecx,%r8d
+    646c6b27:	je     646c6b59 <exp+0x69>
+    646c6b29:	cmp    $0x7ff00000,%ecx
+    646c6b2f:	je     646c6bf0 <exp+0x100>
+    646c6b35:	ucomisd 0x293b(%rip),%xmm0        # 646c9478 <.rdata+0x18>
+    646c6b3d:	movapd %xmm0,%xmm1
+    646c6b41:	ja     646c6c42 <exp+0x152>
+    646c6b47:	movsd  0x2931(%rip),%xmm0        # 646c9480 <.rdata+0x20>
+    646c6b4f:	pxor   %xmm6,%xmm6
+    646c6b53:	ucomisd %xmm1,%xmm0
+    646c6b57:	jbe    646c6b70 <exp+0x80>
+    646c6b59:	movapd %xmm6,%xmm0
+    646c6b5d:	movaps 0x40(%rsp),%xmm6
+    646c6b62:	add    $0x50,%rsp
+    646c6b66:	pop    %rbx
+    646c6b67:	ret
+    646c6b68:	nopl   0x0(%rax,%rax,1)
+    646c6b70:	mov    %rbx,0x30(%rsp)
+    646c6b75:	fldl   0x30(%rsp)
+    646c6b79:	fldl2e
+    646c6b7b:	fmul   %st(1),%st
+    646c6b7d:	sub    $0x8,%rsp
+    646c6b81:	fnstcw 0x4(%rsp)
+    646c6b85:	movzwl 0x4(%rsp),%eax
+    646c6b8a:	or     $0xc,%ah
+    646c6b8d:	mov    %ax,(%rsp)
+    646c6b91:	fldcw  (%rsp)
+    646c6b94:	frndint
+    646c6b96:	fld    %st(1)
+    646c6b98:	frndint
+    646c6b9a:	fldcw  0x4(%rsp)
+    646c6b9e:	add    $0x8,%rsp
+    646c6ba2:	fld    %st(1)
+    646c6ba4:	fldt   0x1496(%rip)        # 646c8040 <c0>
+    646c6baa:	fld    %st(2)
+    646c6bac:	fmul   %st(1),%st
+    646c6bae:	fsubp  %st,%st(2)
+    646c6bb0:	fld    %st(4)
+    646c6bb2:	fsub   %st(3),%st
+    646c6bb4:	fmulp  %st,%st(1)
+    646c6bb6:	faddp  %st,%st(1)
+    646c6bb8:	fldt   0x1472(%rip)        # 646c8030 <c1>
+    646c6bbe:	fmul   %st(4),%st
+    646c6bc0:	faddp  %st,%st(1)
+    646c6bc2:	f2xm1
+    646c6bc4:	fld1
+    646c6bc6:	faddp  %st,%st(1)
+    646c6bc8:	fstp   %st(1)
+    646c6bca:	fscale
+    646c6bcc:	fstp   %st(1)
+    646c6bce:	fstp   %st(1)
+    646c6bd0:	fstpl  0x38(%rsp)
+    646c6bd4:	movsd  0x38(%rsp),%xmm6
+    646c6bda:	movapd %xmm6,%xmm0
+    646c6bde:	movaps 0x40(%rsp),%xmm6
+    646c6be3:	add    $0x50,%rsp
+    646c6be7:	pop    %rbx
+    646c6be8:	ret
+    646c6be9:	nopl   0x0(%rax)
+    646c6bf0:	test   %eax,%eax
+    646c6bf2:	jne    646c6ca0 <exp+0x1b0>
+    646c6bf8:	test   %edx,%edx
+    646c6bfa:	js     646c6c84 <exp+0x194>
+    646c6c00:	call   646c7918 <_errno>
+    646c6c05:	movsd  0x285b(%rip),%xmm6        # 646c9468 <.rdata+0x8>
+    646c6c0d:	mov    $0x4,%ecx
+    646c6c12:	movl   $0x22,(%rax)
+    646c6c18:	movsd  %xmm6,0x20(%rsp)
+    646c6c1e:	movq   %rbx,%xmm2
+    646c6c23:	pxor   %xmm3,%xmm3
+    646c6c27:	lea    0x2832(%rip),%rdx        # 646c9460 <.rdata>
+    646c6c2e:	call   646c7b90 <__mingw_raise_matherr>
+    646c6c33:	movapd %xmm6,%xmm0
+    646c6c37:	movaps 0x40(%rsp),%xmm6
+    646c6c3c:	add    $0x50,%rsp
+    646c6c40:	pop    %rbx
+    646c6c41:	ret
+    646c6c42:	call   646c7918 <_errno>
+    646c6c47:	movq   %rbx,%xmm2
+    646c6c4c:	mov    $0x3,%ecx
+    646c6c51:	movsd  0x280f(%rip),%xmm6        # 646c9468 <.rdata+0x8>
+    646c6c59:	movl   $0x22,(%rax)
+    646c6c5f:	lea    0x27fa(%rip),%rdx        # 646c9460 <.rdata>
+    646c6c66:	pxor   %xmm3,%xmm3
+    646c6c6a:	movsd  %xmm6,0x20(%rsp)
+    646c6c70:	call   646c7b90 <__mingw_raise_matherr>
+    646c6c75:	movapd %xmm6,%xmm0
+    646c6c79:	movaps 0x40(%rsp),%xmm6
+    646c6c7e:	add    $0x50,%rsp
+    646c6c82:	pop    %rbx
+    646c6c83:	ret
+    646c6c84:	call   646c7918 <_errno>
+    646c6c89:	pxor   %xmm6,%xmm6
+    646c6c8d:	mov    $0x3,%ecx
+    646c6c92:	movl   $0x22,(%rax)
+    646c6c98:	jmp    646c6c18 <exp+0x128>
+    646c6c9d:	nopl   (%rax)
+    646c6ca0:	call   646c7918 <_errno>
+    646c6ca5:	movq   %rbx,%xmm2
+    646c6caa:	mov    $0x1,%ecx
+    646c6caf:	pxor   %xmm3,%xmm3
+    646c6cb3:	movl   $0x21,(%rax)
+    646c6cb9:	lea    0x27a0(%rip),%rdx        # 646c9460 <.rdata>
+    646c6cc0:	movq   %rbx,%xmm6
+    646c6cc5:	mov    %rbx,0x20(%rsp)
+    646c6cca:	call   646c7b90 <__mingw_raise_matherr>
+    646c6ccf:	jmp    646c6b59 <exp+0x69>
+    646c6cd4:	nop
+    646c6cd5:	nop
+    646c6cd6:	nop
+    646c6cd7:	nop
+    646c6cd8:	nop
+    646c6cd9:	nop
+    646c6cda:	nop
+    646c6cdb:	nop
+    646c6cdc:	nop
+    646c6cdd:	nop
+    646c6cde:	nop
+    646c6cdf:	nop
+
+00000000646c6ce0 <log>:
+    646c6ce0:	push   %rbx
+    646c6ce1:	sub    $0x70,%rsp
+    646c6ce5:	movaps %xmm6,0x60(%rsp)
+    646c6cea:	movq   %xmm0,%rdx
+    646c6cef:	movq   %xmm0,%rbx
+    646c6cf4:	shr    $0x20,%rdx
+    646c6cf8:	mov    %edx,%eax
+    646c6cfa:	mov    %edx,%ecx
+    646c6cfc:	and    $0xfffff,%eax
+    646c6d01:	and    $0x7ff00000,%ecx
+    646c6d07:	or     %ebx,%eax
+    646c6d09:	mov    %eax,%r8d
+    646c6d0c:	or     %ecx,%r8d
+    646c6d0f:	je     646c6d70 <log+0x90>
+    646c6d11:	test   %ecx,%ecx
+    646c6d13:	jne    646c6d52 <log+0x72>
+    646c6d15:	test   %edx,%edx
+    646c6d17:	js     646c6dbe <log+0xde>
+    646c6d1d:	mov    %rbx,0x30(%rsp)
+    646c6d22:	lea    0x50(%rsp),%rcx
+    646c6d27:	fldl   0x30(%rsp)
+    646c6d2b:	fstpt  0x40(%rsp)
+    646c6d2f:	lea    0x40(%rsp),%rdx
+    646c6d34:	call   646c7700 <__logl_internal>
+    646c6d39:	fldt   0x50(%rsp)
+    646c6d3d:	fstpl  0x38(%rsp)
+    646c6d41:	movsd  0x38(%rsp),%xmm0
+    646c6d47:	movaps 0x60(%rsp),%xmm6
+    646c6d4c:	add    $0x70,%rsp
+    646c6d50:	pop    %rbx
+    646c6d51:	ret
+    646c6d52:	cmp    $0x7ff00000,%ecx
+    646c6d58:	jne    646c6d15 <log+0x35>
+    646c6d5a:	test   %eax,%eax
+    646c6d5c:	je     646c6db2 <log+0xd2>
+    646c6d5e:	test   %edx,%edx
+    646c6d60:	js     646c6dbe <log+0xde>
+    646c6d62:	movsd  0x2736(%rip),%xmm0        # 646c94a0 <.rdata+0x10>
+    646c6d6a:	jmp    646c6d47 <log+0x67>
+    646c6d6c:	nopl   0x0(%rax)
+    646c6d70:	call   646c7918 <_errno>
+    646c6d75:	movq   %rbx,%xmm2
+    646c6d7a:	mov    $0x3,%ecx
+    646c6d7f:	movsd  0x2711(%rip),%xmm6        # 646c9498 <.rdata+0x8>
+    646c6d87:	movl   $0x22,(%rax)
+    646c6d8d:	lea    0x26fc(%rip),%rdx        # 646c9490 <.rdata>
+    646c6d94:	pxor   %xmm3,%xmm3
+    646c6d98:	movsd  %xmm6,0x20(%rsp)
+    646c6d9e:	call   646c7b90 <__mingw_raise_matherr>
+    646c6da3:	movapd %xmm6,%xmm0
+    646c6da7:	movaps 0x60(%rsp),%xmm6
+    646c6dac:	add    $0x70,%rsp
+    646c6db0:	pop    %rbx
+    646c6db1:	ret
+    646c6db2:	test   %edx,%edx
+    646c6db4:	movsd  0x26ec(%rip),%xmm0        # 646c94a8 <.rdata+0x18>
+    646c6dbc:	jns    646c6d47 <log+0x67>
+    646c6dbe:	call   646c7918 <_errno>
+    646c6dc3:	movq   %rbx,%xmm2
+    646c6dc8:	mov    $0x1,%ecx
+    646c6dcd:	movsd  0x26cb(%rip),%xmm6        # 646c94a0 <.rdata+0x10>
+    646c6dd5:	movl   $0x21,(%rax)
+    646c6ddb:	lea    0x26ae(%rip),%rdx        # 646c9490 <.rdata>
+    646c6de2:	pxor   %xmm3,%xmm3
+    646c6de6:	movsd  %xmm6,0x20(%rsp)
+    646c6dec:	call   646c7b90 <__mingw_raise_matherr>
+    646c6df1:	movapd %xmm6,%xmm0
+    646c6df5:	movaps 0x60(%rsp),%xmm6
+    646c6dfa:	add    $0x70,%rsp
+    646c6dfe:	pop    %rbx
+    646c6dff:	ret
+
+00000000646c6e00 <internal_modf>:
+    646c6e00:	sub    $0x18,%rsp
+    646c6e04:	movsd  %xmm0,0x8(%rsp)
+    646c6e0a:	fldl   0x8(%rsp)
+    646c6e0e:	push   %rax
+    646c6e0f:	sub    $0x8,%rsp
+    646c6e13:	fnstcw 0x4(%rsp)
+    646c6e17:	movzwl 0x4(%rsp),%eax
+    646c6e1c:	or     $0xc,%ah
+    646c6e1f:	mov    %ax,(%rsp)
+    646c6e23:	fldcw  (%rsp)
+    646c6e26:	frndint
+    646c6e28:	fldcw  0x4(%rsp)
+    646c6e2c:	add    $0x8,%rsp
+    646c6e30:	pop    %rax
+    646c6e31:	movq   %xmm0,%rax
+    646c6e36:	fstpl  0x8(%rsp)
+    646c6e3a:	movsd  0x8(%rsp),%xmm1
+    646c6e40:	shr    $0x20,%rax
+    646c6e44:	mov    %eax,%ecx
+    646c6e46:	movsd  %xmm1,(%rdx)
+    646c6e4a:	movq   %xmm0,%rdx
+    646c6e4f:	and    $0x7ff00000,%eax
+    646c6e54:	and    $0xfffff,%ecx
+    646c6e5a:	or     %edx,%ecx
+    646c6e5c:	mov    %ecx,%edx
+    646c6e5e:	or     %eax,%edx
+    646c6e60:	sete   %dl
+    646c6e63:	test   %eax,%eax
+    646c6e65:	sete   %r8b
+    646c6e69:	or     %r8d,%edx
+    646c6e6c:	xor    $0x1,%edx
+    646c6e6f:	cmp    $0x7ff00000,%eax
+    646c6e74:	sete   %al
+    646c6e77:	test   %al,%dl
+    646c6e79:	je     646c6e7f <internal_modf+0x7f>
+    646c6e7b:	test   %ecx,%ecx
+    646c6e7d:	je     646c6e90 <internal_modf+0x90>
+    646c6e7f:	subsd  0x8(%rsp),%xmm0
+    646c6e85:	add    $0x18,%rsp
+    646c6e89:	ret
+    646c6e8a:	nopw   0x0(%rax,%rax,1)
+    646c6e90:	pxor   %xmm0,%xmm0
+    646c6e94:	jmp    646c6e85 <internal_modf+0x85>
+    646c6e96:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6ea0 <pow>:
+    646c6ea0:	push   %r12
+    646c6ea2:	push   %rbp
+    646c6ea3:	push   %rdi
+    646c6ea4:	push   %rsi
+    646c6ea5:	push   %rbx
+    646c6ea6:	sub    $0x90,%rsp
+    646c6ead:	movaps %xmm6,0x70(%rsp)
+    646c6eb2:	movaps %xmm7,0x80(%rsp)
+    646c6eba:	mov    $0x4000,%edx
+    646c6ebf:	movq   %xmm0,%rbx
+    646c6ec4:	movq   %xmm0,%rdi
+    646c6ec9:	movq   %xmm1,%rbp
+    646c6ece:	shr    $0x20,%rbx
+    646c6ed2:	mov    %ebx,%eax
+    646c6ed4:	mov    %ebx,%ecx
+    646c6ed6:	and    $0xfffff,%eax
+    646c6edb:	and    $0x7ff00000,%ecx
+    646c6ee1:	or     %edi,%eax
+    646c6ee3:	mov    %ecx,%esi
+    646c6ee5:	or     %eax,%esi
+    646c6ee7:	je     646c6ef6 <pow+0x56>
+    646c6ee9:	test   %ecx,%ecx
+    646c6eeb:	mov    $0x4400,%edx
+    646c6ef0:	jne    646c7041 <pow+0x1a1>
+    646c6ef6:	mov    %rbp,%rsi
+    646c6ef9:	movsd  0x25df(%rip),%xmm6        # 646c94e0 <.rdata+0x30>
+    646c6f01:	shr    $0x20,%rsi
+    646c6f05:	mov    %esi,%eax
+    646c6f07:	mov    %esi,%ecx
+    646c6f09:	and    $0xfffff,%eax
+    646c6f0e:	and    $0x7ff00000,%ecx
+    646c6f14:	or     %ebp,%eax
+    646c6f16:	mov    %ecx,%r9d
+    646c6f19:	or     %eax,%r9d
+    646c6f1c:	je     646c6fab <pow+0x10b>
+    646c6f22:	test   %ecx,%ecx
+    646c6f24:	jne    646c6fd0 <pow+0x130>
+    646c6f2a:	mov    $0x4400,%r8d
+    646c6f30:	movsd  0x25a8(%rip),%xmm2        # 646c94e0 <.rdata+0x30>
+    646c6f38:	movq   %rdi,%xmm4
+    646c6f3d:	ucomisd %xmm2,%xmm4
+    646c6f41:	jp     646c6f49 <pow+0xa9>
+    646c6f43:	je     646c7398 <pow+0x4f8>
+    646c6f49:	cmp    $0x100,%edx
+    646c6f4f:	je     646c7000 <pow+0x160>
+    646c6f55:	cmp    $0x4000,%edx
+    646c6f5b:	je     646c7070 <pow+0x1d0>
+    646c6f61:	cmp    $0x500,%r8d
+    646c6f68:	je     646c70c0 <pow+0x220>
+    646c6f6e:	cmp    $0x500,%edx
+    646c6f74:	jne    646c70e5 <pow+0x245>
+    646c6f7a:	test   %ebx,%ebx
+    646c6f7c:	js     646c7281 <pow+0x3e1>
+    646c6f82:	mov    $0xffffffff,%edx
+    646c6f87:	movq   %rbp,%xmm0
+    646c6f8c:	call   646c7750 <ldexp>
+    646c6f91:	lea    0x68(%rsp),%rdx
+    646c6f96:	call   646c6e00 <internal_modf>
+    646c6f9b:	test   %esi,%esi
+    646c6f9d:	js     646c70a2 <pow+0x202>
+    646c6fa3:	movsd  0x252d(%rip),%xmm6        # 646c94d8 <.rdata+0x28>
+    646c6fab:	movapd %xmm6,%xmm0
+    646c6faf:	movaps 0x80(%rsp),%xmm7
+    646c6fb7:	movaps 0x70(%rsp),%xmm6
+    646c6fbc:	add    $0x90,%rsp
+    646c6fc3:	pop    %rbx
+    646c6fc4:	pop    %rsi
+    646c6fc5:	pop    %rdi
+    646c6fc6:	pop    %rbp
+    646c6fc7:	pop    %r12
+    646c6fc9:	ret
+    646c6fca:	nopw   0x0(%rax,%rax,1)
+    646c6fd0:	cmp    $0x7ff00000,%ecx
+    646c6fd6:	mov    $0x400,%r8d
+    646c6fdc:	jne    646c6f30 <pow+0x90>
+    646c6fe2:	test   %eax,%eax
+    646c6fe4:	mov    $0x500,%r8d
+    646c6fea:	je     646c6f30 <pow+0x90>
+    646c6ff0:	movq   %rdi,%xmm5
+    646c6ff5:	ucomisd %xmm6,%xmm5
+    646c6ff9:	jp     646c7000 <pow+0x160>
+    646c6ffb:	je     646c6fab <pow+0x10b>
+    646c6ffd:	nopl   (%rax)
+    646c7000:	test   %ebx,%ebx
+    646c7002:	movsd  0x24b6(%rip),%xmm6        # 646c94c0 <.rdata+0x10>
+    646c700a:	js     646c70b0 <pow+0x210>
+    646c7010:	call   646c7918 <_errno>
+    646c7015:	movl   $0x21,(%rax)
+    646c701b:	movsd  %xmm6,0x20(%rsp)
+    646c7021:	movq   %rbp,%xmm3
+    646c7026:	movq   %rdi,%xmm2
+    646c702b:	mov    $0x1,%ecx
+    646c7030:	lea    0x2479(%rip),%rdx        # 646c94b0 <.rdata>
+    646c7037:	call   646c7b90 <__mingw_raise_matherr>
+    646c703c:	jmp    646c6fab <pow+0x10b>
+    646c7041:	cmp    $0x7ff00000,%ecx
+    646c7047:	mov    $0x400,%edx
+    646c704c:	jne    646c6ef6 <pow+0x56>
+    646c7052:	cmp    $0x1,%eax
+    646c7055:	sbb    %edx,%edx
+    646c7057:	and    $0x400,%edx
+    646c705d:	add    $0x100,%edx
+    646c7063:	jmp    646c6ef6 <pow+0x56>
+    646c7068:	nopl   0x0(%rax,%rax,1)
+    646c7070:	cmp    $0x500,%r8d
+    646c7077:	je     646c709a <pow+0x1fa>
+    646c7079:	test   %ebx,%ebx
+    646c707b:	js     646c7240 <pow+0x3a0>
+    646c7081:	mov    $0xffffffff,%edx
+    646c7086:	movq   %rbp,%xmm0
+    646c708b:	call   646c7750 <ldexp>
+    646c7090:	lea    0x68(%rsp),%rdx
+    646c7095:	call   646c6e00 <internal_modf>
+    646c709a:	test   %esi,%esi
+    646c709c:	js     646c6fa3 <pow+0x103>
+    646c70a2:	pxor   %xmm6,%xmm6
+    646c70a6:	jmp    646c6fab <pow+0x10b>
+    646c70ab:	nopl   0x0(%rax,%rax,1)
+    646c70b0:	movsd  0x2400(%rip),%xmm6        # 646c94b8 <.rdata+0x8>
+    646c70b8:	jmp    646c7010 <pow+0x170>
     646c70bd:	nopl   (%rax)
-    646c70c0:	test   %ebx,%ebx
-    646c70c2:	movsd  0x23d6(%rip),%xmm6        # 646c94a0 <.rdata+0x10>
-    646c70ca:	js     646c7170 <pow+0x210>
-    646c70d0:	call   646c79d8 <_errno>
-    646c70d5:	movl   $0x21,(%rax)
-    646c70db:	movsd  %xmm6,0x20(%rsp)
-    646c70e1:	movq   %rbp,%xmm3
-    646c70e6:	movq   %rdi,%xmm2
-    646c70eb:	mov    $0x1,%ecx
-    646c70f0:	lea    0x2399(%rip),%rdx        # 646c9490 <.rdata>
-    646c70f7:	call   646c7c50 <__mingw_raise_matherr>
-    646c70fc:	jmp    646c706b <pow+0x10b>
-    646c7101:	cmp    $0x7ff00000,%ecx
-    646c7107:	mov    $0x400,%edx
-    646c710c:	jne    646c6fb6 <pow+0x56>
-    646c7112:	cmp    $0x1,%eax
-    646c7115:	sbb    %edx,%edx
-    646c7117:	and    $0x400,%edx
-    646c711d:	add    $0x100,%edx
-    646c7123:	jmp    646c6fb6 <pow+0x56>
-    646c7128:	nopl   0x0(%rax,%rax,1)
-    646c7130:	cmp    $0x500,%r8d
-    646c7137:	je     646c715a <pow+0x1fa>
-    646c7139:	test   %ebx,%ebx
-    646c713b:	js     646c7300 <pow+0x3a0>
-    646c7141:	mov    $0xffffffff,%edx
-    646c7146:	movq   %rbp,%xmm0
-    646c714b:	call   646c7810 <ldexp>
-    646c7150:	lea    0x68(%rsp),%rdx
-    646c7155:	call   646c6ec0 <internal_modf>
-    646c715a:	test   %esi,%esi
-    646c715c:	js     646c7063 <pow+0x103>
-    646c7162:	pxor   %xmm6,%xmm6
-    646c7166:	jmp    646c706b <pow+0x10b>
-    646c716b:	nopl   0x0(%rax,%rax,1)
-    646c7170:	movsd  0x2320(%rip),%xmm6        # 646c9498 <.rdata+0x8>
-    646c7178:	jmp    646c70d0 <pow+0x170>
-    646c717d:	nopl   (%rax)
-    646c7180:	cmp    $0x500,%edx
-    646c7186:	je     646c705b <pow+0xfb>
-    646c718c:	test   %ebx,%ebx
-    646c718e:	js     646c7435 <pow+0x4d5>
-    646c7194:	movq   %rdi,%xmm5
-    646c7199:	ucomisd %xmm2,%xmm5
-    646c719d:	ja     646c705b <pow+0xfb>
-    646c71a3:	jmp    646c715a <pow+0x1fa>
-    646c71a5:	lea    0x68(%rsp),%rsi
-    646c71aa:	movq   %rbp,%xmm0
-    646c71af:	pxor   %xmm7,%xmm7
-    646c71b3:	mov    %rsi,%rdx
-    646c71b6:	call   646c6ec0 <internal_modf>
-    646c71bb:	ucomisd %xmm7,%xmm0
-    646c71bf:	jp     646c7281 <pow+0x321>
-    646c71c5:	jne    646c7281 <pow+0x321>
-    646c71cb:	movsd  0x68(%rsp),%xmm0
-    646c71d1:	movsd  0x2317(%rip),%xmm1        # 646c94f0 <.rdata+0x60>
-    646c71d9:	ucomisd %xmm0,%xmm1
-    646c71dd:	jb     646c71ed <pow+0x28d>
-    646c71df:	ucomisd 0x2311(%rip),%xmm0        # 646c94f8 <.rdata+0x68>
-    646c71e7:	jae    646c7493 <pow+0x533>
-    646c71ed:	lea    0x50(%rsp),%r12
-    646c71f2:	movq   %rdi,%xmm5
-    646c71f7:	andpd  0x2301(%rip),%xmm5        # 646c9500 <.rdata+0x70>
-    646c71ff:	movsd  %xmm5,0x30(%rsp)
-    646c7205:	lea    0x40(%rsp),%rdi
-    646c720a:	fldl   0x30(%rsp)
-    646c720e:	mov    %r12,%rcx
-    646c7211:	fstpt  0x40(%rsp)
-    646c7215:	mov    %rdi,%rdx
-    646c7218:	call   646c78e0 <log2l>
-    646c721d:	mov    %rdi,%rdx
-    646c7220:	mov    %r12,%rcx
-    646c7223:	fldt   0x50(%rsp)
-    646c7227:	mov    %rbp,0x30(%rsp)
-    646c722c:	fldl   0x30(%rsp)
-    646c7230:	fmulp  %st,%st(1)
-    646c7232:	fstpt  0x40(%rsp)
-    646c7236:	call   646c7740 <exp2l>
-    646c723b:	test   %ebx,%ebx
-    646c723d:	fldt   0x50(%rsp)
-    646c7241:	fstpl  0x38(%rsp)
-    646c7245:	movsd  0x38(%rsp),%xmm6
-    646c724b:	jns    646c706b <pow+0x10b>
-    646c7251:	mov    $0xffffffff,%edx
-    646c7256:	movq   %rbp,%xmm0
-    646c725b:	call   646c7810 <ldexp>
-    646c7260:	mov    %rsi,%rdx
-    646c7263:	call   646c6ec0 <internal_modf>
-    646c7268:	ucomisd %xmm7,%xmm0
-    646c726c:	jp     646c7274 <pow+0x314>
-    646c726e:	je     646c706b <pow+0x10b>
-    646c7274:	xorpd  0x2254(%rip),%xmm6        # 646c94d0 <.rdata+0x40>
-    646c727c:	jmp    646c706b <pow+0x10b>
-    646c7281:	test   %ebx,%ebx
-    646c7283:	js     646c747b <pow+0x51b>
-    646c7289:	movq   %rbp,%xmm5
-    646c728e:	ucomisd 0x2252(%rip),%xmm5        # 646c94e8 <.rdata+0x58>
-    646c7296:	jp     646c729e <pow+0x33e>
-    646c7298:	je     646c7461 <pow+0x501>
-    646c729e:	lea    0x50(%rsp),%rbx
-    646c72a3:	movq   %rdi,%xmm3
-    646c72a8:	andpd  0x2250(%rip),%xmm3        # 646c9500 <.rdata+0x70>
-    646c72b0:	movsd  %xmm3,0x30(%rsp)
-    646c72b6:	lea    0x40(%rsp),%rsi
-    646c72bb:	fldl   0x30(%rsp)
-    646c72bf:	mov    %rbx,%rcx
-    646c72c2:	fstpt  0x40(%rsp)
-    646c72c6:	mov    %rsi,%rdx
-    646c72c9:	call   646c78e0 <log2l>
-    646c72ce:	mov    %rsi,%rdx
-    646c72d1:	mov    %rbx,%rcx
-    646c72d4:	fldt   0x50(%rsp)
-    646c72d8:	mov    %rbp,0x30(%rsp)
-    646c72dd:	fldl   0x30(%rsp)
-    646c72e1:	fmulp  %st,%st(1)
-    646c72e3:	fstpt  0x40(%rsp)
-    646c72e7:	call   646c7740 <exp2l>
-    646c72ec:	fldt   0x50(%rsp)
-    646c72f0:	fstpl  0x38(%rsp)
-    646c72f4:	movsd  0x38(%rsp),%xmm6
-    646c72fa:	jmp    646c706b <pow+0x10b>
-    646c72ff:	nop
-    646c7300:	lea    0x68(%rsp),%rbx
-    646c7305:	movq   %rbp,%xmm0
-    646c730a:	pxor   %xmm7,%xmm7
-    646c730e:	mov    %rbx,%rdx
-    646c7311:	call   646c6ec0 <internal_modf>
-    646c7316:	ucomisd %xmm7,%xmm0
-    646c731a:	jp     646c7322 <pow+0x3c2>
-    646c731c:	je     646c7401 <pow+0x4a1>
-    646c7322:	test   %esi,%esi
-    646c7324:	jns    646c7162 <pow+0x202>
-    646c732a:	btc    $0x3f,%rdi
-    646c732f:	movq   %rdi,%xmm5
-    646c7334:	divsd  %xmm5,%xmm2
-    646c7338:	movapd %xmm2,%xmm6
-    646c733c:	jmp    646c706b <pow+0x10b>
-    646c7341:	lea    0x68(%rsp),%rbx
+    646c70c0:	cmp    $0x500,%edx
+    646c70c6:	je     646c6f9b <pow+0xfb>
+    646c70cc:	test   %ebx,%ebx
+    646c70ce:	js     646c7375 <pow+0x4d5>
+    646c70d4:	movq   %rdi,%xmm5
+    646c70d9:	ucomisd %xmm2,%xmm5
+    646c70dd:	ja     646c6f9b <pow+0xfb>
+    646c70e3:	jmp    646c709a <pow+0x1fa>
+    646c70e5:	lea    0x68(%rsp),%rsi
+    646c70ea:	movq   %rbp,%xmm0
+    646c70ef:	pxor   %xmm7,%xmm7
+    646c70f3:	mov    %rsi,%rdx
+    646c70f6:	call   646c6e00 <internal_modf>
+    646c70fb:	ucomisd %xmm7,%xmm0
+    646c70ff:	jp     646c71c1 <pow+0x321>
+    646c7105:	jne    646c71c1 <pow+0x321>
+    646c710b:	movsd  0x68(%rsp),%xmm0
+    646c7111:	movsd  0x23f7(%rip),%xmm1        # 646c9510 <.rdata+0x60>
+    646c7119:	ucomisd %xmm0,%xmm1
+    646c711d:	jb     646c712d <pow+0x28d>
+    646c711f:	ucomisd 0x23f1(%rip),%xmm0        # 646c9518 <.rdata+0x68>
+    646c7127:	jae    646c73d3 <pow+0x533>
+    646c712d:	lea    0x50(%rsp),%r12
+    646c7132:	movq   %rdi,%xmm5
+    646c7137:	andpd  0x23e1(%rip),%xmm5        # 646c9520 <.rdata+0x70>
+    646c713f:	movsd  %xmm5,0x30(%rsp)
+    646c7145:	lea    0x40(%rsp),%rdi
+    646c714a:	fldl   0x30(%rsp)
+    646c714e:	mov    %r12,%rcx
+    646c7151:	fstpt  0x40(%rsp)
+    646c7155:	mov    %rdi,%rdx
+    646c7158:	call   646c7820 <log2l>
+    646c715d:	mov    %rdi,%rdx
+    646c7160:	mov    %r12,%rcx
+    646c7163:	fldt   0x50(%rsp)
+    646c7167:	mov    %rbp,0x30(%rsp)
+    646c716c:	fldl   0x30(%rsp)
+    646c7170:	fmulp  %st,%st(1)
+    646c7172:	fstpt  0x40(%rsp)
+    646c7176:	call   646c7680 <exp2l>
+    646c717b:	test   %ebx,%ebx
+    646c717d:	fldt   0x50(%rsp)
+    646c7181:	fstpl  0x38(%rsp)
+    646c7185:	movsd  0x38(%rsp),%xmm6
+    646c718b:	jns    646c6fab <pow+0x10b>
+    646c7191:	mov    $0xffffffff,%edx
+    646c7196:	movq   %rbp,%xmm0
+    646c719b:	call   646c7750 <ldexp>
+    646c71a0:	mov    %rsi,%rdx
+    646c71a3:	call   646c6e00 <internal_modf>
+    646c71a8:	ucomisd %xmm7,%xmm0
+    646c71ac:	jp     646c71b4 <pow+0x314>
+    646c71ae:	je     646c6fab <pow+0x10b>
+    646c71b4:	xorpd  0x2334(%rip),%xmm6        # 646c94f0 <.rdata+0x40>
+    646c71bc:	jmp    646c6fab <pow+0x10b>
+    646c71c1:	test   %ebx,%ebx
+    646c71c3:	js     646c73bb <pow+0x51b>
+    646c71c9:	movq   %rbp,%xmm5
+    646c71ce:	ucomisd 0x2332(%rip),%xmm5        # 646c9508 <.rdata+0x58>
+    646c71d6:	jp     646c71de <pow+0x33e>
+    646c71d8:	je     646c73a1 <pow+0x501>
+    646c71de:	lea    0x50(%rsp),%rbx
+    646c71e3:	movq   %rdi,%xmm3
+    646c71e8:	andpd  0x2330(%rip),%xmm3        # 646c9520 <.rdata+0x70>
+    646c71f0:	movsd  %xmm3,0x30(%rsp)
+    646c71f6:	lea    0x40(%rsp),%rsi
+    646c71fb:	fldl   0x30(%rsp)
+    646c71ff:	mov    %rbx,%rcx
+    646c7202:	fstpt  0x40(%rsp)
+    646c7206:	mov    %rsi,%rdx
+    646c7209:	call   646c7820 <log2l>
+    646c720e:	mov    %rsi,%rdx
+    646c7211:	mov    %rbx,%rcx
+    646c7214:	fldt   0x50(%rsp)
+    646c7218:	mov    %rbp,0x30(%rsp)
+    646c721d:	fldl   0x30(%rsp)
+    646c7221:	fmulp  %st,%st(1)
+    646c7223:	fstpt  0x40(%rsp)
+    646c7227:	call   646c7680 <exp2l>
+    646c722c:	fldt   0x50(%rsp)
+    646c7230:	fstpl  0x38(%rsp)
+    646c7234:	movsd  0x38(%rsp),%xmm6
+    646c723a:	jmp    646c6fab <pow+0x10b>
+    646c723f:	nop
+    646c7240:	lea    0x68(%rsp),%rbx
+    646c7245:	movq   %rbp,%xmm0
+    646c724a:	pxor   %xmm7,%xmm7
+    646c724e:	mov    %rbx,%rdx
+    646c7251:	call   646c6e00 <internal_modf>
+    646c7256:	ucomisd %xmm7,%xmm0
+    646c725a:	jp     646c7262 <pow+0x3c2>
+    646c725c:	je     646c7341 <pow+0x4a1>
+    646c7262:	test   %esi,%esi
+    646c7264:	jns    646c70a2 <pow+0x202>
+    646c726a:	btc    $0x3f,%rdi
+    646c726f:	movq   %rdi,%xmm5
+    646c7274:	divsd  %xmm5,%xmm2
+    646c7278:	movapd %xmm2,%xmm6
+    646c727c:	jmp    646c6fab <pow+0x10b>
+    646c7281:	lea    0x68(%rsp),%rbx
+    646c7286:	movq   %rbp,%xmm0
+    646c728b:	pxor   %xmm7,%xmm7
+    646c728f:	mov    %rbx,%rdx
+    646c7292:	call   646c6e00 <internal_modf>
+    646c7297:	ucomisd %xmm7,%xmm0
+    646c729b:	jp     646c729f <pow+0x3ff>
+    646c729d:	je     646c72c1 <pow+0x421>
+    646c729f:	test   %esi,%esi
+    646c72a1:	movq   %rdi,%xmm6
+    646c72a6:	xorpd  0x2242(%rip),%xmm6        # 646c94f0 <.rdata+0x40>
+    646c72ae:	jns    646c6fab <pow+0x10b>
+    646c72b4:	divsd  %xmm6,%xmm2
+    646c72b8:	movapd %xmm2,%xmm6
+    646c72bc:	jmp    646c6fab <pow+0x10b>
+    646c72c1:	mov    $0xffffffff,%edx
+    646c72c6:	movq   %rbp,%xmm0
+    646c72cb:	call   646c7750 <ldexp>
+    646c72d0:	mov    %rbx,%rdx
+    646c72d3:	call   646c6e00 <internal_modf>
+    646c72d8:	mov    $0x0,%edx
+    646c72dd:	ucomisd %xmm7,%xmm0
+    646c72e1:	setnp  %al
+    646c72e4:	cmovne %edx,%eax
+    646c72e7:	mov    %esi,%edx
+    646c72e9:	shr    $0x1f,%edx
+    646c72ec:	test   %dl,%dl
+    646c72ee:	je     646c72f8 <pow+0x458>
+    646c72f0:	test   %al,%al
+    646c72f2:	jne    646c70a2 <pow+0x202>
+    646c72f8:	mov    %esi,%edx
+    646c72fa:	mov    $0x1,%r8d
+    646c7300:	not    %edx
+    646c7302:	shr    $0x1f,%edx
+    646c7305:	ucomisd %xmm7,%xmm0
+    646c7309:	setp   %cl
+    646c730c:	cmovne %r8d,%ecx
+    646c7310:	test   %cl,%cl
+    646c7312:	je     646c7318 <pow+0x478>
+    646c7314:	test   %dl,%dl
+    646c7316:	jne    646c7334 <pow+0x494>
+    646c7318:	test   %al,%al
+    646c731a:	je     646c7324 <pow+0x484>
+    646c731c:	test   %dl,%dl
+    646c731e:	jne    646c6fa3 <pow+0x103>
+    646c7324:	test   %esi,%esi
+    646c7326:	js     646c735c <pow+0x4bc>
+    646c7328:	ucomisd %xmm7,%xmm0
+    646c732c:	jp     646c7334 <pow+0x494>
+    646c732e:	je     646c6fa3 <pow+0x103>
+    646c7334:	movsd  0x2194(%rip),%xmm6        # 646c94d0 <.rdata+0x20>
+    646c733c:	jmp    646c6fab <pow+0x10b>
+    646c7341:	mov    $0xffffffff,%edx
     646c7346:	movq   %rbp,%xmm0
-    646c734b:	pxor   %xmm7,%xmm7
-    646c734f:	mov    %rbx,%rdx
-    646c7352:	call   646c6ec0 <internal_modf>
-    646c7357:	ucomisd %xmm7,%xmm0
-    646c735b:	jp     646c735f <pow+0x3ff>
-    646c735d:	je     646c7381 <pow+0x421>
-    646c735f:	test   %esi,%esi
-    646c7361:	movq   %rdi,%xmm6
-    646c7366:	xorpd  0x2162(%rip),%xmm6        # 646c94d0 <.rdata+0x40>
-    646c736e:	jns    646c706b <pow+0x10b>
-    646c7374:	divsd  %xmm6,%xmm2
-    646c7378:	movapd %xmm2,%xmm6
-    646c737c:	jmp    646c706b <pow+0x10b>
-    646c7381:	mov    $0xffffffff,%edx
-    646c7386:	movq   %rbp,%xmm0
-    646c738b:	call   646c7810 <ldexp>
-    646c7390:	mov    %rbx,%rdx
-    646c7393:	call   646c6ec0 <internal_modf>
-    646c7398:	mov    $0x0,%edx
-    646c739d:	ucomisd %xmm7,%xmm0
-    646c73a1:	setnp  %al
-    646c73a4:	cmovne %edx,%eax
-    646c73a7:	mov    %esi,%edx
-    646c73a9:	shr    $0x1f,%edx
-    646c73ac:	test   %dl,%dl
-    646c73ae:	je     646c73b8 <pow+0x458>
-    646c73b0:	test   %al,%al
-    646c73b2:	jne    646c7162 <pow+0x202>
-    646c73b8:	mov    %esi,%edx
-    646c73ba:	mov    $0x1,%r8d
-    646c73c0:	not    %edx
-    646c73c2:	shr    $0x1f,%edx
-    646c73c5:	ucomisd %xmm7,%xmm0
-    646c73c9:	setp   %cl
-    646c73cc:	cmovne %r8d,%ecx
-    646c73d0:	test   %cl,%cl
-    646c73d2:	je     646c73d8 <pow+0x478>
-    646c73d4:	test   %dl,%dl
-    646c73d6:	jne    646c73f4 <pow+0x494>
-    646c73d8:	test   %al,%al
-    646c73da:	je     646c73e4 <pow+0x484>
-    646c73dc:	test   %dl,%dl
-    646c73de:	jne    646c7063 <pow+0x103>
-    646c73e4:	test   %esi,%esi
-    646c73e6:	js     646c741c <pow+0x4bc>
-    646c73e8:	ucomisd %xmm7,%xmm0
-    646c73ec:	jp     646c73f4 <pow+0x494>
-    646c73ee:	je     646c7063 <pow+0x103>
-    646c73f4:	movsd  0x20b4(%rip),%xmm6        # 646c94b0 <.rdata+0x20>
-    646c73fc:	jmp    646c706b <pow+0x10b>
-    646c7401:	mov    $0xffffffff,%edx
-    646c7406:	movq   %rbp,%xmm0
-    646c740b:	call   646c7810 <ldexp>
-    646c7410:	mov    %rbx,%rdx
-    646c7413:	call   646c6ec0 <internal_modf>
-    646c7418:	test   %esi,%esi
-    646c741a:	js     646c73e8 <pow+0x488>
-    646c741c:	ucomisd %xmm7,%xmm0
-    646c7420:	jp     646c7428 <pow+0x4c8>
-    646c7422:	je     646c7162 <pow+0x202>
-    646c7428:	movsd  0x2078(%rip),%xmm6        # 646c94a8 <.rdata+0x18>
-    646c7430:	jmp    646c706b <pow+0x10b>
-    646c7435:	movq   %rdi,%xmm5
-    646c743a:	xorpd  0x208e(%rip),%xmm5        # 646c94d0 <.rdata+0x40>
-    646c7442:	movq   %xmm5,%rax
-    646c7447:	movq   %rdi,%xmm5
-    646c744c:	ucomisd 0x208c(%rip),%xmm5        # 646c94e0 <.rdata+0x50>
-    646c7454:	jp     646c74af <pow+0x54f>
-    646c7456:	jne    646c74af <pow+0x54f>
-    646c7458:	movapd %xmm2,%xmm6
-    646c745c:	jmp    646c706b <pow+0x10b>
-    646c7461:	mov    %rdi,0x30(%rsp)
-    646c7466:	fldl   0x30(%rsp)
-    646c746a:	fsqrt
-    646c746c:	fstpl  0x30(%rsp)
-    646c7470:	movsd  0x30(%rsp),%xmm6
-    646c7476:	jmp    646c706b <pow+0x10b>
-    646c747b:	call   646c79d8 <_errno>
-    646c7480:	movsd  0x2010(%rip),%xmm6        # 646c9498 <.rdata+0x8>
-    646c7488:	movl   $0x21,(%rax)
-    646c748e:	jmp    646c70db <pow+0x17b>
-    646c7493:	movq   %rbp,%xmm3
-    646c7498:	movq   %rdi,%xmm0
-    646c749d:	cvttsd2si %xmm3,%edx
-    646c74a1:	call   646c74c0 <__powi>
-    646c74a6:	movapd %xmm0,%xmm6
-    646c74aa:	jmp    646c706b <pow+0x10b>
-    646c74af:	mov    %rax,%rdi
-    646c74b2:	jmp    646c7194 <pow+0x234>
-    646c74b7:	nop
-    646c74b8:	nop
-    646c74b9:	nop
-    646c74ba:	nop
-    646c74bb:	nop
-    646c74bc:	nop
-    646c74bd:	nop
-    646c74be:	nop
-    646c74bf:	nop
-
-00000000646c74c0 <__powi>:
-    646c74c0:	sub    $0x58,%rsp
-    646c74c4:	movaps %xmm6,0x40(%rsp)
-    646c74c9:	movsd  0x2057(%rip),%xmm1        # 646c9528 <.rdata+0x18>
-    646c74d1:	mov    $0x0,%r10d
-    646c74d7:	movq   %xmm0,%r8
-    646c74dc:	movq   %xmm0,%rax
-    646c74e1:	shr    $0x20,%r8
-    646c74e5:	mov    %r8d,%ecx
-    646c74e8:	mov    %r8d,%r9d
-    646c74eb:	and    $0xfffff,%ecx
-    646c74f1:	and    $0x7ff00000,%r9d
-    646c74f8:	or     %eax,%ecx
-    646c74fa:	ucomisd %xmm1,%xmm0
-    646c74fe:	mov    %r9d,%r11d
-    646c7501:	setnp  %al
-    646c7504:	cmovne %r10d,%eax
-    646c7508:	test   %edx,%edx
-    646c750a:	sete   %r10b
-    646c750e:	or     %r10d,%eax
-    646c7511:	or     %ecx,%r11d
-    646c7514:	jne    646c7550 <__powi+0x90>
-    646c7516:	test   %al,%al
-    646c7518:	movapd %xmm1,%xmm6
-    646c751c:	jne    646c7540 <__powi+0x80>
-    646c751e:	mov    %edx,%eax
-    646c7520:	and    $0x1,%eax
-    646c7523:	test   %edx,%edx
-    646c7525:	js     646c7615 <__powi+0x155>
-    646c752b:	test   %eax,%eax
-    646c752d:	pxor   %xmm6,%xmm6
-    646c7531:	je     646c7540 <__powi+0x80>
-    646c7533:	test   %r8d,%r8d
-    646c7536:	jns    646c7540 <__powi+0x80>
-    646c7538:	movsd  0x1ff0(%rip),%xmm6        # 646c9530 <.rdata+0x20>
-    646c7540:	movapd %xmm6,%xmm0
-    646c7544:	movaps 0x40(%rsp),%xmm6
-    646c7549:	add    $0x58,%rsp
-    646c754d:	ret
-    646c754e:	xchg   %ax,%ax
-    646c7550:	test   %r9d,%r9d
-    646c7553:	jne    646c75c0 <__powi+0x100>
-    646c7555:	test   %al,%al
-    646c7557:	movapd %xmm1,%xmm6
-    646c755b:	jne    646c7540 <__powi+0x80>
-    646c755d:	mov    %edx,%eax
-    646c755f:	movapd %xmm0,%xmm6
-    646c7563:	andpd  0x1fe5(%rip),%xmm6        # 646c9550 <.rdata+0x40>
-    646c756b:	and    $0x1,%eax
-    646c756e:	test   %edx,%edx
-    646c7570:	js     646c7602 <__powi+0x142>
-    646c7576:	cmp    $0x1,%edx
-    646c7579:	je     646c75a1 <__powi+0xe1>
-    646c757b:	test   $0x1,%dl
-    646c757e:	jne    646c76b0 <__powi+0x1f0>
-    646c7584:	movapd %xmm6,%xmm0
-    646c7588:	shr    %edx
-    646c758a:	movapd %xmm1,%xmm6
-    646c758e:	xchg   %ax,%ax
-    646c7590:	mulsd  %xmm0,%xmm0
-    646c7594:	test   $0x1,%dl
-    646c7597:	je     646c759d <__powi+0xdd>
-    646c7599:	mulsd  %xmm0,%xmm6
-    646c759d:	shr    %edx
-    646c759f:	jne    646c7590 <__powi+0xd0>
-    646c75a1:	shr    $0x1f,%r8d
-    646c75a5:	test   %r8b,%r8b
-    646c75a8:	je     646c7540 <__powi+0x80>
-    646c75aa:	test   %eax,%eax
-    646c75ac:	je     646c7540 <__powi+0x80>
-    646c75ae:	xorpd  0x1faa(%rip),%xmm6        # 646c9560 <.rdata+0x50>
-    646c75b6:	jmp    646c7540 <__powi+0x80>
-    646c75b8:	nopl   0x0(%rax,%rax,1)
-    646c75c0:	cmp    $0x7ff00000,%r9d
-    646c75c7:	jne    646c7555 <__powi+0x95>
-    646c75c9:	test   %ecx,%ecx
-    646c75cb:	jne    646c7640 <__powi+0x180>
-    646c75cd:	mov    %edx,%r9d
-    646c75d0:	movapd %xmm1,%xmm6
-    646c75d4:	and    $0x1,%r9d
-    646c75d8:	test   %al,%al
-    646c75da:	jne    646c7540 <__powi+0x80>
-    646c75e0:	test   %r8d,%r8d
-    646c75e3:	js     646c76d0 <__powi+0x210>
-    646c75e9:	test   %edx,%edx
-    646c75eb:	movsd  0x1f45(%rip),%xmm6        # 646c9538 <.rdata+0x28>
-    646c75f3:	jns    646c7540 <__powi+0x80>
-    646c75f9:	pxor   %xmm6,%xmm6
-    646c75fd:	jmp    646c7540 <__powi+0x80>
-    646c7602:	movapd %xmm1,%xmm4
-    646c7606:	neg    %edx
-    646c7608:	divsd  %xmm6,%xmm4
-    646c760c:	movapd %xmm4,%xmm6
-    646c7610:	jmp    646c7576 <__powi+0xb6>
-    646c7615:	test   %eax,%eax
-    646c7617:	movsd  0x1f19(%rip),%xmm6        # 646c9538 <.rdata+0x28>
-    646c761f:	je     646c7540 <__powi+0x80>
-    646c7625:	test   %r8d,%r8d
-    646c7628:	jns    646c7540 <__powi+0x80>
-    646c762e:	movsd  0x1f0a(%rip),%xmm6        # 646c9540 <.rdata+0x30>
-    646c7636:	jmp    646c7540 <__powi+0x80>
-    646c763b:	nopl   0x0(%rax,%rax,1)
-    646c7640:	test   %al,%al
-    646c7642:	movapd %xmm1,%xmm6
-    646c7646:	jne    646c7540 <__powi+0x80>
-    646c764c:	test   %r8d,%r8d
-    646c764f:	movsd  0x1ec9(%rip),%xmm6        # 646c9520 <.rdata+0x10>
-    646c7657:	js     646c76c0 <__powi+0x200>
-    646c7659:	mov    %edx,0x3c(%rsp)
-    646c765d:	movsd  %xmm0,0x30(%rsp)
-    646c7663:	call   646c79d8 <_errno>
-    646c7668:	mov    0x3c(%rsp),%edx
-    646c766c:	pxor   %xmm3,%xmm3
-    646c7670:	mov    $0x1,%ecx
-    646c7675:	movsd  0x30(%rsp),%xmm0
-    646c767b:	movl   $0x21,(%rax)
-    646c7681:	movsd  %xmm6,0x20(%rsp)
-    646c7687:	movapd %xmm0,%xmm2
-    646c768b:	cvtsi2sd %edx,%xmm3
-    646c768f:	lea    0x1e7a(%rip),%rdx        # 646c9510 <.rdata>
-    646c7696:	call   646c7c50 <__mingw_raise_matherr>
-    646c769b:	movapd %xmm6,%xmm0
-    646c769f:	movaps 0x40(%rsp),%xmm6
-    646c76a4:	add    $0x58,%rsp
-    646c76a8:	ret
-    646c76a9:	nopl   0x0(%rax)
-    646c76b0:	movapd %xmm6,%xmm1
-    646c76b4:	jmp    646c7584 <__powi+0xc4>
-    646c76b9:	nopl   0x0(%rax)
-    646c76c0:	movsd  0x1e50(%rip),%xmm6        # 646c9518 <.rdata+0x8>
-    646c76c8:	jmp    646c7659 <__powi+0x199>
-    646c76ca:	nopw   0x0(%rax,%rax,1)
-    646c76d0:	mov    %edx,%eax
-    646c76d2:	not    %eax
-    646c76d4:	mov    %eax,%ecx
-    646c76d6:	and    $0x1,%ecx
-    646c76d9:	test   %edx,%edx
-    646c76db:	jns    646c76e9 <__powi+0x229>
-    646c76dd:	test   %cl,%cl
-    646c76df:	pxor   %xmm6,%xmm6
-    646c76e3:	jne    646c7540 <__powi+0x80>
-    646c76e9:	shr    $0x1f,%eax
-    646c76ec:	test   $0x1,%dl
-    646c76ef:	je     646c7701 <__powi+0x241>
-    646c76f1:	test   %al,%al
-    646c76f3:	movsd  0x1e45(%rip),%xmm6        # 646c9540 <.rdata+0x30>
-    646c76fb:	jne    646c7540 <__powi+0x80>
-    646c7701:	test   %cl,%cl
-    646c7703:	je     646c7715 <__powi+0x255>
-    646c7705:	test   %al,%al
-    646c7707:	movsd  0x1e29(%rip),%xmm6        # 646c9538 <.rdata+0x28>
-    646c770f:	jne    646c7540 <__powi+0x80>
-    646c7715:	test   %edx,%edx
-    646c7717:	js     646c7730 <__powi+0x270>
-    646c7719:	and    $0x1,%dl
-    646c771c:	jne    646c762e <__powi+0x16e>
-    646c7722:	movsd  0x1e0e(%rip),%xmm6        # 646c9538 <.rdata+0x28>
-    646c772a:	jmp    646c7540 <__powi+0x80>
-    646c772f:	nop
-    646c7730:	test   %r9d,%r9d
-    646c7733:	jne    646c7538 <__powi+0x78>
-    646c7739:	jmp    646c75f9 <__powi+0x139>
-    646c773e:	nop
-    646c773f:	nop
-
-00000000646c7740 <exp2l>:
-    646c7740:	fldt   (%rdx)
-    646c7742:	fxam
-    646c7744:	fstsw  %ax
-    646c7747:	mov    $0x45,%dh
-    646c7749:	and    %ah,%dh
-    646c774b:	cmp    $0x5,%dh
-    646c774e:	je     646c778f <exp2l+0x4f>
-    646c7750:	fld    %st(0)
-    646c7752:	sub    $0x8,%rsp
-    646c7756:	fnstcw 0x4(%rsp)
-    646c775a:	movzwl 0x4(%rsp),%eax
-    646c775f:	or     $0xc,%ah
-    646c7762:	mov    %ax,(%rsp)
-    646c7766:	fldcw  (%rsp)
-    646c7769:	frndint
-    646c776b:	fldcw  0x4(%rsp)
-    646c776f:	add    $0x8,%rsp
-    646c7773:	fsubr  %st,%st(1)
-    646c7775:	fxch   %st(1)
-    646c7777:	f2xm1
-    646c7779:	fld1
-    646c777b:	faddp  %st,%st(1)
-    646c777d:	fscale
-    646c777f:	fstp   %st(1)
-    646c7781:	mov    %rcx,%rax
-    646c7784:	movq   $0x0,0x8(%rcx)
-    646c778c:	fstpt  (%rcx)
-    646c778e:	ret
-    646c778f:	test   $0x200,%eax
-    646c7794:	je     646c779a <exp2l+0x5a>
-    646c7796:	fstp   %st(0)
-    646c7798:	fldz
-    646c779a:	mov    %rcx,%rax
-    646c779d:	movq   $0x0,0x8(%rcx)
-    646c77a5:	fstpt  (%rcx)
-    646c77a7:	ret
-    646c77a8:	nop
-    646c77a9:	nop
-    646c77aa:	nop
-    646c77ab:	nop
-    646c77ac:	nop
-    646c77ad:	nop
-    646c77ae:	nop
-    646c77af:	nop
-
-00000000646c77b0 <one>:
-    646c77b0:	add    %al,(%rax)
-    646c77b2:	add    %al,(%rax)
-    646c77b4:	add    %al,(%rax)
-    646c77b6:	lock (bad)
-
-00000000646c77b8 <limit>:
-    646c77b8:	pop    %rdx
-    646c77ba:	cmc
-    646c77bb:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c77bf:	(bad)
-
-00000000646c77c0 <__logl_internal>:
-    646c77c0:	fldln2
-    646c77c2:	fldt   (%rdx)
-    646c77c4:	fld    %st(0)
-    646c77c6:	fsubl  -0x1c(%rip)        # 646c77b0 <one>
-    646c77cc:	fld    %st(0)
-    646c77ce:	fabs
-    646c77d0:	fcompl -0x1e(%rip)        # 646c77b8 <limit>
-    646c77d6:	fnstsw %ax
-    646c77d8:	and    $0x45,%ah
-    646c77db:	je     646c77ef <__logl_internal+0x2f>
-    646c77dd:	fstp   %st(1)
-    646c77df:	fyl2xp1
-    646c77e1:	mov    %rcx,%rax
-    646c77e4:	movq   $0x0,0x8(%rcx)
-    646c77ec:	fstpt  (%rcx)
-    646c77ee:	ret
-    646c77ef:	fstp   %st(0)
-    646c77f1:	fyl2x
-    646c77f3:	mov    %rcx,%rax
-    646c77f6:	movq   $0x0,0x8(%rcx)
-    646c77fe:	fstpt  (%rcx)
-    646c7800:	ret
-    646c7801:	nop
-    646c7802:	nop
-    646c7803:	nop
-    646c7804:	nop
-    646c7805:	nop
-    646c7806:	nop
-    646c7807:	nop
-    646c7808:	nop
-    646c7809:	nop
-    646c780a:	nop
-    646c780b:	nop
-    646c780c:	nop
-    646c780d:	nop
+    646c734b:	call   646c7750 <ldexp>
+    646c7350:	mov    %rbx,%rdx
+    646c7353:	call   646c6e00 <internal_modf>
+    646c7358:	test   %esi,%esi
+    646c735a:	js     646c7328 <pow+0x488>
+    646c735c:	ucomisd %xmm7,%xmm0
+    646c7360:	jp     646c7368 <pow+0x4c8>
+    646c7362:	je     646c70a2 <pow+0x202>
+    646c7368:	movsd  0x2158(%rip),%xmm6        # 646c94c8 <.rdata+0x18>
+    646c7370:	jmp    646c6fab <pow+0x10b>
+    646c7375:	movq   %rdi,%xmm5
+    646c737a:	xorpd  0x216e(%rip),%xmm5        # 646c94f0 <.rdata+0x40>
+    646c7382:	movq   %xmm5,%rax
+    646c7387:	movq   %rdi,%xmm5
+    646c738c:	ucomisd 0x216c(%rip),%xmm5        # 646c9500 <.rdata+0x50>
+    646c7394:	jp     646c73ef <pow+0x54f>
+    646c7396:	jne    646c73ef <pow+0x54f>
+    646c7398:	movapd %xmm2,%xmm6
+    646c739c:	jmp    646c6fab <pow+0x10b>
+    646c73a1:	mov    %rdi,0x30(%rsp)
+    646c73a6:	fldl   0x30(%rsp)
+    646c73aa:	fsqrt
+    646c73ac:	fstpl  0x30(%rsp)
+    646c73b0:	movsd  0x30(%rsp),%xmm6
+    646c73b6:	jmp    646c6fab <pow+0x10b>
+    646c73bb:	call   646c7918 <_errno>
+    646c73c0:	movsd  0x20f0(%rip),%xmm6        # 646c94b8 <.rdata+0x8>
+    646c73c8:	movl   $0x21,(%rax)
+    646c73ce:	jmp    646c701b <pow+0x17b>
+    646c73d3:	movq   %rbp,%xmm3
+    646c73d8:	movq   %rdi,%xmm0
+    646c73dd:	cvttsd2si %xmm3,%edx
+    646c73e1:	call   646c7400 <__powi>
+    646c73e6:	movapd %xmm0,%xmm6
+    646c73ea:	jmp    646c6fab <pow+0x10b>
+    646c73ef:	mov    %rax,%rdi
+    646c73f2:	jmp    646c70d4 <pow+0x234>
+    646c73f7:	nop
+    646c73f8:	nop
+    646c73f9:	nop
+    646c73fa:	nop
+    646c73fb:	nop
+    646c73fc:	nop
+    646c73fd:	nop
+    646c73fe:	nop
+    646c73ff:	nop
+
+00000000646c7400 <__powi>:
+    646c7400:	sub    $0x58,%rsp
+    646c7404:	movaps %xmm6,0x40(%rsp)
+    646c7409:	movsd  0x2137(%rip),%xmm1        # 646c9548 <.rdata+0x18>
+    646c7411:	mov    $0x0,%r10d
+    646c7417:	movq   %xmm0,%r8
+    646c741c:	movq   %xmm0,%rax
+    646c7421:	shr    $0x20,%r8
+    646c7425:	mov    %r8d,%ecx
+    646c7428:	mov    %r8d,%r9d
+    646c742b:	and    $0xfffff,%ecx
+    646c7431:	and    $0x7ff00000,%r9d
+    646c7438:	or     %eax,%ecx
+    646c743a:	ucomisd %xmm1,%xmm0
+    646c743e:	mov    %r9d,%r11d
+    646c7441:	setnp  %al
+    646c7444:	cmovne %r10d,%eax
+    646c7448:	test   %edx,%edx
+    646c744a:	sete   %r10b
+    646c744e:	or     %r10d,%eax
+    646c7451:	or     %ecx,%r11d
+    646c7454:	jne    646c7490 <__powi+0x90>
+    646c7456:	test   %al,%al
+    646c7458:	movapd %xmm1,%xmm6
+    646c745c:	jne    646c7480 <__powi+0x80>
+    646c745e:	mov    %edx,%eax
+    646c7460:	and    $0x1,%eax
+    646c7463:	test   %edx,%edx
+    646c7465:	js     646c7555 <__powi+0x155>
+    646c746b:	test   %eax,%eax
+    646c746d:	pxor   %xmm6,%xmm6
+    646c7471:	je     646c7480 <__powi+0x80>
+    646c7473:	test   %r8d,%r8d
+    646c7476:	jns    646c7480 <__powi+0x80>
+    646c7478:	movsd  0x20d0(%rip),%xmm6        # 646c9550 <.rdata+0x20>
+    646c7480:	movapd %xmm6,%xmm0
+    646c7484:	movaps 0x40(%rsp),%xmm6
+    646c7489:	add    $0x58,%rsp
+    646c748d:	ret
+    646c748e:	xchg   %ax,%ax
+    646c7490:	test   %r9d,%r9d
+    646c7493:	jne    646c7500 <__powi+0x100>
+    646c7495:	test   %al,%al
+    646c7497:	movapd %xmm1,%xmm6
+    646c749b:	jne    646c7480 <__powi+0x80>
+    646c749d:	mov    %edx,%eax
+    646c749f:	movapd %xmm0,%xmm6
+    646c74a3:	andpd  0x20c5(%rip),%xmm6        # 646c9570 <.rdata+0x40>
+    646c74ab:	and    $0x1,%eax
+    646c74ae:	test   %edx,%edx
+    646c74b0:	js     646c7542 <__powi+0x142>
+    646c74b6:	cmp    $0x1,%edx
+    646c74b9:	je     646c74e1 <__powi+0xe1>
+    646c74bb:	test   $0x1,%dl
+    646c74be:	jne    646c75f0 <__powi+0x1f0>
+    646c74c4:	movapd %xmm6,%xmm0
+    646c74c8:	shr    %edx
+    646c74ca:	movapd %xmm1,%xmm6
+    646c74ce:	xchg   %ax,%ax
+    646c74d0:	mulsd  %xmm0,%xmm0
+    646c74d4:	test   $0x1,%dl
+    646c74d7:	je     646c74dd <__powi+0xdd>
+    646c74d9:	mulsd  %xmm0,%xmm6
+    646c74dd:	shr    %edx
+    646c74df:	jne    646c74d0 <__powi+0xd0>
+    646c74e1:	shr    $0x1f,%r8d
+    646c74e5:	test   %r8b,%r8b
+    646c74e8:	je     646c7480 <__powi+0x80>
+    646c74ea:	test   %eax,%eax
+    646c74ec:	je     646c7480 <__powi+0x80>
+    646c74ee:	xorpd  0x208a(%rip),%xmm6        # 646c9580 <.rdata+0x50>
+    646c74f6:	jmp    646c7480 <__powi+0x80>
+    646c74f8:	nopl   0x0(%rax,%rax,1)
+    646c7500:	cmp    $0x7ff00000,%r9d
+    646c7507:	jne    646c7495 <__powi+0x95>
+    646c7509:	test   %ecx,%ecx
+    646c750b:	jne    646c7580 <__powi+0x180>
+    646c750d:	mov    %edx,%r9d
+    646c7510:	movapd %xmm1,%xmm6
+    646c7514:	and    $0x1,%r9d
+    646c7518:	test   %al,%al
+    646c751a:	jne    646c7480 <__powi+0x80>
+    646c7520:	test   %r8d,%r8d
+    646c7523:	js     646c7610 <__powi+0x210>
+    646c7529:	test   %edx,%edx
+    646c752b:	movsd  0x2025(%rip),%xmm6        # 646c9558 <.rdata+0x28>
+    646c7533:	jns    646c7480 <__powi+0x80>
+    646c7539:	pxor   %xmm6,%xmm6
+    646c753d:	jmp    646c7480 <__powi+0x80>
+    646c7542:	movapd %xmm1,%xmm4
+    646c7546:	neg    %edx
+    646c7548:	divsd  %xmm6,%xmm4
+    646c754c:	movapd %xmm4,%xmm6
+    646c7550:	jmp    646c74b6 <__powi+0xb6>
+    646c7555:	test   %eax,%eax
+    646c7557:	movsd  0x1ff9(%rip),%xmm6        # 646c9558 <.rdata+0x28>
+    646c755f:	je     646c7480 <__powi+0x80>
+    646c7565:	test   %r8d,%r8d
+    646c7568:	jns    646c7480 <__powi+0x80>
+    646c756e:	movsd  0x1fea(%rip),%xmm6        # 646c9560 <.rdata+0x30>
+    646c7576:	jmp    646c7480 <__powi+0x80>
+    646c757b:	nopl   0x0(%rax,%rax,1)
+    646c7580:	test   %al,%al
+    646c7582:	movapd %xmm1,%xmm6
+    646c7586:	jne    646c7480 <__powi+0x80>
+    646c758c:	test   %r8d,%r8d
+    646c758f:	movsd  0x1fa9(%rip),%xmm6        # 646c9540 <.rdata+0x10>
+    646c7597:	js     646c7600 <__powi+0x200>
+    646c7599:	mov    %edx,0x3c(%rsp)
+    646c759d:	movsd  %xmm0,0x30(%rsp)
+    646c75a3:	call   646c7918 <_errno>
+    646c75a8:	mov    0x3c(%rsp),%edx
+    646c75ac:	pxor   %xmm3,%xmm3
+    646c75b0:	mov    $0x1,%ecx
+    646c75b5:	movsd  0x30(%rsp),%xmm0
+    646c75bb:	movl   $0x21,(%rax)
+    646c75c1:	movsd  %xmm6,0x20(%rsp)
+    646c75c7:	movapd %xmm0,%xmm2
+    646c75cb:	cvtsi2sd %edx,%xmm3
+    646c75cf:	lea    0x1f5a(%rip),%rdx        # 646c9530 <.rdata>
+    646c75d6:	call   646c7b90 <__mingw_raise_matherr>
+    646c75db:	movapd %xmm6,%xmm0
+    646c75df:	movaps 0x40(%rsp),%xmm6
+    646c75e4:	add    $0x58,%rsp
+    646c75e8:	ret
+    646c75e9:	nopl   0x0(%rax)
+    646c75f0:	movapd %xmm6,%xmm1
+    646c75f4:	jmp    646c74c4 <__powi+0xc4>
+    646c75f9:	nopl   0x0(%rax)
+    646c7600:	movsd  0x1f30(%rip),%xmm6        # 646c9538 <.rdata+0x8>
+    646c7608:	jmp    646c7599 <__powi+0x199>
+    646c760a:	nopw   0x0(%rax,%rax,1)
+    646c7610:	mov    %edx,%eax
+    646c7612:	not    %eax
+    646c7614:	mov    %eax,%ecx
+    646c7616:	and    $0x1,%ecx
+    646c7619:	test   %edx,%edx
+    646c761b:	jns    646c7629 <__powi+0x229>
+    646c761d:	test   %cl,%cl
+    646c761f:	pxor   %xmm6,%xmm6
+    646c7623:	jne    646c7480 <__powi+0x80>
+    646c7629:	shr    $0x1f,%eax
+    646c762c:	test   $0x1,%dl
+    646c762f:	je     646c7641 <__powi+0x241>
+    646c7631:	test   %al,%al
+    646c7633:	movsd  0x1f25(%rip),%xmm6        # 646c9560 <.rdata+0x30>
+    646c763b:	jne    646c7480 <__powi+0x80>
+    646c7641:	test   %cl,%cl
+    646c7643:	je     646c7655 <__powi+0x255>
+    646c7645:	test   %al,%al
+    646c7647:	movsd  0x1f09(%rip),%xmm6        # 646c9558 <.rdata+0x28>
+    646c764f:	jne    646c7480 <__powi+0x80>
+    646c7655:	test   %edx,%edx
+    646c7657:	js     646c7670 <__powi+0x270>
+    646c7659:	and    $0x1,%dl
+    646c765c:	jne    646c756e <__powi+0x16e>
+    646c7662:	movsd  0x1eee(%rip),%xmm6        # 646c9558 <.rdata+0x28>
+    646c766a:	jmp    646c7480 <__powi+0x80>
+    646c766f:	nop
+    646c7670:	test   %r9d,%r9d
+    646c7673:	jne    646c7478 <__powi+0x78>
+    646c7679:	jmp    646c7539 <__powi+0x139>
+    646c767e:	nop
+    646c767f:	nop
+
+00000000646c7680 <exp2l>:
+    646c7680:	fldt   (%rdx)
+    646c7682:	fxam
+    646c7684:	fstsw  %ax
+    646c7687:	mov    $0x45,%dh
+    646c7689:	and    %ah,%dh
+    646c768b:	cmp    $0x5,%dh
+    646c768e:	je     646c76cf <exp2l+0x4f>
+    646c7690:	fld    %st(0)
+    646c7692:	sub    $0x8,%rsp
+    646c7696:	fnstcw 0x4(%rsp)
+    646c769a:	movzwl 0x4(%rsp),%eax
+    646c769f:	or     $0xc,%ah
+    646c76a2:	mov    %ax,(%rsp)
+    646c76a6:	fldcw  (%rsp)
+    646c76a9:	frndint
+    646c76ab:	fldcw  0x4(%rsp)
+    646c76af:	add    $0x8,%rsp
+    646c76b3:	fsubr  %st,%st(1)
+    646c76b5:	fxch   %st(1)
+    646c76b7:	f2xm1
+    646c76b9:	fld1
+    646c76bb:	faddp  %st,%st(1)
+    646c76bd:	fscale
+    646c76bf:	fstp   %st(1)
+    646c76c1:	mov    %rcx,%rax
+    646c76c4:	movq   $0x0,0x8(%rcx)
+    646c76cc:	fstpt  (%rcx)
+    646c76ce:	ret
+    646c76cf:	test   $0x200,%eax
+    646c76d4:	je     646c76da <exp2l+0x5a>
+    646c76d6:	fstp   %st(0)
+    646c76d8:	fldz
+    646c76da:	mov    %rcx,%rax
+    646c76dd:	movq   $0x0,0x8(%rcx)
+    646c76e5:	fstpt  (%rcx)
+    646c76e7:	ret
+    646c76e8:	nop
+    646c76e9:	nop
+    646c76ea:	nop
+    646c76eb:	nop
+    646c76ec:	nop
+    646c76ed:	nop
+    646c76ee:	nop
+    646c76ef:	nop
+
+00000000646c76f0 <one>:
+    646c76f0:	add    %al,(%rax)
+    646c76f2:	add    %al,(%rax)
+    646c76f4:	add    %al,(%rax)
+    646c76f6:	lock (bad)
+
+00000000646c76f8 <limit>:
+    646c76f8:	pop    %rdx
+    646c76fa:	cmc
+    646c76fb:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c76ff:	(bad)
+
+00000000646c7700 <__logl_internal>:
+    646c7700:	fldln2
+    646c7702:	fldt   (%rdx)
+    646c7704:	fld    %st(0)
+    646c7706:	fsubl  -0x1c(%rip)        # 646c76f0 <one>
+    646c770c:	fld    %st(0)
+    646c770e:	fabs
+    646c7710:	fcompl -0x1e(%rip)        # 646c76f8 <limit>
+    646c7716:	fnstsw %ax
+    646c7718:	and    $0x45,%ah
+    646c771b:	je     646c772f <__logl_internal+0x2f>
+    646c771d:	fstp   %st(1)
+    646c771f:	fyl2xp1
+    646c7721:	mov    %rcx,%rax
+    646c7724:	movq   $0x0,0x8(%rcx)
+    646c772c:	fstpt  (%rcx)
+    646c772e:	ret
+    646c772f:	fstp   %st(0)
+    646c7731:	fyl2x
+    646c7733:	mov    %rcx,%rax
+    646c7736:	movq   $0x0,0x8(%rcx)
+    646c773e:	fstpt  (%rcx)
+    646c7740:	ret
+    646c7741:	nop
+    646c7742:	nop
+    646c7743:	nop
+    646c7744:	nop
+    646c7745:	nop
+    646c7746:	nop
+    646c7747:	nop
+    646c7748:	nop
+    646c7749:	nop
+    646c774a:	nop
+    646c774b:	nop
+    646c774c:	nop
+    646c774d:	nop
+    646c774e:	nop
+    646c774f:	nop
+
+00000000646c7750 <ldexp>:
+    646c7750:	push   %rbx
+    646c7751:	sub    $0x30,%rsp
+    646c7755:	movq   %xmm0,%rax
+    646c775a:	movq   %xmm0,%rbx
+    646c775f:	shr    $0x20,%rax
+    646c7763:	mov    %eax,%r8d
+    646c7766:	and    $0x7fffffff,%r8d
+    646c776d:	or     %ebx,%r8d
+    646c7770:	sete   %r8b
+    646c7774:	and    $0x7ff00000,%eax
+    646c7779:	sete   %cl
+    646c777c:	or     %cl,%r8b
+    646c777f:	jne    646c7788 <ldexp+0x38>
+    646c7781:	cmp    $0x7ff00000,%eax
+    646c7786:	je     646c7803 <ldexp+0xb3>
+    646c7788:	movq   %rbx,%xmm1
+    646c778d:	pxor   %xmm0,%xmm0
+    646c7791:	ucomisd %xmm0,%xmm1
+    646c7795:	jp     646c7799 <ldexp+0x49>
+    646c7797:	je     646c7803 <ldexp+0xb3>
+    646c7799:	pxor   %xmm2,%xmm2
+    646c779d:	cvtsi2sd %edx,%xmm2
+    646c77a1:	mov    %rbx,0x20(%rsp)
+    646c77a6:	fldl   0x20(%rsp)
+    646c77aa:	movsd  %xmm2,0x28(%rsp)
+    646c77b0:	fldl   0x28(%rsp)
+    646c77b4:	fxch   %st(1)
+    646c77b6:	fscale
+    646c77b8:	fstp   %st(1)
+    646c77ba:	fstpl  0x20(%rsp)
+    646c77be:	mov    0x20(%rsp),%rbx
+    646c77c3:	mov    %rbx,%rax
+    646c77c6:	shr    $0x20,%rax
+    646c77ca:	mov    %eax,%ecx
+    646c77cc:	and    $0x7fffffff,%ecx
+    646c77d2:	or     %ebx,%ecx
+    646c77d4:	sete   %cl
+    646c77d7:	and    $0x7ff00000,%eax
+    646c77dc:	sete   %dl
+    646c77df:	or     %dl,%cl
+    646c77e1:	jne    646c77ea <ldexp+0x9a>
+    646c77e3:	cmp    $0x7ff00000,%eax
+    646c77e8:	je     646c77f8 <ldexp+0xa8>
+    646c77ea:	movsd  0x20(%rsp),%xmm3
+    646c77f0:	ucomisd %xmm0,%xmm3
+    646c77f4:	jp     646c7803 <ldexp+0xb3>
+    646c77f6:	jne    646c7803 <ldexp+0xb3>
+    646c77f8:	call   646c7918 <_errno>
+    646c77fd:	movl   $0x22,(%rax)
+    646c7803:	movq   %rbx,%xmm0
+    646c7808:	add    $0x30,%rsp
+    646c780c:	pop    %rbx
+    646c780d:	ret
     646c780e:	nop
     646c780f:	nop
 
-00000000646c7810 <ldexp>:
-    646c7810:	push   %rbx
-    646c7811:	sub    $0x30,%rsp
-    646c7815:	movq   %xmm0,%rax
-    646c781a:	movq   %xmm0,%rbx
-    646c781f:	shr    $0x20,%rax
-    646c7823:	mov    %eax,%r8d
-    646c7826:	and    $0x7fffffff,%r8d
-    646c782d:	or     %ebx,%r8d
-    646c7830:	sete   %r8b
-    646c7834:	and    $0x7ff00000,%eax
-    646c7839:	sete   %cl
-    646c783c:	or     %cl,%r8b
-    646c783f:	jne    646c7848 <ldexp+0x38>
-    646c7841:	cmp    $0x7ff00000,%eax
-    646c7846:	je     646c78c3 <ldexp+0xb3>
-    646c7848:	movq   %rbx,%xmm1
-    646c784d:	pxor   %xmm0,%xmm0
-    646c7851:	ucomisd %xmm0,%xmm1
-    646c7855:	jp     646c7859 <ldexp+0x49>
-    646c7857:	je     646c78c3 <ldexp+0xb3>
-    646c7859:	pxor   %xmm2,%xmm2
-    646c785d:	cvtsi2sd %edx,%xmm2
-    646c7861:	mov    %rbx,0x20(%rsp)
-    646c7866:	fldl   0x20(%rsp)
-    646c786a:	movsd  %xmm2,0x28(%rsp)
-    646c7870:	fldl   0x28(%rsp)
-    646c7874:	fxch   %st(1)
-    646c7876:	fscale
-    646c7878:	fstp   %st(1)
-    646c787a:	fstpl  0x20(%rsp)
-    646c787e:	mov    0x20(%rsp),%rbx
-    646c7883:	mov    %rbx,%rax
-    646c7886:	shr    $0x20,%rax
-    646c788a:	mov    %eax,%ecx
-    646c788c:	and    $0x7fffffff,%ecx
-    646c7892:	or     %ebx,%ecx
-    646c7894:	sete   %cl
-    646c7897:	and    $0x7ff00000,%eax
-    646c789c:	sete   %dl
-    646c789f:	or     %dl,%cl
-    646c78a1:	jne    646c78aa <ldexp+0x9a>
-    646c78a3:	cmp    $0x7ff00000,%eax
-    646c78a8:	je     646c78b8 <ldexp+0xa8>
-    646c78aa:	movsd  0x20(%rsp),%xmm3
-    646c78b0:	ucomisd %xmm0,%xmm3
-    646c78b4:	jp     646c78c3 <ldexp+0xb3>
-    646c78b6:	jne    646c78c3 <ldexp+0xb3>
-    646c78b8:	call   646c79d8 <_errno>
-    646c78bd:	movl   $0x22,(%rax)
-    646c78c3:	movq   %rbx,%xmm0
-    646c78c8:	add    $0x30,%rsp
-    646c78cc:	pop    %rbx
-    646c78cd:	ret
+00000000646c7810 <one>:
+    646c7810:	add    %al,(%rax)
+    646c7812:	add    %al,(%rax)
+    646c7814:	add    %al,(%rax)
+    646c7816:	lock (bad)
+
+00000000646c7818 <limit>:
+    646c7818:	pop    %rdx
+    646c781a:	cmc
+    646c781b:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c781f:	(bad)
+
+00000000646c7820 <log2l>:
+    646c7820:	fldl   -0x16(%rip)        # 646c7810 <one>
+    646c7826:	fldt   (%rdx)
+    646c7828:	fxam
+    646c782a:	fnstsw %ax
+    646c782c:	fld    %st(0)
+    646c782e:	sahf
+    646c782f:	jb     646c7868 <log2l+0x48>
+    646c7831:	fsub   %st(2),%st
+    646c7833:	fld    %st(0)
+    646c7835:	fabs
+    646c7837:	fcompl -0x25(%rip)        # 646c7818 <limit>
+    646c783d:	fnstsw %ax
+    646c783f:	and    $0x45,%ah
+    646c7842:	je     646c7856 <log2l+0x36>
+    646c7844:	fstp   %st(1)
+    646c7846:	fyl2xp1
+    646c7848:	mov    %rcx,%rax
+    646c784b:	movq   $0x0,0x8(%rcx)
+    646c7853:	fstpt  (%rcx)
+    646c7855:	ret
+    646c7856:	fstp   %st(0)
+    646c7858:	fyl2x
+    646c785a:	mov    %rcx,%rax
+    646c785d:	movq   $0x0,0x8(%rcx)
+    646c7865:	fstpt  (%rcx)
+    646c7867:	ret
+    646c7868:	jp     646c7831 <log2l+0x11>
+    646c786a:	fstp   %st(1)
+    646c786c:	fstp   %st(1)
+    646c786e:	mov    %rcx,%rax
+    646c7871:	movq   $0x0,0x8(%rcx)
+    646c7879:	fstpt  (%rcx)
+    646c787b:	ret
+    646c787c:	nop
+    646c787d:	nop
+    646c787e:	nop
+    646c787f:	nop
+
+00000000646c7880 <vfprintf>:
+    646c7880:	jmp    *0x6ac6(%rip)        # 646ce34c <__imp_vfprintf>
+    646c7886:	nop
+    646c7887:	nop
+
+00000000646c7888 <strncmp>:
+    646c7888:	jmp    *0x6ab6(%rip)        # 646ce344 <__imp_strncmp>
+    646c788e:	nop
+    646c788f:	nop
+
+00000000646c7890 <strlen>:
+    646c7890:	jmp    *0x6aa6(%rip)        # 646ce33c <__imp_strlen>
+    646c7896:	nop
+    646c7897:	nop
+
+00000000646c7898 <signal>:
+    646c7898:	jmp    *0x6a96(%rip)        # 646ce334 <__imp_signal>
+    646c789e:	nop
+    646c789f:	nop
+
+00000000646c78a0 <printf>:
+    646c78a0:	jmp    *0x6a7e(%rip)        # 646ce324 <__imp_printf>
+    646c78a6:	nop
+    646c78a7:	nop
+
+00000000646c78a8 <perror>:
+    646c78a8:	jmp    *0x6a6e(%rip)        # 646ce31c <__imp_perror>
+    646c78ae:	nop
+    646c78af:	nop
+
+00000000646c78b0 <malloc>:
+    646c78b0:	jmp    *0x6a5e(%rip)        # 646ce314 <__imp_malloc>
+    646c78b6:	nop
+    646c78b7:	nop
+
+00000000646c78b8 <log10>:
+    646c78b8:	jmp    *0x6a4e(%rip)        # 646ce30c <__imp_log10>
+    646c78be:	nop
+    646c78bf:	nop
+
+00000000646c78c0 <fwrite>:
+    646c78c0:	jmp    *0x6a3e(%rip)        # 646ce304 <__imp_fwrite>
+    646c78c6:	nop
+    646c78c7:	nop
+
+00000000646c78c8 <free>:
+    646c78c8:	jmp    *0x6a2e(%rip)        # 646ce2fc <__imp_free>
     646c78ce:	nop
     646c78cf:	nop
 
-00000000646c78d0 <one>:
-    646c78d0:	add    %al,(%rax)
-    646c78d2:	add    %al,(%rax)
-    646c78d4:	add    %al,(%rax)
-    646c78d6:	lock (bad)
-
-00000000646c78d8 <limit>:
-    646c78d8:	pop    %rdx
-    646c78da:	cmc
-    646c78db:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c78df:	(bad)
-
-00000000646c78e0 <log2l>:
-    646c78e0:	fldl   -0x16(%rip)        # 646c78d0 <one>
-    646c78e6:	fldt   (%rdx)
-    646c78e8:	fxam
-    646c78ea:	fnstsw %ax
-    646c78ec:	fld    %st(0)
-    646c78ee:	sahf
-    646c78ef:	jb     646c7928 <log2l+0x48>
-    646c78f1:	fsub   %st(2),%st
-    646c78f3:	fld    %st(0)
-    646c78f5:	fabs
-    646c78f7:	fcompl -0x25(%rip)        # 646c78d8 <limit>
-    646c78fd:	fnstsw %ax
-    646c78ff:	and    $0x45,%ah
-    646c7902:	je     646c7916 <log2l+0x36>
-    646c7904:	fstp   %st(1)
-    646c7906:	fyl2xp1
-    646c7908:	mov    %rcx,%rax
-    646c790b:	movq   $0x0,0x8(%rcx)
-    646c7913:	fstpt  (%rcx)
-    646c7915:	ret
-    646c7916:	fstp   %st(0)
-    646c7918:	fyl2x
-    646c791a:	mov    %rcx,%rax
-    646c791d:	movq   $0x0,0x8(%rcx)
-    646c7925:	fstpt  (%rcx)
-    646c7927:	ret
-    646c7928:	jp     646c78f1 <log2l+0x11>
-    646c792a:	fstp   %st(1)
-    646c792c:	fstp   %st(1)
-    646c792e:	mov    %rcx,%rax
-    646c7931:	movq   $0x0,0x8(%rcx)
-    646c7939:	fstpt  (%rcx)
-    646c793b:	ret
-    646c793c:	nop
-    646c793d:	nop
-    646c793e:	nop
-    646c793f:	nop
-
-00000000646c7940 <vfprintf>:
-    646c7940:	jmp    *0x6a06(%rip)        # 646ce34c <__imp_vfprintf>
-    646c7946:	nop
-    646c7947:	nop
-
-00000000646c7948 <strncmp>:
-    646c7948:	jmp    *0x69f6(%rip)        # 646ce344 <__imp_strncmp>
-    646c794e:	nop
-    646c794f:	nop
-
-00000000646c7950 <strlen>:
-    646c7950:	jmp    *0x69e6(%rip)        # 646ce33c <__imp_strlen>
-    646c7956:	nop
-    646c7957:	nop
-
-00000000646c7958 <signal>:
-    646c7958:	jmp    *0x69d6(%rip)        # 646ce334 <__imp_signal>
-    646c795e:	nop
-    646c795f:	nop
-
-00000000646c7960 <printf>:
-    646c7960:	jmp    *0x69be(%rip)        # 646ce324 <__imp_printf>
-    646c7966:	nop
-    646c7967:	nop
-
-00000000646c7968 <perror>:
-    646c7968:	jmp    *0x69ae(%rip)        # 646ce31c <__imp_perror>
-    646c796e:	nop
-    646c796f:	nop
-
-00000000646c7970 <malloc>:
-    646c7970:	jmp    *0x699e(%rip)        # 646ce314 <__imp_malloc>
-    646c7976:	nop
-    646c7977:	nop
-
-00000000646c7978 <log10>:
-    646c7978:	jmp    *0x698e(%rip)        # 646ce30c <__imp_log10>
-    646c797e:	nop
-    646c797f:	nop
-
-00000000646c7980 <fwrite>:
-    646c7980:	jmp    *0x697e(%rip)        # 646ce304 <__imp_fwrite>
-    646c7986:	nop
-    646c7987:	nop
-
-00000000646c7988 <free>:
-    646c7988:	jmp    *0x696e(%rip)        # 646ce2fc <__imp_free>
-    646c798e:	nop
-    646c798f:	nop
-
-00000000646c7990 <fprintf>:
-    646c7990:	jmp    *0x695e(%rip)        # 646ce2f4 <__imp_fprintf>
-    646c7996:	nop
-    646c7997:	nop
-
-00000000646c7998 <fopen>:
-    646c7998:	jmp    *0x694e(%rip)        # 646ce2ec <__imp_fopen>
-    646c799e:	nop
-    646c799f:	nop
-
-00000000646c79a0 <fclose>:
-    646c79a0:	jmp    *0x693e(%rip)        # 646ce2e4 <__imp_fclose>
-    646c79a6:	nop
-    646c79a7:	nop
-
-00000000646c79a8 <exit>:
-    646c79a8:	jmp    *0x692e(%rip)        # 646ce2dc <__imp_exit>
-    646c79ae:	nop
-    646c79af:	nop
-
-00000000646c79b0 <calloc>:
-    646c79b0:	jmp    *0x691e(%rip)        # 646ce2d4 <__imp_calloc>
-    646c79b6:	nop
-    646c79b7:	nop
-
-00000000646c79b8 <abort>:
-    646c79b8:	jmp    *0x690e(%rip)        # 646ce2cc <__imp_abort>
-    646c79be:	nop
-    646c79bf:	nop
-
-00000000646c79c0 <_vsnprintf>:
-    646c79c0:	jmp    *0x68fe(%rip)        # 646ce2c4 <__imp__vsnprintf>
-    646c79c6:	nop
-    646c79c7:	nop
-
-00000000646c79c8 <_mkdir>:
-    646c79c8:	jmp    *0x68e6(%rip)        # 646ce2b4 <__imp__mkdir>
-    646c79ce:	nop
-    646c79cf:	nop
-
-00000000646c79d0 <_initterm>:
-    646c79d0:	jmp    *0x68ce(%rip)        # 646ce2a4 <__imp__initterm>
-    646c79d6:	nop
-    646c79d7:	nop
-
-00000000646c79d8 <_errno>:
-    646c79d8:	jmp    *0x68be(%rip)        # 646ce29c <__imp__errno>
-    646c79de:	nop
-    646c79df:	nop
-
-00000000646c79e0 <_amsg_exit>:
-    646c79e0:	jmp    *0x68ae(%rip)        # 646ce294 <__imp__amsg_exit>
-    646c79e6:	nop
-    646c79e7:	nop
-    646c79e8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c79f0 <_initialize_onexit_table>:
-    646c79f0:	test   %rcx,%rcx
-    646c79f3:	je     646c7a0f <_initialize_onexit_table+0x1f>
-    646c79f5:	xor    %eax,%eax
-    646c79f7:	movq   $0x0,0x10(%rcx)
-    646c79ff:	movq   $0x0,0x8(%rcx)
-    646c7a07:	movq   $0x0,(%rcx)
-    646c7a0e:	ret
-    646c7a0f:	mov    $0xffffffff,%eax
-    646c7a14:	ret
-    646c7a15:	nop
-    646c7a16:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7a20 <_register_onexit_function>:
-    646c7a20:	push   %rbp
-    646c7a21:	push   %rdi
-    646c7a22:	push   %rsi
-    646c7a23:	push   %rbx
-    646c7a24:	sub    $0x28,%rsp
-    646c7a28:	test   %rcx,%rcx
-    646c7a2b:	mov    %rcx,%rbx
-    646c7a2e:	mov    %rdx,%rdi
-    646c7a31:	je     646c7ad0 <_register_onexit_function+0xb0>
-    646c7a37:	mov    $0x8,%ecx
-    646c7a3c:	call   646c7b90 <_lock>
-    646c7a41:	cmpq   $0x0,(%rbx)
-    646c7a45:	je     646c7aa4 <_register_onexit_function+0x84>
-    646c7a47:	mov    0x8(%rbx),%rsi
-    646c7a4b:	mov    0x10(%rbx),%rax
-    646c7a4f:	cmp    %rsi,%rax
-    646c7a52:	je     646c7a74 <_register_onexit_function+0x54>
-    646c7a54:	lea    0x8(%rsi),%rax
-    646c7a58:	mov    $0x8,%ecx
-    646c7a5d:	mov    %rax,0x8(%rbx)
-    646c7a61:	mov    %rdi,(%rsi)
-    646c7a64:	call   646c7b88 <_unlock>
-    646c7a69:	xor    %eax,%eax
-    646c7a6b:	add    $0x28,%rsp
-    646c7a6f:	pop    %rbx
-    646c7a70:	pop    %rsi
-    646c7a71:	pop    %rdi
-    646c7a72:	pop    %rbp
-    646c7a73:	ret
-    646c7a74:	mov    (%rbx),%rcx
-    646c7a77:	sub    %rcx,%rsi
-    646c7a7a:	mov    %rsi,%rax
-    646c7a7d:	sar    $0x3,%rax
-    646c7a81:	shl    $0x4,%rax
-    646c7a85:	mov    %rax,%rdx
-    646c7a88:	mov    %rax,%rbp
-    646c7a8b:	call   646c7b80 <realloc>
-    646c7a90:	test   %rax,%rax
-    646c7a93:	je     646c7ad7 <_register_onexit_function+0xb7>
-    646c7a95:	mov    %rax,(%rbx)
-    646c7a98:	add    %rax,%rsi
-    646c7a9b:	add    %rbp,%rax
-    646c7a9e:	mov    %rax,0x10(%rbx)
-    646c7aa2:	jmp    646c7a54 <_register_onexit_function+0x34>
-    646c7aa4:	mov    $0x8,%edx
-    646c7aa9:	mov    $0x20,%ecx
-    646c7aae:	call   646c79b0 <calloc>
-    646c7ab3:	test   %rax,%rax
-    646c7ab6:	mov    %rax,%rsi
-    646c7ab9:	mov    %rax,(%rbx)
-    646c7abc:	je     646c7ad7 <_register_onexit_function+0xb7>
-    646c7abe:	mov    %rax,0x8(%rbx)
-    646c7ac2:	lea    0x100(%rax),%rax
-    646c7ac9:	mov    %rax,0x10(%rbx)
-    646c7acd:	jmp    646c7a4f <_register_onexit_function+0x2f>
+00000000646c78d0 <fprintf>:
+    646c78d0:	jmp    *0x6a1e(%rip)        # 646ce2f4 <__imp_fprintf>
+    646c78d6:	nop
+    646c78d7:	nop
+
+00000000646c78d8 <fopen>:
+    646c78d8:	jmp    *0x6a0e(%rip)        # 646ce2ec <__imp_fopen>
+    646c78de:	nop
+    646c78df:	nop
+
+00000000646c78e0 <fclose>:
+    646c78e0:	jmp    *0x69fe(%rip)        # 646ce2e4 <__imp_fclose>
+    646c78e6:	nop
+    646c78e7:	nop
+
+00000000646c78e8 <exit>:
+    646c78e8:	jmp    *0x69ee(%rip)        # 646ce2dc <__imp_exit>
+    646c78ee:	nop
+    646c78ef:	nop
+
+00000000646c78f0 <calloc>:
+    646c78f0:	jmp    *0x69de(%rip)        # 646ce2d4 <__imp_calloc>
+    646c78f6:	nop
+    646c78f7:	nop
+
+00000000646c78f8 <abort>:
+    646c78f8:	jmp    *0x69ce(%rip)        # 646ce2cc <__imp_abort>
+    646c78fe:	nop
+    646c78ff:	nop
+
+00000000646c7900 <_vsnprintf>:
+    646c7900:	jmp    *0x69be(%rip)        # 646ce2c4 <__imp__vsnprintf>
+    646c7906:	nop
+    646c7907:	nop
+
+00000000646c7908 <_mkdir>:
+    646c7908:	jmp    *0x69a6(%rip)        # 646ce2b4 <__imp__mkdir>
+    646c790e:	nop
+    646c790f:	nop
+
+00000000646c7910 <_initterm>:
+    646c7910:	jmp    *0x698e(%rip)        # 646ce2a4 <__imp__initterm>
+    646c7916:	nop
+    646c7917:	nop
+
+00000000646c7918 <_errno>:
+    646c7918:	jmp    *0x697e(%rip)        # 646ce29c <__imp__errno>
+    646c791e:	nop
+    646c791f:	nop
+
+00000000646c7920 <_amsg_exit>:
+    646c7920:	jmp    *0x696e(%rip)        # 646ce294 <__imp__amsg_exit>
+    646c7926:	nop
+    646c7927:	nop
+    646c7928:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7930 <_initialize_onexit_table>:
+    646c7930:	test   %rcx,%rcx
+    646c7933:	je     646c794f <_initialize_onexit_table+0x1f>
+    646c7935:	xor    %eax,%eax
+    646c7937:	movq   $0x0,0x10(%rcx)
+    646c793f:	movq   $0x0,0x8(%rcx)
+    646c7947:	movq   $0x0,(%rcx)
+    646c794e:	ret
+    646c794f:	mov    $0xffffffff,%eax
+    646c7954:	ret
+    646c7955:	nop
+    646c7956:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7960 <_register_onexit_function>:
+    646c7960:	push   %rbp
+    646c7961:	push   %rdi
+    646c7962:	push   %rsi
+    646c7963:	push   %rbx
+    646c7964:	sub    $0x28,%rsp
+    646c7968:	test   %rcx,%rcx
+    646c796b:	mov    %rcx,%rbx
+    646c796e:	mov    %rdx,%rdi
+    646c7971:	je     646c7a10 <_register_onexit_function+0xb0>
+    646c7977:	mov    $0x8,%ecx
+    646c797c:	call   646c7ad0 <_lock>
+    646c7981:	cmpq   $0x0,(%rbx)
+    646c7985:	je     646c79e4 <_register_onexit_function+0x84>
+    646c7987:	mov    0x8(%rbx),%rsi
+    646c798b:	mov    0x10(%rbx),%rax
+    646c798f:	cmp    %rsi,%rax
+    646c7992:	je     646c79b4 <_register_onexit_function+0x54>
+    646c7994:	lea    0x8(%rsi),%rax
+    646c7998:	mov    $0x8,%ecx
+    646c799d:	mov    %rax,0x8(%rbx)
+    646c79a1:	mov    %rdi,(%rsi)
+    646c79a4:	call   646c7ac8 <_unlock>
+    646c79a9:	xor    %eax,%eax
+    646c79ab:	add    $0x28,%rsp
+    646c79af:	pop    %rbx
+    646c79b0:	pop    %rsi
+    646c79b1:	pop    %rdi
+    646c79b2:	pop    %rbp
+    646c79b3:	ret
+    646c79b4:	mov    (%rbx),%rcx
+    646c79b7:	sub    %rcx,%rsi
+    646c79ba:	mov    %rsi,%rax
+    646c79bd:	sar    $0x3,%rax
+    646c79c1:	shl    $0x4,%rax
+    646c79c5:	mov    %rax,%rdx
+    646c79c8:	mov    %rax,%rbp
+    646c79cb:	call   646c7ac0 <realloc>
+    646c79d0:	test   %rax,%rax
+    646c79d3:	je     646c7a17 <_register_onexit_function+0xb7>
+    646c79d5:	mov    %rax,(%rbx)
+    646c79d8:	add    %rax,%rsi
+    646c79db:	add    %rbp,%rax
+    646c79de:	mov    %rax,0x10(%rbx)
+    646c79e2:	jmp    646c7994 <_register_onexit_function+0x34>
+    646c79e4:	mov    $0x8,%edx
+    646c79e9:	mov    $0x20,%ecx
+    646c79ee:	call   646c78f0 <calloc>
+    646c79f3:	test   %rax,%rax
+    646c79f6:	mov    %rax,%rsi
+    646c79f9:	mov    %rax,(%rbx)
+    646c79fc:	je     646c7a17 <_register_onexit_function+0xb7>
+    646c79fe:	mov    %rax,0x8(%rbx)
+    646c7a02:	lea    0x100(%rax),%rax
+    646c7a09:	mov    %rax,0x10(%rbx)
+    646c7a0d:	jmp    646c798f <_register_onexit_function+0x2f>
+    646c7a0f:	nop
+    646c7a10:	mov    $0xffffffff,%eax
+    646c7a15:	jmp    646c79ab <_register_onexit_function+0x4b>
+    646c7a17:	mov    $0x8,%ecx
+    646c7a1c:	call   646c7ac8 <_unlock>
+    646c7a21:	mov    $0xffffffff,%eax
+    646c7a26:	jmp    646c79ab <_register_onexit_function+0x4b>
+    646c7a28:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7a30 <_execute_onexit_table>:
+    646c7a30:	push   %rdi
+    646c7a31:	push   %rsi
+    646c7a32:	push   %rbx
+    646c7a33:	sub    $0x20,%rsp
+    646c7a37:	mov    %rcx,%rdi
+    646c7a3a:	mov    $0x8,%ecx
+    646c7a3f:	call   646c7ad0 <_lock>
+    646c7a44:	mov    (%rdi),%rsi
+    646c7a47:	mov    $0x8,%ecx
+    646c7a4c:	movq   $0x0,0x10(%rdi)
+    646c7a54:	mov    0x8(%rdi),%rbx
+    646c7a58:	movq   $0x0,(%rdi)
+    646c7a5f:	movq   $0x0,0x8(%rdi)
+    646c7a67:	call   646c7ac8 <_unlock>
+    646c7a6c:	test   %rsi,%rsi
+    646c7a6f:	je     646c7a95 <_execute_onexit_table+0x65>
+    646c7a71:	sub    $0x8,%rbx
+    646c7a75:	cmp    %rbx,%rsi
+    646c7a78:	ja     646c7a8d <_execute_onexit_table+0x5d>
+    646c7a7a:	mov    (%rbx),%rax
+    646c7a7d:	test   %rax,%rax
+    646c7a80:	je     646c7a71 <_execute_onexit_table+0x41>
+    646c7a82:	call   *%rax
+    646c7a84:	sub    $0x8,%rbx
+    646c7a88:	cmp    %rbx,%rsi
+    646c7a8b:	jbe    646c7a7a <_execute_onexit_table+0x4a>
+    646c7a8d:	mov    %rsi,%rcx
+    646c7a90:	call   646c78c8 <free>
+    646c7a95:	xor    %eax,%eax
+    646c7a97:	add    $0x20,%rsp
+    646c7a9b:	pop    %rbx
+    646c7a9c:	pop    %rsi
+    646c7a9d:	pop    %rdi
+    646c7a9e:	ret
+    646c7a9f:	nop
+
+00000000646c7aa0 <__acrt_iob_func>:
+    646c7aa0:	push   %rbx
+    646c7aa1:	sub    $0x20,%rsp
+    646c7aa5:	mov    %ecx,%ebx
+    646c7aa7:	call   646c7ad8 <__iob_func>
+    646c7aac:	mov    %ebx,%ecx
+    646c7aae:	lea    (%rcx,%rcx,2),%rdx
+    646c7ab2:	shl    $0x4,%rdx
+    646c7ab6:	add    %rdx,%rax
+    646c7ab9:	add    $0x20,%rsp
+    646c7abd:	pop    %rbx
+    646c7abe:	ret
+    646c7abf:	nop
+
+00000000646c7ac0 <realloc>:
+    646c7ac0:	jmp    *0x6866(%rip)        # 646ce32c <__imp_realloc>
+    646c7ac6:	nop
+    646c7ac7:	nop
+
+00000000646c7ac8 <_unlock>:
+    646c7ac8:	jmp    *0x67ee(%rip)        # 646ce2bc <__imp__unlock>
+    646c7ace:	nop
     646c7acf:	nop
-    646c7ad0:	mov    $0xffffffff,%eax
-    646c7ad5:	jmp    646c7a6b <_register_onexit_function+0x4b>
-    646c7ad7:	mov    $0x8,%ecx
-    646c7adc:	call   646c7b88 <_unlock>
-    646c7ae1:	mov    $0xffffffff,%eax
-    646c7ae6:	jmp    646c7a6b <_register_onexit_function+0x4b>
-    646c7ae8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7af0 <_execute_onexit_table>:
-    646c7af0:	push   %rdi
-    646c7af1:	push   %rsi
-    646c7af2:	push   %rbx
-    646c7af3:	sub    $0x20,%rsp
-    646c7af7:	mov    %rcx,%rdi
-    646c7afa:	mov    $0x8,%ecx
-    646c7aff:	call   646c7b90 <_lock>
-    646c7b04:	mov    (%rdi),%rsi
-    646c7b07:	mov    $0x8,%ecx
-    646c7b0c:	movq   $0x0,0x10(%rdi)
-    646c7b14:	mov    0x8(%rdi),%rbx
-    646c7b18:	movq   $0x0,(%rdi)
-    646c7b1f:	movq   $0x0,0x8(%rdi)
-    646c7b27:	call   646c7b88 <_unlock>
-    646c7b2c:	test   %rsi,%rsi
-    646c7b2f:	je     646c7b55 <_execute_onexit_table+0x65>
-    646c7b31:	sub    $0x8,%rbx
-    646c7b35:	cmp    %rbx,%rsi
-    646c7b38:	ja     646c7b4d <_execute_onexit_table+0x5d>
-    646c7b3a:	mov    (%rbx),%rax
-    646c7b3d:	test   %rax,%rax
-    646c7b40:	je     646c7b31 <_execute_onexit_table+0x41>
-    646c7b42:	call   *%rax
-    646c7b44:	sub    $0x8,%rbx
-    646c7b48:	cmp    %rbx,%rsi
-    646c7b4b:	jbe    646c7b3a <_execute_onexit_table+0x4a>
-    646c7b4d:	mov    %rsi,%rcx
-    646c7b50:	call   646c7988 <free>
-    646c7b55:	xor    %eax,%eax
-    646c7b57:	add    $0x20,%rsp
-    646c7b5b:	pop    %rbx
-    646c7b5c:	pop    %rsi
-    646c7b5d:	pop    %rdi
-    646c7b5e:	ret
+
+00000000646c7ad0 <_lock>:
+    646c7ad0:	jmp    *0x67d6(%rip)        # 646ce2ac <__imp__lock>
+    646c7ad6:	nop
+    646c7ad7:	nop
+
+00000000646c7ad8 <__iob_func>:
+    646c7ad8:	jmp    *0x67a6(%rip)        # 646ce284 <__imp___iob_func>
+    646c7ade:	nop
+    646c7adf:	nop
+
+00000000646c7ae0 <VirtualQuery>:
+    646c7ae0:	jmp    *0x678e(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c7ae6:	nop
+    646c7ae7:	nop
+
+00000000646c7ae8 <VirtualProtect>:
+    646c7ae8:	jmp    *0x677e(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c7aee:	nop
+    646c7aef:	nop
+
+00000000646c7af0 <UnhandledExceptionFilter>:
+    646c7af0:	jmp    *0x676e(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c7af6:	nop
+    646c7af7:	nop
+
+00000000646c7af8 <TlsGetValue>:
+    646c7af8:	jmp    *0x675e(%rip)        # 646ce25c <__imp_TlsGetValue>
+    646c7afe:	nop
+    646c7aff:	nop
+
+00000000646c7b00 <TerminateProcess>:
+    646c7b00:	jmp    *0x674e(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c7b06:	nop
+    646c7b07:	nop
+
+00000000646c7b08 <SetUnhandledExceptionFilter>:
+    646c7b08:	jmp    *0x6736(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c7b0e:	nop
+    646c7b0f:	nop
+
+00000000646c7b10 <RtlVirtualUnwind>:
+    646c7b10:	jmp    *0x6726(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c7b16:	nop
+    646c7b17:	nop
+
+00000000646c7b18 <RtlLookupFunctionEntry>:
+    646c7b18:	jmp    *0x6716(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c7b1e:	nop
+    646c7b1f:	nop
+
+00000000646c7b20 <RtlCaptureContext>:
+    646c7b20:	jmp    *0x6706(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c7b26:	nop
+    646c7b27:	nop
+
+00000000646c7b28 <RtlAddFunctionTable>:
+    646c7b28:	jmp    *0x66f6(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c7b2e:	nop
+    646c7b2f:	nop
+
+00000000646c7b30 <QueryPerformanceCounter>:
+    646c7b30:	jmp    *0x66e6(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c7b36:	nop
+    646c7b37:	nop
+
+00000000646c7b38 <LeaveCriticalSection>:
+    646c7b38:	jmp    *0x66d6(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c7b3e:	nop
+    646c7b3f:	nop
+
+00000000646c7b40 <InitializeCriticalSection>:
+    646c7b40:	jmp    *0x66c6(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c7b46:	nop
+    646c7b47:	nop
+
+00000000646c7b48 <GetTickCount>:
+    646c7b48:	jmp    *0x66b6(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c7b4e:	nop
+    646c7b4f:	nop
+
+00000000646c7b50 <GetSystemTimeAsFileTime>:
+    646c7b50:	jmp    *0x66a6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c7b56:	nop
+    646c7b57:	nop
+
+00000000646c7b58 <GetLastError>:
+    646c7b58:	jmp    *0x6696(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c7b5e:	nop
     646c7b5f:	nop
 
-00000000646c7b60 <__acrt_iob_func>:
-    646c7b60:	push   %rbx
-    646c7b61:	sub    $0x20,%rsp
-    646c7b65:	mov    %ecx,%ebx
-    646c7b67:	call   646c7b98 <__iob_func>
-    646c7b6c:	mov    %ebx,%ecx
-    646c7b6e:	lea    (%rcx,%rcx,2),%rdx
-    646c7b72:	shl    $0x4,%rdx
-    646c7b76:	add    %rdx,%rax
-    646c7b79:	add    $0x20,%rsp
-    646c7b7d:	pop    %rbx
-    646c7b7e:	ret
+00000000646c7b60 <GetCurrentThreadId>:
+    646c7b60:	jmp    *0x6686(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c7b66:	nop
+    646c7b67:	nop
+
+00000000646c7b68 <GetCurrentProcessId>:
+    646c7b68:	jmp    *0x6676(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c7b6e:	nop
+    646c7b6f:	nop
+
+00000000646c7b70 <GetCurrentProcess>:
+    646c7b70:	jmp    *0x6666(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c7b76:	nop
+    646c7b77:	nop
+
+00000000646c7b78 <EnterCriticalSection>:
+    646c7b78:	jmp    *0x6656(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c7b7e:	nop
     646c7b7f:	nop
 
-00000000646c7b80 <realloc>:
-    646c7b80:	jmp    *0x67a6(%rip)        # 646ce32c <__imp_realloc>
+00000000646c7b80 <DeleteCriticalSection>:
+    646c7b80:	jmp    *0x6646(%rip)        # 646ce1cc <__IAT_start__>
     646c7b86:	nop
     646c7b87:	nop
+    646c7b88:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7b88 <_unlock>:
-    646c7b88:	jmp    *0x672e(%rip)        # 646ce2bc <__imp__unlock>
-    646c7b8e:	nop
-    646c7b8f:	nop
-
-00000000646c7b90 <_lock>:
-    646c7b90:	jmp    *0x6716(%rip)        # 646ce2ac <__imp__lock>
-    646c7b96:	nop
-    646c7b97:	nop
-
-00000000646c7b98 <__iob_func>:
-    646c7b98:	jmp    *0x66e6(%rip)        # 646ce284 <__imp___iob_func>
-    646c7b9e:	nop
-    646c7b9f:	nop
-
-00000000646c7ba0 <VirtualQuery>:
-    646c7ba0:	jmp    *0x66ce(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c7ba6:	nop
-    646c7ba7:	nop
-
-00000000646c7ba8 <VirtualProtect>:
-    646c7ba8:	jmp    *0x66be(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c7bae:	nop
-    646c7baf:	nop
-
-00000000646c7bb0 <UnhandledExceptionFilter>:
-    646c7bb0:	jmp    *0x66ae(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c7bb6:	nop
-    646c7bb7:	nop
-
-00000000646c7bb8 <TlsGetValue>:
-    646c7bb8:	jmp    *0x669e(%rip)        # 646ce25c <__imp_TlsGetValue>
-    646c7bbe:	nop
-    646c7bbf:	nop
-
-00000000646c7bc0 <TerminateProcess>:
-    646c7bc0:	jmp    *0x668e(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c7bc6:	nop
-    646c7bc7:	nop
-
-00000000646c7bc8 <SetUnhandledExceptionFilter>:
-    646c7bc8:	jmp    *0x6676(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c7bce:	nop
-    646c7bcf:	nop
-
-00000000646c7bd0 <RtlVirtualUnwind>:
-    646c7bd0:	jmp    *0x6666(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c7bd6:	nop
-    646c7bd7:	nop
-
-00000000646c7bd8 <RtlLookupFunctionEntry>:
-    646c7bd8:	jmp    *0x6656(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c7bde:	nop
-    646c7bdf:	nop
-
-00000000646c7be0 <RtlCaptureContext>:
-    646c7be0:	jmp    *0x6646(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c7be6:	nop
-    646c7be7:	nop
-
-00000000646c7be8 <RtlAddFunctionTable>:
-    646c7be8:	jmp    *0x6636(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c7bee:	nop
-    646c7bef:	nop
-
-00000000646c7bf0 <QueryPerformanceCounter>:
-    646c7bf0:	jmp    *0x6626(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c7bf6:	nop
-    646c7bf7:	nop
-
-00000000646c7bf8 <LeaveCriticalSection>:
-    646c7bf8:	jmp    *0x6616(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c7bfe:	nop
-    646c7bff:	nop
-
-00000000646c7c00 <InitializeCriticalSection>:
-    646c7c00:	jmp    *0x6606(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c7c06:	nop
-    646c7c07:	nop
-
-00000000646c7c08 <GetTickCount>:
-    646c7c08:	jmp    *0x65f6(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c7c0e:	nop
-    646c7c0f:	nop
-
-00000000646c7c10 <GetSystemTimeAsFileTime>:
-    646c7c10:	jmp    *0x65e6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c7c16:	nop
-    646c7c17:	nop
-
-00000000646c7c18 <GetLastError>:
-    646c7c18:	jmp    *0x65d6(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c7c1e:	nop
-    646c7c1f:	nop
-
-00000000646c7c20 <GetCurrentThreadId>:
-    646c7c20:	jmp    *0x65c6(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c7c26:	nop
-    646c7c27:	nop
-
-00000000646c7c28 <GetCurrentProcessId>:
-    646c7c28:	jmp    *0x65b6(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c7c2e:	nop
-    646c7c2f:	nop
-
-00000000646c7c30 <GetCurrentProcess>:
-    646c7c30:	jmp    *0x65a6(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c7c36:	nop
-    646c7c37:	nop
-
-00000000646c7c38 <EnterCriticalSection>:
-    646c7c38:	jmp    *0x6596(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c7c3e:	nop
-    646c7c3f:	nop
-
-00000000646c7c40 <DeleteCriticalSection>:
-    646c7c40:	jmp    *0x6586(%rip)        # 646ce1cc <__IAT_start__>
-    646c7c46:	nop
-    646c7c47:	nop
-    646c7c48:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7c50 <__mingw_raise_matherr>:
-    646c7c50:	sub    $0x58,%rsp
-    646c7c54:	mov    0x4ed5(%rip),%rax        # 646ccb30 <stUserMathErr>
-    646c7c5b:	test   %rax,%rax
-    646c7c5e:	je     646c7c8c <__mingw_raise_matherr+0x3c>
-    646c7c60:	movsd  0x80(%rsp),%xmm0
-    646c7c69:	mov    %ecx,0x20(%rsp)
-    646c7c6d:	lea    0x20(%rsp),%rcx
-    646c7c72:	mov    %rdx,0x28(%rsp)
-    646c7c77:	movsd  %xmm2,0x30(%rsp)
-    646c7c7d:	movsd  %xmm3,0x38(%rsp)
-    646c7c83:	movsd  %xmm0,0x40(%rsp)
-    646c7c89:	call   *%rax
-    646c7c8b:	nop
-    646c7c8c:	add    $0x58,%rsp
-    646c7c90:	ret
-    646c7c91:	nopl   0x0(%rax,%rax,1)
-    646c7c96:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7ca0 <__mingw_setusermatherr>:
-    646c7ca0:	mov    %rcx,0x4e89(%rip)        # 646ccb30 <stUserMathErr>
-    646c7ca7:	jmp    646c7db0 <__setusermatherr>
+00000000646c7b90 <__mingw_raise_matherr>:
+    646c7b90:	sub    $0x58,%rsp
+    646c7b94:	mov    0x4f75(%rip),%rax        # 646ccb10 <stUserMathErr>
+    646c7b9b:	test   %rax,%rax
+    646c7b9e:	je     646c7bcc <__mingw_raise_matherr+0x3c>
+    646c7ba0:	movsd  0x80(%rsp),%xmm0
+    646c7ba9:	mov    %ecx,0x20(%rsp)
+    646c7bad:	lea    0x20(%rsp),%rcx
+    646c7bb2:	mov    %rdx,0x28(%rsp)
+    646c7bb7:	movsd  %xmm2,0x30(%rsp)
+    646c7bbd:	movsd  %xmm3,0x38(%rsp)
+    646c7bc3:	movsd  %xmm0,0x40(%rsp)
+    646c7bc9:	call   *%rax
+    646c7bcb:	nop
+    646c7bcc:	add    $0x58,%rsp
+    646c7bd0:	ret
+    646c7bd1:	nopl   0x0(%rax,%rax,1)
+    646c7bd6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7be0 <__mingw_setusermatherr>:
+    646c7be0:	mov    %rcx,0x4f29(%rip)        # 646ccb10 <stUserMathErr>
+    646c7be7:	jmp    646c7cf0 <__setusermatherr>
+    646c7bec:	nopl   0x0(%rax)
+
+00000000646c7bf0 <_matherr>:
+    646c7bf0:	push   %rsi
+    646c7bf1:	push   %rbx
+    646c7bf2:	sub    $0x78,%rsp
+    646c7bf6:	movaps %xmm6,0x40(%rsp)
+    646c7bfb:	movaps %xmm7,0x50(%rsp)
+    646c7c00:	movaps %xmm8,0x60(%rsp)
+    646c7c06:	cmpl   $0x6,(%rcx)
+    646c7c09:	ja     646c7ce0 <_matherr+0xf0>
+    646c7c0f:	mov    (%rcx),%eax
+    646c7c11:	lea    0x1a9c(%rip),%rdx        # 646c96b4 <.rdata+0x124>
+    646c7c18:	movslq (%rdx,%rax,4),%rax
+    646c7c1c:	add    %rdx,%rax
+    646c7c1f:	jmp    *%rax
+    646c7c21:	lea    0x1968(%rip),%rbx        # 646c9590 <.rdata>
+    646c7c28:	mov    0x8(%rcx),%rsi
+    646c7c2c:	movsd  0x20(%rcx),%xmm8
+    646c7c32:	movsd  0x18(%rcx),%xmm7
+    646c7c37:	movsd  0x10(%rcx),%xmm6
+    646c7c3c:	mov    $0x2,%ecx
+    646c7c41:	call   646c7aa0 <__acrt_iob_func>
+    646c7c46:	movsd  %xmm8,0x30(%rsp)
+    646c7c4d:	mov    %rsi,%r9
+    646c7c50:	mov    %rbx,%r8
+    646c7c53:	movsd  %xmm7,0x28(%rsp)
+    646c7c59:	lea    0x1a28(%rip),%rdx        # 646c9688 <.rdata+0xf8>
+    646c7c60:	mov    %rax,%rcx
+    646c7c63:	movsd  %xmm6,0x20(%rsp)
+    646c7c69:	call   646c78d0 <fprintf>
+    646c7c6e:	nop
+    646c7c6f:	movaps 0x40(%rsp),%xmm6
+    646c7c74:	xor    %eax,%eax
+    646c7c76:	movaps 0x50(%rsp),%xmm7
+    646c7c7b:	movaps 0x60(%rsp),%xmm8
+    646c7c81:	add    $0x78,%rsp
+    646c7c85:	pop    %rbx
+    646c7c86:	pop    %rsi
+    646c7c87:	ret
+    646c7c88:	nopl   0x0(%rax,%rax,1)
+    646c7c90:	lea    0x1918(%rip),%rbx        # 646c95af <.rdata+0x1f>
+    646c7c97:	jmp    646c7c28 <_matherr+0x38>
+    646c7c99:	nopl   0x0(%rax)
+    646c7ca0:	lea    0x1929(%rip),%rbx        # 646c95d0 <.rdata+0x40>
+    646c7ca7:	jmp    646c7c28 <_matherr+0x38>
     646c7cac:	nopl   0x0(%rax)
-
-00000000646c7cb0 <_matherr>:
-    646c7cb0:	push   %rsi
-    646c7cb1:	push   %rbx
-    646c7cb2:	sub    $0x78,%rsp
-    646c7cb6:	movaps %xmm6,0x40(%rsp)
-    646c7cbb:	movaps %xmm7,0x50(%rsp)
-    646c7cc0:	movaps %xmm8,0x60(%rsp)
-    646c7cc6:	cmpl   $0x6,(%rcx)
-    646c7cc9:	ja     646c7da0 <_matherr+0xf0>
-    646c7ccf:	mov    (%rcx),%eax
-    646c7cd1:	lea    0x19bc(%rip),%rdx        # 646c9694 <.rdata+0x124>
-    646c7cd8:	movslq (%rdx,%rax,4),%rax
-    646c7cdc:	add    %rdx,%rax
-    646c7cdf:	jmp    *%rax
-    646c7ce1:	lea    0x1888(%rip),%rbx        # 646c9570 <.rdata>
-    646c7ce8:	mov    0x8(%rcx),%rsi
-    646c7cec:	movsd  0x20(%rcx),%xmm8
-    646c7cf2:	movsd  0x18(%rcx),%xmm7
-    646c7cf7:	movsd  0x10(%rcx),%xmm6
-    646c7cfc:	mov    $0x2,%ecx
-    646c7d01:	call   646c7b60 <__acrt_iob_func>
-    646c7d06:	movsd  %xmm8,0x30(%rsp)
-    646c7d0d:	mov    %rsi,%r9
-    646c7d10:	mov    %rbx,%r8
-    646c7d13:	movsd  %xmm7,0x28(%rsp)
-    646c7d19:	lea    0x1948(%rip),%rdx        # 646c9668 <.rdata+0xf8>
-    646c7d20:	mov    %rax,%rcx
-    646c7d23:	movsd  %xmm6,0x20(%rsp)
-    646c7d29:	call   646c7990 <fprintf>
-    646c7d2e:	nop
-    646c7d2f:	movaps 0x40(%rsp),%xmm6
-    646c7d34:	xor    %eax,%eax
-    646c7d36:	movaps 0x50(%rsp),%xmm7
-    646c7d3b:	movaps 0x60(%rsp),%xmm8
-    646c7d41:	add    $0x78,%rsp
-    646c7d45:	pop    %rbx
-    646c7d46:	pop    %rsi
-    646c7d47:	ret
-    646c7d48:	nopl   0x0(%rax,%rax,1)
-    646c7d50:	lea    0x1838(%rip),%rbx        # 646c958f <.rdata+0x1f>
-    646c7d57:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d59:	nopl   0x0(%rax)
-    646c7d60:	lea    0x1849(%rip),%rbx        # 646c95b0 <.rdata+0x40>
-    646c7d67:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d6c:	nopl   0x0(%rax)
-    646c7d70:	lea    0x18a9(%rip),%rbx        # 646c9620 <.rdata+0xb0>
-    646c7d77:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d7c:	nopl   0x0(%rax)
-    646c7d80:	lea    0x1871(%rip),%rbx        # 646c95f8 <.rdata+0x88>
-    646c7d87:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d8c:	nopl   0x0(%rax)
-    646c7d90:	lea    0x1839(%rip),%rbx        # 646c95d0 <.rdata+0x60>
-    646c7d97:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d9c:	nopl   0x0(%rax)
-    646c7da0:	lea    0x18af(%rip),%rbx        # 646c9656 <.rdata+0xe6>
-    646c7da7:	jmp    646c7ce8 <_matherr+0x38>
-    646c7dac:	nop
-    646c7dad:	nop
-    646c7dae:	nop
-    646c7daf:	nop
-
-00000000646c7db0 <__setusermatherr>:
-    646c7db0:	jmp    *0x64d6(%rip)        # 646ce28c <__imp___setusermatherr>
-    646c7db6:	nop
-    646c7db7:	nop
-    646c7db8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7dc0 <__report_error>:
-    646c7dc0:	push   %rsi
-    646c7dc1:	push   %rbx
-    646c7dc2:	sub    $0x38,%rsp
-    646c7dc6:	lea    0x58(%rsp),%rax
-    646c7dcb:	mov    %rcx,%rbx
-    646c7dce:	mov    $0x2,%ecx
-    646c7dd3:	mov    %rdx,0x58(%rsp)
-    646c7dd8:	mov    %r8,0x60(%rsp)
-    646c7ddd:	mov    %r9,0x68(%rsp)
-    646c7de2:	mov    %rax,0x28(%rsp)
-    646c7de7:	call   646c7b60 <__acrt_iob_func>
-    646c7dec:	mov    $0x1b,%r8d
-    646c7df2:	mov    $0x1,%edx
-    646c7df7:	lea    0x14e2(%rip),%rcx        # 646c92e0 <.rdata>
-    646c7dfe:	mov    %rax,%r9
-    646c7e01:	call   646c7980 <fwrite>
-    646c7e06:	mov    0x28(%rsp),%rsi
-    646c7e0b:	mov    $0x2,%ecx
-    646c7e10:	call   646c7b60 <__acrt_iob_func>
-    646c7e15:	mov    %rbx,%rdx
-    646c7e18:	mov    %rax,%rcx
-    646c7e1b:	mov    %rsi,%r8
-    646c7e1e:	call   646c7940 <vfprintf>
-    646c7e23:	call   646c79b8 <abort>
-    646c7e28:	nop
-    646c7e29:	nop
-    646c7e2a:	nop
-    646c7e2b:	nop
-    646c7e2c:	nop
-    646c7e2d:	nop
-    646c7e2e:	nop
-    646c7e2f:	nop
-
-00000000646c7e30 <register_frame_ctor>:
-    646c7e30:	jmp    646c1390 <__gcc_register_frame>
-    646c7e35:	nop
-    646c7e36:	nop
-    646c7e37:	nop
-    646c7e38:	nop
-    646c7e39:	nop
-    646c7e3a:	nop
-    646c7e3b:	nop
-    646c7e3c:	nop
-    646c7e3d:	nop
-    646c7e3e:	nop
-    646c7e3f:	nop
-
-00000000646c7e40 <__CTOR_LIST__>:
-    646c7e40:	(bad)
-    646c7e41:	(bad)
-    646c7e42:	(bad)
-    646c7e43:	(bad)
-    646c7e44:	(bad)
-    646c7e45:	(bad)
-    646c7e46:	(bad)
-    646c7e47:	push   (%rax)
-
-00000000646c7e48 <.ctors.65535>:
-    646c7e48:	xor    %bh,0x6c(%rsi)
-    646c7e4b:	add    %al,%fs:(%rax)
-	...
-
-00000000646c7e58 <__DTOR_LIST__>:
-    646c7e58:	(bad)
-    646c7e59:	(bad)
-    646c7e5a:	(bad)
-    646c7e5b:	(bad)
-    646c7e5c:	(bad)
-    646c7e5d:	(bad)
-    646c7e5e:	(bad)
-    646c7e5f:	incl   (%rax)
-    646c7e61:	add    %al,(%rax)
-    646c7e63:	add    %al,(%rax)
-    646c7e65:	add    %al,(%rax)
+    646c7cb0:	lea    0x1989(%rip),%rbx        # 646c9640 <.rdata+0xb0>
+    646c7cb7:	jmp    646c7c28 <_matherr+0x38>
+    646c7cbc:	nopl   0x0(%rax)
+    646c7cc0:	lea    0x1951(%rip),%rbx        # 646c9618 <.rdata+0x88>
+    646c7cc7:	jmp    646c7c28 <_matherr+0x38>
+    646c7ccc:	nopl   0x0(%rax)
+    646c7cd0:	lea    0x1919(%rip),%rbx        # 646c95f0 <.rdata+0x60>
+    646c7cd7:	jmp    646c7c28 <_matherr+0x38>
+    646c7cdc:	nopl   0x0(%rax)
+    646c7ce0:	lea    0x198f(%rip),%rbx        # 646c9676 <.rdata+0xe6>
+    646c7ce7:	jmp    646c7c28 <_matherr+0x38>
+    646c7cec:	nop
+    646c7ced:	nop
+    646c7cee:	nop
+    646c7cef:	nop
+
+00000000646c7cf0 <__setusermatherr>:
+    646c7cf0:	jmp    *0x6596(%rip)        # 646ce28c <__imp___setusermatherr>
+    646c7cf6:	nop
+    646c7cf7:	nop
+    646c7cf8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7d00 <__report_error>:
+    646c7d00:	push   %rsi
+    646c7d01:	push   %rbx
+    646c7d02:	sub    $0x38,%rsp
+    646c7d06:	lea    0x58(%rsp),%rax
+    646c7d0b:	mov    %rcx,%rbx
+    646c7d0e:	mov    $0x2,%ecx
+    646c7d13:	mov    %rdx,0x58(%rsp)
+    646c7d18:	mov    %r8,0x60(%rsp)
+    646c7d1d:	mov    %r9,0x68(%rsp)
+    646c7d22:	mov    %rax,0x28(%rsp)
+    646c7d27:	call   646c7aa0 <__acrt_iob_func>
+    646c7d2c:	mov    $0x1b,%r8d
+    646c7d32:	mov    $0x1,%edx
+    646c7d37:	lea    0x15c2(%rip),%rcx        # 646c9300 <.rdata>
+    646c7d3e:	mov    %rax,%r9
+    646c7d41:	call   646c78c0 <fwrite>
+    646c7d46:	mov    0x28(%rsp),%rsi
+    646c7d4b:	mov    $0x2,%ecx
+    646c7d50:	call   646c7aa0 <__acrt_iob_func>
+    646c7d55:	mov    %rbx,%rdx
+    646c7d58:	mov    %rax,%rcx
+    646c7d5b:	mov    %rsi,%r8
+    646c7d5e:	call   646c7880 <vfprintf>
+    646c7d63:	call   646c78f8 <abort>
+    646c7d68:	nop
+    646c7d69:	nop
+    646c7d6a:	nop
+    646c7d6b:	nop
+    646c7d6c:	nop
+    646c7d6d:	nop
+    646c7d6e:	nop
+    646c7d6f:	nop
+
+00000000646c7d70 <register_frame_ctor>:
+    646c7d70:	jmp    646c1390 <__gcc_register_frame>
+    646c7d75:	nop
+    646c7d76:	nop
+    646c7d77:	nop
+    646c7d78:	nop
+    646c7d79:	nop
+    646c7d7a:	nop
+    646c7d7b:	nop
+    646c7d7c:	nop
+    646c7d7d:	nop
+    646c7d7e:	nop
+    646c7d7f:	nop
+
+00000000646c7d80 <__CTOR_LIST__>:
+    646c7d80:	(bad)
+    646c7d81:	(bad)
+    646c7d82:	(bad)
+    646c7d83:	(bad)
+    646c7d84:	(bad)
+    646c7d85:	(bad)
+    646c7d86:	(bad)
+    646c7d87:	push   0x7d(%rax)
+
+00000000646c7d88 <.ctors.65535>:
+    646c7d88:	jo     646c7e07 <__DTOR_LIST__+0x6f>
+    646c7d8a:	insb   (%dx),%es:(%rdi)
+    646c7d8b:	add    %al,%fs:(%rax)
+	...
+
+00000000646c7d98 <__DTOR_LIST__>:
+    646c7d98:	(bad)
+    646c7d99:	(bad)
+    646c7d9a:	(bad)
+    646c7d9b:	(bad)
+    646c7d9c:	(bad)
+    646c7d9d:	(bad)
+    646c7d9e:	(bad)
+    646c7d9f:	incl   (%rax)
+    646c7da1:	add    %al,(%rax)
+    646c7da3:	add    %al,(%rax)
+    646c7da5:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000000646c8000 <__data_start__>:
-    646c8000:	(bad)
-    646c8001:	jle    646c806f <__imp__initialize_onexit_table+0xf>
-    646c8003:	add    %al,%fs:(%rax)
+    646c8000:	movabs 0x646c7d,%al
+    646c8009:	add    %al,(%rax)
+    646c800b:	add    %al,(%rax)
+    646c800d:	add    %al,(%rax)
 	...
 
 00000000646c8010 <__native_vcclrit_reason>:
     646c8010:	(bad)
     646c8011:	(bad)
     646c8012:	(bad)
     646c8013:	(bad)
@@ -10487,32 +10464,34 @@
     646c8044:	add    %al,(%rax)
     646c8046:	stos   %al,%es:(%rdi)
     646c8047:	mov    $0x3fff,%eax
     646c804c:	add    %al,(%rax)
 	...
 
 00000000646c8050 <__imp__execute_onexit_table>:
-    646c8050:	lock jp 646c80bf <__data_end__+0x1f>
+    646c8050:	xor    %bh,0x6c(%rdx)
     646c8053:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8058 <__imp__register_onexit_function>:
-    646c8058:	and    %bh,0x6c(%rdx)
+    646c8058:	(bad)
+    646c8059:	jns    646c80c7 <__data_end__+0x27>
     646c805b:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8060 <__imp__initialize_onexit_table>:
-    646c8060:	lock jns 646c80cf <__data_end__+0x2f>
+    646c8060:	xor    %bh,0x6c(%rcx)
     646c8063:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8070 <__imp___acrt_iob_func>:
-    646c8070:	(bad)
-    646c8071:	jnp    646c80df <__data_end__+0x3f>
-    646c8073:	add    %al,%fs:(%rax)
+    646c8070:	movabs 0x646c7a,%al
+    646c8079:	add    %al,(%rax)
+    646c807b:	add    %al,(%rax)
+    646c807d:	add    %al,(%rax)
 	...
 
 00000000646c8080 <__security_cookie>:
     646c8080:	xor    0x2b992ddf(%rdx),%ah
 	...
 
 00000000646c8090 <__security_cookie_complement>:
@@ -10600,1017 +10579,1022 @@
     646c9098:	sbb    %ch,0x21fb5444(%rip)        # 8667e4e2 <.debug_str+0x21fa64e2>
     646c909e:	sbb    %eax,0x0(%rax)
 
 00000000646c90a0 <.rdata>:
     646c90a0:	add    %al,(%rax)
     646c90a2:	add    %al,(%rax)
     646c90a4:	add    %al,(%rax)
-    646c90a6:	or     %al,%al
-    646c90a8:	add    %al,(%rax)
-    646c90aa:	add    %al,(%rax)
-    646c90ac:	add    %al,(%rax)
-    646c90ae:	lock (bad)
-
-00000000646c90b0 <.rdata>:
-    646c90b0:	or     (%rax),%al
-    646c90b2:	add    %al,(%rax)
+    646c90a6:	lock (bad)
+	...
     646c90b4:	add    %al,(%rax)
-    646c90b6:	add    %al,(%rax)
-    646c90b8:	or     (%rax),%al
-    646c90ba:	add    %al,(%rax)
-    646c90bc:	add    %al,(%rax)
-    646c90be:	add    %al,(%rax)
-    646c90c0:	add    %al,%fs:(%rax)
-    646c90c3:	add    %al,(%rax)
-    646c90c5:	add    %al,(%rax)
-    646c90c7:	add    %ah,0x0(%rax,%rax,1)
-    646c90cb:	add    %al,(%rax)
-    646c90cd:	add    %al,(%rax)
-    646c90cf:	add    %al,0x45a1cac0(%rbx)
-    646c90d5:	mov    $0xfb,%dh
-    646c90d7:	(bad)
-	...
-    646c90e0:	(bad)
-    646c90e1:	(bad)
-    646c90e2:	(bad)
-    646c90e3:	(bad)
-    646c90e4:	(bad)
-    646c90e5:	(bad)
-    646c90e6:	(bad)
-    646c90e7:	jg     646c90e8 <.rdata+0x38>
-    646c90e9:	(bad)
-    646c90ea:	(bad)
-    646c90eb:	(bad)
-    646c90ec:	(bad)
-    646c90ed:	(bad)
-    646c90ee:	(bad)
-    646c90ef:	jg     646c90f2 <.rdata+0x42>
-    646c90f1:	add    %al,(%rax)
-    646c90f3:	add    %al,(%rax)
-    646c90f5:	add    %al,(%rax)
-    646c90f7:	add    %al,(%rcx)
-    646c90f9:	add    %al,(%rax)
-    646c90fb:	add    %al,(%rax)
-    646c90fd:	add    %al,(%rax)
-    646c90ff:	add    %bh,%bh
-    646c9101:	(bad)
-    646c9102:	(bad)
-    646c9103:	(bad)
-    646c9104:	(bad)
-    646c9105:	(bad)
-    646c9106:	(bad)
-    646c9107:	jg     646c9109 <.rdata+0x59>
-	...
-    646c9115:	add    %dh,%al
-    646c9117:	(bad)
-    646c9118:	add    %al,(%rax)
+    646c90b6:	or     %al,%al
+	...
+
+00000000646c90c0 <.rdata>:
+    646c90c0:	add    $0xffffffca,%eax
+    646c90c3:	movabs 0x3ffbb645,%eax
+    646c90cc:	add    %al,(%rax)
+    646c90ce:	add    %al,(%rax)
+    646c90d0:	(bad)
+    646c90d1:	(bad)
+    646c90d2:	(bad)
+    646c90d3:	(bad)
+    646c90d4:	(bad)
+    646c90d5:	(bad)
+    646c90d6:	(bad)
+    646c90d7:	jg     646c90d8 <.rdata+0x18>
+    646c90d9:	(bad)
+    646c90da:	(bad)
+    646c90db:	(bad)
+    646c90dc:	(bad)
+    646c90dd:	(bad)
+    646c90de:	(bad)
+    646c90df:	jg     646c90e2 <.rdata+0x22>
+    646c90e1:	add    %al,(%rax)
+    646c90e3:	add    %al,(%rax)
+    646c90e5:	add    %al,(%rax)
+    646c90e7:	add    %al,(%rcx)
+    646c90e9:	add    %al,(%rax)
+    646c90eb:	add    %al,(%rax)
+    646c90ed:	add    %al,(%rax)
+    646c90ef:	add    %bh,%bh
+    646c90f1:	(bad)
+    646c90f2:	(bad)
+    646c90f3:	(bad)
+    646c90f4:	(bad)
+    646c90f5:	(bad)
+    646c90f6:	(bad)
+    646c90f7:	jg     646c90f9 <.rdata+0x39>
+	...
+    646c9105:	add    %dh,%al
+    646c9107:	(bad)
+    646c9108:	add    %al,(%rax)
+    646c910a:	add    %al,(%rax)
+    646c910c:	add    %al,(%rax)
+    646c910e:	loopne 646c914f <.rdata+0xf>
+    646c9110:	add    %al,(%rax)
+    646c9112:	add    %al,(%rax)
+    646c9114:	add    %eax,(%rax)
+    646c9116:	add    %al,(%rax)
+    646c9118:	add    (%rax),%al
     646c911a:	add    %al,(%rax)
-    646c911c:	add    %al,(%rax)
-    646c911e:	loopne 646c915f <.rdata+0xf>
-    646c9120:	add    %al,(%rax)
+    646c911c:	add    (%rax),%eax
+    646c911e:	add    %al,(%rax)
+    646c9120:	add    $0x0,%al
     646c9122:	add    %al,(%rax)
-    646c9124:	add    %eax,(%rax)
+    646c9124:	add    $0x0,%al
     646c9126:	add    %al,(%rax)
-    646c9128:	add    (%rax),%al
+    646c9128:	add    $0x0,%al
     646c912a:	add    %al,(%rax)
-    646c912c:	add    (%rax),%eax
-    646c912e:	add    %al,(%rax)
-    646c9130:	add    $0x0,%al
-    646c9132:	add    %al,(%rax)
-    646c9134:	add    $0x0,%al
-    646c9136:	add    %al,(%rax)
-    646c9138:	add    $0x0,%al
-    646c913a:	add    %al,(%rax)
-    646c913c:	add    $0x0,%al
+    646c912c:	add    $0x0,%al
 	...
-    646c9146:	lock (bad)
-    646c9148:	add    %al,(%rax)
-    646c914a:	add    %al,(%rax)
-    646c914c:	add    %al,(%rax)
-    646c914e:	lock (bad)
-
-00000000646c9150 <.rdata>:
-    646c9150:	and    $0x25732573,%eax
-    646c9155:	and    $0x64642530,%eax
-    646c915a:	je,pn  646c91d5 <.rdata+0x85>
-    646c915d:	je     646c915f <.rdata+0xf>
-    646c915f:	rex.RX outsl %ds:(%rsi),(%dx)
-    646c9161:	insb   (%dx),%es:(%rdi)
-    646c9162:	fs gs jb 646c9186 <.rdata+0x36>
-    646c9166:	(bad)
-    646c9167:	insb   (%dx),%es:(%rdi)
-    646c9168:	jb     646c91cf <.rdata+0x7f>
-    646c916a:	(bad)
-    646c916b:	fs jns 646c918e <.rdata+0x3e>
-    646c916e:	gs js  646c91da <.rdata+0x8a>
-    646c9171:	jae    646c91e7 <.rdata+0x97>
-    646c9173:	and    %eax,(%rax)
-    646c9175:	ja     646c9177 <.rdata+0x27>
-    646c9177:	rex.RX (bad)
-    646c9179:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
-    646c9181:	outsl  %ds:(%rsi),(%dx)
-    646c9182:	jo     646c91e9 <.rdata+0x99>
-    646c9184:	outsb  %ds:(%rsi),(%dx)
-    646c9185:	and    %dh,0x65(%rax,%rbp,2)
-    646c9189:	and    %ah,0x69(%rsi)
-    646c918c:	insb   (%dx),%es:(%rdi)
-    646c918d:	add    %ah,%gs:0x2e250964(%rip)        # 92919af8 <.debug_str+0x2e241af8>
-    646c9194:	xor    %esi,(%rax)
-    646c9196:	data16 or (%rax),%al
-	...
-    646c91a1:	add    %al,(%rax)
-    646c91a3:	add    %al,(%rcx)
-    646c91a5:	add    %al,(%rax)
-    646c91a7:	add    %al,(%rdx)
-    646c91a9:	add    %al,(%rax)
-    646c91ab:	add    %al,(%rbx)
-    646c91ad:	add    %al,(%rax)
-    646c91af:	add    %al,(%rax,%rax,1)
+    646c9136:	lock (bad)
+    646c9138:	add    %al,(%rax)
+    646c913a:	add    %al,(%rax)
+    646c913c:	add    %al,(%rax)
+    646c913e:	lock (bad)
+
+00000000646c9140 <.rdata>:
+    646c9140:	and    $0x25732573,%eax
+    646c9145:	and    $0x64642530,%eax
+    646c914a:	je,pn  646c91c5 <.rdata+0x85>
+    646c914d:	je     646c914f <.rdata+0xf>
+    646c914f:	rex.RX outsl %ds:(%rsi),(%dx)
+    646c9151:	insb   (%dx),%es:(%rdi)
+    646c9152:	fs gs jb 646c9176 <.rdata+0x36>
+    646c9156:	(bad)
+    646c9157:	insb   (%dx),%es:(%rdi)
+    646c9158:	jb     646c91bf <.rdata+0x7f>
+    646c915a:	(bad)
+    646c915b:	fs jns 646c917e <.rdata+0x3e>
+    646c915e:	gs js  646c91ca <.rdata+0x8a>
+    646c9161:	jae    646c91d7 <.rdata+0x97>
+    646c9163:	and    %eax,(%rax)
+    646c9165:	ja     646c9167 <.rdata+0x27>
+    646c9167:	rex.RX (bad)
+    646c9169:	imul   $0x206f7420,0x64(%rbp,%riz,2),%ebp
+    646c9171:	outsl  %ds:(%rsi),(%dx)
+    646c9172:	jo     646c91d9 <.rdata+0x99>
+    646c9174:	outsb  %ds:(%rsi),(%dx)
+    646c9175:	and    %dh,0x65(%rax,%rbp,2)
+    646c9179:	and    %ah,0x69(%rsi)
+    646c917c:	insb   (%dx),%es:(%rdi)
+    646c917d:	add    %ah,%gs:0x2e250964(%rip)        # 92919ae8 <.debug_str+0x2e241ae8>
+    646c9184:	xor    %esi,(%rax)
+    646c9186:	data16 or (%rax),%al
+	...
+    646c9191:	add    %al,(%rax)
+    646c9193:	add    %al,(%rcx)
+    646c9195:	add    %al,(%rax)
+    646c9197:	add    %al,(%rdx)
+    646c9199:	add    %al,(%rax)
+    646c919b:	add    %al,(%rbx)
+    646c919d:	add    %al,(%rax)
+    646c919f:	add    %al,(%rax,%rax,1)
+    646c91a2:	add    %al,(%rax)
+    646c91a4:	add    $0x0,%al
+    646c91a6:	add    %al,(%rax)
+    646c91a8:	add    $0x0,%al
+    646c91aa:	add    %al,(%rax)
+    646c91ac:	add    $0x0,%al
+    646c91ae:	add    %al,(%rax)
+    646c91b0:	add    %eax,(%rax)
     646c91b2:	add    %al,(%rax)
-    646c91b4:	add    $0x0,%al
+    646c91b4:	add    %eax,(%rax)
     646c91b6:	add    %al,(%rax)
-    646c91b8:	add    $0x0,%al
+    646c91b8:	add    %eax,(%rax)
     646c91ba:	add    %al,(%rax)
-    646c91bc:	add    $0x0,%al
-    646c91be:	add    %al,(%rax)
-    646c91c0:	add    %eax,(%rax)
-    646c91c2:	add    %al,(%rax)
-    646c91c4:	add    %eax,(%rax)
-    646c91c6:	add    %al,(%rax)
-    646c91c8:	add    %eax,(%rax)
-    646c91ca:	add    %al,(%rax)
-    646c91cc:	add    %eax,(%rax)
+    646c91bc:	add    %eax,(%rax)
 	...
-    646c91d6:	lock (bad)
+    646c91c6:	lock (bad)
 	...
-    646c91e0:	(bad)
+    646c91d0:	(bad)
+    646c91d1:	(bad)
+    646c91d2:	(bad)
+    646c91d3:	(bad)
+    646c91d4:	(bad)
+    646c91d5:	(bad)
+    646c91d6:	(bad)
+    646c91d7:	jg     646c91d9 <.rdata+0x99>
+    646c91d9:	add    %al,(%rax)
+    646c91db:	add    %al,(%rax)
+    646c91dd:	add    %al,(%rax)
+    646c91df:	add    %bh,%bh
     646c91e1:	(bad)
     646c91e2:	(bad)
     646c91e3:	(bad)
     646c91e4:	(bad)
     646c91e5:	(bad)
     646c91e6:	(bad)
-    646c91e7:	jg     646c91e9 <.rdata+0x99>
-    646c91e9:	add    %al,(%rax)
-    646c91eb:	add    %al,(%rax)
-    646c91ed:	add    %al,(%rax)
-    646c91ef:	add    %bh,%bh
-    646c91f1:	(bad)
-    646c91f2:	(bad)
-    646c91f3:	(bad)
-    646c91f4:	(bad)
-    646c91f5:	(bad)
-    646c91f6:	(bad)
-    646c91f7:	jg     646c91f8 <.rdata+0xa8>
-    646c91f9:	(bad)
-    646c91fa:	(bad)
-    646c91fb:	(bad)
-    646c91fc:	(bad)
-    646c91fd:	(bad)
-    646c91fe:	(bad)
-    646c91ff:	jg     646c9201 <.rdata+0xb1>
-    646c9201:	add    %al,(%rax)
-    646c9203:	add    %al,(%rax)
-    646c9205:	add    %dh,(%rax)
-    646c9207:	rex.XB add %al,(%r8)
-    646c920a:	add    %al,(%rax)
-    646c920c:	add    %al,(%rax)
-	...
-
-00000000646c9210 <.rdata>:
-    646c9210:	rex.WRX jne 646c9280 <__dyn_tls_init_callback>
-    646c9213:	(bad)
-    646c9215:	jb     646c9237 <.rdata+0x27>
-    646c9217:	cmp    $0xa642520,%eax
-    646c921c:	add    %ch,(%rsi)
-    646c921e:	(bad)
-    646c921f:	push   %rdx
-    646c9220:	gs (bad)
-    646c9222:	insb   (%dx),%es:(%rdi)
-    646c9223:	imul   $0x6e6f6974,0x61(%rdx),%edi
-    646c922a:	jae    646c925b <.rdata+0x4b>
-    646c922c:	add    %dl,0x65(%rdx)
-    646c922f:	(bad)
-    646c9230:	insb   (%dx),%es:(%rdi)
-    646c9231:	imul   $0x6e6f6974,0x61(%rdx),%edi
-    646c9238:	jae    646c923a <.rdata+0x2a>
-    646c923a:	cs (bad)
-    646c923c:	push   %rdx
-    646c923d:	gs (bad)
-    646c923f:	insb   (%dx),%es:(%rdi)
-    646c9240:	imul   $0x6e6f6974,0x61(%rdx),%edi
-    646c9247:	jae    646c9278 <GS_ExceptionPointers+0x8>
-    646c9249:	push   %rsi
-    646c924a:	(bad)
-    646c924b:	jb     646c92b6 <_tls_used+0x16>
-    646c924d:	outsl  %ds:(%rsi),(%dx)
-    646c924e:	addr32 jb 646c92b2 <_tls_used+0x12>
-    646c9251:	insl   (%dx),%es:(%rdi)
-    646c9252:	(bad)
-    646c9253:	add    %dl,0x61(%rsi)
-    646c9256:	jb     646c92c1 <_tls_used+0x21>
-    646c9258:	outsl  %ds:(%rsi),(%dx)
-    646c9259:	addr32 jb 646c92bd <_tls_used+0x1d>
-    646c925c:	insl   (%dx),%es:(%rdi)
-    646c925d:	add    %al,(%rax)
-	...
-
-00000000646c9260 <.rdata>:
-    646c9260:	add    %al,(%rax)
-    646c9262:	add    %al,(%rax)
-    646c9264:	add    %al,(%rax)
-    646c9266:	lock (bad)
-    646c9268:	(bad)
-    646c9269:	in     (%dx),%eax
-    646c926a:	mov    $0xa0,%ch
-    646c926c:	test   $0xc7403eb0,%esi
-
-00000000646c9270 <GS_ExceptionPointers>:
-    646c9270:	rex (bad)
-    646c9272:	insb   (%dx),%es:(%rdi)
-    646c9273:	add    %al,%fs:(%rax)
-    646c9276:	add    %al,(%rax)
-    646c9278:	(bad)
-    646c9279:	ret    $0x646c
+    646c91e7:	jg     646c91e8 <.rdata+0xa8>
+    646c91e9:	(bad)
+    646c91ea:	(bad)
+    646c91eb:	(bad)
+    646c91ec:	(bad)
+    646c91ed:	(bad)
+    646c91ee:	(bad)
+    646c91ef:	jg     646c91f1 <.rdata+0xb1>
+    646c91f1:	add    %al,(%rax)
+    646c91f3:	add    %al,(%rax)
+    646c91f5:	add    %dh,(%rax)
+    646c91f7:	rex.XB add %al,(%r8)
+    646c91fa:	add    %al,(%rax)
+    646c91fc:	add    %al,(%rax)
+	...
+
+00000000646c9200 <.rdata>:
+    646c9200:	rex.WRX jne 646c9270 <.rdata+0x70>
+    646c9203:	(bad)
+    646c9205:	jb     646c9227 <.rdata+0x27>
+    646c9207:	cmp    $0xa642520,%eax
+    646c920c:	add    %ch,(%rsi)
+    646c920e:	(bad)
+    646c920f:	push   %rdx
+    646c9210:	gs (bad)
+    646c9212:	insb   (%dx),%es:(%rdi)
+    646c9213:	imul   $0x6e6f6974,0x61(%rdx),%edi
+    646c921a:	jae    646c924b <.rdata+0x4b>
+    646c921c:	add    %dl,0x65(%rdx)
+    646c921f:	(bad)
+    646c9220:	insb   (%dx),%es:(%rdi)
+    646c9221:	imul   $0x6e6f6974,0x61(%rdx),%edi
+    646c9228:	jae    646c922a <.rdata+0x2a>
+    646c922a:	cs (bad)
+    646c922c:	push   %rdx
+    646c922d:	gs (bad)
+    646c922f:	insb   (%dx),%es:(%rdi)
+    646c9230:	imul   $0x6e6f6974,0x61(%rdx),%edi
+    646c9237:	jae    646c9268 <.rdata+0x68>
+    646c9239:	push   %rsi
+    646c923a:	(bad)
+    646c923b:	jb     646c92a6 <__dyn_tls_init_callback+0x6>
+    646c923d:	outsl  %ds:(%rsi),(%dx)
+    646c923e:	addr32 jb 646c92a2 <__dyn_tls_init_callback+0x2>
+    646c9241:	insl   (%dx),%es:(%rdi)
+    646c9242:	(bad)
+    646c9243:	add    %dl,0x61(%rsi)
+    646c9246:	jb     646c92b1 <__dyn_tls_init_callback+0x11>
+    646c9248:	outsl  %ds:(%rsi),(%dx)
+    646c9249:	addr32 jb 646c92ad <__dyn_tls_init_callback+0xd>
+    646c924c:	insl   (%dx),%es:(%rdi)
+	...
+    646c9255:	add    %ah,%al
+    646c9257:	(bad)
+    646c9258:	add    %al,(%rax)
+    646c925a:	add    %al,(%rax)
+    646c925c:	add    %al,(%rax)
+    646c925e:	adc    %al,-0x73(%rax)
+    646c9261:	in     (%dx),%eax
+    646c9262:	mov    $0xa0,%ch
+    646c9264:	test   $0x3eb0,%esi
+	...
+    646c9276:	add    %al,0x0(%rax)
     646c927c:	add    %al,(%rax)
 	...
 
-00000000646c9280 <__dyn_tls_init_callback>:
-    646c9280:	rcrb   $0x64,0x6c(%rax)
+00000000646c9280 <.rdata>:
+    646c9280:	add    %al,(%rax)
+    646c9282:	add    %al,(%rax)
+    646c9284:	add    %al,(%rax)
+    646c9286:	lock (bad)
+    646c9288:	(bad)
+    646c9289:	in     (%dx),%eax
+    646c928a:	mov    $0xa0,%ch
+    646c928c:	test   $0xc7203eb0,%esi
+
+00000000646c9290 <GS_ExceptionPointers>:
+    646c9290:	and    %al,%bh
+    646c9292:	insb   (%dx),%es:(%rdi)
+    646c9293:	add    %al,%fs:(%rax)
+    646c9296:	add    %al,(%rax)
+    646c9298:	rex ret $0x646c
+    646c929c:	add    %al,(%rax)
 	...
 
-00000000646c92a0 <_tls_used>:
-    646c92a0:	add    %al,(%rax)
-    646c92a2:	insl   (%dx),%es:(%rdi)
+00000000646c92a0 <__dyn_tls_init_callback>:
+    646c92a0:	add    %bl,0x6c(%rax)
     646c92a3:	add    %al,%fs:(%rax)
-    646c92a6:	add    %al,(%rax)
-    646c92a8:	or     %al,(%rax)
-    646c92aa:	insl   (%dx),%es:(%rdi)
-    646c92ab:	add    %al,%fs:(%rax)
-    646c92ae:	add    %al,(%rax)
-    646c92b0:	in     (%dx),%al
-    646c92b1:	(bad)
-    646c92b2:	insb   (%dx),%es:(%rdi)
-    646c92b3:	add    %al,%fs:(%rax)
-    646c92b6:	add    %al,(%rax)
-    646c92b8:	xor    %dh,%al
-    646c92ba:	insb   (%dx),%es:(%rdi)
-    646c92bb:	add    %al,%fs:(%rax)
-	...
-
-00000000646c92e0 <.rdata>:
-    646c92e0:	imul   $0x36772d77,0x67(%r14),%r13
-    646c92e8:	xor    $0x20,%al
-    646c92ea:	jb     646c9361 <.rdata+0x81>
-    646c92ec:	outsb  %ds:(%rsi),(%dx)
-    646c92ed:	je     646c9358 <.rdata+0x78>
-    646c92ef:	insl   (%dx),%es:(%rdi)
-    646c92f0:	and    %ah,%gs:0x61(%rsi)
-    646c92f4:	imul   $0xa3a65,0x72(%rbp,%rsi,2),%ebp
-    646c92fc:	add    %al,(%rax)
-    646c92fe:	add    %al,(%rax)
-    646c9300:	rex.B
-    646c9301:	fs fs jb 646c936a <.rdata+0x8a>
-    646c9305:	jae    646c937a <.rdata+0x9a>
-    646c9307:	and    %ah,0x61682070(%rip)        # c5d4b37d <.debug_str+0x6167337d>
-    646c930d:	jae    646c932f <.rdata+0x4f>
-    646c930f:	outsb  %ds:(%rsi),(%dx)
-    646c9310:	outsl  %ds:(%rsi),(%dx)
-    646c9311:	and    %ch,0x6d(%rcx)
-    646c9314:	(bad)
-    646c9315:	addr32 gs sub $0x74636573,%eax
-    646c931c:	imul   $0x56202000,0x6e(%rdi),%ebp
-    646c9323:	imul   $0x516c6175,0x74(%rdx),%esi
-    646c932a:	jne    646c9391 <.rdata+0xb1>
-    646c932c:	jb     646c93a7 <.rdata+0xc7>
-    646c932e:	and    %ah,0x61(%rsi)
-    646c9331:	imul   $0x726f6620,0x64(%rbp,%riz,2),%ebp
-    646c9339:	and    %ah,0x79622064(%rip)        # ddceb3a3 <.debug_str+0x796133a3>
-    646c933f:	je     646c93a6 <.rdata+0xc6>
-    646c9341:	jae    646c9363 <.rdata+0x83>
-    646c9343:	(bad)
-    646c9344:	je     646c9366 <.rdata+0x86>
-    646c9346:	(bad)
-    646c9347:	fs fs jb 646c93b0 <.rdata+0xd0>
-    646c934b:	jae    646c93c0 <.rdata+0xe0>
-    646c934d:	and    %ah,0x70(%rip)        # 646c93c3 <.rdata+0xe3>
-    646c9353:	add    %al,(%rax)
-    646c9355:	add    %al,(%rax)
-    646c9357:	add    %ah,(%rax)
-    646c9359:	and    %dl,0x69(%rsi)
-    646c935c:	jb     646c93d2 <.rdata+0xf2>
-    646c935e:	jne    646c93c1 <.rdata+0xe1>
-    646c9360:	insb   (%dx),%es:(%rdi)
-    646c9361:	push   %rax
-    646c9362:	jb     646c93d3 <.rdata+0xf3>
-    646c9364:	je     646c93cb <.rdata+0xeb>
-    646c9366:	movsxd 0x66(%rax,%riz,1),%esi
-    646c936a:	(bad)
-    646c936b:	imul   $0x74697720,0x64(%rbp,%riz,2),%ebp
-    646c9373:	push   $0x646f6320
-    646c9378:	and    %dh,%gs:(%rax)
-    646c937b:	js     646c93a2 <.rdata+0xc2>
-    646c937d:	js     646c937f <.rdata+0x9f>
-    646c937f:	add    %ah,(%rax)
-    646c9381:	and    %dl,0x6e(%rbp)
-    646c9384:	imul   $0x77,0x6f(%rsi),%ebp
-    646c9388:	outsb  %ds:(%rsi),(%dx)
-    646c9389:	and    %dh,0x73(%rax)
-    646c938c:	gs jne 646c93f3 <.rdata+0x3>
-    646c938f:	outsl  %ds:(%rsi),(%dx)
-    646c9390:	and    %dh,0x65(%rdx)
-    646c9393:	insb   (%dx),%es:(%rdi)
-    646c9394:	outsl  %ds:(%rsi),(%dx)
-    646c9395:	movsxd 0x74(%rcx),%esp
-    646c9398:	imul   $0x6f727020,0x6e(%rdi),%ebp
-    646c939f:	je     646c9410 <.rdata+0x10>
-    646c93a1:	movsxd 0x6c(%rdi),%ebp
-    646c93a4:	and    %dh,0x65(%rsi)
-    646c93a7:	jb     646c941c <.rdata+0x1c>
-    646c93a9:	imul   $0x2e642520,0x6e(%rdi),%ebp
-    646c93b0:	or     (%rax),%al
-    646c93b2:	add    %al,(%rax)
-    646c93b4:	add    %al,(%rax)
-    646c93b6:	add    %al,(%rax)
-    646c93b8:	and    %ah,(%rax)
-    646c93ba:	push   %rbp
-    646c93bb:	outsb  %ds:(%rsi),(%dx)
-    646c93bc:	imul   $0x77,0x6f(%rsi),%ebp
-    646c93c0:	outsb  %ds:(%rsi),(%dx)
-    646c93c1:	and    %dh,0x73(%rax)
-    646c93c4:	gs jne 646c942b <.rdata+0x2b>
-    646c93c7:	outsl  %ds:(%rsi),(%dx)
-    646c93c8:	and    %dh,0x65(%rdx)
-    646c93cb:	insb   (%dx),%es:(%rdi)
-    646c93cc:	outsl  %ds:(%rsi),(%dx)
-    646c93cd:	movsxd 0x74(%rcx),%esp
-    646c93d0:	imul   $0x74696220,0x6e(%rdi),%ebp
-    646c93d7:	and    %dh,0x69(%rbx)
-    646c93da:	jp     646c9441 <.rdata+0x1>
-    646c93dc:	and    %ah,0xa2e64(%rip)        # 6476c246 <.debug_str+0x94246>
-	...
-
-00000000646c93f0 <.rdata>:
-    646c93f0:	jo,pn  646c9457 <.rdata+0x17>
-    646c93f3:	(bad)
-    646c93f4:	je     646c9457 <.rdata+0x17>
-	...
-
-00000000646c9400 <.rdata>:
-    646c9400:	jae    646c9473 <.rdata+0x3>
-    646c9402:	jb     646c9478 <.rdata+0x8>
-	...
-    646c940c:	add    %al,(%rax)
-    646c940e:	add    %al,0x0(%rax)
-    646c9414:	add    %al,(%rax)
-    646c9416:	clc
-    646c9417:	incl   (%rax)
-    646c9419:	add    %al,(%rax)
-    646c941b:	add    %al,(%rax)
-    646c941d:	add    %dh,%al
-    646c941f:	jg     646c9421 <.rdata+0x21>
-    646c9421:	add    %al,(%rax)
-    646c9423:	add    %al,(%rax)
-    646c9425:	add    %dh,%al
-    646c9427:	(bad)
 	...
 
-00000000646c9430 <.rdata>:
-    646c9430:	movsxd 0x73(%rdi),%ebp
-	...
+00000000646c92c0 <_tls_used>:
+    646c92c0:	add    %al,(%rax)
+    646c92c2:	insl   (%dx),%es:(%rdi)
+    646c92c3:	add    %al,%fs:(%rax)
+    646c92c6:	add    %al,(%rax)
+    646c92c8:	or     %al,(%rax)
+    646c92ca:	insl   (%dx),%es:(%rdi)
+    646c92cb:	add    %al,%fs:(%rax)
+    646c92ce:	add    %al,(%rax)
+    646c92d0:	int3
+    646c92d1:	(bad)
+    646c92d2:	insb   (%dx),%es:(%rdi)
+    646c92d3:	add    %al,%fs:(%rax)
+    646c92d6:	add    %al,(%rax)
+    646c92d8:	xor    %dh,%al
+    646c92da:	insb   (%dx),%es:(%rdi)
+    646c92db:	add    %al,%fs:(%rax)
+	...
+
+00000000646c9300 <.rdata>:
+    646c9300:	imul   $0x36772d77,0x67(%r14),%r13
+    646c9308:	xor    $0x20,%al
+    646c930a:	jb     646c9381 <.rdata+0x81>
+    646c930c:	outsb  %ds:(%rsi),(%dx)
+    646c930d:	je     646c9378 <.rdata+0x78>
+    646c930f:	insl   (%dx),%es:(%rdi)
+    646c9310:	and    %ah,%gs:0x61(%rsi)
+    646c9314:	imul   $0xa3a65,0x72(%rbp,%rsi,2),%ebp
+    646c931c:	add    %al,(%rax)
+    646c931e:	add    %al,(%rax)
+    646c9320:	rex.B
+    646c9321:	fs fs jb 646c938a <.rdata+0x8a>
+    646c9325:	jae    646c939a <.rdata+0x9a>
+    646c9327:	and    %ah,0x61682070(%rip)        # c5d4b39d <.debug_str+0x6167339d>
+    646c932d:	jae    646c934f <.rdata+0x4f>
+    646c932f:	outsb  %ds:(%rsi),(%dx)
+    646c9330:	outsl  %ds:(%rsi),(%dx)
+    646c9331:	and    %ch,0x6d(%rcx)
+    646c9334:	(bad)
+    646c9335:	addr32 gs sub $0x74636573,%eax
+    646c933c:	imul   $0x56202000,0x6e(%rdi),%ebp
+    646c9343:	imul   $0x516c6175,0x74(%rdx),%esi
+    646c934a:	jne    646c93b1 <.rdata+0xb1>
+    646c934c:	jb     646c93c7 <.rdata+0xc7>
+    646c934e:	and    %ah,0x61(%rsi)
+    646c9351:	imul   $0x726f6620,0x64(%rbp,%riz,2),%ebp
+    646c9359:	and    %ah,0x79622064(%rip)        # ddceb3c3 <.debug_str+0x796133c3>
+    646c935f:	je     646c93c6 <.rdata+0xc6>
+    646c9361:	jae    646c9383 <.rdata+0x83>
+    646c9363:	(bad)
+    646c9364:	je     646c9386 <.rdata+0x86>
+    646c9366:	(bad)
+    646c9367:	fs fs jb 646c93d0 <.rdata+0xd0>
+    646c936b:	jae    646c93e0 <.rdata+0xe0>
+    646c936d:	and    %ah,0x70(%rip)        # 646c93e3 <.rdata+0xe3>
+    646c9373:	add    %al,(%rax)
+    646c9375:	add    %al,(%rax)
+    646c9377:	add    %ah,(%rax)
+    646c9379:	and    %dl,0x69(%rsi)
+    646c937c:	jb     646c93f2 <.rdata+0xf2>
+    646c937e:	jne    646c93e1 <.rdata+0xe1>
+    646c9380:	insb   (%dx),%es:(%rdi)
+    646c9381:	push   %rax
+    646c9382:	jb     646c93f3 <.rdata+0xf3>
+    646c9384:	je     646c93eb <.rdata+0xeb>
+    646c9386:	movsxd 0x66(%rax,%riz,1),%esi
+    646c938a:	(bad)
+    646c938b:	imul   $0x74697720,0x64(%rbp,%riz,2),%ebp
+    646c9393:	push   $0x646f6320
+    646c9398:	and    %dh,%gs:(%rax)
+    646c939b:	js     646c93c2 <.rdata+0xc2>
+    646c939d:	js     646c939f <.rdata+0x9f>
+    646c939f:	add    %ah,(%rax)
+    646c93a1:	and    %dl,0x6e(%rbp)
+    646c93a4:	imul   $0x77,0x6f(%rsi),%ebp
+    646c93a8:	outsb  %ds:(%rsi),(%dx)
+    646c93a9:	and    %dh,0x73(%rax)
+    646c93ac:	gs jne 646c9413 <.rdata+0x3>
+    646c93af:	outsl  %ds:(%rsi),(%dx)
+    646c93b0:	and    %dh,0x65(%rdx)
+    646c93b3:	insb   (%dx),%es:(%rdi)
+    646c93b4:	outsl  %ds:(%rsi),(%dx)
+    646c93b5:	movsxd 0x74(%rcx),%esp
+    646c93b8:	imul   $0x6f727020,0x6e(%rdi),%ebp
+    646c93bf:	je     646c9430 <.rdata+0x10>
+    646c93c1:	movsxd 0x6c(%rdi),%ebp
+    646c93c4:	and    %dh,0x65(%rsi)
+    646c93c7:	jb     646c943c <.rdata+0x1c>
+    646c93c9:	imul   $0x2e642520,0x6e(%rdi),%ebp
+    646c93d0:	or     (%rax),%al
+    646c93d2:	add    %al,(%rax)
+    646c93d4:	add    %al,(%rax)
+    646c93d6:	add    %al,(%rax)
+    646c93d8:	and    %ah,(%rax)
+    646c93da:	push   %rbp
+    646c93db:	outsb  %ds:(%rsi),(%dx)
+    646c93dc:	imul   $0x77,0x6f(%rsi),%ebp
+    646c93e0:	outsb  %ds:(%rsi),(%dx)
+    646c93e1:	and    %dh,0x73(%rax)
+    646c93e4:	gs jne 646c944b <.rdata+0x2b>
+    646c93e7:	outsl  %ds:(%rsi),(%dx)
+    646c93e8:	and    %dh,0x65(%rdx)
+    646c93eb:	insb   (%dx),%es:(%rdi)
+    646c93ec:	outsl  %ds:(%rsi),(%dx)
+    646c93ed:	movsxd 0x74(%rcx),%esp
+    646c93f0:	imul   $0x74696220,0x6e(%rdi),%ebp
+    646c93f7:	and    %dh,0x69(%rbx)
+    646c93fa:	jp     646c9461 <.rdata+0x1>
+    646c93fc:	and    %ah,0xa2e64(%rip)        # 6476c266 <.debug_str+0x94266>
+	...
+
+00000000646c9410 <.rdata>:
+    646c9410:	jo,pn  646c9477 <.rdata+0x17>
+    646c9413:	(bad)
+    646c9414:	je     646c9477 <.rdata+0x17>
+	...
+
+00000000646c9420 <.rdata>:
+    646c9420:	jae    646c9493 <.rdata+0x3>
+    646c9422:	jb     646c9498 <.rdata+0x8>
+	...
+    646c942c:	add    %al,(%rax)
+    646c942e:	add    %al,0x0(%rax)
+    646c9434:	add    %al,(%rax)
+    646c9436:	clc
+    646c9437:	incl   (%rax)
+    646c9439:	add    %al,(%rax)
     646c943b:	add    %al,(%rax)
-    646c943d:	add    %bh,%al
-    646c943f:	jg     646c94a6 <.rdata+0x16>
-
-00000000646c9440 <.rdata>:
-    646c9440:	gs js  646c94b3 <.rdata+0x23>
+    646c943d:	add    %dh,%al
+    646c943f:	jg     646c9441 <.rdata+0x21>
+    646c9441:	add    %al,(%rax)
+    646c9443:	add    %al,(%rax)
+    646c9445:	add    %dh,%al
+    646c9447:	(bad)
+	...
+
+00000000646c9450 <.rdata>:
+    646c9450:	movsxd 0x73(%rdi),%ebp
+	...
+    646c945b:	add    %al,(%rax)
+    646c945d:	add    %bh,%al
+    646c945f:	jg     646c94c6 <.rdata+0x16>
+
+00000000646c9460 <.rdata>:
+    646c9460:	gs js  646c94d3 <.rdata+0x23>
+	...
+    646c946b:	add    %al,(%rax)
+    646c946d:	add    %dh,%al
+    646c946f:	jg     646c9471 <.rdata+0x11>
+    646c9471:	add    %al,(%rax)
+    646c9473:	add    %al,(%rax)
+    646c9475:	add    %dh,%al
+    646c9477:	(bad)
+    646c9478:	out    %eax,(%dx)
+    646c9479:	cmp    %edi,%edx
+    646c947b:	incb   0x2e(%rdx)
+    646c947e:	xchg   %al,0x51(%rax)
+    646c9481:	xor    %ch,-0x78b6ef2b(%rip)        # ffffffffebb5a55c <.debug_str+0xffffffff8748255c>
+    646c9487:	rolb   $0x0,(%rax)
+    646c948a:	add    %al,(%rax)
+    646c948c:	add    %al,(%rax)
 	...
-    646c944b:	add    %al,(%rax)
-    646c944d:	add    %dh,%al
-    646c944f:	jg     646c9451 <.rdata+0x11>
-    646c9451:	add    %al,(%rax)
-    646c9453:	add    %al,(%rax)
-    646c9455:	add    %dh,%al
-    646c9457:	(bad)
-    646c9458:	out    %eax,(%dx)
-    646c9459:	cmp    %edi,%edx
-    646c945b:	incb   0x2e(%rdx)
-    646c945e:	xchg   %al,0x51(%rax)
-    646c9461:	xor    %ch,-0x78b6ef2b(%rip)        # ffffffffebb5a53c <.debug_str+0xffffffff8748253c>
-    646c9467:	rolb   $0x0,(%rax)
-    646c946a:	add    %al,(%rax)
-    646c946c:	add    %al,(%rax)
-	...
-
-00000000646c9470 <.rdata>:
-    646c9470:	insb   (%dx),%es:(%rdi)
-    646c9471:	outsl  %ds:(%rsi),(%dx)
-    646c9472:	add    %al,(%eax)
-	...
-    646c947d:	add    %dh,%al
-    646c947f:	incl   (%rax)
-    646c9481:	add    %al,(%rax)
-    646c9483:	add    %al,(%rax)
-    646c9485:	add    %bh,%al
-    646c9487:	jg     646c9489 <.rdata+0x19>
-    646c9489:	add    %al,(%rax)
-    646c948b:	add    %al,(%rax)
-    646c948d:	add    %dh,%al
-    646c948f:	jg     646c9501 <.rdata+0x71>
 
 00000000646c9490 <.rdata>:
-    646c9490:	jo     646c9501 <.rdata+0x71>
-    646c9492:	ja     646c9494 <.rdata+0x4>
+    646c9490:	insb   (%dx),%es:(%rdi)
+    646c9491:	outsl  %ds:(%rsi),(%dx)
+    646c9492:	add    %al,(%eax)
 	...
-    646c949c:	add    %al,(%rax)
-    646c949e:	clc
+    646c949d:	add    %dh,%al
     646c949f:	incl   (%rax)
     646c94a1:	add    %al,(%rax)
     646c94a3:	add    %al,(%rax)
     646c94a5:	add    %bh,%al
     646c94a7:	jg     646c94a9 <.rdata+0x19>
     646c94a9:	add    %al,(%rax)
     646c94ab:	add    %al,(%rax)
-    646c94ad:	add    %al,(%rax)
-    646c94af:	addb   $0x0,(%rax)
-    646c94b2:	add    %al,(%rax)
-    646c94b4:	add    %al,(%rax)
-    646c94b6:	lock incl (%rax)
-    646c94b9:	add    %al,(%rax)
-    646c94bb:	add    %al,(%rax)
-    646c94bd:	add    %dh,%al
-    646c94bf:	jg     646c94c1 <.rdata+0x31>
+    646c94ad:	add    %dh,%al
+    646c94af:	jg     646c9521 <.rdata+0x71>
+
+00000000646c94b0 <.rdata>:
+    646c94b0:	jo     646c9521 <.rdata+0x71>
+    646c94b2:	ja     646c94b4 <.rdata+0x4>
+	...
+    646c94bc:	add    %al,(%rax)
+    646c94be:	clc
+    646c94bf:	incl   (%rax)
     646c94c1:	add    %al,(%rax)
     646c94c3:	add    %al,(%rax)
-    646c94c5:	add    %dh,%al
-    646c94c7:	(bad)
-	...
+    646c94c5:	add    %bh,%al
+    646c94c7:	jg     646c94c9 <.rdata+0x19>
+    646c94c9:	add    %al,(%rax)
+    646c94cb:	add    %al,(%rax)
+    646c94cd:	add    %al,(%rax)
+    646c94cf:	addb   $0x0,(%rax)
+    646c94d2:	add    %al,(%rax)
     646c94d4:	add    %al,(%rax)
-    646c94d6:	add    %al,0x0(%rax)
-	...
-    646c94e4:	add    %al,(%rax)
-    646c94e6:	lock mov $0x0,%edi
-    646c94ec:	add    %al,(%rax)
-    646c94ee:	loopne 646c952f <.rdata+0x1f>
-    646c94f0:	add    %al,(%rax)
-    646c94f2:	sar    $0xff,%bh
-    646c94f5:	(bad)
-    646c94f6:	filds  0x0(%rcx)
-    646c94f9:	add    %al,(%rax)
-    646c94fb:	add    %al,(%rax)
-    646c94fd:	add    %ah,%al
-    646c94ff:	sar    $0xff,%edi
-    646c9502:	(bad)
-    646c9503:	(bad)
-    646c9504:	(bad)
-    646c9505:	(bad)
-    646c9506:	(bad)
-    646c9507:	jg     646c9509 <.rdata+0x79>
-    646c9509:	add    %al,(%rax)
-    646c950b:	add    %al,(%rax)
-    646c950d:	add    %al,(%rax)
-	...
-
-00000000646c9510 <.rdata>:
-    646c9510:	pop    %rdi
-    646c9511:	pop    %rdi
-    646c9512:	jo     646c9583 <.rdata+0x13>
-    646c9514:	ja     646c957f <.rdata+0xf>
-	...
-    646c951e:	clc
-    646c951f:	incl   (%rax)
-    646c9521:	add    %al,(%rax)
-    646c9523:	add    %al,(%rax)
-    646c9525:	add    %bh,%al
-    646c9527:	jg     646c9529 <.rdata+0x19>
+    646c94d6:	lock incl (%rax)
+    646c94d9:	add    %al,(%rax)
+    646c94db:	add    %al,(%rax)
+    646c94dd:	add    %dh,%al
+    646c94df:	jg     646c94e1 <.rdata+0x31>
+    646c94e1:	add    %al,(%rax)
+    646c94e3:	add    %al,(%rax)
+    646c94e5:	add    %dh,%al
+    646c94e7:	(bad)
+	...
+    646c94f4:	add    %al,(%rax)
+    646c94f6:	add    %al,0x0(%rax)
+	...
+    646c9504:	add    %al,(%rax)
+    646c9506:	lock mov $0x0,%edi
+    646c950c:	add    %al,(%rax)
+    646c950e:	loopne 646c954f <.rdata+0x1f>
+    646c9510:	add    %al,(%rax)
+    646c9512:	sar    $0xff,%bh
+    646c9515:	(bad)
+    646c9516:	filds  0x0(%rcx)
+    646c9519:	add    %al,(%rax)
+    646c951b:	add    %al,(%rax)
+    646c951d:	add    %ah,%al
+    646c951f:	sar    $0xff,%edi
+    646c9522:	(bad)
+    646c9523:	(bad)
+    646c9524:	(bad)
+    646c9525:	(bad)
+    646c9526:	(bad)
+    646c9527:	jg     646c9529 <.rdata+0x79>
     646c9529:	add    %al,(%rax)
     646c952b:	add    %al,(%rax)
-    646c952d:	add    %dh,%al
-    646c952f:	(bad)
-    646c9530:	add    %al,(%rax)
-    646c9532:	add    %al,(%rax)
-    646c9534:	add    %al,(%rax)
-    646c9536:	add    %al,0x0(%rax)
-    646c953c:	add    %al,(%rax)
-    646c953e:	lock jg 646c9541 <.rdata+0x31>
+    646c952d:	add    %al,(%rax)
+	...
+
+00000000646c9530 <.rdata>:
+    646c9530:	pop    %rdi
+    646c9531:	pop    %rdi
+    646c9532:	jo     646c95a3 <.rdata+0x13>
+    646c9534:	ja     646c959f <.rdata+0xf>
+	...
+    646c953e:	clc
+    646c953f:	incl   (%rax)
     646c9541:	add    %al,(%rax)
     646c9543:	add    %al,(%rax)
-    646c9545:	add    %dh,%al
-    646c9547:	incl   (%rax)
+    646c9545:	add    %bh,%al
+    646c9547:	jg     646c9549 <.rdata+0x19>
     646c9549:	add    %al,(%rax)
     646c954b:	add    %al,(%rax)
-    646c954d:	add    %al,(%rax)
-    646c954f:	add    %bh,%bh
-    646c9551:	(bad)
-    646c9552:	(bad)
-    646c9553:	(bad)
-    646c9554:	(bad)
-    646c9555:	(bad)
-    646c9556:	(bad)
-    646c9557:	jg     646c9559 <.rdata+0x49>
-	...
-    646c9565:	add    %al,(%rax)
-    646c9567:	addb   $0x0,(%rax)
-    646c956a:	add    %al,(%rax)
-    646c956c:	add    %al,(%rax)
-	...
-
-00000000646c9570 <.rdata>:
-    646c9570:	rex.B jb 646c95da <.rdata+0x6a>
-    646c9573:	jne    646c95e2 <.rdata+0x72>
-    646c9575:	outsb  %gs:(%rsi),(%dx)
-    646c9577:	je     646c9599 <.rdata+0x29>
-    646c9579:	outsl  %fs:(%rsi),(%dx)
-    646c957b:	insl   (%dx),%es:(%rdi)
-    646c957c:	(bad)
-    646c957d:	imul   $0x6f727265,0x20(%rsi),%ebp
-    646c9584:	jb     646c95a6 <.rdata+0x36>
-    646c9586:	sub    %al,0x4d(%rdi,%rcx,2)
-    646c958a:	rex.B
-    646c958b:	rex.WB
-    646c958c:	rex.WRX sub %r8,(%rax)
-    646c958f:	rex.B jb 646c95f9 <.rdata+0x89>
-    646c9592:	jne    646c9601 <.rdata+0x91>
-    646c9594:	outsb  %gs:(%rsi),(%dx)
-    646c9596:	je     646c95b8 <.rdata+0x48>
-    646c9598:	jae    646c9603 <.rdata+0x93>
-    646c959a:	outsb  %ds:(%rsi),(%dx)
-    646c959b:	addr32 jne 646c960a <.rdata+0x9a>
-    646c959e:	(bad)
-    646c959f:	jb     646c960a <.rdata+0x9a>
-    646c95a1:	je     646c961c <.rdata+0xac>
-    646c95a3:	and    %ch,(%rax)
-    646c95a5:	push   %rbx
-    646c95a6:	rex.WB
-    646c95a7:	rex.RXB
-    646c95a8:	rex.WRX sub %r8,(%rax)
-    646c95ab:	add    %al,(%rax)
-    646c95ad:	add    %al,(%rax)
-    646c95af:	add    %cl,0x76(%rdi)
-    646c95b2:	gs jb  646c961b <.rdata+0xab>
-    646c95b5:	insb   (%dx),%es:(%rdi)
-    646c95b6:	outsl  %ds:(%rsi),(%dx)
-    646c95b7:	ja     646c95d9 <.rdata+0x69>
-    646c95b9:	jb     646c961c <.rdata+0xac>
-    646c95bb:	outsb  %ds:(%rsi),(%dx)
-    646c95bc:	and    %ah,%gs:0x72(%ebp)
-    646c95c1:	jb     646c9632 <.rdata+0xc2>
-    646c95c3:	jb     646c95e5 <.rdata+0x75>
-    646c95c5:	sub    %cl,0x56(%rdi)
-    646c95c8:	rex.RB push %r10
-    646c95ca:	rex.RX
-    646c95cb:	rex.WR
-    646c95cc:	rex.WRXB push %r15
-    646c95ce:	sub    %eax,(%rax)
-    646c95d0:	push   %rax
-    646c95d1:	(bad)
-    646c95d2:	jb     646c9648 <.rdata+0xd8>
-    646c95d4:	imul   $0x736f6c20,0x6c(%rcx),%esp
-    646c95db:	jae    646c95fd <.rdata+0x8d>
-    646c95dd:	outsl  %ds:(%rsi),(%dx)
-    646c95de:	data16 and %dh,0x69(%rbx)
-    646c95e2:	outsb  %ds:(%esi),(%dx)
-    646c95e4:	imul   $0x636e6163,0x69(%rsi),%esp
-    646c95eb:	and    %ch,%gs:(%rax)
-    646c95ee:	push   %rax
-    646c95ef:	rex.WR
-    646c95f0:	rex.WRXB push %r11
-    646c95f2:	push   %rbx
-    646c95f3:	sub    %eax,(%rax)
-    646c95f5:	add    %al,(%rax)
-    646c95f7:	add    %dl,0x74(%rdi,%rbp,2)
-    646c95fb:	(bad)
-    646c95fc:	insb   (%dx),%es:(%rdi)
-    646c95fd:	and    %ch,0x73(%rdi,%rbp,2)
-    646c9601:	jae    646c9623 <.rdata+0xb3>
-    646c9603:	outsl  %ds:(%rsi),(%dx)
-    646c9604:	data16 and %dh,0x69(%rbx)
-    646c9608:	outsb  %ds:(%esi),(%dx)
-    646c960a:	imul   $0x636e6163,0x69(%rsi),%esp
-    646c9611:	and    %ch,%gs:(%rax)
-    646c9614:	push   %rsp
-    646c9615:	rex.WR
-    646c9616:	rex.WRXB push %r11
-    646c9618:	push   %rbx
-    646c9619:	sub    %eax,(%rax)
-    646c961b:	add    %al,(%rax)
-    646c961d:	add    %al,(%rax)
-    646c961f:	add    %dl,0x65(%rax,%rbp,2)
-    646c9623:	and    %dh,0x65(%rdx)
-    646c9626:	jae    646c969d <.rdata+0x12d>
-    646c9628:	insb   (%dx),%es:(%rdi)
-    646c9629:	je     646c964b <.rdata+0xdb>
-    646c962b:	imul   $0x206f6f74,0x20(%rbx),%esi
-    646c9632:	jae    646c96a1 <.rdata+0x131>
-    646c9634:	(bad)
-    646c9635:	insb   (%dx),%es:(%rdi)
-    646c9636:	insb   (%dx),%es:(%rdi)
-    646c9637:	and    %dh,0x20(%rdi,%rbp,2)
-    646c963b:	(bad)
-    646c963d:	and    %dh,0x65(%rdx)
-    646c9640:	jo     646c96b4 <.refptr._CRT_MT+0x4>
-    646c9642:	gs jae 646c96aa <.rdata+0x13a>
-    646c9645:	outsb  %ds:(%rsi),(%dx)
-    646c9646:	je     646c96ad <.rdata+0x13d>
-    646c9648:	and    %ch,%fs:(%rax)
-    646c964b:	push   %rbp
-    646c964c:	rex.WRX
-    646c964d:	rex.R
-    646c964e:	rex.RB push %r10
-    646c9650:	rex.RX
-    646c9651:	rex.WR
-    646c9652:	rex.WRXB push %r15
-    646c9654:	sub    %eax,(%rax)
-    646c9656:	push   %rbp
-    646c9657:	outsb  %ds:(%rsi),(%dx)
-    646c9658:	imul   $0x77,0x6f(%rsi),%ebp
-    646c965c:	outsb  %ds:(%rsi),(%dx)
-    646c965d:	and    %ah,0x72(%rbp)
-    646c9660:	jb     646c96d1 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x1>
-    646c9662:	jb     646c9664 <.rdata+0xf4>
-    646c9664:	add    %al,(%rax)
-    646c9666:	add    %al,(%rax)
-    646c9668:	pop    %rdi
-    646c9669:	insl   (%dx),%es:(%rdi)
-    646c966a:	(bad)
-    646c966b:	je     646c96d5 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x5>
-    646c966d:	gs jb  646c96e2 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__+0x2>
-    646c9670:	sub    %ch,(%rcx)
-    646c9672:	cmp    (%rax),%ah
-    646c9674:	and    $0x6e692073,%eax
-    646c9679:	and    %ah,0x67252873(%rip)        # cb91bef2 <.debug_str+0x67243ef2>
-    646c967f:	sub    $0x20,%al
-    646c9681:	and    $0x20202967,%eax
-    646c9686:	sub    %dh,0x65(%rdx)
-    646c9689:	je     646c9701 <.refptr.__image_base__+0x1>
-    646c968b:	(bad)
-    646c968c:	insb   (%dx),%es:(%rdi)
-    646c968d:	cmp    $0xa296725,%eax
-    646c9692:	add    %al,(%rax)
-    646c9694:	or     $0xe7,%al
-    646c9696:	(bad)
-    646c9697:	decl   -0x1a(%rbp)
-    646c969a:	(bad)
-    646c969b:	(bad)
-    646c969c:	mov    $0xccffffe6,%esp
-    646c96a1:	out    %al,$0xff
-    646c96a3:	(bad)
-    646c96a4:	fsub   %st,%st(6)
-    646c96a6:	(bad)
-    646c96a7:	(bad)
-    646c96a8:	in     (%dx),%al
-    646c96a9:	out    %al,$0xff
+    646c954d:	add    %dh,%al
+    646c954f:	(bad)
+    646c9550:	add    %al,(%rax)
+    646c9552:	add    %al,(%rax)
+    646c9554:	add    %al,(%rax)
+    646c9556:	add    %al,0x0(%rax)
+    646c955c:	add    %al,(%rax)
+    646c955e:	lock jg 646c9561 <.rdata+0x31>
+    646c9561:	add    %al,(%rax)
+    646c9563:	add    %al,(%rax)
+    646c9565:	add    %dh,%al
+    646c9567:	incl   (%rax)
+    646c9569:	add    %al,(%rax)
+    646c956b:	add    %al,(%rax)
+    646c956d:	add    %al,(%rax)
+    646c956f:	add    %bh,%bh
+    646c9571:	(bad)
+    646c9572:	(bad)
+    646c9573:	(bad)
+    646c9574:	(bad)
+    646c9575:	(bad)
+    646c9576:	(bad)
+    646c9577:	jg     646c9579 <.rdata+0x49>
+	...
+    646c9585:	add    %al,(%rax)
+    646c9587:	addb   $0x0,(%rax)
+    646c958a:	add    %al,(%rax)
+    646c958c:	add    %al,(%rax)
+	...
+
+00000000646c9590 <.rdata>:
+    646c9590:	rex.B jb 646c95fa <.rdata+0x6a>
+    646c9593:	jne    646c9602 <.rdata+0x72>
+    646c9595:	outsb  %gs:(%rsi),(%dx)
+    646c9597:	je     646c95b9 <.rdata+0x29>
+    646c9599:	outsl  %fs:(%rsi),(%dx)
+    646c959b:	insl   (%dx),%es:(%rdi)
+    646c959c:	(bad)
+    646c959d:	imul   $0x6f727265,0x20(%rsi),%ebp
+    646c95a4:	jb     646c95c6 <.rdata+0x36>
+    646c95a6:	sub    %al,0x4d(%rdi,%rcx,2)
+    646c95aa:	rex.B
+    646c95ab:	rex.WB
+    646c95ac:	rex.WRX sub %r8,(%rax)
+    646c95af:	rex.B jb 646c9619 <.rdata+0x89>
+    646c95b2:	jne    646c9621 <.rdata+0x91>
+    646c95b4:	outsb  %gs:(%rsi),(%dx)
+    646c95b6:	je     646c95d8 <.rdata+0x48>
+    646c95b8:	jae    646c9623 <.rdata+0x93>
+    646c95ba:	outsb  %ds:(%rsi),(%dx)
+    646c95bb:	addr32 jne 646c962a <.rdata+0x9a>
+    646c95be:	(bad)
+    646c95bf:	jb     646c962a <.rdata+0x9a>
+    646c95c1:	je     646c963c <.rdata+0xac>
+    646c95c3:	and    %ch,(%rax)
+    646c95c5:	push   %rbx
+    646c95c6:	rex.WB
+    646c95c7:	rex.RXB
+    646c95c8:	rex.WRX sub %r8,(%rax)
+    646c95cb:	add    %al,(%rax)
+    646c95cd:	add    %al,(%rax)
+    646c95cf:	add    %cl,0x76(%rdi)
+    646c95d2:	gs jb  646c963b <.rdata+0xab>
+    646c95d5:	insb   (%dx),%es:(%rdi)
+    646c95d6:	outsl  %ds:(%rsi),(%dx)
+    646c95d7:	ja     646c95f9 <.rdata+0x69>
+    646c95d9:	jb     646c963c <.rdata+0xac>
+    646c95db:	outsb  %ds:(%rsi),(%dx)
+    646c95dc:	and    %ah,%gs:0x72(%ebp)
+    646c95e1:	jb     646c9652 <.rdata+0xc2>
+    646c95e3:	jb     646c9605 <.rdata+0x75>
+    646c95e5:	sub    %cl,0x56(%rdi)
+    646c95e8:	rex.RB push %r10
+    646c95ea:	rex.RX
+    646c95eb:	rex.WR
+    646c95ec:	rex.WRXB push %r15
+    646c95ee:	sub    %eax,(%rax)
+    646c95f0:	push   %rax
+    646c95f1:	(bad)
+    646c95f2:	jb     646c9668 <.rdata+0xd8>
+    646c95f4:	imul   $0x736f6c20,0x6c(%rcx),%esp
+    646c95fb:	jae    646c961d <.rdata+0x8d>
+    646c95fd:	outsl  %ds:(%rsi),(%dx)
+    646c95fe:	data16 and %dh,0x69(%rbx)
+    646c9602:	outsb  %ds:(%esi),(%dx)
+    646c9604:	imul   $0x636e6163,0x69(%rsi),%esp
+    646c960b:	and    %ch,%gs:(%rax)
+    646c960e:	push   %rax
+    646c960f:	rex.WR
+    646c9610:	rex.WRXB push %r11
+    646c9612:	push   %rbx
+    646c9613:	sub    %eax,(%rax)
+    646c9615:	add    %al,(%rax)
+    646c9617:	add    %dl,0x74(%rdi,%rbp,2)
+    646c961b:	(bad)
+    646c961c:	insb   (%dx),%es:(%rdi)
+    646c961d:	and    %ch,0x73(%rdi,%rbp,2)
+    646c9621:	jae    646c9643 <.rdata+0xb3>
+    646c9623:	outsl  %ds:(%rsi),(%dx)
+    646c9624:	data16 and %dh,0x69(%rbx)
+    646c9628:	outsb  %ds:(%esi),(%dx)
+    646c962a:	imul   $0x636e6163,0x69(%rsi),%esp
+    646c9631:	and    %ch,%gs:(%rax)
+    646c9634:	push   %rsp
+    646c9635:	rex.WR
+    646c9636:	rex.WRXB push %r11
+    646c9638:	push   %rbx
+    646c9639:	sub    %eax,(%rax)
+    646c963b:	add    %al,(%rax)
+    646c963d:	add    %al,(%rax)
+    646c963f:	add    %dl,0x65(%rax,%rbp,2)
+    646c9643:	and    %dh,0x65(%rdx)
+    646c9646:	jae    646c96bd <.rdata+0x12d>
+    646c9648:	insb   (%dx),%es:(%rdi)
+    646c9649:	je     646c966b <.rdata+0xdb>
+    646c964b:	imul   $0x206f6f74,0x20(%rbx),%esi
+    646c9652:	jae    646c96c1 <.rdata+0x131>
+    646c9654:	(bad)
+    646c9655:	insb   (%dx),%es:(%rdi)
+    646c9656:	insb   (%dx),%es:(%rdi)
+    646c9657:	and    %dh,0x20(%rdi,%rbp,2)
+    646c965b:	(bad)
+    646c965d:	and    %dh,0x65(%rdx)
+    646c9660:	jo     646c96d4 <.refptr._CRT_MT+0x4>
+    646c9662:	gs jae 646c96ca <.rdata+0x13a>
+    646c9665:	outsb  %ds:(%rsi),(%dx)
+    646c9666:	je     646c96cd <.rdata+0x13d>
+    646c9668:	and    %ch,%fs:(%rax)
+    646c966b:	push   %rbp
+    646c966c:	rex.WRX
+    646c966d:	rex.R
+    646c966e:	rex.RB push %r10
+    646c9670:	rex.RX
+    646c9671:	rex.WR
+    646c9672:	rex.WRXB push %r15
+    646c9674:	sub    %eax,(%rax)
+    646c9676:	push   %rbp
+    646c9677:	outsb  %ds:(%rsi),(%dx)
+    646c9678:	imul   $0x77,0x6f(%rsi),%ebp
+    646c967c:	outsb  %ds:(%rsi),(%dx)
+    646c967d:	and    %ah,0x72(%rbp)
+    646c9680:	jb     646c96f1 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x1>
+    646c9682:	jb     646c9684 <.rdata+0xf4>
+    646c9684:	add    %al,(%rax)
+    646c9686:	add    %al,(%rax)
+    646c9688:	pop    %rdi
+    646c9689:	insl   (%dx),%es:(%rdi)
+    646c968a:	(bad)
+    646c968b:	je     646c96f5 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x5>
+    646c968d:	gs jb  646c9702 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__+0x2>
+    646c9690:	sub    %ch,(%rcx)
+    646c9692:	cmp    (%rax),%ah
+    646c9694:	and    $0x6e692073,%eax
+    646c9699:	and    %ah,0x67252873(%rip)        # cb91bf12 <.debug_str+0x67243f12>
+    646c969f:	sub    $0x20,%al
+    646c96a1:	and    $0x20202967,%eax
+    646c96a6:	sub    %dh,0x65(%rdx)
+    646c96a9:	je     646c9721 <.refptr.__image_base__+0x1>
     646c96ab:	(bad)
-    646c96ac:	cld
-    646c96ad:	out    %al,$0xff
-    646c96af:	jmp    *(%rax)
-
-00000000646c96b0 <.refptr._CRT_MT>:
-    646c96b0:	and    %al,0x646c(%rax)
+    646c96ac:	insb   (%dx),%es:(%rdi)
+    646c96ad:	cmp    $0xa296725,%eax
+    646c96b2:	add    %al,(%rax)
+    646c96b4:	sub    $0xe6,%al
+    646c96b6:	(bad)
+    646c96b7:	ljmp   *-0x1b(%rbp)
+    646c96ba:	(bad)
+    646c96bb:	(bad)
+    646c96bc:	fsub   %st,%st(5)
+    646c96be:	(bad)
+    646c96bf:	(bad)
+    646c96c0:	in     (%dx),%al
+    646c96c1:	in     $0xff,%eax
+    646c96c3:	(bad)
+    646c96c4:	cld
+    646c96c5:	in     $0xff,%eax
+    646c96c7:	decl   (%rsi,%riz,8)
+    646c96ca:	(bad)
+    646c96cb:	lcall  *(%rsi,%riz,8)
+    646c96ce:	(bad)
+    646c96cf:	jmp    *(%rax)
+
+00000000646c96d0 <.refptr._CRT_MT>:
+    646c96d0:	and    %al,0x646c(%rax)
+	...
+
+00000000646c96e0 <.refptr.__CTOR_LIST__>:
+    646c96e0:	cmpb   $0x64,0x6c(%rbp)
+	...
+
+00000000646c96f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
+    646c96f0:	lock cltd
+    646c96f2:	insb   (%dx),%es:(%rdi)
+    646c96f3:	add    %al,%fs:(%rax)
 	...
 
-00000000646c96c0 <.refptr.__CTOR_LIST__>:
-    646c96c0:	rex jle 646c972f <.refptr.__native_startup_lock+0xf>
-    646c96c3:	add    %al,%fs:(%rax)
-	...
-
-00000000646c96d0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
-    646c96d0:	rcrb   0x646c(%rcx)
-	...
-
-00000000646c96e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>:
-    646c96e0:	rcrb   0x646c(%rcx)
-	...
-
-00000000646c96f0 <.refptr.__dyn_tls_init_callback>:
-    646c96f0:	adcb   $0x0,0x646c(%rdx)
-	...
-
-00000000646c9700 <.refptr.__image_base__>:
-    646c9700:	add    %al,(%rax)
+00000000646c9700 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>:
+    646c9700:	lock cltd
     646c9702:	insb   (%dx),%es:(%rdi)
     646c9703:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9710 <.refptr.__native_dllmain_reason>:
-    646c9710:	adc    $0x80,%al
-    646c9712:	insb   (%dx),%es:(%rdi)
-    646c9713:	add    %al,%fs:(%rax)
+00000000646c9710 <.refptr.__dyn_tls_init_callback>:
+    646c9710:	movabs 0x646c92,%al
+    646c9719:	add    %al,(%rax)
+    646c971b:	add    %al,(%rax)
+    646c971d:	add    %al,(%rax)
 	...
 
-00000000646c9720 <.refptr.__native_startup_lock>:
-    646c9720:	lretq
+00000000646c9720 <.refptr.__image_base__>:
+    646c9720:	add    %al,(%rax)
     646c9722:	insb   (%dx),%es:(%rdi)
     646c9723:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9730 <.refptr.__native_startup_state>:
-    646c9730:	rex lret
+00000000646c9730 <.refptr.__native_dllmain_reason>:
+    646c9730:	adc    $0x80,%al
     646c9732:	insb   (%dx),%es:(%rdi)
     646c9733:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9740 <.refptr.__xc_a>:
-    646c9740:	add    %dh,%al
+00000000646c9740 <.refptr.__native_startup_lock>:
+    646c9740:	sub    %cl,%bl
     646c9742:	insb   (%dx),%es:(%rdi)
     646c9743:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9750 <.refptr.__xc_z>:
-    646c9750:	or     %dh,%al
+00000000646c9750 <.refptr.__native_startup_state>:
+    646c9750:	and    %cl,%bl
     646c9752:	insb   (%dx),%es:(%rdi)
     646c9753:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9760 <.refptr.__xi_a>:
-    646c9760:	adc    %dh,%al
+00000000646c9760 <.refptr.__xc_a>:
+    646c9760:	add    %dh,%al
     646c9762:	insb   (%dx),%es:(%rdi)
     646c9763:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9770 <.refptr.__xi_z>:
-    646c9770:	and    %dh,%al
+00000000646c9770 <.refptr.__xc_z>:
+    646c9770:	or     %dh,%al
     646c9772:	insb   (%dx),%es:(%rdi)
     646c9773:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9780 <.refptr.mingw_app_type>:
-    646c9780:	lock (bad)
+00000000646c9780 <.refptr.__xi_a>:
+    646c9780:	adc    %dh,%al
     646c9782:	insb   (%dx),%es:(%rdi)
     646c9783:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9790 <.rdata$zzz>:
-    646c9790:	rex.RXB
-    646c9791:	rex.XB
-    646c9792:	rex.XB cmp (%r8),%spl
-    646c9795:	sub    %bh,0x38(%rax)
-    646c9798:	ss pop %rdi
-    646c979a:	ss xor $0x2d,%al
-    646c979d:	ja     646c9808 <.rdata$zzz+0x38>
-    646c979f:	outsb  %ds:(%rsi),(%dx)
-    646c97a0:	xor    (%rdx),%esi
-    646c97a2:	sub    $0x2d686573,%eax
-    646c97a7:	jb     646c980e <.rdata$zzz+0x3e>
-    646c97a9:	jbe    646c97db <.rdata$zzz+0xb>
-    646c97ab:	sub    $0x20,%al
-    646c97ad:	rex.X jne 646c9819 <.rdata$zzz+0x9>
-    646c97b0:	insb   (%dx),%es:(%rdi)
-    646c97b1:	je     646c97d3 <.rdata$zzz+0x3>
-    646c97b3:	(bad)
-    646c97b4:	jns    646c97d6 <.rdata$zzz+0x6>
-    646c97b6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c97be:	xor    $0x20,%al
-    646c97c0:	jo     646c9834 <.rdata$zzz+0x24>
-    646c97c2:	outsl  %ds:(%rsi),(%dx)
-    646c97c3:	push   $0x65
-    646c97c5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c97c9:	cmp    %ch,(%rsi)
-    646c97cb:	xor    %ebp,(%rsi)
-    646c97cd:	xor    %al,(%rax)
-	...
-
-00000000646c97d0 <.rdata$zzz>:
-    646c97d0:	rex.RXB
-    646c97d1:	rex.XB
-    646c97d2:	rex.XB cmp (%r8),%spl
-    646c97d5:	sub    %bh,0x38(%rax)
-    646c97d8:	ss pop %rdi
-    646c97da:	ss xor $0x2d,%al
-    646c97dd:	ja     646c9848 <.rdata$zzz+0x38>
-    646c97df:	outsb  %ds:(%rsi),(%dx)
-    646c97e0:	xor    (%rdx),%esi
-    646c97e2:	sub    $0x2d686573,%eax
-    646c97e7:	jb     646c984e <.rdata$zzz+0x3e>
-    646c97e9:	jbe    646c981b <.rdata$zzz+0xb>
-    646c97eb:	sub    $0x20,%al
-    646c97ed:	rex.X jne 646c9859 <.rdata$zzz+0x9>
-    646c97f0:	insb   (%dx),%es:(%rdi)
-    646c97f1:	je     646c9813 <.rdata$zzz+0x3>
-    646c97f3:	(bad)
-    646c97f4:	jns    646c9816 <.rdata$zzz+0x6>
-    646c97f6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c97fe:	xor    $0x20,%al
-    646c9800:	jo     646c9874 <.rdata$zzz+0x24>
-    646c9802:	outsl  %ds:(%rsi),(%dx)
-    646c9803:	push   $0x65
-    646c9805:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9809:	cmp    %ch,(%rsi)
-    646c980b:	xor    %ebp,(%rsi)
-    646c980d:	xor    %al,(%rax)
-	...
-
-00000000646c9810 <.rdata$zzz>:
-    646c9810:	rex.RXB
-    646c9811:	rex.XB
-    646c9812:	rex.XB cmp (%r8),%spl
-    646c9815:	sub    %bh,0x38(%rax)
-    646c9818:	ss pop %rdi
-    646c981a:	ss xor $0x2d,%al
-    646c981d:	ja     646c9888 <.rdata$zzz+0x38>
-    646c981f:	outsb  %ds:(%rsi),(%dx)
-    646c9820:	xor    (%rdx),%esi
-    646c9822:	sub    $0x2d686573,%eax
-    646c9827:	jb     646c988e <.rdata$zzz+0x3e>
-    646c9829:	jbe    646c985b <.rdata$zzz+0xb>
-    646c982b:	sub    $0x20,%al
-    646c982d:	rex.X jne 646c9899 <.rdata$zzz+0x9>
-    646c9830:	insb   (%dx),%es:(%rdi)
-    646c9831:	je     646c9853 <.rdata$zzz+0x3>
-    646c9833:	(bad)
-    646c9834:	jns    646c9856 <.rdata$zzz+0x6>
-    646c9836:	imul   $0x36572d57,0x47(%r14),%r13
-    646c983e:	xor    $0x20,%al
-    646c9840:	jo     646c98b4 <.rdata$zzz+0x24>
-    646c9842:	outsl  %ds:(%rsi),(%dx)
-    646c9843:	push   $0x65
-    646c9845:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9849:	cmp    %ch,(%rsi)
-    646c984b:	xor    %ebp,(%rsi)
-    646c984d:	xor    %al,(%rax)
-	...
-
-00000000646c9850 <.rdata$zzz>:
-    646c9850:	rex.RXB
-    646c9851:	rex.XB
-    646c9852:	rex.XB cmp (%r8),%spl
-    646c9855:	sub    %bh,0x38(%rax)
-    646c9858:	ss pop %rdi
-    646c985a:	ss xor $0x2d,%al
-    646c985d:	ja     646c98c8 <.rdata$zzz+0x38>
-    646c985f:	outsb  %ds:(%rsi),(%dx)
-    646c9860:	xor    (%rdx),%esi
-    646c9862:	sub    $0x2d686573,%eax
-    646c9867:	jb     646c98ce <.rdata$zzz+0x3e>
-    646c9869:	jbe    646c989b <.rdata$zzz+0xb>
-    646c986b:	sub    $0x20,%al
-    646c986d:	rex.X jne 646c98d9 <.rdata$zzz+0x9>
-    646c9870:	insb   (%dx),%es:(%rdi)
-    646c9871:	je     646c9893 <.rdata$zzz+0x3>
-    646c9873:	(bad)
-    646c9874:	jns    646c9896 <.rdata$zzz+0x6>
-    646c9876:	imul   $0x36572d57,0x47(%r14),%r13
-    646c987e:	xor    $0x20,%al
-    646c9880:	jo     646c98f4 <.rdata$zzz+0x24>
-    646c9882:	outsl  %ds:(%rsi),(%dx)
-    646c9883:	push   $0x65
-    646c9885:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9889:	cmp    %ch,(%rsi)
-    646c988b:	xor    %ebp,(%rsi)
-    646c988d:	xor    %al,(%rax)
-	...
-
-00000000646c9890 <.rdata$zzz>:
-    646c9890:	rex.RXB
-    646c9891:	rex.XB
-    646c9892:	rex.XB cmp (%r8),%spl
-    646c9895:	sub    %bh,0x38(%rax)
-    646c9898:	ss pop %rdi
-    646c989a:	ss xor $0x2d,%al
-    646c989d:	ja     646c9908 <.rdata$zzz+0x38>
-    646c989f:	outsb  %ds:(%rsi),(%dx)
-    646c98a0:	xor    (%rdx),%esi
-    646c98a2:	sub    $0x2d686573,%eax
-    646c98a7:	jb     646c990e <.rdata$zzz+0x3e>
-    646c98a9:	jbe    646c98db <.rdata$zzz+0xb>
-    646c98ab:	sub    $0x20,%al
-    646c98ad:	rex.X jne 646c9919 <.rdata$zzz+0x9>
-    646c98b0:	insb   (%dx),%es:(%rdi)
-    646c98b1:	je     646c98d3 <.rdata$zzz+0x3>
-    646c98b3:	(bad)
-    646c98b4:	jns    646c98d6 <.rdata$zzz+0x6>
-    646c98b6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c98be:	xor    $0x20,%al
-    646c98c0:	jo     646c9934 <.rdata$zzz+0x24>
-    646c98c2:	outsl  %ds:(%rsi),(%dx)
-    646c98c3:	push   $0x65
-    646c98c5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c98c9:	cmp    %ch,(%rsi)
-    646c98cb:	xor    %ebp,(%rsi)
-    646c98cd:	xor    %al,(%rax)
-	...
-
-00000000646c98d0 <.rdata$zzz>:
-    646c98d0:	rex.RXB
-    646c98d1:	rex.XB
-    646c98d2:	rex.XB cmp (%r8),%spl
-    646c98d5:	sub    %bh,0x38(%rax)
-    646c98d8:	ss pop %rdi
-    646c98da:	ss xor $0x2d,%al
-    646c98dd:	ja     646c9948 <.rdata$zzz+0x38>
-    646c98df:	outsb  %ds:(%rsi),(%dx)
-    646c98e0:	xor    (%rdx),%esi
-    646c98e2:	sub    $0x2d686573,%eax
-    646c98e7:	jb     646c994e <.rdata$zzz+0x3e>
-    646c98e9:	jbe    646c991b <.rdata$zzz+0xb>
-    646c98eb:	sub    $0x20,%al
-    646c98ed:	rex.X jne 646c9959 <.rdata$zzz+0x9>
-    646c98f0:	insb   (%dx),%es:(%rdi)
-    646c98f1:	je     646c9913 <.rdata$zzz+0x3>
-    646c98f3:	(bad)
-    646c98f4:	jns    646c9916 <.rdata$zzz+0x6>
-    646c98f6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c98fe:	xor    $0x20,%al
-    646c9900:	jo     646c9974 <.rdata$zzz+0x24>
-    646c9902:	outsl  %ds:(%rsi),(%dx)
-    646c9903:	push   $0x65
-    646c9905:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9909:	cmp    %ch,(%rsi)
-    646c990b:	xor    %ebp,(%rsi)
-    646c990d:	xor    %al,(%rax)
-	...
-
-00000000646c9910 <.rdata$zzz>:
-    646c9910:	rex.RXB
-    646c9911:	rex.XB
-    646c9912:	rex.XB cmp (%r8),%spl
-    646c9915:	sub    %bh,0x38(%rax)
-    646c9918:	ss pop %rdi
-    646c991a:	ss xor $0x2d,%al
-    646c991d:	ja     646c9988 <.rdata$zzz+0x38>
-    646c991f:	outsb  %ds:(%rsi),(%dx)
-    646c9920:	xor    (%rdx),%esi
-    646c9922:	sub    $0x2d686573,%eax
-    646c9927:	jb     646c998e <.rdata$zzz+0x3e>
-    646c9929:	jbe    646c995b <.rdata$zzz+0xb>
-    646c992b:	sub    $0x20,%al
-    646c992d:	rex.X jne 646c9999 <.rdata$zzz+0x9>
-    646c9930:	insb   (%dx),%es:(%rdi)
-    646c9931:	je     646c9953 <.rdata$zzz+0x3>
-    646c9933:	(bad)
-    646c9934:	jns    646c9956 <.rdata$zzz+0x6>
-    646c9936:	imul   $0x36572d57,0x47(%r14),%r13
-    646c993e:	xor    $0x20,%al
-    646c9940:	jo     646c99b4 <.rdata$zzz+0x24>
-    646c9942:	outsl  %ds:(%rsi),(%dx)
-    646c9943:	push   $0x65
-    646c9945:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9949:	cmp    %ch,(%rsi)
-    646c994b:	xor    %ebp,(%rsi)
-    646c994d:	xor    %al,(%rax)
-	...
-
-00000000646c9950 <.rdata$zzz>:
-    646c9950:	rex.RXB
-    646c9951:	rex.XB
-    646c9952:	rex.XB cmp (%r8),%spl
-    646c9955:	sub    %bh,0x38(%rax)
-    646c9958:	ss pop %rdi
-    646c995a:	ss xor $0x2d,%al
-    646c995d:	ja     646c99c8 <.rdata$zzz+0x38>
-    646c995f:	outsb  %ds:(%rsi),(%dx)
-    646c9960:	xor    (%rdx),%esi
-    646c9962:	sub    $0x2d686573,%eax
-    646c9967:	jb     646c99ce <.rdata$zzz+0x3e>
-    646c9969:	jbe    646c999b <.rdata$zzz+0xb>
-    646c996b:	sub    $0x20,%al
-    646c996d:	rex.X jne 646c99d9 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x9>
-    646c9970:	insb   (%dx),%es:(%rdi)
-    646c9971:	je     646c9993 <.rdata$zzz+0x3>
-    646c9973:	(bad)
-    646c9974:	jns    646c9996 <.rdata$zzz+0x6>
-    646c9976:	imul   $0x36572d57,0x47(%r14),%r13
-    646c997e:	xor    $0x20,%al
-    646c9980:	jo     646c99f4 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x24>
-    646c9982:	outsl  %ds:(%rsi),(%dx)
-    646c9983:	push   $0x65
-    646c9985:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9989:	cmp    %ch,(%rsi)
-    646c998b:	xor    %ebp,(%rsi)
-    646c998d:	xor    %al,(%rax)
-	...
-
-00000000646c9990 <.rdata$zzz>:
-    646c9990:	rex.RXB
-    646c9991:	rex.XB
-    646c9992:	rex.XB cmp (%r8),%spl
-    646c9995:	sub    %bh,0x38(%rax)
-    646c9998:	ss pop %rdi
-    646c999a:	ss xor $0x2d,%al
-    646c999d:	ja     646c9a08 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x38>
-    646c999f:	outsb  %ds:(%rsi),(%dx)
-    646c99a0:	xor    (%rdx),%esi
-    646c99a2:	sub    $0x2d686573,%eax
-    646c99a7:	jb     646c9a0e <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3e>
-    646c99a9:	jbe    646c99db <__RUNTIME_PSEUDO_RELOC_LIST_END__+0xb>
-    646c99ab:	sub    $0x20,%al
-    646c99ad:	rex.X jne 646c9a19 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x49>
-    646c99b0:	insb   (%dx),%es:(%rdi)
-    646c99b1:	je     646c99d3 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3>
-    646c99b3:	(bad)
-    646c99b4:	jns    646c99d6 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x6>
-    646c99b6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c99be:	xor    $0x20,%al
-    646c99c0:	jo     646c9a34 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x64>
-    646c99c2:	outsl  %ds:(%rsi),(%dx)
-    646c99c3:	push   $0x65
-    646c99c5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c99c9:	cmp    %ch,(%rsi)
-    646c99cb:	xor    %ebp,(%rsi)
-    646c99cd:	xor    %al,(%rax)
+00000000646c9790 <.refptr.__xi_z>:
+    646c9790:	and    %dh,%al
+    646c9792:	insb   (%dx),%es:(%rdi)
+    646c9793:	add    %al,%fs:(%rax)
+	...
+
+00000000646c97a0 <.refptr.mingw_app_type>:
+    646c97a0:	rol    %bh
+    646c97a2:	insb   (%dx),%es:(%rdi)
+    646c97a3:	add    %al,%fs:(%rax)
+	...
+
+00000000646c97b0 <.rdata$zzz>:
+    646c97b0:	rex.RXB
+    646c97b1:	rex.XB
+    646c97b2:	rex.XB cmp (%r8),%spl
+    646c97b5:	sub    %bh,0x38(%rax)
+    646c97b8:	ss pop %rdi
+    646c97ba:	ss xor $0x2d,%al
+    646c97bd:	ja     646c9828 <.rdata$zzz+0x38>
+    646c97bf:	outsb  %ds:(%rsi),(%dx)
+    646c97c0:	xor    (%rdx),%esi
+    646c97c2:	sub    $0x2d686573,%eax
+    646c97c7:	jb     646c982e <.rdata$zzz+0x3e>
+    646c97c9:	jbe    646c97fb <.rdata$zzz+0xb>
+    646c97cb:	sub    $0x20,%al
+    646c97cd:	rex.X jne 646c9839 <.rdata$zzz+0x9>
+    646c97d0:	insb   (%dx),%es:(%rdi)
+    646c97d1:	je     646c97f3 <.rdata$zzz+0x3>
+    646c97d3:	(bad)
+    646c97d4:	jns    646c97f6 <.rdata$zzz+0x6>
+    646c97d6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c97de:	xor    $0x20,%al
+    646c97e0:	jo     646c9854 <.rdata$zzz+0x24>
+    646c97e2:	outsl  %ds:(%rsi),(%dx)
+    646c97e3:	push   $0x65
+    646c97e5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c97e9:	cmp    %ch,(%rsi)
+    646c97eb:	xor    %ebp,(%rsi)
+    646c97ed:	xor    %al,(%rax)
+	...
+
+00000000646c97f0 <.rdata$zzz>:
+    646c97f0:	rex.RXB
+    646c97f1:	rex.XB
+    646c97f2:	rex.XB cmp (%r8),%spl
+    646c97f5:	sub    %bh,0x38(%rax)
+    646c97f8:	ss pop %rdi
+    646c97fa:	ss xor $0x2d,%al
+    646c97fd:	ja     646c9868 <.rdata$zzz+0x38>
+    646c97ff:	outsb  %ds:(%rsi),(%dx)
+    646c9800:	xor    (%rdx),%esi
+    646c9802:	sub    $0x2d686573,%eax
+    646c9807:	jb     646c986e <.rdata$zzz+0x3e>
+    646c9809:	jbe    646c983b <.rdata$zzz+0xb>
+    646c980b:	sub    $0x20,%al
+    646c980d:	rex.X jne 646c9879 <.rdata$zzz+0x9>
+    646c9810:	insb   (%dx),%es:(%rdi)
+    646c9811:	je     646c9833 <.rdata$zzz+0x3>
+    646c9813:	(bad)
+    646c9814:	jns    646c9836 <.rdata$zzz+0x6>
+    646c9816:	imul   $0x36572d57,0x47(%r14),%r13
+    646c981e:	xor    $0x20,%al
+    646c9820:	jo     646c9894 <.rdata$zzz+0x24>
+    646c9822:	outsl  %ds:(%rsi),(%dx)
+    646c9823:	push   $0x65
+    646c9825:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9829:	cmp    %ch,(%rsi)
+    646c982b:	xor    %ebp,(%rsi)
+    646c982d:	xor    %al,(%rax)
+	...
+
+00000000646c9830 <.rdata$zzz>:
+    646c9830:	rex.RXB
+    646c9831:	rex.XB
+    646c9832:	rex.XB cmp (%r8),%spl
+    646c9835:	sub    %bh,0x38(%rax)
+    646c9838:	ss pop %rdi
+    646c983a:	ss xor $0x2d,%al
+    646c983d:	ja     646c98a8 <.rdata$zzz+0x38>
+    646c983f:	outsb  %ds:(%rsi),(%dx)
+    646c9840:	xor    (%rdx),%esi
+    646c9842:	sub    $0x2d686573,%eax
+    646c9847:	jb     646c98ae <.rdata$zzz+0x3e>
+    646c9849:	jbe    646c987b <.rdata$zzz+0xb>
+    646c984b:	sub    $0x20,%al
+    646c984d:	rex.X jne 646c98b9 <.rdata$zzz+0x9>
+    646c9850:	insb   (%dx),%es:(%rdi)
+    646c9851:	je     646c9873 <.rdata$zzz+0x3>
+    646c9853:	(bad)
+    646c9854:	jns    646c9876 <.rdata$zzz+0x6>
+    646c9856:	imul   $0x36572d57,0x47(%r14),%r13
+    646c985e:	xor    $0x20,%al
+    646c9860:	jo     646c98d4 <.rdata$zzz+0x24>
+    646c9862:	outsl  %ds:(%rsi),(%dx)
+    646c9863:	push   $0x65
+    646c9865:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9869:	cmp    %ch,(%rsi)
+    646c986b:	xor    %ebp,(%rsi)
+    646c986d:	xor    %al,(%rax)
+	...
+
+00000000646c9870 <.rdata$zzz>:
+    646c9870:	rex.RXB
+    646c9871:	rex.XB
+    646c9872:	rex.XB cmp (%r8),%spl
+    646c9875:	sub    %bh,0x38(%rax)
+    646c9878:	ss pop %rdi
+    646c987a:	ss xor $0x2d,%al
+    646c987d:	ja     646c98e8 <.rdata$zzz+0x38>
+    646c987f:	outsb  %ds:(%rsi),(%dx)
+    646c9880:	xor    (%rdx),%esi
+    646c9882:	sub    $0x2d686573,%eax
+    646c9887:	jb     646c98ee <.rdata$zzz+0x3e>
+    646c9889:	jbe    646c98bb <.rdata$zzz+0xb>
+    646c988b:	sub    $0x20,%al
+    646c988d:	rex.X jne 646c98f9 <.rdata$zzz+0x9>
+    646c9890:	insb   (%dx),%es:(%rdi)
+    646c9891:	je     646c98b3 <.rdata$zzz+0x3>
+    646c9893:	(bad)
+    646c9894:	jns    646c98b6 <.rdata$zzz+0x6>
+    646c9896:	imul   $0x36572d57,0x47(%r14),%r13
+    646c989e:	xor    $0x20,%al
+    646c98a0:	jo     646c9914 <.rdata$zzz+0x24>
+    646c98a2:	outsl  %ds:(%rsi),(%dx)
+    646c98a3:	push   $0x65
+    646c98a5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c98a9:	cmp    %ch,(%rsi)
+    646c98ab:	xor    %ebp,(%rsi)
+    646c98ad:	xor    %al,(%rax)
+	...
+
+00000000646c98b0 <.rdata$zzz>:
+    646c98b0:	rex.RXB
+    646c98b1:	rex.XB
+    646c98b2:	rex.XB cmp (%r8),%spl
+    646c98b5:	sub    %bh,0x38(%rax)
+    646c98b8:	ss pop %rdi
+    646c98ba:	ss xor $0x2d,%al
+    646c98bd:	ja     646c9928 <.rdata$zzz+0x38>
+    646c98bf:	outsb  %ds:(%rsi),(%dx)
+    646c98c0:	xor    (%rdx),%esi
+    646c98c2:	sub    $0x2d686573,%eax
+    646c98c7:	jb     646c992e <.rdata$zzz+0x3e>
+    646c98c9:	jbe    646c98fb <.rdata$zzz+0xb>
+    646c98cb:	sub    $0x20,%al
+    646c98cd:	rex.X jne 646c9939 <.rdata$zzz+0x9>
+    646c98d0:	insb   (%dx),%es:(%rdi)
+    646c98d1:	je     646c98f3 <.rdata$zzz+0x3>
+    646c98d3:	(bad)
+    646c98d4:	jns    646c98f6 <.rdata$zzz+0x6>
+    646c98d6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c98de:	xor    $0x20,%al
+    646c98e0:	jo     646c9954 <.rdata$zzz+0x24>
+    646c98e2:	outsl  %ds:(%rsi),(%dx)
+    646c98e3:	push   $0x65
+    646c98e5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c98e9:	cmp    %ch,(%rsi)
+    646c98eb:	xor    %ebp,(%rsi)
+    646c98ed:	xor    %al,(%rax)
+	...
+
+00000000646c98f0 <.rdata$zzz>:
+    646c98f0:	rex.RXB
+    646c98f1:	rex.XB
+    646c98f2:	rex.XB cmp (%r8),%spl
+    646c98f5:	sub    %bh,0x38(%rax)
+    646c98f8:	ss pop %rdi
+    646c98fa:	ss xor $0x2d,%al
+    646c98fd:	ja     646c9968 <.rdata$zzz+0x38>
+    646c98ff:	outsb  %ds:(%rsi),(%dx)
+    646c9900:	xor    (%rdx),%esi
+    646c9902:	sub    $0x2d686573,%eax
+    646c9907:	jb     646c996e <.rdata$zzz+0x3e>
+    646c9909:	jbe    646c993b <.rdata$zzz+0xb>
+    646c990b:	sub    $0x20,%al
+    646c990d:	rex.X jne 646c9979 <.rdata$zzz+0x9>
+    646c9910:	insb   (%dx),%es:(%rdi)
+    646c9911:	je     646c9933 <.rdata$zzz+0x3>
+    646c9913:	(bad)
+    646c9914:	jns    646c9936 <.rdata$zzz+0x6>
+    646c9916:	imul   $0x36572d57,0x47(%r14),%r13
+    646c991e:	xor    $0x20,%al
+    646c9920:	jo     646c9994 <.rdata$zzz+0x24>
+    646c9922:	outsl  %ds:(%rsi),(%dx)
+    646c9923:	push   $0x65
+    646c9925:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9929:	cmp    %ch,(%rsi)
+    646c992b:	xor    %ebp,(%rsi)
+    646c992d:	xor    %al,(%rax)
+	...
+
+00000000646c9930 <.rdata$zzz>:
+    646c9930:	rex.RXB
+    646c9931:	rex.XB
+    646c9932:	rex.XB cmp (%r8),%spl
+    646c9935:	sub    %bh,0x38(%rax)
+    646c9938:	ss pop %rdi
+    646c993a:	ss xor $0x2d,%al
+    646c993d:	ja     646c99a8 <.rdata$zzz+0x38>
+    646c993f:	outsb  %ds:(%rsi),(%dx)
+    646c9940:	xor    (%rdx),%esi
+    646c9942:	sub    $0x2d686573,%eax
+    646c9947:	jb     646c99ae <.rdata$zzz+0x3e>
+    646c9949:	jbe    646c997b <.rdata$zzz+0xb>
+    646c994b:	sub    $0x20,%al
+    646c994d:	rex.X jne 646c99b9 <.rdata$zzz+0x9>
+    646c9950:	insb   (%dx),%es:(%rdi)
+    646c9951:	je     646c9973 <.rdata$zzz+0x3>
+    646c9953:	(bad)
+    646c9954:	jns    646c9976 <.rdata$zzz+0x6>
+    646c9956:	imul   $0x36572d57,0x47(%r14),%r13
+    646c995e:	xor    $0x20,%al
+    646c9960:	jo     646c99d4 <.rdata$zzz+0x24>
+    646c9962:	outsl  %ds:(%rsi),(%dx)
+    646c9963:	push   $0x65
+    646c9965:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9969:	cmp    %ch,(%rsi)
+    646c996b:	xor    %ebp,(%rsi)
+    646c996d:	xor    %al,(%rax)
+	...
+
+00000000646c9970 <.rdata$zzz>:
+    646c9970:	rex.RXB
+    646c9971:	rex.XB
+    646c9972:	rex.XB cmp (%r8),%spl
+    646c9975:	sub    %bh,0x38(%rax)
+    646c9978:	ss pop %rdi
+    646c997a:	ss xor $0x2d,%al
+    646c997d:	ja     646c99e8 <.rdata$zzz+0x38>
+    646c997f:	outsb  %ds:(%rsi),(%dx)
+    646c9980:	xor    (%rdx),%esi
+    646c9982:	sub    $0x2d686573,%eax
+    646c9987:	jb     646c99ee <.rdata$zzz+0x3e>
+    646c9989:	jbe    646c99bb <.rdata$zzz+0xb>
+    646c998b:	sub    $0x20,%al
+    646c998d:	rex.X jne 646c99f9 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x9>
+    646c9990:	insb   (%dx),%es:(%rdi)
+    646c9991:	je     646c99b3 <.rdata$zzz+0x3>
+    646c9993:	(bad)
+    646c9994:	jns    646c99b6 <.rdata$zzz+0x6>
+    646c9996:	imul   $0x36572d57,0x47(%r14),%r13
+    646c999e:	xor    $0x20,%al
+    646c99a0:	jo     646c9a14 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x24>
+    646c99a2:	outsl  %ds:(%rsi),(%dx)
+    646c99a3:	push   $0x65
+    646c99a5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c99a9:	cmp    %ch,(%rsi)
+    646c99ab:	xor    %ebp,(%rsi)
+    646c99ad:	xor    %al,(%rax)
+	...
+
+00000000646c99b0 <.rdata$zzz>:
+    646c99b0:	rex.RXB
+    646c99b1:	rex.XB
+    646c99b2:	rex.XB cmp (%r8),%spl
+    646c99b5:	sub    %bh,0x38(%rax)
+    646c99b8:	ss pop %rdi
+    646c99ba:	ss xor $0x2d,%al
+    646c99bd:	ja     646c9a28 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x38>
+    646c99bf:	outsb  %ds:(%rsi),(%dx)
+    646c99c0:	xor    (%rdx),%esi
+    646c99c2:	sub    $0x2d686573,%eax
+    646c99c7:	jb     646c9a2e <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3e>
+    646c99c9:	jbe    646c99fb <__RUNTIME_PSEUDO_RELOC_LIST_END__+0xb>
+    646c99cb:	sub    $0x20,%al
+    646c99cd:	rex.X jne 646c9a39 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x49>
+    646c99d0:	insb   (%dx),%es:(%rdi)
+    646c99d1:	je     646c99f3 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3>
+    646c99d3:	(bad)
+    646c99d4:	jns    646c99f6 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x6>
+    646c99d6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c99de:	xor    $0x20,%al
+    646c99e0:	jo     646c9a54 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x64>
+    646c99e2:	outsl  %ds:(%rsi),(%dx)
+    646c99e3:	push   $0x65
+    646c99e5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c99e9:	cmp    %ch,(%rsi)
+    646c99eb:	xor    %ebp,(%rsi)
+    646c99ed:	xor    %al,(%rax)
 	...
 
 Disassembly of section .pdata:
 
 00000000646ca000 <.pdata>:
     646ca000:	add    %dl,(%rax)
     646ca002:	add    %al,(%rax)
@@ -11822,427 +11806,455 @@
     646ca1fd:	xor    $0x0,%al
     646ca1ff:	add    %bh,(%rax)
     646ca201:	mov    $0x0,%cl
 	...
 
 00000000646ca204 <.pdata>:
     646ca204:	and    %dh,(%rax,%rax,1)
-    646ca207:	add    %cl,0x34(%rbx)
+    646ca207:	add    %bl,0x34(%rcx)
     646ca20a:	add    %al,(%rax)
     646ca20c:	rex.W mov $0x0,%cl
-    646ca20f:	add    %dl,0x34(%rax)
+    646ca20f:	add    %ah,0x34(%rax)
     646ca212:	add    %al,(%rax)
-    646ca214:	add    $0x35,%al
+    646ca214:	adc    $0x35,%al
     646ca216:	add    %al,(%rax)
     646ca218:	rex.WR mov $0x0,%cl
-    646ca21b:	add    %dl,(%rax)
-    646ca21d:	xor    $0x360d0000,%eax
+    646ca21b:	add    %ah,(%rax)
+    646ca21d:	xor    $0x361d0000,%eax
     646ca222:	add    %al,(%rax)
-    646ca224:	push   $0x100000b1
+    646ca224:	push   $0x200000b1
 
 00000000646ca228 <.pdata>:
-    646ca228:	adc    %dh,(%rsi)
+    646ca228:	and    %dh,(%rsi)
     646ca22a:	add    %al,(%rax)
-    646ca22c:	ja     646ca264 <.pdata+0x3c>
+    646ca22c:	xchg   %esi,(%rsi)
     646ca22e:	add    %al,(%rax)
-    646ca230:	mov    %?,0x36800000(%rcx)
+    646ca230:	mov    %?,0x36900000(%rcx)
     646ca236:	add    %al,(%rax)
-    646ca238:	mov    (%rsi),%dh
-    646ca23a:	add    %al,(%rax)
+    646ca238:	(bad)
+    646ca239:	ss add %al,(%rax)
     646ca23c:	pushf
     646ca23d:	mov    $0x0,%cl
-    646ca23f:	add    %dl,0x44000036(%rax)
+    646ca23f:	add    %ah,0x6b000036(%rax)
     646ca245:	cmp    %al,(%rax)
-    646ca247:	add    %ah,0x500000b1(%rax)
+    646ca247:	add    %ah,0x700000b1(%rax)
     646ca24d:	cmp    %al,(%rax)
-    646ca24f:	add    %al,(%rbx,%rdi,1)
+    646ca24f:	add    %ah,(%rbx,%rdi,1)
     646ca252:	add    %al,(%rax)
-    646ca254:	mov    $0xb1,%al
+    646ca254:	mov    $0xb1,%ah
     646ca256:	add    %al,(%rax)
-    646ca258:	adc    %bh,(%rbx)
+    646ca258:	xor    %bh,(%rbx)
     646ca25a:	add    %al,(%rax)
-    646ca25c:	jl     646ca29c <.pdata+0x20>
-    646ca25e:	add    %al,(%rax)
-    646ca260:	(bad)
-    646ca261:	mov    $0x0,%cl
-    646ca263:	add    %al,-0x18ffffc2(%rax)
-    646ca269:	(bad)
-    646ca26a:	add    %al,(%rax)
-    646ca26c:	fdivs  0x3ff00000(%rcx)
-    646ca272:	add    %al,(%rax)
-    646ca274:	lock rex add %al,(%rax)
-    646ca278:	call   546ca32e <__size_of_stack_reserve__+0x544ca32e>
+    646ca25c:	pushf
+    646ca25d:	ds add %al,(%rax)
+    646ca260:	enter  $0xb1,$0x0
+    646ca264:	movabs 0xdc0000400700003e,%al
+    646ca26d:	mov    $0x0,%cl
+    646ca26f:	add    %dl,(%rax)
+    646ca271:	rex add %al,(%rax)
+    646ca274:	add    %al,0x0(%rcx)
+    646ca277:	add    %ch,%ah
+    646ca279:	mov    $0x0,%cl
+	...
 
 00000000646ca27c <.pdata>:
-    646ca27c:	lock rex add %al,(%rax)
-    646ca280:	adc    0x0(%rcx),%al
-    646ca283:	add    %dh,%ah
+    646ca27c:	add    %al,0x0(%rcx)
+    646ca27f:	add    %ah,(%rdx)
+    646ca281:	add    %al,(%r8)
+    646ca284:	clc
     646ca285:	mov    $0x0,%cl
-    646ca287:	add    %ah,(%rax)
+    646ca287:	add    %dh,(%rax)
     646ca289:	add    %al,(%r8)
-    646ca28c:	test   $0xfc000043,%eax
-    646ca291:	mov    $0x0,%cl
-    646ca293:	add    %dh,-0x5fffffbd(%rax)
-    646ca299:	rex.RXB add %r8b,(%r8)
-    646ca29c:	adc    %dh,0x47a00000(%rdx)
-    646ca2a2:	add    %al,(%rax)
-    646ca2a4:	and    $0x48,%al
-    646ca2a6:	add    %al,(%rax)
-    646ca2a8:	sub    %dh,0x48300000(%rdx)
-    646ca2ae:	add    %al,(%rax)
-    646ca2b0:	add    %cl,0x0(%rcx)
-    646ca2b3:	add    %dh,(%rax)
-    646ca2b5:	mov    $0x0,%dl
-    646ca2b7:	add    %al,(%rax)
-    646ca2b9:	rex.WB add %al,(%r8)
-    646ca2bc:	rex.RB
-    646ca2bd:	rex.WX add %al,(%rax)
-    646ca2c0:	cmp    %dh,0x4a500000(%rdx)
+    646ca28c:	mov    $0x43,%ecx
+    646ca291:	mov    $0x0,%dl
+    646ca293:	add    %al,%al
+    646ca295:	rex.XB add %al,(%r8)
+    646ca298:	and    0x0(%rsi),%eax
+    646ca29b:	add    %dl,(%rdx,%rsi,4)
+    646ca29e:	add    %al,(%rax)
+    646ca2a0:	xor    %al,0x0(%rsi)
+    646ca2a3:	add    %dh,-0x4dd40000(%rsi,%rax,2)
+    646ca2aa:	add    %al,(%rax)
+    646ca2ac:	rolb   $0x0,0x0(%rsi)
+    646ca2b0:	nop
+    646ca2b1:	rex.RXB add %r8b,(%r8)
+    646ca2b4:	xor    $0xb2,%al
+    646ca2b6:	add    %al,(%rax)
+    646ca2b8:	nop
+    646ca2b9:	rex.RXB add %r8b,(%r8)
+    646ca2bc:	(bad)
+    646ca2bd:	rex.W add %al,(%rax)
+    646ca2c0:	cmp    $0xb2,%al
+    646ca2c2:	add    %al,(%rax)
+    646ca2c4:	loopne 646ca30e <.pdata+0x2>
     646ca2c6:	add    %al,(%rax)
-    646ca2c8:	cmp    0x0(%rbx),%cl
-    646ca2cb:	add    %dl,-0x4e(%rax)
-    646ca2ce:	add    %al,(%rax)
-    646ca2d0:	rex
-    646ca2d1:	rex.WXB add %al,(%r8)
-    646ca2d4:	mov    $0x6400004c,%ebx
-    646ca2d9:	mov    $0x0,%dl
-	...
+    646ca2c8:	lret   $0x49
+    646ca2cb:	add    %dl,0x0(%rdx,%rsi,4)
+    646ca2cf:	add    %dl,%al
+    646ca2d1:	rex.WB add %al,(%r8)
+    646ca2d4:	rex.WXB
+    646ca2d5:	rex.WXB add %al,(%r8)
+    646ca2d8:	push   $0x500000b2
 
 00000000646ca2dc <.pdata>:
-    646ca2dc:	rorb   $0x5,0x0(%rax,%rax,1)
-    646ca2e1:	rex.WRB add %r8b,(%r8)
-    646ca2e4:	js     646ca298 <.pdata+0x1c>
+    646ca2dc:	push   %rax
+    646ca2dd:	rex.WXB add %al,(%r8)
+    646ca2e0:	xchg   %eax,%ebp
+    646ca2e1:	rex.WXB add %al,(%r8)
+    646ca2e4:	jl     646ca298 <.pdata+0x1c>
 	...
 
 00000000646ca2e8 <.pdata>:
-    646ca2e8:	adc    %cl,0x0(%rbp)
-    646ca2eb:	add    %ch,0x4d(%rdx)
-    646ca2ee:	add    %al,(%rax)
-    646ca2f0:	test   %dh,0x4d700000(%rdx)
+    646ca2e8:	movabs 0x8800004c3b00004b,%al
+    646ca2f1:	mov    $0x0,%dl
+    646ca2f3:	add    %al,0x4c(%rax)
     646ca2f6:	add    %al,(%rax)
-    646ca2f8:	(bad)
-    646ca2f9:	push   %rax
-    646ca2fa:	add    %al,(%rax)
-    646ca2fc:	mov    %?,0x50e00000(%rdx)
+    646ca2f8:	sbb    $0x94000050,%eax
+    646ca2fd:	mov    $0x0,%dl
+    646ca2ff:	add    %ah,(%rax)
+    646ca301:	push   %rax
     646ca302:	add    %al,(%rax)
-    646ca304:	jmp    86ca359 <__size_of_stack_reserve__+0x84ca359>
-    646ca309:	mov    $0x0,%dl
-	...
+    646ca304:	sub    %edx,0x0(%rax)
+    646ca307:	add    %ch,0x50300000(%rdx,%rsi,4)
 
 00000000646ca30c <.pdata>:
-    646ca30c:	lock push %rax
-    646ca30e:	add    %al,(%rax)
-    646ca310:	or     0x0(%rcx),%edx
-    646ca313:	add    %ch,0x100000b2(%rax)
-    646ca319:	push   %rcx
+    646ca30c:	xor    %dl,0x0(%rax)
+    646ca30f:	add    %cl,0x50(%rbx)
+    646ca312:	add    %al,(%rax)
+    646ca314:	mov    $0xb2,%al
+    646ca316:	add    %al,(%rax)
+    646ca318:	push   %rax
+    646ca319:	push   %rax
     646ca31a:	add    %al,(%rax)
-    646ca31c:	jno    646ca36f <.pdata+0x1b>
+    646ca31c:	mov    $0x50,%cl
     646ca31e:	add    %al,(%rax)
-    646ca320:	lods   %ds:(%rsi),%al
-    646ca321:	mov    $0x0,%dl
-    646ca323:	add    %al,0x17000051(%rax)
-    646ca329:	push   %rdx
+    646ca320:	mov    $0xb2,%ah
+    646ca322:	add    %al,(%rax)
+    646ca324:	rclb   $0x0,0x0(%rax)
+    646ca328:	push   %rdi
+    646ca329:	push   %rcx
     646ca32a:	add    %al,(%rax)
-    646ca32c:	mov    $0xb2,%al
-    646ca32e:	add    %al,(%rax)
-    646ca330:	and    %dl,0x0(%rdx)
-    646ca333:	add    %dl,%bh
+    646ca32c:	mov    $0x600000b2,%eax
+    646ca331:	push   %rcx
+    646ca332:	add    %al,(%rax)
+    646ca334:	(bad)
     646ca335:	push   %rdx
     646ca336:	add    %al,(%rax)
-    646ca338:	shlb   $0x0,0x52e00000(%rdx)
+    646ca338:	enter  $0xb2,$0x0
 
 00000000646ca33c <.pdata>:
-    646ca33c:	loopne 646ca390 <.pdata>
-    646ca33e:	add    %al,(%rax)
-    646ca340:	mov    $0x54,%bl
+    646ca33c:	and    %dl,0x0(%rdx)
+    646ca33f:	add    %dh,%bl
+    646ca341:	push   %rbx
     646ca342:	add    %al,(%rax)
-    646ca344:	shlb   0x54c00000(%rdx)
+    646ca344:	fdivs  0x54000000(%rdx)
     646ca34a:	add    %al,(%rax)
-    646ca34c:	enter  $0x55,$0x0
-    646ca350:	lock mov $0x0,%dl
+    646ca34c:	or     %dl,0x0(%rbp)
+    646ca34f:	add    %bh,%al
+    646ca351:	mov    $0x0,%dl
 	...
 
 00000000646ca354 <.pdata>:
-    646ca354:	loopne 646ca3ab <.pdata+0x1b>
-    646ca356:	add    %al,(%rax)
-    646ca358:	adc    $0xf4000056,%eax
+    646ca354:	and    %dl,0x0(%rbp)
+    646ca357:	add    %dl,0x55(%rbp)
+    646ca35a:	add    %al,(%rax)
+    646ca35c:	cld
     646ca35d:	mov    $0x0,%dl
-    646ca35f:	add    %ah,(%rax)
-    646ca361:	push   %rsi
+    646ca35f:	add    %ah,0x55(%rax)
     646ca362:	add    %al,(%rax)
-    646ca364:	xchg   %dl,0x0(%rsi)
-    646ca367:	add    %bh,%ah
-    646ca369:	mov    $0x0,%dl
-    646ca36b:	add    %dl,-0x50ffffaa(%rax)
-    646ca371:	push   %rsi
+    646ca364:	(bad)
+    646ca365:	push   %rbp
+    646ca366:	add    %al,(%rax)
+    646ca368:	add    $0xb3,%al
+    646ca36a:	add    %al,(%rax)
+    646ca36c:	rclb   0x0(%rbp)
+    646ca36f:	add    %ch,%bh
+    646ca371:	push   %rbp
     646ca372:	add    %al,(%rax)
-    646ca374:	or     %dh,0x56b00000(%rbx)
+    646ca374:	adc    %dh,0x55f00000(%rbx)
 
 00000000646ca378 <.pdata>:
-    646ca378:	mov    $0x56,%al
+    646ca378:	lock push %rbp
     646ca37a:	add    %al,(%rax)
-    646ca37c:	xchg   %dl,0x0(%rdi)
-    646ca37f:	add    %cl,(%rbx,%rsi,4)
+    646ca37c:	(bad)
+    646ca37d:	push   %rsi
+    646ca37e:	add    %al,(%rax)
+    646ca380:	adc    $0xb3,%al
     646ca382:	add    %al,(%rax)
-    646ca384:	nop
-    646ca385:	push   %rdi
-    646ca386:	add    %al,(%rax)
-    646ca388:	mov    %bl,0x0(%rax)
-    646ca38b:	add    %bl,(%rbx,%rsi,4)
+    646ca384:	rclb   0x0(%rsi)
+    646ca387:	add    %cl,%al
+    646ca389:	push   %rdi
+    646ca38a:	add    %al,(%rax)
+    646ca38c:	and    $0xb3,%al
 	...
 
 00000000646ca390 <.pdata>:
-    646ca390:	nop
-    646ca391:	pop    %rax
-    646ca392:	add    %al,(%rax)
-    646ca394:	mov    $0x2c000058,%edi
-    646ca399:	mov    $0x0,%bl
-    646ca39b:	add    %al,%al
-    646ca39d:	pop    %rax
-    646ca39e:	add    %al,(%rax)
-    646ca3a0:	xor    0x0(%rcx),%ebx
-    646ca3a3:	add    %dh,(%rbx,%rsi,4)
+    646ca390:	rclb   0x0(%rdi)
+    646ca393:	add    %bh,%bh
+    646ca395:	push   %rdi
+    646ca396:	add    %al,(%rax)
+    646ca398:	xor    $0xb3,%al
+    646ca39a:	add    %al,(%rax)
+    646ca39c:	add    %bl,0x0(%rax)
+    646ca39f:	add    %dh,0x58(%rbx)
+    646ca3a2:	add    %al,(%rax)
+    646ca3a4:	cmp    $0xb3,%al
     646ca3a6:	add    %al,(%rax)
-    646ca3a8:	rex pop %rcx
-    646ca3aa:	add    %al,(%rax)
-    646ca3ac:	rex.XB pop %r9
-    646ca3ae:	add    %al,(%rax)
-    646ca3b0:	rex mov $0x0,%bl
+    646ca3a8:	sbbb   $0x0,0x0(%rax)
+    646ca3ac:	sbbl   $0x0,0x0(%rax)
+    646ca3b0:	rex.W mov $0x0,%bl
 	...
 
 00000000646ca3b4 <.pdata>:
-    646ca3b4:	push   %rax
-    646ca3b5:	pop    %rcx
+    646ca3b4:	nop
+    646ca3b5:	pop    %rax
     646ca3b6:	add    %al,(%rax)
-    646ca3b8:	push   %rsp
-    646ca3b9:	pop    %rcx
+    646ca3b8:	xchg   %eax,%esp
+    646ca3b9:	pop    %rax
     646ca3ba:	add    %al,(%rax)
-    646ca3bc:	rex.R mov $0x0,%bl
-    646ca3bf:	add    %ah,0x59(%rax)
-    646ca3c2:	add    %al,(%rax)
-    646ca3c4:	fs pop %rcx
+    646ca3bc:	rex.WR mov $0x0,%bl
+    646ca3bf:	add    %ah,-0x5bffffa8(%rax)
+    646ca3c5:	pop    %rax
     646ca3c6:	add    %al,(%rax)
-    646ca3c8:	rex.W mov $0x0,%bl
+    646ca3c8:	push   %rax
+    646ca3c9:	mov    $0x0,%bl
 	...
 
 00000000646ca3cc <.pdata.unlikely>:
-    646ca3cc:	jo     646ca427 <.pdata+0x13>
+    646ca3cc:	mov    $0x58,%al
     646ca3ce:	add    %al,(%rax)
-    646ca3d0:	cmp    $0x5800005b,%eax
+    646ca3d0:	jge    646ca42c <.pdata+0x18>
+    646ca3d2:	add    %al,(%rax)
+    646ca3d4:	(bad)
     646ca3d5:	mov    $0x0,%bl
 	...
 
 00000000646ca3d8 <.pdata>:
-    646ca3d8:	rex pop %rbx
-    646ca3da:	add    %al,(%rax)
-    646ca3dc:	sti
-    646ca3dd:	pop    %rbp
-    646ca3de:	add    %al,(%rax)
-    646ca3e0:	push   $0xb3
-    646ca3e5:	pop    %rsi
+    646ca3d8:	sbbb   $0x0,0x0(%rdx)
+    646ca3dc:	cmp    0x0(%rbp),%ebx
+    646ca3df:	add    %dh,-0x4d(%rax)
+    646ca3e2:	add    %al,(%rax)
+    646ca3e4:	rex pop %rbp
     646ca3e6:	add    %al,(%rax)
-    646ca3e8:	movabs 0xa00000b38000005f,%al
+    646ca3e8:	loopne 646ca448 <.pdata+0x4>
+    646ca3ea:	add    %al,(%rax)
+    646ca3ec:	mov    %dh,0x5ee00000(%rbx)
 
 00000000646ca3f0 <.pdata>:
-    646ca3f0:	movabs 0x880000608c00005f,%al
+    646ca3f0:	loopne 646ca450 <.pdata+0xc>
+    646ca3f2:	add    %al,(%rax)
+    646ca3f4:	int3
+    646ca3f5:	pop    %rdi
+    646ca3f6:	add    %al,(%rax)
+    646ca3f8:	nop
     646ca3f9:	mov    $0x0,%bl
-    646ca3fb:	add    %dl,0x77000060(%rax)
-    646ca401:	(bad)
+    646ca3fb:	add    %dl,%al
+    646ca3fd:	pop    %rdi
+    646ca3fe:	add    %al,(%rax)
+    646ca400:	mov    $0x61,%bh
     646ca402:	add    %al,(%rax)
-    646ca404:	cwtl
-    646ca405:	mov    $0x0,%bl
-    646ca407:	add    %al,-0x15ffff9e(%rax)
+    646ca404:	movabs 0x2a000061c00000b3,%al
     646ca40d:	(bad)
     646ca40e:	add    %al,(%rax)
-    646ca410:	movabs 0x6f000062f00000b3,%al
+    646ca410:	test   $0xb3,%al
+	...
 
 00000000646ca414 <.pdata>:
-    646ca414:	lock (bad)
-    646ca416:	add    %al,(%rax)
-    646ca418:	outsl  %ds:(%rsi),(%dx)
-    646ca419:	movsxd (%rax),%eax
-    646ca41b:	add    %dh,0x700000b3(%rax)
-    646ca421:	movsxd (%rax),%eax
-    646ca423:	add    %dl,(%rax)
-    646ca425:	add    %al,%fs:(%rax)
-    646ca428:	shlb   $0x0,0x64100000(%rbx)
-    646ca42f:	add    %ch,%dl
-    646ca431:	add    %al,%fs:(%rax)
-    646ca434:	enter  $0xb3,$0x0
-    646ca438:	lock add %al,%fs:(%rax)
-    646ca43c:	(bad)
-    646ca43d:	add    %al,%gs:(%rax)
-    646ca440:	shlb   0x65100000(%rbx)
+    646ca414:	xor    %ah,0x0(%rdx)
+    646ca417:	add    %ch,-0x47ffff9e(%rdi)
+    646ca41d:	mov    $0x0,%bl
+    646ca41f:	add    %dh,0x50000062(%rax)
+    646ca425:	movsxd (%rax),%eax
+    646ca427:	add    %cl,%al
+    646ca429:	mov    $0x0,%bl
+    646ca42b:	add    %dl,0x63(%rax)
+    646ca42e:	add    %al,(%rax)
+    646ca430:	sub    0x0(%rax,%rax,1),%ah
+    646ca434:	shlb   0x64300000(%rbx)
+    646ca43a:	add    %al,(%rax)
+    646ca43c:	rex.WRX
+    646ca43d:	add    %al,%fs:(%rax)
+    646ca440:	fdivs  0x64500000(%rbx)
 
 00000000646ca444 <.pdata>:
-    646ca444:	adc    %ah,0x0(%rbp)
-    646ca447:	add    %ah,(%rdx)
-    646ca449:	add    %al,%gs:(%rax)
-    646ca44c:	(bad)
-    646ca44d:	mov    $0x0,%bl
-    646ca44f:	add    %dh,(%rax)
-    646ca451:	add    %al,%gs:(%rax)
-    646ca454:	je     646ca4bb <.pdata+0x77>
+    646ca444:	push   %rax
+    646ca445:	add    %al,%fs:(%rax)
+    646ca448:	(bad)
+    646ca449:	add    %al,%fs:(%rax)
+    646ca44c:	fdivl  0x64700000(%rbx)
+    646ca452:	add    %al,(%rax)
+    646ca454:	mov    $0x64,%ah
     646ca456:	add    %al,(%rax)
-    646ca458:	fdivs  0x65800000(%rbx)
-    646ca45e:	add    %al,(%rax)
-    646ca460:	or     $0xdc000066,%eax
-    646ca465:	mov    $0x0,%bl
-    646ca467:	add    %dl,(%rax)
-    646ca469:	data16 add %al,(%rax)
-    646ca46c:	test   %ah,0x0(%rsi)
-    646ca46f:	add    %ch,%al
-    646ca471:	mov    $0x0,%bl
-    646ca473:	add    %dl,-0x31ffff9a(%rax)
+    646ca458:	loopne 646ca40d <.pdata+0x1d>
+    646ca45a:	add    %al,(%rax)
+    646ca45c:	shlb   $0x4d,0x0(%rax,%rax,1)
+    646ca461:	add    %al,%gs:(%rax)
+    646ca464:	in     $0xb3,%al
+    646ca466:	add    %al,(%rax)
+    646ca468:	push   %rax
+    646ca469:	add    %al,%gs:(%rax)
+    646ca46c:	(bad)
+    646ca46d:	add    %al,%gs:(%rax)
+    646ca470:	lock mov $0x0,%bl
+    646ca473:	add    %dl,%al
+    646ca475:	add    %al,%gs:(%rax)
+    646ca478:	(bad)
     646ca479:	data16 add %al,(%rax)
-    646ca47c:	lock mov $0x0,%bl
-    646ca47f:	add    %dl,%al
+    646ca47c:	clc
+    646ca47d:	mov    $0x0,%bl
+    646ca47f:	add    %dl,(%rax)
     646ca481:	data16 add %al,(%rax)
-    646ca484:	(bad)
-    646ca485:	add    %al,(%eax)
-    646ca488:	clc
-    646ca489:	mov    $0x0,%bl
-    646ca48b:	add    %al,0x67(%rax)
-    646ca48e:	add    %al,(%rax)
-    646ca490:	ja     646ca4f9 <.pdata+0x1>
-    646ca492:	add    %al,(%rax)
-    646ca494:	add    %dh,0x678000(%rax,%rax,1)
-    646ca49b:	add    %dl,(%rcx)
-    646ca49d:	push   $0xffffffffb4080000
-    646ca4a2:	add    %al,(%rax)
-    646ca4a4:	and    %ch,0x0(%rax)
-    646ca4a7:	add    %al,%dh
-    646ca4a9:	push   $0xffffffffb4100000
+    646ca484:	jg     646ca4ec <.pdata>
+    646ca486:	add    %al,(%rax)
+    646ca488:	add    %dh,0x668000(%rax,%rax,1)
+    646ca48f:	add    %dh,0x8000066(%rdi)
+    646ca495:	mov    $0x0,%ah
+    646ca497:	add    %al,%al
+    646ca499:	data16 add %al,(%rax)
+    646ca49c:	push   %rcx
+    646ca49d:	add    %al,(%eax)
+    646ca4a0:	adc    %dh,0x676000(%rax,%rax,1)
+    646ca4a7:	add    %al,(%rsi)
+    646ca4a9:	push   $0xffffffffb4180000
     646ca4ae:	add    %al,(%rax)
-    646ca4b0:	shrb   0x0(%rax)
-    646ca4b3:	add    %dl,%bl
-    646ca4b5:	push   $0xffffffffb4180000
+    646ca4b0:	adc    %ch,0x0(%rax)
+    646ca4b3:	add    %dl,(%rbx)
+    646ca4b5:	push   $0xffffffffb4200000
 	...
 
 00000000646ca4bc <.pdata>:
-    646ca4bc:	and    %ch,0x0(%rcx)
-    646ca4bf:	add    %ah,(%rsi)
-    646ca4c1:	imul   $0xb41c00,(%rax),%eax
+    646ca4bc:	(bad)
+    646ca4bd:	push   $0x68660000
+    646ca4c2:	add    %al,(%rax)
+    646ca4c4:	and    $0xb4,%al
 	...
 
 00000000646ca4c8 <.pdata>:
-    646ca4c8:	xor    %ch,0x0(%rcx)
-    646ca4cb:	add    %dh,(%rsi)
-    646ca4cd:	imul   $0xb42000,(%rax),%eax
-	...
+    646ca4c8:	jo     646ca532 <.pdata+0x16>
+    646ca4ca:	add    %al,(%rax)
+    646ca4cc:	jbe    646ca536 <.pdata+0x2>
+    646ca4ce:	add    %al,(%rax)
+    646ca4d0:	sub    %dh,0x688000(%rax,%rax,1)
 
 00000000646ca4d4 <.pdata>:
-    646ca4d4:	rex imul $0x6a6600,(%rax),%eax
-    646ca4db:	add    %ah,(%rsp,%rsi,4)
+    646ca4d4:	subb   $0x0,0x0(%rax)
+    646ca4d8:	cmpsb  %es:(%rdi),%ds:(%rsi)
+    646ca4d9:	imul   $0xb42c00,(%rax),%eax
 	...
 
 00000000646ca4e0 <.pdata>:
-    646ca4e0:	jo     646ca54c <.pdata>
+    646ca4e0:	mov    $0x69,%al
     646ca4e2:	add    %al,(%rax)
-    646ca4e4:	jne    646ca550 <.pdata+0x4>
+    646ca4e4:	mov    $0x69,%ch
     646ca4e6:	add    %al,(%rax)
-    646ca4e8:	xor    %dh,0x6a8000(%rax,%rax,1)
+    646ca4e8:	cmp    %dh,0x69c000(%rax,%rax,1)
 
 00000000646ca4ec <.pdata>:
-    646ca4ec:	subb   $0x0,0x0(%rdx)
-    646ca4f0:	je     646ca55d <.pdata+0x11>
+    646ca4ec:	shrb   $0x0,0x0(%rcx)
+    646ca4f0:	mov    $0x6a,%ah
     646ca4f2:	add    %al,(%rax)
-    646ca4f4:	xor    $0xb4,%al
+    646ca4f4:	cmp    $0xb4,%al
 	...
 
 00000000646ca4f8 <.pdata>:
-    646ca4f8:	mov    $0x6b,%al
-    646ca4fa:	add    %al,(%rax)
-    646ca4fc:	xchg   %eax,%esp
-    646ca4fd:	insl   (%dx),%es:(%rdi)
+    646ca4f8:	lock push $0x0
+    646ca4fb:	add    %dl,%ah
+    646ca4fd:	insb   (%dx),%es:(%rdi)
     646ca4fe:	add    %al,(%rax)
-    646ca500:	mov    $0x0,%spl
+    646ca500:	rex.W mov $0x0,%spl
 	...
 
 00000000646ca504 <.pdata>:
-    646ca504:	movabs 0x4c00006ec000006d,%al
-    646ca50d:	mov    $0x0,%ah
+    646ca504:	loopne 646ca572 <.pdata+0x2>
+    646ca506:	add    %al,(%rax)
+    646ca508:	add    %ch,0x0(%rsi)
+    646ca50b:	add    %dl,0x0(%rsp,%rsi,4)
 	...
 
 00000000646ca510 <.pdata>:
-    646ca510:	shrb   $0x0,0x0(%rsi)
-    646ca514:	push   %rsi
-    646ca515:	outsl  %ds:(%rsi),(%dx)
-    646ca516:	add    %al,(%rax)
-    646ca518:	pop    %rax
+    646ca510:	add    %ch,0x0(%rsi)
+    646ca513:	add    %dl,0x6000006e(%rsi)
     646ca519:	mov    $0x0,%ah
 	...
 
 00000000646ca51c <.pdata>:
-    646ca51c:	(bad)
-    646ca51d:	outsl  %ds:(%rsi),(%dx)
-    646ca51e:	add    %al,(%rax)
-    646ca520:	mov    $0x74,%bh
-    646ca522:	add    %al,(%rax)
-    646ca524:	(bad)
+    646ca51c:	movabs 0x68000073f700006e,%al
     646ca525:	mov    $0x0,%ah
-    646ca527:	add    %al,%al
+    646ca527:	add    %al,(%rax)
     646ca529:	je     646ca52b <.pdata+0xf>
-    646ca52b:	add    %bh,(%rsi)
-    646ca52d:	ja     646ca52f <.pdata+0x13>
-    646ca52f:	add    %bh,0x0(%rsp,%rsi,4)
-	...
+    646ca52b:	add    %bh,0x76(%rsi)
+    646ca52e:	add    %al,(%rax)
+    646ca530:	test   %dh,0x775000(%rax,%rax,1)
 
 00000000646ca534 <.pdata>:
-    646ca534:	adc    %bh,0x0(%rax)
-    646ca537:	add    %cl,%dh
+    646ca534:	push   %rax
+    646ca535:	ja     646ca537 <.pdata+0x3>
+    646ca537:	add    %cl,(%rsi)
     646ca539:	js     646ca53b <.pdata+0x7>
-    646ca53b:	add    %cl,-0xfffff4c(%rax)
+    646ca53b:	add    %dl,0x300000b4(%rax)
 
 00000000646ca540 <.pdata>:
-    646ca540:	lock jns 646ca543 <.pdata+0x3>
-    646ca543:	add    %dl,-0x6fffff86(%rip)        # fffffffff46ca5c3 <.debug_str+0xffffffff8fff25c3>
+    646ca540:	xor    %bh,0x0(%rcx)
+    646ca543:	add    %dl,0x79(%rbp)
+    646ca546:	add    %al,(%rax)
+    646ca548:	cwtl
     646ca549:	mov    $0x0,%ah
 	...
 
 00000000646ca54c <.pdata>:
-    646ca54c:	and    %bh,0x0(%rdx)
-    646ca54f:	add    %ch,%al
+    646ca54c:	(bad)
+    646ca54d:	jns    646ca54f <.pdata+0x3>
+    646ca54f:	add    %ch,(%rax)
     646ca551:	jp     646ca553 <.pdata+0x7>
-    646ca553:	add    %dl,0x7af00000(%rsp,%rsi,4)
+    646ca553:	add    %bl,0x7a300000(%rsp,%rsi,4)
     646ca55a:	add    %al,(%rax)
-    646ca55c:	pop    %rdi
-    646ca55d:	jnp    646ca55f <.pdata+0x13>
-    646ca55f:	add    %ah,0x7b600000(%rsp,%rsi,4)
+    646ca55c:	lahf
+    646ca55d:	jp     646ca55f <.pdata+0x13>
+    646ca55f:	add    %ch,0x7aa00000(%rsp,%rsi,4)
     646ca566:	add    %al,(%rax)
-    646ca568:	jg     646ca5e5 <.pdata.startup+0x45>
-    646ca56a:	add    %al,(%rax)
-    646ca56c:	mov    $0xb4,%al
+    646ca568:	mov    $0xb800007a,%edi
+    646ca56d:	mov    $0x0,%ah
 	...
 
 00000000646ca570 <.pdata>:
-    646ca570:	push   %rax
-    646ca571:	jl     646ca573 <.pdata+0x3>
-    646ca573:	add    %dl,-0x47ffff84(%rcx)
+    646ca570:	nop
+    646ca571:	jnp    646ca573 <.pdata+0x3>
+    646ca573:	add    %dl,%cl
+    646ca575:	jnp    646ca577 <.pdata+0x7>
+    646ca577:	add    %al,%al
     646ca579:	mov    $0x0,%ah
 	...
 
 00000000646ca57c <.pdata>:
-    646ca57c:	movabs 0xc000007cac00007c,%al
+    646ca57c:	loopne 646ca5f9 <.pdata.startup+0x59>
+    646ca57e:	add    %al,(%rax)
+    646ca580:	in     (%dx),%al
+    646ca581:	jnp    646ca583 <.pdata+0x7>
+    646ca583:	add    %cl,%al
     646ca585:	mov    $0x0,%ah
-    646ca587:	add    %dh,-0x53ffff84(%rax)
-    646ca58d:	jge    646ca58f <.pdata+0x13>
-    646ca58f:	add    %al,%ah
+    646ca587:	add    %dh,%al
+    646ca589:	jnp    646ca58b <.pdata+0xf>
+    646ca58b:	add    %ch,%ah
+    646ca58d:	jl     646ca58f <.pdata+0x13>
+    646ca58f:	add    %cl,%ah
     646ca591:	mov    $0x0,%ah
-    646ca593:	add    %al,%al
+    646ca593:	add    %al,(%rax)
     646ca595:	jge    646ca597 <.pdata+0x1b>
-    646ca597:	add    %ch,(%rcx)
-    646ca599:	jle    646ca59b <.pdata+0x1f>
-    646ca59b:	add    %cl,0x0(%rbx,%rsi,4)
+    646ca597:	add    %ch,0x7d(%rcx)
+    646ca59a:	add    %al,(%rax)
+    646ca59c:	push   %rsp
+    646ca59d:	mov    $0x0,%bl
 	...
 
 00000000646ca5a0 <.pdata.startup>:
-    646ca5a0:	xor    %bh,0x0(%rsi)
-    646ca5a3:	add    %dh,-0x23ffff82(%rip)        # 406ca627 <__size_of_stack_reserve__+0x404ca627>
-    646ca5a9:	mov    $0x0,%ah
+    646ca5a0:	jo     646ca61f <.pdata.startup+0x7f>
+    646ca5a2:	add    %al,(%rax)
+    646ca5a4:	jne    646ca623 <.pdata.startup+0x83>
+    646ca5a6:	add    %al,(%rax)
+    646ca5a8:	in     $0xb4,%al
 	...
 
 Disassembly of section .xdata:
 
 00000000646cb000 <.xdata>:
     646cb000:	add    %eax,(%rax)
     646cb002:	add    %al,(%rax)
@@ -12426,605 +12438,616 @@
     646cb193:	add    %al,(%rsi)
     646cb195:	(bad)
     646cb197:	xor    %al,(%rcx)
     646cb199:	(bad)
     646cb19a:	add    %al,(%rax)
     646cb19c:	add    %eax,(%rax)
     646cb19e:	add    %al,(%rax)
-    646cb1a0:	add    %ecx,(%rsi,%rax,1)
-    646cb1a3:	add    %cl,(%rax,%rbp,2)
-    646cb1a6:	add    (%rax),%al
-    646cb1a8:	(bad)
+    646cb1a0:	add    %ecx,(%rdi)
+    646cb1a2:	or     %al,(%rax)
+    646cb1a4:	punpckhbw (%rdx),%mm0
+    646cb1a7:	add    %cl,(%rdx)
     646cb1a9:	push   %rdx
-    646cb1aa:	add    (%rax),%esi
-    646cb1ac:	add    0x1(%rax),%ah
-    646cb1af:	jo     646cb1b2 <.xdata+0x26>
-    646cb1b1:	adc    %al,(%rdi)
-    646cb1b3:	add    %dl,(%rax)
-    646cb1b5:	js     646cb1bb <.xdata+0x2f>
-    646cb1b7:	add    %cl,(%rbx)
-    646cb1b9:	push   $0xffffffffa2060003
-    646cb1be:	add    (%rax),%dh
-    646cb1c0:	add    %esp,0x0(%rax)
-    646cb1c3:	add    %al,(%rcx)
-    646cb1c5:	invd
-    646cb1c7:	add    %cl,(%rdi)
-    646cb1c9:	push   $0x520a0002
-    646cb1ce:	(bad)
-    646cb1cf:	xor    %al,0x3700460(%rip)        # 67dcb635 <.debug_str+0x36f3635>
-    646cb1d5:	push   %rax
-    646cb1d6:	add    %al,%al
-    646cb1d8:	add    %ecx,0x780d0005(%rip)        # dc79b1e3 <.debug_str+0x780c31e3>
-    646cb1de:	add    %eax,(%rax)
-    646cb1e0:	or     %ch,0x0(%rax)
-    646cb1e3:	add    %al,(%rdx,%rax,2)
-    646cb1e6:	add    %al,(%rax)
-    646cb1e8:	add    %eax,(%rdi)
-    646cb1ea:	add    $0x0,%al
-    646cb1ec:	(bad)
-    646cb1ed:	xor    (%rbx),%al
-    646cb1ef:	xor    %al,(%rdx)
-    646cb1f1:	(bad)
-    646cb1f2:	add    %esi,0x1(%rax)
-
-00000000646cb1f4 <.xdata>:
-    646cb1f4:	add    %eax,(%rcx,%rax,1)
-    646cb1f7:	add    %al,(%rdx,%riz,2)
-    646cb1fa:	add    %al,(%rax)
-    646cb1fc:	add    %ecx,(%rax,%rcx,1)
-    646cb1ff:	add    %cl,(%rax,%rsi,1)
-    646cb202:	or     0xa(%rax),%esp
-    646cb205:	jo     646cb210 <.xdata+0x1c>
-    646cb207:	push   %rax
-    646cb208:	or     %al,%al
-    646cb20a:	(bad)
-    646cb20b:	rolb   (%rax,%riz,8)
-    646cb20e:	add    %al,%dh
-    646cb210:	add    %edx,(%rbx)
-    646cb212:	or     (%rax),%al
-    646cb214:	adc    (%rcx),%eax
-    646cb216:	adc    $0xb300c00,%eax
-    646cb21b:	(bad)
-    646cb21c:	or     0x9(%rax),%dh
-    646cb21f:	push   %rax
-    646cb220:	or     %al,%al
-    646cb222:	(bad)
-    646cb223:	rolb   (%rax,%riz,8)
-    646cb226:	add    %al,%dh
-    646cb228:	add    %eax,0x32050002(%rip)        # 9671b230 <.debug_str+0x32043230>
-    646cb22e:	add    %esi,(%rax)
-    646cb230:	add    %eax,0x32050002(%rip)        # 9671b238 <.debug_str+0x32043238>
-    646cb236:	add    %esi,(%rax)
-    646cb238:	add    %edx,(%rax)
-    646cb23a:	or     %eax,(%rax)
-    646cb23c:	adc    %al,0xc(%rdx)
-    646cb23f:	xor    %cl,(%rbx)
-    646cb241:	(bad)
-    646cb242:	or     0x9(%rax),%dh
-    646cb245:	push   %rax
-    646cb246:	or     %al,%al
-    646cb248:	(bad)
-    646cb249:	rolb   (%rax,%riz,8)
-    646cb24c:	add    %al,%dh
-    646cb24e:	add    %al,(%rax)
-    646cb250:	add    %ecx,(%rdx)
-    646cb252:	(bad)
-    646cb253:	add    %cl,(%rdx)
-    646cb255:	xor    %cl,(%rcx)
-    646cb257:	(bad)
-    646cb258:	or     %dh,0x7(%rax)
-    646cb25b:	push   %rax
-    646cb25c:	(bad)
-    646cb25d:	rolb   $0x2,(%rax,%rdx,8)
-    646cb261:	loopne 646cb263 <.xdata+0x6f>
-    646cb263:	add    %al,(%rcx)
-    646cb265:	invd
-    646cb267:	add    %cl,(%rdi)
-    646cb269:	add    %edi,(%rbx)
-    646cb26b:	add    %cl,(%rax)
-    646cb26d:	xor    %al,(%rdi)
-    646cb26f:	(bad)
-    646cb270:	(bad)
-    646cb271:	jo     646cb278 <.xdata>
-    646cb273:	push   %rax
-    646cb274:	add    $0xc0,%al
-    646cb276:	add    %al,%dl
-
-00000000646cb278 <.xdata>:
-    646cb278:	add    %eax,(%rdi)
-    646cb27a:	add    $0x0,%al
-    646cb27c:	(bad)
-    646cb27d:	xor    (%rbx),%al
-    646cb27f:	xor    %al,(%rdx)
-    646cb281:	(bad)
-    646cb282:	add    %esi,0x1(%rax)
-
-00000000646cb284 <.xdata>:
-    646cb284:	add    %eax,0x32050002(%rip)        # 9671b28c <.debug_str+0x3204328c>
-    646cb28a:	add    %esi,(%rax)
-    646cb28c:	add    %edx,(%rbx)
-    646cb28e:	or     (%rax),%al
-    646cb290:	adc    (%rcx),%eax
-    646cb292:	add    %ecx,(%r8,%rsi,1)
-    646cb296:	or     0xa(%rax),%esp
-    646cb299:	jo     646cb2a4 <.xdata+0x20>
-    646cb29b:	push   %rax
-    646cb29c:	or     %al,%al
-    646cb29e:	(bad)
-    646cb29f:	rolb   (%rax,%riz,8)
-    646cb2a2:	add    %al,%dh
-    646cb2a4:	add    %eax,(%rax)
-	...
-
-00000000646cb2a8 <.xdata>:
-    646cb2a8:	add    %eax,(%rax)
-    646cb2aa:	add    %al,(%rax)
+    646cb1aa:	(bad)
+    646cb1ab:	xor    %al,0x3700460(%rip)        # 67dcb611 <.debug_str+0x36f3611>
+    646cb1b1:	push   %rax
+    646cb1b2:	add    %al,%al
+    646cb1b4:	add    %edx,(%rax)
+    646cb1b6:	(bad)
+    646cb1b7:	add    %dl,(%rax)
+    646cb1b9:	js     646cb1bf <.xdata+0x33>
+    646cb1bb:	add    %cl,(%rbx)
+    646cb1bd:	push   $0xffffffffa2060003
+    646cb1c2:	add    (%rax),%dh
+    646cb1c4:	add    %esp,0x0(%rax)
+    646cb1c7:	add    %al,(%rcx)
+    646cb1c9:	invd
+    646cb1cb:	add    %cl,(%rdi)
+    646cb1cd:	push   $0x520a0002
+    646cb1d2:	(bad)
+    646cb1d3:	xor    %al,0x3700460(%rip)        # 67dcb639 <.debug_str+0x36f3639>
+    646cb1d9:	push   %rax
+    646cb1da:	add    %al,%al
+    646cb1dc:	add    %ecx,0x780d0005(%rip)        # dc79b1e7 <.debug_str+0x780c31e7>
+    646cb1e2:	add    %eax,(%rax)
+    646cb1e4:	or     %ch,0x0(%rax)
+    646cb1e7:	add    %al,(%rdx,%rax,2)
+    646cb1ea:	add    %al,(%rax)
+    646cb1ec:	add    %eax,(%rdi)
+    646cb1ee:	add    $0x0,%al
+    646cb1f0:	(bad)
+    646cb1f1:	xor    (%rbx),%al
+    646cb1f3:	xor    %al,(%rdx)
+    646cb1f5:	(bad)
+    646cb1f6:	add    %esi,0x1(%rax)
+
+00000000646cb1f8 <.xdata>:
+    646cb1f8:	add    %eax,(%rcx,%rax,1)
+    646cb1fb:	add    %al,(%rdx,%riz,2)
+    646cb1fe:	add    %al,(%rax)
+    646cb200:	add    %ecx,(%rax,%rcx,1)
+    646cb203:	add    %cl,(%rax,%rsi,1)
+    646cb206:	or     0xa(%rax),%esp
+    646cb209:	jo     646cb214 <.xdata+0x1c>
+    646cb20b:	push   %rax
+    646cb20c:	or     %al,%al
+    646cb20e:	(bad)
+    646cb20f:	rolb   (%rax,%riz,8)
+    646cb212:	add    %al,%dh
+    646cb214:	add    %edx,(%rax)
+    646cb216:	or     %eax,(%rax)
+    646cb218:	adc    %ah,0xc(%rdx)
+    646cb21b:	xor    %cl,(%rbx)
+    646cb21d:	(bad)
+    646cb21e:	or     0x9(%rax),%dh
+    646cb221:	push   %rax
+    646cb222:	or     %al,%al
+    646cb224:	(bad)
+    646cb225:	rolb   (%rax,%riz,8)
+    646cb228:	add    %al,%dh
+    646cb22a:	add    %al,(%rax)
+    646cb22c:	add    %eax,0x32050002(%rip)        # 9671b234 <.debug_str+0x32043234>
+    646cb232:	add    %esi,(%rax)
+    646cb234:	add    %eax,0x32050002(%rip)        # 9671b23c <.debug_str+0x3204323c>
+    646cb23a:	add    %esi,(%rax)
+    646cb23c:	add    %edx,(%rax)
+    646cb23e:	or     %eax,(%rax)
+    646cb240:	adc    %al,0xc(%rdx)
+    646cb243:	xor    %cl,(%rbx)
+    646cb245:	(bad)
+    646cb246:	or     0x9(%rax),%dh
+    646cb249:	push   %rax
+    646cb24a:	or     %al,%al
+    646cb24c:	(bad)
+    646cb24d:	rolb   (%rax,%riz,8)
+    646cb250:	add    %al,%dh
+    646cb252:	add    %al,(%rax)
+    646cb254:	add    %ecx,(%rdx)
+    646cb256:	(bad)
+    646cb257:	add    %cl,(%rdx)
+    646cb259:	xor    %cl,(%rcx)
+    646cb25b:	(bad)
+    646cb25c:	or     %dh,0x7(%rax)
+    646cb25f:	push   %rax
+    646cb260:	(bad)
+    646cb261:	rolb   $0x2,(%rax,%rdx,8)
+    646cb265:	loopne 646cb267 <.xdata+0x6f>
+    646cb267:	add    %al,(%rcx)
+    646cb269:	invd
+    646cb26b:	add    %cl,(%rdi)
+    646cb26d:	add    %edi,(%rbx)
+    646cb26f:	add    %cl,(%rax)
+    646cb271:	xor    %al,(%rdi)
+    646cb273:	(bad)
+    646cb274:	(bad)
+    646cb275:	jo     646cb27c <.xdata>
+    646cb277:	push   %rax
+    646cb278:	add    $0xc0,%al
+    646cb27a:	add    %al,%dl
+
+00000000646cb27c <.xdata>:
+    646cb27c:	add    %eax,(%rdi)
+    646cb27e:	add    $0x0,%al
+    646cb280:	(bad)
+    646cb281:	xor    (%rbx),%al
+    646cb283:	xor    %al,(%rdx)
+    646cb285:	(bad)
+    646cb286:	add    %esi,0x1(%rax)
+
+00000000646cb288 <.xdata>:
+    646cb288:	add    %eax,(%rsi)
+    646cb28a:	add    (%rax),%eax
+    646cb28c:	(bad)
+    646cb28d:	rex.X add (%rax),%sil
+    646cb290:	add    %esp,0x0(%rax)
+    646cb293:	add    %al,(%rcx)
+    646cb295:	adc    (%rdx),%ecx
+    646cb297:	add    %dl,(%rbx)
+    646cb299:	add    %eax,0x1(%rcx)
+    646cb29c:	or     $0x30,%al
+    646cb29e:	or     0xa(%rax),%esp
+    646cb2a1:	jo     646cb2ac <.xdata+0x24>
+    646cb2a3:	push   %rax
+    646cb2a4:	or     %al,%al
+    646cb2a6:	(bad)
+    646cb2a7:	rolb   (%rax,%riz,8)
+    646cb2aa:	add    %al,%dh
     646cb2ac:	add    %eax,(%rax)
-    646cb2ae:	add    %al,(%rax)
-    646cb2b0:	add    %ecx,(%rax)
-    646cb2b2:	add    $0x4420800,%eax
-    646cb2b7:	xor    %al,(%rbx)
-    646cb2b9:	(bad)
-    646cb2ba:	add    0x1(%rax),%dh
-    646cb2bd:	push   %rax
-    646cb2be:	add    %al,(%rax)
-    646cb2c0:	add    %eax,(%rsi)
-    646cb2c2:	add    $0x5300600,%eax
-    646cb2c7:	(bad)
-    646cb2c8:	add    $0x70,%al
-    646cb2ca:	add    0x2(%rax),%edx
-    646cb2cd:	rolb   $0x0,(%rax)
-
-00000000646cb2d0 <.xdata>:
-    646cb2d0:	add    %ebx,(%rdx)
-    646cb2d2:	or     $0x5781a00,%eax
-    646cb2d7:	add    %dl,0x10000468(%rip)        # 746cb745 <.debug_str+0xfff3745>
-    646cb2dd:	ret    $0x300c
-    646cb2e0:	or     0xa(%rax),%esp
-    646cb2e3:	jo     646cb2ee <.xdata+0x1e>
-    646cb2e5:	push   %rax
-    646cb2e6:	or     %al,%al
-    646cb2e8:	(bad)
-    646cb2e9:	rolb   (%rax,%riz,8)
-    646cb2ec:	add    %al,%dh
-    646cb2ee:	add    %al,(%rax)
-    646cb2f0:	add    %eax,(%rax)
-	...
-
-00000000646cb2f4 <.xdata>:
-    646cb2f4:	add    %eax,(%rcx,%rax,1)
-    646cb2f7:	add    %al,(%rdx,%rax,2)
-    646cb2fa:	add    %al,(%rax)
-    646cb2fc:	add    %eax,(%rsi)
-    646cb2fe:	add    (%rax),%eax
-    646cb300:	(bad)
-    646cb301:	rex.X add (%rax),%sil
-    646cb304:	add    %esp,0x0(%rax)
-    646cb307:	add    %al,(%rcx)
-    646cb309:	add    %al,(%rax)
-	...
-
-00000000646cb30c <.xdata>:
-    646cb30c:	add    %ecx,(%rdx)
-    646cb30e:	(bad)
-    646cb30f:	add    %cl,(%rdx)
-    646cb311:	push   %rdx
-    646cb312:	(bad)
-    646cb313:	xor    %al,0x3700460(%rip)        # 67dcb779 <.debug_str+0x36f3779>
-    646cb319:	push   %rax
-    646cb31a:	add    %al,%al
-    646cb31c:	add    %ecx,(%rdx)
-    646cb31e:	add    $0x6d20a05,%eax
-    646cb323:	add    (%rbx),%eax
-    646cb325:	xor    %al,(%rdx)
-    646cb327:	(bad)
-    646cb328:	add    %edx,0x0(%rax)
-	...
-
-00000000646cb32c <.xdata>:
-    646cb32c:	add    %eax,(%rcx,%rax,1)
-    646cb32f:	add    %al,(%rdx,%rax,2)
-    646cb332:	add    %al,(%rax)
-    646cb334:	add    %eax,(%rsi)
-    646cb336:	add    (%rax),%eax
-    646cb338:	(bad)
-    646cb339:	rex.X add (%rax),%sil
-    646cb33c:	add    %esp,0x0(%rax)
-    646cb33f:	add    %al,(%rcx)
-    646cb341:	add    %al,(%rax)
-	...
-
-00000000646cb344 <.xdata>:
-    646cb344:	add    %eax,(%rax)
-    646cb346:	add    %al,(%rax)
-    646cb348:	add    %eax,(%rax)
-	...
-
-00000000646cb34c <.xdata.unlikely>:
-    646cb34c:	add    %eax,(%rsi)
-    646cb34e:	add    (%rax),%eax
-    646cb350:	(bad)
-    646cb351:	(bad)
-    646cb353:	xor    %al,(%rcx)
-    646cb355:	(bad)
-	...
-
-00000000646cb358 <.xdata>:
-    646cb358:	add    %ecx,(%rdx)
-    646cb35a:	(bad)
-    646cb35b:	add    %cl,(%rdx)
-    646cb35d:	xchg   %eax,%edx
-    646cb35e:	(bad)
-    646cb35f:	xor    %al,0x3700460(%rip)        # 67dcb7c5 <.debug_str+0x36f37c5>
-    646cb365:	push   %rax
-    646cb366:	add    %al,%al
-    646cb368:	add    %ebx,(%rax)
-    646cb36a:	or     0x62100318(%rbp),%al
-    646cb370:	or     $0x30,%al
-    646cb372:	or     0xa(%rax),%esp
-    646cb375:	jo     646cb380 <.xdata>
-    646cb377:	rolb   $0xd0,(%rdi)
-    646cb37a:	add    $0x1f003e0,%eax
-    646cb37f:	push   %rax
-
-00000000646cb380 <.xdata>:
-    646cb380:	add    %eax,(%rcx,%rax,1)
-    646cb383:	add    %al,(%rdx,%rax,2)
-    646cb386:	add    %al,(%rax)
-    646cb388:	add    %ecx,(%rdx)
-    646cb38a:	(bad)
-    646cb38b:	add    %cl,(%rdx)
-    646cb38d:	xor    (%rsi),%al
-    646cb38f:	xor    %al,0x3700460(%rip)        # 67dcb7f5 <.debug_str+0x36f37f5>
-    646cb395:	push   %rax
-    646cb396:	add    %al,%al
-    646cb398:	add    %eax,0x32050002(%rip)        # 9671b3a0 <.debug_str+0x320433a0>
-    646cb39e:	add    %esi,(%rax)
-
-00000000646cb3a0 <.xdata>:
-    646cb3a0:	add    %ecx,(%rax)
-    646cb3a2:	add    $0x4420800,%eax
-    646cb3a7:	xor    %al,(%rbx)
-    646cb3a9:	(bad)
-    646cb3aa:	add    0x1(%rax),%dh
-    646cb3ad:	push   %rax
-    646cb3ae:	add    %al,(%rax)
-    646cb3b0:	add    %ecx,(%rax)
-    646cb3b2:	add    $0x4420800,%eax
-    646cb3b7:	xor    %al,(%rbx)
-    646cb3b9:	(bad)
-    646cb3ba:	add    0x1(%rax),%dh
-    646cb3bd:	push   %rax
-    646cb3be:	add    %al,(%rax)
-    646cb3c0:	add    %eax,0x32050002(%rip)        # 9671b3c8 <.debug_str+0x320433c8>
-    646cb3c6:	add    %esi,(%rax)
+	...
+
+00000000646cb2b0 <.xdata>:
+    646cb2b0:	add    %eax,(%rax)
+    646cb2b2:	add    %al,(%rax)
+    646cb2b4:	add    %eax,(%rax)
+    646cb2b6:	add    %al,(%rax)
+    646cb2b8:	add    %ecx,(%rax)
+    646cb2ba:	add    $0x4420800,%eax
+    646cb2bf:	xor    %al,(%rbx)
+    646cb2c1:	(bad)
+    646cb2c2:	add    0x1(%rax),%dh
+    646cb2c5:	push   %rax
+    646cb2c6:	add    %al,(%rax)
+    646cb2c8:	add    %eax,(%rsi)
+    646cb2ca:	add    $0x5300600,%eax
+    646cb2cf:	(bad)
+    646cb2d0:	add    $0x70,%al
+    646cb2d2:	add    0x2(%rax),%edx
+    646cb2d5:	rolb   $0x0,(%rax)
+
+00000000646cb2d8 <.xdata>:
+    646cb2d8:	add    %ebx,(%rdx)
+    646cb2da:	or     $0x5781a00,%eax
+    646cb2df:	add    %dl,0x10000468(%rip)        # 746cb74d <.debug_str+0xfff374d>
+    646cb2e5:	ret    $0x300c
+    646cb2e8:	or     0xa(%rax),%esp
+    646cb2eb:	jo     646cb2f6 <.xdata+0x1e>
+    646cb2ed:	push   %rax
+    646cb2ee:	or     %al,%al
+    646cb2f0:	(bad)
+    646cb2f1:	rolb   (%rax,%riz,8)
+    646cb2f4:	add    %al,%dh
+    646cb2f6:	add    %al,(%rax)
+    646cb2f8:	add    %eax,(%rax)
+	...
+
+00000000646cb2fc <.xdata>:
+    646cb2fc:	add    %eax,(%rcx,%rax,1)
+    646cb2ff:	add    %al,(%rdx,%rax,2)
+    646cb302:	add    %al,(%rax)
+    646cb304:	add    %eax,(%rsi)
+    646cb306:	add    (%rax),%eax
+    646cb308:	(bad)
+    646cb309:	rex.X add (%rax),%sil
+    646cb30c:	add    %esp,0x0(%rax)
+    646cb30f:	add    %al,(%rcx)
+    646cb311:	add    %al,(%rax)
+	...
+
+00000000646cb314 <.xdata>:
+    646cb314:	add    %ecx,(%rdx)
+    646cb316:	(bad)
+    646cb317:	add    %cl,(%rdx)
+    646cb319:	push   %rdx
+    646cb31a:	(bad)
+    646cb31b:	xor    %al,0x3700460(%rip)        # 67dcb781 <.debug_str+0x36f3781>
+    646cb321:	push   %rax
+    646cb322:	add    %al,%al
+    646cb324:	add    %ecx,(%rdx)
+    646cb326:	add    $0x6d20a05,%eax
+    646cb32b:	add    (%rbx),%eax
+    646cb32d:	xor    %al,(%rdx)
+    646cb32f:	(bad)
+    646cb330:	add    %edx,0x0(%rax)
+	...
+
+00000000646cb334 <.xdata>:
+    646cb334:	add    %eax,(%rcx,%rax,1)
+    646cb337:	add    %al,(%rdx,%rax,2)
+    646cb33a:	add    %al,(%rax)
+    646cb33c:	add    %eax,(%rsi)
+    646cb33e:	add    (%rax),%eax
+    646cb340:	(bad)
+    646cb341:	rex.X add (%rax),%sil
+    646cb344:	add    %esp,0x0(%rax)
+    646cb347:	add    %al,(%rcx)
+    646cb349:	add    %al,(%rax)
+	...
+
+00000000646cb34c <.xdata>:
+    646cb34c:	add    %eax,(%rax)
+    646cb34e:	add    %al,(%rax)
+    646cb350:	add    %eax,(%rax)
+	...
+
+00000000646cb354 <.xdata.unlikely>:
+    646cb354:	add    %eax,(%rsi)
+    646cb356:	add    (%rax),%eax
+    646cb358:	(bad)
+    646cb359:	(bad)
+    646cb35b:	xor    %al,(%rcx)
+    646cb35d:	(bad)
+	...
+
+00000000646cb360 <.xdata>:
+    646cb360:	add    %ecx,(%rdx)
+    646cb362:	(bad)
+    646cb363:	add    %cl,(%rdx)
+    646cb365:	xchg   %eax,%edx
+    646cb366:	(bad)
+    646cb367:	xor    %al,0x3700460(%rip)        # 67dcb7cd <.debug_str+0x36f37cd>
+    646cb36d:	push   %rax
+    646cb36e:	add    %al,%al
+    646cb370:	add    %ebx,(%rax)
+    646cb372:	or     0x62100318(%rbp),%al
+    646cb378:	or     $0x30,%al
+    646cb37a:	or     0xa(%rax),%esp
+    646cb37d:	jo     646cb388 <.xdata>
+    646cb37f:	rolb   $0xd0,(%rdi)
+    646cb382:	add    $0x1f003e0,%eax
+    646cb387:	push   %rax
+
+00000000646cb388 <.xdata>:
+    646cb388:	add    %eax,(%rcx,%rax,1)
+    646cb38b:	add    %al,(%rdx,%rax,2)
+    646cb38e:	add    %al,(%rax)
+    646cb390:	add    %ecx,(%rdx)
+    646cb392:	(bad)
+    646cb393:	add    %cl,(%rdx)
+    646cb395:	xor    (%rsi),%al
+    646cb397:	xor    %al,0x3700460(%rip)        # 67dcb7fd <.debug_str+0x36f37fd>
+    646cb39d:	push   %rax
+    646cb39e:	add    %al,%al
+    646cb3a0:	add    %eax,0x32050002(%rip)        # 9671b3a8 <.debug_str+0x320433a8>
+    646cb3a6:	add    %esi,(%rax)
+
+00000000646cb3a8 <.xdata>:
+    646cb3a8:	add    %ecx,(%rax)
+    646cb3aa:	add    $0x4420800,%eax
+    646cb3af:	xor    %al,(%rbx)
+    646cb3b1:	(bad)
+    646cb3b2:	add    0x1(%rax),%dh
+    646cb3b5:	push   %rax
+    646cb3b6:	add    %al,(%rax)
+    646cb3b8:	add    %ecx,(%rax)
+    646cb3ba:	add    $0x4420800,%eax
+    646cb3bf:	xor    %al,(%rbx)
+    646cb3c1:	(bad)
+    646cb3c2:	add    0x1(%rax),%dh
+    646cb3c5:	push   %rax
+    646cb3c6:	add    %al,(%rax)
     646cb3c8:	add    %eax,0x32050002(%rip)        # 9671b3d0 <.debug_str+0x320433d0>
     646cb3ce:	add    %esi,(%rax)
+    646cb3d0:	add    %eax,0x32050002(%rip)        # 9671b3d8 <.debug_str+0x320433d8>
+    646cb3d6:	add    %esi,(%rax)
 
-00000000646cb3d0 <.xdata>:
-    646cb3d0:	add    %eax,(%rax)
-    646cb3d2:	add    %al,(%rax)
-    646cb3d4:	add    %eax,(%rax)
-    646cb3d6:	add    %al,(%rax)
+00000000646cb3d8 <.xdata>:
     646cb3d8:	add    %eax,(%rax)
     646cb3da:	add    %al,(%rax)
-    646cb3dc:	add    %eax,(%rdi)
-    646cb3de:	add    $0x0,%al
-    646cb3e0:	(bad)
-    646cb3e1:	xor    (%rbx),%al
-    646cb3e3:	xor    %al,(%rdx)
-    646cb3e5:	(bad)
-    646cb3e6:	add    %esi,0x1(%rax)
-    646cb3e9:	add    $0x1,%al
-    646cb3eb:	add    %al,(%rdx,%rax,2)
-    646cb3ee:	add    %al,(%rax)
-    646cb3f0:	add    %eax,(%rcx,%rax,1)
+    646cb3dc:	add    %eax,(%rax)
+    646cb3de:	add    %al,(%rax)
+    646cb3e0:	add    %eax,(%rax)
+    646cb3e2:	add    %al,(%rax)
+    646cb3e4:	add    %eax,(%rdi)
+    646cb3e6:	add    $0x0,%al
+    646cb3e8:	(bad)
+    646cb3e9:	xor    (%rbx),%al
+    646cb3eb:	xor    %al,(%rdx)
+    646cb3ed:	(bad)
+    646cb3ee:	add    %esi,0x1(%rax)
+    646cb3f1:	add    $0x1,%al
     646cb3f3:	add    %al,(%rdx,%rax,2)
     646cb3f6:	add    %al,(%rax)
     646cb3f8:	add    %eax,(%rcx,%rax,1)
     646cb3fb:	add    %al,(%rdx,%rax,2)
     646cb3fe:	add    %al,(%rax)
     646cb400:	add    %eax,(%rcx,%rax,1)
     646cb403:	add    %al,(%rdx,%rax,2)
     646cb406:	add    %al,(%rax)
     646cb408:	add    %eax,(%rcx,%rax,1)
     646cb40b:	add    %al,(%rdx,%rax,2)
     646cb40e:	add    %al,(%rax)
     646cb410:	add    %eax,(%rcx,%rax,1)
     646cb413:	add    %al,(%rdx,%rax,2)
+    646cb416:	add    %al,(%rax)
+    646cb418:	add    %eax,(%rcx,%rax,1)
+    646cb41b:	add    %al,(%rdx,%rax,2)
 	...
 
-00000000646cb418 <.xdata>:
-    646cb418:	add    %eax,(%rax)
+00000000646cb420 <.xdata>:
+    646cb420:	add    %eax,(%rax)
 	...
 
-00000000646cb41c <.xdata>:
-    646cb41c:	add    %eax,(%rax)
+00000000646cb424 <.xdata>:
+    646cb424:	add    %eax,(%rax)
 	...
 
-00000000646cb420 <.xdata>:
-    646cb420:	add    %eax,(%rax)
+00000000646cb428 <.xdata>:
+    646cb428:	add    %eax,(%rax)
 	...
 
-00000000646cb424 <.xdata>:
-    646cb424:	add    %ecx,(%rdx)
-    646cb426:	add    $0x0,%al
-    646cb428:	or     0x4(%rax),%ch
-    646cb42b:	add    %al,0x1300192(%rip)        # 659cb5c3 <.debug_str+0x12f35c3>
-
-00000000646cb430 <.xdata>:
-    646cb430:	add    %eax,(%rax)
-	...
-
-00000000646cb434 <.xdata>:
-    646cb434:	add    %ecx,(%rdx)
-    646cb436:	add    $0x0,%al
-    646cb438:	or     0x6(%rax),%ch
-    646cb43b:	add    %al,0x13001d2(%rip)        # 659cb613 <.debug_str+0x12f3613>
-
-00000000646cb440 <.xdata>:
-    646cb440:	add    %ecx,(%rdx)
-    646cb442:	add    $0x0,%al
-    646cb444:	or     0x4(%rax),%ch
-    646cb447:	add    %al,0x1300192(%rip)        # 659cb5df <.debug_str+0x12f35df>
-
-00000000646cb44c <.xdata>:
-    646cb44c:	add    %ecx,(%rdx)
-    646cb44e:	add    $0x0,%al
-    646cb450:	or     0x6(%rax),%ch
-    646cb453:	add    %al,0x13001d2(%rip)        # 659cb62b <.debug_str+0x12f362b>
-
-00000000646cb458 <.xdata>:
-    646cb458:	add    %eax,(%rcx,%rax,1)
-    646cb45b:	add    %al,(%rdx,%riz,1)
-    646cb45e:	add    %al,(%rax)
-    646cb460:	add    %ebx,(%rdx)
-    646cb462:	or     (%rax),%eax
-    646cb464:	sbb    0x8(%rax),%bh
-    646cb467:	add    %dl,(%rdx)
-    646cb469:	push   $0x10d0007
-    646cb46e:	adc    (%rax),%al
-    646cb470:	(bad)
-    646cb471:	xor    %al,0x3700460(%rip)        # 67dcb8d7 <.debug_str+0x36f38d7>
-    646cb477:	push   %rax
-    646cb478:	add    %al,%al
-	...
-
-00000000646cb47c <.xdata>:
-    646cb47c:	add    %ecx,(%rcx)
-    646cb47e:	add    (%rax),%eax
-    646cb480:	or     %ebp,0x4(%rax)
-    646cb483:	add    %al,(%rdx,%riz,4)
-	...
-
-00000000646cb488 <.xdata>:
-    646cb488:	add    %eax,0x52050002(%rip)        # b671b490 <.debug_str+0x52043490>
-    646cb48e:	add    %esi,(%rax)
+00000000646cb42c <.xdata>:
+    646cb42c:	add    %ecx,(%rdx)
+    646cb42e:	add    $0x0,%al
+    646cb430:	or     0x4(%rax),%ch
+    646cb433:	add    %al,0x1300192(%rip)        # 659cb5cb <.debug_str+0x12f35cb>
+
+00000000646cb438 <.xdata>:
+    646cb438:	add    %eax,(%rax)
+	...
+
+00000000646cb43c <.xdata>:
+    646cb43c:	add    %ecx,(%rdx)
+    646cb43e:	add    $0x0,%al
+    646cb440:	or     0x6(%rax),%ch
+    646cb443:	add    %al,0x13001d2(%rip)        # 659cb61b <.debug_str+0x12f361b>
+
+00000000646cb448 <.xdata>:
+    646cb448:	add    %ecx,(%rdx)
+    646cb44a:	add    $0x0,%al
+    646cb44c:	or     0x4(%rax),%ch
+    646cb44f:	add    %al,0x1300192(%rip)        # 659cb5e7 <.debug_str+0x12f35e7>
+
+00000000646cb454 <.xdata>:
+    646cb454:	add    %ecx,(%rdx)
+    646cb456:	add    $0x0,%al
+    646cb458:	or     0x6(%rax),%ch
+    646cb45b:	add    %al,0x13001d2(%rip)        # 659cb633 <.debug_str+0x12f3633>
+
+00000000646cb460 <.xdata>:
+    646cb460:	add    %eax,(%rcx,%rax,1)
+    646cb463:	add    %al,(%rdx,%riz,1)
+    646cb466:	add    %al,(%rax)
+    646cb468:	add    %ebx,(%rdx)
+    646cb46a:	or     (%rax),%eax
+    646cb46c:	sbb    0x8(%rax),%bh
+    646cb46f:	add    %dl,(%rdx)
+    646cb471:	push   $0x10d0007
+    646cb476:	adc    (%rax),%al
+    646cb478:	(bad)
+    646cb479:	xor    %al,0x3700460(%rip)        # 67dcb8df <.debug_str+0x36f38df>
+    646cb47f:	push   %rax
+    646cb480:	add    %al,%al
+	...
+
+00000000646cb484 <.xdata>:
+    646cb484:	add    %ecx,(%rcx)
+    646cb486:	add    (%rax),%eax
+    646cb488:	or     %ebp,0x4(%rax)
+    646cb48b:	add    %al,(%rdx,%riz,4)
+	...
 
 00000000646cb490 <.xdata>:
-    646cb490:	add    %eax,(%rax)
-    646cb492:	add    %al,(%rax)
-    646cb494:	add    %ecx,(%rax)
-    646cb496:	add    $0x4420800,%eax
-    646cb49b:	xor    %al,(%rbx)
-    646cb49d:	(bad)
-    646cb49e:	add    0x1(%rax),%dh
-    646cb4a1:	push   %rax
-    646cb4a2:	add    %al,(%rax)
-    646cb4a4:	add    %eax,(%rdi)
-    646cb4a6:	add    $0x0,%al
-    646cb4a8:	(bad)
-    646cb4a9:	xor    (%rbx),%al
-    646cb4ab:	xor    %al,(%rdx)
-    646cb4ad:	(bad)
-    646cb4ae:	add    %esi,0x1(%rax)
-
-00000000646cb4b0 <.xdata>:
-    646cb4b0:	add    %eax,0x32050002(%rip)        # 9671b4b8 <.debug_str+0x320434b8>
-    646cb4b6:	add    %esi,(%rax)
+    646cb490:	add    %eax,0x52050002(%rip)        # b671b498 <.debug_str+0x52043498>
+    646cb496:	add    %esi,(%rax)
+
+00000000646cb498 <.xdata>:
+    646cb498:	add    %eax,(%rax)
+    646cb49a:	add    %al,(%rax)
+    646cb49c:	add    %ecx,(%rax)
+    646cb49e:	add    $0x4420800,%eax
+    646cb4a3:	xor    %al,(%rbx)
+    646cb4a5:	(bad)
+    646cb4a6:	add    0x1(%rax),%dh
+    646cb4a9:	push   %rax
+    646cb4aa:	add    %al,(%rax)
+    646cb4ac:	add    %eax,(%rdi)
+    646cb4ae:	add    $0x0,%al
+    646cb4b0:	(bad)
+    646cb4b1:	xor    (%rbx),%al
+    646cb4b3:	xor    %al,(%rdx)
+    646cb4b5:	(bad)
+    646cb4b6:	add    %esi,0x1(%rax)
 
 00000000646cb4b8 <.xdata>:
-    646cb4b8:	add    %eax,(%rcx,%rax,1)
-    646cb4bb:	add    %al,(%rdx,%riz,4)
-    646cb4be:	add    %al,(%rax)
-    646cb4c0:	add    %eax,(%rax)
-    646cb4c2:	add    %al,(%rax)
-    646cb4c4:	add    %edx,(%rsi)
-    646cb4c6:	or     %eax,(%rax)
-    646cb4c8:	(bad)
-    646cb4c9:	mov    %al,(%rsi)
-    646cb4cb:	add    %dl,(%rax)
-    646cb4cd:	js     646cb4d4 <.xdata+0x1c>
-    646cb4cf:	add    %cl,(%rbx)
-    646cb4d1:	push   $0xffffffffe2060004
-    646cb4d6:	add    (%rax),%dh
-    646cb4d8:	add    %esp,0x0(%rax)
+    646cb4b8:	add    %eax,0x32050002(%rip)        # 9671b4c0 <.debug_str+0x320434c0>
+    646cb4be:	add    %esi,(%rax)
+
+00000000646cb4c0 <.xdata>:
+    646cb4c0:	add    %eax,(%rcx,%rax,1)
+    646cb4c3:	add    %al,(%rdx,%riz,4)
+    646cb4c6:	add    %al,(%rax)
+    646cb4c8:	add    %eax,(%rax)
+    646cb4ca:	add    %al,(%rax)
+    646cb4cc:	add    %edx,(%rsi)
+    646cb4ce:	or     %eax,(%rax)
+    646cb4d0:	(bad)
+    646cb4d1:	mov    %al,(%rsi)
+    646cb4d3:	add    %dl,(%rax)
+    646cb4d5:	js     646cb4dc <.xdata+0x1c>
+    646cb4d7:	add    %cl,(%rbx)
+    646cb4d9:	push   $0xffffffffe2060004
+    646cb4de:	add    (%rax),%dh
+    646cb4e0:	add    %esp,0x0(%rax)
 	...
 
-00000000646cb4dc <.xdata.startup>:
-    646cb4dc:	add    %eax,(%rax)
+00000000646cb4e4 <.xdata.startup>:
+    646cb4e4:	add    %eax,(%rax)
 	...
 
 Disassembly of section .bss:
 
 00000000646cc000 <__bss_start__>:
 	...
 
 00000000646cc018 <__proc_attached>:
 	...
 
-00000000646cc020 <datacov>:
+00000000646cc020 <data_cov>:
 	...
 
 00000000646cc040 <pdist_temp>:
 	...
 
-00000000646cc060 <array2d_temp>:
+00000000646cc060 <distance_mat>:
 	...
 
 00000000646cc080 <weights>:
 	...
 
 00000000646cc0a0 <flatten_temp>:
 	...
 
-00000000646cc0c0 <loc_cov2>:
-	...
-
-00000000646cc0e0 <data_temp>:
+00000000646cc0c0 <location_cov2d>:
 	...
 
-00000000646cc100 <loc_cov>:
+00000000646cc0e0 <location_cov>:
 	...
 
-00000000646cc120 <location>:
+00000000646cc100 <location>:
 	...
 
-00000000646cc138 <kriging_var>:
+00000000646cc118 <kriging_var>:
 	...
 
-00000000646cc140 <estimation>:
+00000000646cc120 <estimation>:
 	...
 
-00000000646cc148 <k_range>:
+00000000646cc128 <k_range>:
 	...
 
-00000000646cc150 <model>:
+00000000646cc130 <model>:
 	...
 
-00000000646cc160 <count>:
-    646cc160:	add    %al,(%rax)
+00000000646cc140 <count>:
+    646cc140:	add    %al,(%rax)
 	...
 
-00000000646cc164 <flag>:
+00000000646cc144 <flag>:
 	...
 
-00000000646cc180 <_sampling>:
+00000000646cc160 <_sampling>:
 	...
 
-00000000646cc1d0 <sgsim_array>:
+00000000646cc1b0 <sgsim_array>:
 	...
 
-00000000646cc1f0 <variogram_array>:
+00000000646cc1d0 <variogram_array>:
 	...
 
-00000000646cc210 <x_grid>:
+00000000646cc1f0 <x_grid>:
 	...
 
-00000000646cc240 <initialized>:
+00000000646cc220 <initialized>:
 	...
 
-00000000646cc250 <.bss>:
+00000000646cc230 <.bss>:
 	...
 
-00000000646cc260 <GS_ContextRecord>:
+00000000646cc240 <GS_ContextRecord>:
 	...
 
-00000000646cc740 <GS_ExceptionRecord>:
+00000000646cc720 <GS_ExceptionRecord>:
 	...
 
-00000000646cc7e0 <mingw_initltssuo_force>:
-    646cc7e0:	add    %al,(%rax)
+00000000646cc7c0 <mingw_initltssuo_force>:
+    646cc7c0:	add    %al,(%rax)
 	...
 
-00000000646cc7e4 <mingw_initltsdyn_force>:
-    646cc7e4:	add    %al,(%rax)
+00000000646cc7c4 <mingw_initltsdyn_force>:
+    646cc7c4:	add    %al,(%rax)
 	...
 
-00000000646cc7e8 <mingw_initltsdrot_force>:
-    646cc7e8:	add    %al,(%rax)
+00000000646cc7c8 <mingw_initltsdrot_force>:
+    646cc7c8:	add    %al,(%rax)
 	...
 
-00000000646cc7ec <_tls_index>:
-    646cc7ec:	add    %al,(%rax)
+00000000646cc7cc <_tls_index>:
+    646cc7cc:	add    %al,(%rax)
 	...
 
-00000000646cc7f0 <mingw_app_type>:
+00000000646cc7d0 <mingw_app_type>:
 	...
 
-00000000646cc800 <was_init.95174>:
-    646cc800:	add    %al,(%rax)
+00000000646cc7e0 <was_init.95174>:
+    646cc7e0:	add    %al,(%rax)
 	...
 
-00000000646cc804 <maxSections>:
-    646cc804:	add    %al,(%rax)
+00000000646cc7e4 <maxSections>:
+    646cc7e4:	add    %al,(%rax)
 	...
 
-00000000646cc808 <the_secs>:
+00000000646cc7e8 <the_secs>:
 	...
 
-00000000646cc820 <__mingw_oldexcpt_handler>:
+00000000646cc800 <__mingw_oldexcpt_handler>:
 	...
 
-00000000646cc828 <was_here.95013>:
+00000000646cc808 <was_here.95013>:
 	...
 
-00000000646cc840 <emu_xdata>:
+00000000646cc820 <emu_xdata>:
 	...
 
-00000000646cc940 <emu_pdata>:
+00000000646cc920 <emu_pdata>:
 	...
 
-00000000646ccac0 <key_dtor_list>:
+00000000646ccaa0 <key_dtor_list>:
 	...
 
-00000000646ccac8 <__mingwthr_cs_init>:
+00000000646ccaa8 <__mingwthr_cs_init>:
 	...
 
-00000000646ccae0 <__mingwthr_cs>:
+00000000646ccac0 <__mingwthr_cs>:
 	...
 
-00000000646ccb20 <.bss>:
+00000000646ccb00 <.bss>:
 	...
 
-00000000646ccb30 <stUserMathErr>:
+00000000646ccb10 <stUserMathErr>:
 	...
 
-00000000646ccb40 <__native_startup_state>:
+00000000646ccb20 <__native_startup_state>:
 	...
 
-00000000646ccb48 <__native_startup_lock>:
+00000000646ccb28 <__native_startup_lock>:
 	...
 
 Disassembly of section .edata:
 
 00000000646cd000 <.edata>:
     646cd000:	add    %al,(%rax)
     646cd002:	add    %al,(%rax)
-    646cd004:	and    $0x64950c,%eax
-    646cd009:	add    %al,(%rax)
-    646cd00b:	add    %bl,0x10000d2(%rsi)
+    646cd004:	or     (%rax),%ecx
+    646cd006:	(bad)
+    646cd007:	add    %al,%fs:(%rax)
+    646cd00a:	add    %al,(%rax)
+    646cd00c:	sahf
+    646cd00d:	rolb   %cl,(%rax)
+    646cd00f:	add    %al,(%rcx)
     646cd011:	add    %al,(%rax)
     646cd013:	add    %bh,(%rdi)
     646cd015:	add    %al,(%rax)
     646cd017:	add    %bh,(%rdi)
     646cd019:	add    %al,(%rax)
     646cd01b:	add    %ch,(%rax)
     646cd01d:	rolb   (%rax)
     646cd01f:	add    %ah,(%rcx,%rdx,8)
     646cd022:	add    %al,(%rax)
     646cd024:	and    %dl,%dl
     646cd026:	add    %al,(%rax)
-    646cd028:	movabs 0xc000001630000047,%al
-    646cd031:	adc    $0x13b00000,%eax
-    646cd036:	add    %al,(%rax)
-    646cd038:	rex adc $0x20600000,%eax
-    646cd03e:	add    %al,(%rax)
-    646cd040:	rex and %al,(%rax)
-    646cd043:	add    %al,(%rax)
-    646cd045:	and    %al,(%rax)
-    646cd047:	add    %ah,(%rax)
-    646cd049:	and    %al,(%rax)
-    646cd04b:	add    %al,(%rax)
-    646cd04d:	sbb    (%rax),%eax
-    646cd04f:	add    %dh,(%rax)
-    646cd051:	sbb    (%rax),%al
-    646cd053:	add    %ah,0x50000016(%rax)
-    646cd059:	sbb    %eax,(%rax)
-    646cd05b:	add    %dh,(%rax)
+    646cd028:	xor    %al,0x0(%rsi)
+    646cd02b:	add    %dh,(%rax)
+    646cd02d:	(bad)
+    646cd02e:	add    %al,(%rax)
+    646cd030:	rclb   $0x0,0x13b00000(%rip)        # 781cd037 <.debug_str+0x13af5037>
+    646cd037:	add    %al,0x15(%rax)
+    646cd03a:	add    %al,(%rax)
+    646cd03c:	(bad)
+    646cd03d:	and    %al,(%rax)
+    646cd03f:	add    %al,0x20(%rax)
+    646cd042:	add    %al,(%rax)
+    646cd044:	add    %ah,(%rax)
+    646cd046:	add    %al,(%rax)
+    646cd048:	and    %ah,(%rax)
+    646cd04a:	add    %al,(%rax)
+    646cd04c:	add    %bl,(%rbx)
+    646cd04e:	add    %al,(%rax)
+    646cd050:	xor    %bl,(%rdx)
+    646cd052:	add    %al,(%rax)
+    646cd054:	movabs 0x3000001950000016,%al
     646cd05d:	(bad)
     646cd05e:	add    %al,(%rax)
     646cd060:	mov    $0x1e,%al
     646cd062:	add    %al,(%rax)
     646cd064:	mov    $0x1d,%al
     646cd066:	add    %al,(%rax)
     646cd068:	xor    %bl,(%rsi)
@@ -13044,67 +13067,64 @@
     646cd08b:	add    %dh,0x23(%rax)
     646cd08e:	add    %al,(%rax)
     646cd090:	rex and (%rax),%eax
     646cd093:	add    %ah,(%rax)
     646cd095:	and    (%rax),%eax
     646cd097:	add    %dh,(%rax)
     646cd099:	and    (%rax),%eax
-    646cd09b:	add    %dl,0x34(%rax)
+    646cd09b:	add    %ah,0x34(%rax)
     646cd09e:	add    %al,(%rax)
-    646cd0a0:	adc    %dh,0x34200000(%rip)        # 988cd0a6 <.debug_str+0x341f50a6>
+    646cd0a0:	and    %dh,0x46c00000(%rip)        # ab2cd0a6 <.debug_str+0x46bf50a6>
     646cd0a6:	add    %al,(%rax)
-    646cd0a8:	xor    %cl,0x0(%rax)
-    646cd0ab:	add    %dl,0x38(%rax)
-    646cd0ae:	add    %al,(%rax)
-    646cd0b0:	lock (bad)
-    646cd0b2:	add    %al,(%rax)
-    646cd0b4:	nop
-    646cd0b5:	ss add %al,(%rax)
-    646cd0b8:	and    %al,0x0(%rcx)
-    646cd0bb:	add    %dh,-0x7fffffbd(%rax)
-    646cd0c1:	ds add %al,(%rax)
-    646cd0c4:	push   %rax
-    646cd0c5:	rex.WX add %al,(%rax)
-    646cd0c8:	loopne 646cd0ed <.edata+0xed>
+    646cd0a8:	jo     646cd0e2 <.edata+0xe2>
+    646cd0aa:	add    %al,(%rax)
+    646cd0ac:	adc    %al,0x0(%rax)
+    646cd0af:	add    %ah,0x30000036(%rax)
+    646cd0b5:	add    %al,(%r8)
+    646cd0b8:	rolb   $0x0,0x0(%rbx)
+    646cd0bc:	movabs 0xe0000048e000003e,%al
+    646cd0c5:	and    (%rax),%eax
+    646cd0c7:	add    %al,0x2e(%rax)
     646cd0ca:	add    %al,(%rax)
-    646cd0cc:	rex
-    646cd0cd:	cs add %al,(%rax)
-    646cd0d0:	shlb   (%rax)
-    646cd0d2:	add    %al,(%rax)
-    646cd0d4:	lock sub %al,(%rax)
-    646cd0d7:	add    %al,0x6000002b(%rax)
-    646cd0dd:	es add %al,(%rax)
-    646cd0e0:	movabs 0x1000003390000023,%al
-    646cd0e9:	push   %rcx
-    646cd0ea:	add    %al,(%rax)
-    646cd0ec:	add    %cl,0x0(%rcx)
-    646cd0ef:	add    %ah,(%rax)
-    646cd0f1:	push   %rdx
-    646cd0f2:	add    %al,(%rax)
-    646cd0f4:	adcb   $0x0,0x0(%rcx)
-    646cd0f8:	rorb   $0x10,0x0(%rax,%rax,1)
+    646cd0cc:	shlb   (%rax)
+    646cd0ce:	add    %al,(%rax)
+    646cd0d0:	lock sub %al,(%rax)
+    646cd0d3:	add    %al,0x6000002b(%rax)
+    646cd0d9:	es add %al,(%rax)
+    646cd0dc:	movabs 0x5000003390000023,%al
+    646cd0e5:	push   %rax
+    646cd0e6:	add    %al,(%rax)
+    646cd0e8:	nop
+    646cd0e9:	rex.RXB add %r8b,(%r8)
+    646cd0ec:	(bad)
+    646cd0ed:	push   %rcx
+    646cd0ee:	add    %al,(%rax)
+    646cd0f0:	rclb   $0x0,0x0(%rax)
+    646cd0f4:	push   %rax
+    646cd0f5:	rex.WXB add %al,(%r8)
+    646cd0f8:	and    %dh,(%rsi)
+    646cd0fa:	add    %al,(%rax)
+    646cd0fc:	nop
     646cd0fd:	ss add %al,(%rax)
-    646cd100:	xorb   $0x0,(%rsi)
-    646cd103:	add    %al,0x4b(%rax)
-    646cd106:	add    %al,(%rax)
-    646cd108:	adc    %cl,0x0(%rbp)
-    646cd10b:	add    %dh,0x4d(%rax)
-    646cd10e:	add    %al,(%rax)
-    646cd110:	loopne 646cd162 <.edata+0x162>
-    646cd112:	add    %al,(%rax)
-    646cd114:	adc    %bh,(%rbx)
-    646cd116:	add    %al,(%rax)
-    646cd118:	lock push %rax
+    646cd100:	rorb   0x0(%rcx)
+    646cd103:	add    %ah,(%rax)
+    646cd105:	xor    $0x0,%al
+    646cd107:	add    %ah,0x4000004b(%rax)
+    646cd10d:	rex.WR add %r8b,(%rax)
+    646cd110:	and    %dl,0x0(%rax)
+    646cd113:	add    %dh,(%rax)
+    646cd115:	cmp    (%rax),%eax
+    646cd117:	add    %dh,(%rax)
+    646cd119:	push   %rax
     646cd11a:	add    %al,(%rax)
-    646cd11c:	rclb   $0xe0,0x0(%rax,%rax,1)
-    646cd121:	push   %rdx
-    646cd122:	add    %al,(%rax)
-    646cd124:	stos   %eax,%es:(%rdi)
-    646cd125:	rolb   %cl,(%rax)
-    646cd127:	add    %dh,-0x3affff2e(%rdx)
+    646cd11c:	add    %dl,0x0(%rax,%rax,1)
+    646cd120:	and    %dl,0x0(%rdx)
+    646cd123:	add    %ch,-0x4dffff2e(%rbx)
+    646cd129:	rolb   %cl,(%rax)
+    646cd12b:	add    %al,%ch
     646cd12d:	rolb   %cl,(%rax)
     646cd12f:	add    %dl,%bh
     646cd131:	rolb   %cl,(%rax)
     646cd133:	add    %ah,%bh
     646cd135:	rolb   %cl,(%rax)
     646cd137:	add    %bh,%ch
     646cd139:	rolb   %cl,(%rax)
@@ -13153,82 +13173,87 @@
     646cd192:	add    %al,(%rax)
     646cd194:	pushf
     646cd195:	(bad)
     646cd196:	add    %al,(%rax)
     646cd198:	test   $0xb30000d4,%eax
     646cd19d:	(bad)
     646cd19e:	add    %al,(%rax)
-    646cd1a0:	mov    $0xce0000d4,%edi
+    646cd1a0:	mov    $0xc80000d4,%edi
     646cd1a5:	(bad)
     646cd1a6:	add    %al,(%rax)
-    646cd1a8:	xlat   %ds:(%rbx)
+    646cd1a8:	(bad)
     646cd1a9:	(bad)
     646cd1aa:	add    %al,(%rax)
-    646cd1ac:	in     $0xd4,%eax
+    646cd1ac:	(bad)
+    646cd1ad:	(bad)
     646cd1ae:	add    %al,(%rax)
-    646cd1b0:	stc
-    646cd1b1:	(bad)
+    646cd1b0:	add    %dl,%ch
     646cd1b2:	add    %al,(%rax)
-    646cd1b4:	pmullw (%rax),%mm0
-    646cd1b7:	add    %ah,(%rax)
-    646cd1b9:	(bad)
+    646cd1b4:	adc    %edx,%ebp
+    646cd1b6:	add    %al,(%rax)
+    646cd1b8:	and    %ebp,%edx
     646cd1ba:	add    %al,(%rax)
-    646cd1bc:	xor    %ch,%dl
+    646cd1bc:	xor    $0xd5,%al
     646cd1be:	add    %al,(%rax)
-    646cd1c0:	rex.XB (bad)
+    646cd1c0:	(bad)
+    646cd1c1:	(bad)
     646cd1c2:	add    %al,(%rax)
-    646cd1c4:	rex.WRX (bad)
+    646cd1c4:	push   %rax
+    646cd1c5:	(bad)
     646cd1c6:	add    %al,(%rax)
-    646cd1c8:	pop    %rdi
-    646cd1c9:	(bad)
+    646cd1c8:	movsxd %ebp,%edx
     646cd1ca:	add    %al,(%rax)
-    646cd1cc:	jb     646cd1a3 <.edata+0x1a3>
+    646cd1cc:	jl     646cd1a3 <.edata+0x1a3>
     646cd1ce:	add    %al,(%rax)
-    646cd1d0:	mov    %ebp,%edx
+    646cd1d0:	mov    %ebp,%ss
     646cd1d2:	add    %al,(%rax)
-    646cd1d4:	popf
+    646cd1d4:	cmpsb  %es:(%rdi),%ds:(%rsi)
     646cd1d5:	(bad)
     646cd1d6:	add    %al,(%rax)
-    646cd1d8:	mov    $0xd5,%ch
-    646cd1da:	add    %al,(%rax)
-    646cd1dc:	int    $0xd5
+    646cd1d8:	mov    $0xcb0000d5,%esi
+    646cd1dd:	(bad)
     646cd1de:	add    %al,(%rax)
-    646cd1e0:	fcmovbe %st(5),%st
+    646cd1e0:	loope  646cd1b7 <.edata+0x1b7>
     646cd1e2:	add    %al,(%rax)
-    646cd1e4:	lock (bad)
+    646cd1e4:	in     (%dx),%eax
+    646cd1e5:	(bad)
     646cd1e6:	add    %al,(%rax)
-    646cd1e8:	cld
-    646cd1e9:	(bad)
+    646cd1e8:	repz (bad)
     646cd1ea:	add    %al,(%rax)
-    646cd1ec:	add    %dh,%dl
+    646cd1ec:	add    %edx,%esi
     646cd1ee:	add    %al,(%rax)
-    646cd1f0:	adc    %dl,%dh
-    646cd1f2:	add    %al,(%rax)
-    646cd1f4:	sbb    $0xd6,%al
+    646cd1f0:	or     $0x180000d6,%eax
+    646cd1f5:	(bad)
     646cd1f6:	add    %al,(%rax)
-    646cd1f8:	(bad)
-    646cd1f9:	(bad)
+    646cd1f8:	sub    $0xd6,%al
     646cd1fa:	add    %al,(%rax)
-    646cd1fc:	cmp    %esi,%edx
+    646cd1fc:	rex.X (bad)
     646cd1fe:	add    %al,(%rax)
-    646cd200:	push   %rcx
-    646cd201:	(bad)
+    646cd200:	rex.WRXB (bad)
     646cd202:	add    %al,(%rax)
-    646cd204:	pop    %rsi
-    646cd205:	(bad)
+    646cd204:	gs (bad)
     646cd206:	add    %al,(%rax)
-    646cd208:	imul   $0xd6730000,%esi,%edx
-    646cd20e:	add    %al,(%rax)
-    646cd210:	adc    $0x0,%dh
-    646cd213:	add    %cl,-0x67ffff2a(%rdi)
+    646cd208:	ja     646cd1e0 <.edata+0x1e0>
+    646cd20a:	add    %al,(%rax)
+    646cd20c:	adc    $0xd68e0000,%esi
+    646cd212:	add    %al,(%rax)
+    646cd214:	popf
+    646cd215:	(bad)
+    646cd216:	add    %al,(%rax)
+    646cd218:	cmpsb  %es:(%rdi),%ds:(%rsi)
     646cd219:	(bad)
     646cd21a:	add    %al,(%rax)
-    646cd21c:	movabs 0x2000100000000d6,%eax
-    646cd225:	add    %al,(%rbx)
-    646cd227:	add    %al,(%rax,%rax,1)
+    646cd21c:	scas   %es:(%rdi),%eax
+    646cd21d:	(bad)
+    646cd21e:	add    %al,(%rax)
+    646cd220:	add    %al,(%rax)
+    646cd222:	add    %eax,(%rax)
+    646cd224:	add    (%rax),%al
+    646cd226:	add    (%rax),%eax
+    646cd228:	add    $0x0,%al
     646cd22a:	add    $0x7000600,%eax
     646cd22f:	add    %cl,(%rax)
     646cd231:	add    %cl,(%rcx)
     646cd233:	add    %cl,(%rdx)
     646cd235:	add    %cl,(%rbx)
     646cd237:	add    %cl,(%rax,%rax,1)
     646cd23a:	or     $0xf000e00,%eax
@@ -13551,220 +13576,230 @@
     646cd4ae:	outsl  %ds:(%rsi),(%dx)
     646cd4af:	fs gs insb (%dx),%es:(%rdi)
     646cd4b2:	add    %ah,0x6f(%rbx)
     646cd4b5:	jbe    646cd516 <.edata+0x516>
     646cd4b7:	insl   (%dx),%es:(%rdi)
     646cd4b8:	outsl  %ds:(%rsi),(%dx)
     646cd4b9:	fs gs insb (%dx),%es:(%rdi)
-    646cd4bc:	xor    0x63(%rax,%rax,1),%ah
-    646cd4c0:	outsl  %ds:(%rsi),(%dx)
-    646cd4c1:	jbe    646cd522 <.edata+0x522>
-    646cd4c3:	insl   (%dx),%es:(%rdi)
-    646cd4c4:	outsl  %ds:(%rsi),(%dx)
-    646cd4c5:	fs gs insb (%dx),%es:(%rdi)
-    646cd4c8:	pop    %rdi
-    646cd4c9:	imul   $0x5f640074,0x69(%rsi),%ebp
-    646cd4d0:	(bad)
-    646cd4d1:	jb     646cd534 <.edata+0x534>
-    646cd4d3:	outsb  %ds:(%rsi),(%dx)
-    646cd4d4:	add    %ah,%gs:0x69(%esi)
-    646cd4d9:	outsb  %ds:(%rsi),(%dx)
-    646cd4da:	fs pop %rdi
-    646cd4dc:	outsb  %ds:(%rsi),(%dx)
-    646cd4dd:	imul   $0x726f62,%gs:0x68(%rdi),%esp
-    646cd4e5:	imul   $0x67,0x69(%rdx),%esi
-    646cd4e9:	imul   $0x6d656d5f,0x67(%rsi),%ebp
-    646cd4f0:	outsl  %ds:(%rsi),(%dx)
-    646cd4f1:	jb     646cd56c <.edata+0x56c>
-    646cd4f3:	pop    %rdi
-    646cd4f4:	data16 jb 646cd55c <.edata+0x55c>
-    646cd4f7:	add    %ch,%gs:0x72(%rbx)
-    646cd4fb:	imul   $0x705f676e,0x69(%rdi),%esp
-    646cd502:	(bad)
-    646cd503:	jb     646cd566 <.edata+0x566>
-    646cd505:	insl   (%dx),%es:(%rdi)
-    646cd506:	pop    %rdi
-    646cd507:	jae    646cd56e <.edata+0x56e>
-    646cd509:	je     646cd57f <.edata+0x57f>
-    646cd50b:	imul   $0x5f756c00,0x67(%rsi),%ebp
-    646cd512:	fs movsxd %gs:0x6d(%rdi),%ebp
-    646cd517:	jo     646cd588 <.edata+0x588>
-    646cd519:	jae    646cd584 <.edata+0x584>
-    646cd51b:	je     646cd586 <.edata+0x586>
-    646cd51d:	outsl  %ds:(%rsi),(%dx)
-    646cd51e:	outsb  %ds:(%rsi),(%dx)
-    646cd51f:	add    %ch,0x5f(%rbp,%rsi,2)
-    646cd523:	imul   $0x65737265,0x76(%rsi),%ebp
-    646cd52a:	pop    %rdi
-    646cd52b:	jae    646cd59c <.edata+0x59c>
-    646cd52d:	insb   (%dx),%es:(%rdi)
-    646cd52e:	jbe    646cd595 <.edata+0x595>
-    646cd530:	jb     646cd532 <.edata+0x532>
-    646cd532:	insl   (%dx),%es:(%rdi)
-    646cd533:	(bad)
-    646cd534:	je     646cd5a8 <.edata+0x5a8>
-    646cd536:	imul   $0x6d756761,0x5f(%rax),%edi
-    646cd53d:	outsb  %gs:(%rsi),(%dx)
-    646cd53f:	je     646cd5a6 <.edata+0x5a6>
-    646cd541:	add    %ch,%fs:0x61(%rbp)
-    646cd545:	je     646cd5b9 <.edata+0x5b9>
-    646cd547:	imul   $0x6d726f,0x66(%rax),%edi
-    646cd54e:	insl   (%dx),%es:(%rdi)
-    646cd54f:	je     646cd582 <.edata+0x582>
-    646cd551:	cmp    %edi,(%rcx)
-    646cd553:	xor    (%rdi),%esi
-    646cd555:	pop    %rdi
-    646cd556:	outsb  %gs:(%esi),(%dx)
-    646cd559:	gs jb  646cd5bd <.edata+0x5bd>
-    646cd55c:	je     646cd5c3 <.edata+0x5c3>
-    646cd55e:	add    %ch,0x74(%rbp)
-    646cd561:	xor    %edi,(%rcx)
-    646cd563:	cmp    %esi,(%rbx)
-    646cd565:	(bad)
-    646cd566:	pop    %rdi
-    646cd567:	addr32 gs je 646cd5ca <.edata+0x5ca>
-    646cd56b:	outsl  %fs:(%rsi),(%dx)
-    646cd56d:	jne    646cd5d1 <.edata+0x5d1>
-    646cd56f:	insb   (%dx),%es:(%rdi)
-    646cd570:	add    %ch,%gs:0x74(%rbp)
-    646cd574:	xor    %edi,(%rcx)
-    646cd576:	cmp    %esi,(%rbx)
-    646cd578:	(bad)
-    646cd579:	pop    %rdi
-    646cd57a:	addr32 gs je 646cd5dd <.edata+0x5dd>
-    646cd57e:	outsl  %fs:(%rsi),(%dx)
-    646cd580:	jne    646cd5e4 <.edata+0x5e4>
-    646cd582:	insb   (%dx),%es:(%rdi)
-    646cd583:	gs pop %rdi
-    646cd585:	jb     646cd5e8 <.edata+0x5e8>
-    646cd587:	outsb  %ds:(%rsi),(%dx)
-    646cd588:	add    %ch,%gs:0x74(%ebp)
-    646cd58d:	xor    %edi,(%rcx)
-    646cd58f:	cmp    %esi,(%rbx)
-    646cd591:	(bad)
-    646cd592:	pop    %rdi
-    646cd593:	addr32 gs je 646cd5f6 <.edata+0x5f6>
-    646cd597:	data16 insb (%dx),%es:(%rdi)
-    646cd599:	outsl  %ds:(%rsi),(%dx)
-    646cd59a:	(bad)
-    646cd59b:	je     646cd59d <.edata+0x59d>
-    646cd59d:	insl   (%dx),%es:(%rdi)
-    646cd59e:	je     646cd5d1 <.edata+0x5d1>
-    646cd5a0:	cmp    %edi,(%rcx)
-    646cd5a2:	xor    (%rdi),%esi
-    646cd5a4:	pop    %rdi
-    646cd5a5:	addr32 gs je 646cd608 <.edata+0x608>
-    646cd5a9:	data16 insb (%dx),%es:(%rdi)
-    646cd5ab:	outsl  %ds:(%rsi),(%dx)
+    646cd4bc:	xor    0x64(%rax,%rax,1),%ah
+    646cd4c0:	pop    %rdi
+    646cd4c1:	(bad)
+    646cd4c2:	jb     646cd525 <.edata+0x525>
+    646cd4c4:	outsb  %ds:(%rsi),(%dx)
+    646cd4c5:	add    %ah,%gs:0x69(%esi)
+    646cd4ca:	outsb  %ds:(%rsi),(%dx)
+    646cd4cb:	fs pop %rdi
+    646cd4cd:	outsb  %ds:(%rsi),(%dx)
+    646cd4ce:	imul   $0x726f62,%gs:0x68(%rdi),%esp
+    646cd4d6:	imul   $0x67,0x69(%rdx),%esi
+    646cd4da:	imul   $0x6d656d5f,0x67(%rsi),%ebp
+    646cd4e1:	outsl  %ds:(%rsi),(%dx)
+    646cd4e2:	jb     646cd55d <.edata+0x55d>
+    646cd4e4:	pop    %rdi
+    646cd4e5:	data16 jb 646cd54d <.edata+0x54d>
+    646cd4e8:	add    %ch,%gs:0x72(%rbx)
+    646cd4ec:	imul   $0x705f676e,0x69(%rdi),%esp
+    646cd4f3:	(bad)
+    646cd4f4:	jb     646cd557 <.edata+0x557>
+    646cd4f6:	insl   (%dx),%es:(%rdi)
+    646cd4f7:	pop    %rdi
+    646cd4f8:	jae    646cd55f <.edata+0x55f>
+    646cd4fa:	je     646cd570 <.edata+0x570>
+    646cd4fc:	imul   $0x5f756c00,0x67(%rsi),%ebp
+    646cd503:	fs movsxd %gs:0x6d(%rdi),%ebp
+    646cd508:	jo     646cd579 <.edata+0x579>
+    646cd50a:	jae    646cd575 <.edata+0x575>
+    646cd50c:	je     646cd577 <.edata+0x577>
+    646cd50e:	outsl  %ds:(%rsi),(%dx)
+    646cd50f:	outsb  %ds:(%rsi),(%dx)
+    646cd510:	add    %ch,0x5f(%rbp,%rsi,2)
+    646cd514:	imul   $0x65737265,0x76(%rsi),%ebp
+    646cd51b:	pop    %rdi
+    646cd51c:	jae    646cd58d <.edata+0x58d>
+    646cd51e:	insb   (%dx),%es:(%rdi)
+    646cd51f:	jbe    646cd586 <.edata+0x586>
+    646cd521:	jb     646cd523 <.edata+0x523>
+    646cd523:	insl   (%dx),%es:(%rdi)
+    646cd524:	(bad)
+    646cd525:	je     646cd599 <.edata+0x599>
+    646cd527:	imul   $0x6d756761,0x5f(%rax),%edi
+    646cd52e:	outsb  %gs:(%rsi),(%dx)
+    646cd530:	je     646cd597 <.edata+0x597>
+    646cd532:	add    %ch,%fs:0x61(%rbp)
+    646cd536:	je     646cd5aa <.edata+0x5aa>
+    646cd538:	imul   $0x6d726f,0x66(%rax),%edi
+    646cd53f:	insl   (%dx),%es:(%rdi)
+    646cd540:	je     646cd573 <.edata+0x573>
+    646cd542:	cmp    %edi,(%rcx)
+    646cd544:	xor    (%rdi),%esi
+    646cd546:	pop    %rdi
+    646cd547:	outsb  %gs:(%esi),(%dx)
+    646cd54a:	gs jb  646cd5ae <.edata+0x5ae>
+    646cd54d:	je     646cd5b4 <.edata+0x5b4>
+    646cd54f:	add    %ch,0x74(%rbp)
+    646cd552:	xor    %edi,(%rcx)
+    646cd554:	cmp    %esi,(%rbx)
+    646cd556:	(bad)
+    646cd557:	pop    %rdi
+    646cd558:	addr32 gs je 646cd5bb <.edata+0x5bb>
+    646cd55c:	outsl  %fs:(%rsi),(%dx)
+    646cd55e:	jne    646cd5c2 <.edata+0x5c2>
+    646cd560:	insb   (%dx),%es:(%rdi)
+    646cd561:	add    %ch,%gs:0x74(%rbp)
+    646cd565:	xor    %edi,(%rcx)
+    646cd567:	cmp    %esi,(%rbx)
+    646cd569:	(bad)
+    646cd56a:	pop    %rdi
+    646cd56b:	addr32 gs je 646cd5ce <.edata+0x5ce>
+    646cd56f:	outsl  %fs:(%rsi),(%dx)
+    646cd571:	jne    646cd5d5 <.edata+0x5d5>
+    646cd573:	insb   (%dx),%es:(%rdi)
+    646cd574:	gs pop %rdi
+    646cd576:	jb     646cd5d9 <.edata+0x5d9>
+    646cd578:	outsb  %ds:(%rsi),(%dx)
+    646cd579:	add    %ch,%gs:0x74(%ebp)
+    646cd57e:	xor    %edi,(%rcx)
+    646cd580:	cmp    %esi,(%rbx)
+    646cd582:	(bad)
+    646cd583:	pop    %rdi
+    646cd584:	addr32 gs je 646cd5e7 <.edata+0x5e7>
+    646cd588:	data16 insb (%dx),%es:(%rdi)
+    646cd58a:	outsl  %ds:(%rsi),(%dx)
+    646cd58b:	(bad)
+    646cd58c:	je     646cd58e <.edata+0x58e>
+    646cd58e:	insl   (%dx),%es:(%rdi)
+    646cd58f:	je     646cd5c2 <.edata+0x5c2>
+    646cd591:	cmp    %edi,(%rcx)
+    646cd593:	xor    (%rdi),%esi
+    646cd595:	pop    %rdi
+    646cd596:	addr32 gs je 646cd5f9 <.edata+0x5f9>
+    646cd59a:	data16 insb (%dx),%es:(%rdi)
+    646cd59c:	outsl  %ds:(%rsi),(%dx)
+    646cd59d:	(bad)
+    646cd59e:	je     646cd5ff <.edata+0x5ff>
+    646cd5a0:	jb     646cd603 <.edata+0x603>
+    646cd5a2:	outsb  %ds:(%rsi),(%dx)
+    646cd5a3:	add    %ch,%gs:0x74(%ebp)
+    646cd5a8:	xor    %edi,(%rcx)
+    646cd5aa:	cmp    %esi,(%rbx)
     646cd5ac:	(bad)
-    646cd5ad:	je     646cd60e <.edata+0x60e>
-    646cd5af:	jb     646cd612 <.edata+0x612>
-    646cd5b1:	outsb  %ds:(%rsi),(%dx)
-    646cd5b2:	add    %ch,%gs:0x74(%ebp)
-    646cd5b7:	xor    %edi,(%rcx)
-    646cd5b9:	cmp    %esi,(%rbx)
-    646cd5bb:	(bad)
-    646cd5bc:	pop    %rdi
-    646cd5bd:	addr32 gs je 646cd620 <.edata+0x620>
-    646cd5c1:	imul   $0x725f3233,0x74(%rsi),%ebp
-    646cd5c8:	(bad)
-    646cd5c9:	outsb  %ds:(%rsi),(%dx)
-    646cd5ca:	add    %ch,%gs:0x74(%ebp)
-    646cd5cf:	xor    %edi,(%rcx)
-    646cd5d1:	cmp    %esi,(%rbx)
-    646cd5d3:	(bad)
-    646cd5d4:	pop    %rdi
-    646cd5d5:	imul   $0x746d0074,0x69(%rsi),%ebp
-    646cd5dc:	xor    %edi,(%rcx)
-    646cd5de:	cmp    %esi,(%rbx)
-    646cd5e0:	(bad)
-    646cd5e1:	pop    %rdi
-    646cd5e2:	jb     646cd645 <.edata+0x645>
-    646cd5e4:	outsb  %ds:(%rsi),(%dx)
-    646cd5e5:	outsl  %fs:(%rsi),(%dx)
-    646cd5e7:	insl   (%dx),%es:(%rdi)
-    646cd5e8:	pop    %rdi
-    646cd5e9:	outsb  %ds:(%rsi),(%dx)
-    646cd5ea:	outsl  %ds:(%rsi),(%dx)
-    646cd5eb:	jb     646cd65a <.edata+0x65a>
-    646cd5ed:	(bad)
-    646cd5ee:	insb   (%dx),%es:(%rdi)
-    646cd5ef:	add    %dh,0x61(%rax)
-    646cd5f2:	jb     646cd668 <.edata+0x668>
-    646cd5f4:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
-    646cd5fc:	jo     646cd662 <.edata+0x662>
-    646cd5fe:	imul   $0x69757100,0x74(%rbx),%esi
-    646cd605:	movsxd 0x73(%rbx),%ebp
-    646cd608:	gs insb (%dx),%es:(%rdi)
-    646cd60a:	movsxd %gs:0x64(%rdx,%rsi,1),%esi
-    646cd60f:	add    %dh,0x75(%rcx)
-    646cd612:	imul   $0x74726f73,0x6b(%rbx),%esp
-    646cd619:	xor    0x72(%rax,%rax,1),%ah
-    646cd61d:	(bad)
-    646cd61e:	outsb  %ds:(%rsi),(%dx)
-    646cd61f:	outsl  %fs:(%rsi),(%dx)
-    646cd621:	insl   (%dx),%es:(%rdi)
-    646cd622:	jo     646cd685 <.edata+0x685>
-    646cd624:	je     646cd68e <.edata+0x68e>
-    646cd626:	add    %dh,0x61(%rbx)
-    646cd629:	insl   (%dx),%es:(%rdi)
-    646cd62a:	jo     646cd698 <.edata+0x698>
-    646cd62c:	imul   $0x6174735f,0x67(%rsi),%ebp
-    646cd633:	je     646cd69a <.edata+0x69a>
-    646cd635:	pop    %rdi
-    646cd636:	imul   $0x61730074,0x69(%rsi),%ebp
-    646cd63d:	insl   (%dx),%es:(%rdi)
-    646cd63e:	jo     646cd6ac <__bss_end__+0xb5c>
-    646cd640:	imul   $0x6174735f,0x67(%rsi),%ebp
-    646cd647:	je     646cd6ae <__bss_end__+0xb5e>
-    646cd649:	pop    %rdi
-    646cd64a:	jne    646cd6bc <__bss_end__+0xb6c>
-    646cd64c:	fs (bad)
-    646cd64e:	je     646cd6b5 <__bss_end__+0xb65>
-    646cd650:	add    %dh,0x61(%rbx)
-    646cd653:	jbe    646cd6ba <__bss_end__+0xb6a>
-    646cd655:	pop    %rdi
-    646cd656:	xor    %esp,0x72(%rcx,%riz,2)
-    646cd65a:	jb     646cd6bd <__bss_end__+0xb6d>
-    646cd65c:	jns    646cd65e <.edata+0x65e>
-    646cd65e:	jae    646cd6c7 <__bss_end__+0xb77>
-    646cd660:	jae    646cd6cb <__bss_end__+0xb7b>
-    646cd662:	insl   (%dx),%es:(%rdi)
-    646cd663:	pop    %rdi
-    646cd664:	imul   $0x67730074,0x69(%rsi),%ebp
-    646cd66b:	jae    646cd6d6 <__bss_end__+0xb86>
+    646cd5ad:	pop    %rdi
+    646cd5ae:	addr32 gs je 646cd611 <.edata+0x611>
+    646cd5b2:	imul   $0x725f3233,0x74(%rsi),%ebp
+    646cd5b9:	(bad)
+    646cd5ba:	outsb  %ds:(%rsi),(%dx)
+    646cd5bb:	add    %ch,%gs:0x74(%ebp)
+    646cd5c0:	xor    %edi,(%rcx)
+    646cd5c2:	cmp    %esi,(%rbx)
+    646cd5c4:	(bad)
+    646cd5c5:	pop    %rdi
+    646cd5c6:	imul   $0x746d0074,0x69(%rsi),%ebp
+    646cd5cd:	xor    %edi,(%rcx)
+    646cd5cf:	cmp    %esi,(%rbx)
+    646cd5d1:	(bad)
+    646cd5d2:	pop    %rdi
+    646cd5d3:	jb     646cd636 <.edata+0x636>
+    646cd5d5:	outsb  %ds:(%rsi),(%dx)
+    646cd5d6:	outsl  %fs:(%rsi),(%dx)
+    646cd5d8:	insl   (%dx),%es:(%rdi)
+    646cd5d9:	pop    %rdi
+    646cd5da:	outsb  %ds:(%rsi),(%dx)
+    646cd5db:	outsl  %ds:(%rsi),(%dx)
+    646cd5dc:	jb     646cd64b <.edata+0x64b>
+    646cd5de:	(bad)
+    646cd5df:	insb   (%dx),%es:(%rdi)
+    646cd5e0:	add    %dh,0x61(%rax)
+    646cd5e3:	jb     646cd659 <.edata+0x659>
+    646cd5e5:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
+    646cd5ed:	jo     646cd653 <.edata+0x653>
+    646cd5ef:	imul   $0x69757100,0x74(%rbx),%esi
+    646cd5f6:	movsxd 0x73(%rbx),%ebp
+    646cd5f9:	gs insb (%dx),%es:(%rdi)
+    646cd5fb:	movsxd %gs:0x64(%rdx,%rsi,1),%esi
+    646cd600:	add    %dh,0x75(%rcx)
+    646cd603:	imul   $0x74726f73,0x6b(%rbx),%esp
+    646cd60a:	xor    0x72(%rax,%rax,1),%ah
+    646cd60e:	(bad)
+    646cd60f:	outsb  %ds:(%rsi),(%dx)
+    646cd610:	outsl  %fs:(%rsi),(%dx)
+    646cd612:	insl   (%dx),%es:(%rdi)
+    646cd613:	jo     646cd676 <.edata+0x676>
+    646cd615:	je     646cd67f <.edata+0x67f>
+    646cd617:	add    %dh,0x61(%rbx)
+    646cd61a:	insl   (%dx),%es:(%rdi)
+    646cd61b:	jo     646cd689 <.edata+0x689>
+    646cd61d:	imul   $0x6174735f,0x67(%rsi),%ebp
+    646cd624:	je     646cd68b <.edata+0x68b>
+    646cd626:	pop    %rdi
+    646cd627:	imul   $0x61730074,0x69(%rsi),%ebp
+    646cd62e:	insl   (%dx),%es:(%rdi)
+    646cd62f:	jo     646cd69d <.edata+0x69d>
+    646cd631:	imul   $0x6174735f,0x67(%rsi),%ebp
+    646cd638:	je     646cd69f <.edata+0x69f>
+    646cd63a:	pop    %rdi
+    646cd63b:	jne    646cd6ad <.edata+0x6ad>
+    646cd63d:	fs (bad)
+    646cd63f:	je     646cd6a6 <.edata+0x6a6>
+    646cd641:	add    %dh,0x61(%rbx)
+    646cd644:	jbe    646cd6ab <.edata+0x6ab>
+    646cd646:	pop    %rdi
+    646cd647:	xor    %esp,0x72(%rcx,%riz,2)
+    646cd64b:	jb     646cd6ae <.edata+0x6ae>
+    646cd64d:	jns    646cd64f <.edata+0x64f>
+    646cd64f:	jae    646cd6b6 <.edata+0x6b6>
+    646cd651:	je     646cd6b2 <.edata+0x6b2>
+    646cd653:	movsxd 0x76(%rdi),%ebp
+    646cd656:	pop    %rdi
+    646cd657:	insl   (%dx),%es:(%rdi)
+    646cd658:	outsl  %ds:(%rsi),(%dx)
+    646cd659:	fs gs insb (%dx),%es:(%rdi)
+    646cd65c:	pop    %rdi
+    646cd65d:	fs gs data16 (bad)
+    646cd661:	jne    646cd6cf <__bss_end__+0xb9f>
+    646cd663:	je     646cd665 <.edata+0x665>
+    646cd665:	jae    646cd6cc <__bss_end__+0xb9c>
+    646cd667:	je     646cd6c8 <__bss_end__+0xb98>
+    646cd669:	jae    646cd6d2 <__bss_end__+0xba2>
+    646cd66b:	jae    646cd6d6 <__bss_end__+0xba6>
     646cd66d:	insl   (%dx),%es:(%rdi)
     646cd66e:	pop    %rdi
-    646cd66f:	jb     646cd6e6 <__bss_end__+0xb96>
-    646cd671:	outsb  %ds:(%rsi),(%dx)
-    646cd672:	add    %dh,0x67(%rbx)
-    646cd675:	jae    646cd6e0 <__bss_end__+0xb90>
-    646cd677:	insl   (%dx),%es:(%rdi)
-    646cd678:	pop    %rdi
-    646cd679:	je     646cd6da <__bss_end__+0xb8a>
-    646cd67b:	data16 jb 646cd6e3 <__bss_end__+0xb93>
-    646cd67e:	add    %dh,%gs:0x69(%rbx)
-    646cd682:	insl   (%dx),%es:(%rdi)
-    646cd683:	jo     646cd6f1 <__bss_end__+0xba1>
-    646cd685:	gs pop %rdi
-    646cd687:	imul   $0x67,0x69(%rdx),%esi
-    646cd68b:	imul   $0x61777300,0x67(%rsi),%ebp
-    646cd692:	jo     646cd706 <__bss_end__+0xbb6>
-    646cd694:	outsl  %ds:(%rsi),(%dx)
-    646cd695:	ja     646cd70a <__bss_end__+0xbba>
-    646cd697:	add    %dh,0x61(%rsi)
-    646cd69a:	jb     646cd705 <__bss_end__+0xbb5>
-    646cd69c:	(bad)
-    646cd69d:	outsb  %ds:(%rsi),(%dx)
-    646cd69e:	movsxd 0x0(%rbp),%esp
-    646cd6a1:	jbe    646cd704 <__bss_end__+0xbb4>
-    646cd6a3:	jb     646cd70e <__bss_end__+0xbbe>
-    646cd6a5:	outsl  %ds:(%rsi),(%dx)
-    646cd6a6:	addr32 jb 646cd70a <__bss_end__+0xbba>
-    646cd6a9:	insl   (%dx),%es:(%rdi)
+    646cd66f:	fs gs data16 (bad)
+    646cd673:	jne    646cd6e1 <__bss_end__+0xbb1>
+    646cd675:	je     646cd677 <.edata+0x677>
+    646cd677:	jae    646cd6e0 <__bss_end__+0xbb0>
+    646cd679:	jae    646cd6e4 <__bss_end__+0xbb4>
+    646cd67b:	insl   (%dx),%es:(%rdi)
+    646cd67c:	pop    %rdi
+    646cd67d:	jb     646cd6f4 <__bss_end__+0xbc4>
+    646cd67f:	outsb  %ds:(%rsi),(%dx)
+    646cd680:	add    %dh,0x67(%rbx)
+    646cd683:	jae    646cd6ee <__bss_end__+0xbbe>
+    646cd685:	insl   (%dx),%es:(%rdi)
+    646cd686:	pop    %rdi
+    646cd687:	je     646cd6e8 <__bss_end__+0xbb8>
+    646cd689:	data16 jb 646cd6f1 <__bss_end__+0xbc1>
+    646cd68c:	add    %dh,%gs:0x69(%rbx)
+    646cd690:	insl   (%dx),%es:(%rdi)
+    646cd691:	jo     646cd6ff <__bss_end__+0xbcf>
+    646cd693:	gs pop %rdi
+    646cd695:	imul   $0x67,0x69(%rdx),%esi
+    646cd699:	imul   $0x61777300,0x67(%rsi),%ebp
+    646cd6a0:	jo     646cd714 <__bss_end__+0xbe4>
+    646cd6a2:	outsl  %ds:(%rsi),(%dx)
+    646cd6a3:	ja     646cd718 <__bss_end__+0xbe8>
+    646cd6a5:	add    %dh,0x61(%rsi)
+    646cd6a8:	jb     646cd713 <__bss_end__+0xbe3>
+    646cd6aa:	(bad)
+    646cd6ab:	outsb  %ds:(%rsi),(%dx)
+    646cd6ac:	movsxd 0x0(%rbp),%esp
+    646cd6af:	jbe    646cd712 <__bss_end__+0xbe2>
+    646cd6b1:	jb     646cd71c <__bss_end__+0xbec>
+    646cd6b3:	outsl  %ds:(%rsi),(%dx)
+    646cd6b4:	addr32 jb 646cd718 <__bss_end__+0xbe8>
+    646cd6b7:	insl   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .idata:
 
 00000000646ce000 <_head_lib64_libkernel32_a>:
     646ce000:	cmp    $0xe0,%al
 	...
@@ -15047,22 +15082,20 @@
 00000000646cf020 <__xi_z>:
 	...
 
 00000000646cf028 <___crt_xi_end__>:
 	...
 
 00000000646cf030 <__xl_c>:
-    646cf030:	rcrb   $0x64,0x6c(%rax)
-    646cf034:	add    %al,(%rax)
+    646cf030:	add    %bl,0x6c(%rax)
+    646cf033:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf038 <__xl_d>:
-    646cf038:	nop
-    646cf039:	pop    %rax
-    646cf03a:	insb   (%dx),%es:(%rdi)
+    646cf038:	rclb   0x6c(%rdi)
     646cf03b:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf040 <__xl_z>:
 	...
 
 00000000646cf048 <___crt_xp_end__>:
@@ -15081,54 +15114,53 @@
 
 Disassembly of section .reloc:
 
 00000000646d1000 <.reloc>:
     646d1000:	add    %dh,0x0(%rax)
     646d1003:	add    %cl,(%rax,%rax,1)
     646d1006:	add    %al,(%rax)
-    646d1008:	rex.W scas %es:(%rdi),%al
-    646d100a:	add    %al,(%rax)
-    646d100c:	add    %al,0x140000(%rax)
+    646d1008:	mov    %ch,-0x80000000(%rbp)
+    646d100e:	add    %al,(%rax)
+    646d1010:	adc    $0x0,%al
     646d1012:	add    %al,(%rax)
     646d1014:	add    %ah,-0x5fa75fb0(%rax)
     646d101a:	(bad)
     646d101b:	movabs 0x90000000a070,%al
     646d1024:	xor    $0x0,%al
     646d1026:	add    %al,(%rax)
-    646d1028:	jo     646d0fcc <___tls_end__+0xfbc>
-    646d102a:	js     646d0fce <___tls_end__+0xfbe>
-    646d102c:	andb   $0xb0,-0x5d575d60(%rdx)
-    646d1033:	movabs %al,0xa6d0a6c0a6b0a2b8
-    646d103c:	loopne 646d0fe4 <___tls_end__+0xfd4>
-    646d103e:	lock cmpsb %es:(%rdi),%ds:(%rsi)
-    646d1040:	add    %ah,-0x58df58f0(%rdi)
-    646d1046:	xor    %ah,-0x58af58c0(%rdi)
-    646d104c:	(bad)
-    646d104d:	cmpsl  %es:(%rdi),%ds:(%rsi)
-    646d104e:	jo     646d0ff7 <___tls_end__+0xfe7>
-    646d1050:	andb   $0x0,-0x10000000(%rdi)
-    646d1057:	add    %dl,(%rax)
-    646d1059:	add    %al,(%rax)
-    646d105b:	add    %bl,(%rax)
-    646d105d:	.byte 0xa0
-    646d105e:	xor    %ah,0xa038(%rax)
+    646d1028:	nop
+    646d1029:	movabs %al,0xa2c8a2c0a2a0a298
+    646d1032:	shlb   -0x592f5d28(%rdx)
+    646d1038:	loopne 646d0fe0 <___tls_end__+0xfd0>
+    646d103a:	lock cmpsb %es:(%rdi),%ds:(%rsi)
+    646d103c:	add    %ah,-0x58df58f0(%rdi)
+    646d1042:	xor    %ah,-0x58af58c0(%rdi)
+    646d1048:	(bad)
+    646d1049:	cmpsl  %es:(%rdi),%ds:(%rsi)
+    646d104a:	jo     646d0ff3 <___tls_end__+0xfe3>
+    646d104c:	andb   $0x0,-0x585f5870(%rdi)
+    646d1053:	add    %al,(%rax)
+    646d1055:	lock add %al,(%rax)
+    646d1058:	adc    %al,(%rax)
+    646d105a:	add    %al,(%rax)
+    646d105c:	sbb    %ah,-0x5fc75fd0(%rax)
+	...
 
 Disassembly of section .debug_aranges:
 
 00000000646d2000 <.debug_aranges>:
     646d2000:	sub    $0x0,%al
     646d2002:	add    %al,(%rax)
     646d2004:	add    (%rax),%al
     646d2006:	add    %al,(%rax)
     646d2008:	add    %al,(%rax)
     646d200a:	or     %al,(%rax)
     646d200c:	add    %al,(%rax)
     646d200e:	add    %al,(%rax)
-    646d2010:	loopne 646d207a <.debug_aranges+0x4a>
-    646d2012:	insb   (%dx),%es:(%rdi)
+    646d2010:	and    %ch,0x6c(%rax)
     646d2013:	add    %al,%fs:(%rax)
     646d2016:	add    %al,(%rax)
     646d2018:	xor    (%rax),%al
 	...
 
 00000000646d2030 <.debug_aranges>:
     646d2030:	sbb    $0x0,%al
@@ -15145,20 +15177,19 @@
     646d3002:	add    %al,(%rax)
     646d3004:	add    (%rax),%al
     646d3006:	add    %al,(%rax)
     646d3008:	add    %al,(%rax)
     646d300a:	or     %al,(%rcx)
     646d300c:	add    %al,(%rax)
     646d300e:	add    %al,(%rax)
-    646d3010:	loopne 646d307a <.debug_info+0x4c>
-    646d3012:	insb   (%dx),%es:(%rdi)
+    646d3010:	and    %ch,0x6c(%rax)
     646d3013:	add    %al,%fs:(%rax)
     646d3016:	add    %al,(%rax)
-    646d3018:	adc    0x6c(%rcx),%ch
-    646d301b:	add    %al,%fs:(%rax)
+    646d3018:	push   %rdx
+    646d3019:	push   $0x646c
     646d301e:	add    %al,(%rax)
     646d3020:	add    %al,(%rax)
     646d3022:	add    %al,(%rax)
     646d3024:	cmp    %eax,(%rax)
     646d3026:	add    %al,(%rax)
     646d3028:	pop    (%rax)
     646d302a:	add    %al,(%rax)
@@ -19273,25 +19304,23 @@
     646d4ed8:	pop    %rdi
     646d4ed9:	add    %cl,(%rax,%rsi,1)
     646d4edc:	adc    %edi,0x0(%rsi,%rbx,1)
     646d4ee0:	add    %bl,(%rax)
     646d4ee2:	xchg   %ebx,(%rsi)
     646d4ee4:	add    %al,(%rax)
     646d4ee6:	or     $0x90a0939,%eax
-    646d4eeb:	add    0x7e(%rax),%eax
-    646d4eee:	insb   (%dx),%es:(%rdi)
-    646d4eef:	add    %al,%fs:(%rax)
-    646d4ef2:	add    %al,(%rax)
-    646d4ef4:	sbb    %bl,0xd00001e(%rbp)
-    646d4efa:	cmp    (%rcx),%cl
-    646d4efc:	or     (%rcx),%cl
-    646d4efe:	add    0x7e(%rax),%ebx
-    646d4f01:	insb   (%dx),%es:(%rdi)
-    646d4f02:	add    %al,%fs:(%rax)
-    646d4f05:	add    %al,(%rax)
+    646d4eeb:	add    0x646c7d(%rax),%eax
+    646d4ef1:	add    %al,(%rax)
+    646d4ef3:	add    %bl,(%rax)
+    646d4ef5:	popf
+    646d4ef6:	(bad)
+    646d4ef7:	add    %al,(%rax)
+    646d4ef9:	or     $0x90a093a,%eax
+    646d4efe:	add    0x646c7d(%rax),%ebx
+    646d4f04:	add    %al,(%rax)
 	...
 
 Disassembly of section .debug_abbrev:
 
 00000000646d5000 <.debug_abbrev>:
     646d5000:	add    %edx,(%rcx)
     646d5002:	add    %dl,(%rax)
@@ -19463,16 +19492,15 @@
     646d604f:	ja     646d60ba <.debug_line+0x3f>
     646d6051:	outsb  %ds:(%rsi),(%dx)
     646d6052:	cs push %rbx
     646d6054:	add    %al,(%rcx)
     646d6056:	add    %al,(%rax)
     646d6058:	add    %al,(%rax)
     646d605a:	or     %eax,(%rdx)
-    646d605c:	loopne 646d60c6 <.debug_line+0x4b>
-    646d605e:	insb   (%dx),%es:(%rdi)
+    646d605c:	and    %ch,0x6c(%rax)
     646d605f:	add    %al,%fs:(%rax)
     646d6062:	add    %al,(%rax)
     646d6064:	add    %esp,%esi
     646d6066:	add    %al,(%rcx)
     646d6068:	and    (%rdx),%ah
     646d606a:	addr32 pop %rcx
     646d606c:	xor    %dh,0x4b(%rbp)
@@ -19636,16 +19664,15 @@
     646d700d:	or     $0x7,%al
     646d700f:	or     %ah,0x1(%rax)
     646d7015:	add    %al,(%rax)
     646d7017:	add    %ch,(%rax,%rax,1)
     646d701a:	add    %al,(%rax)
     646d701c:	add    %al,(%rax)
     646d701e:	add    %al,(%rax)
-    646d7020:	loopne 646d708a <.debug_frame+0x8a>
-    646d7022:	insb   (%dx),%es:(%rdi)
+    646d7020:	and    %ch,0x6c(%rax)
     646d7023:	add    %al,%fs:(%rax)
     646d7026:	add    %al,(%rax)
     646d7028:	xor    (%rax),%al
     646d702a:	add    %al,(%rax)
     646d702c:	add    %al,(%rax)
     646d702e:	add    %al,(%rax)
     646d7030:	rex.B (bad)
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/cov_model/base.py` & `uc_sgsim-1.2.5/uc_sgsim/cov_model/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,24 +55,23 @@
             var[i] = self.model(x[i])
 
         return var
 
     def variogram(self, x: np.array) -> np.array:
         dist = cdist(x[:, :1], x[:, :1])
         variogram = []
-        # variogram = np.zeros(len(self.__bandwidth))
 
-        for idx, h in enumerate(self.__bandwidth):
+        for h in self.__bandwidth:
             indices = np.where(
                 (dist >= h - self.__bandwidth_step) & (dist <= h + self.__bandwidth_step),
             )
             z = np.power(x[indices[0], 1] - x[indices[1], 1], 2)
             z_sum = np.sum(z)
             if z_sum >= 1e-7:
                 variogram.append(z_sum / (2 * len(z)))
 
         return np.array(variogram)
 
     def variogram_plot(self, fig: int = None):
-        from ..plot.plot import Visualize
+        from ..plotting.sgsim_plot import SgsimPlot
 
-        Visualize(model=self).theory_variogram_plot(fig=fig)
+        SgsimPlot(model=self).theory_variogram_plot(fig=fig)
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/cov_model/model.py` & `uc_sgsim-1.2.5/uc_sgsim/cov_model/model.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.4/uc_sgsim/kriging/base.py` & `uc_sgsim-1.2.5/uc_sgsim/kriging/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.4/uc_sgsim/kriging/kriging.py` & `uc_sgsim-1.2.5/uc_sgsim/kriging/kriging.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,14 @@
         if kriging_var < 0:
             kriging_var = 0
 
         kriging_std = np.sqrt(kriging_var)
 
         return estimation, kriging_std
 
-    def matrix_agumented(self, mat):
+    def matrix_agumented(self, mat: np.array):
         ones_column = np.ones((mat.shape[0], 1))
         cov_data_augmented = np.hstack([mat, ones_column])
         ones_row = np.ones((1, cov_data_augmented.shape[1]))
         ones_row[0][-1] = 0
         cov_data_augmented = np.vstack((cov_data_augmented, ones_row))
         return cov_data_augmented
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/random_field.py` & `uc_sgsim-1.2.5/uc_sgsim/random_field.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from __future__ import annotations
+
 import numpy as np
+from uc_sgsim.plotting import SgsimPlot
 from uc_sgsim.exception import VariogramDoesNotCompute
+from uc_sgsim.kriging import SimpleKriging, OrdinaryKriging, Kriging
 from uc_sgsim.utils import save_as_multiple_file, save_as_one_file
 from uc_sgsim.cov_model.base import CovModel
 
 
 class RandomField:
     def __init__(self, x: int, realization_number: int):
         self.__realization_number = realization_number
@@ -89,25 +93,45 @@
                     file_type,
                     'Variogram',
                 )
         else:
             save_as_one_file(path, self.variogram)
 
 
-class SgsimField(RandomField):
+class SgsimField(RandomField, SgsimPlot):
     def __init__(
         self,
         x: int,
         realization_number: int,
         model: CovModel,
+        kriging: str | Kriging = 'SimpleKriging',
+        **kwargs,
     ):
-        super().__init__(x, realization_number)
+        RandomField.__init__(self, x, realization_number)
+        SgsimPlot.__init__(self, model)
+
         self.__model = model
         self.__bandwidth_step = model.bandwidth_step
         self.__bandwidth = model.bandwidth
+        self.__set_kriging_method(kriging)
+        self.__set_kwargs(**kwargs)
+
+    def __set_kriging_method(self, kriging) -> None:
+        if kriging == 'SimpleKriging':
+            self.kriging = SimpleKriging(self.model)
+        elif kriging == 'OrdinaryKriging':
+            self.kriging = OrdinaryKriging(self.model)
+        else:
+            if not isinstance(kriging, (SimpleKriging, OrdinaryKriging)):
+                raise TypeError('Kriging should be class SimpleKriging or OrdinaryKriging')
+
+    def __set_kwargs(self, **kwargs) -> None:
+        self.z_min = kwargs.get('z_min', -(self.model.sill**0.5 * 4))
+        self.z_max = kwargs.get('z_max', self.model.sill**0.5 * 4)
+        self.max_neigh = kwargs.get('max_neigh', 8)
 
     @property
     def model(self) -> CovModel:
         return self.__model
 
     @property
     def bandwidth(self) -> np.array:
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/sgsim.py` & `uc_sgsim-1.2.5/uc_sgsim/sgsim.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,46 +2,44 @@
 import sys
 from pathlib import Path
 from typing import Union
 from ctypes import CDLL, POINTER, c_double, c_int
 from multiprocessing import Pool
 
 import numpy as np
-from uc_sgsim.exception import VariogramDoesNotCompute
-from uc_sgsim.kriging import SimpleKriging, OrdinaryKriging, Kriging
+from uc_sgsim.kriging import Kriging
 from uc_sgsim.random_field import SgsimField
-from uc_sgsim.plot.plot import Visualize
 from uc_sgsim.cov_model.base import CovModel
 from uc_sgsim.utils import CovModelStructure, SgsimStructure
 
 BASE_DIR = Path(__file__).resolve().parent
 
 
 class UCSgsim(SgsimField):
     def __init__(
         self,
         x: int,
         model: CovModel,
         realization_number: int,
         kriging: Union[str, Kriging] = 'SimpleKriging',
+        **kwargs,
     ):
-        super().__init__(x, model, realization_number)
-        self.kriging = kriging
-        self.__set_kriging_method()
+        super().__init__(x, model, realization_number, kriging, **kwargs)
 
     def _process(self, randomseed: int = 0, parallel: bool = False) -> np.array:
         self.randomseed = randomseed
         if parallel is False:
             self.n_process = 1
 
         counts = 0
 
         start_time = time.time()
         np.random.seed(self.randomseed)
-        for _ in range(self.realization_number // self.n_process):
+        while counts < (self.realization_number // self.n_process):
+            drop = False
             unsampled = np.linspace(1, self.x_size - 2, self.x_size - 2)
             y_value = np.random.normal(0, self.model.sill**0.5, 2).reshape(2, 1)
             x_grid = np.array([0, self.x_size - 1]).reshape(2, 1)
             z = np.zeros(self.x_size)
             z[0], z[-1] = y_value[0], y_value[1]
             neigh = 0
 
@@ -55,24 +53,27 @@
 
             for i in range(len(unsampled)):
                 z[int(randompath[i])] = self.kriging.simulation(
                     grid,
                     randompath[i],
                     neighbor=neigh,
                 )
+                if z[int(randompath[i])] >= self.z_max or z[int(randompath[i])] <= self.z_min:
+                    drop = True
+                    break
                 temp = np.hstack([randompath[i], z[int(randompath[i])]])
                 grid = np.vstack([grid, temp])
 
-                if neigh < 8:
+                if neigh < self.max_neigh:
                     neigh += 1
 
             self.randomseed += 1
-
-            self.random_field[counts, :] = z
-            counts = counts + 1
+            if drop is False:
+                self.random_field[counts, :] = z
+                counts = counts + 1
             print('Progress = %.2f' % (counts / self.realization_number * 100) + '%', end='\r')
 
         print('Progress = %.2f' % 100 + '%\n', end='\r')
         end_time = time.time()
         print('Time = %f' % (end_time - start_time), 's\n')
 
         return self.random_field
@@ -109,59 +110,25 @@
         ]
         self.variogram = pool.starmap(self.model.variogram, zip(grid))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
         self.variogram = np.array(self.variogram)
 
-    def plot(self, realizations: list[int] = None, mean: float = 0):
-        plot = Visualize(self.model, self.random_field)
-        plot.plot(realizations, mean)
-
-    def mean_plot(self, mean: float = 0) -> None:
-        m_plot = Visualize(self.model, self.random_field)
-        m_plot.mean_plot(mean)
-
-    def variance_plot(self) -> None:
-        s_plot = Visualize(self.model, self.random_field)
-        s_plot.variance_plot()
-
-    def cdf_plot(self, x_location: int) -> None:
-        c_plot = Visualize(self.model, self.random_field)
-        c_plot.cdf_plot(x_location)
-
-    def hist_plot(self, x_location: int) -> None:
-        h_plot = Visualize(self.model, self.random_field)
-        h_plot.hist_plot(x_location)
-
-    def variogram_plot(self) -> None:
-        if type(self.variogram) == int:
-            raise VariogramDoesNotCompute()
-        v_plot = Visualize(self.model, self.random_field)
-        v_plot.variogram_plot(self.variogram)
-
-    def __set_kriging_method(self) -> None:
-        if self.kriging == 'SimpleKriging':
-            self.kriging = SimpleKriging(self.model)
-        elif self.kriging == 'OrdinaryKriging':
-            self.kriging = OrdinaryKriging(self.model)
-        else:
-            if not isinstance(self.kriging, (SimpleKriging, OrdinaryKriging)):
-                raise TypeError('Kriging should be class SimpleKriging or OrdinaryKriging')
-
 
 class UCSgsimDLL(UCSgsim):
     def __init__(
         self,
         x: int,
         model: CovModel,
         realization_number: int,
         kriging: str = 'SimpleKriging',
+        **kwargs,
     ):
-        super().__init__(x, model, realization_number)
+        super().__init__(x, model, realization_number, **kwargs)
         self.kriging = kriging
 
     def _lib_read(self) -> CDLL:
         if sys.platform.startswith('linux'):
             lib = CDLL(str(BASE_DIR) + r'/c_core/uc_sgsim.so')
         elif sys.platform.startswith('win32'):
             lib = CDLL(str(BASE_DIR) + r'/c_core/uc_sgsim.dll', winmode=0)
@@ -169,51 +136,40 @@
 
     def _cpdll(self, randomseed: int) -> np.array:
         lib = self._lib_read()
         mlen = int(self.x_size)
         realization_number = int(self.realization_number // self.n_process)
         random_field = np.empty([realization_number, self.x_size])
 
-        sgsim_init = lib.sgsim_init
-        sgsim_init.argtypes = (
-            POINTER(SgsimStructure),
-            c_int,
-            c_int,
-            c_int,
-            c_int,
-            c_int,
-        )
         kriging = 1 if self.kriging == 'OrdinaryKriging' else 0
-        sgsim_s = SgsimStructure()
-        sgsim_init(sgsim_s, mlen, realization_number, randomseed, kriging, 0)
-        sgsim_s.array = (c_double * (mlen * realization_number))()
-
-        cov_init = lib.cov_model_init
-        cov_s = CovModelStructure()
-        cov_init.argtypes = (
-            POINTER(CovModelStructure),
-            c_int,
-            c_int,
-            c_double,
-            c_double,
+        sgsim_s = SgsimStructure(
+            x_len=mlen,
+            realization_numbers=realization_number,
+            randomseed=randomseed,
+            kirging_method=kriging,
+            if_alloc_memory=0,
+            array=(c_double * (mlen * realization_number))(),
+            z_min=self.z_min,
+            z_max=self.z_max,
         )
-        cov_init(
-            cov_s,
-            self.model.bandwidth_len,
-            self.model.bandwidth_step,
-            self.model.k_range,
-            self.model.sill,
-            self.model.nugget,
+
+        cov_s = CovModelStructure(
+            bw_l=self.model.bandwidth_len,
+            bw_s=self.model.bandwidth_step,
+            bw=self.model.bandwidth_len // self.model.bandwidth_step,
+            max_neighbor=self.max_neigh,
+            range=self.model.k_range,
+            sill=self.model.sill,
+            nugget=self.model.nugget,
         )
 
         sgsim = lib.sgsim_run
         sgsim.argtypes = (POINTER(SgsimStructure), POINTER(CovModelStructure), c_int)
         sgsim(sgsim_s, cov_s, 0)
 
-        # array = as_array(sgsim_s.array, shape=(realization_number * mlen, 1))
         for i in range(realization_number):
             random_field[i, :] = sgsim_s.array[i * mlen : (i + 1) * mlen]
         return random_field
 
     def compute(self, n_process: int, randomseed: int) -> np.array:
         pool = Pool(processes=n_process)
         self.n_process = n_process
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim/utils.py` & `uc_sgsim-1.2.5/uc_sgsim/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,24 +31,28 @@
                     file=f,
                     end=end,
                 )
 
 
 class SgsimStructure(Structure):
     _fields_ = [
-        ('x_grid', c_int),
+        ('x_len', c_int),
         ('realization_numbers', c_int),
         ('randomseed', c_int),
         ('kriging_method', c_int),
-        ('vario_flag', c_int),
+        ('if_alloc_memory', c_int),
         ('array', POINTER(c_double)),
+        ('z_min', c_double),
+        ('z_max', c_double),
     ]
 
 
 class CovModelStructure(Structure):
     _fields_ = [
+        ('bw_l', c_int),
+        ('bw_s', c_int),
         ('bw', c_int),
-        ('hs', c_int),
+        ('max_neighbor', c_int),
         ('range', c_double),
         ('sill', c_double),
         ('nugget', c_double),
     ]
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim.egg-info/PKG-INFO` & `uc_sgsim-1.2.5/uc_sgsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc-sgsim
-Version: 1.2.4
+Version: 1.2.5
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -105,15 +105,15 @@
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
 * Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-## Example
+## Examples
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
@@ -128,14 +128,22 @@
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
     cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
+    # You could also set z_min, z_max and max_neighbor for sgsim by key words
+    # sgsim = uc.UCSgsimDLL(x, nR, cov_model, z_min=-6, z_max=6, max_neigh=10)
+    # set z_min, z_max and max_neighbor by directly assign
+    # sgsim.z_min = -6
+    # sgsim.z_max = 6
+    # sgsim.max_neigh = 10
+
+    # Create simulation with default z_min, z_max and max_neigh params
     sgsim_py = uc.UCSgsim(x, nR, cov_model) # run sgsim with python
     sgsim_c = uc.UCSgsimDLL(x, nR, cov_model) # run sgsim with c
 
     # Start compute with n CPUs
     sgsim_c.compute(n_process=2, randomseed=randomseed)
     sgsim_py.compute(n_process=2, randomseed=987654)
 
@@ -159,14 +167,56 @@
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
+If you would like to use pure C to run this code, you can modify the c_example.c file in this root directory. After modifying the c_example.c file, run ```sh cmake_build.sh``` on Linux or ```cmake_build.bat``` on Windows to compile and execute the code.
+
+```c
+// c_example.c
+# include <stdio.h>
+# include <stdlib.h>
+
+# include "./uc_sgsim/c_core/include/sgsim.h"
+# include "./uc_sgsim/c_core/include/cov_model.h"
+# if defined(__linux__) || defined(__unix__)
+# define PAUSE printf("Press Enter key to continue..."); fgetc(stdin);//NOLINT
+# elif _WIN32
+# define PAUSE system("PAUSE");
+# endif
+
+int main() {
+    // you can also set z_min and z_max at sgsim_t. Default value will depend on
+    // sill value in cov_model_t
+    sgsim_t sgsim_example = {
+        .x_len = 150,
+        .realization_numbers = 5,
+        .randomseed = 12345,
+        .kriging_method = 1,
+        .if_alloc_memory = 1,  // This should be equal to 1 if you want to run by c.
+    };
+
+    // you can also set max_negibor at cov_model_t. Defualt value is 4.
+    cov_model_t cov_example = {
+        .bw_l = 35,
+        .bw_s = 1,
+        .k_range = 17.32,
+        .sill = 1,
+        .nugget = 0,
+    };
+
+    sgsim_run(&sgsim_example, &cov_example, 0);
+    sgsim_t_free(&sgsim_example);
+    PAUSE
+    return 0;
+}
+```
+
 ## Future plans
 * 2D unconditional randomfield generation
 * GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
```

### Comparing `uc_sgsim-1.2.4/uc_sgsim.egg-info/SOURCES.txt` & `uc_sgsim-1.2.5/uc_sgsim.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 uc_sgsim/c_core/uc_sgsim.so
 uc_sgsim/cov_model/__init__.py
 uc_sgsim/cov_model/base.py
 uc_sgsim/cov_model/model.py
 uc_sgsim/kriging/__init__.py
 uc_sgsim/kriging/base.py
 uc_sgsim/kriging/kriging.py
-uc_sgsim/plot/__init__.py
-uc_sgsim/plot/base.py
-uc_sgsim/plot/plot.py
+uc_sgsim/plotting/__init__.py
+uc_sgsim/plotting/base.py
+uc_sgsim/plotting/sgsim_plot.py
```

