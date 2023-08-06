# Comparing `tmp/wwwgetpy-0.1.0.tar.gz` & `tmp/wwwgetpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwwgetpy-0.1.0.tar", last modified: Sun Aug  6 10:16:16 2023, max compression
+gzip compressed data, was "wwwgetpy-0.1.1.tar", last modified: Sun Aug  6 10:19:55 2023, max compression
```

## Comparing `wwwgetpy-0.1.0.tar` & `wwwgetpy-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 10:16:16.180717 wwwgetpy-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-08-05 18:17:59.000000 wwwgetpy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      878 2023-08-06 10:16:16.180717 wwwgetpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-08-05 18:17:59.000000 wwwgetpy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 10:16:16.163197 wwwgetpy-0.1.0/app/
-drwxrwxrwx   0        0        0        0 2023-08-06 10:16:16.171152 wwwgetpy-0.1.0/app/wwwgetpy/
--rw-rw-rw-   0        0        0       93 2023-08-06 09:20:30.000000 wwwgetpy-0.1.0/app/wwwgetpy/__init__.py
--rw-rw-rw-   0        0        0     5651 2023-08-06 09:30:37.000000 wwwgetpy-0.1.0/app/wwwgetpy/core.py
-drwxrwxrwx   0        0        0        0 2023-08-06 10:16:16.178717 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/
--rw-rw-rw-   0        0        0      878 2023-08-06 10:16:16.000000 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-08-06 10:16:16.000000 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 10:16:16.000000 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-06 10:16:16.000000 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-06 10:16:16.000000 wwwgetpy-0.1.0/app/wwwgetpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 10:16:16.180717 wwwgetpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      948 2023-08-06 10:16:04.000000 wwwgetpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:19:55.201169 wwwgetpy-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-08-05 18:17:59.000000 wwwgetpy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      878 2023-08-06 10:19:55.201169 wwwgetpy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-08-05 18:17:59.000000 wwwgetpy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 10:19:55.183137 wwwgetpy-0.1.1/app/
+drwxrwxrwx   0        0        0        0 2023-08-06 10:19:55.191165 wwwgetpy-0.1.1/app/wwwgetpy/
+-rw-rw-rw-   0        0        0       93 2023-08-06 09:20:30.000000 wwwgetpy-0.1.1/app/wwwgetpy/__init__.py
+-rw-rw-rw-   0        0        0     5651 2023-08-06 09:30:37.000000 wwwgetpy-0.1.1/app/wwwgetpy/core.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:19:55.199165 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/
+-rw-rw-rw-   0        0        0      878 2023-08-06 10:19:55.000000 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-08-06 10:19:55.000000 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 10:19:55.000000 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-06 10:19:55.000000 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 10:19:55.000000 wwwgetpy-0.1.1/app/wwwgetpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 10:19:55.201169 wwwgetpy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      948 2023-08-06 10:19:39.000000 wwwgetpy-0.1.1/setup.py
```

### Comparing `wwwgetpy-0.1.0/LICENSE` & `wwwgetpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwwgetpy-0.1.0/PKG-INFO` & `wwwgetpy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwwgetpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: It is a Windows WSL wget python lib to use it for HTML folder directories in paralel
 Home-page: https://github.com/sacamar2/wwwget_py
 Author: sacamar2
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `wwwgetpy-0.1.0/app/wwwgetpy/core.py` & `wwwgetpy-0.1.1/app/wwwgetpy/core.py`

 * *Files identical despite different names*

### Comparing `wwwgetpy-0.1.0/app/wwwgetpy.egg-info/PKG-INFO` & `wwwgetpy-0.1.1/app/wwwgetpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwwgetpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: It is a Windows WSL wget python lib to use it for HTML folder directories in paralel
 Home-page: https://github.com/sacamar2/wwwget_py
 Author: sacamar2
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `wwwgetpy-0.1.0/setup.py` & `wwwgetpy-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     sys.exit(1)
 
 with open("app/wwwgetpy/Readme.md",'r') as f:
     long_description=f.read()
 
 setup(
 	name="wwwgetpy",
-    version="0.1.0",
+    version="0.1.1",
     description="It is a Windows WSL wget python lib to use it for HTML folder directories in paralel",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"":"app"},
     packages=find_packages(where="app"),
 	author="sacamar2",
     url="https://github.com/sacamar2/wwwget_py",
```

