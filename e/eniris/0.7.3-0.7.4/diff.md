# Comparing `tmp/eniris-0.7.3.tar.gz` & `tmp/eniris-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.7.3.tar", last modified: Sun Aug  6 17:14:39 2023, max compression
+gzip compressed data, was "eniris-0.7.4.tar", last modified: Sun Aug  6 17:53:46 2023, max compression
```

## Comparing `eniris-0.7.3.tar` & `eniris-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:14:27.000000 eniris-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:14:39.453792 eniris-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 17:14:27.000000 eniris-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 17:14:27.000000 eniris-0.7.3/eniris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 17:14:27.000000 eniris-0.7.3/eniris/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:14:39.453792 eniris-0.7.3/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 17:14:39.000000 eniris-0.7.3/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:14:39.453792 eniris-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:14:27.000000 eniris-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:53:46.847840 eniris-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:53:37.000000 eniris-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:53:46.847840 eniris-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 17:53:37.000000 eniris-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:53:46.847840 eniris-0.7.4/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 17:53:37.000000 eniris-0.7.4/eniris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 17:53:37.000000 eniris-0.7.4/eniris/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:53:46.847840 eniris-0.7.4/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 17:53:46.000000 eniris-0.7.4/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 17:53:46.000000 eniris-0.7.4/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:53:46.000000 eniris-0.7.4/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 17:53:46.000000 eniris-0.7.4/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 17:53:46.000000 eniris-0.7.4/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:53:46.847840 eniris-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 17:53:37.000000 eniris-0.7.4/setup.py
```

### Comparing `eniris-0.7.3/LICENSE` & `eniris-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.7.3/PKG-INFO` & `eniris-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.3
+Version: 0.7.4
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.4.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.3/README.md` & `eniris-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.7.3/eniris/driver.py` & `eniris-0.7.4/eniris/driver.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.3/eniris.egg-info/PKG-INFO` & `eniris-0.7.4/eniris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.3
+Version: 0.7.4
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.4.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.3/setup.py` & `eniris-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.7.3',
+  version = '0.7.4',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.4.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

