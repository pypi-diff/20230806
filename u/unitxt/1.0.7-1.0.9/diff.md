# Comparing `tmp/unitxt-1.0.7.tar.gz` & `tmp/unitxt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.0.7.tar", last modified: Sun Jul 16 11:51:23 2023, max compression
+gzip compressed data, was "unitxt-1.0.9.tar", last modified: Tue Jul 18 07:56:19 2023, max compression
```

## Comparing `unitxt-1.0.7.tar` & `unitxt-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 11:51:14.000000 unitxt-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 11:51:14.000000 unitxt-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 11:51:23.665161 unitxt-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-16 11:51:14.000000 unitxt-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-16 11:51:14.000000 unitxt-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:51:23.665161 unitxt-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-16 11:51:22.000000 unitxt-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.661161 unitxt-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/src/unitxt/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/fusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/src/unitxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:19.359628 unitxt-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 07:56:07.000000 unitxt-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 07:56:07.000000 unitxt-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-18 07:56:19.359628 unitxt-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-18 07:56:07.000000 unitxt-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:56:07.000000 unitxt-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:56:19.359628 unitxt-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-18 07:56:18.000000 unitxt-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:19.355628 unitxt-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:19.355628 unitxt-1.0.9/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:19.359628 unitxt-1.0.9/src/unitxt/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/test_utils/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/test_utils/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 07:56:07.000000 unitxt-1.0.9/src/unitxt/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:19.359628 unitxt-1.0.9/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-18 07:56:19.000000 unitxt-1.0.9/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-18 07:56:19.000000 unitxt-1.0.9/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:56:19.000000 unitxt-1.0.9/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 07:56:19.000000 unitxt-1.0.9/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 07:56:19.000000 unitxt-1.0.9/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.0.7/LICENSE` & `unitxt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/PKG-INFO` & `unitxt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.0.7
+Version: 1.0.9
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unitxt-1.0.7/README.md` & `unitxt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/setup.py` & `unitxt-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
     
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="unitxt",
-    version="1.0.7",
+    version="1.0.9",
     author="IBM Research",
     author_email="elron.bandel@ibm.com",
     description="Load any mixture of text to text data in one line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibm/unitxt",
     packages=setuptools.find_packages('src'),
```

### Comparing `unitxt-1.0.7/src/unitxt/artifact.py` & `unitxt-1.0.9/src/unitxt/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __next__(self):
         return next(self.artifactories)
 
     def register_atrifactory(self, artifactory):
         assert isinstance(artifactory, Artifactory), "Artifactory must be an instance of Artifactory"
         assert hasattr(artifactory, "__contains__"), "Artifactory must have __contains__ method"
         assert hasattr(artifactory, "__getitem__"), "Artifactory must have __getitem__ method"
-        self.artifactories.append(artifactory)
+        self.artifactories = [artifactory] + self.artifactories
 
 
 class BaseArtifact(ABC):
     _class_register = {}
 
     @classmethod
     def is_artifact_dict(cls, d):
```

### Comparing `unitxt-1.0.7/src/unitxt/blocks.py` & `unitxt-1.0.9/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/card.py` & `unitxt-1.0.9/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/catalog.py` & `unitxt-1.0.9/src/unitxt/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/collections.py` & `unitxt-1.0.9/src/unitxt/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 class ListCollection(Collection):
     items: list = field(default_factory=list)
 
     def __getitem__(self, index):
         return self.items[index]
 
+    def __len__(self):
+        return len(self.items)
+
 
 class DictCollection(Collection):
     items: dict = field(default_factory=dict)
 
     def __getitem__(self, key):
         return self.items[key]
```

### Comparing `unitxt-1.0.7/src/unitxt/common.py` & `unitxt-1.0.9/src/unitxt/common.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/dataclass.py` & `unitxt-1.0.9/src/unitxt/dataclass.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/dataset.py` & `unitxt-1.0.9/src/unitxt/dataset.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/file_utils.py` & `unitxt-1.0.9/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/generator_utils.py` & `unitxt-1.0.9/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/instructions.py` & `unitxt-1.0.9/src/unitxt/instructions.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/loaders.py` & `unitxt-1.0.9/src/unitxt/loaders.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/metric.py` & `unitxt-1.0.9/src/unitxt/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,28 @@
             MergeStreams(),
         ]
 
 
 UNITXT_METRIC_SCHEMA = Features({"predictions": Value("string"), "references": dict(UNITXT_DATASET_SCHEMA)})
 
 
+def _compute(predictions: List[str], references: Iterable, flatten: bool = False, split_name: str = "all"):
+        recipe = MetricRecipe()
+
+        multi_stream = recipe(predictions=predictions, references=references, split_name=split_name)
+
+        if flatten:
+            operator = FlattenInstances()
+            multi_stream = operator(multi_stream)
+
+        stream = multi_stream[split_name]
+
+        return list(stream)
+
+
 # @evaluate.utils.file_utils.add_start_docstrings(_DESCRIPTION, _KWARGS_DESCRIPTION)
 class Metric(evaluate.Metric):
     def _info(self):
         return evaluate.MetricInfo(
             description="_DESCRIPTION",
             citation="_CITATION",
             # inputs_description=_KWARGS_DESCRIPTION,
@@ -124,18 +138,8 @@
             reference_urls=[
                 "https://",
                 "https://",
             ],
         )
 
     def _compute(self, predictions: List[str], references: Iterable, flatten: bool = False, split_name: str = "all"):
-        recipe = MetricRecipe()
-
-        multi_stream = recipe(predictions=predictions, references=references, split_name=split_name)
-
-        if flatten:
-            operator = FlattenInstances()
-            multi_stream = operator(multi_stream)
-
-        stream = multi_stream[split_name]
-
-        return list(stream)
+        return _compute(predictions=predictions, references=references, flatten=flatten, split_name=split_name)
```

### Comparing `unitxt-1.0.7/src/unitxt/metrics.py` & `unitxt-1.0.9/src/unitxt/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/normalizers.py` & `unitxt-1.0.9/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/operator.py` & `unitxt-1.0.9/src/unitxt/operator.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/operators.py` & `unitxt-1.0.9/src/unitxt/operators.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,28 @@
 
 class FromIterables(StreamInitializerOperator):
     def process(self, iterables: Dict[str, Iterable]) -> MultiStream:
         return MultiStream.from_iterables(iterables)
 
 
 class MapInstanceValues(StreamInstanceOperator):
+    """A class used to map instance values in a stream.
+
+    This class is a type of StreamInstanceOperator, and its main purpose
+    is to map values of instances in a stream using predefined mappers.
+
+    Attributes:
+        mappers (Dict[str, Dict[str, str]]): The mappers to use for mapping instance values.
+            Keys are the names of the fields to be mapped, and values are dictionaries
+            that define the mapping from old values to new values.
+        strict (bool): If True, the mapping is applied strictly. That means if a value 
+            does not exist in the mapper, it will raise a KeyError. If False, values 
+            that are not present in the mapper are kept as they are.
+
+    """
     mappers: Dict[str, Dict[str, str]]
     strict: bool = True
 
     def verify(self):
         # make sure the mappers are valid
         for key, mapper in self.mappers.items():
             assert isinstance(mapper, dict), f"Mapper for given field {key} should be a dict, got {type(mapper)}"
@@ -53,16 +67,20 @@
             items.extend(flatten_dict(v, new_key, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 
 class FlattenInstances(StreamInstanceOperator):
+    
+    parent_key: str = ""
+    sep: str = "_"
+    
     def process(self, instance: Dict[str, Any], stream_name: str = None) -> Dict[str, Any]:
-        return flatten_dict(instance)
+        return flatten_dict(instance, parent_key=self.parent_key, sep=self.sep)
 
 
 class AddFields(StreamInstanceOperator):
     fields: Dict[str, object]
 
     def process(self, instance: Dict[str, Any], stream_name: str = None) -> Dict[str, Any]:
         return {**instance, **self.fields}
```

### Comparing `unitxt-1.0.7/src/unitxt/register.py` & `unitxt-1.0.9/src/unitxt/register.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,30 @@
     "register.py",
     "metric.py",
     "dataset.py",
     "blocks.py",
 ]
 
 
+
+def _register_catalog(catalog: LocalCatalog):
+    Artifactories().register_atrifactory(catalog)
+
+def register_local_catalog(catalog_path: str):
+    assert os.path.exists(catalog_path), f"Catalog path {catalog_path} does not exist."
+    assert os.path.isdir(catalog_path), f"Catalog path {catalog_path} is not a directory."
+    _register_catalog(LocalCatalog(location=catalog_path))
+
 def _register_all_catalogs():
-    Artifactories().register_atrifactory(LocalCatalog())
+    _register_catalog(GithubCatalog())
+    _register_catalog(LocalCatalog())
     if UNITXT_ARTIFACTORIES_ENV_VAR in os.environ:
         for path in os.environ[UNITXT_ARTIFACTORIES_ENV_VAR].split(PATHS_SEP):
-            Artifactories().register_atrifactory(LocalCatalog(location=path))
-    Artifactories().register_atrifactory(GithubCatalog())
+            _register_catalog(LocalCatalog(location=path))
+    
 
 def _register_all_artifacts():
     dir = os.path.dirname(__file__)
     file_name = os.path.basename(__file__)
 
     for file in os.listdir(dir):
         if file.endswith(".py") and file not in non_registered_files and file != file_name:
```

### Comparing `unitxt-1.0.7/src/unitxt/schema.py` & `unitxt-1.0.9/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/split_utils.py` & `unitxt-1.0.9/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/splitters.py` & `unitxt-1.0.9/src/unitxt/splitters.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/stream.py` & `unitxt-1.0.9/src/unitxt/stream.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/task.py` & `unitxt-1.0.9/src/unitxt/task.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/templates.py` & `unitxt-1.0.9/src/unitxt/templates.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/text_utils.py` & `unitxt-1.0.9/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt/validate.py` & `unitxt-1.0.9/src/unitxt/validate.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.7/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.0.9/src/unitxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.0.7
+Version: 1.0.9
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unitxt-1.0.7/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.0.9/src/unitxt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 src/unitxt/schema.py
 src/unitxt/split_utils.py
 src/unitxt/splitters.py
 src/unitxt/stream.py
 src/unitxt/task.py
 src/unitxt/templates.py
 src/unitxt/text_utils.py
+src/unitxt/type_utils.py
 src/unitxt/utils.py
 src/unitxt/validate.py
 src/unitxt.egg-info/PKG-INFO
 src/unitxt.egg-info/SOURCES.txt
 src/unitxt.egg-info/dependency_links.txt
 src/unitxt.egg-info/requires.txt
-src/unitxt.egg-info/top_level.txt
+src/unitxt.egg-info/top_level.txt
+src/unitxt/test_utils/__init__.py
+src/unitxt/test_utils/card.py
+src/unitxt/test_utils/operators.py
```

