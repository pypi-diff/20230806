# Comparing `tmp/vmapper-0.1.0.dev202304232359-py3-none-any.whl.zip` & `tmp/vmapper-0.1.0.dev202308060456-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9944 bytes, number of entries: 7
+Zip file size: 9941 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 vmapper/__init__.py
 -rw-r--r--  2.0 unx     7759 b- defN 80-Jan-01 00:00 vmapper/color.py
 -rw-r--r--  2.0 unx     3395 b- defN 80-Jan-01 00:00 vmapper/meta_func.py
 -rw-r--r--  2.0 unx    29669 b- defN 80-Jan-01 00:00 vmapper/vmapper.py
--rw-r--r--  2.0 unx     1962 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304232359.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202304232359.dist-info/WHEEL
-?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202304232359.dist-info/RECORD
-7 files, 43479 bytes uncompressed, 8966 bytes compressed:  79.4%
+-rw-r--r--  2.0 unx     2007 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202308060456.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 vmapper-0.1.0.dev202308060456.dist-info/WHEEL
+?rw-r--r--  2.0 unx      554 b- defN 16-Jan-01 00:00 vmapper-0.1.0.dev202308060456.dist-info/RECORD
+7 files, 43524 bytes uncompressed, 8963 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: vmapper/meta_func.py
 Comment: 
 
 Filename: vmapper/vmapper.py
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304232359.dist-info/METADATA
+Filename: vmapper-0.1.0.dev202308060456.dist-info/METADATA
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304232359.dist-info/WHEEL
+Filename: vmapper-0.1.0.dev202308060456.dist-info/WHEEL
 Comment: 
 
-Filename: vmapper-0.1.0.dev202304232359.dist-info/RECORD
+Filename: vmapper-0.1.0.dev202308060456.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vmapper-0.1.0.dev202304232359.dist-info/METADATA` & `vmapper-0.1.0.dev202308060456.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vmapper
-Version: 0.1.0.dev202304232359
+Version: 0.1.0.dev202308060456
 Summary: V-Mapper
 Home-page: https://github.com/yusuke-imoto-lab/V-Mapper
 Author: Yusuke Imoto
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: graphviz (>=0.17)
 Requires-Dist: matplotlib (>=3.4.3)
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: scikit-learn (>=0.24)
 Project-URL: Documentation, https://yusuke-imoto-lab.github.io/V-Mapper/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/V-Mapper
 Description-Content-Type: text/markdown
```

