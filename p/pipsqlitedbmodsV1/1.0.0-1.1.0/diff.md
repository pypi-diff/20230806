# Comparing `tmp/pipsqlitedbmodsV1-1.0.0.tar.gz` & `tmp/pipsqlitedbmodsV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlitedbmodsV1-1.0.0.tar", last modified: Sun Aug  6 15:57:01 2023, max compression
+gzip compressed data, was "pipsqlitedbmodsV1-1.1.0.tar", last modified: Sun Aug  6 15:59:07 2023, max compression
```

## Comparing `pipsqlitedbmodsV1-1.0.0.tar` & `pipsqlitedbmodsV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:57:01.425360 pipsqlitedbmodsV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:57:01.421360 pipsqlitedbmodsV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:57:01.421360 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 15:57:00.000000 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:57:01.421360 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:57:01.000000 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-08-06 15:57:01.000000 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:57:01.000000 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-06 15:57:01.000000 pipsqlitedbmodsV1-1.0.0/pipsqlitedbmodsV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:57:01.425360 pipsqlitedbmodsV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-08-06 15:57:00.000000 pipsqlitedbmodsV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:59:07.300875 pipsqlitedbmodsV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:59:07.296875 pipsqlitedbmodsV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:59:07.296875 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1/
+-rw-r--r--   0 root         (0) root         (0)    96645 2023-08-06 15:59:06.000000 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:59:07.296875 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:59:07.000000 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-08-06 15:59:07.000000 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:59:07.000000 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-06 15:59:07.000000 pipsqlitedbmodsV1-1.1.0/pipsqlitedbmodsV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:59:07.300875 pipsqlitedbmodsV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-06 15:59:06.000000 pipsqlitedbmodsV1-1.1.0/setup.py
```

### Comparing `pipsqlitedbmodsV1-1.0.0/setup.py` & `pipsqlitedbmodsV1-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pipsqlitedbmodsV1",
     version=VERSION,
```

