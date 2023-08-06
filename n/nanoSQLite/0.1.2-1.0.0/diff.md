# Comparing `tmp/nanoSQLite-0.1.2.tar.gz` & `tmp/nanoSQLite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoSQLite-0.1.2.tar", last modified: Sun Aug  6 00:11:09 2023, max compression
+gzip compressed data, was "nanoSQLite-1.0.0.tar", last modified: Sun Aug  6 12:14:57 2023, max compression
```

## Comparing `nanoSQLite-0.1.2.tar` & `nanoSQLite-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:11:09.283110 nanoSQLite-0.1.2/
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2183 2023-08-06 00:11:09.282110 nanoSQLite-0.1.2/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1999 2023-08-05 23:50:53.000000 nanoSQLite-0.1.2/README.md
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:11:09.282110 nanoSQLite-0.1.2/nanoSQLite/
--rw-r--r--   0 stefan    (1000) stefan    (1000)       26 2023-08-06 00:03:23.000000 nanoSQLite-0.1.2/nanoSQLite/__init__.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)     6735 2023-08-05 23:48:12.000000 nanoSQLite-0.1.2/nanoSQLite/nanoSQLite.py
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 00:11:09.282110 nanoSQLite-0.1.2/nanoSQLite.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2183 2023-08-06 00:11:09.000000 nanoSQLite-0.1.2/nanoSQLite.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)      202 2023-08-06 00:11:09.000000 nanoSQLite-0.1.2/nanoSQLite.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2023-08-06 00:11:09.000000 nanoSQLite-0.1.2/nanoSQLite.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)       11 2023-08-06 00:11:09.000000 nanoSQLite-0.1.2/nanoSQLite.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)       38 2023-08-06 00:11:09.283110 nanoSQLite-0.1.2/setup.cfg
--rw-r--r--   0 stefan    (1000) stefan    (1000)      327 2023-08-06 00:11:06.000000 nanoSQLite-0.1.2/setup.py
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 12:14:57.690494 nanoSQLite-1.0.0/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     3233 2023-08-06 12:14:57.690494 nanoSQLite-1.0.0/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     3049 2023-08-06 12:11:37.000000 nanoSQLite-1.0.0/README.md
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 12:14:57.689494 nanoSQLite-1.0.0/nanoSQLite/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       26 2023-08-06 00:03:23.000000 nanoSQLite-1.0.0/nanoSQLite/__init__.py
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     6746 2023-08-06 11:58:59.000000 nanoSQLite-1.0.0/nanoSQLite/nanoSQLite.py
+drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2023-08-06 12:14:57.690494 nanoSQLite-1.0.0/nanoSQLite.egg-info/
+-rw-r--r--   0 stefan    (1000) stefan    (1000)     3233 2023-08-06 12:14:57.000000 nanoSQLite-1.0.0/nanoSQLite.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      202 2023-08-06 12:14:57.000000 nanoSQLite-1.0.0/nanoSQLite.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2023-08-06 12:14:57.000000 nanoSQLite-1.0.0/nanoSQLite.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       11 2023-08-06 12:14:57.000000 nanoSQLite-1.0.0/nanoSQLite.egg-info/top_level.txt
+-rw-r--r--   0 stefan    (1000) stefan    (1000)       38 2023-08-06 12:14:57.690494 nanoSQLite-1.0.0/setup.cfg
+-rw-r--r--   0 stefan    (1000) stefan    (1000)      327 2023-08-06 11:48:46.000000 nanoSQLite-1.0.0/setup.py
```

### Comparing `nanoSQLite-0.1.2/PKG-INFO` & `nanoSQLite-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,91 @@
-Metadata-Version: 2.1
-Name: nanoSQLite
-Version: 0.1.2
-Home-page: https://github.com/stefanluth/nanoSQLite
-Author: Stefan Luthardt
-License: MIT
-Description-Content-Type: text/markdown
-
 # nanoSQLite
 
 `nanoSQLite` is a lightweight Python wrapper for SQLite.
 With around 200 lines of Python code, it provides an uncomplicated interface for managing SQLite databases.
 
 Despite its simplicity, nanoSQLite offers a robust set of functionalities that enable you to interact with
 SQLite databases seamlessly, without having to worry about managing cursors and connections manually.
 
 It's designed to make working with SQLite in Python as straightforward and Pythonic as possible.
 
 ## Features
 
 - Easy Setup: Create connections to SQLite databases with a single function call.
-- Simple Query Execution:
-Execute your SQL commands easily, without having to manage cursors and connections manually.
-- Transaction Management:
-Handle transactions effectively with commit and rollback operations.
-- Pythonic Interface:
-The nanoSQLite API is designed to be as Pythonic as possible, which makes it intuitive and easy to use.
+- Intuitive Interface: Insert, update, and delete data using a simple syntax.
+- Quick Prototyping: Manage data efficiently with a few lines of code, perfect for rapid prototyping and basic projects.
+- Flexible: Execute custom SQL statements using the underlying `sqlite3.Cursor` and `sqlite3.Connection` objects.
+- Robust: The `sqlite3` module is part of the Python standard library and has been extensively tested.
+- Pythonic: The nanoSQLite API is designed to be as Pythonic as possible, which makes it intuitive and easy to use.
+- Pure Python: nanoSQLite is written with no dependencies.
+- Lightweight: nanoSQLite is a single-file module with around 200 lines of code.
+- Open Source: nanoSQLite is distributed under the MIT license.
 
 ## Examples
 
-Create a new SQLite database with a table:
-
-```python
-from nanoSQLite import NanoSQLite
-
-db = NanoSQLite("people")
-db.create_table(
-    "friends",
-    {
-        "id": "INTEGER PRIMARY KEY AUTOINCREMENT",
-        "name": "TEXT",
-        "age": "INTEGER",
-        "height": "REAL",
-        "is_cool": "BOOLEAN",
-    },
-)
-```
-
-Insert data:
-
-```python
-db.insert("friends", {"name": "John", "age": 20, "height": 1.8, "is_cool": True})
-db.insert("friends", {"name": "Jane", "height": 1.7, "is_cool": False})
-db.insert("friends", {"name": "Bob"})
-```
+Most of database operations can be covered with the following examples:
 
-Update data:
+1. Create a new SQLite database with a table:
 
-```python
-db.update("friends", {"age": 21, "height": 1.9}, {"name": "John"})
-db.update("friends", {"age": 5}, {"name": "Bob"})
-```
+    ```python
+    from nanoSQLite import NanoSQLite
 
-Delete data:
-
-```python
-db.delete("friends", {"name": "Jane"})
-```
+    db = NanoSQLite("people")
+    db.create_table(
+        "friends",
+        {
+            "id": "INTEGER PRIMARY KEY AUTOINCREMENT",
+            "name": "TEXT",
+            "age": "INTEGER",
+            "height": "REAL",
+            "is_cool": "BOOLEAN",
+        },
+    )
+    ```
+
+2. Insert data:
+
+    ```python
+    db.insert("friends", {"name": "John", "age": 20, "height": 1.8, "is_cool": True})
+    db.insert("friends", {"name": "Jane", "height": 1.7, "is_cool": False})
+    db.insert("friends", {"name": "Bob"})
+    ```
+
+3. Update data:
+
+    ```python
+    db.update("friends", {"age": 21, "height": 1.9}, {"name": "John"})
+    db.update("friends", {"age": 5}, {"name": "Bob"})
+    ```
+
+4. Delete data:
+
+    ```python
+    db.delete("friends", {"name": "Jane"})
+    ```
+
+5. Select data:
+
+    ```python
+    db.select("friends", ["name", "age", "height", "is_cool"], {"name": "Bob"})
+    db.select_first("friends", ["name", "age", "height", "is_cool"], {"name": "Bob"})
+    db.select_all("friends")
+    ```
 
-Select data:
+When more advanced functionality is required, you can still execute custom SQL statements,
+using the underlying `sqlite3.Cursor` and `sqlite3.Connection` objects:
 
 ```python
-db.select("friends", ["name", "age", "height", "is_cool"], {"name": "Bob"})
-db.select_first("friends", ["name", "age", "height", "is_cool"], {"name": "Bob"})
-db.select_all("friends")
+data = [
+    ("Monty Python Live at the Hollywood Bowl", 1982, 7.9),
+    ("Monty Python's The Meaning of Life", 1983, 7.5),
+    ("Monty Python's Life of Brian", 1979, 8.0),
+]
+db.cursor.executemany("INSERT INTO movie VALUES(?, ?, ?)", data)
+db.connection.commit()
 ```
 
 ## Installation
 
 You can install nanoSQLite from PyPI:
 
 ```bash
```

### Comparing `nanoSQLite-0.1.2/nanoSQLite/nanoSQLite.py` & `nanoSQLite-1.0.0/nanoSQLite/nanoSQLite.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,37 +40,37 @@
 
     def close(self):
         """
         Close the database connection.
         """
         self.connection.close()
 
-    def _execute(self, query: str) -> None:
+    def execute(self, query: str) -> sqlite3.Cursor:
         with self._lock:
             with self.connection:
-                self.cursor.execute(query)
+                return self.cursor.execute(query)
 
     def create_table(self, name: str, columns: dict[str, str]) -> None:
         """
         Create a table in the database.
         :param name: The name of the table.
         :type name: str
         :param columns: The columns of the table. Each column is a tuple of the column name and the column type.
         :type columns: dict[str, str]
         """
-        self._execute(f"CREATE TABLE {name} ({', '.join([f'{col} {columns[col]}' for col in columns])})")
+        self.execute(f"CREATE TABLE {name} ({', '.join([f'{col} {columns[col]}' for col in columns])})")
         self.tables[name] = columns
 
     def delete_table(self, name: str) -> None:
         """
         Delete a table from the database.
         :param name: The name of the table.
         :type name: str
         """
-        self._execute(f"DROP TABLE {name}")
+        self.execute(f"DROP TABLE {name}")
         self.tables.pop(name)
 
     def insert(self, table: str, data: dict[str, str]) -> None:
         """
         Insert values into a table.
         :param table: The name of the table.
         :type table: str
@@ -83,15 +83,15 @@
 
         columns = ", ".join(data.keys())
         values = [
             convert(TYPE_CONVERSIONS.get(self.tables[table][col], lambda x: x), data[col], self.tables[table][col])
             for col in data
         ]
 
-        self._execute(f"INSERT INTO {table} ({columns}) VALUES ({', '.join([str(value) for value in values])})")
+        self.execute(f"INSERT INTO {table} ({columns}) VALUES ({', '.join([str(value) for value in values])})")
 
     def update(self, table: str, data: dict[str, str], where: dict[str, str]) -> None:
         """
         Update values in a table.
         :param table: The name of the table.
         :type table: str
         :param data: The data to update in the table. The keys are the column names and the values are the values to update.
@@ -108,15 +108,15 @@
             for col in data
         ]
         converted_where = [
             f"{col} = {convert(TYPE_CONVERSIONS.get(self.tables[table][col], lambda x: x), where[col], self.tables[table][col])}"
             for col in where
         ]
 
-        self._execute(f"UPDATE {table} SET {', '.join(converted_data)} WHERE {', '.join(converted_where)}")
+        self.execute(f"UPDATE {table} SET {', '.join(converted_data)} WHERE {', '.join(converted_where)}")
 
     def delete(self, table: str, where: dict[str, str]) -> None:
         """
         Delete values from a table.
         :param table: The name of the table.
         :type table: str
         :param where: The WHERE clause of the query.
@@ -127,15 +127,15 @@
             raise ValueError("At least one column must be specified.")
 
         converted_where = [
             f"{col} = {convert(TYPE_CONVERSIONS.get(self.tables[table][col], lambda x: x), where[col], self.tables[table][col])}"
             for col in where
         ]
 
-        self._execute(f"DELETE FROM {table} WHERE {', '.join(converted_where)}")
+        self.execute(f"DELETE FROM {table} WHERE {', '.join(converted_where)}")
 
     def select(self, table: str, columns: list[str], where: dict[str, str]) -> list[dict] | None:
         """
         Select values from a table.
         :param table: The name of the table.
         :type table: str
         :param columns: The columns to select.
```

