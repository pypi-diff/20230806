# Comparing `tmp/starco_pkl-2.0.tar.gz` & `tmp/starco_pkl-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starco_pkl-2.0.tar", last modified: Sun Aug  6 14:47:55 2023, max compression
+gzip compressed data, was "starco_pkl-3.0.tar", last modified: Sun Aug  6 14:51:44 2023, max compression
```

## Comparing `starco_pkl-2.0.tar` & `starco_pkl-3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:47:55.187177 starco_pkl-2.0/
--rw-r--r--   0 root         (0) root         (0)      158 2023-08-06 14:47:55.183177 starco_pkl-2.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:47:55.183177 starco_pkl-2.0/pkl/
--rw-rw-r--   0 root         (0) root         (0)       20 2023-08-06 13:52:14.000000 starco_pkl-2.0/pkl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2208 2023-08-06 14:05:17.000000 starco_pkl-2.0/pkl/pkl.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:47:55.187177 starco_pkl-2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      298 2023-08-06 14:47:50.000000 starco_pkl-2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:47:55.183177 starco_pkl-2.0/starco_pkl.egg-info/
--rw-r--r--   0 root         (0) root         (0)      158 2023-08-06 14:47:55.000000 starco_pkl-2.0/starco_pkl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      204 2023-08-06 14:47:55.000000 starco_pkl-2.0/starco_pkl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:47:55.000000 starco_pkl-2.0/starco_pkl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-08-06 14:47:55.000000 starco_pkl-2.0/starco_pkl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-08-06 14:47:55.000000 starco_pkl-2.0/starco_pkl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:51:44.849167 starco_pkl-3.0/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-08-06 14:51:44.849167 starco_pkl-3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:51:44.845167 starco_pkl-3.0/pkl/
+-rw-rw-r--   0 root         (0) root         (0)       20 2023-08-06 13:52:14.000000 starco_pkl-3.0/pkl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2208 2023-08-06 14:05:17.000000 starco_pkl-3.0/pkl/pkl.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 14:51:44.849167 starco_pkl-3.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      252 2023-08-06 14:51:39.000000 starco_pkl-3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 14:51:44.845167 starco_pkl-3.0/starco_pkl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-08-06 14:51:44.000000 starco_pkl-3.0/starco_pkl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      204 2023-08-06 14:51:44.000000 starco_pkl-3.0/starco_pkl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 14:51:44.000000 starco_pkl-3.0/starco_pkl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-06 14:51:44.000000 starco_pkl-3.0/starco_pkl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-06 14:51:44.000000 starco_pkl-3.0/starco_pkl.egg-info/top_level.txt
```

### Comparing `starco_pkl-2.0/pkl/pkl.py` & `starco_pkl-3.0/pkl/pkl.py`

 * *Files identical despite different names*

