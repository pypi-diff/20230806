# Comparing `tmp/pysigma-0.9.8.tar.gz` & `tmp/pysigma-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma-0.9.8.tar", max compression
+gzip compressed data, was "pysigma-0.9.9.tar", max compression
```

## Comparing `pysigma-0.9.8.tar` & `pysigma-0.9.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    26526 2023-04-30 23:18:55.855612 pysigma-0.9.8/LICENSE
--rw-r--r--   0        0        0     9849 2023-04-30 23:18:55.855612 pysigma-0.9.8/README.md
--rw-r--r--   0        0        0      992 2023-04-30 23:18:55.859612 pysigma-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      238 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/backends/test/__init__.py
--rw-r--r--   0        0        0     5504 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/backends/test/backend.py
--rw-r--r--   0        0        0     8202 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/collection.py
--rw-r--r--   0        0        0     9805 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/conditions.py
--rw-r--r--   0        0        0        0 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/conversion/__init__.py
--rw-r--r--   0        0        0    52093 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/conversion/base.py
--rw-r--r--   0        0        0     3401 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/conversion/deferred.py
--rw-r--r--   0        0        0     1307 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/conversion/state.py
--rw-r--r--   0        0        0    43469 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/data/mitre_attack.py
--rw-r--r--   0        0        0     3735 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/exceptions.py
--rw-r--r--   0        0        0    14729 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/modifiers.py
--rw-r--r--   0        0        0     8799 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/pipelines/common.py
--rw-r--r--   0        0        0      212 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/pipelines/test/__init__.py
--rw-r--r--   0        0        0      874 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/pipelines/test/pipeline.py
--rw-r--r--   0        0        0     8401 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/plugins.py
--rw-r--r--   0        0        0        0 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/__init__.py
--rw-r--r--   0        0        0    12233 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/conditions.py
--rw-r--r--   0        0        0    16539 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/pipeline.py
--rw-r--r--   0        0        0     3680 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/resolver.py
--rw-r--r--   0        0        0     2763 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/tracking.py
--rw-r--r--   0        0        0    25461 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/processing/transformations.py
--rw-r--r--   0        0        0    30901 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/rule.py
--rw-r--r--   0        0        0    30355 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/types.py
--rw-r--r--   0        0        0     5956 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validation.py
--rw-r--r--   0        0        0    10301 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/base.py
--rw-r--r--   0        0        0      773 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/condition.py
--rw-r--r--   0        0        0     2976 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/logsources.py
--rw-r--r--   0        0        0     1545 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/metadata.py
--rw-r--r--   0        0        0     2832 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/modifiers.py
--rw-r--r--   0        0        0     3280 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/tags.py
--rw-r--r--   0        0        0     5627 2023-04-30 23:18:55.859612 pysigma-0.9.8/sigma/validators/core/values.py
--rw-r--r--   0        0        0    11003 1970-01-01 00:00:00.000000 pysigma-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-11 23:09:14.948389 pysigma-0.9.9/LICENSE
+-rw-r--r--   0        0        0     9849 2023-05-11 23:09:14.948389 pysigma-0.9.9/README.md
+-rw-r--r--   0        0        0      992 2023-05-11 23:09:14.952389 pysigma-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/backends/test/__init__.py
+-rw-r--r--   0        0        0     5504 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/backends/test/backend.py
+-rw-r--r--   0        0        0     8202 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/collection.py
+-rw-r--r--   0        0        0     9805 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/conditions.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/conversion/__init__.py
+-rw-r--r--   0        0        0    52093 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/conversion/base.py
+-rw-r--r--   0        0        0     3401 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/conversion/deferred.py
+-rw-r--r--   0        0        0     1307 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/conversion/state.py
+-rw-r--r--   0        0        0    70089 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/data/mitre_attack.py
+-rw-r--r--   0        0        0     3735 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/exceptions.py
+-rw-r--r--   0        0        0    14729 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/modifiers.py
+-rw-r--r--   0        0        0     8799 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/pipelines/common.py
+-rw-r--r--   0        0        0      212 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/pipelines/test/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/pipelines/test/pipeline.py
+-rw-r--r--   0        0        0     8401 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/processing/__init__.py
+-rw-r--r--   0        0        0    12233 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/processing/conditions.py
+-rw-r--r--   0        0        0    16539 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/processing/pipeline.py
+-rw-r--r--   0        0        0     3680 2023-05-11 23:09:14.952389 pysigma-0.9.9/sigma/processing/resolver.py
+-rw-r--r--   0        0        0     2763 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/processing/tracking.py
+-rw-r--r--   0        0        0    25461 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/processing/transformations.py
+-rw-r--r--   0        0        0    30901 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/rule.py
+-rw-r--r--   0        0        0    30355 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/types.py
+-rw-r--r--   0        0        0     5956 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validation.py
+-rw-r--r--   0        0        0    10301 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/base.py
+-rw-r--r--   0        0        0      773 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/__init__.py
+-rw-r--r--   0        0        0     4099 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/condition.py
+-rw-r--r--   0        0        0     2976 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/logsources.py
+-rw-r--r--   0        0        0     1545 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/metadata.py
+-rw-r--r--   0        0        0     2832 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/modifiers.py
+-rw-r--r--   0        0        0     3280 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/tags.py
+-rw-r--r--   0        0        0     5627 2023-05-11 23:09:14.956389 pysigma-0.9.9/sigma/validators/core/values.py
+-rw-r--r--   0        0        0    11003 1970-01-01 00:00:00.000000 pysigma-0.9.9/PKG-INFO
```

### Comparing `pysigma-0.9.8/LICENSE` & `pysigma-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/README.md` & `pysigma-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/pyproject.toml` & `pysigma-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma"
-version = "0.9.8"
+version = "0.9.9"
 license = "LGPL-2.1-only"
 description = "Sigma rule processing and conversion tools"
 authors = ["Thomas Patzke <thomas@patzke.org>"]
 readme = "README.md"
 repository = "https://github.com/SigmaHQ/pySigma"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pysigma-0.9.8/sigma/backends/test/backend.py` & `pysigma-0.9.9/sigma/backends/test/backend.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/collection.py` & `pysigma-0.9.9/sigma/collection.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/conditions.py` & `pysigma-0.9.9/sigma/conditions.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/conversion/base.py` & `pysigma-0.9.9/sigma/conversion/base.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/conversion/deferred.py` & `pysigma-0.9.9/sigma/conversion/deferred.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/conversion/state.py` & `pysigma-0.9.9/sigma/conversion/state.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/exceptions.py` & `pysigma-0.9.9/sigma/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/modifiers.py` & `pysigma-0.9.9/sigma/modifiers.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/pipelines/common.py` & `pysigma-0.9.9/sigma/pipelines/common.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/pipelines/test/pipeline.py` & `pysigma-0.9.9/sigma/pipelines/test/pipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/plugins.py` & `pysigma-0.9.9/sigma/plugins.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/processing/conditions.py` & `pysigma-0.9.9/sigma/processing/conditions.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/processing/pipeline.py` & `pysigma-0.9.9/sigma/processing/pipeline.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/processing/resolver.py` & `pysigma-0.9.9/sigma/processing/resolver.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/processing/tracking.py` & `pysigma-0.9.9/sigma/processing/tracking.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/processing/transformations.py` & `pysigma-0.9.9/sigma/processing/transformations.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/rule.py` & `pysigma-0.9.9/sigma/rule.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/types.py` & `pysigma-0.9.9/sigma/types.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validation.py` & `pysigma-0.9.9/sigma/validation.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/base.py` & `pysigma-0.9.9/sigma/validators/base.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/__init__.py` & `pysigma-0.9.9/sigma/validators/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/condition.py` & `pysigma-0.9.9/sigma/validators/core/condition.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/logsources.py` & `pysigma-0.9.9/sigma/validators/core/logsources.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/metadata.py` & `pysigma-0.9.9/sigma/validators/core/metadata.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/modifiers.py` & `pysigma-0.9.9/sigma/validators/core/modifiers.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/tags.py` & `pysigma-0.9.9/sigma/validators/core/tags.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/sigma/validators/core/values.py` & `pysigma-0.9.9/sigma/validators/core/values.py`

 * *Files identical despite different names*

### Comparing `pysigma-0.9.8/PKG-INFO` & `pysigma-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma
-Version: 0.9.8
+Version: 0.9.9
 Summary: Sigma rule processing and conversion tools
 Home-page: https://github.com/SigmaHQ/pySigma
 License: LGPL-2.1-only
 Author: Thomas Patzke
 Author-email: thomas@patzke.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

