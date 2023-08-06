# Comparing `tmp/cerberuspy-1.0.0.tar.gz` & `tmp/cerberuspy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerberuspy-1.0.0.tar", last modified: Sat Aug  5 20:32:50 2023, max compression
+gzip compressed data, was "cerberuspy-1.0.1.tar", last modified: Sun Aug  6 17:55:07 2023, max compression
```

## Comparing `cerberuspy-1.0.0.tar` & `cerberuspy-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-05 20:32:50.825430 cerberuspy-1.0.0/
--rw-r--r--   0 avate     (1000) avate     (1000)      190 2023-08-05 20:32:50.825430 cerberuspy-1.0.0/PKG-INFO
-drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-05 20:32:50.821430 cerberuspy-1.0.0/cerberuspy/
--rw-r--r--   0 avate     (1000) avate     (1000)       27 2023-08-03 14:36:51.000000 cerberuspy-1.0.0/cerberuspy/__init__.py
--rw-r--r--   0 avate     (1000) avate     (1000)      714 2023-08-05 19:49:34.000000 cerberuspy-1.0.0/cerberuspy/client.py
-drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-05 20:32:50.825430 cerberuspy-1.0.0/cerberuspy.egg-info/
--rw-r--r--   0 avate     (1000) avate     (1000)      190 2023-08-05 20:32:50.000000 cerberuspy-1.0.0/cerberuspy.egg-info/PKG-INFO
--rw-r--r--   0 avate     (1000) avate     (1000)      198 2023-08-05 20:32:50.000000 cerberuspy-1.0.0/cerberuspy.egg-info/SOURCES.txt
--rw-r--r--   0 avate     (1000) avate     (1000)        1 2023-08-05 20:32:50.000000 cerberuspy-1.0.0/cerberuspy.egg-info/dependency_links.txt
--rw-r--r--   0 avate     (1000) avate     (1000)       11 2023-08-05 20:32:50.000000 cerberuspy-1.0.0/cerberuspy.egg-info/top_level.txt
--rw-r--r--   0 avate     (1000) avate     (1000)       38 2023-08-05 20:32:50.825430 cerberuspy-1.0.0/setup.cfg
--rw-r--r--   0 avate     (1000) avate     (1000)      224 2023-08-05 20:32:36.000000 cerberuspy-1.0.0/setup.py
+drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-06 17:55:07.885542 cerberuspy-1.0.1/
+-rw-r--r--   0 avate     (1000) avate     (1000)      242 2023-08-06 17:55:07.885542 cerberuspy-1.0.1/PKG-INFO
+drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-06 17:55:07.881542 cerberuspy-1.0.1/cerberuspy/
+-rw-r--r--   0 avate     (1000) avate     (1000)       27 2023-08-03 14:36:51.000000 cerberuspy-1.0.1/cerberuspy/__init__.py
+-rw-r--r--   0 avate     (1000) avate     (1000)      714 2023-08-05 19:49:34.000000 cerberuspy-1.0.1/cerberuspy/client.py
+drwxr-xr-x   0 avate     (1000) avate     (1000)        0 2023-08-06 17:55:07.885542 cerberuspy-1.0.1/cerberuspy.egg-info/
+-rw-r--r--   0 avate     (1000) avate     (1000)      242 2023-08-06 17:55:07.000000 cerberuspy-1.0.1/cerberuspy.egg-info/PKG-INFO
+-rw-r--r--   0 avate     (1000) avate     (1000)      198 2023-08-06 17:55:07.000000 cerberuspy-1.0.1/cerberuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 avate     (1000) avate     (1000)        1 2023-08-06 17:55:07.000000 cerberuspy-1.0.1/cerberuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 avate     (1000) avate     (1000)       11 2023-08-06 17:55:07.000000 cerberuspy-1.0.1/cerberuspy.egg-info/top_level.txt
+-rw-r--r--   0 avate     (1000) avate     (1000)       38 2023-08-06 17:55:07.885542 cerberuspy-1.0.1/setup.cfg
+-rw-r--r--   0 avate     (1000) avate     (1000)      280 2023-08-06 17:54:55.000000 cerberuspy-1.0.1/setup.py
```

### Comparing `cerberuspy-1.0.0/cerberuspy/client.py` & `cerberuspy-1.0.1/cerberuspy/client.py`

 * *Files identical despite different names*

