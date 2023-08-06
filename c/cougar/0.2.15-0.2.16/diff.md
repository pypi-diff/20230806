# Comparing `tmp/cougar-0.2.15-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/cougar-0.2.16-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25264 bytes, number of entries: 10
--rw-r--r--  2.0 unx      287 b- defN 23-Aug-06 06:25 cougar/__init__.py
--rwxr-xr-x  2.0 unx    86456 b- defN 23-Aug-06 06:26 cougar/rolling.cpython-39-darwin.so
--rw-r--r--  2.0 unx       26 b- defN 23-Aug-06 06:25 cougar/numpy/__init__.py
--rw-r--r--  2.0 unx     1470 b- defN 23-Aug-06 06:25 cougar/numpy/functional.py
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 06:25 tests/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-06 06:26 cougar-0.2.15.dist-info/LICENSE
--rw-r--r--  2.0 unx     1000 b- defN 23-Aug-06 06:26 cougar-0.2.15.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Aug-06 06:26 cougar-0.2.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Aug-06 06:26 cougar-0.2.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      788 b- defN 23-Aug-06 06:26 cougar-0.2.15.dist-info/RECORD
-10 files, 101505 bytes uncompressed, 23924 bytes compressed:  76.4%
+Zip file size: 25266 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      287 b- defN 23-Aug-06 06:34 cougar/__init__.py
+-rwxr-xr-x  2.0 unx    86456 b- defN 23-Aug-06 06:34 cougar/rolling.cpython-39-darwin.so
+-rw-r--r--  2.0 unx       26 b- defN 23-Aug-06 06:34 cougar/numpy/__init__.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-Aug-06 06:34 cougar/numpy/functional.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 06:34 tests/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-06 06:34 cougar-0.2.16.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1000 b- defN 23-Aug-06 06:34 cougar-0.2.16.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Aug-06 06:34 cougar-0.2.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Aug-06 06:34 cougar-0.2.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      788 b- defN 23-Aug-06 06:34 cougar-0.2.16.dist-info/RECORD
+10 files, 101505 bytes uncompressed, 23926 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: cougar/numpy/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: cougar-0.2.15.dist-info/LICENSE
+Filename: cougar-0.2.16.dist-info/LICENSE
 Comment: 
 
-Filename: cougar-0.2.15.dist-info/METADATA
+Filename: cougar-0.2.16.dist-info/METADATA
 Comment: 
 
-Filename: cougar-0.2.15.dist-info/WHEEL
+Filename: cougar-0.2.16.dist-info/WHEEL
 Comment: 
 
-Filename: cougar-0.2.15.dist-info/top_level.txt
+Filename: cougar-0.2.16.dist-info/top_level.txt
 Comment: 
 
-Filename: cougar-0.2.15.dist-info/RECORD
+Filename: cougar-0.2.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cougar/rolling.cpython-39-darwin.so

### llvm-readobj --symbols {}

```diff
@@ -258,15 +258,15 @@
   Symbol {
     Name: /Users/runner/work/cougar/cougar/build/temp.macosx-11.7-x86_64-3.9/cougar/rolling.o (963)
     Type: SymDebugTable (0x66)
     Section:  (0x3)
     RefType: ReferenceFlagUndefinedLazy (0x1)
     Flags [ (0x0)
     ]
-    Value: 0x64CF3D15
+    Value: 0x64CF3EF5
   }
   Symbol {
     Name:  (1)
     Type: SymDebugTable (0x2E)
     Section:  (0x1)
     RefType: UndefinedNonLazy (0x0)
     Flags [ (0x0)
```

### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 bundle, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL>*

```diff
@@ -5185,15 +5185,15 @@
 00014400: 5003 0100 0000 0000 5103 0000 0e09 0000  P.......Q.......
 00014410: 8003 0100 0000 0000 6803 0000 0e09 0000  ........h.......
 00014420: b003 0100 0000 0000 8303 0000 0e0a 0000  ................
 00014430: e003 0100 0000 0000 0100 0000 6401 0000  ............d...
 00014440: 0000 0000 0000 0000 9003 0000 6400 0000  ............d...
 00014450: 0000 0000 0000 0000 b903 0000 6400 0000  ............d...
 00014460: 0000 0000 0000 0000 c303 0000 6603 0100  ............f...
-00014470: 153d cf64 0000 0000 0100 0000 2e01 0000  .=.d............
+00014470: f53e cf64 0000 0000 0100 0000 2e01 0000  .>.d............
 00014480: f021 0000 0000 0000 1704 0000 2401 0000  .!..........$...
 00014490: f021 0000 0000 0000 0100 0000 2400 0000  .!..........$...
 000144a0: 0009 0000 0000 0000 0100 0000 4e01 0000  ............N...
 000144b0: f021 0000 0000 0000 0100 0000 2e01 0000  .!..............
 000144c0: f02a 0000 0000 0000 2704 0000 2401 0000  .*......'...$...
 000144d0: f02a 0000 0000 0000 0100 0000 2400 0000  .*..........$...
 000144e0: 2009 0000 0000 0000 0100 0000 4e01 0000   ...........N...
```

## Comparing `cougar-0.2.15.dist-info/LICENSE` & `cougar-0.2.16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cougar-0.2.15.dist-info/METADATA` & `cougar-0.2.16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.2.15
+Version: 0.2.16
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cougar-0.2.15.dist-info/RECORD` & `cougar-0.2.16.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cougar/__init__.py,sha256=j3D3jX-Fn9vgbSAftoZUen46tmJU7TqEO0z8xdikGIE,287
-cougar/rolling.cpython-39-darwin.so,sha256=GtH-Ir2RfgL5lSObq46RXkraa9Nbl__2qUCbElRVaC0,86456
+cougar/rolling.cpython-39-darwin.so,sha256=nFBN7mtuoEq1VcB6enlMIWJAZHHm2xRARDTn_RRuwoE,86456
 cougar/numpy/__init__.py,sha256=QsZLoNOPzs17hbkFTJowo2Ik_wJ55Nl9OreWblIHQPk,26
 cougar/numpy/functional.py,sha256=ag9K7AfVtZ0GjZMq1T4GCdxh_WGCTvk1TxptbnCyWKQ,1470
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cougar-0.2.15.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cougar-0.2.15.dist-info/METADATA,sha256=oaFMRy8M27CT2ROZJHmmmoCKO6cZcu0iYO16_hDPQgE,1000
-cougar-0.2.15.dist-info/WHEEL,sha256=qa7UCzQrw0O8LdRePGEUO46f6cYwmvJf5thkdmXZjYY,108
-cougar-0.2.15.dist-info/top_level.txt,sha256=uMu_r6zhlzkRMPivWA_2X6CBTOgkkDTkmliDumvQFCo,13
-cougar-0.2.15.dist-info/RECORD,,
+cougar-0.2.16.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cougar-0.2.16.dist-info/METADATA,sha256=nT_OYabczjx73ETfy64vvHWuQv-lHGOvUjHPjuwPfts,1000
+cougar-0.2.16.dist-info/WHEEL,sha256=qa7UCzQrw0O8LdRePGEUO46f6cYwmvJf5thkdmXZjYY,108
+cougar-0.2.16.dist-info/top_level.txt,sha256=uMu_r6zhlzkRMPivWA_2X6CBTOgkkDTkmliDumvQFCo,13
+cougar-0.2.16.dist-info/RECORD,,
```

