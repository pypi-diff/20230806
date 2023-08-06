# Comparing `tmp/toolcat-0.0.7.tar.gz` & `tmp/toolcat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolcat-0.0.7.tar", max compression
+gzip compressed data, was "toolcat-0.0.8.tar", max compression
```

## Comparing `toolcat-0.0.7.tar` & `toolcat-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.7/LICENSE
--rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.7/README.md
--rw-r--r--   0        0        0     1085 2023-08-03 06:33:03.693815 toolcat-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.7/src/toolcat/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-03 23:01:48.937333 toolcat-0.0.7/src/toolcat/database.py
--rw-r--r--   0        0        0     1400 2023-06-03 23:01:51.316471 toolcat-0.0.7/src/toolcat/database_test.py
--rw-r--r--   0        0        0      831 2023-07-01 08:42:42.223538 toolcat-0.0.7/src/toolcat/project.py
--rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.7/src/toolcat/projects_test.py
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 toolcat-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-03 18:15:32.691464 toolcat-0.0.8/LICENSE
+-rw-r--r--   0        0        0      182 2023-06-03 20:00:15.609596 toolcat-0.0.8/README.md
+-rw-r--r--   0        0        0     1086 2023-08-06 07:03:17.814155 toolcat-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-03 18:15:32.694245 toolcat-0.0.8/src/toolcat/__init__.py
+-rw-r--r--   0        0        0     2764 2023-08-06 06:53:39.305497 toolcat-0.0.8/src/toolcat/database.py
+-rw-r--r--   0        0        0     2359 2023-08-06 06:59:56.904750 toolcat-0.0.8/src/toolcat/database_test.py
+-rw-r--r--   0        0        0      306 2023-08-06 06:50:05.288824 toolcat-0.0.8/src/toolcat/files.py
+-rw-r--r--   0        0        0      831 2023-07-01 08:42:42.223538 toolcat-0.0.8/src/toolcat/project.py
+-rw-r--r--   0        0        0     1096 2023-06-03 19:12:14.817042 toolcat-0.0.8/src/toolcat/projects_test.py
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 toolcat-0.0.8/PKG-INFO
```

### Comparing `toolcat-0.0.7/LICENSE` & `toolcat-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.7/pyproject.toml` & `toolcat-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.bandit]
 exclude_dirs = ["tests", "features"]
 
 [tool.black]
-max-line-length = 99
+max-line-length = 120
 target-version = ['py310', 'py311']
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "toolcat"
-version = "0.0.7"
+version = "0.0.8"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [{ include = "toolcat", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `toolcat-0.0.7/src/toolcat/database.py` & `toolcat-0.0.8/src/toolcat/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 import os
 import pathlib
 from typing import Optional
 
 from sqlalchemy import create_engine, text
+from sqlalchemy.exc import OperationalError as _OperationalError
 from sqlalchemy.orm import Session as _Session
 from sqlalchemy.orm import sessionmaker
 
-Session = _Session
+
+class OperationalError(Exception):
+    pass
+
+
+class Session(_Session):
+    def execute(self, *args, **kwargs):
+        try:
+            return super().execute(*args, **kwargs)
+        except _OperationalError as e:
+            raise OperationalError(f"execute sql statement: {str(e)}")
 
 
 class Database:
     """
     Creates a database.
 
     The database is created in the path defined by the DATABASE environment
@@ -70,9 +81,10 @@
         Runs the SQL file against the database.
 
         Args:
             sql_file_path (pathlib.Path): Path to the SQL file to execute.
         """
         with open(sql_file_path) as sql_file:
             sql = sql_file.read()
-            self.session.execute(text(sql))
-            self.session.commit()
+            for stmt in sql.split(";"):
+                self.session.execute(text(stmt))
+                self.session.commit()
```

### Comparing `toolcat-0.0.7/src/toolcat/database_test.py` & `toolcat-0.0.8/src/toolcat/database_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
-from toolcat.database import Database, Session, text
+from toolcat.database import Database, OperationalError, Session, text
+from toolcat.files import append
 
 
 class TestDatabase:
     def test_should_raise_a_key_error_when_environment_variable_is_not_defined(self):
         with pytest.raises(KeyError):
             _ = Database()
 
@@ -14,26 +15,52 @@
 
         _ = Database()
 
         assert database.exists()  # nosec
 
     def test_remove_the_database_file_when_remove_is_called(self, tmp_path):
         database_file = tmp_path / "database"
-        sql_file = tmp_path / "sql_file.sql"
-        sql_file.write_text("CREATE TABLE test_table (id INTEGER PRIMARY KEY);")
-        db = Database(database_file, sql_file=sql_file)
+        db = Database(database_file)
 
         db.remove()
 
         database_file = tmp_path / "database.db"
         assert not database_file.exists()  # nosec
 
+
+class TestDatabaseCreateWithSqlFile:
+    def test_raise_custom_error_when_an_error_happens(self, tmp_path):
+        sql_file = tmp_path / "sql_file.sql"
+        sql_file.write_text("")
+
+        database = Database(tmp_path, sql_file=sql_file)
+
+        sql_stmt = "SELECT * FROM test_table;"
+
+        with Session(database.engine) as session:
+            with pytest.raises(OperationalError) as excinfo:
+                session.execute(text(sql_stmt))
+
+        assert "execute sql statement" in excinfo.value.args[0]  # nosec
+
     def test_create_database_given_initial_sql_file(self, tmp_path):
         sql_file = tmp_path / "sql_file.sql"
         sql_file.write_text("CREATE TABLE test_table (id INTEGER PRIMARY KEY);")
 
         database = Database(tmp_path, sql_file=sql_file)
 
         sql_stmt = "SELECT * FROM test_table;"
         with Session(database.engine) as session:
             result = session.execute(text(sql_stmt))
         assert result.fetchall() == []  # nosec
+
+    def test_execute_multiple_sql_statements(self, tmp_path):
+        sql_file = tmp_path / "sql_file.sql"
+        sql_file.write_text("CREATE TABLE test_table (id INTEGER PRIMARY KEY);")
+        append(sql_file, "CREATE TABLE test_table2 (id INTEGER PRIMARY KEY);")
+
+        database = Database(tmp_path, sql_file=sql_file)
+
+        sql_stmt = "SELECT * FROM test_table2;"
+        with Session(database.engine) as session:
+            result = session.execute(text(sql_stmt))
+        assert result.fetchall() == []  # nosec
```

### Comparing `toolcat-0.0.7/src/toolcat/project.py` & `toolcat-0.0.8/src/toolcat/project.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.7/src/toolcat/projects_test.py` & `toolcat-0.0.8/src/toolcat/projects_test.py`

 * *Files identical despite different names*

### Comparing `toolcat-0.0.7/PKG-INFO` & `toolcat-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolcat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Essential Libraries and Tools for Streamlined Development
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

