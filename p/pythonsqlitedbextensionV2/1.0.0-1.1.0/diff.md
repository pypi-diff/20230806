# Comparing `tmp/pythonsqlitedbextensionV2-1.0.0.tar.gz` & `tmp/pythonsqlitedbextensionV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqlitedbextensionV2-1.0.0.tar", last modified: Sun Aug  6 13:12:19 2023, max compression
+gzip compressed data, was "pythonsqlitedbextensionV2-1.1.0.tar", last modified: Sun Aug  6 13:14:25 2023, max compression
```

## Comparing `pythonsqlitedbextensionV2-1.0.0.tar` & `pythonsqlitedbextensionV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:12:19.762652 pythonsqlitedbextensionV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-08-06 13:12:19.758652 pythonsqlitedbextensionV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:12:19.758652 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:12:19.758652 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/pythonsqlitedbextensionV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 13:12:19.762652 pythonsqlitedbextensionV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-08-06 13:12:19.000000 pythonsqlitedbextensionV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:14:25.610231 pythonsqlitedbextensionV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-08-06 13:14:25.610231 pythonsqlitedbextensionV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:14:25.606232 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2/
+-rw-r--r--   0 root         (0) root         (0)    96645 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 13:14:25.606232 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/pythonsqlitedbextensionV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 13:14:25.610231 pythonsqlitedbextensionV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-08-06 13:14:25.000000 pythonsqlitedbextensionV2-1.1.0/setup.py
```

### Comparing `pythonsqlitedbextensionV2-1.0.0/setup.py` & `pythonsqlitedbextensionV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="pythonsqlitedbextensionV2",
     version=VERSION,
```

