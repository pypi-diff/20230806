# Comparing `tmp/bec_scan_bundler-0.9.1.tar.gz` & `tmp/bec_scan_bundler-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scan_bundler-0.9.1.tar", last modified: Mon Jul  3 16:24:04 2023, max compression
+gzip compressed data, was "bec_scan_bundler-0.9.2.tar", last modified: Tue Jul  4 13:48:15 2023, max compression
```

## Comparing `bec_scan_bundler-0.9.1.tar` & `bec_scan_bundler-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:04.078943 bec_scan_bundler-0.9.1/
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-03 16:24:04.078943 bec_scan_bundler-0.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:04.077943 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-03 16:24:04.000000 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2023-07-03 16:24:04.000000 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:24:04.000000 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 16:24:04.000000 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-03 16:24:04.000000 bec_scan_bundler-0.9.1/bec_scan_bundler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:24:04.076943 bec_scan_bundler-0.9.1/scan_bundler/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-24 15:23:42.000000 bec_scan_bundler-0.9.1/scan_bundler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-28 10:41:58.000000 bec_scan_bundler-0.9.1/scan_bundler/bec_emitter.py
--rw-r--r--   0 root         (0) root         (0)     5491 2023-06-28 15:23:35.000000 bec_scan_bundler-0.9.1/scan_bundler/bluesky_emitter.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-28 10:41:58.000000 bec_scan_bundler-0.9.1/scan_bundler/emitter.py
--rw-r--r--   0 root         (0) root         (0)    14743 2023-06-28 15:23:35.000000 bec_scan_bundler-0.9.1/scan_bundler/scan_bundler.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-07-03 16:24:04.078943 bec_scan_bundler-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-28 14:27:03.000000 bec_scan_bundler-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:15.303766 bec_scan_bundler-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-04 13:48:15.303766 bec_scan_bundler-0.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:15.303766 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-04 13:48:15.000000 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-04 13:48:15.000000 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:48:15.000000 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-04 13:48:15.000000 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-04 13:48:15.000000 bec_scan_bundler-0.9.2/bec_scan_bundler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:15.302766 bec_scan_bundler-0.9.2/scan_bundler/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-24 15:23:42.000000 bec_scan_bundler-0.9.2/scan_bundler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-28 10:41:58.000000 bec_scan_bundler-0.9.2/scan_bundler/bec_emitter.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2023-06-28 15:23:35.000000 bec_scan_bundler-0.9.2/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-06-28 10:41:58.000000 bec_scan_bundler-0.9.2/scan_bundler/emitter.py
+-rw-r--r--   0 root         (0) root         (0)    14743 2023-06-28 15:23:35.000000 bec_scan_bundler-0.9.2/scan_bundler/scan_bundler.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-07-04 13:48:15.303766 bec_scan_bundler-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-28 14:27:03.000000 bec_scan_bundler-0.9.2/setup.py
```

### Comparing `bec_scan_bundler-0.9.1/scan_bundler/bec_emitter.py` & `bec_scan_bundler-0.9.2/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-0.9.1/scan_bundler/bluesky_emitter.py` & `bec_scan_bundler-0.9.2/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-0.9.1/scan_bundler/emitter.py` & `bec_scan_bundler-0.9.2/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-0.9.1/scan_bundler/scan_bundler.py` & `bec_scan_bundler-0.9.2/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-0.9.1/setup.cfg` & `bec_scan_bundler-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-0.9.1/setup.py` & `bec_scan_bundler-0.9.2/setup.py`

 * *Files identical despite different names*

