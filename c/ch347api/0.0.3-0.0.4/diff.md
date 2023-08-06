# Comparing `tmp/ch347api-0.0.3.tar.gz` & `tmp/ch347api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch347api-0.0.3.tar", last modified: Thu Nov 24 03:08:42 2022, max compression
+gzip compressed data, was "ch347api-0.0.4.tar", last modified: Mon Nov 28 06:30:56 2022, max compression
```

## Comparing `ch347api-0.0.3.tar` & `ch347api-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-11-24 03:08:42.032206 ch347api-0.0.3/
--rw-rw-rw-   0        0        0     1087 2022-11-22 02:17:19.000000 ch347api-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1783 2022-11-24 03:08:42.023479 ch347api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2022-11-24 02:01:30.000000 ch347api-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-24 03:08:41.905206 ch347api-0.0.3/ch347api/
--rw-rw-rw-   0        0        0      186 1970-01-01 00:00:00.000000 ch347api-0.0.3/ch347api/__init__.py
--rw-rw-rw-   0        0        0    12974 2022-11-24 02:56:43.000000 ch347api-0.0.3/ch347api/spi.py
-drwxrwxrwx   0        0        0        0 2022-11-24 03:08:42.012045 ch347api-0.0.3/ch347api.egg-info/
--rw-rw-rw-   0        0        0     1783 2022-11-24 03:08:41.000000 ch347api-0.0.3/ch347api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2022-11-24 03:08:41.000000 ch347api-0.0.3/ch347api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-24 03:08:41.000000 ch347api-0.0.3/ch347api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-11-24 03:08:41.000000 ch347api-0.0.3/ch347api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-24 03:08:41.000000 ch347api-0.0.3/ch347api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-24 03:08:42.032206 ch347api-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1328 2022-11-24 02:28:25.000000 ch347api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-28 06:30:56.093967 ch347api-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2022-11-22 02:17:19.000000 ch347api-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1779 2022-11-28 06:30:56.089968 ch347api-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1028 2022-11-28 06:29:43.000000 ch347api-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2022-11-28 06:30:56.042951 ch347api-0.0.4/ch347api/
+-rw-rw-rw-   0        0        0      186 1970-01-01 00:00:00.000000 ch347api-0.0.4/ch347api/__init__.py
+-rw-rw-rw-   0        0        0    12974 2022-11-24 02:56:43.000000 ch347api-0.0.4/ch347api/spi.py
+drwxrwxrwx   0        0        0        0 2022-11-28 06:30:56.084297 ch347api-0.0.4/ch347api.egg-info/
+-rw-rw-rw-   0        0        0     1779 2022-11-28 06:30:55.000000 ch347api-0.0.4/ch347api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2022-11-28 06:30:55.000000 ch347api-0.0.4/ch347api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-28 06:30:55.000000 ch347api-0.0.4/ch347api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2022-11-28 06:30:55.000000 ch347api-0.0.4/ch347api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-11-28 06:30:55.000000 ch347api-0.0.4/ch347api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-28 06:30:56.093967 ch347api-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2022-11-28 06:30:53.000000 ch347api-0.0.4/setup.py
```

### Comparing `ch347api-0.0.3/LICENSE` & `ch347api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ch347api-0.0.3/PKG-INFO` & `ch347api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch347api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library provides full access of SPI settings and communication with CH347 USB-SPI bridge chip in Python language.
 Home-page: https://github.com/i2cy/ch347-hidapi
 Author: I2cy Cloud
 Author-email: i2cy@outlook.com
 Project-URL: Bug Tracker, https://github.com/i2cy/ch347-hidapi/issues
 Project-URL: Source Code, https://github.com/i2cy/ch347-hidapi
 Project-URL: Documentation, https://github.com/i2cy/CH347-HIDAPI/blob/master/README.md
@@ -26,15 +26,15 @@
 </div>
 
 <p align="center">
   <a href="https://github.com/i2cy/ch347-hidapi/master/LICENSE">
     <img src="https://img.shields.io/github/license/i2cy/ch347-hidapi.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/ch347api">
-    <img src="https://img.shields.io/pypi/v/ch347-hidapi.svg" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/ch347api.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </p>
 
 ## Abstract
 This project is the API library of CH347 USB-SPI bridge chip based on Python.
 Only support standard USB-HID mode setting of CH347 chip.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ch347api Version: 0.0.3 Summary: A Python Library
+Metadata-Version: 2.1 Name: ch347api Version: 0.0.4 Summary: A Python Library
 provides full access of SPI settings and communication with CH347 USB-SPI
 bridge chip in Python language. Home-page: https://github.com/i2cy/ch347-hidapi
 Author: I2cy Cloud Author-email: i2cy@outlook.com Project-URL: Bug Tracker,
 https://github.com/i2cy/ch347-hidapi/issues Project-URL: Source Code, https://
 github.com/i2cy/ch347-hidapi Project-URL: Documentation, https://github.com/
 i2cy/CH347-HIDAPI/blob/master/README.md Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `ch347api-0.0.3/README.md` & `ch347api-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </div>
 
 <p align="center">
   <a href="https://github.com/i2cy/ch347-hidapi/master/LICENSE">
     <img src="https://img.shields.io/github/license/i2cy/ch347-hidapi.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/ch347api">
-    <img src="https://img.shields.io/pypi/v/ch347-hidapi.svg" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/ch347api.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </p>
 
 ## Abstract
 This project is the API library of CH347 USB-SPI bridge chip based on Python.
 Only support standard USB-HID mode setting of CH347 chip.
```

### Comparing `ch347api-0.0.3/ch347api/spi.py` & `ch347api-0.0.4/ch347api/spi.py`

 * *Files identical despite different names*

### Comparing `ch347api-0.0.3/ch347api.egg-info/PKG-INFO` & `ch347api-0.0.4/ch347api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch347api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library provides full access of SPI settings and communication with CH347 USB-SPI bridge chip in Python language.
 Home-page: https://github.com/i2cy/ch347-hidapi
 Author: I2cy Cloud
 Author-email: i2cy@outlook.com
 Project-URL: Bug Tracker, https://github.com/i2cy/ch347-hidapi/issues
 Project-URL: Source Code, https://github.com/i2cy/ch347-hidapi
 Project-URL: Documentation, https://github.com/i2cy/CH347-HIDAPI/blob/master/README.md
@@ -26,15 +26,15 @@
 </div>
 
 <p align="center">
   <a href="https://github.com/i2cy/ch347-hidapi/master/LICENSE">
     <img src="https://img.shields.io/github/license/i2cy/ch347-hidapi.svg" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/ch347api">
-    <img src="https://img.shields.io/pypi/v/ch347-hidapi.svg" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/ch347api.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="python">
 </p>
 
 ## Abstract
 This project is the API library of CH347 USB-SPI bridge chip based on Python.
 Only support standard USB-HID mode setting of CH347 chip.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ch347api Version: 0.0.3 Summary: A Python Library
+Metadata-Version: 2.1 Name: ch347api Version: 0.0.4 Summary: A Python Library
 provides full access of SPI settings and communication with CH347 USB-SPI
 bridge chip in Python language. Home-page: https://github.com/i2cy/ch347-hidapi
 Author: I2cy Cloud Author-email: i2cy@outlook.com Project-URL: Bug Tracker,
 https://github.com/i2cy/ch347-hidapi/issues Project-URL: Source Code, https://
 github.com/i2cy/ch347-hidapi Project-URL: Documentation, https://github.com/
 i2cy/CH347-HIDAPI/blob/master/README.md Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `ch347api-0.0.3/setup.py` & `ch347api-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ch347api",
-    version="0.0.3",
+    version="0.0.4",
     author="I2cy Cloud",
     author_email="i2cy@outlook.com",
     description="A Python Library provides full access of SPI settings and communication"
                 " with CH347 USB-SPI bridge chip in Python language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/i2cy/ch347-hidapi",
```

