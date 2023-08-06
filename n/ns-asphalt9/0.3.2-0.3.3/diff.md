# Comparing `tmp/ns_asphalt9-0.3.2.tar.gz` & `tmp/ns_asphalt9-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.3.2.tar", last modified: Sat Aug  5 03:05:14 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.3.3.tar", last modified: Sun Aug  6 04:47:54 2023, max compression
```

## Comparing `ns_asphalt9-0.3.2.tar` & `ns_asphalt9-0.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.971293 ns_asphalt9-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-05 03:05:14.971293 ns_asphalt9-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.963293 ns_asphalt9-0.3.2/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.967293 ns_asphalt9-0.3.2/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.967293 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.967293 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.967293 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.971293 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/core/utils/track_navi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.963293 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-05 03:05:14.000000 ns_asphalt9-0.3.2/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-05 03:05:14.971293 ns_asphalt9-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 03:05:14.971293 ns_asphalt9-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-05 03:05:02.000000 ns_asphalt9-0.3.2/tests/test_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.742322 ns_asphalt9-0.3.3/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25358 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/core/utils/track_navi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.742322 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 04:47:54.000000 ns_asphalt9-0.3.3/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:47:54.746322 ns_asphalt9-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-06 04:47:42.000000 ns_asphalt9-0.3.3/tests/test_pages.py
```

### Comparing `ns_asphalt9-0.3.2/LICENSE` & `ns_asphalt9-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/PKG-INFO` & `ns_asphalt9-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.3.2
+Version: 0.3.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.3.2/README.md` & `ns_asphalt9-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.3.3/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,24 @@
 class LoadingCarHunt(Page):
     """寻车加载页"""
 
     name = consts.loading_carhunt
     feature = "CAR HUNT.*BEST TIME"
     part_match = False
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if match_count:
+            if "CAR HUNT EVENT PACK" in text:
+                match_count = 0
+            else:
+                match_count = 10
+        return match_count
+
 
 @cache_decorator("page")
 class ConnectController(Page):
     """连接手柄"""
 
     name = consts.connect_controller
     feature = "Press.*on the controller"
```

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/utils/track_data.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/utils/track_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/core/utils/track_navi_data.py` & `ns_asphalt9-0.3.3/ns_asphalt9/core/utils/track_navi_data.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9/main.py` & `ns_asphalt9-0.3.3/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.3.3/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.3.2
+Version: 0.3.3
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.3.2/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.3.3/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.3.2/setup.cfg` & `ns_asphalt9-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.3.2
+version = 0.3.3
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.3.2/tests/test_pages.py` & `ns_asphalt9-0.3.3/tests/test_pages.py`

 * *Files identical despite different names*

