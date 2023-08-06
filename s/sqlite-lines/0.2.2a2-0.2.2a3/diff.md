# Comparing `tmp/sqlite_lines-0.2.2a2-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_lines-0.2.2a3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9316 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx    15792 b- defN 23-Aug-06 06:56 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      531 b- defN 23-Aug-06 06:56 sqlite_lines/__init__.py
--rw-r--r--  2.0 unx    21784 b- defN 23-Aug-06 06:56 sqlite_lines/lines0.so
--rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 06:56 sqlite_lines/version.py
--rw-r--r--  2.0 unx      506 b- defN 23-Aug-06 06:56 sqlite_lines-0.2.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Aug-06 06:56 sqlite_lines-0.2.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Aug-06 06:56 sqlite_lines-0.2.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Aug-06 06:56 sqlite_lines-0.2.2a2.dist-info/RECORD
-8 files, 39473 bytes uncompressed, 8164 bytes compressed:  79.3%
+Zip file size: 9318 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx    15792 b- defN 23-Aug-06 07:06 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      531 b- defN 23-Aug-06 07:06 sqlite_lines/__init__.py
+-rw-r--r--  2.0 unx    21784 b- defN 23-Aug-06 07:06 sqlite_lines/lines0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-Aug-06 07:06 sqlite_lines/version.py
+-rw-r--r--  2.0 unx      506 b- defN 23-Aug-06 07:06 sqlite_lines-0.2.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Aug-06 07:06 sqlite_lines-0.2.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Aug-06 07:06 sqlite_lines-0.2.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-Aug-06 07:06 sqlite_lines-0.2.2a3.dist-info/RECORD
+8 files, 39473 bytes uncompressed, 8166 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: sqlite_lines/lines0.so
 Comment: 
 
 Filename: sqlite_lines/version.py
 Comment: 
 
-Filename: sqlite_lines-0.2.2a2.dist-info/METADATA
+Filename: sqlite_lines-0.2.2a3.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_lines-0.2.2a2.dist-info/WHEEL
+Filename: sqlite_lines-0.2.2a3.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_lines-0.2.2a2.dist-info/top_level.txt
+Filename: sqlite_lines-0.2.2a3.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_lines-0.2.2a2.dist-info/RECORD
+Filename: sqlite_lines-0.2.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_lines/lines0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7d446ab6dcee7f58cf53384f4b3ab87a45c432ba
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 1698765bb309dd23538b13fba646fbef00bdb347
```

### strings --all --bytes=8 {}

```diff
@@ -17,17 +17,17 @@
 unable to allocate memory for idxStr
 path argument is required
 Error reading document, size=%d: %s
 Delimiter must be 1 character long, got %d characters
 path is null
 Error reading %s: %s
 CREATE TABLE x(line text,path hidden, delimiter hidden)
-8bd1e1f0016751a6fb2977c0f27c6cec1dd30f7e
-2023-08-06T06:56:38Z+0000
-v0.2.2-alpha.2
+9c87bf7b8971d0778cfa478481c3a9cf60cc0fef
+2023-08-06T07:05:58Z+0000
+v0.2.2-alpha.3
 Version: %s
 Date: %s
 Source: %s
 lines_version
 lines_debug
 lines_read
 Version: %s
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -21,20 +21,20 @@
   0x00003120 25642063 68617261 63746572 73000070 %d characters..p
   0x00003130 61746820 6973206e 756c6c00 4572726f ath is null.Erro
   0x00003140 72207265 6164696e 67202573 3a202573 r reading %s: %s
   0x00003150 00000000 00000000 43524541 54452054 ........CREATE T
   0x00003160 41424c45 2078286c 696e6520 74657874 ABLE x(line text
   0x00003170 2c706174 68206869 6464656e 2c206465 ,path hidden, de
   0x00003180 6c696d69 74657220 68696464 656e2900 limiter hidden).
-  0x00003190 38626431 65316630 30313637 35316136 8bd1e1f0016751a6
-  0x000031a0 66623239 37376330 66323763 36636563 fb2977c0f27c6cec
-  0x000031b0 31646433 30663765 00323032 332d3038 1dd30f7e.2023-08
-  0x000031c0 2d303654 30363a35 363a3338 5a2b3030 -06T06:56:38Z+00
+  0x00003190 39633837 62663762 38393731 64303737 9c87bf7b8971d077
+  0x000031a0 38636661 34373834 38316333 61396366 8cfa478481c3a9cf
+  0x000031b0 36306363 30666566 00323032 332d3038 60cc0fef.2023-08
+  0x000031c0 2d303654 30373a30 353a3538 5a2b3030 -06T07:05:58Z+00
   0x000031d0 30300076 302e322e 322d616c 7068612e 00.v0.2.2-alpha.
-  0x000031e0 32000000 00000000 56657273 696f6e3a 2.......Version:
+  0x000031e0 33000000 00000000 56657273 696f6e3a 3.......Version:
   0x000031f0 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003200 7263653a 20257300 6c696e65 735f7665 rce: %s.lines_ve
   0x00003210 7273696f 6e006c69 6e65735f 64656275 rsion.lines_debu
   0x00003220 67006c69 6e657300 6c696e65 735f7265 g.lines.lines_re
   0x00003230 61640000 00000000 56657273 696f6e3a ad......Version:
   0x00003240 2025730a 44617465 3a202573 0a536f75  %s.Date: %s.Sou
   0x00003250 7263653a 2025730a 4e4f2046 494c4553 rce: %s.NO FILES
```

## sqlite_lines/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.2.2-alpha.2"
+__version__ = "0.2.2-alpha.3"
 __version_info__ = tuple(__version__.split("."))
```

