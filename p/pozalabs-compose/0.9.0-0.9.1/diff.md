# Comparing `tmp/pozalabs-compose-0.9.0.tar.gz` & `tmp/pozalabs-compose-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pozalabs-compose-0.9.0.tar", max compression
+gzip compressed data, was "pozalabs-compose-0.9.1.tar", max compression
```

## Comparing `pozalabs-compose-0.9.0.tar` & `pozalabs-compose-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1065 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/LICENSE.md
--rw-r--r--   0        0        0      328 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/__init__.py
--rw-r--r--   0        0        0       52 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/command/__init__.py
--rw-r--r--   0        0        0       71 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/command/command.py
--rw-r--r--   0        0        0     2634 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/container.py
--rw-r--r--   0        0        0      143 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/dependency/__init__.py
--rw-r--r--   0        0        0     2267 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/dependency/wiring.py
--rw-r--r--   0        0        0      842 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/entity.py
--rw-r--r--   0        0        0       46 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/event/__init__.py
--rw-r--r--   0        0        0      175 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/event/event.py
--rw-r--r--   0        0        0      809 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/exceptions.py
--rw-r--r--   0        0        0      564 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/field.py
--rw-r--r--   0        0        0      926 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/pagination.py
--rw-r--r--   0        0        0      133 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/__init__.py
--rw-r--r--   0        0        0      128 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/base.py
--rw-r--r--   0        0        0       94 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/__init__.py
--rw-r--r--   0        0        0      388 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/__init__.py
--rw-r--r--   0        0        0      561 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/aggregation.py
--rw-r--r--   0        0        0     1704 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/base.py
--rw-r--r--   0        0        0     1818 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/comparison.py
--rw-r--r--   0        0        0      871 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/logical.py
--rw-r--r--   0        0        0     1249 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/pagination.py
--rw-r--r--   0        0        0      279 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/pipeline.py
--rw-r--r--   0        0        0      256 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/sort.py
--rw-r--r--   0        0        0     4300 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/stage.py
--rw-r--r--   0        0        0      557 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/types.py
--rw-r--r--   0        0        0      432 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/op/utils.py
--rw-r--r--   0        0        0      595 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/query/mongo/query.py
--rw-r--r--   0        0        0       66 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/repository/__init__.py
--rw-r--r--   0        0        0       30 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/repository/base.py
--rw-r--r--   0        0        0     3201 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/repository/mongo.py
--rw-r--r--   0        0        0      131 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/schema/__init__.py
--rw-r--r--   0        0        0     1439 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/schema/extra.py
--rw-r--r--   0        0        0     2610 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/schema/schema.py
--rw-r--r--   0        0        0      103 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/types/__init__.py
--rw-r--r--   0        0        0      586 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/types/datetime.py
--rw-r--r--   0        0        0      578 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/types/object_id.py
--rw-r--r--   0        0        0      419 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/compose/utils.py
--rw-r--r--   0        0        0     1184 2023-04-08 04:13:55.263667 pozalabs-compose-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 pozalabs-compose-0.9.0/setup.py
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 pozalabs-compose-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0      328 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/command/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/command/command.py
+-rw-r--r--   0        0        0     2634 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/container.py
+-rw-r--r--   0        0        0      143 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/dependency/__init__.py
+-rw-r--r--   0        0        0     2267 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/dependency/wiring.py
+-rw-r--r--   0        0        0      842 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/entity.py
+-rw-r--r--   0        0        0       46 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/event/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/event/event.py
+-rw-r--r--   0        0        0      809 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/exceptions.py
+-rw-r--r--   0        0        0      564 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/field.py
+-rw-r--r--   0        0        0      926 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/pagination.py
+-rw-r--r--   0        0        0      133 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/__init__.py
+-rw-r--r--   0        0        0      128 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/base.py
+-rw-r--r--   0        0        0       94 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/__init__.py
+-rw-r--r--   0        0        0      388 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/__init__.py
+-rw-r--r--   0        0        0      561 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/aggregation.py
+-rw-r--r--   0        0        0     1704 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/base.py
+-rw-r--r--   0        0        0     1818 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/comparison.py
+-rw-r--r--   0        0        0      871 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/logical.py
+-rw-r--r--   0        0        0     1249 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/pagination.py
+-rw-r--r--   0        0        0      279 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/pipeline.py
+-rw-r--r--   0        0        0      256 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/sort.py
+-rw-r--r--   0        0        0     4299 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/stage.py
+-rw-r--r--   0        0        0      557 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/types.py
+-rw-r--r--   0        0        0      432 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/op/utils.py
+-rw-r--r--   0        0        0      595 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/query/mongo/query.py
+-rw-r--r--   0        0        0       66 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/repository/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/repository/base.py
+-rw-r--r--   0        0        0     3201 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/repository/mongo.py
+-rw-r--r--   0        0        0      131 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/schema/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/schema/extra.py
+-rw-r--r--   0        0        0     2610 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/schema/schema.py
+-rw-r--r--   0        0        0      103 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/types/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/types/datetime.py
+-rw-r--r--   0        0        0      578 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/types/object_id.py
+-rw-r--r--   0        0        0      419 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/compose/utils.py
+-rw-r--r--   0        0        0     1184 2023-04-08 05:12:03.217059 pozalabs-compose-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 pozalabs-compose-0.9.1/setup.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 pozalabs-compose-0.9.1/PKG-INFO
```

### Comparing `pozalabs-compose-0.9.0/LICENSE.md` & `pozalabs-compose-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/container.py` & `pozalabs-compose-0.9.1/compose/container.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/dependency/wiring.py` & `pozalabs-compose-0.9.1/compose/dependency/wiring.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/entity.py` & `pozalabs-compose-0.9.1/compose/entity.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/exceptions.py` & `pozalabs-compose-0.9.1/compose/exceptions.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/field.py` & `pozalabs-compose-0.9.1/compose/field.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/pagination.py` & `pozalabs-compose-0.9.1/compose/pagination.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/aggregation.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/aggregation.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/base.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/base.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/comparison.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/comparison.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/logical.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/logical.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/pagination.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/pagination.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/stage.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 class TextSearchOperator(Operator):
     def __init__(self, query: str, path: Union[str, list[str]]):
         self.query = query
         self.path = path
 
     def expression(self) -> DictExpression:
-        return {"$text": {"query": self.query, "path": self.path}}
+        return {"text": {"query": self.query, "path": self.path}}
 
 
 class Search(Stage):
     def __init__(self, index: str, op: Operator):
         self.index = index
         self.op = op
```

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/op/types.py` & `pozalabs-compose-0.9.1/compose/query/mongo/op/types.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/query/mongo/query.py` & `pozalabs-compose-0.9.1/compose/query/mongo/query.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/repository/mongo.py` & `pozalabs-compose-0.9.1/compose/repository/mongo.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/schema/extra.py` & `pozalabs-compose-0.9.1/compose/schema/extra.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/schema/schema.py` & `pozalabs-compose-0.9.1/compose/schema/schema.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/types/datetime.py` & `pozalabs-compose-0.9.1/compose/types/datetime.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/compose/types/object_id.py` & `pozalabs-compose-0.9.1/compose/types/object_id.py`

 * *Files identical despite different names*

### Comparing `pozalabs-compose-0.9.0/pyproject.toml` & `pozalabs-compose-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pozalabs-compose"
-version = "0.9.0"
+version = "0.9.1"
 description = "Backend components for POZAlabs"
 license = "MIT"
 authors = ["sunwoong <sunwoong@pozalabs.com>"]
 packages = [{include = "compose"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `pozalabs-compose-0.9.0/setup.py` & `pozalabs-compose-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'inflection>=0.5.1,<0.6.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pymongo[aws]>=4.3.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'pozalabs-compose',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Backend components for POZAlabs',
     'long_description': 'None',
     'author': 'sunwoong',
     'author_email': 'sunwoong@pozalabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pozalabs-compose-0.9.0/PKG-INFO` & `pozalabs-compose-0.9.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pozalabs-compose
-Version: 0.9.0
+Version: 0.9.1
 Summary: Backend components for POZAlabs
 License: MIT
 Author: sunwoong
 Author-email: sunwoong@pozalabs.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

