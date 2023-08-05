# Comparing `tmp/hyprland_autocompile-0.0.1a0.tar.gz` & `tmp/hyprland_autocompile-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprland_autocompile-0.0.1a0.tar", max compression
+gzip compressed data, was "hyprland_autocompile-0.0.2a0.tar", max compression
```

## Comparing `hyprland_autocompile-0.0.1a0.tar` & `hyprland_autocompile-0.0.2a0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      219 2023-08-04 14:28:24.587390 hyprland_autocompile-0.0.1a0/README.md
--rw-r--r--   0        0        0        0 2023-08-04 14:28:24.591390 hyprland_autocompile-0.0.1a0/hyprland_autocompile/__init__.py
--rw-r--r--   0        0        0     5310 2023-08-04 14:28:37.379552 hyprland_autocompile-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 hyprland_autocompile-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      219 2023-08-05 22:59:05.304926 hyprland_autocompile-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 22:59:05.304926 hyprland_autocompile-0.0.2a0/hyprland_autocompile/__init__.py
+-rw-r--r--   0        0        0     5310 2023-08-05 22:59:14.297810 hyprland_autocompile-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1269 1970-01-01 00:00:00.000000 hyprland_autocompile-0.0.2a0/PKG-INFO
```

### Comparing `hyprland_autocompile-0.0.1a0/pyproject.toml` & `hyprland_autocompile-0.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # region: Poetry
 
 [tool.poetry]
 name = "hyprland-autocompile"
-version = "0.0.1a0" # Managed by poetry-dynamic-versioning
+version = "0.0.2a0" # Managed by poetry-dynamic-versioning
 description = "Script for easy compilation of hyprland"
 authors = ["ItsDrike <itsdrike@protonmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ItsDrike/hyprland-autocompile"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
```

### Comparing `hyprland_autocompile-0.0.1a0/PKG-INFO` & `hyprland_autocompile-0.0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprland-autocompile
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Script for easy compilation of hyprland
 Home-page: https://github.com/ItsDrike/hyprland-autocompile
 License: GPL-3.0-or-later
 Author: ItsDrike
 Author-email: itsdrike@protonmail.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
```

