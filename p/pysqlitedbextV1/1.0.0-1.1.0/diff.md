# Comparing `tmp/pysqlitedbextV1-1.0.0.tar.gz` & `tmp/pysqlitedbextV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlitedbextV1-1.0.0.tar", last modified: Sun Aug  6 14:19:48 2023, max compression
+gzip compressed data, was "pysqlitedbextV1-1.1.0.tar", last modified: Sun Aug  6 14:21:54 2023, max compression
```

## Comparing `pysqlitedbextV1-1.0.0.tar` & `pysqlitedbextV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:19:48.504318 pysqlitedbextV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-06 14:19:48.504318 pysqlitedbextV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:19:48.500318 pysqlitedbextV1-1.0.0/pysqlitedbextV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/pysqlitedbextV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:19:48.504318 pysqlitedbextV1-1.0.0/pysqlitedbextV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/pysqlitedbextV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/pysqlitedbextV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/pysqlitedbextV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/pysqlitedbextV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:19:48.504318 pysqlitedbextV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      556 2023-08-06 14:19:48.000000 pysqlitedbextV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:21:54.243885 pysqlitedbextV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-06 14:21:54.243885 pysqlitedbextV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:21:54.239885 pysqlitedbextV1-1.1.0/pysqlitedbextV1/
+-rw-r--r--   0 root         (0) root         (0)    96645 2023-08-06 14:21:53.000000 pysqlitedbextV1-1.1.0/pysqlitedbextV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:21:54.239885 pysqlitedbextV1-1.1.0/pysqlitedbextV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-06 14:21:54.000000 pysqlitedbextV1-1.1.0/pysqlitedbextV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-08-06 14:21:54.000000 pysqlitedbextV1-1.1.0/pysqlitedbextV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:21:54.000000 pysqlitedbextV1-1.1.0/pysqlitedbextV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-06 14:21:54.000000 pysqlitedbextV1-1.1.0/pysqlitedbextV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:21:54.243885 pysqlitedbextV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      556 2023-08-06 14:21:53.000000 pysqlitedbextV1-1.1.0/setup.py
```

### Comparing `pysqlitedbextV1-1.0.0/setup.py` & `pysqlitedbextV1-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pysqlitedbextV1",
     version=VERSION,
```

