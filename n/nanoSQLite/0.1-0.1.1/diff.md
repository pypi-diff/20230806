# Comparing `tmp/nanoSQLite-0.1.tar.gz` & `tmp/nanoSQLite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoSQLite-0.1.tar", last modified: Sat Aug  5 23:58:24 2023, max compression
+gzip compressed data, was "nanoSQLite-0.1.1.tar", last modified: Sun Aug  6 00:03:46 2023, max compression
```

## Comparing `nanoSQLite-0.1.tar` & `nanoSQLite-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-05 23:58:24.791519 nanoSQLite-0.1/
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2092 2023-08-05 23:58:24.791519 nanoSQLite-0.1/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1999 2023-08-05 23:50:53.000000 nanoSQLite-0.1/README.md
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-05 23:58:24.790518 nanoSQLite-0.1/nanoSQLite/
--rw-r--r--   0 stefan    (1000) stefan    (1000)        0 2023-08-05 23:28:58.000000 nanoSQLite-0.1/nanoSQLite/__init__.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     6735 2023-08-05 23:48:12.000000 nanoSQLite-0.1/nanoSQLite/nanoSQLite.py
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-05 23:58:24.791519 nanoSQLite-0.1/nanoSQLite.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2092 2023-08-05 23:58:24.000000 nanoSQLite-0.1/nanoSQLite.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)      202 2023-08-05 23:58:24.000000 nanoSQLite-0.1/nanoSQLite.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2023-08-05 23:58:24.000000 nanoSQLite-0.1/nanoSQLite.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)       11 2023-08-05 23:58:24.000000 nanoSQLite-0.1/nanoSQLite.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)       38 2023-08-05 23:58:24.791519 nanoSQLite-0.1/setup.cfg
--rw-r--r--   0 stefan    (1000) stefan    (1000)      304 2023-08-05 23:58:22.000000 nanoSQLite-0.1/setup.py
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:03:46.451254 nanoSQLite-0.1.1/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     2094 2023-08-06 00:03:46.451254 nanoSQLite-0.1.1/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     1999 2023-08-05 23:50:53.000000 nanoSQLite-0.1.1/README.md
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:03:46.451254 nanoSQLite-0.1.1/nanoSQLite/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       26 2023-08-06 00:03:23.000000 nanoSQLite-0.1.1/nanoSQLite/__init__.py
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     6735 2023-08-05 23:48:12.000000 nanoSQLite-0.1.1/nanoSQLite/nanoSQLite.py
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:03:46.451254 nanoSQLite-0.1.1/nanoSQLite.egg-info/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     2094 2023-08-06 00:03:46.000000 nanoSQLite-0.1.1/nanoSQLite.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      202 2023-08-06 00:03:46.000000 nanoSQLite-0.1.1/nanoSQLite.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2023-08-06 00:03:46.000000 nanoSQLite-0.1.1/nanoSQLite.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       11 2023-08-06 00:03:46.000000 nanoSQLite-0.1.1/nanoSQLite.egg-info/top_level.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       38 2023-08-06 00:03:46.451254 nanoSQLite-0.1.1/setup.cfg
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      226 2023-08-06 00:03:02.000000 nanoSQLite-0.1.1/setup.py
```

### Comparing `nanoSQLite-0.1/PKG-INFO` & `nanoSQLite-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoSQLite
-Version: 0.1
+Version: 0.1.1
 Description-Content-Type: text/markdown
 
 # nanoSQLite
 
 `nanoSQLite` is a lightweight Python wrapper for SQLite.
 With around 200 lines of Python code, it provides an uncomplicated interface for managing SQLite databases.
```

### Comparing `nanoSQLite-0.1/README.md` & `nanoSQLite-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nanoSQLite-0.1/nanoSQLite/nanoSQLite.py` & `nanoSQLite-0.1.1/nanoSQLite/nanoSQLite.py`

 * *Files identical despite different names*

### Comparing `nanoSQLite-0.1/nanoSQLite.egg-info/PKG-INFO` & `nanoSQLite-0.1.1/nanoSQLite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoSQLite
-Version: 0.1
+Version: 0.1.1
 Description-Content-Type: text/markdown
 
 # nanoSQLite
 
 `nanoSQLite` is a lightweight Python wrapper for SQLite.
 With around 200 lines of Python code, it provides an uncomplicated interface for managing SQLite databases.
```

