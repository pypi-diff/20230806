# Comparing `tmp/importer-local-0.0.8.tar.gz` & `tmp/importer-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.8.tar", last modified: Tue Jul 18 10:47:22 2023, max compression
+gzip compressed data, was "importer-local-0.0.9.tar", last modified: Wed Jul 19 09:02:31 2023, max compression
```

## Comparing `importer-local-0.0.8.tar` & `importer-local-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.389577 importer-local-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/CirclesImporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:05.000000 importer-local-0.0.8/CirclesImporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-18 10:47:05.000000 importer-local-0.0.8/CirclesImporter/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 10:47:22.389577 importer-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 10:47:05.000000 importer-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 10:47:22.000000 importer-local-0.0.8/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:47:22.389577 importer-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 10:47:05.000000 importer-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:47:22.385576 importer-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-18 10:47:05.000000 importer-local-0.0.8/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:31.618174 importer-local-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:31.618174 importer-local-0.0.9/CirclesImporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:11.000000 importer-local-0.0.9/CirclesImporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-19 09:02:11.000000 importer-local-0.0.9/CirclesImporter/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-19 09:02:31.618174 importer-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-19 09:02:11.000000 importer-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:31.618174 importer-local-0.0.9/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-19 09:02:31.000000 importer-local-0.0.9/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-19 09:02:31.000000 importer-local-0.0.9/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:02:31.000000 importer-local-0.0.9/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 09:02:31.000000 importer-local-0.0.9/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:02:31.618174 importer-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-19 09:02:11.000000 importer-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:02:31.618174 importer-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-19 09:02:11.000000 importer-local-0.0.9/tests/test_importer.py
```

### Comparing `importer-local-0.0.8/CirclesImporter/importer.py` & `importer-local-0.0.9/CirclesImporter/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from circles_local_database_python.database import database
 from CirclesGetCountryName.opencage_get_country_name import Country
 from dotenv import load_dotenv
-from LoggerLocalPythonPackage import LocalLogger
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger as local_logger
 from functools import wraps
 load_dotenv()
 
-Local_Logger=LocalLogger._Local_Logger
+
 def log_function_execution(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
-        Local_Logger.start("Function %s started." % func.__name__)
+        local_logger.start("Function %s started." % func.__name__)
         result = func(*args, **kwargs)  # Execute the function
-        Local_Logger.end("Function %s completed." % func.__name__)
+        local_logger.end("Function %s completed." % func.__name__)
         return result
     return wrapper
 
 
 class Importer:
     def __init__(self, source):
         self.source_name = source
 
     @log_function_execution
     def insert_new_entity(self, entity_type_name):
-        Local_Logger.start("Start Insert Entity %s ." % entity_type_name)
+        local_logger.start("Start Insert Entity %s ." % entity_type_name)
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT entity_type_id FROM {} WHERE entity_type_name = '{}'".format('entity_type.entity_type_ml_table', entity_type_name))
         entity_type_id = cursor.fetchone()
 
@@ -36,23 +36,23 @@
             cursor.execute(query_entity)
             db.commit()
 
             last_inserted_id = cursor.lastrowid
             query_entity_ml = "INSERT INTO {}(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, %s, 1, 1)".format('entity_type.entity_type_ml_table')
             cursor.execute(query_entity_ml, (entity_type_name, last_inserted_id, 'en'))
-            Local_Logger.end("End Inserted Entity %s ." % entity_type_name)
+            local_logger.end("End Inserted Entity %s ." % entity_type_name)
             db.commit()
         else:
-            Local_Logger.end("Entity %s already exist." % entity_type_name)
+            local_logger.end("Entity %s already exist." % entity_type_name)
         db.close()
 
     @log_function_execution
     def insert_new_source(self):
-        Local_Logger.start("Start insert_new_source()")
+        local_logger.start("Start insert_new_source()")
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT source_id FROM {} WHERE source_name = '{}'".format('source.source_ml_table', self.source_name))
         source_id = cursor.fetchone()
 
@@ -63,44 +63,43 @@
             db.commit()
 
             last_inserted_id = cursor.lastrowid
             query_importer_source_ml = "INSERT INTO {}(`source_name`,`source_id`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, 1, 1)".format('source.source_ml_table')
             cursor.execute(query_importer_source_ml, (self.source_name, last_inserted_id))
             db.commit()
-            Local_Logger.end("end insert_new_source %s."%self.source_name)
+            local_logger.end("end insert_new_source %s."%self.source_name)
         else:
-            Local_Logger.end("Source %s already exist." % self.source_name)
+            local_logger.end("Source %s already exist." % self.source_name)
         db.close()
 
     @log_function_execution
     def insert_record_source(self, location, entity_type_name, entity_id, url):
-        Local_Logger.start("Function insert_record_source() started")
+        local_logger.start("Function insert_record_source() started")
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
 
         cursor.execute("SELECT source_id FROM {} WHERE source_name = '{}'".format('source.source_ml_table', self.source_name))
         source_id = cursor.fetchone()
 
-        find_country = Country()
-        country_name = find_country.get_country_name(location)
+        country_name =  Country.get_country_name(location)
         cursor.execute(
             "SELECT id FROM {} WHERE name = '{}'".format('location.country_table', country_name))
         country_id = cursor.fetchone()
 
         cursor.execute("SELECT entity_type_id FROM {} WHERE entity_type_name = '{}'".format('entity_type.entity_type_ml_table', entity_type_name))
         entity_type_id = cursor.fetchone()
 
         query_importer = "INSERT INTO {}(`source_id`,`country_id`,`entity_type_id`,`entity_id`,`url`,`created_user_id`,`updated_user_id`)" \
                           " VALUES (%s, %s, %s, %s, %s, 1, 1)".format('importer.importer_table')
 
         cursor.execute(query_importer, (source_id[0], country_id[0], entity_type_id[0], entity_id, url))
 
         db.commit()
         db.close()
-        Local_Logger.end("Function insert_record_source() ended")
+        local_logger.end("Function insert_record_source() ended")
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `importer-local-0.0.8/README.md` & `importer-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `importer-local-0.0.8/setup.py` & `importer-local-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='importer-local',  
-     version='0.0.8',
+     version='0.0.9',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles <project-name> Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `importer-local-0.0.8/tests/test_importer.py` & `importer-local-0.0.9/tests/test_importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 from unittest.mock import MagicMock, patch
 import sys
 import os
-from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
 # Add the parent directory to the sys.path
 parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 sys.path.append(parent_dir)
 # Import the correct module from the CirclesImporter package
 from CirclesImporter import importer
 
 
@@ -17,15 +16,14 @@
 
     @patch('CirclesImporter.importer.database')
     def test_insert_new_entity(self, database_mock):
         entity_type_name = "TestEntity"
         cursor_mock = MagicMock()
         cursor_mock.fetchone.return_value = None
         cursor_mock.lastrowid = 1
-        _Local_Logger.info(os.getenv("OPENCAGE_KEY"))
         database_mock.return_value.connect_to_database.return_value.cursor.return_value = cursor_mock
         self.importer.database = database_mock
         self.importer.insert_new_entity(entity_type_name)
 
         expected_query_entity = "INSERT INTO entity_type.entity_type_table(`created_user_id`,`updated_user_id`) VALUES (1, 1)"
         expected_query_entity_ml = "INSERT INTO entity_type.entity_type_ml_table(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`) VALUES (%s, %s, %s, 1, 1)"
```

