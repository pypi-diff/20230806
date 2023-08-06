# Comparing `tmp/syscolouringspackageV1-1.0.0.tar.gz` & `tmp/syscolouringspackageV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringspackageV1-1.0.0.tar", last modified: Sun Aug  6 14:39:41 2023, max compression
+gzip compressed data, was "syscolouringspackageV1-1.1.0.tar", last modified: Sun Aug  6 14:41:46 2023, max compression
```

## Comparing `syscolouringspackageV1-1.0.0.tar` & `syscolouringspackageV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:39:41.796823 syscolouringspackageV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-08-06 14:39:41.796823 syscolouringspackageV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:39:41.796823 syscolouringspackageV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:39:41.796823 syscolouringspackageV1-1.0.0/syscolouringspackageV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/syscolouringspackageV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:39:41.796823 syscolouringspackageV1-1.0.0/syscolouringspackageV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/syscolouringspackageV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/syscolouringspackageV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/syscolouringspackageV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-08-06 14:39:41.000000 syscolouringspackageV1-1.0.0/syscolouringspackageV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:41:46.860623 syscolouringspackageV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-08-06 14:41:46.860623 syscolouringspackageV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:41:46.864623 syscolouringspackageV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:41:46.856624 syscolouringspackageV1-1.1.0/syscolouringspackageV1/
+-rw-r--r--   0 root         (0) root         (0)    96645 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/syscolouringspackageV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:41:46.860623 syscolouringspackageV1-1.1.0/syscolouringspackageV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/syscolouringspackageV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/syscolouringspackageV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/syscolouringspackageV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-06 14:41:46.000000 syscolouringspackageV1-1.1.0/syscolouringspackageV1.egg-info/top_level.txt
```

### Comparing `syscolouringspackageV1-1.0.0/setup.py` & `syscolouringspackageV1-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull tweak package"
 LONG_DESCRIPTION = "Usefull tweak package"
 
 # Setting up
 setup(
     name="syscolouringspackageV1",
     version=VERSION,
```

