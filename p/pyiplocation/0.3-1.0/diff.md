# Comparing `tmp/pyiplocation-0.3.tar.gz` & `tmp/pyiplocation-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiplocation-0.3.tar", last modified: Sat Aug  5 13:46:46 2023, max compression
+gzip compressed data, was "pyiplocation-1.0.tar", last modified: Sun Aug  6 13:50:59 2023, max compression
```

## Comparing `pyiplocation-0.3.tar` & `pyiplocation-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.584478 pyiplocation-0.3/
--rw-rw-rw-   0        0        0     1107 2023-08-04 10:34:13.000000 pyiplocation-0.3/LICENSE
--rw-rw-rw-   0        0        0     1495 2023-08-05 13:46:46.583475 pyiplocation-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-08-05 13:30:20.000000 pyiplocation-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.563865 pyiplocation-0.3/pyiplocation/
--rw-rw-rw-   0        0        0     2760 2023-08-04 21:22:43.000000 pyiplocation-0.3/pyiplocation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 13:46:46.582464 pyiplocation-0.3/pyiplocation.egg-info/
--rw-rw-rw-   0        0        0     1495 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 13:46:46.000000 pyiplocation-0.3/pyiplocation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 13:46:46.585500 pyiplocation-0.3/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-08-05 13:46:39.000000 pyiplocation-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 13:50:59.283739 pyiplocation-1.0/
+-rw-rw-rw-   0        0        0     1107 2023-08-04 10:34:13.000000 pyiplocation-1.0/LICENSE
+-rw-rw-rw-   0        0        0     1598 2023-08-06 13:50:59.283739 pyiplocation-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-08-06 13:49:52.000000 pyiplocation-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 13:50:59.250184 pyiplocation-1.0/pyiplocation/
+-rw-rw-rw-   0        0        0     2760 2023-08-04 21:22:43.000000 pyiplocation-1.0/pyiplocation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 13:50:59.280176 pyiplocation-1.0/pyiplocation.egg-info/
+-rw-rw-rw-   0        0        0     1598 2023-08-06 13:50:59.000000 pyiplocation-1.0/pyiplocation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-08-06 13:50:59.000000 pyiplocation-1.0/pyiplocation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 13:50:59.000000 pyiplocation-1.0/pyiplocation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 13:50:59.000000 pyiplocation-1.0/pyiplocation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-06 13:50:59.000000 pyiplocation-1.0/pyiplocation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 13:50:59.285003 pyiplocation-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      851 2023-08-06 13:50:46.000000 pyiplocation-1.0/setup.py
```

### Comparing `pyiplocation-0.3/LICENSE` & `pyiplocation-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiplocation-0.3/PKG-INFO` & `pyiplocation-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiplocation
-Version: 0.3
+Version: 1.0
 Summary: A package for geolocating IPs
 Home-page: https://github.com/gugu256/gugu256
 Author: gugu256
 Author-email: gugu256@mail.com
 License: MIT
 Project-URL: Homepage, https://github.com/gugu256/pyiplocation
 Keywords: ip location
@@ -15,14 +15,16 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyiplocation
 
+[![Downloads](https://static.pepy.tech/badge/pyiplocation)](https://pepy.tech/project/pyiplocation)
+
 A simple python package to geolocate IPs without the need for a paid/limited API.<br>
 
 ## Usage
 
 This code snippet :
 ```py
 from pyiplocation import geolocate
```

### Comparing `pyiplocation-0.3/README.md` & `pyiplocation-1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pyiplocation
 
+[![Downloads](https://static.pepy.tech/badge/pyiplocation)](https://pepy.tech/project/pyiplocation)
+
 A simple python package to geolocate IPs without the need for a paid/limited API.<br>
 
 ## Usage
 
 This code snippet :
 ```py
 from pyiplocation import geolocate
```

### Comparing `pyiplocation-0.3/pyiplocation/__init__.py` & `pyiplocation-1.0/pyiplocation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiplocation-0.3/pyiplocation.egg-info/PKG-INFO` & `pyiplocation-1.0/pyiplocation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiplocation
-Version: 0.3
+Version: 1.0
 Summary: A package for geolocating IPs
 Home-page: https://github.com/gugu256/gugu256
 Author: gugu256
 Author-email: gugu256@mail.com
 License: MIT
 Project-URL: Homepage, https://github.com/gugu256/pyiplocation
 Keywords: ip location
@@ -15,14 +15,16 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyiplocation
 
+[![Downloads](https://static.pepy.tech/badge/pyiplocation)](https://pepy.tech/project/pyiplocation)
+
 A simple python package to geolocate IPs without the need for a paid/limited API.<br>
 
 ## Usage
 
 This code snippet :
 ```py
 from pyiplocation import geolocate
```

### Comparing `pyiplocation-0.3/setup.py` & `pyiplocation-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='pyiplocation',
-    version='0.3',
+    version='1.0',
     license='MIT',
     description= "A package for geolocating IPs",
     long_description= open("README.md").read(),
     long_description_content_type= "text/markdown",
     project_urls={"Homepage": "https://github.com/gugu256/pyiplocation"},
     author="gugu256",
     author_email='gugu256@mail.com',
```

