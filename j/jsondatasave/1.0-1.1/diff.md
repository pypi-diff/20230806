# Comparing `tmp/jsondatasave-1.0.tar.gz` & `tmp/jsondatasave-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsondatasave-1.0.tar", last modified: Sun Aug  6 08:26:11 2023, max compression
+gzip compressed data, was "jsondatasave-1.1.tar", last modified: Sun Aug  6 08:57:22 2023, max compression
```

## Comparing `jsondatasave-1.0.tar` & `jsondatasave-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:26:11.200288 jsondatasave-1.0/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)     1017 2023-08-06 08:26:11.200162 jsondatasave-1.0/PKG-INFO
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      511 2023-08-06 07:27:42.000000 jsondatasave-1.0/README.md
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:26:11.199233 jsondatasave-1.0/jsondatasave/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       32 2023-08-06 02:27:43.000000 jsondatasave-1.0/jsondatasave/__init__.py
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      256 2023-08-06 02:26:38.000000 jsondatasave-1.0/jsondatasave/datasave.py
-drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:26:11.199911 jsondatasave-1.0/jsondatasave.egg-info/
--rw-r--r--   0 andrewzhuang   (501) staff       (20)     1017 2023-08-06 08:26:11.000000 jsondatasave-1.0/jsondatasave.egg-info/PKG-INFO
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      212 2023-08-06 08:26:11.000000 jsondatasave-1.0/jsondatasave.egg-info/SOURCES.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)        1 2023-08-06 08:26:11.000000 jsondatasave-1.0/jsondatasave.egg-info/dependency_links.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-06 08:26:11.000000 jsondatasave-1.0/jsondatasave.egg-info/top_level.txt
--rw-r--r--   0 andrewzhuang   (501) staff       (20)       38 2023-08-06 08:26:11.200345 jsondatasave-1.0/setup.cfg
--rw-r--r--   0 andrewzhuang   (501) staff       (20)      931 2023-08-06 08:26:01.000000 jsondatasave-1.0/setup.py
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:57:22.029060 jsondatasave-1.1/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     1971 2023-08-06 08:57:22.028930 jsondatasave-1.1/PKG-INFO
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     1512 2023-08-06 08:37:40.000000 jsondatasave-1.1/README.md
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:57:22.028019 jsondatasave-1.1/jsondatasave/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       32 2023-08-06 02:27:43.000000 jsondatasave-1.1/jsondatasave/__init__.py
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      256 2023-08-06 02:26:38.000000 jsondatasave-1.1/jsondatasave/datasave.py
+drwxr-xr-x   0 andrewzhuang   (501) staff       (20)        0 2023-08-06 08:57:22.028675 jsondatasave-1.1/jsondatasave.egg-info/
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)     1971 2023-08-06 08:57:22.000000 jsondatasave-1.1/jsondatasave.egg-info/PKG-INFO
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      212 2023-08-06 08:57:22.000000 jsondatasave-1.1/jsondatasave.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)        1 2023-08-06 08:57:22.000000 jsondatasave-1.1/jsondatasave.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       13 2023-08-06 08:57:22.000000 jsondatasave-1.1/jsondatasave.egg-info/top_level.txt
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)       38 2023-08-06 08:57:22.029112 jsondatasave-1.1/setup.cfg
+-rw-r--r--   0 andrewzhuang   (501) staff       (20)      884 2023-08-06 08:56:23.000000 jsondatasave-1.1/setup.py
```

### Comparing `jsondatasave-1.0/setup.py` & `jsondatasave-1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '1.0'
+VERSION = '1.1'
 DESCRIPTION = 'Facilitating the process to store JSON data'
 
 with open("README.md", 'r') as r:
     long_description = r.read()
 
 # Setting up
 setup(
@@ -17,14 +17,13 @@
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[],  # Review if 'hashl' is truly needed
     keywords=['python', 'JSON', 'Data Storage'],  # Adjusted the keywords to be more representative
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     license="MIT"
 )
```

