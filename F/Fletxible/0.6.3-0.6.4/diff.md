# Comparing `tmp/Fletxible-0.6.3.tar.gz` & `tmp/Fletxible-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.6.3.tar", last modified: Sun Aug  6 11:08:41 2023, max compression
+gzip compressed data, was "Fletxible-0.6.4.tar", last modified: Sun Aug  6 12:45:11 2023, max compression
```

## Comparing `Fletxible-0.6.3.tar` & `Fletxible-0.6.4.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.577840 Fletxible-0.6.3/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.568159 Fletxible-0.6.3/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      972 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        4 2023-08-06 11:08:41.000000 Fletxible-0.6.3/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.3/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 11:08:41.577641 Fletxible-0.6.3/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.3/README.md
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 11:08:41.577905 Fletxible-0.6.3/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1238 2023-08-06 11:08:26.000000 Fletxible-0.6.3/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.569010 Fletxible-0.6.3/src/
--rw-r--r--   0 ahmad      (501) staff       (20)       44 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-05 19:28:09.000000 Fletxible-0.6.3/src/config.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.572187 Fletxible-0.6.3/src/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-04 18:54:13.000000 Fletxible-0.6.3/src/core/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-03 12:18:42.000000 Fletxible-0.6.3/src/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-03 12:14:58.000000 Fletxible-0.6.3/src/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-05 09:36:32.000000 Fletxible-0.6.3/src/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-04 18:55:35.000000 Fletxible-0.6.3/src/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-04 18:58:27.000000 Fletxible-0.6.3/src/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-03 11:47:17.000000 Fletxible-0.6.3/src/core/repo_data.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-05 09:39:08.000000 Fletxible-0.6.3/src/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.573178 Fletxible-0.6.3/src/fx_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/fx_material/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/fx_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/fx_material/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-03 20:55:56.000000 Fletxible-0.6.3/src/fx_material/typography.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-05 17:42:37.000000 Fletxible-0.6.3/src/main.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.574006 Fletxible-0.6.3/src/scripts/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:28.000000 Fletxible-0.6.3/src/scripts/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-05 17:57:44.000000 Fletxible-0.6.3/src/scripts/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2226 2023-08-06 11:04:30.000000 Fletxible-0.6.3/src/scripts/create.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.576852 Fletxible-0.6.3/src/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-05 18:02:39.000000 Fletxible-0.6.3/src/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-05-30 15:27:55.000000 Fletxible-0.6.3/src/utilities/fx_cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-02 17:47:19.000000 Fletxible-0.6.3/src/utilities/fx_config.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-05 17:55:14.000000 Fletxible-0.6.3/src/utilities/fx_error.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 10:54:11.000000 Fletxible-0.6.3/src/utilities/fx_main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-03 20:51:41.000000 Fletxible-0.6.3/src/utilities/fx_scratch.py
--rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-05 17:51:41.000000 Fletxible-0.6.3/src/utilities/fx_sub_router.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-05 17:52:40.000000 Fletxible-0.6.3/src/utilities/fx_sub_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-05 17:52:50.000000 Fletxible-0.6.3/src/utilities/fx_template.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 11:08:41.577170 Fletxible-0.6.3/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.3/tests/test_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.538479 Fletxible-0.6.4/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.6.4/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 12:45:11.538274 Fletxible-0.6.4/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.6.4/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.527793 Fletxible-0.6.4/fletxible/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.530302 Fletxible-0.6.4/fletxible/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     1152 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 12:45:11.000000 Fletxible-0.6.4/fletxible/Fletxible.egg-info/top_level.txt
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.533373 Fletxible-0.6.4/fletxible/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/repo_data.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.534397 Fletxible-0.6.4/fletxible/fx_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/fx_material/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/fx_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/fx_material/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/fx_material/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.535195 Fletxible-0.6.4/fletxible/scripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/scripts/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/scripts/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2232 2023-08-06 12:43:05.000000 Fletxible-0.6.4/fletxible/scripts/create.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.537582 Fletxible-0.6.4/fletxible/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_error.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_scratch.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_sub_router.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_sub_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-06 12:27:15.000000 Fletxible-0.6.4/fletxible/utilities/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 12:45:11.538541 Fletxible-0.6.4/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1250 2023-08-06 12:45:05.000000 Fletxible-0.6.4/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 12:45:11.537835 Fletxible-0.6.4/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.6.4/tests/test_template.py
```

### Comparing `Fletxible-0.6.3/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.6.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.3
+Version: 0.6.4
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.3/LICENSE` & `Fletxible-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/PKG-INFO` & `Fletxible-0.6.4/fletxible/Fletxible.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.6.3
+Version: 0.6.4
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.6.3/README.md` & `Fletxible-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/setup.py` & `Fletxible-0.6.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Fletxible",
-    version="0.6.3",
+    version="0.6.4",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",  # noqa: E501
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
-    packages=find_packages("."),
-    # package_dir={"": "src"},
+    packages=find_packages("fletxible"),
+    package_dir={"": "fletxible"},
     install_requires=[
         "click>=8.1.3",
         "flet>=0.9.0",
         "beautifulsoup4>=4.12.2",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `Fletxible-0.6.3/src/core/base.py` & `Fletxible-0.6.4/fletxible/core/base.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/drawer.py` & `Fletxible-0.6.4/fletxible/core/drawer.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/header.py` & `Fletxible-0.6.4/fletxible/core/header.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/left_panel.py` & `Fletxible-0.6.4/fletxible/core/left_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/middle_panel.py` & `Fletxible-0.6.4/fletxible/core/middle_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/mobile_drop_down.py` & `Fletxible-0.6.4/fletxible/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/navigation.py` & `Fletxible-0.6.4/fletxible/core/navigation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/repo_data.py` & `Fletxible-0.6.4/fletxible/core/repo_data.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/core/right_panel.py` & `Fletxible-0.6.4/fletxible/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/fx_material/annotation.py` & `Fletxible-0.6.4/fletxible/fx_material/annotation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/fx_material/block.py` & `Fletxible-0.6.4/fletxible/fx_material/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/main.py` & `Fletxible-0.6.4/fletxible/utilities/fx_main.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/scripts/build.py` & `Fletxible-0.6.4/fletxible/scripts/build.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/scripts/create.py` & `Fletxible-0.6.4/fletxible/scripts/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         else:
             continue
 
 
 def create_src_file_structure():
     source = Path(__file__).parent.parent
     dublicate = Path("./src")
-    fx_file_src = Path("./src/utilities")
+    fx_file_src = Path("./fletxible/utilities")
 
     def create_dir_file_structure(dir_path: str, key: str, file: str):
         source_path = os.path.join(source, key, file)
         dublicate_path = os.path.join(dir_path, file)
 
         with open(source_path, "r") as src_file, open(dublicate_path, "w") as dst_file:
             dst_file.write(src_file.read())
```

### Comparing `Fletxible-0.6.3/src/utilities/fx_cli.py` & `Fletxible-0.6.4/fletxible/utilities/fx_cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/utilities/fx_error.py` & `Fletxible-0.6.4/fletxible/utilities/fx_error.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/utilities/fx_scratch.py` & `Fletxible-0.6.4/fletxible/utilities/fx_scratch.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/utilities/fx_sub_template.py` & `Fletxible-0.6.4/fletxible/utilities/fx_sub_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.6.3/src/utilities/fx_template.py` & `Fletxible-0.6.4/fletxible/utilities/fx_template.py`

 * *Files identical despite different names*

