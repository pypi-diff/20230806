# Comparing `tmp/cougar-0.2.19-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/cougar-0.2.20-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25262 bytes, number of entries: 10
--rw-r--r--  2.0 unx      287 b- defN 23-Aug-06 06:47 cougar/__init__.py
--rwxr-xr-x  2.0 unx    86456 b- defN 23-Aug-06 06:47 cougar/rolling.cpython-39-darwin.so
--rw-r--r--  2.0 unx       26 b- defN 23-Aug-06 06:47 cougar/numpy/__init__.py
--rw-r--r--  2.0 unx     1470 b- defN 23-Aug-06 06:47 cougar/numpy/functional.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 06:47 tests/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-06 06:47 cougar-0.2.19.dist-info/LICENSE
--rw-r--r--  2.0 unx     1000 b- defN 23-Aug-06 06:47 cougar-0.2.19.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Aug-06 06:47 cougar-0.2.19.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-06 06:47 cougar-0.2.19.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      788 b- defN 23-Aug-06 06:47 cougar-0.2.19.dist-info/RECORD
-10 files, 101505 bytes uncompressed, 23922 bytes compressed:  76.4%
+Zip file size: 103043 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-06 06:51 cougar/__init__.py
+-rwxr-xr-x  2.0 unx   238240 b- defN 23-Aug-06 06:52 cougar/rolling.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       26 b- defN 23-Aug-06 06:51 cougar/numpy/__init__.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-Aug-06 06:51 cougar/numpy/functional.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 06:51 tests/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-06 06:52 cougar-0.2.20.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1000 b- defN 23-Aug-06 06:52 cougar-0.2.20.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Aug-06 06:52 cougar-0.2.20.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-06 06:52 cougar-0.2.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      799 b- defN 23-Aug-06 06:52 cougar-0.2.20.dist-info/RECORD
+10 files, 253300 bytes uncompressed, 101683 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
 Filename: cougar/__init__.py
 Comment: 
 
-Filename: cougar/rolling.cpython-39-darwin.so
+Filename: cougar/rolling.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: cougar/numpy/__init__.py
 Comment: 
 
 Filename: cougar/numpy/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: cougar-0.2.19.dist-info/LICENSE
+Filename: cougar-0.2.20.dist-info/LICENSE
 Comment: 
 
-Filename: cougar-0.2.19.dist-info/METADATA
+Filename: cougar-0.2.20.dist-info/METADATA
 Comment: 
 
-Filename: cougar-0.2.19.dist-info/WHEEL
+Filename: cougar-0.2.20.dist-info/WHEEL
 Comment: 
 
-Filename: cougar-0.2.19.dist-info/top_level.txt
+Filename: cougar-0.2.20.dist-info/top_level.txt
 Comment: 
 
-Filename: cougar-0.2.19.dist-info/RECORD
+Filename: cougar-0.2.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cougar-0.2.19.dist-info/LICENSE` & `cougar-0.2.20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cougar-0.2.19.dist-info/METADATA` & `cougar-0.2.20.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.2.19
+Version: 0.2.20
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cougar-0.2.19.dist-info/RECORD` & `cougar-0.2.20.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cougar/__init__.py,sha256=j3D3jX-Fn9vgbSAftoZUen46tmJU7TqEO0z8xdikGIE,287
-cougar/rolling.cpython-39-darwin.so,sha256=W5H_LoHHd13NVUBUIO84doGCMiLwSRL7xO51tX1fQHk,86456
+cougar/rolling.cpython-39-x86_64-linux-gnu.so,sha256=R8kftD2XEENikYrm3dX-8MHtbqPr9pr5-Y4YnRcnruI,238240
 cougar/numpy/__init__.py,sha256=QsZLoNOPzs17hbkFTJowo2Ik_wJ55Nl9OreWblIHQPk,26
 cougar/numpy/functional.py,sha256=ag9K7AfVtZ0GjZMq1T4GCdxh_WGCTvk1TxptbnCyWKQ,1470
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cougar-0.2.19.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cougar-0.2.19.dist-info/METADATA,sha256=TTErKg0LNN7k4fmnGDYq_fsUJj6l4rLm7c5UF6rLhTo,1000
-cougar-0.2.19.dist-info/WHEEL,sha256=qa7UCzQrw0O8LdRePGEUO46f6cYwmvJf5thkdmXZjYY,108
-cougar-0.2.19.dist-info/top_level.txt,sha256=uMu_r6zhlzkRMPivWA_2X6CBTOgkkDTkmliDumvQFCo,13
-cougar-0.2.19.dist-info/RECORD,,
+cougar-0.2.20.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cougar-0.2.20.dist-info/METADATA,sha256=GI1NSmsC_xm5Zg2q9I5yfsp4cxjqeKZvP0gGMqiTBzE,1000
+cougar-0.2.20.dist-info/WHEEL,sha256=qa7UCzQrw0O8LdRePGEUO46f6cYwmvJf5thkdmXZjYY,108
+cougar-0.2.20.dist-info/top_level.txt,sha256=uMu_r6zhlzkRMPivWA_2X6CBTOgkkDTkmliDumvQFCo,13
+cougar-0.2.20.dist-info/RECORD,,
```

