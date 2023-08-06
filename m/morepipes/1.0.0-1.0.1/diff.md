# Comparing `tmp/morepipes-1.0.0.tar.gz` & `tmp/morepipes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morepipes-1.0.0.tar", last modified: Sun Aug  6 07:43:26 2023, max compression
+gzip compressed data, was "morepipes-1.0.1.tar", last modified: Sun Aug  6 07:59:02 2023, max compression
```

## Comparing `morepipes-1.0.0.tar` & `morepipes-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 07:43:26.088980 morepipes-1.0.0/
--rw-rw-rw-   0        0        0     1086 2023-08-06 07:37:43.000000 morepipes-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1991 2023-08-06 07:43:26.087975 morepipes-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-08-06 07:36:39.000000 morepipes-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 07:43:26.075993 morepipes-1.0.0/morepipes.egg-info/
--rw-rw-rw-   0        0        0     1991 2023-08-06 07:43:25.000000 morepipes-1.0.0/morepipes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-08-06 07:43:25.000000 morepipes-1.0.0/morepipes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 07:43:25.000000 morepipes-1.0.0/morepipes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 07:43:25.000000 morepipes-1.0.0/morepipes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 07:43:25.000000 morepipes-1.0.0/morepipes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3430 2023-08-06 07:42:46.000000 morepipes-1.0.0/morepipes.py
--rw-rw-rw-   0        0        0      708 2023-08-06 07:41:23.000000 morepipes-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 07:43:26.089980 morepipes-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 07:59:02.896406 morepipes-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-08-06 07:37:43.000000 morepipes-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2617 2023-08-06 07:59:02.892789 morepipes-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-08-06 07:51:58.000000 morepipes-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 07:59:02.889785 morepipes-1.0.1/morepipes.egg-info/
+-rw-rw-rw-   0        0        0     2617 2023-08-06 07:59:02.000000 morepipes-1.0.1/morepipes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-08-06 07:59:02.000000 morepipes-1.0.1/morepipes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 07:59:02.000000 morepipes-1.0.1/morepipes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 07:59:02.000000 morepipes-1.0.1/morepipes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 07:59:02.000000 morepipes-1.0.1/morepipes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3430 2023-08-06 07:42:46.000000 morepipes-1.0.1/morepipes.py
+-rw-rw-rw-   0        0        0      708 2023-08-06 07:58:38.000000 morepipes-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 07:59:02.897323 morepipes-1.0.1/setup.cfg
```

### Comparing `morepipes-1.0.0/LICENSE` & `morepipes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morepipes-1.0.0/PKG-INFO` & `morepipes-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morepipes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extended pipes for functional programming
 License: MIT License
         
         Copyright (c) 2023 tovicheung
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,9 +33,40 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # morepipes
 Based on the [pipe](https://github.com/JulienPalard/Pipe) library, adding more utilities and pipes to it
 
+Some pipes are inspired by other programming languages (eg Rust)
+
 ## Installation
--
+`pip install morepipes`
+
+## Examples
+Consume iterable
+```py
+range(9) | where(lambda x: x % 2) | collect(list)
+# List of odd numbers
+```
+Side effects
+```py
+range(9) | ... | inspect | ...
+# Prints out each object received on evaluation
+```
+Or, more generally
+```py
+range(9) | ... | foreach(print) | ...
+```
+## New: Partial Pipes
+Creating a partial pipe
+```py
+reverse_sort = P | reverse | sort
+# P is a special object placeholder
+```
+Using a partial pipe
+```py
+[1, 3, 4, 2] | reverse_sort
+# Just like any other pipe
+```
+---
+Have fun!
```

### Comparing `morepipes-1.0.0/morepipes.egg-info/PKG-INFO` & `morepipes-1.0.1/morepipes.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morepipes
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extended pipes for functional programming
 License: MIT License
         
         Copyright (c) 2023 tovicheung
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,9 +33,40 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # morepipes
 Based on the [pipe](https://github.com/JulienPalard/Pipe) library, adding more utilities and pipes to it
 
+Some pipes are inspired by other programming languages (eg Rust)
+
 ## Installation
--
+`pip install morepipes`
+
+## Examples
+Consume iterable
+```py
+range(9) | where(lambda x: x % 2) | collect(list)
+# List of odd numbers
+```
+Side effects
+```py
+range(9) | ... | inspect | ...
+# Prints out each object received on evaluation
+```
+Or, more generally
+```py
+range(9) | ... | foreach(print) | ...
+```
+## New: Partial Pipes
+Creating a partial pipe
+```py
+reverse_sort = P | reverse | sort
+# P is a special object placeholder
+```
+Using a partial pipe
+```py
+[1, 3, 4, 2] | reverse_sort
+# Just like any other pipe
+```
+---
+Have fun!
```

### Comparing `morepipes-1.0.0/morepipes.py` & `morepipes-1.0.1/morepipes.py`

 * *Files identical despite different names*

### Comparing `morepipes-1.0.0/pyproject.toml` & `morepipes-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "morepipes"
-version = "1.0.0"
+version = "1.0.1"
 description = "Extended pipes for functional programming"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

