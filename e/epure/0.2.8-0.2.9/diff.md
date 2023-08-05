# Comparing `tmp/epure-0.2.8.tar.gz` & `tmp/epure-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epure-0.2.8.tar", max compression
+gzip compressed data, was "epure-0.2.9.tar", max compression
```

## Comparing `epure-0.2.8.tar` & `epure-0.2.9.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0      127 2023-03-14 20:09:06.468541 epure-0.2.8/epure/__init__.py
--rw-r--r--   0        0        0     9073 2023-03-17 16:17:48.659990 epure-0.2.8/epure/epure.py
--rw-r--r--   0        0        0     1142 2022-08-31 19:03:53.723614 epure-0.2.8/epure/errors.py
--rw-r--r--   0        0        0        0 2022-06-28 12:09:28.349607 epure-0.2.8/epure/helpers/__init__.py
--rw-r--r--   0        0        0       90 2022-08-21 12:32:23.299046 epure-0.2.8/epure/helpers/dict_helper.py
--rw-r--r--   0        0        0     1378 2022-08-21 12:34:27.443772 epure-0.2.8/epure/helpers/string_helper.py
--rw-r--r--   0        0        0     1155 2022-07-06 16:52:49.911311 epure-0.2.8/epure/helpers/type_helper.py
--rw-r--r--   0        0        0     1298 2023-03-22 18:49:50.685733 epure-0.2.8/epure/named.py
--rw-r--r--   0        0        0        0 2022-08-04 10:31:26.416932 epure-0.2.8/epure/parser/__init__.py
--rw-r--r--   0        0        0     4632 2022-08-29 19:09:59.755549 epure-0.2.8/epure/parser/bin_operation.py
--rw-r--r--   0        0        0     4809 2022-08-30 11:03:23.905101 epure-0.2.8/epure/parser/binary.py
--rw-r--r--   0        0        0     5546 2022-12-08 16:10:08.964083 epure-0.2.8/epure/parser/leaf.py
--rw-r--r--   0        0        0     7599 2022-08-30 12:00:18.088852 epure-0.2.8/epure/parser/term.py
--rw-r--r--   0        0        0     3398 2022-08-17 16:04:12.439497 epure-0.2.8/epure/parser/term_debugger.py
--rw-r--r--   0        0        0     5669 2022-08-30 16:05:08.013160 epure-0.2.8/epure/parser/term_parser.py
--rw-r--r--   0        0        0       44 2023-03-14 20:09:06.471404 epure-0.2.8/epure/resource/__init__.py
--rw-r--r--   0        0        0        0 2022-06-27 17:03:34.063241 epure-0.2.8/epure/resource/db/__init__.py
--rw-r--r--   0        0        0     3336 2022-07-12 21:05:52.476583 epure-0.2.8/epure/resource/db/constraint.py
--rw-r--r--   0        0        0     3996 2023-03-22 18:49:50.685819 epure-0.2.8/epure/resource/db/db.py
--rw-r--r--   0        0        0      863 2023-03-22 18:49:50.686852 epure-0.2.8/epure/resource/db/db_entity.py
--rw-r--r--   0        0        0     1901 2023-03-09 18:59:58.739323 epure-0.2.8/epure/resource/db/db_entity_resource.py
--rw-r--r--   0        0        0     2289 2022-08-20 13:34:35.871078 epure-0.2.8/epure/resource/db/pseudo_table.py
--rw-r--r--   0        0        0     5658 2022-08-23 16:16:42.813631 epure-0.2.8/epure/resource/db/query_old.py
--rw-r--r--   0        0        0     2786 2022-08-20 13:33:33.942474 epure-0.2.8/epure/resource/db/select_query.py
--rw-r--r--   0        0        0    12367 2023-03-22 17:31:09.776493 epure-0.2.8/epure/resource/db/table.py
--rw-r--r--   0        0        0     1152 2023-03-22 18:49:50.687362 epure-0.2.8/epure/resource/db/table_column.py
--rw-r--r--   0        0        0    10820 2022-12-26 13:56:31.189855 epure-0.2.8/epure/resource/db/table_header.py
--rw-r--r--   0        0        0     6415 2023-03-22 18:49:50.688063 epure-0.2.8/epure/resource/db/table_storage.py
--rw-r--r--   0        0        0     4300 2022-08-30 13:13:39.030768 epure-0.2.8/epure/resource/db/term.py
--rw-r--r--   0        0        0        0 2022-06-27 17:03:34.063241 epure-0.2.8/epure/resource/file/__init__.py
--rw-r--r--   0        0        0      250 2022-06-27 20:51:27.249400 epure-0.2.8/epure/resource/file/file_storage.py
--rw-r--r--   0        0        0     1196 2022-06-29 17:52:26.917194 epure-0.2.8/epure/resource/file/ini_file.py
--rw-r--r--   0        0        0     2018 2022-07-04 09:46:52.543521 epure-0.2.8/epure/resource/file/ini_section.py
--rw-r--r--   0        0        0      440 2022-08-31 14:27:18.622070 epure-0.2.8/epure/resource/file/json_file.py
--rw-r--r--   0        0        0        0 2023-03-14 20:09:06.473626 epure-0.2.8/epure/resource/gres/__init__.py
--rw-r--r--   0        0        0    11298 2023-03-22 18:49:50.688063 epure-0.2.8/epure/resource/gres/gres_db.py
--rw-r--r--   0        0        0      131 2023-03-22 18:49:50.688865 epure-0.2.8/epure/resource/gres/gres_entity.py
--rw-r--r--   0        0        0     3142 2022-07-30 14:05:34.408470 epure-0.2.8/epure/resource/gres/gres_header.py
--rw-r--r--   0        0        0     4109 2022-08-30 17:47:42.514071 epure-0.2.8/epure/resource/gres/gres_table.py
--rw-r--r--   0        0        0     1047 2022-08-04 11:26:14.405214 epure-0.2.8/epure/resource/gres/jsonb_table.py
--rw-r--r--   0        0        0       53 2022-07-08 11:19:47.780813 epure-0.2.8/epure/resource/lite_db/lite_db.py
--rw-r--r--   0        0        0       65 2022-07-08 11:19:43.337675 epure-0.2.8/epure/resource/lite_db/lite_table.py
--rw-r--r--   0        0        0        0 2022-06-27 17:22:02.669404 epure-0.2.8/epure/resource/node/__init__.py
--rw-r--r--   0        0        0     2217 2023-03-22 18:49:50.689175 epure-0.2.8/epure/resource/node/node.py
--rw-r--r--   0        0        0     2784 2022-08-30 15:47:47.528468 epure-0.2.8/epure/resource/node/proto.py
--rw-r--r--   0        0        0      693 2022-08-28 20:52:52.931764 epure-0.2.8/epure/resource/node_promise.py
--rw-r--r--   0        0        0     1758 2023-03-22 18:49:50.689175 epure-0.2.8/epure/resource/resource.py
--rw-r--r--   0        0        0     1484 2023-03-22 18:49:50.689897 epure-0.2.8/epure/resource/savable.py
--rw-r--r--   0        0        0      961 2023-03-22 18:51:02.689885 epure-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2906 2023-03-16 20:51:09.929086 epure-0.2.8/README.md
--rw-r--r--   0        0        0     3763 2023-03-22 18:52:26.028120 epure-0.2.8/setup.py
--rw-r--r--   0        0        0     3509 2023-03-22 18:52:26.028951 epure-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       88 2023-03-23 21:31:00.602482 epure-0.2.9/epure/__init__.py
+-rw-r--r--   0        0        0       41 2023-03-23 21:18:47.453712 epure-0.2.9/epure/dbs.py
+-rw-r--r--   0        0        0     9012 2023-03-23 21:27:24.407599 epure-0.2.9/epure/epure.py
+-rw-r--r--   0        0        0     1142 2022-08-31 19:03:53.723614 epure-0.2.9/epure/errors.py
+-rw-r--r--   0        0        0       90 2023-03-23 21:08:03.110255 epure-0.2.9/epure/files.py
+-rw-r--r--   0        0        0        0 2022-06-28 12:09:28.349607 epure-0.2.9/epure/helpers/__init__.py
+-rw-r--r--   0        0        0       90 2022-08-21 12:32:23.299046 epure-0.2.9/epure/helpers/dict_helper.py
+-rw-r--r--   0        0        0     1378 2022-08-21 12:34:27.443772 epure-0.2.9/epure/helpers/string_helper.py
+-rw-r--r--   0        0        0     1155 2022-07-06 16:52:49.911311 epure-0.2.9/epure/helpers/type_helper.py
+-rw-r--r--   0        0        0     1298 2023-03-22 18:49:50.685733 epure-0.2.9/epure/named.py
+-rw-r--r--   0        0        0        0 2022-08-04 10:31:26.416932 epure-0.2.9/epure/parser/__init__.py
+-rw-r--r--   0        0        0     4632 2022-08-29 19:09:59.755549 epure-0.2.9/epure/parser/bin_operation.py
+-rw-r--r--   0        0        0     4809 2022-08-30 11:03:23.905101 epure-0.2.9/epure/parser/binary.py
+-rw-r--r--   0        0        0     5546 2022-12-08 16:10:08.964083 epure-0.2.9/epure/parser/leaf.py
+-rw-r--r--   0        0        0     7599 2022-08-30 12:00:18.088852 epure-0.2.9/epure/parser/term.py
+-rw-r--r--   0        0        0     3398 2022-08-17 16:04:12.439497 epure-0.2.9/epure/parser/term_debugger.py
+-rw-r--r--   0        0        0     5669 2022-08-30 16:05:08.013160 epure-0.2.9/epure/parser/term_parser.py
+-rw-r--r--   0        0        0       44 2023-03-14 20:09:06.471404 epure-0.2.9/epure/resource/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-27 17:03:34.063241 epure-0.2.9/epure/resource/db/__init__.py
+-rw-r--r--   0        0        0     3336 2022-07-12 21:05:52.476583 epure-0.2.9/epure/resource/db/constraint.py
+-rw-r--r--   0        0        0     3996 2023-03-22 18:49:50.685819 epure-0.2.9/epure/resource/db/db.py
+-rw-r--r--   0        0        0      863 2023-03-22 18:49:50.686852 epure-0.2.9/epure/resource/db/db_entity.py
+-rw-r--r--   0        0        0     1901 2023-03-09 18:59:58.739323 epure-0.2.9/epure/resource/db/db_entity_resource.py
+-rw-r--r--   0        0        0     2289 2022-08-20 13:34:35.871078 epure-0.2.9/epure/resource/db/pseudo_table.py
+-rw-r--r--   0        0        0     5658 2022-08-23 16:16:42.813631 epure-0.2.9/epure/resource/db/query_old.py
+-rw-r--r--   0        0        0     2786 2022-08-20 13:33:33.942474 epure-0.2.9/epure/resource/db/select_query.py
+-rw-r--r--   0        0        0    12367 2023-03-22 17:31:09.776493 epure-0.2.9/epure/resource/db/table.py
+-rw-r--r--   0        0        0     1152 2023-03-22 18:49:50.687362 epure-0.2.9/epure/resource/db/table_column.py
+-rw-r--r--   0        0        0    10820 2022-12-26 13:56:31.189855 epure-0.2.9/epure/resource/db/table_header.py
+-rw-r--r--   0        0        0     6479 2023-03-23 21:26:58.245401 epure-0.2.9/epure/resource/db/table_storage.py
+-rw-r--r--   0        0        0     4300 2022-08-30 13:13:39.030768 epure-0.2.9/epure/resource/db/term.py
+-rw-r--r--   0        0        0        0 2022-06-27 17:03:34.063241 epure-0.2.9/epure/resource/file/__init__.py
+-rw-r--r--   0        0        0      250 2022-06-27 20:51:27.249400 epure-0.2.9/epure/resource/file/file_storage.py
+-rw-r--r--   0        0        0     1196 2022-06-29 17:52:26.917194 epure-0.2.9/epure/resource/file/ini_file.py
+-rw-r--r--   0        0        0     2018 2022-07-04 09:46:52.543521 epure-0.2.9/epure/resource/file/ini_section.py
+-rw-r--r--   0        0        0      440 2022-08-31 14:27:18.622070 epure-0.2.9/epure/resource/file/json_file.py
+-rw-r--r--   0        0        0        0 2023-03-14 20:09:06.473626 epure-0.2.9/epure/resource/gres/__init__.py
+-rw-r--r--   0        0        0    11298 2023-03-22 18:49:50.688063 epure-0.2.9/epure/resource/gres/gres_db.py
+-rw-r--r--   0        0        0      131 2023-03-22 18:49:50.688865 epure-0.2.9/epure/resource/gres/gres_entity.py
+-rw-r--r--   0        0        0     3142 2022-07-30 14:05:34.408470 epure-0.2.9/epure/resource/gres/gres_header.py
+-rw-r--r--   0        0        0     4109 2022-08-30 17:47:42.514071 epure-0.2.9/epure/resource/gres/gres_table.py
+-rw-r--r--   0        0        0     1047 2022-08-04 11:26:14.405214 epure-0.2.9/epure/resource/gres/jsonb_table.py
+-rw-r--r--   0        0        0       53 2022-07-08 11:19:47.780813 epure-0.2.9/epure/resource/lite_db/lite_db.py
+-rw-r--r--   0        0        0       65 2022-07-08 11:19:43.337675 epure-0.2.9/epure/resource/lite_db/lite_table.py
+-rw-r--r--   0        0        0        0 2022-06-27 17:22:02.669404 epure-0.2.9/epure/resource/node/__init__.py
+-rw-r--r--   0        0        0     2217 2023-03-22 18:49:50.689175 epure-0.2.9/epure/resource/node/node.py
+-rw-r--r--   0        0        0     2784 2022-08-30 15:47:47.528468 epure-0.2.9/epure/resource/node/proto.py
+-rw-r--r--   0        0        0      693 2022-08-28 20:52:52.931764 epure-0.2.9/epure/resource/node_promise.py
+-rw-r--r--   0        0        0     1758 2023-03-22 18:49:50.689175 epure-0.2.9/epure/resource/resource.py
+-rw-r--r--   0        0        0     1484 2023-03-22 18:49:50.689897 epure-0.2.9/epure/resource/savable.py
+-rw-r--r--   0        0        0      961 2023-03-23 21:36:35.276722 epure-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2908 2023-03-23 21:33:02.005511 epure-0.2.9/README.md
+-rw-r--r--   0        0        0     3765 2023-03-23 21:37:32.255240 epure-0.2.9/setup.py
+-rw-r--r--   0        0        0     3511 2023-03-23 21:37:32.255240 epure-0.2.9/PKG-INFO
```

### Comparing `epure-0.2.8/epure/epure.py` & `epure-0.2.9/epure/epure.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from .resource.db.db_entity import DbEntity
 import functools
 from .parser.term import Term
 from .resource.node.proto import Proto
 from inspect import signature
 
 
-def connect(edb:TableStorage) -> None:
-    Epure.EDb = edb
 
 class Epure(type, Savable):
     
     EDb:TableStorage
     epures:List[Epure] = []
     # annotations:Dict[str,Any]
     resource:Savable
```

### Comparing `epure-0.2.8/epure/errors.py` & `epure-0.2.9/epure/errors.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/helpers/string_helper.py` & `epure-0.2.9/epure/helpers/string_helper.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/helpers/type_helper.py` & `epure-0.2.9/epure/helpers/type_helper.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/named.py` & `epure-0.2.9/epure/named.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/bin_operation.py` & `epure-0.2.9/epure/parser/bin_operation.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/binary.py` & `epure-0.2.9/epure/parser/binary.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/leaf.py` & `epure-0.2.9/epure/parser/leaf.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/term.py` & `epure-0.2.9/epure/parser/term.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/term_debugger.py` & `epure-0.2.9/epure/parser/term_debugger.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/parser/term_parser.py` & `epure-0.2.9/epure/parser/term_parser.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/constraint.py` & `epure-0.2.9/epure/resource/db/constraint.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/db.py` & `epure-0.2.9/epure/resource/db/db.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/db_entity.py` & `epure-0.2.9/epure/resource/db/db_entity.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/db_entity_resource.py` & `epure-0.2.9/epure/resource/db/db_entity_resource.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/pseudo_table.py` & `epure-0.2.9/epure/resource/db/pseudo_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/query_old.py` & `epure-0.2.9/epure/resource/db/query_old.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/select_query.py` & `epure-0.2.9/epure/resource/db/select_query.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/table.py` & `epure-0.2.9/epure/resource/db/table.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/table_column.py` & `epure-0.2.9/epure/resource/db/table_column.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/table_header.py` & `epure-0.2.9/epure/resource/db/table_header.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/db/table_storage.py` & `epure-0.2.9/epure/resource/db/table_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
     def __contains__(self, table_name:str) -> bool:
         full_name = self._get_full_table_name(table_name)
         if full_name.full_name in self.tables:
             return True
         table = self.read(table_name)
         return bool(table)
+    
+    def connect(self) -> None:
+        Epure.EDb = self
         
     def create_namespace(self, namespace):
         script = self.serialize_namespace_for_create(namespace)
         script = str(script)
         self.execute(script)
 
         self._set_namespace(namespace)
```

### Comparing `epure-0.2.8/epure/resource/db/term.py` & `epure-0.2.9/epure/resource/db/term.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/file/ini_file.py` & `epure-0.2.9/epure/resource/file/ini_file.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/file/ini_section.py` & `epure-0.2.9/epure/resource/file/ini_section.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/gres/gres_db.py` & `epure-0.2.9/epure/resource/gres/gres_db.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/gres/gres_header.py` & `epure-0.2.9/epure/resource/gres/gres_header.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/gres/gres_table.py` & `epure-0.2.9/epure/resource/gres/gres_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/gres/jsonb_table.py` & `epure-0.2.9/epure/resource/gres/jsonb_table.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/node/node.py` & `epure-0.2.9/epure/resource/node/node.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/node/proto.py` & `epure-0.2.9/epure/resource/node/proto.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/node_promise.py` & `epure-0.2.9/epure/resource/node_promise.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/resource.py` & `epure-0.2.9/epure/resource/resource.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/epure/resource/savable.py` & `epure-0.2.9/epure/resource/savable.py`

 * *Files identical despite different names*

### Comparing `epure-0.2.8/pyproject.toml` & `epure-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epure"
-version = "0.2.8"
+version = "0.2.9"
 description = "purest architecture"
 authors = ["Nikita Umarov <nagvalhm@yandex.ru>", "Pavel Pichugin"]
 license = "MIT"
 readme = "README.md"
 packages = [
     # { include = "pypi_stub" },
     { include = "epure" }
```

### Comparing `epure-0.2.8/README.md` & `epure-0.2.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -31,27 +31,27 @@
     # import connection functions from Epure
     from epure import GresDb
     from epure import connect
 
     # First way to connect database to epure
 
     # Format of string to connect ('database://user:password@host:port')
-    connect(GresDb('postgres://postgres:postgres@localhost:5432',
-    log_level=3))
+    GresDb('postgres://postgres:postgres@localhost:5432',
+    log_level=3).connect()
 
     # Alternative way of connection
 
     db = GresDb('postgres://postgres:postgres@localhost:32', 
     # host="localhost", 
     port="5432", 
     # database="postgres", 
     # user="postgres", 
     password="postgres",
     log_level=3)
-    connect(db)
+    db.connect()
 
     # log_level defines level of description of opertaions with DB in auto-generated file epure_db.log
 
 ```
 
 
 A Simple Example
```

#### html2text {}

```diff
@@ -2,19 +2,19 @@
 idea about database, table and columns. All technical details hidden from you.
 Care only about your business logic. Installing ---------- Install and update
 using `pip`: ``` $ pip install -U epure ``` Install and update using `poetry`:
 ``` $ poetry add epure ``` Connecting Epure to database ---------- Create
 example class with Epure, create instance of it and read it from DB. ```python
 # import connection functions from Epure from epure import GresDb from epure
 import connect # First way to connect database to epure # Format of string to
-connect ('database://user:password@host:port') connect(GresDb('postgres://
-postgres:postgres@localhost:5432', log_level=3)) # Alternative way of
+connect ('database://user:password@host:port') GresDb('postgres://postgres:
+postgres@localhost:5432', log_level=3).connect() # Alternative way of
 connection db = GresDb('postgres://postgres:postgres@localhost:32', #
 host="localhost", port="5432", # database="postgres", # user="postgres",
-password="postgres", log_level=3) connect(db) # log_level defines level of
+password="postgres", log_level=3) db.connect() # log_level defines level of
 description of opertaions with DB in auto-generated file epure_db.log ``` A
 Simple Example ---------------- ```python # save this as epure_example.py from
 epure import epure # different types hints avalible import types # In order to
 save attributes of class to db, type hints is required! # decorate class by
 @epure() wrap function @epure() class Example: int_attr:int bool_attr:bool
 str_attr:str complex_attr:complex list_attr:list dict_attr:Dict[int, str]
 str_attr_with_default_val:str = 'example_str' epure_cls_attr:SomeEpureCls
```

### Comparing `epure-0.2.8/setup.py` & `epure-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 ['inflection>=0.5.1,<0.6.0',
  'jsonpickle>=2.2.0,<3.0.0',
  'psycopg2==2.9.3',
  'twine>=4.0.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'epure',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'purest architecture',
-    'long_description': 'Epure\n=====\n\n<a href="https://github.com/nagvalhm/epure">Epure</a> is agnostic ORM - you can store and retrieve data having no idea about database, table and columns. \nAll technical details hidden from you. Care only about your business logic.\n\n\nInstalling\n----------\n\nInstall and update using <a href="https://pip.pypa.io/en/stable/getting-started/">`pip`</a>:\n\n```\n    $ pip install -U epure\n```\n\nInstall and update using <a href="https://python-poetry.org/docs/">`poetry`</a>:\n\n```\n    $ poetry add epure\n```\n\n\nConnecting Epure to database\n----------\n\nCreate example class with Epure, create instance of it and read it from DB.\n\n```python\n\n    # import connection functions from Epure\n    from epure import GresDb\n    from epure import connect\n\n    # First way to connect database to epure\n\n    # Format of string to connect (\'database://user:password@host:port\')\n    connect(GresDb(\'postgres://postgres:postgres@localhost:5432\',\n    log_level=3))\n\n    # Alternative way of connection\n\n    db = GresDb(\'postgres://postgres:postgres@localhost:32\', \n    # host="localhost", \n    port="5432", \n    # database="postgres", \n    # user="postgres", \n    password="postgres",\n    log_level=3)\n    connect(db)\n\n    # log_level defines level of description of opertaions with DB in auto-generated file epure_db.log\n\n```\n\n\nA Simple Example\n----------------\n\n```python\n\n    # save this as epure_example.py\n    from epure import epure\n\n    # different types hints avalible\n    import types\n\n    # In order to save attributes of class to db, type hints is required!\n\n    # decorate class by @epure() wrap function\n    @epure()\n    class Example:\n\n        int_attr:int\n        bool_attr:bool\n        str_attr:str\n        complex_attr:complex\n        list_attr:list\n        dict_attr:Dict[int, str]\n        str_attr_with_default_val:str = \'example_str\'\n        epure_cls_attr:SomeEpureCls\n        NoneType_attr:types.NoneType\n\n    # creating instance of epurized Example class\n    obj = Example()\n    \n    # assigning vals to instance\n    obj.int_attr = 1\n    obj.str_attr = "example"\n    obj.list_attr = [1,2,3,4]\n\n    #saving obj instance to database\n    obj.save()\n\n    # saved instance has attribute of node_id that is unique\n    node_id = epure.node_id \n    \n    # node_id is used to search epure objects and retrive them from DB via read() method\n    res = epure.table.read(node_id=node_id)\n\n```\n\nDevelopers\n-----\nNikita Umarov (Pichugin), \nPavel Pichugin\n\n\nLinks\n-----\n\n-   Documentation: https://github.com/nagvalhm/epure/blob/main/README.md\n-   Changes: https://github.com/nagvalhm/epure\n-   PyPI Releases: https://pypi.org/project/epure/\n-   Source Code: https://github.com/nagvalhm/epure\n-   Issue Tracker: https://github.com/nagvalhm/epure/issues\n-   Website: https://pypi.org/project/epure/',
+    'long_description': 'Epure\n=====\n\n<a href="https://github.com/nagvalhm/epure">Epure</a> is agnostic ORM - you can store and retrieve data having no idea about database, table and columns. \nAll technical details hidden from you. Care only about your business logic.\n\n\nInstalling\n----------\n\nInstall and update using <a href="https://pip.pypa.io/en/stable/getting-started/">`pip`</a>:\n\n```\n    $ pip install -U epure\n```\n\nInstall and update using <a href="https://python-poetry.org/docs/">`poetry`</a>:\n\n```\n    $ poetry add epure\n```\n\n\nConnecting Epure to database\n----------\n\nCreate example class with Epure, create instance of it and read it from DB.\n\n```python\n\n    # import connection functions from Epure\n    from epure import GresDb\n    from epure import connect\n\n    # First way to connect database to epure\n\n    # Format of string to connect (\'database://user:password@host:port\')\n    GresDb(\'postgres://postgres:postgres@localhost:5432\',\n    log_level=3).connect()\n\n    # Alternative way of connection\n\n    db = GresDb(\'postgres://postgres:postgres@localhost:32\', \n    # host="localhost", \n    port="5432", \n    # database="postgres", \n    # user="postgres", \n    password="postgres",\n    log_level=3)\n    db.connect()\n\n    # log_level defines level of description of opertaions with DB in auto-generated file epure_db.log\n\n```\n\n\nA Simple Example\n----------------\n\n```python\n\n    # save this as epure_example.py\n    from epure import epure\n\n    # different types hints avalible\n    import types\n\n    # In order to save attributes of class to db, type hints is required!\n\n    # decorate class by @epure() wrap function\n    @epure()\n    class Example:\n\n        int_attr:int\n        bool_attr:bool\n        str_attr:str\n        complex_attr:complex\n        list_attr:list\n        dict_attr:Dict[int, str]\n        str_attr_with_default_val:str = \'example_str\'\n        epure_cls_attr:SomeEpureCls\n        NoneType_attr:types.NoneType\n\n    # creating instance of epurized Example class\n    obj = Example()\n    \n    # assigning vals to instance\n    obj.int_attr = 1\n    obj.str_attr = "example"\n    obj.list_attr = [1,2,3,4]\n\n    #saving obj instance to database\n    obj.save()\n\n    # saved instance has attribute of node_id that is unique\n    node_id = epure.node_id \n    \n    # node_id is used to search epure objects and retrive them from DB via read() method\n    res = epure.table.read(node_id=node_id)\n\n```\n\nDevelopers\n-----\nNikita Umarov (Pichugin), \nPavel Pichugin\n\n\nLinks\n-----\n\n-   Documentation: https://github.com/nagvalhm/epure/blob/main/README.md\n-   Changes: https://github.com/nagvalhm/epure\n-   PyPI Releases: https://pypi.org/project/epure/\n-   Source Code: https://github.com/nagvalhm/epure\n-   Issue Tracker: https://github.com/nagvalhm/epure/issues\n-   Website: https://pypi.org/project/epure/',
     'author': 'Nikita Umarov',
     'author_email': 'nagvalhm@yandex.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['epure',
 'epure.helpers', 'epure.parser', 'epure.resource', 'epure.resource.db',
 'epure.resource.file', 'epure.resource.gres', 'epure.resource.lite_db',
 'epure.resource.node'] package_data = \ {'': ['*']} install_requires = \
 ['inflection>=0.5.1,<0.6.0', 'jsonpickle>=2.2.0,<3.0.0', 'psycopg2==2.9.3',
-'twine>=4.0.2,<5.0.0'] setup_kwargs = { 'name': 'epure', 'version': '0.2.8',
+'twine>=4.0.2,<5.0.0'] setup_kwargs = { 'name': 'epure', 'version': '0.2.9',
 'description': 'purest architecture', 'long_description':
 'Epure\n=====\n\nEpure is agnostic ORM - you can store and retrieve data having
 no idea about database, table and columns. \nAll technical details hidden from
 you. Care only about your business logic.\n\n\nInstalling\n----------
 \n\nInstall and update using `pip`:\n\n```\n $ pip install -
 U epure\n```\n\nInstall and update using `poetry`:\n\n```\n $ poetry add
 epure\n```\n\n\nConnecting Epure to database\n----------\n\nCreate example
 class with Epure, create instance of it and read it from DB.\n\n```python\n\n #
 import connection functions from Epure\n from epure import GresDb\n from epure
 import connect\n\n # First way to connect database to epure\n\n # Format of
-string to connect (\'database://user:password@host:port\')\n connect(GresDb
-(\'postgres://postgres:postgres@localhost:5432\',\n log_level=3))\n\n #
+string to connect (\'database://user:password@host:port\')\n GresDb(\'postgres:
+//postgres:postgres@localhost:5432\',\n log_level=3).connect()\n\n #
 Alternative way of connection\n\n db = GresDb(\'postgres://postgres:
 postgres@localhost:32\', \n # host="localhost", \n port="5432", \n #
 database="postgres", \n # user="postgres", \n password="postgres",\n
-log_level=3)\n connect(db)\n\n # log_level defines level of description of
+log_level=3)\n db.connect()\n\n # log_level defines level of description of
 opertaions with DB in auto-generated file epure_db.log\n\n```\n\n\nA Simple
 Example\n----------------\n\n```python\n\n # save this as epure_example.py\n
 from epure import epure\n\n # different types hints avalible\n import types\n\n
 # In order to save attributes of class to db, type hints is required!\n\n #
 decorate class by @epure() wrap function\n @epure()\n class Example:\n\n
 int_attr:int\n bool_attr:bool\n str_attr:str\n complex_attr:complex\n
 list_attr:list\n dict_attr:Dict[int, str]\n str_attr_with_default_val:str =
```

### Comparing `epure-0.2.8/PKG-INFO` & `epure-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epure
-Version: 0.2.8
+Version: 0.2.9
 Summary: purest architecture
 License: MIT
 Author: Nikita Umarov
 Author-email: nagvalhm@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -51,27 +51,27 @@
     # import connection functions from Epure
     from epure import GresDb
     from epure import connect
 
     # First way to connect database to epure
 
     # Format of string to connect ('database://user:password@host:port')
-    connect(GresDb('postgres://postgres:postgres@localhost:5432',
-    log_level=3))
+    GresDb('postgres://postgres:postgres@localhost:5432',
+    log_level=3).connect()
 
     # Alternative way of connection
 
     db = GresDb('postgres://postgres:postgres@localhost:32', 
     # host="localhost", 
     port="5432", 
     # database="postgres", 
     # user="postgres", 
     password="postgres",
     log_level=3)
-    connect(db)
+    db.connect()
 
     # log_level defines level of description of opertaions with DB in auto-generated file epure_db.log
 
 ```
 
 
 A Simple Example
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epure Version: 0.2.8 Summary: purest architecture
+Metadata-Version: 2.1 Name: epure Version: 0.2.9 Summary: purest architecture
 License: MIT Author: Nikita Umarov Author-email: nagvalhm@yandex.ru Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: inflection (>=0.5.1,<0.6.0) Requires-
 Dist: jsonpickle (>=2.2.0,<3.0.0) Requires-Dist: psycopg2 (==2.9.3) Requires-
 Dist: twine (>=4.0.2,<5.0.0) Project-URL: Documentation, https://github.com/
 nagvalhm/epure/blob/main/README.md Project-URL: Homepage, https://github.com/
@@ -12,19 +12,19 @@
 All technical details hidden from you. Care only about your business logic.
 Installing ---------- Install and update using `pip`: ``` $ pip install -
 U epure ``` Install and update using `poetry`: ``` $ poetry add epure ```
 Connecting Epure to database ---------- Create example class with Epure, create
 instance of it and read it from DB. ```python # import connection functions
 from Epure from epure import GresDb from epure import connect # First way to
 connect database to epure # Format of string to connect ('database://user:
-password@host:port') connect(GresDb('postgres://postgres:postgres@localhost:
-5432', log_level=3)) # Alternative way of connection db = GresDb('postgres://
+password@host:port') GresDb('postgres://postgres:postgres@localhost:5432',
+log_level=3).connect() # Alternative way of connection db = GresDb('postgres://
 postgres:postgres@localhost:32', # host="localhost", port="5432", #
 database="postgres", # user="postgres", password="postgres", log_level=3)
-connect(db) # log_level defines level of description of opertaions with DB in
+db.connect() # log_level defines level of description of opertaions with DB in
 auto-generated file epure_db.log ``` A Simple Example ---------------
 - ```python # save this as epure_example.py from epure import epure # different
 types hints avalible import types # In order to save attributes of class to db,
 type hints is required! # decorate class by @epure() wrap function @epure()
 class Example: int_attr:int bool_attr:bool str_attr:str complex_attr:complex
 list_attr:list dict_attr:Dict[int, str] str_attr_with_default_val:str =
 'example_str' epure_cls_attr:SomeEpureCls NoneType_attr:types.NoneType #
```

