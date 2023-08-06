# Comparing `tmp/Fletxible-0.6.0.tar.gz` & `tmp/Fletxible-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.6.0.tar", last modified: Sat Aug  5 22:17:19 2023, max compression
+gzip compressed data, was "Fletxible-0.6.1.tar", last modified: Sun Aug  6 10:09:29 2023, max compression
```

## Comparing `Fletxible-0.6.0.tar` & `Fletxible-0.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.614362 Fletxible-0.6.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-05 22:17:19.614142 Fletxible-0.6.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.0/README.md
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-05 22:17:19.614431 Fletxible-0.6.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1279 2023-08-05 22:16:12.000000 Fletxible-0.6.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.603581 Fletxible-0.6.0/src/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.605638 Fletxible-0.6.0/src/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      929 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       60 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-05 22:17:19.000000 Fletxible-0.6.0/src/Fletxible.egg-info/top_level.txt
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.609192 Fletxible-0.6.0/src/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-04 18:54:13.000000 Fletxible-0.6.0/src/core/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-03 12:18:42.000000 Fletxible-0.6.0/src/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-03 12:14:58.000000 Fletxible-0.6.0/src/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-05 09:36:32.000000 Fletxible-0.6.0/src/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-04 18:55:35.000000 Fletxible-0.6.0/src/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-04 18:58:27.000000 Fletxible-0.6.0/src/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-03 11:47:17.000000 Fletxible-0.6.0/src/core/repo_data.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-05 09:39:08.000000 Fletxible-0.6.0/src/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.610303 Fletxible-0.6.0/src/fx_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/fx_material/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-03 20:55:56.000000 Fletxible-0.6.0/src/fx_material/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.611095 Fletxible-0.6.0/src/scripts/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:28.000000 Fletxible-0.6.0/src/scripts/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-05 17:57:44.000000 Fletxible-0.6.0/src/scripts/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2203 2023-08-05 22:04:24.000000 Fletxible-0.6.0/src/scripts/create.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.613415 Fletxible-0.6.0/src/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:39.000000 Fletxible-0.6.0/src/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:27:55.000000 Fletxible-0.6.0/src/utilities/fx_cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-02 17:47:19.000000 Fletxible-0.6.0/src/utilities/fx_config.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-05 17:55:14.000000 Fletxible-0.6.0/src/utilities/fx_error.py
--rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-03 20:51:41.000000 Fletxible-0.6.0/src/utilities/fx_scratch.py
--rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-05 17:51:41.000000 Fletxible-0.6.0/src/utilities/fx_sub_router.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-05 17:52:40.000000 Fletxible-0.6.0/src/utilities/fx_sub_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-05 17:52:50.000000 Fletxible-0.6.0/src/utilities/fx_template.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-05 22:17:19.613704 Fletxible-0.6.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.0/tests/test_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.840973 Fletxible-0.6.1/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 10:09:29.840698 Fletxible-0.6.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.1/README.md
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 10:09:29.841046 Fletxible-0.6.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1269 2023-08-06 10:09:20.000000 Fletxible-0.6.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.829782 Fletxible-0.6.1/src/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.832171 Fletxible-0.6.1/src/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      929 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 10:09:29.000000 Fletxible-0.6.1/src/Fletxible.egg-info/top_level.txt
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.835673 Fletxible-0.6.1/src/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-04 18:54:13.000000 Fletxible-0.6.1/src/core/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-03 12:18:42.000000 Fletxible-0.6.1/src/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-03 12:14:58.000000 Fletxible-0.6.1/src/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-05 09:36:32.000000 Fletxible-0.6.1/src/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-04 18:55:35.000000 Fletxible-0.6.1/src/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-04 18:58:27.000000 Fletxible-0.6.1/src/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-03 11:47:17.000000 Fletxible-0.6.1/src/core/repo_data.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-05 09:39:08.000000 Fletxible-0.6.1/src/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.836771 Fletxible-0.6.1/src/fx_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/fx_material/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/fx_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/fx_material/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-03 20:55:56.000000 Fletxible-0.6.1/src/fx_material/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.837580 Fletxible-0.6.1/src/scripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:28.000000 Fletxible-0.6.1/src/scripts/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-05 17:57:44.000000 Fletxible-0.6.1/src/scripts/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2203 2023-08-05 22:04:24.000000 Fletxible-0.6.1/src/scripts/create.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.839810 Fletxible-0.6.1/src/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:39.000000 Fletxible-0.6.1/src/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:27:55.000000 Fletxible-0.6.1/src/utilities/fx_cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-02 17:47:19.000000 Fletxible-0.6.1/src/utilities/fx_config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-05 17:55:14.000000 Fletxible-0.6.1/src/utilities/fx_error.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-03 20:51:41.000000 Fletxible-0.6.1/src/utilities/fx_scratch.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-05 17:51:41.000000 Fletxible-0.6.1/src/utilities/fx_sub_router.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-05 17:52:40.000000 Fletxible-0.6.1/src/utilities/fx_sub_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-05 17:52:50.000000 Fletxible-0.6.1/src/utilities/fx_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 10:09:29.840254 Fletxible-0.6.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.1/tests/test_template.py
```

### Comparing `Fletxible-0.6.0/LICENSE` & `Fletxible-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/PKG-INFO` & `Fletxible-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.0
+Version: 0.6.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.0/README.md` & `Fletxible-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/setup.py` & `Fletxible-0.6.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Fletxible",
-    version="0.6.0",
+    version="0.6.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",  # noqa: E501
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=find_packages("src"),
@@ -20,12 +20,12 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "fletxible-init=fletxible.command:create",
+            "fx-init=scripts.create:create",
         ],
     },
     keywords=["python web template", "web application", "theme"],
 )
```

### Comparing `Fletxible-0.6.0/src/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.6.1/src/Fletxible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.0
+Version: 0.6.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.0/src/Fletxible.egg-info/SOURCES.txt` & `Fletxible-0.6.1/src/Fletxible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/base.py` & `Fletxible-0.6.1/src/core/base.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/drawer.py` & `Fletxible-0.6.1/src/core/drawer.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/header.py` & `Fletxible-0.6.1/src/core/header.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/left_panel.py` & `Fletxible-0.6.1/src/core/left_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/middle_panel.py` & `Fletxible-0.6.1/src/core/middle_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/mobile_drop_down.py` & `Fletxible-0.6.1/src/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/navigation.py` & `Fletxible-0.6.1/src/core/navigation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/repo_data.py` & `Fletxible-0.6.1/src/core/repo_data.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/core/right_panel.py` & `Fletxible-0.6.1/src/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/fx_material/annotation.py` & `Fletxible-0.6.1/src/fx_material/annotation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/fx_material/block.py` & `Fletxible-0.6.1/src/fx_material/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/scripts/build.py` & `Fletxible-0.6.1/src/scripts/build.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/scripts/create.py` & `Fletxible-0.6.1/src/scripts/create.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/utilities/fx_cli.py` & `Fletxible-0.6.1/src/utilities/fx_cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/utilities/fx_error.py` & `Fletxible-0.6.1/src/utilities/fx_error.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/utilities/fx_scratch.py` & `Fletxible-0.6.1/src/utilities/fx_scratch.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/utilities/fx_sub_template.py` & `Fletxible-0.6.1/src/utilities/fx_sub_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.0/src/utilities/fx_template.py` & `Fletxible-0.6.1/src/utilities/fx_template.py`

 * *Files identical despite different names*

