# Comparing `tmp/JanexPT-0.0.1.tar.gz` & `tmp/JanexPT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.1.tar", last modified: Sat Aug  5 16:14:21 2023, max compression
+gzip compressed data, was "JanexPT-0.0.2.tar", last modified: Sun Aug  6 12:42:31 2023, max compression
```

## Comparing `JanexPT-0.0.1.tar` & `JanexPT-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-05 16:14:21.140747 JanexPT-0.0.1/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-05 16:14:21.140747 JanexPT-0.0.1/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-05 16:14:21.140747 JanexPT-0.0.1/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.1/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.1/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 15:15:17.000000 JanexPT-0.0.1/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-05 15:58:06.000000 JanexPT-0.0.1/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3754 2023-08-05 16:12:24.000000 JanexPT-0.0.1/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       14 2023-08-05 16:00:07.000000 JanexPT-0.0.1/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-05 16:14:21.140747 JanexPT-0.0.1/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-05 16:14:21.000000 JanexPT-0.0.1/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-05 16:14:21.000000 JanexPT-0.0.1/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-05 16:14:21.000000 JanexPT-0.0.1/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 16:14:21.000000 JanexPT-0.0.1/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-05 16:14:21.000000 JanexPT-0.0.1/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-05 14:49:33.000000 JanexPT-0.0.1/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-05 16:14:21.140747 JanexPT-0.0.1/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1500 2023-08-05 16:10:30.000000 JanexPT-0.0.1/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-05 16:14:21.140747 JanexPT-0.0.1/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-05 14:51:31.000000 JanexPT-0.0.1/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.2/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.2/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 15:15:17.000000 JanexPT-0.0.2/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-05 15:58:06.000000 JanexPT-0.0.2/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3754 2023-08-05 16:12:24.000000 JanexPT-0.0.2/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-06 12:38:40.000000 JanexPT-0.0.2/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-05 14:49:33.000000 JanexPT-0.0.2/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:42:31.604591 JanexPT-0.0.2/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1500 2023-08-05 16:10:30.000000 JanexPT-0.0.2/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-06 12:42:31.604591 JanexPT-0.0.2/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-06 12:42:24.000000 JanexPT-0.0.2/setup.py
```

### Comparing `JanexPT-0.0.1/JanexPT/main.py` & `JanexPT-0.0.2/JanexPT/main.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.1/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.2/JanexPT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.1/LICENSE` & `JanexPT-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.1/PKG-INFO` & `JanexPT-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.1/README.md` & `JanexPT-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.1/setup.py` & `JanexPT-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
```

