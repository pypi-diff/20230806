# Comparing `tmp/YandexHome-0.1.5.tar.gz` & `tmp/YandexHome-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.5.tar", last modified: Sun Aug  6 15:12:30 2023, max compression
+gzip compressed data, was "YandexHome-0.1.6.tar", last modified: Sun Aug  6 15:37:28 2023, max compression
```

## Comparing `YandexHome-0.1.5.tar` & `YandexHome-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:12:30.519101 YandexHome-0.1.5/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:12:30.518104 YandexHome-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-06 15:12:15.000000 YandexHome-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 15:12:30.519101 YandexHome-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 15:12:30.498461 YandexHome-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 15:12:30.507394 YandexHome-0.1.5/src/YandexHome/
--rw-rw-rw-   0        0        0     5331 2023-08-06 14:58:22.000000 YandexHome-0.1.5/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.5/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3103 2023-08-06 14:41:53.000000 YandexHome-0.1.5/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.5/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:12:30.516101 YandexHome-0.1.5/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:12:30.000000 YandexHome-0.1.5/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 15:12:30.000000 YandexHome-0.1.5/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:12:30.000000 YandexHome-0.1.5/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-06 15:12:30.000000 YandexHome-0.1.5/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 15:12:30.000000 YandexHome-0.1.5/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:37:28.916621 YandexHome-0.1.6/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:37:28.916621 YandexHome-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-06 15:37:13.000000 YandexHome-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:37:28.917630 YandexHome-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:37:28.897608 YandexHome-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 15:37:28.905606 YandexHome-0.1.6/src/YandexHome/
+-rw-rw-rw-   0        0        0     8380 2023-08-06 15:37:07.000000 YandexHome-0.1.6/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.6/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3103 2023-08-06 14:41:53.000000 YandexHome-0.1.6/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.6/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:37:28.914551 YandexHome-0.1.6/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:37:28.000000 YandexHome-0.1.6/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 15:37:28.000000 YandexHome-0.1.6/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:37:28.000000 YandexHome-0.1.6/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-06 15:37:28.000000 YandexHome-0.1.6/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 15:37:28.000000 YandexHome-0.1.6/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.5/src/YandexHome/device.py` & `YandexHome-0.1.6/src/YandexHome/device.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.5/src/YandexHome/group.py` & `YandexHome-0.1.6/src/YandexHome/group.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.5/src/YandexHome/scenario.py` & `YandexHome-0.1.6/src/YandexHome/scenario.py`

 * *Files identical despite different names*

