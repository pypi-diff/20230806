# Comparing `tmp/datasette_sqlite_hello-0.1.0a60-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a61-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2220 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      279 b- defN 23-Jul-24 00:58 datasette_sqlite_hello/__init__.py
--rw-rw-rw-  2.0 fat       82 b- defN 23-Jul-24 00:58 datasette_sqlite_hello/version.py
--rw-rw-rw-  2.0 fat      586 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      660 b- defN 23-Jul-24 00:59 datasette_sqlite_hello-0.1.0a60.dist-info/RECORD
-7 files, 1772 bytes uncompressed, 1016 bytes compressed:  42.7%
+Zip file size: 2201 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      269 b- defN 23-Jul-24 01:14 datasette_sqlite_hello/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Jul-24 01:14 datasette_sqlite_hello/version.py
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-24 01:14 datasette_sqlite_hello-0.1.0a61.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 01:14 datasette_sqlite_hello-0.1.0a61.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-24 01:14 datasette_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-24 01:14 datasette_sqlite_hello-0.1.0a61.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      660 b- defN 23-Jul-24 01:14 datasette_sqlite_hello-0.1.0a61.dist-info/RECORD
+7 files, 1744 bytes uncompressed, 997 bytes compressed:  42.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a60.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a61.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a60.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a61.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a60.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a61.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a60.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a61.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a60.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a61.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/__init__.py

 * *Ordering differences only*

```diff
@@ -1,10 +1,10 @@
-from datasette import hookimpl
-import sqlite_hello
-
-from datasette_sqlite_hello.version import __version_info__, __version__
-
-@hookimpl
-def prepare_connection(conn):
-    conn.enable_load_extension(True)
-    sqlite_hello.load(conn)
-    conn.enable_load_extension(False)
+from datasette import hookimpl
+import sqlite_hello
+
+from datasette_sqlite_hello.version import __version_info__, __version__
+
+@hookimpl
+def prepare_connection(conn):
+    conn.enable_load_extension(True)
+    sqlite_hello.load(conn)
+    conn.enable_load_extension(False)
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.60"
-__version_info__ = tuple(__version__.split("."))
+__version__ = "0.1.0-alpha.61"
+__version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a60.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a61.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
-Name: datasette-sqlite-hello
-Version: 0.1.0a60
-Home-page: https://github.com/asg017/sqlite-hello
-Author: Alex Garcia
-License: MIT License, Apache License, Version 2.0
-Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
-Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
-Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: datasette
-Requires-Dist: sqlite-hello
-Provides-Extra: test
-Requires-Dist: pytest ; extra == 'test'
-
+Metadata-Version: 2.1
+Name: datasette-sqlite-hello
+Version: 0.1.0a61
+Home-page: https://github.com/asg017/sqlite-hello
+Author: Alex Garcia
+License: MIT License, Apache License, Version 2.0
+Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
+Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
+Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: datasette
+Requires-Dist: sqlite-hello
+Provides-Extra: test
+Requires-Dist: pytest ; extra == 'test'
+
```

## Comparing `datasette_sqlite_hello-0.1.0a60.dist-info/RECORD` & `datasette_sqlite_hello-0.1.0a61.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-datasette_sqlite_hello/__init__.py,sha256=_bTDo2EMxavW_7jeQuin3Zjfcbjf_EWPBejF3967Zlw,279
-datasette_sqlite_hello/version.py,sha256=HlUiuzrv6zTP1AdX8bGiIbzFdycLI__qMH7FaxjqjAA,82
-datasette_sqlite_hello-0.1.0a60.dist-info/METADATA,sha256=oaVK52KPxoWFEITnAUMmq09sJ9XdBLZs9J4hjfCjq0o,586
-datasette_sqlite_hello-0.1.0a60.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-datasette_sqlite_hello-0.1.0a60.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
-datasette_sqlite_hello-0.1.0a60.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
-datasette_sqlite_hello-0.1.0a60.dist-info/RECORD,,
+datasette_sqlite_hello/__init__.py,sha256=GiwcIRu3EMST18OdDMuooqh_Ncg2ePiuYkVT46SHliE,269
+datasette_sqlite_hello/version.py,sha256=GUVYGCmBwrxEaVh-nxq-MZfYW9gEDDfShgRKT9RRMi8,80
+datasette_sqlite_hello-0.1.0a61.dist-info/METADATA,sha256=0RRMhZY62fU9sZEISVMcGL7OaMfn4uw3ykEc5tm_AIc,570
+datasette_sqlite_hello-0.1.0a61.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+datasette_sqlite_hello-0.1.0a61.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
+datasette_sqlite_hello-0.1.0a61.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
+datasette_sqlite_hello-0.1.0a61.dist-info/RECORD,,
```

