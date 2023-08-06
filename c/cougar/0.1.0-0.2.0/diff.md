# Comparing `tmp/cougar-0.1.0.tar.gz` & `tmp/cougar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.1.0.tar", last modified: Sat Jul 29 07:26:34 2023, max compression
+gzip compressed data, was "cougar-0.2.0.tar", last modified: Sun Jul 30 13:05:10 2023, max compression
```

## Comparing `cougar-0.1.0.tar` & `cougar-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-29 07:26:34.446880 cougar-0.1.0/
--rw-r--r--   0 ganyunchong   (501) staff       (20)    11357 2023-07-29 07:01:09.000000 cougar-0.1.0/LICENSE
--rw-r--r--   0 ganyunchong   (501) staff       (20)      127 2023-07-29 07:26:34.445430 cougar-0.1.0/PKG-INFO
--rw-r--r--   0 ganyunchong   (501) staff       (20)        8 2023-07-29 07:01:09.000000 cougar-0.1.0/README.md
-drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-29 07:26:34.439945 cougar-0.1.0/cougar/
--rw-r--r--   0 ganyunchong   (501) staff       (20)       99 2023-07-29 07:22:03.000000 cougar-0.1.0/cougar/__init__.py
--rw-r--r--   0 ganyunchong   (501) staff       (20)     1196 2023-07-29 07:19:06.000000 cougar-0.1.0/cougar/rolling.c
-drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-29 07:26:34.443608 cougar-0.1.0/cougar.egg-info/
--rw-r--r--   0 ganyunchong   (501) staff       (20)      127 2023-07-29 07:26:34.000000 cougar-0.1.0/cougar.egg-info/PKG-INFO
--rw-r--r--   0 ganyunchong   (501) staff       (20)      182 2023-07-29 07:26:34.000000 cougar-0.1.0/cougar.egg-info/SOURCES.txt
--rw-r--r--   0 ganyunchong   (501) staff       (20)        1 2023-07-29 07:26:34.000000 cougar-0.1.0/cougar.egg-info/dependency_links.txt
--rw-r--r--   0 ganyunchong   (501) staff       (20)        7 2023-07-29 07:26:34.000000 cougar-0.1.0/cougar.egg-info/top_level.txt
--rw-r--r--   0 ganyunchong   (501) staff       (20)       38 2023-07-29 07:26:34.447182 cougar-0.1.0/setup.cfg
--rw-r--r--   0 ganyunchong   (501) staff       (20)      434 2023-07-29 07:21:57.000000 cougar-0.1.0/setup.py
+drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-30 13:05:10.100053 cougar-0.2.0/
+-rw-r--r--   0 ganyunchong   (501) staff       (20)    11357 2023-07-29 07:01:09.000000 cougar-0.2.0/LICENSE
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      463 2023-07-30 13:05:10.099081 cougar-0.2.0/PKG-INFO
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      206 2023-07-30 13:03:53.000000 cougar-0.2.0/README.md
+drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-30 13:05:10.089535 cougar-0.2.0/cougar/
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      287 2023-07-30 13:04:23.000000 cougar-0.2.0/cougar/__init__.py
+-rw-r--r--   0 ganyunchong   (501) staff       (20)     2307 2023-07-30 12:45:18.000000 cougar-0.2.0/cougar/rolling.c
+drwxr-xr-x   0 ganyunchong   (501) staff       (20)        0 2023-07-30 13:05:10.097037 cougar-0.2.0/cougar.egg-info/
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      463 2023-07-30 13:05:09.000000 cougar-0.2.0/cougar.egg-info/PKG-INFO
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      211 2023-07-30 13:05:10.000000 cougar-0.2.0/cougar.egg-info/SOURCES.txt
+-rw-r--r--   0 ganyunchong   (501) staff       (20)        1 2023-07-30 13:05:09.000000 cougar-0.2.0/cougar.egg-info/dependency_links.txt
+-rw-r--r--   0 ganyunchong   (501) staff       (20)        6 2023-07-30 13:05:09.000000 cougar-0.2.0/cougar.egg-info/requires.txt
+-rw-r--r--   0 ganyunchong   (501) staff       (20)        7 2023-07-30 13:05:09.000000 cougar-0.2.0/cougar.egg-info/top_level.txt
+-rw-r--r--   0 ganyunchong   (501) staff       (20)       38 2023-07-30 13:05:10.100783 cougar-0.2.0/setup.cfg
+-rw-r--r--   0 ganyunchong   (501) staff       (20)      828 2023-07-30 13:04:35.000000 cougar-0.2.0/setup.py
```

### Comparing `cougar-0.1.0/LICENSE` & `cougar-0.2.0/LICENSE`

 * *Files identical despite different names*

