# Comparing `tmp/mediumvers123-0.1.0.tar.gz` & `tmp/mediumvers123-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediumvers123-0.1.0.tar", last modified: Thu Jul 20 15:15:36 2023, max compression
+gzip compressed data, was "mediumvers123-0.1.2.tar", last modified: Sun Aug  6 16:50:47 2023, max compression
```

## Comparing `mediumvers123-0.1.0.tar` & `mediumvers123-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 15:15:36.530345 mediumvers123-0.1.0/
--rw-rw-rw-   0        0        0     1166 2023-07-20 15:15:36.530345 mediumvers123-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-07-20 15:13:31.000000 mediumvers123-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 15:15:36.466344 mediumvers123-0.1.0/medium_multi/
--rw-rw-rw-   0        0        0        0 2023-07-19 14:32:18.000000 mediumvers123-0.1.0/medium_multi/__init__.py
--rw-rw-rw-   0        0        0      769 2023-07-19 14:32:18.000000 mediumvers123-0.1.0/medium_multi/multi.py
-drwxrwxrwx   0        0        0        0 2023-07-20 15:15:36.482345 mediumvers123-0.1.0/mediumvers123.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-07-20 15:15:36.000000 mediumvers123-0.1.0/mediumvers123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-07-20 15:15:36.000000 mediumvers123-0.1.0/mediumvers123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 15:15:36.000000 mediumvers123-0.1.0/mediumvers123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 15:15:36.000000 mediumvers123-0.1.0/mediumvers123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-20 15:15:36.000000 mediumvers123-0.1.0/mediumvers123.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 15:15:36.538349 mediumvers123-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1330 2023-07-20 15:13:04.000000 mediumvers123-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 15:15:36.530345 mediumvers123-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-19 14:32:18.000000 mediumvers123-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1372 2023-07-19 14:46:24.000000 mediumvers123-0.1.0/tests/multi_tests.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:50:47.897845 mediumvers123-0.1.2/
+-rw-rw-rw-   0        0        0     1166 2023-08-06 16:50:47.896329 mediumvers123-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-20 15:13:31.000000 mediumvers123-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 16:50:47.873557 mediumvers123-0.1.2/medium_multi/
+-rw-rw-rw-   0        0        0        0 2023-07-19 14:32:18.000000 mediumvers123-0.1.2/medium_multi/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-07-19 14:32:18.000000 mediumvers123-0.1.2/medium_multi/multi.py
+-rw-rw-rw-   0        0        0    15671 2023-08-06 15:53:21.000000 mediumvers123-0.1.2/medium_multi/stats.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:50:47.881565 mediumvers123-0.1.2/mediumvers123.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-08-06 16:50:47.000000 mediumvers123-0.1.2/mediumvers123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-08-06 16:50:47.000000 mediumvers123-0.1.2/mediumvers123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 16:50:47.000000 mediumvers123-0.1.2/mediumvers123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-06 16:50:47.000000 mediumvers123-0.1.2/mediumvers123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-06 16:50:47.000000 mediumvers123-0.1.2/mediumvers123.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 16:50:47.897845 mediumvers123-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1387 2023-08-06 16:49:00.000000 mediumvers123-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:50:47.889557 mediumvers123-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-19 14:32:18.000000 mediumvers123-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-07-19 14:46:24.000000 mediumvers123-0.1.2/tests/multi_tests.py
```

### Comparing `mediumvers123-0.1.0/PKG-INFO` & `mediumvers123-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediumvers123
-Version: 0.1.0
+Version: 0.1.2
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mediumvers123-0.1.0/medium_multi/multi.py` & `mediumvers123-0.1.2/medium_multi/multi.py`

 * *Files identical despite different names*

### Comparing `mediumvers123-0.1.0/mediumvers123.egg-info/PKG-INFO` & `mediumvers123-0.1.2/mediumvers123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediumvers123
-Version: 0.1.0
+Version: 0.1.2
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `mediumvers123-0.1.0/setup.py` & `mediumvers123-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="mediumvers123",
-    version="0.1.0",
+    version="0.1.2",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
@@ -33,9 +33,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["numpy"]
+    install_requires=["numpy","pandas","scipy","sklearn","reportlab","matplotlib","io"]
 )
```

### Comparing `mediumvers123-0.1.0/tests/multi_tests.py` & `mediumvers123-0.1.2/tests/multi_tests.py`

 * *Files identical despite different names*

