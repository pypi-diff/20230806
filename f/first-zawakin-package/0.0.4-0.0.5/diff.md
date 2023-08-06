# Comparing `tmp/first_zawakin_package-0.0.4.tar.gz` & `tmp/first_zawakin_package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first_zawakin_package-0.0.4.tar", max compression
+gzip compressed data, was "first_zawakin_package-0.0.5.tar", last modified: Sun Aug  6 05:04:11 2023, max compression
```

## Comparing `first_zawakin_package-0.0.4.tar` & `first_zawakin_package-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,14 @@
--rw-r--r--   0        0        0       24 2023-08-05 05:38:48.089648 first_zawakin_package-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-08-05 19:58:50.518108 first_zawakin_package-0.0.4/first_zawakin_package/__init__.py
--rw-r--r--   0        0        0      327 2023-08-05 20:15:20.523992 first_zawakin_package-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 first_zawakin_package-0.0.4/PKG-INFO
+drwxr-xr-x   0 zawawahoge   (501) staff       (20)        0 2023-08-06 05:04:11.070167 first_zawakin_package-0.0.5/
+-rw-r--r--   0 zawawahoge   (501) staff       (20)      248 2023-08-06 05:04:11.069856 first_zawakin_package-0.0.5/PKG-INFO
+-rw-r--r--   0 zawawahoge   (501) staff       (20)       24 2023-08-05 05:38:48.000000 first_zawakin_package-0.0.5/README.md
+drwxr-xr-x   0 zawawahoge   (501) staff       (20)        0 2023-08-06 05:04:11.066957 first_zawakin_package-0.0.5/first_zawakin_package/
+-rw-r--r--   0 zawawahoge   (501) staff       (20)        0 2023-08-05 19:58:50.000000 first_zawakin_package-0.0.5/first_zawakin_package/__init__.py
+drwxr-xr-x   0 zawawahoge   (501) staff       (20)        0 2023-08-06 05:04:11.069135 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/
+-rw-r--r--   0 zawawahoge   (501) staff       (20)      248 2023-08-06 05:04:11.000000 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/PKG-INFO
+-rw-r--r--   0 zawawahoge   (501) staff       (20)      287 2023-08-06 05:04:11.000000 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/SOURCES.txt
+-rw-r--r--   0 zawawahoge   (501) staff       (20)        1 2023-08-06 05:04:11.000000 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/dependency_links.txt
+-rw-r--r--   0 zawawahoge   (501) staff       (20)       22 2023-08-06 05:04:11.000000 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/top_level.txt
+-rw-r--r--   0 zawawahoge   (501) staff       (20)        1 2023-08-05 19:31:07.000000 first_zawakin_package-0.0.5/first_zawakin_package.egg-info/zip-safe
+-rw-r--r--   0 zawawahoge   (501) staff       (20)      328 2023-08-05 20:27:13.000000 first_zawakin_package-0.0.5/pyproject.toml
+-rw-r--r--   0 zawawahoge   (501) staff       (20)       38 2023-08-06 05:04:11.070260 first_zawakin_package-0.0.5/setup.cfg
+-rw-r--r--   0 zawawahoge   (501) staff       (20)     1078 2023-08-06 05:03:25.000000 first_zawakin_package-0.0.5/setup.py
```

