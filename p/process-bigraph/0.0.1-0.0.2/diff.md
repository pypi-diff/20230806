# Comparing `tmp/process-bigraph-0.0.1.tar.gz` & `tmp/process-bigraph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-bigraph-0.0.1.tar", last modified: Wed May 17 16:11:35 2023, max compression
+gzip compressed data, was "process-bigraph-0.0.2.tar", last modified: Sun Aug  6 16:12:49 2023, max compression
```

## Comparing `process-bigraph-0.0.1.tar` & `process-bigraph-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-17 16:11:35.134801 process-bigraph-0.0.1/
--rw-r--r--   0 eranagmon   (502) staff       (20)     1400 2023-05-17 16:11:35.134677 process-bigraph-0.0.1/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)      484 2023-05-17 16:02:25.000000 process-bigraph-0.0.1/README.md
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-17 16:11:35.133621 process-bigraph-0.0.1/process_bigraph/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2023-05-17 15:56:41.000000 process-bigraph-0.0.1/process_bigraph/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     8772 2023-05-17 15:56:41.000000 process-bigraph-0.0.1/process_bigraph/composite.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-17 16:11:35.134449 process-bigraph-0.0.1/process_bigraph.egg-info/
--rw-r--r--   0 eranagmon   (502) staff       (20)     1400 2023-05-17 16:11:35.000000 process-bigraph-0.0.1/process_bigraph.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)      269 2023-05-17 16:11:35.000000 process-bigraph-0.0.1/process_bigraph.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-05-17 16:11:35.000000 process-bigraph-0.0.1/process_bigraph.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       15 2023-05-17 16:11:35.000000 process-bigraph-0.0.1/process_bigraph.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       16 2023-05-17 16:11:35.000000 process-bigraph-0.0.1/process_bigraph.egg-info/top_level.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-05-17 16:11:35.134846 process-bigraph-0.0.1/setup.cfg
--rw-r--r--   0 eranagmon   (502) staff       (20)     1639 2023-05-17 16:02:59.000000 process-bigraph-0.0.1/setup.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-06 16:12:49.646236 process-bigraph-0.0.2/
+-rw-r--r--   0 eranagmon   (502) staff       (20)      143 2023-06-07 17:02:47.000000 process-bigraph-0.0.2/AUTHORS.md
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11358 2023-06-07 17:02:15.000000 process-bigraph-0.0.2/LICENSE
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3896 2023-08-06 16:12:49.646128 process-bigraph-0.0.2/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2933 2023-06-07 17:02:15.000000 process-bigraph-0.0.2/README.md
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-06 16:12:49.645029 process-bigraph-0.0.2/process_bigraph/
+-rw-r--r--   0 eranagmon   (502) staff       (20)      109 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    16602 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/composite.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-06 16:12:49.645924 process-bigraph-0.0.2/process_bigraph/experiments/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/experiments/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5354 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/experiments/minimal_gillespie.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      976 2023-07-14 17:11:01.000000 process-bigraph-0.0.2/process_bigraph/protocol.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3111 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/tests.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5565 2023-08-06 16:09:52.000000 process-bigraph-0.0.2/process_bigraph/type_system.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-08-06 16:12:49.645689 process-bigraph-0.0.2/process_bigraph.egg-info/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3896 2023-08-06 16:12:49.000000 process-bigraph-0.0.2/process_bigraph.egg-info/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)      461 2023-08-06 16:12:49.000000 process-bigraph-0.0.2/process_bigraph.egg-info/SOURCES.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-08-06 16:12:49.000000 process-bigraph-0.0.2/process_bigraph.egg-info/dependency_links.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       15 2023-08-06 16:12:49.000000 process-bigraph-0.0.2/process_bigraph.egg-info/requires.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       16 2023-08-06 16:12:49.000000 process-bigraph-0.0.2/process_bigraph.egg-info/top_level.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-08-06 16:12:49.646275 process-bigraph-0.0.2/setup.cfg
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1639 2023-08-06 16:10:29.000000 process-bigraph-0.0.2/setup.py
```

### Comparing `process-bigraph-0.0.1/setup.py` & `process-bigraph-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
     # Patch the relative links to absolute URLs that will work on PyPI.
     description2 = re.sub(
         r']\(([\w/.-]+\.png)\)',
```

