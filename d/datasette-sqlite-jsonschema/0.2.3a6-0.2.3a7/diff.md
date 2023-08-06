# Comparing `tmp/datasette_sqlite_jsonschema-0.2.3a6-py3-none-any.whl.zip` & `tmp/datasette_sqlite_jsonschema-0.2.3a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2286 bytes, number of entries: 7
--rw-r--r--  2.0 unx      284 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema/version.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema-0.2.3a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema-0.2.3a6.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema-0.2.3a6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema-0.2.3a6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      690 b- defN 23-Jun-10 21:36 datasette_sqlite_jsonschema-0.2.3a6.dist-info/RECORD
-7 files, 1832 bytes uncompressed, 1022 bytes compressed:  44.2%
+Zip file size: 2283 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      284 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema/version.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema-0.2.3a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema-0.2.3a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema-0.2.3a7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema-0.2.3a7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      690 b- defN 23-Aug-06 00:11 datasette_sqlite_jsonschema-0.2.3a7.dist-info/RECORD
+7 files, 1832 bytes uncompressed, 1019 bytes compressed:  44.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_jsonschema/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_jsonschema/version.py
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a6.dist-info/METADATA
+Filename: datasette_sqlite_jsonschema-0.2.3a7.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a6.dist-info/WHEEL
+Filename: datasette_sqlite_jsonschema-0.2.3a7.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a6.dist-info/entry_points.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a7.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a6.dist-info/top_level.txt
+Filename: datasette_sqlite_jsonschema-0.2.3a7.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_jsonschema-0.2.3a6.dist-info/RECORD
+Filename: datasette_sqlite_jsonschema-0.2.3a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_jsonschema/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.3-alpha.6"
+__version__ = "0.2.3-alpha.7"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_jsonschema-0.2.3a6.dist-info/METADATA` & `datasette_sqlite_jsonschema-0.2.3a7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-jsonschema
-Version: 0.2.3a6
+Version: 0.2.3a7
 Home-page: https://github.com/asg017/sqlite-jsonschema
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-jsonschema/issues
 Project-URL: CI, https://github.com/asg017/sqlite-jsonschema/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-jsonschema/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_jsonschema-0.2.3a6.dist-info/RECORD` & `datasette_sqlite_jsonschema-0.2.3a7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_jsonschema/__init__.py,sha256=CkEgCNG1ogAHTmP5eAR4aQ3TdxqqmgBIs9kLzsEp29U,284
-datasette_sqlite_jsonschema/version.py,sha256=lJ1zT0l1sW8a6j7QSzGGs7rWHxwIQ2jpDfsHr9yJSAM,79
-datasette_sqlite_jsonschema-0.2.3a6.dist-info/METADATA,sha256=eSOZeFEiae0Bm_kuTzTy2u6qyl3MrX64ZdcZqP_BGUI,599
-datasette_sqlite_jsonschema-0.2.3a6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_jsonschema-0.2.3a6.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
-datasette_sqlite_jsonschema-0.2.3a6.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
-datasette_sqlite_jsonschema-0.2.3a6.dist-info/RECORD,,
+datasette_sqlite_jsonschema/version.py,sha256=A28y-VC9rJoXlBjbqXe664JVG4M8eRV92cMF5jv8w_c,79
+datasette_sqlite_jsonschema-0.2.3a7.dist-info/METADATA,sha256=Er7yro9JLg3-i3QM8JryXl79dSg3d-GOqaUWAB0BeuI,599
+datasette_sqlite_jsonschema-0.2.3a7.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+datasette_sqlite_jsonschema-0.2.3a7.dist-info/entry_points.txt,sha256=GudkqSm13Ou5ZqFjwDzCYFo5oo9FSVgstqZWdGYOGTo,60
+datasette_sqlite_jsonschema-0.2.3a7.dist-info/top_level.txt,sha256=gGoRXv89K-JydhKqkfeF25P05Er5OkO8wqnHPcKfim0,28
+datasette_sqlite_jsonschema-0.2.3a7.dist-info/RECORD,,
```

