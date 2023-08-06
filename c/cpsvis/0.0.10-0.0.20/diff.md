# Comparing `tmp/cpsvis-0.0.10-py3-none-any.whl.zip` & `tmp/cpsvis-0.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2640 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Aug-05 23:25 cpsvis/__init__.py
 -rw-rw-r--  2.0 unx       38 b- defN 23-Aug-05 23:55 cpsvis/main.py
--rw-rw-r--  2.0 unx     1071 b- defN 23-Aug-05 23:59 cpsvis-0.0.10.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1026 b- defN 23-Aug-05 23:59 cpsvis-0.0.10.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-05 23:59 cpsvis-0.0.10.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Aug-05 23:59 cpsvis-0.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      526 b- defN 23-Aug-05 23:59 cpsvis-0.0.10.dist-info/RECORD
+-rw-rw-r--  2.0 unx     1071 b- defN 23-Aug-06 00:16 cpsvis-0.0.20.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1026 b- defN 23-Aug-06 00:16 cpsvis-0.0.20.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-06 00:16 cpsvis-0.0.20.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Aug-06 00:16 cpsvis-0.0.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      526 b- defN 23-Aug-06 00:16 cpsvis-0.0.20.dist-info/RECORD
 7 files, 2760 bytes uncompressed, 1704 bytes compressed:  38.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cpsvis/__init__.py
 Comment: 
 
 Filename: cpsvis/main.py
 Comment: 
 
-Filename: cpsvis-0.0.10.dist-info/LICENSE
+Filename: cpsvis-0.0.20.dist-info/LICENSE
 Comment: 
 
-Filename: cpsvis-0.0.10.dist-info/METADATA
+Filename: cpsvis-0.0.20.dist-info/METADATA
 Comment: 
 
-Filename: cpsvis-0.0.10.dist-info/WHEEL
+Filename: cpsvis-0.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: cpsvis-0.0.10.dist-info/top_level.txt
+Filename: cpsvis-0.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: cpsvis-0.0.10.dist-info/RECORD
+Filename: cpsvis-0.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cpsvis-0.0.10.dist-info/LICENSE` & `cpsvis-0.0.20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cpsvis-0.0.10.dist-info/METADATA` & `cpsvis-0.0.20.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cpsvis
-Version: 0.0.10
+Version: 0.0.20
 Summary: Convex Projective Surface Visualisation Tool
 Home-page: https://github.com/sepehrsaryazdi/cpsvis2
 Author: Sepehr Saryazdi
 Author-email: sepehr.saryazdi@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: numpy (>=1.21.5)
 Requires-Dist: tkinter (>=8.6)
 Provides-Extra: dev
 Requires-Dist: pytest (>=7.0) ; extra == 'dev'
 Requires-Dist: twine (>=4.0.2) ; extra == 'dev'
```

