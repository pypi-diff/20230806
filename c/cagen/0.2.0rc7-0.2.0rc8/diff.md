# Comparing `tmp/cagen-0.2.0rc7.tar.gz` & `tmp/cagen-0.2.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0rc7.tar", last modified: Sun Aug  6 14:38:40 2023, max compression
+gzip compressed data, was "cagen-0.2.0rc8.tar", last modified: Sun Aug  6 15:09:57 2023, max compression
```

## Comparing `cagen-0.2.0rc7.tar` & `cagen-0.2.0rc8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 14:38:40.904861 cagen-0.2.0rc7/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0rc7/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-08-06 14:38:40.904861 cagen-0.2.0rc7/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0rc7/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1148 2023-08-06 14:37:39.000000 cagen-0.2.0rc7/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-08-06 14:38:40.904861 cagen-0.2.0rc7/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 14:38:40.901528 cagen-0.2.0rc7/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 14:38:40.901528 cagen-0.2.0rc7/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0rc7/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4659 2023-05-07 17:29:41.000000 cagen-0.2.0rc7/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     9440 2023-08-06 14:38:16.000000 cagen-0.2.0rc7/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 14:38:40.901528 cagen-0.2.0rc7/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      786 2023-05-08 16:32:54.000000 cagen-0.2.0rc7/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0rc7/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     3998 2023-05-07 17:21:41.000000 cagen-0.2.0rc7/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0rc7/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 14:38:40.901528 cagen-0.2.0rc7/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       80 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-08-06 14:38:40.000000 cagen-0.2.0rc7/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0rc8/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0rc8/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1148 2023-08-06 15:09:14.000000 cagen-0.2.0rc8/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0rc8/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4659 2023-05-07 17:29:41.000000 cagen-0.2.0rc8/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     9446 2023-08-06 15:09:38.000000 cagen-0.2.0rc8/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      786 2023-05-08 16:32:54.000000 cagen-0.2.0rc8/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0rc8/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     3998 2023-05-07 17:21:41.000000 cagen-0.2.0rc8/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0rc8/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-08-06 15:09:57.913236 cagen-0.2.0rc8/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       80 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-08-06 15:09:57.000000 cagen-0.2.0rc8/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0rc7/PKG-INFO` & `cagen-0.2.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0rc7/README.md` & `cagen-0.2.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc7/pyproject.toml` & `cagen-0.2.0rc8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.rc7"
+version = "0.2.0.rc8"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0rc7/src/cagen/cmd.py` & `cagen-0.2.0rc8/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc7/src/cagen/libcagen.py` & `cagen-0.2.0rc8/src/cagen/libcagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 c = criterium(x)
                 if isinstance(c, list) and v in c:
                     grouped[v].append(x)
                 if c == v:
                     grouped[v].append(x)
         return grouped
 
-    def select(criterium: Optional[types.FunctionType], value: Optional[str]):
+    def select(self, criterium: Optional[types.FunctionType], value: Optional[str]):
         """
         It return a list of entries.
         By default, it returns all entries
         Else, it returns [entry | criterium(entry) == value]
 
         It's up to user to define useful criterium for `Entry` collections: such backlinks,
         has_author, etc.
```

### Comparing `cagen-0.2.0rc7/src/cagen/templates/list.md.tmpl` & `cagen-0.2.0rc8/src/cagen/templates/list.md.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc7/src/cagen/templates/schema.tmpl` & `cagen-0.2.0rc8/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0rc7/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0rc8/src/cagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

