# Comparing `tmp/BeyotekTools-0.0.7.tar.gz` & `tmp/BeyotekTools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyotekTools-0.0.7.tar", last modified: Sun Aug  6 00:39:45 2023, max compression
+gzip compressed data, was "BeyotekTools-0.0.8.tar", last modified: Sun Aug  6 00:53:22 2023, max compression
```

## Comparing `BeyotekTools-0.0.7.tar` & `BeyotekTools-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 00:39:45.462075 BeyotekTools-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-08-06 00:39:45.461081 BeyotekTools-0.0.7/BeyotekTools.egg-info/
--rw-rw-rw-   0        0        0      485 2023-08-06 00:39:45.000000 BeyotekTools-0.0.7/BeyotekTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-08-06 00:39:45.000000 BeyotekTools-0.0.7/BeyotekTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 00:39:45.000000 BeyotekTools-0.0.7/BeyotekTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-06 00:39:45.000000 BeyotekTools-0.0.7/BeyotekTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 00:39:45.000000 BeyotekTools-0.0.7/BeyotekTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      485 2023-08-06 00:39:45.462075 BeyotekTools-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 00:39:45.462075 BeyotekTools-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-08-06 00:39:32.000000 BeyotekTools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-08-06 00:53:22.207908 BeyotekTools-0.0.8/BeyotekTools.egg-info/
+-rw-rw-rw-   0        0        0      485 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 00:53:22.000000 BeyotekTools-0.0.8/BeyotekTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      485 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 00:53:22.208904 BeyotekTools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-08-06 00:53:08.000000 BeyotekTools-0.0.8/setup.py
```

### Comparing `BeyotekTools-0.0.7/LICENSE` & `BeyotekTools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.7/setup.py` & `BeyotekTools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='BeyotekTools',
-  version='0.0.7',
+  version='0.0.8',
   description='BeyotekTools',
   long_description=open('README.md').read(),
   url='http://beyotek.com',
   author='Beyotek Inc',
   author_email='chuck@beyotek.com',
   license='MIT',
   classifiers=classifiers,
```

