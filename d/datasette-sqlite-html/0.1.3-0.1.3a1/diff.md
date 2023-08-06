# Comparing `tmp/datasette_sqlite_html-0.1.3-py3-none-any.whl.zip` & `tmp/datasette_sqlite_html-0.1.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2140 bytes, number of entries: 7
--rw-r--r--  2.0 unx      266 b- defN 23-Aug-06 01:25 datasette_sqlite_html/__init__.py
--rw-r--r--  2.0 unx       71 b- defN 23-Aug-06 01:25 datasette_sqlite_html/version.py
--rw-r--r--  2.0 unx      561 b- defN 23-Aug-06 01:25 datasette_sqlite_html-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:25 datasette_sqlite_html-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Aug-06 01:25 datasette_sqlite_html-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Aug-06 01:25 datasette_sqlite_html-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      638 b- defN 23-Aug-06 01:25 datasette_sqlite_html-0.1.3.dist-info/RECORD
-7 files, 1698 bytes uncompressed, 980 bytes compressed:  42.3%
+Zip file size: 2173 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      266 b- defN 23-Aug-06 01:08 datasette_sqlite_html/__init__.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 01:08 datasette_sqlite_html/version.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      648 b- defN 23-Aug-06 01:08 datasette_sqlite_html-0.1.3a1.dist-info/RECORD
+7 files, 1718 bytes uncompressed, 993 bytes compressed:  42.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_html/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_html/version.py
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.3.dist-info/METADATA
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.3.dist-info/WHEEL
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.3.dist-info/entry_points.txt
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.3.dist-info/top_level.txt
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_html-0.1.3.dist-info/RECORD
+Filename: datasette_sqlite_html-0.1.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_html/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.3"
+__version__ = "0.1.3-alpha.1"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_html-0.1.3.dist-info/METADATA` & `datasette_sqlite_html-0.1.3a1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-html
-Version: 0.1.3
+Version: 0.1.3a1
 Home-page: https://github.com/asg017/sqlite-html
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-html/issues
 Project-URL: CI, https://github.com/asg017/sqlite-html/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-html/releases
 Requires-Python: >=3.7
```

## Comparing `datasette_sqlite_html-0.1.3.dist-info/RECORD` & `datasette_sqlite_html-0.1.3a1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_html/__init__.py,sha256=ziq-rB8yRAubkqikIZWqeA0LneQKWCSDJnOW7xBsbCk,266
-datasette_sqlite_html/version.py,sha256=D9O3Uo_hAjRYpn9mVLh27HzJjOfc6vbGXP6Le4G3XLM,71
-datasette_sqlite_html-0.1.3.dist-info/METADATA,sha256=CyqMs-V0soQ_mOgGZ8L8iJ4EqGqJoJI8ttTr9MWF2Y4,561
-datasette_sqlite_html-0.1.3.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-datasette_sqlite_html-0.1.3.dist-info/entry_points.txt,sha256=Ty_dShJsQ23N4JA2PDKNMxbZ5bPiqj27zovbiCDI39I,48
-datasette_sqlite_html-0.1.3.dist-info/top_level.txt,sha256=bWwftX05h2WWmdOY-2uemMvvSCnkABrOTsdkOEgVOEg,22
-datasette_sqlite_html-0.1.3.dist-info/RECORD,,
+datasette_sqlite_html/version.py,sha256=QSbXvlEjLHCYYQgBaFmAk9xQ5lvlXwdcrxjtaqam8BM,79
+datasette_sqlite_html-0.1.3a1.dist-info/METADATA,sha256=3UplHUEYBQtfjzSHzErQuBU4ydCmbXgIm6_RoYMguOw,563
+datasette_sqlite_html-0.1.3a1.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+datasette_sqlite_html-0.1.3a1.dist-info/entry_points.txt,sha256=Ty_dShJsQ23N4JA2PDKNMxbZ5bPiqj27zovbiCDI39I,48
+datasette_sqlite_html-0.1.3a1.dist-info/top_level.txt,sha256=bWwftX05h2WWmdOY-2uemMvvSCnkABrOTsdkOEgVOEg,22
+datasette_sqlite_html-0.1.3a1.dist-info/RECORD,,
```

