# Comparing `tmp/pipeline_ai-1.0.0b1.tar.gz` & `tmp/pipeline_ai-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-1.0.0b1.tar", max compression
+gzip compressed data, was "pipeline_ai-1.0.0b2.tar", max compression
```

## Comparing `pipeline_ai-1.0.0b1.tar` & `pipeline_ai-1.0.0b2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    10176 2023-08-02 11:56:14.698178 pipeline_ai-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     6130 2023-08-02 11:56:14.698178 pipeline_ai-1.0.0b1/README.md
--rw-r--r--   0        0        0      368 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/__main__.py
--rw-r--r--   0        0        0      300 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/__init__.py
--rw-r--r--   0        0        0      707 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/compute_requirements.py
--rw-r--r--   0        0        0      650 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/environments.py
--rw-r--r--   0        0        0     3827 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/http.py
--rw-r--r--   0        0        0     7936 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/pipelines.py
--rw-r--r--   0        0        0     1061 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/pointers.py
--rw-r--r--   0        0        0      706 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/__init__.py
--rw-r--r--   0        0        0     1209 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pipelines.py
--rw-r--r--   0        0        0      701 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pointers.py
--rw-r--r--   0        0        0     4268 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/runs.py
--rw-r--r--   0        0        0     3347 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0     1392 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/__init__.py
--rw-r--r--   0        0        0     2924 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/cluster.py
--rw-r--r--   0        0        0     2961 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/commands.py
--rw-r--r--   0        0        0        0 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/__init__.py
--rw-r--r--   0        0        0      410 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/environments.py
--rw-r--r--   0        0        0     4561 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/pipelines.py
--rw-r--r--   0        0        0     4960 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/pointers.py
--rw-r--r--   0        0        0     1859 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/resources.py
--rw-r--r--   0        0        0      509 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4764 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     1374 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/function.py
--rw-r--r--   0        0        0    13525 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/graph.py
--rw-r--r--   0        0        0     1090 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0      744 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/model.py
--rw-r--r--   0        0        0     1773 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1712 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0     2210 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1127 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0     1217 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pipeline_ai-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     6130 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/README.md
+-rw-r--r--   0        0        0      368 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/__main__.py
+-rw-r--r--   0        0        0      300 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/__init__.py
+-rw-r--r--   0        0        0     1827 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/compute_requirements.py
+-rw-r--r--   0        0        0      650 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/environments.py
+-rw-r--r--   0        0        0     3827 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/http.py
+-rw-r--r--   0        0        0     7936 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/pipelines.py
+-rw-r--r--   0        0        0     1061 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/pointers.py
+-rw-r--r--   0        0        0      706 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/schemas/__init__.py
+-rw-r--r--   0        0        0     1209 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/schemas/pipelines.py
+-rw-r--r--   0        0        0      701 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/schemas/pointers.py
+-rw-r--r--   0        0        0     4268 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/cloud/schemas/runs.py
+-rw-r--r--   0        0        0     3347 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0     1392 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     2924 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/cluster.py
+-rw-r--r--   0        0        0     2961 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/commands.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/targets/__init__.py
+-rw-r--r--   0        0        0      410 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/targets/environments.py
+-rw-r--r--   0        0        0     4561 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/targets/pipelines.py
+-rw-r--r--   0        0        0     4960 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/targets/pointers.py
+-rw-r--r--   0        0        0     2598 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/console/targets/resources.py
+-rw-r--r--   0        0        0      509 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4764 2023-08-06 14:24:12.388221 pipeline_ai-1.0.0b2/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     1374 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/function.py
+-rw-r--r--   0        0        0    13525 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/graph.py
+-rw-r--r--   0        0        0     1090 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0      744 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/model.py
+-rw-r--r--   0        0        0     1773 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1712 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0     2210 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1127 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0     1217 2023-08-06 14:24:12.392221 pipeline_ai-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pipeline_ai-1.0.0b2/PKG-INFO
```

### Comparing `pipeline_ai-1.0.0b1/LICENSE` & `pipeline_ai-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/README.md` & `pipeline_ai-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/environments.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/http.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/http.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/pipelines.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/pointers.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/__init__.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pipelines.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/schemas/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pointers.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/schemas/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/runs.py` & `pipeline_ai-1.0.0b2/pipeline/cloud/schemas/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/configuration/__init__.py` & `pipeline_ai-1.0.0b2/pipeline/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/console/__init__.py` & `pipeline_ai-1.0.0b2/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/console/cluster.py` & `pipeline_ai-1.0.0b2/pipeline/console/cluster.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/console/commands.py` & `pipeline_ai-1.0.0b2/pipeline/console/commands.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/console/targets/pipelines.py` & `pipeline_ai-1.0.0b2/pipeline/console/targets/pipelines.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/console/targets/pointers.py` & `pipeline_ai-1.0.0b2/pipeline/console/targets/pointers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/decorators.py` & `pipeline_ai-1.0.0b2/pipeline/objects/decorators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/environment/__init__.py` & `pipeline_ai-1.0.0b2/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/function.py` & `pipeline_ai-1.0.0b2/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/graph.py` & `pipeline_ai-1.0.0b2/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-1.0.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/model.py` & `pipeline_ai-1.0.0b2/pipeline/objects/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/pipeline.py` & `pipeline_ai-1.0.0b2/pipeline/objects/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/objects/wrappers.py` & `pipeline_ai-1.0.0b2/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/util/__init__.py` & `pipeline_ai-1.0.0b2/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pipeline/util/logging.py` & `pipeline_ai-1.0.0b2/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-1.0.0b1/pyproject.toml` & `pipeline_ai-1.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "1.0.0b1"
+version = "1.0.0b2"
 
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
   "Yvan Buggy <yvan@mystic.ai>",
```

### Comparing `pipeline_ai-1.0.0b1/PKG-INFO` & `pipeline_ai-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

