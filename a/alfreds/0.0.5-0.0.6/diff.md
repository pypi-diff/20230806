# Comparing `tmp/alfreds-0.0.5-py3-none-any.whl.zip` & `tmp/alfreds-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 7799 bytes, number of entries: 19
--rwxr-xr-x  2.0 unx     2616 b- defN 23-Aug-06 08:13 alfreds-0.0.5.data/scripts/alfreds
--rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.5.data/scripts/main.py
+Zip file size: 8369 bytes, number of entries: 19
+-rwxr-xr-x  2.0 unx     2616 b- defN 23-Aug-06 08:15 alfreds-0.0.6.data/scripts/alfreds
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Aug-03 10:35 alfreds-0.0.6.data/scripts/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_init/__init__.py
 -rw-r--r--  2.0 unx     6598 b- defN 23-Aug-06 08:07 alfreds_init/init.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_seed/__init__.py
 -rw-r--r--  2.0 unx      889 b- defN 23-Aug-04 11:07 alfreds_seed/seed.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_start/__init__.py
 -rw-r--r--  2.0 unx      880 b- defN 23-Aug-05 07:22 alfreds_start/start.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_stop/__init__.py
 -rw-r--r--  2.0 unx      139 b- defN 23-Aug-04 11:07 alfreds_stop/stop.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-04 11:07 alfreds_update/__init__.py
 -rw-r--r--  2.0 unx     1022 b- defN 23-Aug-04 11:07 alfreds_update/update_agent.py
 -rw-r--r--  2.0 unx      990 b- defN 23-Aug-04 11:07 alfreds_update/update_working_directory.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-05 08:02 refresh/__init__.py
 -rw-r--r--  2.0 unx      484 b- defN 23-Aug-05 08:04 refresh/refresh.py
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-06 08:13 alfreds-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 08:13 alfreds-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 23-Aug-06 08:13 alfreds-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1509 b- defN 23-Aug-06 08:13 alfreds-0.0.5.dist-info/RECORD
-19 files, 15795 bytes uncompressed, 5313 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2226 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       76 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-Aug-06 08:15 alfreds-0.0.6.dist-info/RECORD
+19 files, 17536 bytes uncompressed, 5883 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: alfreds-0.0.5.data/scripts/alfreds
+Filename: alfreds-0.0.6.data/scripts/alfreds
 Comment: 
 
-Filename: alfreds-0.0.5.data/scripts/main.py
+Filename: alfreds-0.0.6.data/scripts/main.py
 Comment: 
 
 Filename: alfreds_init/__init__.py
 Comment: 
 
 Filename: alfreds_init/init.py
 Comment: 
@@ -39,20 +39,20 @@
 
 Filename: refresh/__init__.py
 Comment: 
 
 Filename: refresh/refresh.py
 Comment: 
 
-Filename: alfreds-0.0.5.dist-info/METADATA
+Filename: alfreds-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: alfreds-0.0.5.dist-info/WHEEL
+Filename: alfreds-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: alfreds-0.0.5.dist-info/top_level.txt
+Filename: alfreds-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: alfreds-0.0.5.dist-info/RECORD
+Filename: alfreds-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `alfreds-0.0.5.data/scripts/alfreds` & `alfreds-0.0.6.data/scripts/alfreds`

 * *Files identical despite different names*

## Comparing `alfreds-0.0.5.dist-info/RECORD` & `alfreds-0.0.6.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-alfreds-0.0.5.data/scripts/alfreds,sha256=rK_vo1SjqlUoR6UBhPSJ5X8sxE2f1YGJKyhn_BsffYQ,2616
-alfreds-0.0.5.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
+alfreds-0.0.6.data/scripts/alfreds,sha256=rK_vo1SjqlUoR6UBhPSJ5X8sxE2f1YGJKyhn_BsffYQ,2616
+alfreds-0.0.6.data/scripts/main.py,sha256=lX4TwHMuSP1Ulvk1iU3JOp2n3NXrj_6lJkb98XjNodE,14
 alfreds_init/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_init/init.py,sha256=tL-bT_cDy1CBTVoVZrwaoAR9CB0_3xpPJ7V1HwN_2yY,6598
 alfreds_seed/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_seed/seed.py,sha256=FLqIgMCJWW8cb6KB7dtstioRW8wdzgKMq_wXiwbO5q4,889
 alfreds_start/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_start/start.py,sha256=YN4VjOKWkNdmUp-BuLChUnqsUOARPoWKoDZ-upEAqk4,880
 alfreds_stop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_stop/stop.py,sha256=T3klfHF8boqT4HpW_7ARtAg8Lql4GgZaK6O4Cm_8OAs,139
 alfreds_update/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 alfreds_update/update_agent.py,sha256=D3-8uk_cKXmiCAFmd-2ib0n8YwmUSOvxgxqCUrWxXQA,1022
 alfreds_update/update_working_directory.py,sha256=IXQp4NYh-IGsgC2Hnl9mbOFPXhtnOJX1hqfO5Ta6iEo,990
 refresh/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 refresh/refresh.py,sha256=MtuP8GmB9Sf4ODYc7UnqeadFkbHTJmI4h12Qy_-T_eU,484
-alfreds-0.0.5.dist-info/METADATA,sha256=XUYvwzru_R17zqQQ81-CqB0TEayIBneZVOyE2Wm99EE,486
-alfreds-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-alfreds-0.0.5.dist-info/top_level.txt,sha256=6Mb9L3LAWttfLTf738HUv9jpgLoTAOFPL7PgL-5cUY0,76
-alfreds-0.0.5.dist-info/RECORD,,
+alfreds-0.0.6.dist-info/METADATA,sha256=owsIRFTXn1eT6SALPGULkSrhLR8scx31b7JJnL_ZpC8,2226
+alfreds-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+alfreds-0.0.6.dist-info/top_level.txt,sha256=6Mb9L3LAWttfLTf738HUv9jpgLoTAOFPL7PgL-5cUY0,76
+alfreds-0.0.6.dist-info/RECORD,,
```

