# Comparing `tmp/apifoncier-0.0.8.tar.gz` & `tmp/apifoncier-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apifoncier-0.0.8.tar", last modified: Mon Jul 10 15:52:29 2023, max compression
+gzip compressed data, was "apifoncier-0.0.9.tar", last modified: Tue Jul 11 06:26:30 2023, max compression
```

## Comparing `apifoncier-0.0.8.tar` & `apifoncier-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.637824 apifoncier-0.0.8/
--rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     9938 2023-07-10 15:52:29.637824 apifoncier-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.625084 apifoncier-0.0.8/apifoncier/
-drwxrwxrwx   0        0        0        0 2023-07-10 15:52:29.635827 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/
--rw-rw-rw-   0        0        0     9938 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2023-07-10 15:52:29.000000 apifoncier-0.0.8/apifoncier/apifoncier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2987 2023-07-10 15:48:13.000000 apifoncier-0.0.8/apifoncier/cartofriches.py
--rw-rw-rw-   0        0        0     5083 2023-07-10 15:45:16.000000 apifoncier-0.0.8/apifoncier/ind_conso_espace.py
--rw-rw-rw-   0        0        0     5349 2023-07-10 15:52:23.000000 apifoncier-0.0.8/apifoncier/ind_dv3f.py
--rw-rw-rw-   0        0        0     9809 2023-07-10 15:15:11.000000 apifoncier-0.0.8/apifoncier/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-10 15:52:29.638824 apifoncier-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-07-10 15:39:36.000000 apifoncier-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:30.100667 apifoncier-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2023-07-10 11:54:34.000000 apifoncier-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9938 2023-07-11 06:26:30.099688 apifoncier-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9344 2023-07-07 12:12:49.000000 apifoncier-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:30.086657 apifoncier-0.0.9/apifoncier/
+drwxrwxrwx   0        0        0        0 2023-07-11 06:26:30.095660 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/
+-rw-rw-rw-   0        0        0     9938 2023-07-11 06:26:30.000000 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-07-11 06:26:30.000000 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 06:26:30.000000 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-11 06:26:30.000000 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2023-07-11 06:26:30.000000 apifoncier-0.0.9/apifoncier/apifoncier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2987 2023-07-10 15:48:13.000000 apifoncier-0.0.9/apifoncier/cartofriches.py
+-rw-rw-rw-   0        0        0     5083 2023-07-10 15:45:16.000000 apifoncier-0.0.9/apifoncier/ind_conso_espace.py
+-rw-rw-rw-   0        0        0     5349 2023-07-10 15:52:23.000000 apifoncier-0.0.9/apifoncier/ind_dv3f.py
+-rw-rw-rw-   0        0        0     9809 2023-07-10 15:15:11.000000 apifoncier-0.0.9/apifoncier/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 06:26:30.100667 apifoncier-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1163 2023-07-11 06:26:04.000000 apifoncier-0.0.9/setup.py
```

### Comparing `apifoncier-0.0.8/LICENSE` & `apifoncier-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/PKG-INFO` & `apifoncier-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apifoncier-0.0.8/README.md` & `apifoncier-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/apifoncier/apifoncier.egg-info/PKG-INFO` & `apifoncier-0.0.9/apifoncier/apifoncier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Home-page: https://github.com/rcadot/py.apifoncier
 Author: Romain Cadot
 Author-email: romain.cadot@cerema.fr
 License: MIT
 Keywords: api,foncier,cerema,dv3f,friches,artificialisation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `apifoncier-0.0.8/apifoncier/cartofriches.py` & `apifoncier-0.0.9/apifoncier/cartofriches.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/apifoncier/ind_conso_espace.py` & `apifoncier-0.0.9/apifoncier/ind_conso_espace.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/apifoncier/ind_dv3f.py` & `apifoncier-0.0.9/apifoncier/ind_dv3f.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/apifoncier/utils.py` & `apifoncier-0.0.9/apifoncier/utils.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.8/setup.py` & `apifoncier-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md","r",encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = "apifoncier",
-    version = "0.0.8",
+    version = "0.0.9",
     description = "Mobiliser les données foncières de l'api du Cerema directement avec python",
     package_dir={"":"apifoncier"},
     packages=find_packages(where="apifoncier"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rcadot/py.apifoncier",
     author="Romain Cadot",
```

