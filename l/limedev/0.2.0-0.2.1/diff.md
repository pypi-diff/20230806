# Comparing `tmp/limedev-0.2.0.tar.gz` & `tmp/limedev-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limedev-0.2.0.tar", last modified: Sun Aug  6 18:43:15 2023, max compression
+gzip compressed data, was "limedev-0.2.1.tar", last modified: Sun Aug  6 19:44:58 2023, max compression
```

## Comparing `limedev-0.2.0.tar` & `limedev-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-06 18:42:57.000000 limedev-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-06 18:43:15.594129 limedev-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-06 18:43:08.000000 limedev-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/_main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/package.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-06 18:43:08.000000 limedev-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:43:15.594129 limedev-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.590129 limedev-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/src/limedev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/_API.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/src/limedev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:58.398364 limedev-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-06 19:44:44.000000 limedev-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-06 19:44:58.398364 limedev-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-06 19:44:51.000000 limedev-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:58.394364 limedev-0.2.1/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/_main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/package.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-06 19:44:44.000000 limedev-0.2.1/dependencies/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-06 19:44:51.000000 limedev-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:44:58.398364 limedev-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:58.394364 limedev-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:58.394364 limedev-0.2.1/src/limedev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-08-06 19:44:44.000000 limedev-0.2.1/src/limedev/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:44:58.398364 limedev-0.2.1/src/limedev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 19:44:58.000000 limedev-0.2.1/src/limedev.egg-info/top_level.txt
```

### Comparing `limedev-0.2.0/LICENSE` & `limedev-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `limedev-0.2.0/PKG-INFO` & `limedev-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limedev
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkit for Python development, especially packaging 
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/limedev
 Project-URL: Changelog, https://github.com/Limespy/limedev/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/limedev/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
 
 # Quick start guide
 
-Here's how you can start numerically
+Here's how you can start
 
 ## The first steps
 
 ### Installing
 
 Install LimeDev with pip
 
@@ -61,14 +61,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
+## 0.2.1 2023-08-06 <!-- omit in toc -->
+
+- Performance results dump sorting fix
+
 ## 0.2.0 2023-08-06 <!-- omit in toc -->
 
 - Bugfixes
 - Cleaner structure
 - Reworked readme build
 
 ## 0.1.0 2023-05-04 <!-- omit in toc -->
```

### Comparing `limedev-0.2.0/README.md` & `limedev-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
 
 # Quick start guide
 
-Here's how you can start numerically
+Here's how you can start
 
 ## The first steps
 
 ### Installing
 
 Install LimeDev with pip
 
@@ -34,14 +34,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
+## 0.2.1 2023-08-06 <!-- omit in toc -->
+
+- Performance results dump sorting fix
+
 ## 0.2.0 2023-08-06 <!-- omit in toc -->
 
 - Bugfixes
 - Cleaner structure
 - Reworked readme build
 
 ## 0.1.0 2023-05-04 <!-- omit in toc -->
```

### Comparing `limedev-0.2.0/pyproject.toml` & `limedev-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "Limespy" },
 ]
 requires-python = ">=3.9"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 dynamic = [
     "dependencies",
     "optional-dependencies",
 ]
 
 [project.scripts]
 package = "limedev.package:main"
```

### Comparing `limedev-0.2.0/src/limedev/_aux.py` & `limedev-0.2.1/src/limedev/_aux.py`

 * *Files identical despite different names*

### Comparing `limedev-0.2.0/src/limedev/package.py` & `limedev-0.2.1/src/limedev/package.py`

 * *Files identical despite different names*

### Comparing `limedev-0.2.0/src/limedev/readme.py` & `limedev-0.2.1/src/limedev/readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     return doc
 #=======================================================================
 def make_setup_guide(name, pypiname, package_name, abbreviation = None
                      ) -> md.Document:
     '''Builds setup guide from metadata'''
     doc = md.Document([
         md.Heading('Quick start guide', 1),
-        "Here's how you can start numerically ",
+        "Here's how you can start ",
         md.Heading('The first steps', 2),
         md.Heading('Installing', 3),
         f'Install {name} with pip',
         md.CodeBlock(f'pip install {pypiname}'),
         md.Heading('Importing', 3),
         md.Paragraph([(f'Import name is '
                        f'{"" if pypiname == package_name else "not "}'
```

### Comparing `limedev-0.2.0/src/limedev/test.py` & `limedev-0.2.1/src/limedev/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     path_performance_data = path_tests / 'performance.yaml'
     version, results = performance_tests()
     with open(path_performance_data, encoding = 'utf8', mode = 'w+') as f:
         if (data := yaml.safe_load(f)) is None:
             data = {}
         f.seek(0)
         data[version] = results
-        f.write(yaml.safe_dump(data))
+        yaml.safe_dump(data, f, sort_keys = False, default_flow_style = False)
         f.truncate()
 #==============================================================================
 TESTS: dict[str, Callable] = {function.__name__: function # type: ignore
                               for function in
                               (lint, unittests, typing, profiling, performance)}
 def main(args: list[str] = sys.argv[1:]) -> int: # pylint: disable=dangerous-default-value
     '''Command line interface entry point'''
```

### Comparing `limedev-0.2.0/src/limedev.egg-info/PKG-INFO` & `limedev-0.2.1/src/limedev.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limedev
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkit for Python development, especially packaging 
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/limedev
 Project-URL: Changelog, https://github.com/Limespy/limedev/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/limedev/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -39,15 +39,15 @@
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
 
 # Quick start guide
 
-Here's how you can start numerically
+Here's how you can start
 
 ## The first steps
 
 ### Installing
 
 Install LimeDev with pip
 
@@ -61,14 +61,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
+## 0.2.1 2023-08-06 <!-- omit in toc -->
+
+- Performance results dump sorting fix
+
 ## 0.2.0 2023-08-06 <!-- omit in toc -->
 
 - Bugfixes
 - Cleaner structure
 - Reworked readme build
 
 ## 0.1.0 2023-05-04 <!-- omit in toc -->
```

### Comparing `limedev-0.2.0/src/limedev.egg-info/requires.txt` & `limedev-0.2.1/src/limedev.egg-info/requires.txt`

 * *Files identical despite different names*

