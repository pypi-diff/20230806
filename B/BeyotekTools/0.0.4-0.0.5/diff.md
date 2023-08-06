# Comparing `tmp/BeyotekTools-0.0.4.tar.gz` & `tmp/BeyotekTools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyotekTools-0.0.4.tar", last modified: Sat Aug  5 23:50:32 2023, max compression
+gzip compressed data, was "BeyotekTools-0.0.5.tar", last modified: Sun Aug  6 00:17:39 2023, max compression
```

## Comparing `BeyotekTools-0.0.4.tar` & `BeyotekTools-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.146136 BeyotekTools-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      363 2023-08-05 23:50:32.146136 BeyotekTools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.4/README.md
--rw-rw-rw-   0        0        0      581 2023-08-05 23:50:16.000000 BeyotekTools-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 23:50:32.147140 BeyotekTools-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.130627 BeyotekTools-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.137633 BeyotekTools-0.0.4/src/BeyotekTools/
--rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.4/src/BeyotekTools/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-05 23:49:22.000000 BeyotekTools-0.0.4/src/BeyotekTools/mongodbutil.py
--rw-rw-rw-   0        0        0     7853 2023-08-05 23:49:59.000000 BeyotekTools-0.0.4/src/BeyotekTools/scraperutil.py
--rw-rw-rw-   0        0        0      745 2023-08-05 22:46:29.000000 BeyotekTools-0.0.4/src/BeyotekTools/speedlimit.py
--rw-rw-rw-   0        0        0     1775 2023-08-05 23:26:53.000000 BeyotekTools-0.0.4/src/BeyotekTools/stringutil.py
-drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.144632 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/
--rw-rw-rw-   0        0        0      363 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 00:17:39.595904 BeyotekTools-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      363 2023-08-06 00:17:39.596909 BeyotekTools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.5/README.md
+-rw-rw-rw-   0        0        0      581 2023-08-06 00:17:26.000000 BeyotekTools-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 00:17:39.596909 BeyotekTools-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 00:17:39.578631 BeyotekTools-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 00:17:39.586020 BeyotekTools-0.0.5/src/BeyotekTools/
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.5/src/BeyotekTools/__init__.py
+-rw-rw-rw-   0        0        0     1582 2023-08-06 00:17:08.000000 BeyotekTools-0.0.5/src/BeyotekTools/mongodbproductutil.py
+-rw-rw-rw-   0        0        0     7853 2023-08-05 23:49:59.000000 BeyotekTools-0.0.5/src/BeyotekTools/scraperutil.py
+-rw-rw-rw-   0        0        0      745 2023-08-05 22:46:29.000000 BeyotekTools-0.0.5/src/BeyotekTools/speedlimit.py
+-rw-rw-rw-   0        0        0     1775 2023-08-05 23:26:53.000000 BeyotekTools-0.0.5/src/BeyotekTools/stringutil.py
+drwxrwxrwx   0        0        0        0 2023-08-06 00:17:39.595904 BeyotekTools-0.0.5/src/BeyotekTools.egg-info/
+-rw-rw-rw-   0        0        0      363 2023-08-06 00:17:39.000000 BeyotekTools-0.0.5/src/BeyotekTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-08-06 00:17:39.000000 BeyotekTools-0.0.5/src/BeyotekTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 00:17:39.000000 BeyotekTools-0.0.5/src/BeyotekTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-06 00:17:39.000000 BeyotekTools-0.0.5/src/BeyotekTools.egg-info/top_level.txt
```

### Comparing `BeyotekTools-0.0.4/LICENSE` & `BeyotekTools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.4/pyproject.toml` & `BeyotekTools-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BeyotekTools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Beyotek", email="chuck@beyotek.com" },
 ]
 description = "Beyotek Tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `BeyotekTools-0.0.4/src/BeyotekTools/scraperutil.py` & `BeyotekTools-0.0.5/src/BeyotekTools/scraperutil.py`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.4/src/BeyotekTools/speedlimit.py` & `BeyotekTools-0.0.5/src/BeyotekTools/speedlimit.py`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.4/src/BeyotekTools/stringutil.py` & `BeyotekTools-0.0.5/src/BeyotekTools/stringutil.py`

 * *Files identical despite different names*

