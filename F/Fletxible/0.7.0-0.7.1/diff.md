# Comparing `tmp/Fletxible-0.7.0.tar.gz` & `tmp/Fletxible-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.7.0.tar", last modified: Sun Aug  6 14:48:14 2023, max compression
+gzip compressed data, was "Fletxible-0.7.1.tar", last modified: Sun Aug  6 15:50:26 2023, max compression
```

## Comparing `Fletxible-0.7.0.tar` & `Fletxible-0.7.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.797521 Fletxible-0.7.0/
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.7.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 14:48:14.797314 Fletxible-0.7.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.7.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.787033 Fletxible-0.7.0/fletxible/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.789636 Fletxible-0.7.0/fletxible/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     1152 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 14:48:14.000000 Fletxible-0.7.0/fletxible/Fletxible.egg-info/top_level.txt
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.792741 Fletxible-0.7.0/fletxible/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/repo_data.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.793710 Fletxible-0.7.0/fletxible/fx_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/fx_material/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/fx_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/fx_material/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/fx_material/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.794459 Fletxible-0.7.0/fletxible/scripts/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/scripts/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4849 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/scripts/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2654 2023-08-06 14:47:22.000000 Fletxible-0.7.0/fletxible/scripts/create.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.796508 Fletxible-0.7.0/fletxible/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_config.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_error.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_main.py
--rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_scratch.py
--rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_sub_router.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_sub_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-06 12:27:15.000000 Fletxible-0.7.0/fletxible/utilities/fx_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 14:48:14.797588 Fletxible-0.7.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1250 2023-08-06 14:48:00.000000 Fletxible-0.7.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 14:48:14.796755 Fletxible-0.7.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.7.0/tests/test_template.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.561458 Fletxible-0.7.1/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-08-02 17:47:19.000000 Fletxible-0.7.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 15:50:26.561308 Fletxible-0.7.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4768 2023-08-02 17:47:19.000000 Fletxible-0.7.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.554280 Fletxible-0.7.1/fletxible/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.556207 Fletxible-0.7.1/fletxible/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      824 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     1152 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       35 2023-08-06 15:50:26.000000 Fletxible-0.7.1/fletxible/Fletxible.egg-info/top_level.txt
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.558228 Fletxible-0.7.1/fletxible/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     5332 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2133 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4647 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1176 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1257 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4678 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      638 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3073 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/repo_data.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1801 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.558814 Fletxible-0.7.1/fletxible/fx_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      193 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/fx_material/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1449 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/fx_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/fx_material/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/fx_material/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.559309 Fletxible-0.7.1/fletxible/scripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/scripts/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4964 2023-08-06 15:48:56.000000 Fletxible-0.7.1/fletxible/scripts/build.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2654 2023-08-06 14:47:22.000000 Fletxible-0.7.1/fletxible/scripts/create.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.560772 Fletxible-0.7.1/fletxible/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2116 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      314 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1027 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_error.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3006 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      567 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_scratch.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      403 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_sub_router.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1042 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_sub_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      903 2023-08-06 12:27:15.000000 Fletxible-0.7.1/fletxible/utilities/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-08-06 15:50:26.561505 Fletxible-0.7.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1250 2023-08-06 15:50:10.000000 Fletxible-0.7.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-08-06 15:50:26.560933 Fletxible-0.7.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-08-02 17:52:36.000000 Fletxible-0.7.1/tests/test_template.py
```

### Comparing `Fletxible-0.7.0/LICENSE` & `Fletxible-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/PKG-INFO` & `Fletxible-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.7.0
+Version: 0.7.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.7.0/README.md` & `Fletxible-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.7.1/fletxible/Fletxible.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.7.0
+Version: 0.7.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,theme
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.7.0/fletxible/Fletxible.egg-info/SOURCES.txt` & `Fletxible-0.7.1/fletxible/Fletxible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/base.py` & `Fletxible-0.7.1/fletxible/core/base.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/drawer.py` & `Fletxible-0.7.1/fletxible/core/drawer.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/header.py` & `Fletxible-0.7.1/fletxible/core/header.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/left_panel.py` & `Fletxible-0.7.1/fletxible/core/left_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/middle_panel.py` & `Fletxible-0.7.1/fletxible/core/middle_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/mobile_drop_down.py` & `Fletxible-0.7.1/fletxible/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/navigation.py` & `Fletxible-0.7.1/fletxible/core/navigation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/repo_data.py` & `Fletxible-0.7.1/fletxible/core/repo_data.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/core/right_panel.py` & `Fletxible-0.7.1/fletxible/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/fx_material/annotation.py` & `Fletxible-0.7.1/fletxible/fx_material/annotation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/fx_material/block.py` & `Fletxible-0.7.1/fletxible/fx_material/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/scripts/build.py` & `Fletxible-0.7.1/fletxible/scripts/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,30 +102,32 @@
                 if file_length >= 3:
                     file.write(sub_view)
                 else:
                     file.write(view)
 
 
 def set_sub_directory_router_file():
-    with open("utilities/fx_sub_router.py", "r") as file:
-        router = file.read()
-
     with open("utilities/fx_error.py", "r") as file:
         error = file.read()
 
-    router_path = os.path.join("pages" + "/router.py")
-    if not os.path.exists(router_path):
-        with open(router_path, "w") as file:
-            file.write(router)
-
     error_path = os.path.join("pages" + "/_error.py")
     if not os.path.exists(error_path):
         with open(error_path, "w") as file:
             file.write(error)
 
+    with open("utilities/fx_sub_router.py", "r") as file:
+        router = file.read()
+
+    for root, dirs, __ in os.walk("pages"):
+        for dir in dirs:
+            router_path = os.path.join(root + "/" + dir + "/" + "router.py")
+            if not os.path.exists(router_path):
+                with open(router_path, "w") as file:
+                    file.write(router)
+
 
 # NOT USED #
 def create_navigation_links_from_keys():
     nav_list: list = []
 
     __, list_of_pages = get_list_of_pages_from_directory()
```

### Comparing `Fletxible-0.7.0/fletxible/scripts/create.py` & `Fletxible-0.7.1/fletxible/scripts/create.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_cli.py` & `Fletxible-0.7.1/fletxible/utilities/fx_cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_error.py` & `Fletxible-0.7.1/fletxible/utilities/fx_error.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_main.py` & `Fletxible-0.7.1/fletxible/utilities/fx_main.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_scratch.py` & `Fletxible-0.7.1/fletxible/utilities/fx_scratch.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_sub_template.py` & `Fletxible-0.7.1/fletxible/utilities/fx_sub_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/fletxible/utilities/fx_template.py` & `Fletxible-0.7.1/fletxible/utilities/fx_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.7.0/setup.py` & `Fletxible-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Fletxible",
-    version="0.7.0",
+    version="0.7.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",  # noqa: E501
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=find_packages("fletxible"),
```

