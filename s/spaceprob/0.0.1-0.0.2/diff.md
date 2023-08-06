# Comparing `tmp/spaceprob-0.0.1.tar.gz` & `tmp/spaceprob-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceprob-0.0.1.tar", last modified: Sun Aug  6 16:22:51 2023, max compression
+gzip compressed data, was "spaceprob-0.0.2.tar", last modified: Sun Aug  6 16:55:48 2023, max compression
```

## Comparing `spaceprob-0.0.1.tar` & `spaceprob-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 16:22:51.143525 spaceprob-0.0.1/
--rw-rw-rw-   0        0        0       81 2023-08-06 16:12:12.000000 spaceprob-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1065 2023-08-06 16:14:27.000000 spaceprob-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-08-06 16:12:46.000000 spaceprob-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      686 2023-08-06 16:22:51.141529 spaceprob-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-08-06 16:17:24.000000 spaceprob-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 16:22:51.143525 spaceprob-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-08-06 16:19:13.000000 spaceprob-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 16:22:51.041525 spaceprob-0.0.1/spaceprob/
--rw-rw-rw-   0        0        0      367 2023-08-06 16:09:16.000000 spaceprob-0.0.1/spaceprob/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 16:22:51.132521 spaceprob-0.0.1/spaceprob.egg-info/
--rw-rw-rw-   0        0        0      686 2023-08-06 16:22:49.000000 spaceprob-0.0.1/spaceprob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-08-06 16:22:50.000000 spaceprob-0.0.1/spaceprob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 16:22:49.000000 spaceprob-0.0.1/spaceprob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 16:22:49.000000 spaceprob-0.0.1/spaceprob.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 16:55:48.641504 spaceprob-0.0.2/
+-rw-rw-rw-   0        0        0      140 2023-08-06 16:54:04.000000 spaceprob-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1065 2023-08-06 16:14:27.000000 spaceprob-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-06 16:12:46.000000 spaceprob-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      745 2023-08-06 16:55:48.636989 spaceprob-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-08-06 16:17:24.000000 spaceprob-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 16:55:48.642552 spaceprob-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-08-06 16:54:26.000000 spaceprob-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:55:48.406581 spaceprob-0.0.2/spaceprob/
+-rw-rw-rw-   0        0        0      314 2023-08-06 16:53:21.000000 spaceprob-0.0.2/spaceprob/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 16:55:48.632233 spaceprob-0.0.2/spaceprob.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-06 16:55:47.000000 spaceprob-0.0.2/spaceprob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-08-06 16:55:47.000000 spaceprob-0.0.2/spaceprob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 16:55:47.000000 spaceprob-0.0.2/spaceprob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 16:55:47.000000 spaceprob-0.0.2/spaceprob.egg-info/top_level.txt
```

### Comparing `spaceprob-0.0.1/LICENSE.txt` & `spaceprob-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spaceprob-0.0.1/PKG-INFO` & `spaceprob-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaceprob
-Version: 0.0.1
+Version: 0.0.2
 Summary: Live stats for Voyager 1 space prob
 Home-page: UNKNOWN
 Author: Sumit Bathla
 Author-email: sumitbathla01@gmail.com
 License: MIT
 Keywords: voyager1
 Platform: UNKNOWN
@@ -20,7 +20,11 @@
 Change Log
 ==========
 
 0.0.1 (06/08/2023)
 ------------------
 - First Release
 
+0.0.2 (06/08/2023)
+------------------
+- Release 0.0.2
+
```

### Comparing `spaceprob-0.0.1/setup.py` & `spaceprob-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='spaceprob',
-  version='0.0.1',
+  version='0.0.2',
   description='Live stats for Voyager 1 space prob',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Sumit Bathla',
   author_email='sumitbathla01@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `spaceprob-0.0.1/spaceprob.egg-info/PKG-INFO` & `spaceprob-0.0.2/spaceprob.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaceprob
-Version: 0.0.1
+Version: 0.0.2
 Summary: Live stats for Voyager 1 space prob
 Home-page: UNKNOWN
 Author: Sumit Bathla
 Author-email: sumitbathla01@gmail.com
 License: MIT
 Keywords: voyager1
 Platform: UNKNOWN
@@ -20,7 +20,11 @@
 Change Log
 ==========
 
 0.0.1 (06/08/2023)
 ------------------
 - First Release
 
+0.0.2 (06/08/2023)
+------------------
+- Release 0.0.2
+
```

