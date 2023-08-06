# Comparing `tmp/datasette_sqlite_lines-0.2.1a2-py3-none-any.whl.zip` & `tmp/datasette_sqlite_lines-0.2.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2294 bytes, number of entries: 7
--rw-r--r--  2.0 unx      515 b- defN 23-Aug-05 03:57 datasette_sqlite_lines/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:57 datasette_sqlite_lines/version.py
--rw-r--r--  2.0 unx      569 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 23-Aug-05 03:57 datasette_sqlite_lines-0.2.1a2.dist-info/RECORD
+-rw-r--r--  2.0 unx      515 b- defN 23-Aug-06 06:42 datasette_sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 06:42 datasette_sqlite_lines/version.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Aug-06 06:42 datasette_sqlite_lines-0.2.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 06:42 datasette_sqlite_lines-0.2.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Aug-06 06:42 datasette_sqlite_lines-0.2.2a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Aug-06 06:42 datasette_sqlite_lines-0.2.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-Aug-06 06:42 datasette_sqlite_lines-0.2.2a1.dist-info/RECORD
 7 files, 1983 bytes uncompressed, 1100 bytes compressed:  44.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_lines/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_lines/version.py
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a2.dist-info/METADATA
+Filename: datasette_sqlite_lines-0.2.2a1.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a2.dist-info/WHEEL
+Filename: datasette_sqlite_lines-0.2.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a2.dist-info/entry_points.txt
+Filename: datasette_sqlite_lines-0.2.2a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a2.dist-info/top_level.txt
+Filename: datasette_sqlite_lines-0.2.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_lines-0.2.1a2.dist-info/RECORD
+Filename: datasette_sqlite_lines-0.2.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.1-alpha.2"
+__version__ = "0.2.2-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_lines-0.2.1a2.dist-info/METADATA` & `datasette_sqlite_lines-0.2.2a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-lines
-Version: 0.2.1a2
+Version: 0.2.2a1
 Home-page: https://github.com/asg017/sqlite-lines
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-lines/issues
 Project-URL: CI, https://github.com/asg017/sqlite-lines/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-lines/releases
 Requires-Python: >=3.7
```

