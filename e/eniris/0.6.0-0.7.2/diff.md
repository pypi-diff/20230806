# Comparing `tmp/eniris-0.6.0.tar.gz` & `tmp/eniris-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.6.0.tar", last modified: Thu Jul 13 16:18:34 2023, max compression
+gzip compressed data, was "eniris-0.7.2.tar", last modified: Sun Aug  6 16:14:35 2023, max compression
```

## Comparing `eniris-0.6.0.tar` & `eniris-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 16:18:24.000000 eniris-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-13 16:18:34.665442 eniris-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-13 16:18:24.000000 eniris-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-13 16:18:24.000000 eniris-0.6.0/eniris/ApiDriver.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 16:18:24.000000 eniris-0.6.0/eniris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:18:34.665442 eniris-0.6.0/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 16:18:34.000000 eniris-0.6.0/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:18:34.665442 eniris-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 16:18:24.000000 eniris-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.084597 eniris-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 16:14:20.000000 eniris-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 16:14:35.084597 eniris-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 16:14:20.000000 eniris-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.080597 eniris-0.7.2/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 16:14:20.000000 eniris-0.7.2/eniris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-08-06 16:14:20.000000 eniris-0.7.2/eniris/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:14:35.084597 eniris-0.7.2/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 16:14:35.000000 eniris-0.7.2/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 16:14:35.084597 eniris-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 16:14:20.000000 eniris-0.7.2/setup.py
```

### Comparing `eniris-0.6.0/LICENSE` & `eniris-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.6.0/PKG-INFO` & `eniris-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.6.0
+Version: 0.7.2
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
 Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
```

### Comparing `eniris-0.6.0/README.md` & `eniris-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.6.0/eniris.egg-info/PKG-INFO` & `eniris-0.7.2/eniris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.6.0
+Version: 0.7.2
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
 Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
```

### Comparing `eniris-0.6.0/setup.py` & `eniris-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 with open("README.md", 'r') as f:
     long_description = f.read()
     
 setup(
   name = 'eniris',
   packages = ['eniris'],
-  version = '0.6.0',
+  version = '0.7.2',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
   download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.6.0.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
-    'requests',
+    'requests'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
```

