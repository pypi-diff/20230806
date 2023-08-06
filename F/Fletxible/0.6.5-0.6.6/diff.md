# Comparing `tmp/Fletxible-0.6.5.tar.gz` & `tmp/Fletxible-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.6.5.tar", last modified: Sun Aug  6 12:55:37 2023, max compression
+gzip compressed data, was "Fletxible-0.6.6.tar", last modified: Sun Aug  6 13:06:48 2023, max compression
```

## Comparing `Fletxible-0.6.5.tar` & `Fletxible-0.6.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.407677 Fletxible-0.6.5/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.5/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 12:55:37.407471 Fletxible-0.6.5/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.5/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.399566 Fletxible-0.6.5/fletxible/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.401477 Fletxible-0.6.5/fletxible/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     1152 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 12:55:37.000000 Fletxible-0.6.5/fletxible/Fletxible.egg-info/top_level.txt
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.403633 Fletxible-0.6.5/fletxible/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/repo_data.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.404765 Fletxible-0.6.5/fletxible/fx_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/fx_material/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/fx_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/fx_material/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/fx_material/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.405322 Fletxible-0.6.5/fletxible/scripts/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/scripts/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/scripts/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2226 2023-08-06 12:53:36.000000 Fletxible-0.6.5/fletxible/scripts/create.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.406970 Fletxible-0.6.5/fletxible/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_config.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_error.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_scratch.py
--rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_sub_router.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_sub_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-06 12:27:15.000000 Fletxible-0.6.5/fletxible/utilities/fx_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 12:55:37.407739 Fletxible-0.6.5/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1250 2023-08-06 12:55:12.000000 Fletxible-0.6.5/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:55:37.407163 Fletxible-0.6.5/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.5/tests/test_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.575728 Fletxible-0.6.6/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.6/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 13:06:48.575526 Fletxible-0.6.6/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.6/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.565345 Fletxible-0.6.6/fletxible/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.567728 Fletxible-0.6.6/fletxible/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     1152 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 13:06:48.000000 Fletxible-0.6.6/fletxible/Fletxible.egg-info/top_level.txt
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.570845 Fletxible-0.6.6/fletxible/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/repo_data.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.571857 Fletxible-0.6.6/fletxible/fx_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/fx_material/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/fx_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/fx_material/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/fx_material/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.572553 Fletxible-0.6.6/fletxible/scripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/scripts/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/scripts/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2226 2023-08-06 12:53:36.000000 Fletxible-0.6.6/fletxible/scripts/create.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.574768 Fletxible-0.6.6/fletxible/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_error.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_scratch.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_sub_router.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_sub_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-06 12:27:15.000000 Fletxible-0.6.6/fletxible/utilities/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 13:06:48.575792 Fletxible-0.6.6/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1250 2023-08-06 13:06:44.000000 Fletxible-0.6.6/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 13:06:48.575074 Fletxible-0.6.6/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.6/tests/test_template.py
```

### Comparing `Fletxible-0.6.5/LICENSE` & `Fletxible-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/PKG-INFO` & `Fletxible-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.5
+Version: 0.6.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.5/README.md` & `Fletxible-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.6.6/fletxible/Fletxible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.5
+Version: 0.6.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.5/fletxible/Fletxible.egg-info/SOURCES.txt` & `Fletxible-0.6.6/fletxible/Fletxible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/base.py` & `Fletxible-0.6.6/fletxible/core/base.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/drawer.py` & `Fletxible-0.6.6/fletxible/core/drawer.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/header.py` & `Fletxible-0.6.6/fletxible/core/header.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/left_panel.py` & `Fletxible-0.6.6/fletxible/core/left_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/middle_panel.py` & `Fletxible-0.6.6/fletxible/core/middle_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/mobile_drop_down.py` & `Fletxible-0.6.6/fletxible/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/navigation.py` & `Fletxible-0.6.6/fletxible/core/navigation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/repo_data.py` & `Fletxible-0.6.6/fletxible/core/repo_data.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/core/right_panel.py` & `Fletxible-0.6.6/fletxible/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/fx_material/annotation.py` & `Fletxible-0.6.6/fletxible/fx_material/annotation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/fx_material/block.py` & `Fletxible-0.6.6/fletxible/fx_material/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/scripts/build.py` & `Fletxible-0.6.6/fletxible/scripts/build.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/scripts/create.py` & `Fletxible-0.6.6/fletxible/scripts/create.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_cli.py` & `Fletxible-0.6.6/fletxible/utilities/fx_cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_error.py` & `Fletxible-0.6.6/fletxible/utilities/fx_error.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_main.py` & `Fletxible-0.6.6/fletxible/utilities/fx_main.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_scratch.py` & `Fletxible-0.6.6/fletxible/utilities/fx_scratch.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_sub_template.py` & `Fletxible-0.6.6/fletxible/utilities/fx_sub_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/fletxible/utilities/fx_template.py` & `Fletxible-0.6.6/fletxible/utilities/fx_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.5/setup.py` & `Fletxible-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Fletxible",
-    version="0.6.5",
+    version="0.6.6",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",  # noqa: E501
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=find_packages("fletxible"),
```

