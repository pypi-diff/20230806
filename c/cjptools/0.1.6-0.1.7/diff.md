# Comparing `tmp/cjptools-0.1.6.tar.gz` & `tmp/cjptools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjptools-0.1.6.tar", last modified: Thu Aug  3 07:48:00 2023, max compression
+gzip compressed data, was "cjptools-0.1.7.tar", last modified: Sun Aug  6 05:59:03 2023, max compression
```

## Comparing `cjptools-0.1.6.tar` & `cjptools-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.256385 cjptools-0.1.6/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      276 2023-08-03 07:48:00.255387 cjptools-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.221532 cjptools-0.1.6/cjptools/
--rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.6/cjptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.232505 cjptools-0.1.6/cjptools/dptools/
--rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.6/cjptools/dptools/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.6/cjptools/dptools/rdpAccount.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.240480 cjptools-0.1.6/cjptools/printModules/
--rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/__init__.py
--rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/absPrinter.py
--rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/printerCompose.py
--rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.6/cjptools/printModules/printers.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.253393 cjptools-0.1.6/cjptools/utils/
--rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.6/cjptools/utils/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.6/cjptools/utils/check.py
--rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.6/cjptools/utils/gpu_mem_track.py
--rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.6/cjptools/utils/modelsize_estimate.py
--rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.6/cjptools/utils/path.py
--rw-rw-rw-   0        0        0      336 2023-08-03 07:47:46.000000 cjptools-0.1.6/cjptools/utils/reflect.py
--rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.6/cjptools/utils/rnd.py
--rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.6/cjptools/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.227515 cjptools-0.1.6/cjptools.egg-info/
--rw-rw-rw-   0        0        0      276 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:48:00.256385 cjptools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-08-03 07:47:55.000000 cjptools-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.142440 cjptools-0.1.7/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-08-06 05:59:03.141443 cjptools-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.055583 cjptools-0.1.7/cjptools/
+-rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.7/cjptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.064251 cjptools-0.1.7/cjptools/dptools/
+-rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.7/cjptools/dptools/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.7/cjptools/dptools/rdpAccount.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.082815 cjptools-0.1.7/cjptools/interfaces/
+-rw-rw-rw-   0        0        0       19 2023-08-06 05:58:36.000000 cjptools-0.1.7/cjptools/interfaces/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-08-06 05:58:13.000000 cjptools-0.1.7/cjptools/interfaces/data.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.091790 cjptools-0.1.7/cjptools/printModules/
+-rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.7/cjptools/printModules/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.7/cjptools/printModules/absPrinter.py
+-rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.7/cjptools/printModules/printerCompose.py
+-rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.7/cjptools/printModules/printers.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.140470 cjptools-0.1.7/cjptools/utils/
+-rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.7/cjptools/utils/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.7/cjptools/utils/check.py
+-rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.7/cjptools/utils/gpu_mem_track.py
+-rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.7/cjptools/utils/modelsize_estimate.py
+-rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.7/cjptools/utils/path.py
+-rw-rw-rw-   0        0        0      336 2023-08-03 07:47:46.000000 cjptools-0.1.7/cjptools/utils/reflect.py
+-rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.7/cjptools/utils/rnd.py
+-rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.7/cjptools/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:59:03.061258 cjptools-0.1.7/cjptools.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-08-06 05:59:02.000000 cjptools-0.1.7/cjptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-08-06 05:59:02.000000 cjptools-0.1.7/cjptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 05:59:02.000000 cjptools-0.1.7/cjptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 05:59:02.000000 cjptools-0.1.7/cjptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 05:59:03.142440 cjptools-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-08-06 05:58:57.000000 cjptools-0.1.7/setup.py
```

### Comparing `cjptools-0.1.6/LICENSE` & `cjptools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/dptools/rdpAccount.py` & `cjptools-0.1.7/cjptools/dptools/rdpAccount.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/printModules/printers.py` & `cjptools-0.1.7/cjptools/printModules/printers.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/utils/gpu_mem_track.py` & `cjptools-0.1.7/cjptools/utils/gpu_mem_track.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/utils/modelsize_estimate.py` & `cjptools-0.1.7/cjptools/utils/modelsize_estimate.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/utils/path.py` & `cjptools-0.1.7/cjptools/utils/path.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools/utils/rnd.py` & `cjptools-0.1.7/cjptools/utils/rnd.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.6/cjptools.egg-info/SOURCES.txt` & `cjptools-0.1.7/cjptools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 cjptools/__init__.py
 cjptools.egg-info/PKG-INFO
 cjptools.egg-info/SOURCES.txt
 cjptools.egg-info/dependency_links.txt
 cjptools.egg-info/top_level.txt
 cjptools/dptools/__init__.py
 cjptools/dptools/rdpAccount.py
+cjptools/interfaces/__init__.py
+cjptools/interfaces/data.py
 cjptools/printModules/__init__.py
 cjptools/printModules/absPrinter.py
 cjptools/printModules/printerCompose.py
 cjptools/printModules/printers.py
 cjptools/utils/__init__.py
 cjptools/utils/check.py
 cjptools/utils/gpu_mem_track.py
```

### Comparing `cjptools-0.1.6/setup.py` & `cjptools-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="cjptools",
-    version="0.1.6",
+    version="0.1.7",
     keywords=("database", "localServer"),
     description="My Personal Toolkit",
     long_description="My Personal Toolkit",
     license="MIT Licence",
     author="Cai Jianping",
     author_email="jpingcai@163.com",
```

