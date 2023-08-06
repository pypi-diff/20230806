# Comparing `tmp/boopy-0.1.tar.gz` & `tmp/boopy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boopy-0.1.tar", last modified: Sun Aug  6 13:53:50 2023, max compression
+gzip compressed data, was "boopy-0.1.1.tar", last modified: Sun Aug  6 15:15:02 2023, max compression
```

## Comparing `boopy-0.1.tar` & `boopy-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 13:53:50.398073 boopy-0.1/
--rw-rw-rw-   0        0        0      159 2023-08-06 13:53:50.397073 boopy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-22 14:36:15.000000 boopy-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 13:53:50.381073 boopy-0.1/boopy/
--rw-rw-rw-   0        0        0      450 2023-08-06 13:48:49.000000 boopy-0.1/boopy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:53:50.392072 boopy-0.1/boopy/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:36:15.000000 boopy-0.1/boopy/helpers/__init__.py
--rw-rw-rw-   0        0        0     3404 2023-08-06 13:48:19.000000 boopy-0.1/boopy/helpers/deposit_helper.py
--rw-rw-rw-   0        0        0     3983 2023-08-06 13:48:18.000000 boopy-0.1/boopy/helpers/fra_helper.py
--rw-rw-rw-   0        0        0      969 2023-08-06 13:48:17.000000 boopy-0.1/boopy/helpers/interest_rate_helper.py
--rw-rw-rw-   0        0        0     4130 2023-08-06 13:48:42.000000 boopy-0.1/boopy/helpers/swap_helper.py
--rw-rw-rw-   0        0        0     1723 2023-07-30 19:20:59.000000 boopy-0.1/boopy/interest_rate.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:53:50.396094 boopy-0.1/boopy/time/
--rw-rw-rw-   0        0        0        0 2023-04-22 14:36:15.000000 boopy-0.1/boopy/time/__init__.py
--rw-rw-rw-   0        0        0      254 2023-08-06 11:12:05.000000 boopy-0.1/boopy/time/frequency.py
--rw-rw-rw-   0        0        0      738 2023-08-06 11:12:05.000000 boopy-0.1/boopy/time/period.py
--rw-rw-rw-   0        0        0     5151 2023-08-06 13:48:49.000000 boopy-0.1/boopy/time/schedule.py
-drwxrwxrwx   0        0        0        0 2023-08-06 13:53:50.387073 boopy-0.1/boopy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-08-06 13:53:50.000000 boopy-0.1/boopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-08-06 13:53:50.000000 boopy-0.1/boopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 13:53:50.000000 boopy-0.1/boopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-06 13:53:50.000000 boopy-0.1/boopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 13:53:50.398073 boopy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      245 2023-08-06 13:48:41.000000 boopy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:15:02.369762 boopy-0.1.1/
+-rw-rw-rw-   0        0        0     1077 2023-08-06 14:22:26.000000 boopy-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      381 2023-08-06 15:15:02.369762 boopy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-22 14:36:15.000000 boopy-0.1.1/README.md
+-rw-rw-rw-   0        0        0      248 2023-08-06 14:22:26.000000 boopy-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-06 15:15:02.345762 boopy-0.1.1/boopy/
+-rw-rw-rw-   0        0        0      450 2023-08-06 13:48:49.000000 boopy-0.1.1/boopy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:15:02.363762 boopy-0.1.1/boopy/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:36:15.000000 boopy-0.1.1/boopy/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3404 2023-08-06 13:48:19.000000 boopy-0.1.1/boopy/helpers/deposit_helper.py
+-rw-rw-rw-   0        0        0     3983 2023-08-06 13:48:18.000000 boopy-0.1.1/boopy/helpers/fra_helper.py
+-rw-rw-rw-   0        0        0      969 2023-08-06 13:48:17.000000 boopy-0.1.1/boopy/helpers/interest_rate_helper.py
+-rw-rw-rw-   0        0        0     4130 2023-08-06 13:48:42.000000 boopy-0.1.1/boopy/helpers/swap_helper.py
+-rw-rw-rw-   0        0        0     1723 2023-07-30 19:20:59.000000 boopy-0.1.1/boopy/interest_rate.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:15:02.367761 boopy-0.1.1/boopy/time/
+-rw-rw-rw-   0        0        0        0 2023-04-22 14:36:15.000000 boopy-0.1.1/boopy/time/__init__.py
+-rw-rw-rw-   0        0        0      254 2023-08-06 11:12:05.000000 boopy-0.1.1/boopy/time/frequency.py
+-rw-rw-rw-   0        0        0      738 2023-08-06 11:12:05.000000 boopy-0.1.1/boopy/time/period.py
+-rw-rw-rw-   0        0        0     5151 2023-08-06 13:48:49.000000 boopy-0.1.1/boopy/time/schedule.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:15:02.358761 boopy-0.1.1/boopy.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-08-06 15:15:02.000000 boopy-0.1.1/boopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-08-06 15:15:02.000000 boopy-0.1.1/boopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:15:02.000000 boopy-0.1.1/boopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-06 15:15:02.000000 boopy-0.1.1/boopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-06 15:15:02.000000 boopy-0.1.1/boopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:15:02.370762 boopy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      717 2023-08-06 15:14:42.000000 boopy-0.1.1/setup.py
```

### Comparing `boopy-0.1/boopy/helpers/deposit_helper.py` & `boopy-0.1.1/boopy/helpers/deposit_helper.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/helpers/fra_helper.py` & `boopy-0.1.1/boopy/helpers/fra_helper.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/helpers/interest_rate_helper.py` & `boopy-0.1.1/boopy/helpers/interest_rate_helper.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/helpers/swap_helper.py` & `boopy-0.1.1/boopy/helpers/swap_helper.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/interest_rate.py` & `boopy-0.1.1/boopy/interest_rate.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/time/period.py` & `boopy-0.1.1/boopy/time/period.py`

 * *Files identical despite different names*

### Comparing `boopy-0.1/boopy/time/schedule.py` & `boopy-0.1.1/boopy/time/schedule.py`

 * *Files identical despite different names*

