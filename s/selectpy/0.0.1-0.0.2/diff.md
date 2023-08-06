# Comparing `tmp/selectpy-0.0.1.tar.gz` & `tmp/selectpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selectpy-0.0.1.tar", last modified: Sun Aug  6 09:43:41 2023, max compression
+gzip compressed data, was "selectpy-0.0.2.tar", last modified: Sun Aug  6 09:59:32 2023, max compression
```

## Comparing `selectpy-0.0.1.tar` & `selectpy-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:43:41.174017 selectpy-0.0.1/
--rw-rw-rw-   0        0        0     1197 2023-08-06 09:43:41.172632 selectpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-08-06 09:31:37.000000 selectpy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 09:43:41.096944 selectpy-0.0.1/selectpy/
--rw-rw-rw-   0        0        0     3649 2023-08-06 09:02:01.000000 selectpy-0.0.1/selectpy/Select.py
--rw-rw-rw-   0        0        0       34 2023-08-06 08:05:52.000000 selectpy-0.0.1/selectpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:43:41.165944 selectpy-0.0.1/selectpy.egg-info/
--rw-rw-rw-   0        0        0     1197 2023-08-06 09:43:40.000000 selectpy-0.0.1/selectpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-08-06 09:43:41.000000 selectpy-0.0.1/selectpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:43:40.000000 selectpy-0.0.1/selectpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-06 09:43:40.000000 selectpy-0.0.1/selectpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-06 09:43:40.000000 selectpy-0.0.1/selectpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 09:43:41.175014 selectpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-08-06 08:46:15.000000 selectpy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:59:32.196499 selectpy-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-08-06 09:52:59.000000 selectpy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1220 2023-08-06 09:59:32.193507 selectpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-08-06 09:31:37.000000 selectpy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 09:59:32.150527 selectpy-0.0.2/selectpy/
+-rw-rw-rw-   0        0        0     3649 2023-08-06 09:02:01.000000 selectpy-0.0.2/selectpy/Select.py
+-rw-rw-rw-   0        0        0       34 2023-08-06 08:05:52.000000 selectpy-0.0.2/selectpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:59:32.187407 selectpy-0.0.2/selectpy.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-08-06 09:59:32.000000 selectpy-0.0.2/selectpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-08-06 09:59:32.000000 selectpy-0.0.2/selectpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:59:32.000000 selectpy-0.0.2/selectpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 09:59:32.000000 selectpy-0.0.2/selectpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 09:59:32.000000 selectpy-0.0.2/selectpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:59:32.197497 selectpy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-08-06 09:59:19.000000 selectpy-0.0.2/setup.py
```

### Comparing `selectpy-0.0.1/PKG-INFO` & `selectpy-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: selectpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fully customizable selection menu for python
 Home-page: UNKNOWN
 Author: Soham P
 Author-email: <sohxmp1204@gmail.com>
 License: UNKNOWN
 Keywords: python,select,select menu,terminal menu,python menu,python select menu
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # SelectPy ( selectpy )
 Selectpy is a simple python module to integrate a fully customizable select menu in your python projects.
 
 ## How To Use
```

### Comparing `selectpy-0.0.1/README.md` & `selectpy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `selectpy-0.0.1/selectpy/Select.py` & `selectpy-0.0.2/selectpy/Select.py`

 * *Files identical despite different names*

### Comparing `selectpy-0.0.1/selectpy.egg-info/PKG-INFO` & `selectpy-0.0.2/selectpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: selectpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fully customizable selection menu for python
 Home-page: UNKNOWN
 Author: Soham P
 Author-email: <sohxmp1204@gmail.com>
 License: UNKNOWN
 Keywords: python,select,select menu,terminal menu,python menu,python select menu
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # SelectPy ( selectpy )
 Selectpy is a simple python module to integrate a fully customizable select menu in your python projects.
 
 ## How To Use
```

### Comparing `selectpy-0.0.1/setup.py` & `selectpy-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A fully customizable selection menu for python'
 LONG_DESCRIPTION = 'A simple python module to integrate a fully customizable select menu in your python projects.'
 
 # Setting up
 setup(
     name="selectpy",
     version=VERSION,
     author="Soham P",
     author_email="<sohxmp1204@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['rich', 'yakh', 're'],
+    install_requires=['rich', 'yakh'],
+    setup_requires=['wheel'],
     keywords=['python', 'select', 'select menu', 'terminal menu', 'python menu', 'python select menu']
 )
```

