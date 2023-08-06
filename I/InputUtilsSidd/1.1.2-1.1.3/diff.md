# Comparing `tmp/InputUtilsSidd-1.1.2.tar.gz` & `tmp/InputUtilsSidd-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InputUtilsSidd-1.1.2.tar", last modified: Sun Aug  6 15:09:50 2023, max compression
+gzip compressed data, was "InputUtilsSidd-1.1.3.tar", last modified: Sun Aug  6 18:52:17 2023, max compression
```

## Comparing `InputUtilsSidd-1.1.2.tar` & `InputUtilsSidd-1.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:09:50.967869 InputUtilsSidd-1.1.2/
-drwxrwxrwx   0        0        0        0 2023-08-06 15:09:50.967869 InputUtilsSidd-1.1.2/InputUtilsSidd.egg-info/
--rw-rw-rw-   0        0        0      148 2023-08-06 15:09:50.000000 InputUtilsSidd-1.1.2/InputUtilsSidd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-08-06 15:09:50.000000 InputUtilsSidd-1.1.2/InputUtilsSidd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:09:50.000000 InputUtilsSidd-1.1.2/InputUtilsSidd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:09:50.000000 InputUtilsSidd-1.1.2/InputUtilsSidd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      148 2023-08-06 15:09:50.967869 InputUtilsSidd-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2023-08-05 22:12:30.000000 InputUtilsSidd-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 15:09:50.967869 InputUtilsSidd-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      242 2023-08-06 15:09:29.000000 InputUtilsSidd-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 18:52:17.395194 InputUtilsSidd-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-08-06 18:52:17.387368 InputUtilsSidd-1.1.3/InputUtilsSidd.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-08-06 18:52:17.000000 InputUtilsSidd-1.1.3/InputUtilsSidd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-08-06 18:52:17.000000 InputUtilsSidd-1.1.3/InputUtilsSidd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 18:52:17.000000 InputUtilsSidd-1.1.3/InputUtilsSidd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 18:52:17.000000 InputUtilsSidd-1.1.3/InputUtilsSidd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      148 2023-08-06 18:52:17.392353 InputUtilsSidd-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2023-08-05 22:12:30.000000 InputUtilsSidd-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 18:52:17.396189 InputUtilsSidd-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      242 2023-08-06 18:51:22.000000 InputUtilsSidd-1.1.3/setup.py
```

### Comparing `InputUtilsSidd-1.1.2/README.md` & `InputUtilsSidd-1.1.3/README.md`

 * *Files identical despite different names*

