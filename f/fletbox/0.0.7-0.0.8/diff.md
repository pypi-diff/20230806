# Comparing `tmp/fletbox-0.0.7.tar.gz` & `tmp/fletbox-0.0.8.tar.gz`

## Comparing `fletbox-0.0.7.tar` & `fletbox-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.0.7/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fletbox-0.0.7/src/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.0.7/src/fletbox/__init__.py
--rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 fletbox-0.0.7/src/fletbox/fletbox.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fletbox-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.0.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fletbox-0.0.7/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fletbox-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fletbox-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/fletbox/__init__.py
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 fletbox-0.0.8/src/fletbox/fletbox.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fletbox-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fletbox-0.0.8/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fletbox-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fletbox-0.0.8/PKG-INFO
```

### Comparing `fletbox-0.0.7/src/fletbox/fletbox.py` & `fletbox-0.0.8/src/fletbox/fletbox.py`

 * *Files identical despite different names*

### Comparing `fletbox-0.0.7/LICENSE` & `fletbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fletbox-0.0.7/pyproject.toml` & `fletbox-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fletbox"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Xynon", email="" },
 ]
 description = "A box for flet, abusing contextmanagers and decorators"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

