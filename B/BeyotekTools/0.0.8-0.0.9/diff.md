# Comparing `tmp/BeyotekTools-0.0.8.tar.gz` & `tmp/BeyotekTools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyotekTools-0.0.8.tar", last modified: Sun Aug  6 00:53:22 2023, max compression
+gzip compressed data, was "BeyotekTools-0.0.9.tar", last modified: Sun Aug  6 01:11:29 2023, max compression
```

## Comparing `BeyotekTools-0.0.8.tar` & `BeyotekTools-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-08-06 00:53:22.207908 BeyotekTools-0.0.8/BeyotekTools.egg-info/
--rw-rw-rw-   0        0        0      485 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      485 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-08-06 00:53:08.000000 BeyotekTools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 01:11:29.795684 BeyotekTools-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-08-06 01:11:29.793688 BeyotekTools-0.0.9/BeyotekTools.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-08-06 01:11:29.000000 BeyotekTools-0.0.9/BeyotekTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-08-06 01:11:29.000000 BeyotekTools-0.0.9/BeyotekTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 01:11:29.000000 BeyotekTools-0.0.9/BeyotekTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-06 01:11:29.000000 BeyotekTools-0.0.9/BeyotekTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 01:11:29.000000 BeyotekTools-0.0.9/BeyotekTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      485 2023-08-06 01:11:29.795684 BeyotekTools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 01:11:29.796673 BeyotekTools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-08-06 01:11:14.000000 BeyotekTools-0.0.9/setup.py
```

### Comparing `BeyotekTools-0.0.8/LICENSE` & `BeyotekTools-0.0.9/LICENSE`

 * *Files identical despite different names*

