# Comparing `tmp/gazekit-0.0.1-py3-none-any.whl.zip` & `tmp/gazekit-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7438 bytes, number of entries: 15
+Zip file size: 8710 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 10:00 gazekit/__init__.py
 -rw-r--r--  2.0 unx       19 b- defN 23-Aug-03 15:56 gazekit/analyze.py
 -rw-r--r--  2.0 unx     3375 b- defN 23-Aug-04 08:45 gazekit/aoi.py
 -rw-r--r--  2.0 unx      456 b- defN 23-Aug-04 02:09 gazekit/denoise.py
 -rw-r--r--  2.0 unx       31 b- defN 23-Aug-03 07:47 gazekit/hello.py
 -rw-r--r--  2.0 unx       94 b- defN 23-Aug-03 15:56 gazekit/plot.py
 -rw-r--r--  2.0 unx     4443 b- defN 23-Aug-04 05:51 gazekit/sequence.py
 -rw-r--r--  2.0 unx      933 b- defN 23-Aug-04 03:51 gazekit/tools.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 07:43 tests/__init__.py
 -rw-r--r--  2.0 unx     1294 b- defN 23-Aug-04 02:47 tests/test_aoi.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Aug-06 01:48 gazekit-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      327 b- defN 23-Aug-06 01:48 gazekit-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:48 gazekit-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Aug-06 01:48 gazekit-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1110 b- defN 23-Aug-06 01:48 gazekit-0.0.1.dist-info/RECORD
-15 files, 13253 bytes uncompressed, 5620 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx     1065 b- defN 23-Aug-06 01:53 gazekit-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3329 b- defN 23-Aug-06 01:53 gazekit-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 01:53 gazekit-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-06 01:53 gazekit-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Aug-06 01:53 gazekit-0.0.2.dist-info/RECORD
+15 files, 16256 bytes uncompressed, 6892 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_aoi.py
 Comment: 
 
-Filename: gazekit-0.0.1.dist-info/LICENSE
+Filename: gazekit-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: gazekit-0.0.1.dist-info/METADATA
+Filename: gazekit-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gazekit-0.0.1.dist-info/WHEEL
+Filename: gazekit-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gazekit-0.0.1.dist-info/top_level.txt
+Filename: gazekit-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gazekit-0.0.1.dist-info/RECORD
+Filename: gazekit-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gazekit-0.0.1.dist-info/LICENSE` & `gazekit-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gazekit-0.0.1.dist-info/RECORD` & `gazekit-0.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 gazekit/denoise.py,sha256=e-xOUHRI2LUxYork7ZD57XwbO37s54LtPHk_mPpy8VU,456
 gazekit/hello.py,sha256=mHAAo8Ss3ihRoaN8AD2YoCNog3wHWd53gGsms37jXl0,31
 gazekit/plot.py,sha256=JtGdHpqFLgUwtxYEM0czQGVyIY2fdwFGU8xgL2dFBdo,94
 gazekit/sequence.py,sha256=kjvxMxYH17oG_4OHJHGWtoLLfltal1sF9AEYfd-ctUE,4443
 gazekit/tools.py,sha256=8qnXQ7tjdHyZoGsP-JfGpPqMcP1AATzoumxbjijrchc,933
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_aoi.py,sha256=KBmE43GtNKilj239pFSwTp8FgYS9MaIMeyQuD9hu0XM,1294
-gazekit-0.0.1.dist-info/LICENSE,sha256=amVfmFxaa5p_mPTqCX4XnlSyQ6t08fgPR1NCEEM9muY,1065
-gazekit-0.0.1.dist-info/METADATA,sha256=tS_qKbxuxyGZs5ml0aiPhipsM15cP0FULFzrTpMA1CM,327
-gazekit-0.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-gazekit-0.0.1.dist-info/top_level.txt,sha256=0VzJA2kLJJAuufhO3RZ8Bu6HAcc1KhXMCVBkB-20Wxo,14
-gazekit-0.0.1.dist-info/RECORD,,
+gazekit-0.0.2.dist-info/LICENSE,sha256=amVfmFxaa5p_mPTqCX4XnlSyQ6t08fgPR1NCEEM9muY,1065
+gazekit-0.0.2.dist-info/METADATA,sha256=ihX07uo0WhYIDqVg2JzNOl65KKeLoY8_OvNLgnetKp4,3329
+gazekit-0.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+gazekit-0.0.2.dist-info/top_level.txt,sha256=0VzJA2kLJJAuufhO3RZ8Bu6HAcc1KhXMCVBkB-20Wxo,14
+gazekit-0.0.2.dist-info/RECORD,,
```

