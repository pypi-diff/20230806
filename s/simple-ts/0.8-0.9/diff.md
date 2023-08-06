# Comparing `tmp/simple_ts-0.8.tar.gz` & `tmp/simple_ts-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.8.tar", last modified: Sun Aug  6 05:54:55 2023, max compression
+gzip compressed data, was "simple_ts-0.9.tar", last modified: Sun Aug  6 06:25:02 2023, max compression
```

## Comparing `simple_ts-0.8.tar` & `simple_ts-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 05:54:55.414922 simple_ts-0.8/
--rw-rw-rw-   0        0        0      125 2023-08-06 05:54:55.413921 simple_ts-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-08-06 05:36:14.000000 simple_ts-0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 05:54:55.438686 simple_ts-0.8/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-08-06 05:54:36.000000 simple_ts-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 05:54:55.354439 simple_ts-0.8/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-08-06 05:54:54.000000 simple_ts-0.8/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-08-06 05:54:54.000000 simple_ts-0.8/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 05:54:54.000000 simple_ts-0.8/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-06 05:54:54.000000 simple_ts-0.8/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-06 05:54:54.000000 simple_ts-0.8/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-06 05:54:55.379584 simple_ts-0.8/simplets/
--rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.8/simplets/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-07-14 17:01:17.000000 simple_ts-0.8/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:25:02.796238 simple_ts-0.9/
+-rw-rw-rw-   0        0        0      871 2023-08-06 06:25:02.795240 simple_ts-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-08-06 06:18:28.000000 simple_ts-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 06:25:02.796238 simple_ts-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-08-06 06:24:47.000000 simple_ts-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:25:02.792239 simple_ts-0.9/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      871 2023-08-06 06:25:02.000000 simple_ts-0.9/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-08-06 06:25:02.000000 simple_ts-0.9/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 06:25:02.000000 simple_ts-0.9/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-06 06:25:02.000000 simple_ts-0.9/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 06:25:02.000000 simple_ts-0.9/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 06:25:02.794244 simple_ts-0.9/simplets/
+-rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.9/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-07-14 17:01:17.000000 simple_ts-0.9/simplets/simplets.py
```

### Comparing `simple_ts-0.8/simplets/simplets.py` & `simple_ts-0.9/simplets/simplets.py`

 * *Files identical despite different names*

