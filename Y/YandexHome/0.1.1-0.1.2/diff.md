# Comparing `tmp/YandexHome-0.1.1.tar.gz` & `tmp/YandexHome-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.1.tar", last modified: Sun Aug  6 13:06:15 2023, max compression
+gzip compressed data, was "YandexHome-0.1.2.tar", last modified: Sun Aug  6 14:30:05 2023, max compression
```

## Comparing `YandexHome-0.1.1.tar` & `YandexHome-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:15.119785 YandexHome-0.1.1/
--rw-rw-rw-   0        0        0      132 2023-08-06 13:06:15.119269 YandexHome-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-08-06 13:06:02.000000 YandexHome-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 13:06:15.119785 YandexHome-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:15.101049 YandexHome-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:15.109253 YandexHome-0.1.1/src/YandexHome/
--rw-rw-rw-   0        0        0     5200 2023-08-06 13:05:18.000000 YandexHome-0.1.1/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.1/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3097 2023-08-06 13:03:56.000000 YandexHome-0.1.1/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.1/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:06:15.117763 YandexHome-0.1.1/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 13:06:15.000000 YandexHome-0.1.1/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 13:06:15.000000 YandexHome-0.1.1/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 13:06:15.000000 YandexHome-0.1.1/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-08-06 13:06:15.000000 YandexHome-0.1.1/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 13:06:15.000000 YandexHome-0.1.1/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.261152 YandexHome-0.1.2/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:30:05.261152 YandexHome-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-08-06 14:29:35.000000 YandexHome-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 14:30:05.261152 YandexHome-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.242187 YandexHome-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.249546 YandexHome-0.1.2/src/YandexHome/
+-rw-rw-rw-   0        0        0     5200 2023-08-06 13:05:18.000000 YandexHome-0.1.2/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.2/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3097 2023-08-06 13:03:56.000000 YandexHome-0.1.2/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.2/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.259152 YandexHome-0.1.2/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.1/src/YandexHome/__init__.py` & `YandexHome-0.1.2/src/YandexHome/__init__.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.1/src/YandexHome/device.py` & `YandexHome-0.1.2/src/YandexHome/device.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.1/src/YandexHome/group.py` & `YandexHome-0.1.2/src/YandexHome/group.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.1/src/YandexHome/scenario.py` & `YandexHome-0.1.2/src/YandexHome/scenario.py`

 * *Files identical despite different names*

