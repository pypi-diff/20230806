# Comparing `tmp/olografos-0.0.0.tar.gz` & `tmp/olografos-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olografos-0.0.0.tar", last modified: Sun Aug  6 21:53:22 2023, max compression
+gzip compressed data, was "olografos-1.0.1.tar", last modified: Sun Aug  6 21:54:17 2023, max compression
```

## Comparing `olografos-0.0.0.tar` & `olografos-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:53:22.265046 olografos-0.0.0/
--rw-r--r--   0 imertz     (501) staff       (20)     2782 2023-08-06 21:53:22.264903 olografos-0.0.0/PKG-INFO
--rw-r--r--   0 imertz     (501) staff       (20)     2523 2023-08-06 21:50:36.000000 olografos-0.0.0/README.md
-drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:53:22.263183 olografos-0.0.0/olografos/
--rw-r--r--   0 imertz     (501) staff       (20)    90090 2023-08-06 21:47:50.000000 olografos-0.0.0/olografos/__init__.py
-drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:53:22.264669 olografos-0.0.0/olografos.egg-info/
--rw-r--r--   0 imertz     (501) staff       (20)     2782 2023-08-06 21:53:22.000000 olografos-0.0.0/olografos.egg-info/PKG-INFO
--rw-r--r--   0 imertz     (501) staff       (20)      172 2023-08-06 21:53:22.000000 olografos-0.0.0/olografos.egg-info/SOURCES.txt
--rw-r--r--   0 imertz     (501) staff       (20)        1 2023-08-06 21:53:22.000000 olografos-0.0.0/olografos.egg-info/dependency_links.txt
--rw-r--r--   0 imertz     (501) staff       (20)       10 2023-08-06 21:53:22.000000 olografos-0.0.0/olografos.egg-info/top_level.txt
--rw-r--r--   0 imertz     (501) staff       (20)       38 2023-08-06 21:53:22.265090 olografos-0.0.0/setup.cfg
--rw-r--r--   0 imertz     (501) staff       (20)      432 2023-08-06 21:21:29.000000 olografos-0.0.0/setup.py
+drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:54:17.686210 olografos-1.0.1/
+-rw-r--r--   0 imertz     (501) staff       (20)     2782 2023-08-06 21:54:17.686084 olografos-1.0.1/PKG-INFO
+-rw-r--r--   0 imertz     (501) staff       (20)     2523 2023-08-06 21:50:36.000000 olografos-1.0.1/README.md
+drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:54:17.684874 olografos-1.0.1/olografos/
+-rw-r--r--   0 imertz     (501) staff       (20)    90090 2023-08-06 21:47:50.000000 olografos-1.0.1/olografos/__init__.py
+drwxr-xr-x   0 imertz     (501) staff       (20)        0 2023-08-06 21:54:17.685892 olografos-1.0.1/olografos.egg-info/
+-rw-r--r--   0 imertz     (501) staff       (20)     2782 2023-08-06 21:54:17.000000 olografos-1.0.1/olografos.egg-info/PKG-INFO
+-rw-r--r--   0 imertz     (501) staff       (20)      172 2023-08-06 21:54:17.000000 olografos-1.0.1/olografos.egg-info/SOURCES.txt
+-rw-r--r--   0 imertz     (501) staff       (20)        1 2023-08-06 21:54:17.000000 olografos-1.0.1/olografos.egg-info/dependency_links.txt
+-rw-r--r--   0 imertz     (501) staff       (20)       10 2023-08-06 21:54:17.000000 olografos-1.0.1/olografos.egg-info/top_level.txt
+-rw-r--r--   0 imertz     (501) staff       (20)       38 2023-08-06 21:54:17.686252 olografos-1.0.1/setup.cfg
+-rw-r--r--   0 imertz     (501) staff       (20)      437 2023-08-06 21:54:15.000000 olografos-1.0.1/setup.py
```

### Comparing `olografos-0.0.0/PKG-INFO` & `olografos-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olografos
-Version: 0.0.0
+Version: 1.0.1
 Summary: A package to convert numbers to greek words
 Home-page: https://github.com/imertz/olografos-py
 Author: Yiannis Mertzanis
 Author-email: imertz@protonmail.com
 Description-Content-Type: text/markdown
 
 # Ολογράφως
```

### Comparing `olografos-0.0.0/README.md` & `olografos-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `olografos-0.0.0/olografos/__init__.py` & `olografos-1.0.1/olografos/__init__.py`

 * *Files identical despite different names*

### Comparing `olografos-0.0.0/olografos.egg-info/PKG-INFO` & `olografos-1.0.1/olografos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olografos
-Version: 0.0.0
+Version: 1.0.1
 Summary: A package to convert numbers to greek words
 Home-page: https://github.com/imertz/olografos-py
 Author: Yiannis Mertzanis
 Author-email: imertz@protonmail.com
 Description-Content-Type: text/markdown
 
 # Ολογράφως
```

