# Comparing `tmp/pyortho-0.0.4.tar.gz` & `tmp/pyortho-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyortho-0.0.4.tar", last modified: Mon Mar 20 02:22:10 2023, max compression
+gzip compressed data, was "pyortho-0.0.5.tar", last modified: Sun Aug  6 14:57:16 2023, max compression
```

## Comparing `pyortho-0.0.4.tar` & `pyortho-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-03-20 02:22:10.535124 pyortho-0.0.4/
--rw-r--r--   0 chenyk     (501) staff       (20)    35149 2023-03-20 02:20:34.000000 pyortho-0.0.4/LICENSE
--rw-r--r--   0 chenyk     (501) staff       (20)     1208 2023-03-20 02:22:10.534646 pyortho-0.0.4/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      188 2023-03-20 02:20:34.000000 pyortho-0.0.4/README.md
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-03-20 02:22:10.530981 pyortho-0.0.4/pyortho/
--rw-r--r--   0 chenyk     (501) staff       (20)     1121 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/__init__.py
--rw-r--r--   0 chenyk     (501) staff       (20)     9794 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/divne.py
--rw-r--r--   0 chenyk     (501) staff       (20)     5166 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/drr3d.py
--rw-r--r--   0 chenyk     (501) staff       (20)     2912 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/localortho.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1891 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/localsimi.py
--rw-r--r--   0 chenyk     (501) staff       (20)     1105 2023-03-20 02:21:20.000000 pyortho-0.0.4/pyortho/snr.py
-drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-03-20 02:22:10.534071 pyortho-0.0.4/pyortho.egg-info/
--rw-r--r--   0 chenyk     (501) staff       (20)     1208 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/PKG-INFO
--rw-r--r--   0 chenyk     (501) staff       (20)      322 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/SOURCES.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/dependency_links.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/not-zip-safe
--rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/requires.txt
--rw-r--r--   0 chenyk     (501) staff       (20)        8 2023-03-20 02:22:10.000000 pyortho-0.0.4/pyortho.egg-info/top_level.txt
--rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-03-20 02:22:10.535277 pyortho-0.0.4/setup.cfg
--rw-r--r--   0 chenyk     (501) staff       (20)     1873 2023-03-20 02:21:48.000000 pyortho-0.0.4/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-08-06 14:57:16.331567 pyortho-0.0.5/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2023-08-06 02:41:09.000000 pyortho-0.0.5/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1164 2023-08-06 14:57:16.331050 pyortho-0.0.5/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     3727 2023-08-06 02:41:09.000000 pyortho-0.0.5/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-08-06 14:57:16.325634 pyortho-0.0.5/pyortho/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1191 2023-08-06 14:24:45.000000 pyortho-0.0.5/pyortho/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9794 2023-08-06 02:41:09.000000 pyortho-0.0.5/pyortho/divne.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     5166 2023-08-06 02:41:09.000000 pyortho-0.0.5/pyortho/drr3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     3798 2023-08-06 14:49:27.000000 pyortho-0.0.5/pyortho/localortho.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2483 2023-08-06 14:57:00.000000 pyortho-0.0.5/pyortho/localsimi.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1105 2023-08-06 02:41:09.000000 pyortho-0.0.5/pyortho/snr.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-08-06 14:57:16.330286 pyortho-0.0.5/pyortho/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    23404 2023-08-06 14:55:20.000000 pyortho-0.0.5/pyortho/src/orthocfuns.c
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-08-06 14:57:16.329888 pyortho-0.0.5/pyortho.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1164 2023-08-06 14:57:16.000000 pyortho-0.0.5/pyortho.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      347 2023-08-06 14:57:16.000000 pyortho-0.0.5/pyortho.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-08-06 14:57:16.000000 pyortho-0.0.5/pyortho.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-08-06 03:20:16.000000 pyortho-0.0.5/pyortho.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-08-06 14:57:16.000000 pyortho-0.0.5/pyortho.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       18 2023-08-06 14:57:16.000000 pyortho-0.0.5/pyortho.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-08-06 14:57:16.331725 pyortho-0.0.5/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     1974 2023-08-06 14:56:33.000000 pyortho-0.0.5/setup.py
```

### Comparing `pyortho-0.0.4/LICENSE` & `pyortho-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyortho-0.0.4/PKG-INFO` & `pyortho-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyortho
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for local signal-and-noise orthogonalization and local similarity calculation
 Home-page: https://github.com/aaspip/pyortho
 Author: pyortho developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
-Keywords: seismology,exploration seismology,array seismology,denoising,science,orthogonalization,local orthogonalization,local similarity,signal-to-noise ratio,damped rank reduction method
+Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
```

### Comparing `pyortho-0.0.4/pyortho/__init__.py` & `pyortho-0.0.5/pyortho/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 # Add formatter
 FORMAT = "[%(asctime)s] - %(name)s - %(levelname)s: %(message)s"
 formatter = logging.Formatter(FORMAT)
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 from .localortho import localortho
+from .localortho import localorthoc
 from .localsimi import localsimi
+from .localsimi import localsimic
 from .divne import divne
 from .drr3d import drr3d
 from .snr import snr
```

### Comparing `pyortho-0.0.4/pyortho/divne.py` & `pyortho-0.0.5/pyortho/divne.py`

 * *Files identical despite different names*

### Comparing `pyortho-0.0.4/pyortho/drr3d.py` & `pyortho-0.0.5/pyortho/drr3d.py`

 * *Files identical despite different names*

### Comparing `pyortho-0.0.4/pyortho/snr.py` & `pyortho-0.0.5/pyortho/snr.py`

 * *Files identical despite different names*

### Comparing `pyortho-0.0.4/pyortho.egg-info/PKG-INFO` & `pyortho-0.0.5/pyortho.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyortho
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for local signal-and-noise orthogonalization and local similarity calculation
 Home-page: https://github.com/aaspip/pyortho
 Author: pyortho developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
-Keywords: seismology,exploration seismology,array seismology,denoising,science,orthogonalization,local orthogonalization,local similarity,signal-to-noise ratio,damped rank reduction method
+Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
```

### Comparing `pyortho-0.0.4/setup.py` & `pyortho-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 #!/usr/bin/env python
 # -*- encoding: utf8 -*-
-import glob
-import inspect
 import io
 import os
 
-from setuptools import find_packages
 from setuptools import setup
+from distutils.core import Extension
+import numpy
 
 
 long_description = """
 Source code: https://github.com/aaspip/pyortho""".strip() 
 
+
 def read(*names, **kwargs):
     return io.open(
         os.path.join(os.path.dirname(__file__), *names),
         encoding=kwargs.get("encoding", "utf8")).read()
 
+orthoc_module = Extension('orthocfun', sources=['pyortho/src/orthocfuns.c'], 
+										include_dirs=[numpy.get_include()])
+
 setup(
     name="pyortho",
-    version="0.0.4",
+    version="0.0.5",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="A python package for local signal-and-noise orthogonalization and local similarity calculation",
     long_description=long_description,
     author="pyortho developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyortho",
+    ext_modules=[orthoc_module],
     packages=['pyortho'],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
@@ -40,15 +44,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     keywords=[
-        "seismology", "exploration seismology", "array seismology", "denoising", "science", "orthogonalization", "local orthogonalization", "local similarity", "signal-to-noise ratio", "damped rank reduction method"
+        "seismology", "earthquake seismology", "exploration seismology", "array seismology", "denoising", "science", "engineering", "structure", "local slope", "filtering"
     ],
     install_requires=[
         "numpy", "scipy", "matplotlib"
     ],
     extras_require={
         "docs": ["sphinx", "ipython", "runipy"]
     }
```

