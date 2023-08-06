# Comparing `tmp/report-dh-0.9.1.tar.gz` & `tmp/report-dh-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report-dh-0.9.1.tar", last modified: Tue Feb 28 21:06:47 2023, max compression
+gzip compressed data, was "report-dh-0.9.2.tar", last modified: Tue Feb 28 21:15:27 2023, max compression
```

## Comparing `report-dh-0.9.1.tar` & `report-dh-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:06:47.484974 report-dh-0.9.1/
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      710 2023-02-28 21:06:47.484974 report-dh-0.9.1/PKG-INFO
-drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:06:47.413630 report-dh-0.9.1/report/
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       41 2023-02-28 21:02:49.000000 report-dh-0.9.1/report/__init__.py
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      989 2023-02-28 20:24:43.000000 report-dh-0.9.1/report/_config.py
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     6933 2023-02-28 19:46:07.000000 report-dh-0.9.1/report/_internal.py
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      599 2023-02-28 20:37:18.000000 report-dh-0.9.1/report/conftest.py
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     2216 2023-02-28 20:24:50.000000 report-dh-0.9.1/report/item.py
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      599 2023-02-28 20:52:37.000000 report-dh-0.9.1/report/plugin.py
-drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:06:47.468186 report-dh-0.9.1/report_dh.egg-info/
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      710 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/PKG-INFO
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      316 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/SOURCES.txt
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        1 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/dependency_links.txt
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       88 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/entry_points.txt
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       16 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/requires.txt
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        7 2023-02-28 21:06:47.000000 report-dh-0.9.1/report_dh.egg-info/top_level.txt
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       38 2023-02-28 21:06:47.484974 report-dh-0.9.1/setup.cfg
--rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     1127 2023-02-28 21:05:48.000000 report-dh-0.9.1/setup.py
+drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:15:27.222175 report-dh-0.9.2/
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      710 2023-02-28 21:15:27.222175 report-dh-0.9.2/PKG-INFO
+drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:15:27.174189 report-dh-0.9.2/report/
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       41 2023-02-28 21:02:49.000000 report-dh-0.9.2/report/__init__.py
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      989 2023-02-28 20:24:43.000000 report-dh-0.9.2/report/_config.py
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     6933 2023-02-28 19:46:07.000000 report-dh-0.9.2/report/_internal.py
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      599 2023-02-28 20:37:18.000000 report-dh-0.9.2/report/conftest.py
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     2216 2023-02-28 20:24:50.000000 report-dh-0.9.2/report/item.py
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      507 2023-02-28 21:14:21.000000 report-dh-0.9.2/report/plugin.py
+drwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        0 2023-02-28 21:15:27.222175 report-dh-0.9.2/report_dh.egg-info/
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      710 2023-02-28 21:15:26.000000 report-dh-0.9.2/report_dh.egg-info/PKG-INFO
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)      316 2023-02-28 21:15:27.000000 report-dh-0.9.2/report_dh.egg-info/SOURCES.txt
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        1 2023-02-28 21:15:26.000000 report-dh-0.9.2/report_dh.egg-info/dependency_links.txt
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       88 2023-02-28 21:15:26.000000 report-dh-0.9.2/report_dh.egg-info/entry_points.txt
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       16 2023-02-28 21:15:26.000000 report-dh-0.9.2/report_dh.egg-info/requires.txt
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)        7 2023-02-28 21:15:26.000000 report-dh-0.9.2/report_dh.egg-info/top_level.txt
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)       38 2023-02-28 21:15:27.222175 report-dh-0.9.2/setup.cfg
+-rwxrwxrwx   0 deyaah    (1000) deyaah    (1000)     1127 2023-02-28 21:15:23.000000 report-dh-0.9.2/setup.py
```

### Comparing `report-dh-0.9.1/PKG-INFO` & `report-dh-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: report-dh
-Version: 0.9.1
+Version: 0.9.2
 Summary: Report Portal API
 Home-page: https://github.com/deyaa562/Report
 Author: Deyaa Hojerat
 Author-email: deyaa.hojerat.98@gmail.com
 License: Apache Software License
 Description: Report Portal API Wrapper
 Platform: UNKNOWN
```

### Comparing `report-dh-0.9.1/report/_config.py` & `report-dh-0.9.2/report/_config.py`

 * *Files identical despite different names*

### Comparing `report-dh-0.9.1/report/_internal.py` & `report-dh-0.9.2/report/_internal.py`

 * *Files identical despite different names*

### Comparing `report-dh-0.9.1/report/conftest.py` & `report-dh-0.9.2/report/conftest.py`

 * *Files identical despite different names*

### Comparing `report-dh-0.9.1/report/item.py` & `report-dh-0.9.2/report/item.py`

 * *Files identical despite different names*

### Comparing `report-dh-0.9.1/report_dh.egg-info/PKG-INFO` & `report-dh-0.9.2/report_dh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: report-dh
-Version: 0.9.1
+Version: 0.9.2
 Summary: Report Portal API
 Home-page: https://github.com/deyaa562/Report
 Author: Deyaa Hojerat
 Author-email: deyaa.hojerat.98@gmail.com
 License: Apache Software License
 Description: Report Portal API Wrapper
 Platform: UNKNOWN
```

### Comparing `report-dh-0.9.1/setup.py` & `report-dh-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='report-dh',
-    version='0.9.1',
+    version='0.9.2',
     packages=find_packages(),
     entry_points={
         'pytest11': [
             'report=report.plugin'
         ],
         'console_scripts': [
             'report-dh=report._config:config'
```

