# Comparing `tmp/logical_rush-0.0.2-py3-none-any.whl.zip` & `tmp/logical_rush-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 776819 bytes, number of entries: 7
+Zip file size: 1274367 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-16 01:14 logical_rush/__init__.py
+-rw-rw-rw-  2.0 fat  1508352 b- defN 23-Jun-16 01:14 logical_rush/_logical_rush.pyd
 -rw-rw-rw-  2.0 fat  1508352 b- defN 23-Jun-16 01:14 logical_rush/logical_rush.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 19:13 logical_rush/logical_rush.py
 -rw-rw-rw-  2.0 fat   793088 b- defN 23-May-02 17:20 logical_rush/logical_rush.so
--rw-rw-rw-  2.0 fat     3502 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      590 b- defN 23-Aug-05 15:49 logical_rush-0.0.2.dist-info/RECORD
-7 files, 2305768 bytes uncompressed, 775775 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     3409 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      762 b- defN 23-Aug-05 19:17 logical_rush-0.0.3.dist-info/RECORD
+9 files, 3814199 bytes uncompressed, 1273055 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: logical_rush/__init__.py
 Comment: 
 
+Filename: logical_rush/_logical_rush.pyd
+Comment: 
+
 Filename: logical_rush/logical_rush.cp310-win_amd64.pyd
 Comment: 
 
+Filename: logical_rush/logical_rush.py
+Comment: 
+
 Filename: logical_rush/logical_rush.so
 Comment: 
 
-Filename: logical_rush-0.0.2.dist-info/METADATA
+Filename: logical_rush-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: logical_rush-0.0.2.dist-info/WHEEL
+Filename: logical_rush-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: logical_rush-0.0.2.dist-info/top_level.txt
+Filename: logical_rush-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: logical_rush-0.0.2.dist-info/RECORD
+Filename: logical_rush-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `logical_rush-0.0.2.dist-info/METADATA` & `logical_rush-0.0.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: logical-rush
-Version: 0.0.2
+Version: 0.0.3
 Summary: Batch-computing solution for cashflow calculations.
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: pandas
-Requires-Dist: urllib3
-Requires-Dist: pytz
 
 
 # logical_rush
 Batch-computing solution for cashflow calculations.
 
 # Developed by Rodolfo Blasser 
 https://www.linkedin.com/in/rodblasser/
```

