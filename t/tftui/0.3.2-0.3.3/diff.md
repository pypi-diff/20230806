# Comparing `tmp/tftui-0.3.2.tar.gz` & `tmp/tftui-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftui-0.3.2.tar", last modified: Sun Aug  6 07:00:59 2023, max compression
+gzip compressed data, was "tftui-0.3.3.tar", last modified: Sun Aug  6 07:20:19 2023, max compression
```

## Comparing `tftui-0.3.2.tar` & `tftui-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:00:59.619469 tftui-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 07:00:47.000000 tftui-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 07:00:47.000000 tftui-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:00:59.619469 tftui-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-06 07:00:47.000000 tftui-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-06 07:00:47.000000 tftui-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:00:59.619469 tftui-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:00:59.615469 tftui-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:00:59.615469 tftui-0.3.2/src/tftui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:00:47.000000 tftui-0.3.2/src/tftui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-06 07:00:47.000000 tftui-0.3.2/src/tftui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-06 07:00:47.000000 tftui-0.3.2/src/tftui/ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:00:59.619469 tftui-0.3.2/src/tftui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:00:59.000000 tftui-0.3.2/src/tftui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 07:20:09.000000 tftui-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 07:20:09.000000 tftui-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:20:19.936768 tftui-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-06 07:20:09.000000 tftui-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-06 07:20:10.000000 tftui-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:20:19.936768 tftui-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.932768 tftui-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/src/tftui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/src/tftui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/top_level.txt
```

### Comparing `tftui-0.3.2/LICENSE` & `tftui-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tftui-0.3.2/PKG-INFO` & `tftui-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.2
+Version: 0.3.3
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `tftui-0.3.2/README.md` & `tftui-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tftui-0.3.2/pyproject.toml` & `tftui-0.3.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tftui"
-version = "0.3.2"
+version = "0.3.3"
 description = "Terraform Textual User Interface"
 readme = "README.md"
 authors = [{ name = "Ido Avraham" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["terraform", "tui"]
 dependencies = [
-    "textual",
+    "textual>=0.32.0",
     "textual-dev",
 ]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/idoavrah/terraform-tui"
```

### Comparing `tftui-0.3.2/src/tftui/__main__.py` & `tftui-0.3.3/src/tftui/__main__.py`

 * *Files identical despite different names*

### Comparing `tftui-0.3.2/src/tftui/ui.css` & `tftui-0.3.3/src/tftui/ui.css`

 * *Files identical despite different names*

### Comparing `tftui-0.3.2/src/tftui.egg-info/PKG-INFO` & `tftui-0.3.3/src/tftui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.2
+Version: 0.3.3
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

