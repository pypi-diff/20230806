# Comparing `tmp/requests_selenium-0.0.3.tar.gz` & `tmp/requests_selenium-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_selenium-0.0.3.tar", last modified: Sun Aug  6 14:43:39 2023, max compression
+gzip compressed data, was "requests_selenium-0.0.4.tar", last modified: Sun Aug  6 14:50:36 2023, max compression
```

## Comparing `requests_selenium-0.0.3.tar` & `requests_selenium-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:43:39.948254 requests_selenium-0.0.3/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 14:43:39.948068 requests_selenium-0.0.3/PKG-INFO
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:43:39.946955 requests_selenium-0.0.3/requests_selenium/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      333 2023-08-06 14:43:30.000000 requests_selenium-0.0.3/requests_selenium/__init__.py
--rw-r--r--   0 benbavonese1   (502) staff       (20)     1309 2023-08-03 16:22:41.000000 requests_selenium-0.0.3/requests_selenium/selenium_utils.py
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:43:39.947841 requests_selenium-0.0.3/requests_selenium.egg-info/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 14:43:39.000000 requests_selenium-0.0.3/requests_selenium.egg-info/PKG-INFO
--rw-r--r--   0 benbavonese1   (502) staff       (20)      278 2023-08-06 14:43:39.000000 requests_selenium-0.0.3/requests_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-06 14:43:39.000000 requests_selenium-0.0.3/requests_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       60 2023-08-06 14:43:39.000000 requests_selenium-0.0.3/requests_selenium.egg-info/requires.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       18 2023-08-06 14:43:39.000000 requests_selenium-0.0.3/requests_selenium.egg-info/top_level.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       38 2023-08-06 14:43:39.948304 requests_selenium-0.0.3/setup.cfg
--rw-r--r--   0 benbavonese1   (502) staff       (20)      918 2023-08-06 14:42:27.000000 requests_selenium-0.0.3/setup.py
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:50:36.188966 requests_selenium-0.0.4/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 14:50:36.188790 requests_selenium-0.0.4/PKG-INFO
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:50:36.187917 requests_selenium-0.0.4/requests_selenium/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      674 2023-08-06 14:50:11.000000 requests_selenium-0.0.4/requests_selenium/__init__.py
+-rw-r--r--   0 benbavonese1   (502) staff       (20)     1309 2023-08-03 16:22:41.000000 requests_selenium-0.0.4/requests_selenium/selenium_utils.py
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 14:50:36.188601 requests_selenium-0.0.4/requests_selenium.egg-info/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 14:50:36.000000 requests_selenium-0.0.4/requests_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      278 2023-08-06 14:50:36.000000 requests_selenium-0.0.4/requests_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-06 14:50:36.000000 requests_selenium-0.0.4/requests_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       60 2023-08-06 14:50:36.000000 requests_selenium-0.0.4/requests_selenium.egg-info/requires.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       18 2023-08-06 14:50:36.000000 requests_selenium-0.0.4/requests_selenium.egg-info/top_level.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       38 2023-08-06 14:50:36.189006 requests_selenium-0.0.4/setup.cfg
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      918 2023-08-06 14:50:24.000000 requests_selenium-0.0.4/setup.py
```

### Comparing `requests_selenium-0.0.3/PKG-INFO` & `requests_selenium-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests_selenium
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for fetching page source using Selenium
 Author: Ben Bavonese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `requests_selenium-0.0.3/requests_selenium/selenium_utils.py` & `requests_selenium-0.0.4/requests_selenium/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `requests_selenium-0.0.3/requests_selenium.egg-info/PKG-INFO` & `requests_selenium-0.0.4/requests_selenium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-selenium
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for fetching page source using Selenium
 Author: Ben Bavonese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `requests_selenium-0.0.3/setup.py` & `requests_selenium-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='requests_selenium',
-    version='0.0.3',
+    version='0.0.4',
     description='A Python package for fetching page source using Selenium',
     author='Ben Bavonese',
     packages=find_packages(), 
     install_requires=[
         'requests',
         'beautifulsoup4',
         'chromedriver_autoinstaller',
```

