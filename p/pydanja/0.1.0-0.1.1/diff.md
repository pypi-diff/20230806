# Comparing `tmp/pydanja-0.1.0.tar.gz` & `tmp/pydanja-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydanja-0.1.0.tar", last modified: Sun Aug  6 06:03:39 2023, max compression
+gzip compressed data, was "pydanja-0.1.1.tar", last modified: Sun Aug  6 10:53:56 2023, max compression
```

## Comparing `pydanja-0.1.0.tar` & `pydanja-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2684 2023-08-06 05:44:26.847331 pydanja-0.1.0/README.md
--rw-r--r--   0        0        0     1035 2023-08-06 06:03:39.589294 pydanja-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5488 2023-08-06 05:42:49.879483 pydanja-0.1.0/src/pydanja/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 pydanja-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2684 2023-08-06 10:16:20.525826 pydanja-0.1.1/README.md
+-rw-r--r--   0        0        0     1084 2023-08-06 10:53:56.004642 pydanja-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5488 2023-08-06 05:42:49.879483 pydanja-0.1.1/src/pydanja/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 04:57:14.398442 pydanja-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 pydanja-0.1.1/PKG-INFO
```

### Comparing `pydanja-0.1.0/README.md` & `pydanja-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.0/pyproject.toml` & `pydanja-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "pydanja"
-version = "0.1.0"
+version = "0.1.1"
 description = "JSON:API Support for Pydantic"
 authors = [
     { name = "Chris Read", email = "centurix@gmail.com" },
 ]
 dependencies = [
     "pydantic>=2.1.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 repository = "https://github.com/Centurix/pydanja"
+homepage = "https://github.com/Centurix/pydanja"
 keywords = [
     "pydantic",
     "jsonapi",
     "json:api",
     "openapi",
     "fastapi",
 ]
```

### Comparing `pydanja-0.1.0/src/pydanja/__init__.py` & `pydanja-0.1.1/src/pydanja/__init__.py`

 * *Files identical despite different names*

### Comparing `pydanja-0.1.0/PKG-INFO` & `pydanja-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydanja
-Version: 0.1.0
+Version: 0.1.1
 Summary: JSON:API Support for Pydantic
 Keywords: pydantic jsonapi json:api openapi fastapi
 Author-Email: Chris Read <centurix@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

