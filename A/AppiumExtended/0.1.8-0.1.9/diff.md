# Comparing `tmp/AppiumExtended-0.1.8.tar.gz` & `tmp/AppiumExtended-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.1.8.tar", last modified: Tue Aug  1 12:56:01 2023, max compression
+gzip compressed data, was "AppiumExtended-0.1.9.tar", last modified: Tue Aug  1 20:41:09 2023, max compression
```

## Comparing `AppiumExtended-0.1.8.tar` & `AppiumExtended-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.216432 AppiumExtended-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.204432 AppiumExtended-0.1.8/AppiumExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28049 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_is.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_swipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumExtended/appium_wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumExtended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 12:56:01.000000 AppiumExtended-0.1.8/AppiumExtended.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumGraph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumGraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumGraph/appium_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumHelpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/appium_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/appium_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumHelpers/helpers_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumNavigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumNavigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumNavigator/appium_navigator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.208432 AppiumExtended-0.1.8/AppiumServer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumServer/appium_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/AppiumWebElementExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_adb_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_click.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_dom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_scroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_tap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/AppiumWebElementsExtended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementsExtended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/AppiumWebElementsExtended/web_elements_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   246568 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:56:01.216432 AppiumExtended-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/aapt.py
--rw-r--r--   0 runner    (1001) docker     (123)    41664 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26266 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/terminal/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:01.212432 AppiumExtended-0.1.8/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 12:55:50.000000 AppiumExtended-0.1.8/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28049 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_swipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumExtended/appium_wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumExtended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 20:41:09.000000 AppiumExtended-0.1.9/AppiumExtended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-01 20:41:09.000000 AppiumExtended-0.1.9/AppiumExtended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:41:09.000000 AppiumExtended-0.1.9/AppiumExtended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 20:41:09.000000 AppiumExtended-0.1.9/AppiumExtended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 20:41:09.000000 AppiumExtended-0.1.9/AppiumExtended.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumGraph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumGraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumGraph/appium_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumHelpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumHelpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumHelpers/appium_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumHelpers/appium_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumHelpers/helpers_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumNavigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumNavigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumNavigator/appium_navigator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumServer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumServer/appium_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.329471 AppiumExtended-0.1.9/AppiumWebElementExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/AppiumWebElementsExtended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementsExtended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/AppiumWebElementsExtended/web_elements_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   258670 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/terminal/aapt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51095 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/terminal/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/terminal/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:41:09.333471 AppiumExtended-0.1.9/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/utils/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-01 20:40:59.000000 AppiumExtended-0.1.9/utils/utils.py
```

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_base.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_base.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_extended.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_get.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_is.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_is.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_swipe.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_tap.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended/appium_wait.py` & `AppiumExtended-0.1.9/AppiumExtended/appium_wait.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumExtended.egg-info/PKG-INFO` & `AppiumExtended-0.1.9/AppiumExtended.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.8
+Version: 0.1.9
 Summary: An extension library for adding ease of use Appium-Python-Client
 Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AppiumExtended-0.1.8/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.1.9/AppiumExtended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.1.9/AppiumHelpers/appium_helpers.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumHelpers/appium_image.py` & `AppiumExtended-0.1.9/AppiumHelpers/appium_image.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.1.9/AppiumHelpers/helpers_decorators.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumNavigator/appium_navigator.py` & `AppiumExtended-0.1.9/AppiumNavigator/appium_navigator.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumServer/appium_server.py` & `AppiumExtended-0.1.9/AppiumServer/appium_server.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_adb_actions.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_click.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_dom.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_scroll.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/AppiumWebElementExtended/web_element_tap.py` & `AppiumExtended-0.1.9/AppiumWebElementExtended/web_element_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/LICENSE` & `AppiumExtended-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.1.8/PKG-INFO` & `AppiumExtended-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppiumExtended
-Version: 0.1.8
+Version: 0.1.9
 Summary: An extension library for adding ease of use Appium-Python-Client
 Home-page: https://github.com/molokov-klim/appium_extended
 Author: molokov-klim
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `AppiumExtended-0.1.8/README.md` & `AppiumExtended-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2109,30 +2109,30 @@
 
 Этот метод выполняет системную команду с использованием утилиты `aapt` (Android Asset Packaging Tool). В процессе работы создаются логи, которые сохраняются с использованием модуля `logging`.
 
 ### Исключения
 
 Метод может генерировать исключения, если указанный файл APK не найден, не может быть прочитан или не содержит ожидаемой информации о пакете. Все такие исключения должны быть обработаны в вызывающем коде. Дополнительно, если утилита `aapt` не установлена или не доступна для вызова в системе, метод может не работать корректно.
 
-## Метод: `get_launchable_activity_from_apk()`
+## Метод: `get_launchable_activity()`
 
 Статический метод, получает название запускаемой активности из APK-файла с помощью команды `aapt`. Используется для извлечения информации о запускаемой активности из файла APK.
 
 ### Параметры
 
 - `path_to_apk`: Путь до APK-файла, из которого требуется извлечь название запускаемой активности. Должен быть строкой, содержащей путь к файлу.
 
 ### Возвращаемое значение
 
 Возвращает строку, содержащую название запускаемой активности, извлеченное из APK-файла. Если название активности не может быть извлечено, возвращается `None`.
 
 ### Пример использования
 
 ```python
-launchable_activity = YourClassName.get_launchable_activity_from_apk(path_to_apk="/path/to/apk/file.apk")
+launchable_activity = YourClassName.get_launchable_activity(path_to_apk="/path/to/apk/file.apk")
 print(launchable_activity)
 ```
 
 ### Дополнительная информация
 
 Этот метод выполняет системную команду с использованием утилиты `aapt` (Android Asset Packaging Tool). В процессе работы создаются логи, которые сохраняются с использованием модуля `logging`.
 
@@ -2420,14 +2420,46 @@
 
 Этот метод использует метод `install_app()` из `driver` для установки приложения. Если установка успешна, метод `install_app()` не возвращает значение, в противном случае он может вызвать исключение.
 
 ### Исключения
 
 Метод может генерировать исключение, если в процессе его выполнения возникают проблемы. Если метод `install_app()` вызывает исключение, это исключение будет логироваться, а метод `install_app()` вернет `False`.
 
+## Метод: `is_app_installed(package: str) -> bool`
+
+Метод класса `Terminal`, предназначенный для проверки установки указанного пакета приложения с помощью Appium.
+
+### Параметры
+
+- `package` (тип: `str`): Имя пакета приложения, для которого нужно проверить установку.
+
+### Возвращаемое значение
+
+Возвращает значение `True`, если указанный пакет приложения установлен на устройстве, и `False` в противном случае.
+
+### Пример использования
+
+```python
+terminal = Terminal(driver)
+if terminal.is_app_installed("com.example.myapp"):
+    print("The app is installed.")
+else:
+    print("The app is not installed.")
+```
+
+### Дополнительная информация
+
+Метод `is_app_installed()` использует команду `pm list packages` для получения списка установленных пакетов приложений. Затем он фильтрует список и проверяет, содержится ли указанный пакет среди установленных. Если пакет найден в списке, метод вернет `True`, в противном случае вернет `False`.
+
+### Исключения
+
+Метод может вызывать исключение типа `KeyError`, если в процессе выполнения возникли проблемы с доступом к списку пакетов. В случае возникновения исключения, оно будет залогировано, и метод `is_app_installed()` вернет значение `False`.
+
+**Примечание:** Для корректной работы метода `is_app_installed()`, убедитесь, что устройство подключено к Appium и правильно настроено для выполнения команд через ADB.
+
 ## Метод: `press_home()`
 
 Метод класса `Terminal`, который эмулирует нажатие кнопки "Домой" на устройстве, используя Android Debug Bridge (ADB).
 
 ### Параметры
 
 Метод не принимает никаких параметров.
@@ -2775,15 +2807,15 @@
 
 Метод `stop_logcat()` сначала получает список всех выполняющихся процессов на устройстве с помощью команды `ps`. Затем он проходит через этот список и отправляет сигнал `SIGINT` каждому процессу `logcat`, который он находит, чтобы остановить его.
 
 ### Исключения
 
 Метод может вызвать исключение `KeyError`, если при его выполнении возникли проблемы. Если возникает исключение, оно будет залогировано, и метод `stop_logcat()` вернет `False`.
 
-## Метод: `know_pid(name)`
+## Метод: `know_pid()`
 
 Это метод класса `Terminal`, который ищет и возвращает идентификатор процесса (PID) по его имени с помощью команды `adb shell ps`.
 
 ### Параметры
 
 * `name (str)`: Имя процесса, PID которого необходимо найти.
 
@@ -2806,14 +2838,81 @@
 
 Метод `know_pid()` получает список всех выполняющихся процессов на устройстве с помощью команды `adb shell ps`, затем проходит по этому списку и ищет процесс с указанным именем. Если такой процесс найден, метод возвращает его PID. Если процесс не найден, метод возвращает `None`.
 
 ### Исключения
 
 Метод не обрабатывает исключения и, таким образом, может вызвать любое исключение, которое может вызвать `adb_shell(command)`.
 
+
+## Метод: `is_process_exist(name)`
+
+Это метод класса `Terminal`, который проверяет, существует ли процесс с указанным именем, используя команду `adb shell ps`.
+
+### Параметры
+
+* `name (str)`: Имя процесса, которое требуется проверить на существование.
+
+### Возвращаемое значение
+
+Метод возвращает `bool`. Если процесс с указанным именем существует, метод возвращает `True`. В противном случае, если процесс не найден, метод возвращает `False`.
+
+### Пример использования
+
+```python
+terminal = Terminal(driver)
+if terminal.is_process_exist("com.example.app"):
+    print("Процесс 'com.example.app' существует.")
+else:
+    print("Процесс 'com.example.app' не существует.")
+```
+
+### Дополнительная информация
+
+Метод `is_process_exist(name)` получает список всех выполняющихся процессов на устройстве с помощью команды `adb shell ps`, затем проверяет, есть ли процесс с указанным именем в этом списке. Если процесс с заданным именем найден, метод возвращает `True`, иначе возвращает `False`.
+
+### Исключения
+
+Метод не обрабатывает исключения и, таким образом, может вызвать любое исключение, которое может возникнуть при выполнении `adb_shell(command)`.
+
+**Примечание:** В описании метода `is_process_exist(name)` вместо `is_process_exist() > True` и `is_process_exist() > False`, используются логгеры для вывода отладочной информации. В реальной реализации эти строки не будут отображаться. Они присутствуют в данном контексте только для демонстрации логгирования.
+
+## Метод: `run_background_process(command, args="", process="")`
+
+Это метод класса `Terminal`, который запускает процесс в фоновом режиме на устройстве Android.
+
+### Параметры
+
+* `command (str)`: Команда для выполнения на устройстве.
+* `args (str)`: Дополнительные аргументы для команды. По умолчанию `""`.
+* `process (str)`: Название процесса, который будет запущен. По умолчанию `""`. Если значение `process` равно `""`, то не будет проверяться его запуск в системе.
+
+### Возвращаемое значение
+
+Метод возвращает `bool`. Если процесс был успешно запущен, метод возвращает `True`. В противном случае, если процесс не удалось запустить или указанный процесс не был найден, метод возвращает `False`.
+
+### Пример использования
+
+```python
+terminal = Terminal(driver)
+command_to_run = "my_background_command arg1 arg2"
+if terminal.run_background_process(command_to_run, args="--option"):
+    print("Процесс был успешно запущен.")
+else:
+    print("Произошла ошибка при запуске процесса или процесс не найден.")
+```
+
+### Дополнительная информация
+
+Метод `run_background_process(command, args="", process="")` выполняет переданную команду `command` на устройстве Android с дополнительными аргументами `args`. Команда запускается в фоновом режиме с использованием `nohup` и перенаправлением вывода в `/dev/null` для игнорирования вывода в консоль.
+
+Если параметр `process` не равен пустой строке, метод после запуска процесса проверяет его существование через метод `is_process_exist(name=process)`. Если процесс не найден, метод вернет `False`. В противном случае, если процесс успешно запущен или параметр `process` равен пустой строке, метод вернет `True`.
+
+Метод может вызывать исключение `KeyError`, и в таком случае он будет логировать ошибку и возвращать `False`.
+
+
 ## Метод: `kill_by_pid(pid)`
 
 Это метод класса `Terminal`, который посылает сигнал SIGINT процессу с указанным идентификатором процесса (PID), используя команду `adb shell kill`.
 
 ### Параметры
 
 * `pid (int)`: Идентификатор процесса (PID), который нужно остановить.
@@ -3091,14 +3190,84 @@
 
 Метод `install_app()` использует команду `adb install` для установки APK-файла на устройство.
 
 ### Исключения
 
 Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может быть вызвано методом `subprocess.check_output()`. Если исключение возникает, оно логируется и метод возвращает `False`.
 
+## Метод: `is_app_installed()`
+
+Этот метод класса `Adb` предназначен для проверки, установлено ли указанное приложение на подключенном устройстве Android с использованием ADB.
+
+### Параметры
+
+Метод принимает следующий параметр:
+
+- `package` (`str`): Имя пакета приложения, которое нужно проверить.
+
+### Возвращаемое значение
+
+Метод возвращает логическое значение `bool`:
+- `True` - если приложение установлено на устройстве.
+- `False` - если приложение не установлено на устройстве или произошла ошибка при проверке.
+
+### Пример использования
+
+```python
+adb = Adb()
+is_installed = adb.is_app_installed("com.example.app")
+if is_installed:
+    print("Приложение установлено на устройстве.")
+else:
+    print("Приложение не установлено на устройстве.")
+```
+
+### Дополнительная информация
+
+Метод `is_app_installed()` использует команду `adb shell pm list packages` для получения списка всех установленных приложений на устройстве. Затем он проверяет, присутствует ли имя пакета в этом списке.
+
+### Исключения
+
+Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может быть вызвано методом `subprocess.check_output()`. Если исключение возникает, оно логируется и метод возвращает `False`.
+
+## Метод: `uninstall_app()`
+
+Этот метод класса `Adb` предназначен для удаления приложения на подключенном устройстве Android.
+
+### Параметры
+
+Метод принимает следующий параметр:
+
+- `package` (`str`): Имя пакета приложения, которое вы хотите удалить.
+
+### Возвращаемое значение
+
+Метод возвращает логическое значение `bool`:
+- `True` - если приложение было успешно удалено с устройства.
+- `False` - если произошла ошибка при удалении приложения.
+
+### Пример использования
+
+```python
+adb = Adb()
+success = adb.uninstall_app("com.example.app")
+if success:
+    print("Приложение успешно удалено с устройства.")
+else:
+    print("Не удалось удалить приложение с устройства.")
+```
+
+### Дополнительная информация
+
+Метод `uninstall_app()` использует команду `adb uninstall` для удаления указанного приложения.
+
+### Исключения
+
+Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может возникнуть при попытке выполнить команду удаления приложения. Если исключение возникает, оно логируется и метод возвращает `False`.
+
 ## Метод: `get_device_model()`
 
 Этот метод класса `Adb` предназначен для получения модели подключенного устройства Android с использованием ADB.
 
 ### Параметры
 
 Метод не принимает никаких параметров.
@@ -3194,48 +3363,14 @@
 
 Метод `pull()` использует команду `adb pull` для копирования файла или директории с устройства.
 
 ### Исключения
 
 Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может быть вызвано методом `subprocess.run()`. Если исключение возникает, оно логируется и метод возвращает `False`.
 
-## Метод: `install()`
-
-Этот метод класса `Adb` предназначен для установки APK-файлов на подключенное устройство Android с использованием ADB.
-
-### Параметры
-
-Метод принимает следующий параметр:
-
-- `source` (`str`): Путь к APK-файлу, который вы хотите установить на устройство.
-
-### Возвращаемое значение
-
-Метод возвращает логическое значение `bool`:
-- `True` - если APK-файл был успешно установлен на устройство.
-- `False` - если произошла ошибка при установке APK-файла.
-
-### Пример использования
-
-```python
-adb = Adb()
-success = adb.install("/path/to/app.apk")
-if success:
-    print("APK успешно установлен на устройство.")
-else:
-    print("Не удалось установить APK на устройство.")
-```
-
-### Дополнительная информация
-
-Метод `install()` использует команду `adb install` для установки APK-файла на устройство. Опция `-r` используется для повторной установки приложения, если оно уже существует на устройстве.
-
-### Исключения
-
-Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может быть вызвано методом `subprocess.run()`. Если исключение возникает, оно логируется и метод возвращает `False`.
 
 ## Метод: `start_activity()`
 
 Этот метод класса `Adb` предназначен для запуска конкретной активности на подключенном устройстве Android с использованием ADB.
 
 ### Параметры
 
@@ -3336,49 +3471,14 @@
 
 Метод `reboot_app()` использует методы `close_app()` и `start_activity()` класса `Adb` для выполнения своей функции.
 
 ### Исключения
 
 Метод не обрабатывает исключения напрямую, но вызываемые им методы `close_app()` и `start_activity()` обрабатывают исключения `subprocess.CalledProcessError`. Если эти методы возвращают `False`, что указывает на появление исключения, то `reboot_app()` также возвращает `False`.
 
-## Метод: `uninstall_app()`
-
-Этот метод класса `Adb` предназначен для удаления приложения на подключенном устройстве Android.
-
-### Параметры
-
-Метод принимает следующий параметр:
-
-- `package` (`str`): Имя пакета приложения, которое вы хотите удалить.
-
-### Возвращаемое значение
-
-Метод возвращает логическое значение `bool`:
-- `True` - если приложение было успешно удалено с устройства.
-- `False` - если произошла ошибка при удалении приложения.
-
-### Пример использования
-
-```python
-adb = Adb()
-success = adb.uninstall_app("com.example.app")
-if success:
-    print("Приложение успешно удалено с устройства.")
-else:
-    print("Не удалось удалить приложение с устройства.")
-```
-
-### Дополнительная информация
-
-Метод `uninstall_app()` использует команду `adb uninstall` для удаления указанного приложения.
-
-### Исключения
-
-Метод обрабатывает исключение `subprocess.CalledProcessError`, которое может возникнуть при попытке выполнить команду удаления приложения. Если исключение возникает, оно логируется и метод возвращает `False`.
-
 ## Метод: `press_home()`
 
 Этот метод класса `Adb` предназначен для отправки события нажатия кнопки Home на подключенном устройстве Android.
 
 ### Параметры
 
 Метод не принимает никаких параметров.
@@ -3837,14 +3937,106 @@
 
 Метод `know_pid()` выполняет команду `adb shell ps` и затем проходит через вывод, пытаясь найти строку, которая содержит имя указанного процесса. Если такая строка найдена, метод извлекает PID из этой строки и возвращает его.
 
 ### Исключения
 
 Метод обрабатывает исключение, которое может возникнуть при попытке выполнить команду ADB. Если исключение возникает, информация об ошибке логируется и метод возвращает `False`. Также, если процесс с указанным именем не найден, метод возвращает `None`.
 
+## Метод: `know_pid()`
+
+Этот метод находит Process ID (PID) процесса по его имени, используя `adb shell ps`.
+
+### Параметры
+
+Метод принимает следующие параметры:
+
+- `name` (str): Имя процесса, PID которого нужно найти.
+
+### Возвращаемое значение
+
+Метод возвращает PID процесса, если он найден, или `None`, если процесс не найден.
+
+### Пример использования
+
+```python
+adb = Adb()
+process_pid = adb.know_pid("my_process")
+if process_pid:
+    print("PID процесса 'my_process' найден.")
+else:
+    print("Процесс 'my_process' не найден.")
+```
+
+### Дополнительная информация
+
+Метод `know_pid()` выполняет команду `adb shell ps` и затем проходит через вывод, пытаясь найти строку, которая содержит имя указанного процесса. Если такая строка найдена, метод извлекает PID из этой строки и возвращает его.
+
+### Исключения
+
+Метод обрабатывает исключение, которое может возникнуть при попытке выполнить команду ADB. Если исключение возникает, информация об ошибке логируется и метод возвращает `False`. Также, если процесс с указанным именем не найден, метод возвращает `None`.
+
+### Метод: `is_process_exist(name)`
+
+Проверяет, запущен ли процесс, используя `adb shell ps`.
+
+#### Параметры
+
+- `name` (str): Имя процесса.
+
+#### Возвращаемое значение
+
+Метод возвращает `True`, если процесс с указанным именем существует, и `False` в ином случае.
+
+#### Пример использования
+
+```python
+adb = Adb()
+if adb.is_process_exist("my_process"):
+    print("Процесс 'my_process' существует.")
+else:
+    print("Процесс 'my_process' не существует.")
+```
+
+Данный метод `is_process_exist()` используется внутри метода `know_pid()` для определения наличия процесса с заданным именем.
+
+
+## Метод: `run_background_process(self, command: str, process: str = "") -> bool`
+
+Запускает процесс в фоновом режиме на устройстве Android с использованием ADB.
+
+### Параметры
+
+- `command` (str): Команда для выполнения на устройстве.
+- `process` (str): Название процесса, который будет запущен. По умолчанию пустая строка (`""`). Если `process == ""`, то не будет проверяться его запуск в системе.
+
+### Возвращаемое значение
+
+Метод возвращает `True`, если процесс был успешно запущен, и `False` в противном случае.
+
+### Пример использования
+
+```python
+adb = Adb()
+command = "my_script.sh"
+process_name = "my_process"
+if adb.run_background_process(command, process_name):
+    print(f"Процесс '{process_name}' был успешно запущен.")
+else:
+    print(f"Не удалось запустить процесс '{process_name}'.")
+```
+
+### Дополнительная информация
+
+Метод `run_background_process()` запускает процесс в фоновом режиме на устройстве Android с использованием команды `adb shell` и `nohup` для выполнения команды без привязки к текущей сессии терминала. Вывод команды перенаправляется в `/dev/null`, чтобы не создавать логов в текущей сессии.
+
+Если указан аргумент `process`, метод проверяет наличие процесса с указанным именем, используя метод `is_process_exist(name)`, чтобы убедиться, что процесс был успешно запущен.
+
+В случае возникновения исключения при выполнении команды, метод возвращает `False`, а также логирует информацию об ошибке.
+
+
 ## Метод: `kill_by_pid()`
 
 Этот метод отправляет сигнал SIGINT для остановки процесса по указанному идентификатору PID с помощью ADB.
 
 ### Параметры
 
 Метод принимает следующий параметр:
```

### Comparing `AppiumExtended-0.1.8/setup.py` & `AppiumExtended-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 An extension library for adding ease of use to Appium-Python-Client.
 
 AppiumExtended is a collection of utilities and convenience functions designed to enhance the usage of Appium-Python-Client for mobile app automation testing. It provides additional functionalities and abstractions to simplify the testing process.
 '''
 
 setup(
     name='AppiumExtended',
-    version='0.1.8',
+    version='0.1.9',
     description='An extension library for adding ease of use Appium-Python-Client',
     author='molokov-klim',
     packages=find_packages(),
     install_requires=[
         'Appium-Python-Client==2.11.1',
         'allure-pytest==2.13.2',
         'zlib-compress==0.0.1',
```

### Comparing `AppiumExtended-0.1.8/terminal/aapt.py` & `AppiumExtended-0.1.9/terminal/aapt.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             raise  # Выбрасываем исключение дальше
 
         logger.info(f"get_package_name() > {package_name}")
         # Возвращение названия пакета в виде строки
         return package_name
 
     @staticmethod
-    def get_launchable_activity_from_apk(path_to_apk: str) -> str:
+    def get_launchable_activity(path_to_apk: str) -> str:
         """
         Получает название запускаемой активности из APK-файла с помощью команды aapt.
         Возвращает название активности в виде строки.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.info(f"get_launchable_activity_from_apk() < {path_to_apk}")
```

### Comparing `AppiumExtended-0.1.8/terminal/adb.py` & `AppiumExtended-0.1.9/terminal/adb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import re
 import subprocess
 import sys
 import time
 import traceback
-from typing import Dict, Union, Tuple
+from typing import Dict, Union, Tuple, Optional, Any
 # sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(
 #    __file__))))  # The sys.path.append line adds the parent directory of the tests directory to the Python module search path, allowing you to import modules from the root folder.
 
 import config
+from utils import operations
 
 
 class Adb:
     def __init__(self):
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
 
     @staticmethod
@@ -26,46 +27,52 @@
         logger.debug("get_device_uuid()")
 
         # Определение команды для выполнения с помощью adb для получения списка устройств
         command = ['adb', 'devices']
 
         try:
             # Выполнение команды и получение вывода
-            response = subprocess.check_output(command)
+            response = str(subprocess.check_output(command))
 
             # Извлечение списка устройств из полученного вывода с использованием регулярных выражений
             device_list = re.findall(r'(\d+\.\d+\.\d+\.\d+:\d+|\d+)', response)
 
-            # Возвращение первого устройства из списка (UUID подключенного устройства Android)
-            logger.debug(f"get_device_uuid() > {device_list[0]}")
-
-            return device_list[0]
+            try:
+                # Возвращение первого устройства из списка (UUID подключенного устройства Android)
+                logger.debug(f"get_device_uuid() > {device_list[0]}")
 
+                return device_list[0]
+            except IndexError:
+                logger.error("get_device_uuid() > None")
+                logger.error("Нет подключенных устройств")
+                return None
         except subprocess.CalledProcessError as e:
             logger.error("get_device_uuid() > None")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
+            return None
 
     @staticmethod
-    def get_device_model() -> Union[str, None]:
+    def get_device_model() -> Optional[str]:
         """
         Получает модель подключенного устройства Android с помощью команды adb.
         Возвращает модель устройства.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug("get_device_model()")
 
         command = ["adb", "shell", "getprop", "ro.product.model"]
         try:
             # Выполнение команды и получение вывода
             model = subprocess.check_output(command)
-            # Возвращение модели устройства в виде строки
-            logger.debug(f"get_device_model() > {model}")
+            # Преобразование байтовой строки в обычную строку и удаление пробельных символов и символов перевода строки
+            model = model.decode().strip()
             return model
+
         except subprocess.CalledProcessError as e:
             logger.error("get_device_model() > None")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
 
     @staticmethod
@@ -76,17 +83,23 @@
         Аргументы:
             source (str): Путь к копируемому файлу или директории.
             destination (str): Путь назначения на устройстве.
 
         Возвращает:
             bool: True, если файл или директория были успешно скопированы, False в противном случае.
         """
+        import os
+
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug(f"push() < {source=}, {destination=}")
 
+        if not os.path.exists(source):
+            logger.error(f"Путь к копируемому файлу или директории не существует: {source=}")
+            return False
+
         command = ["adb", "push", source, destination]
         try:
             subprocess.run(command, check=True)
             logger.debug("push() > True")
             return True
         except subprocess.CalledProcessError as e:
             logger.error("push() > False")
@@ -119,15 +132,15 @@
             logger.error("pull() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
     @staticmethod
-    def install(source: str) -> bool:
+    def install_app(source: str) -> bool:
         """
         Устанавливает файл APK на подключенном устройстве.
 
         Аргументы:
             source (str): Путь к файлу APK для установки.
 
         Возвращает:
@@ -145,14 +158,64 @@
             logger.error("install() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
     @staticmethod
+    def is_app_installed(package) -> bool:
+        """
+        Проверяет, установлен ли пакет.
+        """
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        logger.debug(f"is_installed() < {package=}")
+
+        command = "adb shell pm list packages"
+        try:
+            result = subprocess.check_output(command, shell=True).decode().strip()
+            # Фильтруем пакеты
+            if any([line.strip().endswith(package) for line in result.splitlines()]):
+                logger.debug("install() > True")
+                return True
+            logger.debug("install() > False")
+            return False
+        except subprocess.CalledProcessError as e:
+            logger.error("install() > False")
+            logger.error(e)
+            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+            logger.error(traceback_info)
+            return False
+
+    @staticmethod
+    def uninstall_app(package: str) -> bool:
+        """
+        Удаляет указанный пакет с помощью ADB.
+
+        Аргументы:
+            package (str): Название пакета приложения для удаления.
+
+        Возвращает:
+            bool: True, если приложение успешно удалено, False в противном случае.
+        """
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        logger.debug(f"uninstall_app() < {package=}")
+
+        command = ['adb', 'uninstall', package]
+        try:
+            subprocess.run(command, check=True)
+            logger.debug("uninstall_app() > True")
+            return True
+        except subprocess.CalledProcessError as e:
+            logger.error("uninstall_app() > False")
+            logger.error(e)
+            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+            logger.error(traceback_info)
+            return False
+
+    @staticmethod
     def start_activity(package: str, activity: str) -> bool:
         """
         Запускает активность на подключенном устройстве.
 
         Аргументы:
             package (str): Название пакета активности.
             activity (str): Название запускаемой активности.
@@ -172,14 +235,120 @@
             logger.error("start_activity() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
     @staticmethod
+    def get_current_activity() -> Union[str, None]:
+        """
+        Получает активити текущего запущенного приложения на устройстве с помощью ADB.
+        Возвращает имя активити в виде строки или None, если произошла ошибка.
+
+        Возвращает:
+            str: Название активити текущего запущенного приложения, либо None, если произошла ошибка.
+        """
+        # Получение логгера
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+        # Вывод информации о запуске функции в лог
+        logger.debug("get_current_activity()")
+
+        # Команда для ADB для получения информации о текущих окнах
+        command = ['adb', 'shell', 'dumpsys', 'window', 'windows']
+
+        try:
+            # Выполнение команды и декодирование результата
+            result = subprocess.check_output(command, shell=True).decode().strip()
+
+            # Определение паттерна для поиска нужной информации в результатах
+            pattern = r'mCurrentFocus|mFocusedApp'
+
+            # Вызов функции grep_pattern для поиска соответствия паттерну
+            matched_lines = operations.grep_pattern(input_string=result, pattern=pattern)
+
+            # Если были найдены соответствующие строки
+            if matched_lines:
+                for line in matched_lines:
+                    # Поиск имени активити в строке
+                    match = re.search(r'\/([^\/}]*)', line)
+                    if match:
+                        # Возвращаем найденное значение, исключая '/'
+                        activity_name = match.group(1)
+                        logger.debug(f"get_current_activity() > {activity_name}")
+                        return activity_name
+
+            # Если не удалось найти активити, возвращаем None
+            logger.error("get_current_activity() > None")
+            return None
+        except subprocess.CalledProcessError as e:
+            # Обработка ошибки при выполнении команды
+            logger.error(e)
+
+            # Вывод информации о трассировке в лог
+            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+            logger.error(traceback_info)
+
+            logger.error("get_current_activity() > None")
+            return None
+
+    @staticmethod
+    def get_current_package() -> Union[str, None]:
+        """
+        Получает пакет текущего запущенного приложения на устройстве с помощью ADB.
+        Возвращает имя пакета в виде строки или None, если произошла ошибка.
+
+        Возвращает:
+            str: Название пакета текущего запущенного приложения, либо None, если произошла ошибка.
+        """
+        # Получение логгера
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+
+        # Вывод информации о запуске функции в лог
+        logger.debug("get_current_app_package()")
+
+        # Команда для ADB для получения информации о текущих окнах
+        command = ['adb', 'shell', 'dumpsys', 'window', 'windows']
+
+        try:
+            # Выполнение команды и декодирование результата
+            result = subprocess.check_output(command, shell=True).decode().strip()
+
+            # Определение паттерна для поиска нужной информации в результатах
+            pattern = r'mCurrentFocus|mFocusedApp'
+
+            # Вызов функции grep_pattern для поиска соответствия паттерну
+            matched_lines = operations.grep_pattern(input_string=result, pattern=pattern)
+
+            # Если были найдены соответствующие строки
+            if matched_lines:
+                for line in matched_lines:
+                    # Поиск имени пакета в строке
+                    match = re.search(r'u0\s(.+?)/', line)
+                    if match:
+                        # Возвращаем найденное значение
+                        package_name = match.group(1)
+                        logger.debug(f"get_current_app_package() > {package_name}")
+                        return package_name
+
+            # Если не удалось найти имя пакета, возвращаем None
+            logger.error("get_current_app_package() > None")
+            return None
+        except subprocess.CalledProcessError as e:
+            # Обработка ошибки при выполнении команды
+            logger.error(e)
+
+            # Вывод информации о трассировке в лог
+            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+            logger.error(traceback_info)
+
+            logger.error("get_current_app_package() > None")
+            return None
+
+    @staticmethod
     def close_app(package: str) -> bool:
         """
         Принудительно останавливает указанный пакет с помощью ADB.
     
         Аргументы:
             package (str): Название пакета приложения для закрытия.
     
@@ -223,40 +392,14 @@
         if not self.start_activity(package=package, activity=activity):
             self.logger.error("reboot_app() > False")
             return False
         self.logger.debug("reboot_app() > True")
         return True
 
     @staticmethod
-    def uninstall_app(package: str) -> bool:
-        """
-        Удаляет указанный пакет с помощью ADB.
-
-        Аргументы:
-            package (str): Название пакета приложения для удаления.
-
-        Возвращает:
-            bool: True, если приложение успешно удалено, False в противном случае.
-        """
-        logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        logger.debug(f"uninstall_app() < {package=}")
-
-        command = ['adb', 'uninstall', package]
-        try:
-            subprocess.run(command, check=True)
-            logger.debug("uninstall_app() > True")
-            return True
-        except subprocess.CalledProcessError as e:
-            logger.error("uninstall_app() > False")
-            logger.error(e)
-            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
-            logger.error(traceback_info)
-            return False
-
-    @staticmethod
     def press_home() -> bool:
         """
         Отправляет событие нажатия кнопки Home на устройство с помощью ADB.
 
         Возвращает:
             bool: True, если команда была успешно выполнена, False в противном случае.
         """
@@ -488,114 +631,136 @@
             logger.error("swipe() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
     @staticmethod
-    def get_current_app_package() -> Union[str, None]:
-        """
-        Получает пакет текущего запущенного приложения на устройстве с помощью ADB.
-
-        Возвращает:
-            str: Название пакета текущего запущенного приложения, либо None, если произошла ошибка.
-        """
-        logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        logger.debug("get_current_app_package()")
-
-        # Определяем команду в виде списка строк
-        command = [
-            "adb", "shell", "dumpsys", "window", "windows", "|", "grep", "-E", "'mCurrentFocus|mFocusedApp'",
-            "|", "grep", "-e", "'mFo'"
-        ]
-        try:
-            # Выполняем команду и получаем результат
-            result = str(subprocess.check_output(command)).strip()
-            # Находим позицию последнего вхождения подстроки "/." в строке
-            end_index = result.rfind("/")
-            # Извлекаем название приложения из предшествующих символов
-            start_index = result.rfind(" ", 0, end_index) + 1
-            app_name = result[start_index:end_index]
-            logger.debug(f"get_current_app_package() > {app_name=}")
-            return app_name
-        except subprocess.CalledProcessError as e:
-            # Логируем ошибку, если возникло исключение
-            logger.error("adb.get_current_app_package() > None")
-            logger.error(e)
-            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
-            logger.error(traceback_info)
-            return None
-
-    @staticmethod
     def check_vpn(ip_address: str = '') -> bool:
         """
         Проверяет, активно ли VPN-соединение на устройстве с помощью ADB.
 
         Аргументы:
             ip_address (str): IP-адрес для проверки VPN-соединения. Если не указан, используется значение из конфигурации.
 
         Возвращает:
             bool: True, если VPN-соединение активно, False в противном случае.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
-        logger.debug(f"check_VPN() < {ip_address=}")
+        logger.debug(f"check_vpn() < {ip_address=}")
 
         # Определяем команду в виде строки
-        command = f"adb shell netstat | grep -w -e {ip_address}"
+        command = "adb shell netstat"
         try:
             # Выполняем команду и получаем вывод
             output = subprocess.run(command, shell=True, capture_output=True, text=True, check=True)
 
-            if "ESTABLISHED" in output.stdout:
-                logger.debug("check_VPN() True")
-                return True
-            logger.debug("check_VPN() False")
+            # Поиск строки
+            lines = output.stdout.split("\n")
+            for line in lines:
+                if "ESTABLISHED" in line and ip_address in line:
+                    logger.debug("check_vpn() True")
+                    return True
+            logger.debug("check_vpn() False")
             return False
         except subprocess.CalledProcessError as e:
             # Логируем ошибку, если возникло исключение
-            logger.error("check_VPN() > False")
+            logger.error("check_vpn() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
-    @staticmethod
-    def stop_logcat() -> bool:
+    def stop_logcat(self) -> bool:
         """
         Останавливает выполнение logcat на устройстве с помощью ADB.
 
         Возвращает:
             bool: True, если выполнение logcat остановлено успешно, False в противном случае.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug("stop_logcat()")
+        if self.is_process_exist(name='logcat'):
+            if self.kill_all(name='logcat'):
+                logger.debug("stop_logcat() > True")
+                return True
+        logger.error("stop_logcat() > False")
+        logger.debug("stop_logcat() [Запущенного процесса logcat не обнаружено]")
+        return False
+
+    @staticmethod
+    def is_process_exist(name) -> bool:
+        """
+        Проверяет, запущен ли процесс, используя adb shell ps.
+
+        Параметры:
+            name (str): Имя процесса.
 
-        command = ['adb', 'shell', 'ps', '|', 'grep', 'logcat']
-        # Получаем список выполняющихся процессов logcat
+        Возвращает:
+            bool: True если процесс с указанным именем существует, False в ином случае.
+        """
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        logger.debug(f"is_process_exist() < {name=}")
+        command = ['adb', 'shell', 'ps']
         try:
-            process_list = subprocess.check_output(command)
+            processes = subprocess.check_output(command, shell=True).decode().strip()
         except subprocess.CalledProcessError as e:
-            logger.error("adb.stop_logcat() > False")
+            logger.error("know_pid() > None")
+            logger.error(e)
+            traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
+            logger.error(traceback_info)
+            return False
+        # Разделение вывода на строки и удаление пустых строк
+        lines = processes.strip().split('\n')
+        # Проход по каждой строке вывода, начиная с 2-й строки, игнорируя заголовки
+        for line in lines[1:]:
+            # Разделение строки на столбцы по пробелам
+            columns = line.split()
+            # Проверка, что строка имеет не менее 9 столбцов
+            if len(columns) >= 9:
+                # Извлечение PID и имени процесса из соответствующих столбцов
+                _, process_name = columns[1], columns[8]
+                # Сравнение имени процесса с искомым именем
+                if name == process_name:
+                    logger.debug("is_process_exist() > True")
+                    return True
+        # Возврат None, если процесс с заданным именем не найден
+        logger.debug("is_process_exist() > False")
+        return False
+
+    def run_background_process(self, command: str, process: str = "") -> bool:
+        """
+        Запускает процесс в фоновом режиме на устройстве Android с использованием ADB.
+
+        Аргументы:
+            command (str): Команда для выполнения на устройстве.
+            process (str): Название процесса, который будет запущен. По умолчанию "".
+            Если process == "", то не будет проверяться его запуск в системе.
+
+        Возвращает:
+            bool: True, если процесс был успешно запущен, False в противном случае.
+        """
+        logger = logging.getLogger(config.APPIUM_LOG_NAME)
+        logger.debug(f"run_background_process() < {command=}")
+
+        command = f"{command} nohup > /dev/null 2>&1 &"
+        try:
+            subprocess.Popen(command, stdout=subprocess.DEVNULL)  # не добавлять with
+            if process != "":
+                time.sleep(1)
+                if not self.is_process_exist(name=process):
+                    return False
+            logger.debug("run_background_process() > True")
+            return True
+        except subprocess.CalledProcessError as e:
+            logger.error("run_background_process() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
-        # Проходим по списку процессов и отправляем каждому сигнал SIGINT
-        for process in process_list.splitlines():
-            pid = process.split()[1]
-            try:
-                subprocess.call(['adb', 'shell', 'kill', '-s', 'SIGINT', pid])
-            except subprocess.CalledProcessError as e:
-                logger.error("adb.stop_logcat() > False")
-                logger.error(e)
-                traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
-                logger.error(traceback_info)
-                return False
-        logger.debug("stop_logcat() > True")
-        return True
 
     @staticmethod
     def reload_adb() -> bool:
         """
         Перезапускает adb-сервер на устройстве.
 
         Возвращает:
@@ -638,25 +803,21 @@
         Возвращает:
             Union[int, None]: PID процесса, если он найден, или None, если процесс не найден.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug(f"know_pid() < {name=}")
         command = ['adb', 'shell', 'ps']
         try:
-            processes = str(subprocess.call(command)).strip()
+            processes = subprocess.check_output(command, shell=True).decode().strip()
         except subprocess.CalledProcessError as e:
-            logger.error("know_pid() > False")
+            logger.error("know_pid() > None")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
-            return False
-        if name not in processes:
-            logger.error("know_pid() > False")
-            logger.error("know_pid() [Процесс не обнаружен]")
-            return False
+            return None
         # Разделение вывода на строки и удаление пустых строк
         lines = processes.strip().split('\n')
         # Проход по каждой строке вывода, начиная с 2-й строки, игнорируя заголовки
         for line in lines[1:]:
             # Разделение строки на столбцы по пробелам
             columns = line.split()
             # Проверка, что строка имеет не менее 9 столбцов
@@ -665,18 +826,19 @@
                 pid, process_name = columns[1], columns[8]
                 # Сравнение имени процесса с искомым именем
                 if name == process_name:
                     logger.debug(f"know_pid() > {pid=}")
                     return int(pid)
         # Возврат None, если процесс с заданным именем не найден
         logger.error("know_pid() > None")
+        logger.error("know_pid() [Процесс не обнаружен]")
         return None
 
     @staticmethod
-    def kill_by_pid(pid: str) -> bool:
+    def kill_by_pid(pid: Union[str, int]) -> bool:
         """
         Отправляет сигнал SIGINT для остановки процесса по указанному идентификатору PID с помощью ADB.
 
         Аргументы:
             pid (str): Идентификатор PID процесса для остановки.
 
         Возвращает:
@@ -735,15 +897,15 @@
             bool: True, если все процессы успешно остановлены, False в противном случае.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug(f"kill_all() < {name=}")
 
         command = ['adb', 'shell', 'pkill', '-f', str(name)]
         try:
-            subprocess.call(command)
+            subprocess.run(command, check=True)
         except subprocess.CalledProcessError as e:
             logger.error("kill_all() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
         logger.debug("kill_all() > True")
@@ -772,53 +934,50 @@
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
         logger.debug("delete_files_from_internal_storage() > True")
         return True
 
     @staticmethod
-    def pull_video(wherefrom: str = None, destination: str = "", delete: bool = True) -> bool:
+    def pull_video(source: str = None, destination: str = ".", delete: bool = True) -> bool:
         """
         Копирует видеофайлы с устройства на компьютер с помощью ADB.
 
         Аргументы:
             wherefrom (str): Путь к исходным видеофайлам на устройстве.
             destination (str): Путь для сохранения скопированных видеофайлов.
             delete (bool): Удалять исходные видеофайлы с устройства после копирования (по умолчанию True).
 
         Возвращает:
             bool: True, если видеофайлы успешно скопированы, False в противном случае.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug(f"pull_video() < {destination=}")
 
-        if not wherefrom:
-            wherefrom = '/sdcard/Movies/'
-        if wherefrom.endswith('/'):
-            wherefrom = wherefrom + "/"
+        if not source:
+            source = '/sdcard/Movies/'
+        if source.endswith('/'):
+            source = source + "/"
         if destination.endswith('/'):
             destination = destination + "/"
 
-        command = ['adb', 'pull', f'{wherefrom}', f'{destination}']
+        command = ['adb', 'pull', f'{source}', f'{destination}']
         try:
-            with subprocess.Popen(command) as process:
-                process.communicate()
-            time.sleep(30)
+            subprocess.run(command, check=True)
         except subprocess.CalledProcessError as e:
             logger.error("pull_video() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
 
         if delete:
-            command = ['adb', 'shell', 'rm', '-rf', f'{wherefrom}*']
+            command = ['adb', 'shell', 'rm', '-rf', f'{source}*']
             try:
-                with subprocess.Popen(command) as process:
-                    process.communicate()
+                subprocess.run(command, check=True)
             except subprocess.CalledProcessError as e:
                 logger.error("pull_video() > False")
                 logger.error(e)
                 traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
                 logger.error(traceback_info)
                 return False
 
@@ -845,44 +1004,69 @@
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
             return False
         logger.debug("stop_video() > True")
         return True
 
     @staticmethod
-    def record_video(filename: str) -> bool:
+    def record_video(path: str = "sdcard/Movies/", filename: str = "screenrecord.mp4") -> \
+            Union[subprocess.Popen[bytes], subprocess.Popen[Union[Union[str, bytes], Any]]]:
         """
         Записывает видео на устройстве с помощью ADB.
 
         Аргументы:
+            path (str): Путь куда сохранить файл
             filename (str): Имя файла для сохранения видео.
 
         Возвращает:
-            bool: True, если запись видео успешно начата, False в противном случае.
+            subprocess.CompletedProcess: Процесс записи видео.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug(f"record_video() < {filename}")
+        if path.endswith('/'):
+            path = path[:-1]
+        if filename.endswith('.mp4'):
+            filename = filename + ".mp4"
 
-        command = ['adb', 'shell', 'screenrecord', f'sdcard/Movies/{filename}']
+        command = ['adb', 'shell', 'screenrecord', f'{path}/{filename}']
         try:
             # Запускаем команду adb shell screenrecord для начала записи видео
-            with subprocess.Popen(command) as process:
-                # Ожидаем завершения процесса записи видео
-                process.communicate()
+            return subprocess.Popen(command)
         except subprocess.CalledProcessError as e:
             # Если произошла ошибка при выполнении команды, логируем ошибку и возвращаем False
             logger.error("record_video() > False")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
-            return False
 
-        # Возвращаем True, т.к. запись видео начата успешно
-        logger.debug("record_video() > True")
-        return True
+    @staticmethod
+    def start_record_video(path: str = "sdcard/Movies/", filename: str = "screenrecord.mp4") -> bool:
+        """
+        Отправляет команду на устройство для начала записи видео.
+
+        Аргументы:
+            path (str): Путь куда сохранить файл
+            filename (str): Имя файла для сохранения видео.
+
+        Возвращает:
+            bool: True, если запись видео успешно начата, False в противном случае.
+        """
+        if path.endswith('/'):
+            path = path[:-1]
+        if not filename.endswith('.mp4'):
+            filename = filename + ".mp4"
+
+        command = ['adb', 'shell', 'screenrecord', f'{path}/{filename}']
+        try:
+            # Запускаем команду adb shell screenrecord для начала записи видео
+            subprocess.Popen(command)   # не добавлять with
+            return True
+        except subprocess.CalledProcessError:
+            # Если произошла ошибка при выполнении команды, возвращаем False
+            return False
 
     @staticmethod
     def reboot() -> bool:
         """
         Перезагружает устройство с помощью ADB.
 
         Возвращает:
@@ -912,20 +1096,21 @@
             tuple[int, int] or None: Кортеж с шириной и высотой экрана в пикселях, или None в случае ошибки.
         """
         logger = logging.getLogger(config.APPIUM_LOG_NAME)
         logger.debug("get_screen_resolution()")
 
         command = ['adb', 'shell', 'wm', 'size']
         try:
-            output = str(subprocess.run(command, check=True)).strip()
+            output = subprocess.check_output(command).decode()
             if "Physical size" in output:
                 resolution_str = output.split(":")[1].strip()
                 width, height = resolution_str.split("x")
                 logger.debug(f"get_screen_resolution() > {width=}, {height=}")
                 return int(width), int(height)
-        except subprocess.CalledProcessError as e:
+            logger.error(f"Unexpected output from adb: {output}")
+        except (subprocess.CalledProcessError, ValueError) as e:
             logger.error("get_screen_resolution() > None")
             logger.error(e)
             traceback_info = "".join(traceback.format_tb(sys.exc_info()[2]))
             logger.error(traceback_info)
-            return None
+        return None
```

### Comparing `AppiumExtended-0.1.8/utils/operations.py` & `AppiumExtended-0.1.9/utils/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,7 +156,14 @@
     """
     # Преобразуем аргумент в строку (на случай, если он уже является строкой)
     number = str(number)
     # Заменяем запятую на точку и удаляем символы "₽" и пробелы, затем преобразуем в float
     number = float(number.replace(',', '.').replace('₽', '').replace(' ', ''))
     # Возвращаем сумму в формате float
     return number
+
+
+def grep_pattern(input_string, pattern):
+    lines = input_string.split('\n')
+    regex = re.compile(pattern)
+    matched_lines = [line for line in lines if regex.search(line)]
+    return matched_lines
```

### Comparing `AppiumExtended-0.1.8/utils/utils.py` & `AppiumExtended-0.1.9/utils/utils.py`

 * *Files identical despite different names*

