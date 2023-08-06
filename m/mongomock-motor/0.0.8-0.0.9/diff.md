# Comparing `tmp/mongomock_motor-0.0.8.tar.gz` & `tmp/mongomock_motor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomock_motor-0.0.8.tar", last modified: Tue May 10 11:57:34 2022, max compression
+gzip compressed data, was "mongomock_motor-0.0.9.tar", last modified: Tue May 24 13:51:07 2022, max compression
```

## Comparing `mongomock_motor-0.0.8.tar` & `mongomock_motor-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 11:57:34.861008 mongomock_motor-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-05-10 11:57:34.861008 mongomock_motor-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 11:57:34.857007 mongomock_motor-0.0.8/mongomock_motor/
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/mongomock_motor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/mongomock_motor/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 11:57:34.857007 mongomock_motor-0.0.8/mongomock_motor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-05-10 11:57:34.000000 mongomock_motor-0.0.8/mongomock_motor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-05-10 11:57:34.000000 mongomock_motor-0.0.8/mongomock_motor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-10 11:57:34.000000 mongomock_motor-0.0.8/mongomock_motor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-10 11:57:34.000000 mongomock_motor-0.0.8/mongomock_motor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-10 11:57:34.000000 mongomock_motor-0.0.8/mongomock_motor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-10 11:57:34.861008 mongomock_motor-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 11:57:34.861008 mongomock_motor-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_async_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_beanie.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_umongo.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_unique.py
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-05-10 11:57:10.000000 mongomock_motor-0.0.8/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 13:51:07.871413 mongomock_motor-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-05-24 13:51:07.871413 mongomock_motor-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 13:51:07.867413 mongomock_motor-0.0.9/mongomock_motor/
+-rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/mongomock_motor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/mongomock_motor/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 13:51:07.871413 mongomock_motor-0.0.9/mongomock_motor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-05-24 13:51:07.000000 mongomock_motor-0.0.9/mongomock_motor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-05-24 13:51:07.000000 mongomock_motor-0.0.9/mongomock_motor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-24 13:51:07.000000 mongomock_motor-0.0.9/mongomock_motor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-24 13:51:07.000000 mongomock_motor-0.0.9/mongomock_motor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-24 13:51:07.000000 mongomock_motor-0.0.9/mongomock_motor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-24 13:51:07.871413 mongomock_motor-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-24 13:51:07.871413 mongomock_motor-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_async_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_beanie.py
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_list_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_umongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_unique.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-05-24 13:50:34.000000 mongomock_motor-0.0.9/tests/test_workflow.py
```

### Comparing `mongomock_motor-0.0.8/PKG-INFO` & `mongomock_motor-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mongomock_motor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for mocking AsyncIOMotorClient built on top of mongomock.
 Home-page: https://github.com/michaelkryukov/mongomock_motor
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
-License: UNKNOWN
 Keywords: library,mongodb
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -35,9 +33,7 @@
     assert await collection.find({}).to_list(None) == []
 
     result = await collection.insert_one({'a': 1})
     assert result.inserted_id
 
     assert len(await collection.find({}).to_list(None)) == 1
 ```
-
-
```

### Comparing `mongomock_motor-0.0.8/README.md` & `mongomock_motor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mongomock_motor-0.0.8/mongomock_motor/__init__.py` & `mongomock_motor-0.0.9/mongomock_motor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,35 @@
             @property
             def __class__(self):
                 return target
         return Wrapper
     return decorator
 
 
+def apply_async_wrappers(instance, async_methods, target):
+    for method_name in async_methods:
+        def make_wrapper(method_name):
+            async def wrapper(*args, **kwargs):
+                return getattr(target, method_name)(*args, **kwargs)
+            return wrapper
+
+        setattr(instance, method_name, make_wrapper(method_name))
+
+
+def apply_chaining_wrappers(instance, chaining_methods, target):
+    for method_name in chaining_methods:
+        def make_wrapper(method_name):
+            def wrapper(*args, **kwargs):
+                getattr(target, method_name)(*args, **kwargs)
+                return instance
+            return wrapper
+
+        setattr(instance, method_name, make_wrapper(method_name))
+
+
 @masquerade_class('motor.motor_asyncio.AsyncIOMotorCursor')
 class AsyncCursor():
     PROXIED_CURSOR_CHAINING_METHODS = [
         'add_option',
         'allow_disk_use',
         'collation',
         'comment',
@@ -41,22 +62,19 @@
         'sort',
         'where',
     ]
 
     def __init__(self, cursor):
         self.__cursor = cursor
 
-        for method_name in self.PROXIED_CURSOR_CHAINING_METHODS:
-            def make_wrapper(method_name):
-                def wrapper(*args, **kwargs):
-                    getattr(self.__cursor, method_name)(*args, **kwargs)
-                    return self
-                return wrapper
-
-            setattr(self, method_name, make_wrapper(method_name))
+        apply_chaining_wrappers(
+            self,
+            self.PROXIED_CURSOR_CHAINING_METHODS,
+            self.__cursor,
+        )
 
     def __getattr__(self, name):
         return getattr(self.__cursor, name)
 
     def __aiter__(self):
         return self
 
@@ -69,95 +87,123 @@
     async def to_list(self, *args, **kwargs):
         return list(self.__cursor)
 
 
 @masquerade_class('motor.motor_asyncio.AsyncIOMotorCollection')
 class AsyncMongoMockCollection():
     ASYNC_METHODS = [
+        'bulk_write',
         'count_documents',
-        'count',
+        'count',  # deprecated
         'create_index',
         'create_indexes',
         'delete_many',
         'delete_one',
+        'drop_index',
+        'drop_indexes',
         'drop',
         'ensure_index',
         'estimated_document_count',
-        'find_and_modify',
+        'find_and_modify',  # deprecated
         'find_one_and_delete',
         'find_one_and_replace',
         'find_one_and_update',
         'find_one',
         'index_information',
+        'inline_map_reduce',
         'insert_many',
         'insert_one',
         'map_reduce',
+        'options',
+        'reindex',
+        'rename',
         'replace_one',
         'save',
         'update_many',
         'update_one',
     ]
 
     def __init__(self, collection):
         self.__collection = collection
-
-        for method_name in self.ASYNC_METHODS:
-            def make_wrapper(method_name):
-                async def wrapper(*args, **kwargs):
-                    return getattr(self.__collection, method_name)(*args, **kwargs)
-                return wrapper
-
-            setattr(self, method_name, make_wrapper(method_name))
+        apply_async_wrappers(self, self.ASYNC_METHODS, self.__collection)
 
     def __getattr__(self, name):
         return getattr(self.__collection, name)
 
     def find(self, *args, **kwargs) -> AsyncCursor:
         return AsyncCursor(self.__collection.find(*args, **kwargs))
 
     def aggregate(self, *args, **kwargs) -> AsyncCursor:
         return AsyncCursor(self.__collection.aggregate(*args, **kwargs))
 
 
 @masquerade_class('motor.motor_asyncio.AsyncIOMotorDatabase')
 class AsyncMongoMockDatabase():
+    ASYNC_METHODS = [
+        'create_collection',
+        'dereference',
+        'drop_collection',
+        'list_collection_names',
+        'validate_collection',
+    ]
+
     def __init__(self, database, mock_build_info=None):
         self.__database = database
-        self.__collections = {}
         self.__build_info = mock_build_info or {'ok': 1.0, 'version': '5.0.5'}
+        apply_async_wrappers(self, self.ASYNC_METHODS, self.__database)
+
+    def get_collection(self, *args, **kwargs):
+        return AsyncMongoMockCollection(
+            _patch_collection_internals(
+                self.__database.get_collection(*args, **kwargs),
+            ),
+        )
+
+    def aggregate(self, *args, **kwargs) -> AsyncCursor:
+        return AsyncCursor(self.__database.aggregate(*args, **kwargs))
 
     async def command(self, *args, **kwargs):
         try:
             return getattr(self.__database, 'command')(*args, **kwargs)
         except NotImplementedError:
             if args == ({'buildInfo': 1},) and not kwargs:
                 return self.__build_info
             raise
 
     def __getitem__(self, name):
-        return getattr(self, name)
+        return self.get_collection(name)
 
     def __getattr__(self, name):
-        if name not in self.__collections:
-            self.__collections[name] = AsyncMongoMockCollection(
-                _patch_collection_internals(self.__database[name]),
-            )
-        return self.__collections[name]
+        if name in dir(self.__database):
+            return getattr(self.__database, name)
+
+        return self.get_collection(name)
 
 
 @masquerade_class('motor.motor_asyncio.AsyncIOMotorClient')
 class AsyncMongoMockClient():
+    ASYNC_METHODS = [
+        'drop_database',
+        'list_database_names',
+        'list_databases',
+        'server_info',
+    ]
+
     def __init__(self, *args, mock_build_info=None, **kwargs):
         self.__client = MongoClient(*args, **kwargs)
-        self.__databases = {}
         self.__build_info = mock_build_info
+        apply_async_wrappers(self, self.ASYNC_METHODS, self.__client)
+
+    def get_database(self, *args, **kwargs):
+        return AsyncMongoMockDatabase(
+            self.__client.get_database(*args, **kwargs),
+            mock_build_info=self.__build_info,
+        )
 
     def __getitem__(self, name):
-        return getattr(self, name)
+        return self.get_database(name)
 
     def __getattr__(self, name):
-        if name not in self.__databases:
-            self.__databases[name] = AsyncMongoMockDatabase(
-                self.__client[name],
-                mock_build_info=self.__build_info,
-            )
-        return self.__databases[name]
+        if name in dir(self.__client):
+            return getattr(self.__client, name)
+
+        return self.get_database(name)
```

### Comparing `mongomock_motor-0.0.8/mongomock_motor/patches.py` & `mongomock_motor-0.0.9/mongomock_motor/patches.py`

 * *Files identical despite different names*

### Comparing `mongomock_motor-0.0.8/mongomock_motor.egg-info/PKG-INFO` & `mongomock_motor-0.0.9/mongomock_motor.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: mongomock-motor
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for mocking AsyncIOMotorClient built on top of mongomock.
 Home-page: https://github.com/michaelkryukov/mongomock_motor
 Author: Michael Krukov
 Author-email: krukov.michael@ya.ru
-License: UNKNOWN
 Keywords: library,mongodb
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -35,9 +33,7 @@
     assert await collection.find({}).to_list(None) == []
 
     result = await collection.insert_one({'a': 1})
     assert result.inserted_id
 
     assert len(await collection.find({}).to_list(None)) == 1
 ```
-
-
```

### Comparing `mongomock_motor-0.0.8/setup.py` & `mongomock_motor-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :copyright: (c) 2021 by Michael Krukov
 :license: MIT, see LICENSE for more details.
 """
 
 import setuptools
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```

### Comparing `mongomock_motor-0.0.8/tests/test_async_cursor.py` & `mongomock_motor-0.0.9/tests/test_async_cursor.py`

 * *Files identical despite different names*

### Comparing `mongomock_motor-0.0.8/tests/test_beanie.py` & `mongomock_motor-0.0.9/tests/test_beanie.py`

 * *Files identical despite different names*

### Comparing `mongomock_motor-0.0.8/tests/test_umongo.py` & `mongomock_motor-0.0.9/tests/test_umongo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pymongo.errors import DuplicateKeyError
 from marshmallow.exceptions import ValidationError
 from umongo import Document, fields
 from umongo.instance import Instance
 import pytest
 from mongomock_motor import AsyncMongoMockClient
 
 
@@ -10,18 +9,18 @@
 async def test_umongo():
     instance = Instance.from_db(AsyncMongoMockClient()['tests'])
 
     @instance.register
     class Something(Document):
         field1 = fields.StrField(required=True, unique=True)
         field2 = fields.StrField()
-        related = fields.ListField(fields.ReferenceField("Something"))
+        related = fields.ListField(fields.ReferenceField('Something'))
 
         class Meta:
-            collection_name = "something"
+            collection_name = 'something'
 
     await Something.ensure_indexes()
 
     something1 = Something(field1='A', field2=':)', related=[])
     await something1.commit()
 
     with pytest.raises(ValidationError, match="^{'field1': 'Field value must be unique.'}$"):
```

### Comparing `mongomock_motor-0.0.8/tests/test_unique.py` & `mongomock_motor-0.0.9/tests/test_unique.py`

 * *Files identical despite different names*

### Comparing `mongomock_motor-0.0.8/tests/test_workflow.py` & `mongomock_motor-0.0.9/tests/test_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import bson
 import pytest
 from datetime import datetime, timezone
+from pymongo import ReplaceOne
 from mongomock_motor import AsyncMongoMockClient
 
 
 @pytest.mark.anyio
 async def test_workflow():
     collection = AsyncMongoMockClient()['tests']['test']
 
@@ -23,31 +24,43 @@
 
     docs = await collection.find({'a': 3}).to_list(None)
     assert len(docs) == 1
     assert docs[0]['_id'] == doc_id
     assert docs[0]['a'] == 3
     assert docs[0]['b'] == 1
 
-    pipeline = [{"$match": {"a": 3}}]
+    pipeline = [{'$match': {'a': 3}}]
     docs = await collection.aggregate(pipeline).to_list(None)
     assert len(docs) == 1
     assert docs[0]['_id'] == doc_id
     assert docs[0]['a'] == 3
     assert docs[0]['b'] == 1
 
 
 @pytest.mark.anyio
 async def test_tz_awareness():
     tz_aware_date = datetime(2022, 4, 26, tzinfo=timezone.utc)
-    
+
     # Naive
     collection = AsyncMongoMockClient()['tests']['test']
     await collection.insert_one({'d': tz_aware_date})
     result = await collection.find_one()
-    assert result["d"].tzinfo is None
+    assert result['d'].tzinfo is None
 
     # Aware
     collection = AsyncMongoMockClient(tz_aware=True)['tests']['test']
     await collection.insert_one({'d': tz_aware_date})
     result = await collection.find_one()
-    assert result["d"].tzinfo.__class__ is bson.tz_util.FixedOffset
+    assert result['d'].tzinfo.__class__ is bson.tz_util.FixedOffset
+
 
+@pytest.mark.anyio
+async def test_bulk_write():
+    collection = AsyncMongoMockClient()['tests']['test']
+    result = await collection.bulk_write([
+        ReplaceOne(
+            filter={'_id': 1},
+            replacement={'_id': 1},
+            upsert=True
+        )
+    ])
+    assert result.bulk_api_result['nUpserted'] == 1
```

