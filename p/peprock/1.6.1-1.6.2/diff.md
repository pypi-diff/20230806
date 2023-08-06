# Comparing `tmp/peprock-1.6.1.tar.gz` & `tmp/peprock-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peprock-1.6.1.tar", max compression
+gzip compressed data, was "peprock-1.6.2.tar", max compression
```

## Comparing `peprock-1.6.1.tar` & `peprock-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1083 2023-08-06 17:14:26.272859 peprock-1.6.1/LICENSE
--rw-r--r--   0        0        0     1780 2023-08-06 17:14:26.272859 peprock-1.6.1/README.md
--rw-r--r--   0        0        0       27 2023-08-06 17:14:52.834633 peprock-1.6.1/peprock/_version/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/_version/py.typed
--rw-r--r--   0        0        0      753 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/__init__.py
--rw-r--r--   0        0        0     2456 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/awareness.py
--rw-r--r--   0        0        0      897 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/constants.py
--rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/py.typed
--rw-r--r--   0        0        0      298 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/__init__.py
--rw-r--r--   0        0        0    20114 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/measurement.py
--rw-r--r--   0        0        0     4312 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/metric_prefix.py
--rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/py.typed
--rw-r--r--   0        0        0     1965 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/unit.py
--rw-r--r--   0        0        0      128 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/__init__.py
--rw-r--r--   0        0        0     2063 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/observer.py
--rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/py.typed
--rw-r--r--   0        0        0     1730 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/subclasses/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/subclasses/py.typed
--rw-r--r--   0        0        0     4081 2023-08-06 17:14:52.894636 peprock-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 peprock-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-06 17:39:59.903303 peprock-1.6.2/LICENSE
+-rw-r--r--   0        0        0     1780 2023-08-06 17:39:59.903303 peprock-1.6.2/README.md
+-rw-r--r--   0        0        0       27 2023-08-06 17:40:22.735294 peprock-1.6.2/peprock/_version/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/_version/py.typed
+-rw-r--r--   0        0        0      753 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/datetime/__init__.py
+-rw-r--r--   0        0        0     2456 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/datetime/awareness.py
+-rw-r--r--   0        0        0      897 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/datetime/constants.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/datetime/py.typed
+-rw-r--r--   0        0        0      298 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/models/__init__.py
+-rw-r--r--   0        0        0    20114 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/models/measurement.py
+-rw-r--r--   0        0        0     4312 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/models/metric_prefix.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/models/py.typed
+-rw-r--r--   0        0        0     1965 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/models/unit.py
+-rw-r--r--   0        0        0      128 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/patterns/__init__.py
+-rw-r--r--   0        0        0     2063 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/patterns/observer.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/patterns/py.typed
+-rw-r--r--   0        0        0     1730 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/subclasses/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:39:59.903303 peprock-1.6.2/peprock/subclasses/py.typed
+-rw-r--r--   0        0        0     4081 2023-08-06 17:40:22.787294 peprock-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 peprock-1.6.2/PKG-INFO
```

### Comparing `peprock-1.6.1/LICENSE` & `peprock-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/README.md` & `peprock-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/datetime/__init__.py` & `peprock-1.6.2/peprock/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/datetime/awareness.py` & `peprock-1.6.2/peprock/datetime/awareness.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/datetime/constants.py` & `peprock-1.6.2/peprock/datetime/constants.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/models/measurement.py` & `peprock-1.6.2/peprock/models/measurement.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/models/metric_prefix.py` & `peprock-1.6.2/peprock/models/metric_prefix.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/models/unit.py` & `peprock-1.6.2/peprock/models/unit.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/patterns/observer.py` & `peprock-1.6.2/peprock/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/peprock/subclasses/__init__.py` & `peprock-1.6.2/peprock/subclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.1/pyproject.toml` & `peprock-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.commitizen]
 bump_message = "chore: bump version to $new_version"
 changelog_incremental = true
 update_changelog_on_bump = true
-version = "1.6.1"
+version = "1.6.2"
 version_files = [
     "peprock/_version/__init__.py",
     "pyproject.toml",
 ]
 
 
 [tool.coverage.report]
@@ -33,15 +33,15 @@
 warn_unused_ignores = true
 warn_unused_configs = true
 warn_unreachable = true
 
 
 [tool.poetry]
 name = "peprock"
-version = "1.6.1"
+version = "1.6.2"
 description = "Foundational Python library"
 license = "MIT"
 authors = [
     "Jakob Keller <57402305+jakob-keller@users.noreply.github.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Ponte-Energy-Partners/peprock"
```

### Comparing `peprock-1.6.1/PKG-INFO` & `peprock-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peprock
-Version: 1.6.1
+Version: 1.6.2
 Summary: Foundational Python library
 Home-page: https://github.com/Ponte-Energy-Partners/peprock
 License: MIT
 Keywords: peprock,datetime,models,patterns,subclasses
 Author: Jakob Keller
 Author-email: 57402305+jakob-keller@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

