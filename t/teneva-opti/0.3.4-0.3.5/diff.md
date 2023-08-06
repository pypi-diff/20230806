# Comparing `tmp/teneva_opti-0.3.4.tar.gz` & `tmp/teneva_opti-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_opti-0.3.4.tar", last modified: Fri Aug  4 14:23:27 2023, max compression
+gzip compressed data, was "teneva_opti-0.3.5.tar", last modified: Sun Aug  6 14:01:08 2023, max compression
```

## Comparing `teneva_opti-0.3.4.tar` & `teneva_opti-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.819507 teneva_opti-0.3.4/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.4/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.4/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-04 14:23:27.819646 teneva_opti-0.3.4/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1923 2023-08-04 14:22:51.000000 teneva_opti-0.3.4/README.md
--rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-04 12:11:01.000000 teneva_opti-0.3.4/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-04 11:56:04.000000 teneva_opti-0.3.4/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-04 14:23:27.820145 teneva_opti-0.3.4/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.4/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.812004 teneva_opti-0.3.4/teneva_opti/
--rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-04 14:22:30.000000 teneva_opti-0.3.4/teneva_opti/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7856 2023-08-04 14:18:29.000000 teneva_opti-0.3.4/teneva_opti/bm_view.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.814038 teneva_opti-0.3.4/teneva_opti/func/
--rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.4/teneva_opti/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6795 2023-08-04 13:52:05.000000 teneva_opti-0.3.4/teneva_opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      171 2023-08-04 11:59:34.000000 teneva_opti-0.3.4/teneva_opti/opti_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     6992 2023-08-04 13:39:55.000000 teneva_opti-0.3.4/teneva_opti/opti_manager.py
--rw-r--r--   0 andrei     (501) staff       (20)     2357 2023-08-04 13:41:01.000000 teneva_opti-0.3.4/teneva_opti/opti_tens.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.819229 teneva_opti-0.3.4/teneva_opti/tens/
--rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.4/teneva_opti/tens/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)     2393 2023-08-04 13:57:19.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1586 2023-08-04 13:43:52.000000 teneva_opti-0.3.4/teneva_opti/tens/opti_tens_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.4/teneva_opti/utils.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-04 14:23:27.813697 teneva_opti-0.3.4/teneva_opti.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3198 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      763 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      137 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-04 14:23:27.000000 teneva_opti-0.3.4/teneva_opti.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 14:01:08.646023 teneva_opti-0.3.5/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:48:03.000000 teneva_opti-0.3.5/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 15:33:45.000000 teneva_opti-0.3.5/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-06 14:01:08.646145 teneva_opti-0.3.5/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2168 2023-08-06 14:00:39.000000 teneva_opti-0.3.5/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)     1244 2023-08-04 12:11:01.000000 teneva_opti-0.3.5/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-06 12:29:21.000000 teneva_opti-0.3.5/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-06 14:01:08.646676 teneva_opti-0.3.5/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2538 2023-08-02 09:28:28.000000 teneva_opti-0.3.5/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 14:01:08.638325 teneva_opti-0.3.5/teneva_opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      191 2023-08-06 14:00:46.000000 teneva_opti-0.3.5/teneva_opti/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7856 2023-08-04 14:18:29.000000 teneva_opti-0.3.5/teneva_opti/bm_view.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 14:01:08.640881 teneva_opti-0.3.5/teneva_opti/func/
+-rw-r--r--   0 andrei     (501) staff       (20)        0 2023-07-31 13:03:34.000000 teneva_opti-0.3.5/teneva_opti/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6846 2023-08-06 13:11:44.000000 teneva_opti-0.3.5/teneva_opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      171 2023-08-04 11:59:34.000000 teneva_opti-0.3.5/teneva_opti/opti_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7059 2023-08-06 13:25:00.000000 teneva_opti-0.3.5/teneva_opti/opti_manager.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2359 2023-08-06 13:12:12.000000 teneva_opti-0.3.5/teneva_opti/opti_tens.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 14:01:08.645531 teneva_opti-0.3.5/teneva_opti/tens/
+-rw-r--r--   0 andrei     (501) staff       (20)      344 2023-08-01 16:02:13.000000 teneva_opti-0.3.5/teneva_opti/tens/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:41.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      391 2023-08-01 15:57:39.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1129 2023-08-02 14:22:34.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-08-01 15:57:37.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2393 2023-08-04 13:57:19.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      377 2023-08-01 15:57:35.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      381 2023-08-01 15:57:33.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1586 2023-08-04 13:43:52.000000 teneva_opti-0.3.5/teneva_opti/tens/opti_tens_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2367 2023-08-02 13:40:17.000000 teneva_opti-0.3.5/teneva_opti/utils.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 14:01:08.640533 teneva_opti-0.3.5/teneva_opti.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3443 2023-08-06 14:01:08.000000 teneva_opti-0.3.5/teneva_opti.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      763 2023-08-06 14:01:08.000000 teneva_opti-0.3.5/teneva_opti.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-06 14:01:08.000000 teneva_opti-0.3.5/teneva_opti.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       95 2023-08-06 14:01:08.000000 teneva_opti-0.3.5/teneva_opti.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       12 2023-08-06 14:01:08.000000 teneva_opti-0.3.5/teneva_opti.egg-info/top_level.txt
```

### Comparing `teneva_opti-0.3.4/LICENSE.txt` & `teneva_opti-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/PKG-INFO` & `teneva_opti-0.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_opti
-Version: 0.3.4
+Version: 0.3.5
 Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
 Home-page: https://github.com/AndreiChertkov/teneva_opti
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
 Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
@@ -30,33 +30,36 @@
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.4".
+1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
+    ```bash
+    pip install teneva_opti==0.3.5
+    ```
+    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
+
+2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
+    ```bash
+    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
+    ```
+    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
 
-The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
 
-We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
-```bash
-wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
-```
-
-> In the case of problems with `scikit-learn`, uninstall it `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
+## Documentation and examples (in progress...)
 
-
-## Documentation and examples (TODO)
-
-Please, run the demo script:
+Please, run the demo script from the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository:
 ```bash
 clear && python demo.py
 ```
 
+> See also other `demo_*.py` scripts in the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository.
+
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_opti-0.3.4/README.md` & `teneva_opti-0.3.5/teneva_opti.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,65 @@
+Metadata-Version: 2.1
+Name: teneva-opti
+Version: 0.3.5
+Summary: Collection of various optimization methods, including tensor based, for multivariate functions and multidimensional data arrays
+Home-page: https://github.com/AndreiChertkov/teneva_opti
+Author: Andrei Chertkov
+Author-email: andre.chertkov@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/AndreiChertkov/teneva_opti
+Keywords: optimization method multidimensional array multivariate function tensor train nevergrad cma ttopt protes genetic algorithm evolutionary strategy
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # teneva_opti
 
 
 ## Description
 
 Collection of various optimization methods (search for the global minimum and/or maximum) for multivariate functions and multidimensional data arrays (tensors). This library is based on a software product [teneva](https://github.com/AndreiChertkov/teneva). See also related benchmarks library [teneva_bm](https://github.com/AndreiChertkov/teneva_bm).
 
 
 ## Installation
 
-> Current version "0.3.4".
-
-The package can be installed via pip: `pip install teneva_opti` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and installed by `python setup.py install` command from the root folder of the project.
+1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
+    ```bash
+    pip install teneva_opti==0.3.5
+    ```
+    > The package can be also downloaded from the repository [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) and be installed by `python setup.py install` command from the root folder of the project.
+
+2. We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym`, `mujoco`, etc.), please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
+    ```bash
+    wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py && python install_all.py --env teneva_opti && rm install_all.py
+    ```
+    > In the case of problems with `scikit-learn`, uninstall it as `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
 
-We test optimizers with benchmarks from [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) library. For installation of additional dependencies (`gym` and `mujoco`) for `agent` collection , please, do the following (for existing conda environment `teneva_opti`; if you are using a different environment name, then please make the appropriate substitution in the script):
-```bash
-wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_mujoco.py && python install_mujoco.py --env teneva_opti && rm install_mujoco.py
-```
 
-> In the case of problems with `scikit-learn`, uninstall it `pip uninstall scikit-learn` and then install it from the anaconda: `conda install -c anaconda scikit-learn`.
+## Documentation and examples (in progress...)
 
-
-## Documentation and examples (TODO)
-
-Please, run the demo script:
+Please, run the demo script from the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository:
 ```bash
 clear && python demo.py
 ```
 
+> See also other `demo_*.py` scripts in the root of the [teneva_opti](https://github.com/AndreiChertkov/teneva_opti) repository.
+
 
 ## Authors
 
 - [Andrei Chertkov](https://github.com/AndreiChertkov)
 - [Gleb Ryzhakov](https://github.com/G-Ryzhakov)
 - [Ivan Oseledets](https://github.com/oseledets)
```

### Comparing `teneva_opti-0.3.4/demo.py` & `teneva_opti-0.3.5/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/setup.py` & `teneva_opti-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti/bm_view.py` & `teneva_opti-0.3.5/teneva_opti/bm_view.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti/opti.py` & `teneva_opti-0.3.5/teneva_opti/opti.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         self.log.info(self.info() + '\n' + self.bm.info())
 
         self.is_fail = False
 
         try:
             self._optimize()
         except Exception as e:
+            # TODO: add error message into history
             self.is_fail = True
             msg = f'Optimization with "{self.name}" is failed [{e}]'
             self.log.err(msg) if with_err else self.log.wrn(msg)
 
         self.log.info(self.bm.info_history())
 
     def render(self, fpath=None, with_wrn=True):
```

### Comparing `teneva_opti-0.3.4/teneva_opti/opti_manager.py` & `teneva_opti-0.3.5/teneva_opti/opti_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
             # Create Bm class instance:
             Bm = task['bm']
             args = task.get('bm_args', {})
             bm = Bm(**args)
             if 'bm_opts' in task:
                 bm.set_opts(**task['bm_opts'])
             if 'bm_seed' in task:
+                # TODO: seed should be the argument of bm.__init__
                 bm.set_seed(task['bm_seed'])
 
             # Create Opti class instance:
             Opti = task['opti']
             args = task.get('opti_args', {})
             args = self.build_args(args, bm)
             opti = Opti(**args)
```

### Comparing `teneva_opti-0.3.4/teneva_opti/opti_tens.py` & `teneva_opti-0.3.5/teneva_opti/opti_tens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import nevergrad as ng
 import numpy as np
+
+
 from teneva_opti import Opti
 
 
 class OptiTens(Opti):
     @property
     def d_inner(self):
         if self.with_quan:
```

### Comparing `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_optimatt.py` & `teneva_opti-0.3.5/teneva_opti/tens/opti_tens_optimatt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_protes.py` & `teneva_opti-0.3.5/teneva_opti/tens/opti_tens_protes.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti/tens/opti_tens_ttopt.py` & `teneva_opti-0.3.5/teneva_opti/tens/opti_tens_ttopt.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti/utils.py` & `teneva_opti-0.3.5/teneva_opti/utils.py`

 * *Files identical despite different names*

### Comparing `teneva_opti-0.3.4/teneva_opti.egg-info/SOURCES.txt` & `teneva_opti-0.3.5/teneva_opti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

