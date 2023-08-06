# Comparing `tmp/pythoncryptokitV2-1.0.0.tar.gz` & `tmp/pythoncryptokitV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncryptokitV2-1.0.0.tar", last modified: Sun Aug  6 15:34:35 2023, max compression
+gzip compressed data, was "pythoncryptokitV2-1.1.0.tar", last modified: Sun Aug  6 15:36:40 2023, max compression
```

## Comparing `pythoncryptokitV2-1.0.0.tar` & `pythoncryptokitV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:34:35.110762 pythoncryptokitV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:34:35.106762 pythoncryptokitV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:34:35.106762 pythoncryptokitV2-1.0.0/pythoncryptokitV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 15:34:34.000000 pythoncryptokitV2-1.0.0/pythoncryptokitV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:34:35.106762 pythoncryptokitV2-1.0.0/pythoncryptokitV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:34:35.000000 pythoncryptokitV2-1.0.0/pythoncryptokitV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-08-06 15:34:35.000000 pythoncryptokitV2-1.0.0/pythoncryptokitV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:34:35.000000 pythoncryptokitV2-1.0.0/pythoncryptokitV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-08-06 15:34:35.000000 pythoncryptokitV2-1.0.0/pythoncryptokitV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:34:35.110762 pythoncryptokitV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-08-06 15:34:34.000000 pythoncryptokitV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:36:39.998355 pythoncryptokitV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:36:39.998355 pythoncryptokitV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:36:39.998355 pythoncryptokitV2-1.1.0/pythoncryptokitV2/
+-rw-r--r--   0 root         (0) root         (0)    96645 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/pythoncryptokitV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:36:39.998355 pythoncryptokitV2-1.1.0/pythoncryptokitV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/pythoncryptokitV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/pythoncryptokitV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/pythoncryptokitV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/pythoncryptokitV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:36:39.998355 pythoncryptokitV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-06 15:36:39.000000 pythoncryptokitV2-1.1.0/setup.py
```

### Comparing `pythoncryptokitV2-1.0.0/setup.py` & `pythoncryptokitV2-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pythoncryptokitV2",
     version=VERSION,
```

