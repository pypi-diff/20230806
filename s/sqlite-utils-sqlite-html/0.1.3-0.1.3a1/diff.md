# Comparing `tmp/sqlite_utils_sqlite_html-0.1.3-py3-none-any.whl.zip` & `tmp/sqlite_utils_sqlite_html-0.1.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2172 bytes, number of entries: 7
--rw-r--r--  2.0 unx      273 b- defN 23-Aug-06 01:25 sqlite_utils_sqlite_html/__init__.py
--rw-r--r--  2.0 unx       71 b- defN 23-Aug-06 01:25 sqlite_utils_sqlite_html/version.py
--rw-r--r--  2.0 unx      514 b- defN 23-Aug-06 01:26 sqlite_utils_sqlite_html-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:26 sqlite_utils_sqlite_html-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Aug-06 01:26 sqlite_utils_sqlite_html-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Aug-06 01:26 sqlite_utils_sqlite_html-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      659 b- defN 23-Aug-06 01:26 sqlite_utils_sqlite_html-0.1.3.dist-info/RECORD
-7 files, 1688 bytes uncompressed, 970 bytes compressed:  42.5%
+Zip file size: 2198 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      273 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html/version.py
+-rw-r--r--  2.0 unx      516 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html-0.1.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html-0.1.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html-0.1.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html-0.1.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      669 b- defN 23-Aug-06 01:08 sqlite_utils_sqlite_html-0.1.3a1.dist-info/RECORD
+7 files, 1708 bytes uncompressed, 976 bytes compressed:  42.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sqlite_utils_sqlite_html/__init__.py
 Comment: 
 
 Filename: sqlite_utils_sqlite_html/version.py
 Comment: 
 
-Filename: sqlite_utils_sqlite_html-0.1.3.dist-info/METADATA
+Filename: sqlite_utils_sqlite_html-0.1.3a1.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_utils_sqlite_html-0.1.3.dist-info/WHEEL
+Filename: sqlite_utils_sqlite_html-0.1.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_utils_sqlite_html-0.1.3.dist-info/entry_points.txt
+Filename: sqlite_utils_sqlite_html-0.1.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_html-0.1.3.dist-info/top_level.txt
+Filename: sqlite_utils_sqlite_html-0.1.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_utils_sqlite_html-0.1.3.dist-info/RECORD
+Filename: sqlite_utils_sqlite_html-0.1.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_utils_sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.3"
+__version__ = "0.1.3-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_utils_sqlite_html-0.1.3.dist-info/METADATA` & `sqlite_utils_sqlite_html-0.1.3a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-sqlite-html
-Version: 0.1.3
+Version: 0.1.3a1
 Summary: TODO
 Author: Alex Garcia
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asg017/sqlite-html
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Description-Content-Type: text/markdown
```

## Comparing `sqlite_utils_sqlite_html-0.1.3.dist-info/RECORD` & `sqlite_utils_sqlite_html-0.1.3a1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 sqlite_utils_sqlite_html/__init__.py,sha256=qnTPpOr8Ta4YmAnF2WdFb6ZgIY7nLWJtXlcAYSR-McA,273
-sqlite_utils_sqlite_html/version.py,sha256=D9O3Uo_hAjRYpn9mVLh27HzJjOfc6vbGXP6Le4G3XLM,71
-sqlite_utils_sqlite_html-0.1.3.dist-info/METADATA,sha256=0K6hMxP94IQpp6eQb0qcFl5qm2zk_BBOiXHHEz4AC2A,514
-sqlite_utils_sqlite_html-0.1.3.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-sqlite_utils_sqlite_html-0.1.3.dist-info/entry_points.txt,sha256=xFpprlEbT-QixAzRP9x6czek6k8cnhQJtjsZxiN29LA,54
-sqlite_utils_sqlite_html-0.1.3.dist-info/top_level.txt,sha256=r_IodRwvO093zmvT9an6x5CeqpII7bilJoIbFwajcnY,25
-sqlite_utils_sqlite_html-0.1.3.dist-info/RECORD,,
+sqlite_utils_sqlite_html/version.py,sha256=QSbXvlEjLHCYYQgBaFmAk9xQ5lvlXwdcrxjtaqam8BM,79
+sqlite_utils_sqlite_html-0.1.3a1.dist-info/METADATA,sha256=vqcsMfKGaHuddgGsVmXh9VQTq89p0P8bE0-ZSbOryOI,516
+sqlite_utils_sqlite_html-0.1.3a1.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+sqlite_utils_sqlite_html-0.1.3a1.dist-info/entry_points.txt,sha256=xFpprlEbT-QixAzRP9x6czek6k8cnhQJtjsZxiN29LA,54
+sqlite_utils_sqlite_html-0.1.3a1.dist-info/top_level.txt,sha256=r_IodRwvO093zmvT9an6x5CeqpII7bilJoIbFwajcnY,25
+sqlite_utils_sqlite_html-0.1.3a1.dist-info/RECORD,,
```

