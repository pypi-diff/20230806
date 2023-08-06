# Comparing `tmp/datasette_sqlite_html-0.1.2a8-py3-none-any.whl.zip` & `tmp/datasette_sqlite_html-0.1.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2173 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Aug-05 03:34 datasette_sqlite_html/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-05 03:34 datasette_sqlite_html/version.py
--rw-r--r--  2.0 unx      563 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      648 b- defN 23-Aug-05 03:34 datasette_sqlite_html-0.1.2a8.dist-info/RECORD
+-rw-r--r--  2.0 unx      266 b- defN 23-Aug-06 01:08 datasette_sqlite_html/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 01:08 datasette_sqlite_html/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/RECORD
 7 files, 1718 bytes uncompressed, 993 bytes compressed:  42.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_html/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_html/version.py
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a8.dist-info/METADATA
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a8.dist-info/WHEEL
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a8.dist-info/entry_points.txt
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a8.dist-info/top_level.txt
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.2a8.dist-info/RECORD
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.2-alpha.8"
+__version__ = "0.1.3-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_html-0.1.2a8.dist-info/METADATA` & `datasette_sqlite_html-0.1.3a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-html
-Version: 0.1.2a8
+Version: 0.1.3a1
 Home-page: https://github.com/asg017/sqlite-html
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Project-URL: CI, https://github.com/asg017/sqlite-html/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Requires-Python: >=3.7
```

