# Comparing `tmp/tensorflow-ml-1.0.4.tar.gz` & `tmp/tensorflow-ml-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-ml-1.0.4.tar", last modified: Sun Aug  6 18:13:08 2023, max compression
+gzip compressed data, was "tensorflow-ml-1.1.tar", last modified: Sun Aug  6 21:04:02 2023, max compression
```

## Comparing `tensorflow-ml-1.0.4.tar` & `tensorflow-ml-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:13:08.674019 tensorflow-ml-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-06 18:10:43.000000 tensorflow-ml-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-06 18:13:08.674019 tensorflow-ml-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-08-06 18:10:43.000000 tensorflow-ml-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:13:08.674019 tensorflow-ml-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-06 18:10:43.000000 tensorflow-ml-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:13:08.674019 tensorflow-ml-1.0.4/tensorflow_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-06 18:10:43.000000 tensorflow-ml-1.0.4/tensorflow_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:13:08.674019 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-06 18:13:08.000000 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-06 18:13:08.000000 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:13:08.000000 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-06 18:13:08.000000 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 18:13:08.000000 tensorflow-ml-1.0.4/tensorflow_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/tensorflow_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-06 21:01:34.000000 tensorflow-ml-1.1/tensorflow_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:04:02.706984 tensorflow-ml-1.1/tensorflow_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-06 21:04:02.000000 tensorflow-ml-1.1/tensorflow_ml.egg-info/top_level.txt
```

### Comparing `tensorflow-ml-1.0.4/LICENSE` & `tensorflow-ml-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-ml-1.0.4/setup.py` & `tensorflow-ml-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0.4' 
+VERSION = '1.1' 
+
 DESCRIPTION = 'Tensorflow ML'
-LONG_DESCRIPTION = 'An abstract implementation of commonly used machine learning algorithms using TensorFlow 2.0'
+
+with open("README.md", 'r') as f:
+    LONG_DESCRIPTION = f.read()
 
 lib_folder = os.path.dirname(os.path.realpath(__file__))
 requirement_path = f"{lib_folder}/requirements.txt"
-install_requires = [] # Here we'll add: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
+install_requires = [] 
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
 
-# Setting up
 setup(
-       # the name must match the folder name 'verysimplemodule'
         name="tensorflow-ml", 
         version=VERSION,
         author="Siddhant Pathak",
         author_email="siddhantpathak2@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
+        long_description_content_type="text/markdown",  # Specify the type of markup used in README.md
         packages=find_packages(),
-        install_requires=install_requires, # add any additional packages that 
-        # needs to be installed along with your package. Eg: 'caer'
-        
-        keywords=['python', 'tensorflow', 'ml'],
+        install_requires=install_requires,        
+        keywords=['python', 'tensorflow', 'ml', 'keras'],
         classifiers= [
-            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: POSIX :: Linux",
         ]
 )
```

### Comparing `tensorflow-ml-1.0.4/tensorflow_ml.egg-info/requires.txt` & `tensorflow-ml-1.1/tensorflow_ml.egg-info/requires.txt`

 * *Files identical despite different names*

