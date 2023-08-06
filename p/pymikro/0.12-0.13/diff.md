# Comparing `tmp/pymikro-0.12.tar.gz` & `tmp/pymikro-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymikro-0.12.tar", last modified: Sun Aug  6 20:09:14 2023, max compression
+gzip compressed data, was "pymikro-0.13.tar", last modified: Sun Aug  6 20:22:49 2023, max compression
```

## Comparing `pymikro-0.12.tar` & `pymikro-0.13.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/
--rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-07-17 08:23:51.000000 pymikro-0.12/LICENSE
--rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:09:14.041136 pymikro-0.12/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)     6787 2023-07-18 17:01:01.000000 pymikro-0.12/README.md
--rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 20:09:14.041136 pymikro-0.12/setup.cfg
--rw-r--r--   0 ze        (1000) ze        (1000)      502 2023-08-06 20:08:59.000000 pymikro-0.12/setup.py
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/pymikro/
--rw-r--r--   0 ze        (1000) ze        (1000)     5299 2023-07-29 13:25:33.000000 pymikro-0.12/src/pymikro/__init__.py
-drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:09:14.041136 pymikro-0.12/src/pymikro.egg-info/
--rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/PKG-INFO
--rw-r--r--   0 ze        (1000) ze        (1000)      224 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/SOURCES.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/dependency_links.txt
--rw-r--r--   0 ze        (1000) ze        (1000)       11 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/requires.txt
--rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-06 20:09:14.000000 pymikro-0.12/src/pymikro.egg-info/top_level.txt
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:22:49.988430 pymikro-0.13/
+-rw-r--r--   0 ze        (1000) ze        (1000)    26526 2023-07-17 08:23:51.000000 pymikro-0.13/LICENSE
+-rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:22:49.988430 pymikro-0.13/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)     6787 2023-07-18 17:01:01.000000 pymikro-0.13/README.md
+-rw-r--r--   0 ze        (1000) ze        (1000)       38 2023-08-06 20:22:49.988430 pymikro-0.13/setup.cfg
+-rw-r--r--   0 ze        (1000) ze        (1000)      543 2023-08-06 20:22:42.000000 pymikro-0.13/setup.py
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:22:49.988430 pymikro-0.13/src/
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:22:49.988430 pymikro-0.13/src/pymikro/
+-rw-r--r--   0 ze        (1000) ze        (1000)     5299 2023-07-29 13:25:33.000000 pymikro-0.13/src/pymikro/__init__.py
+-rw-r--r--   0 ze        (1000) ze        (1000)     1456 2023-07-15 21:23:26.000000 pymikro-0.13/src/pymikro/maschine_mikro_mk3.json
+drwxr-xr-x   0 ze        (1000) ze        (1000)        0 2023-08-06 20:22:49.988430 pymikro-0.13/src/pymikro.egg-info/
+-rw-r--r--   0 ze        (1000) ze        (1000)      286 2023-08-06 20:22:49.000000 pymikro-0.13/src/pymikro.egg-info/PKG-INFO
+-rw-r--r--   0 ze        (1000) ze        (1000)      260 2023-08-06 20:22:49.000000 pymikro-0.13/src/pymikro.egg-info/SOURCES.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        1 2023-08-06 20:22:49.000000 pymikro-0.13/src/pymikro.egg-info/dependency_links.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)       11 2023-08-06 20:22:49.000000 pymikro-0.13/src/pymikro.egg-info/requires.txt
+-rw-r--r--   0 ze        (1000) ze        (1000)        8 2023-08-06 20:22:49.000000 pymikro-0.13/src/pymikro.egg-info/top_level.txt
```

### Comparing `pymikro-0.12/LICENSE` & `pymikro-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pymikro-0.12/README.md` & `pymikro-0.13/README.md`

 * *Files identical despite different names*

### Comparing `pymikro-0.12/src/pymikro/__init__.py` & `pymikro-0.13/src/pymikro/__init__.py`

 * *Files identical despite different names*

