# Comparing `tmp/sqlite_utils_sqlite_hello-0.1.0a61-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_hello-0.1.0a62-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2234 bytes, number of entries: 7
--rw-r--r--  2.0 unx      276 b- defN 23-Jul-24 01:14 sqlite_utils_sqlite_hello/__init__.py
--rw-r--r--  2.0 unx       80 b- defN 23-Jul-24 01:14 sqlite_utils_sqlite_hello/version.py
--rw-r--r--  2.0 unx      524 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      681 b- defN 23-Jul-24 01:15 sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD
-7 files, 1735 bytes uncompressed, 988 bytes compressed:  43.1%
+Zip file size: 2233 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      276 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello/version.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello-0.1.0a62.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello-0.1.0a62.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello-0.1.0a62.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       26 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello-0.1.0a62.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 23-Aug-06 08:48 sqlite_utils_sqlite_hello-0.1.0a62.dist-info/RECORD
+7 files, 1735 bytes uncompressed, 987 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_hello/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA
+Filename: sqlite_utils_sqlite_hello-0.1.0a62.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_hello-0.1.0a62.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a62.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_hello-0.1.0a62.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD
+Filename: sqlite_utils_sqlite_hello-0.1.0a62.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.61"
+__version__ = "0.1.0-alpha.62"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA` & `sqlite_utils_sqlite_hello-0.1.0a62.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-sqlite-hello
-Version: 0.1.0a61
+Version: 0.1.0a62
 Summary: TODO
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asg017/sqlite-hello
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Description-Content-Type: text/markdown
```

## Comparing `sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD` & `sqlite_utils_sqlite_hello-0.1.0a62.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sqlite_utils_sqlite_hello/__init__.py,sha256=1kBGZZAQRzS0XkdUqDVFeze5gh1w8HkN_Sdc6Q6GNMg,276
-sqlite_utils_sqlite_hello/version.py,sha256=GUVYGCmBwrxEaVh-nxq-MZfYW9gEDDfShgRKT9RRMi8,80
-sqlite_utils_sqlite_hello-0.1.0a61.dist-info/METADATA,sha256=KI55MRaIKGpHaq0G5j7fa8NKh6NVM9xDrfjtC3xgatE,524
-sqlite_utils_sqlite_hello-0.1.0a61.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-sqlite_utils_sqlite_hello-0.1.0a61.dist-info/entry_points.txt,sha256=GkeiI1YN1zuw1rIf-3BWSz_aKo03ttq1AAbPMv7Z5Wc,56
-sqlite_utils_sqlite_hello-0.1.0a61.dist-info/top_level.txt,sha256=RDXX67SyuHEZi7qGbD-6OKES0y-shx1CMoviTs_KLjM,26
-sqlite_utils_sqlite_hello-0.1.0a61.dist-info/RECORD,,
+sqlite_utils_sqlite_hello/version.py,sha256=YwAB48BvQJsrwJUy0dFenS5JVeHPuiRkA93joj-nfZ0,80
+sqlite_utils_sqlite_hello-0.1.0a62.dist-info/METADATA,sha256=_YV85a1I8sCm0ALPBv4Z8k3qmdNe7psF_TFPiksarDk,524
+sqlite_utils_sqlite_hello-0.1.0a62.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+sqlite_utils_sqlite_hello-0.1.0a62.dist-info/entry_points.txt,sha256=GkeiI1YN1zuw1rIf-3BWSz_aKo03ttq1AAbPMv7Z5Wc,56
+sqlite_utils_sqlite_hello-0.1.0a62.dist-info/top_level.txt,sha256=RDXX67SyuHEZi7qGbD-6OKES0y-shx1CMoviTs_KLjM,26
+sqlite_utils_sqlite_hello-0.1.0a62.dist-info/RECORD,,
```

