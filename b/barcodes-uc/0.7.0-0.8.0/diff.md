# Comparing `tmp/barcodes_uc-0.7.0.tar.gz` & `tmp/barcodes_uc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcodes_uc-0.7.0.tar", max compression
+gzip compressed data, was "barcodes_uc-0.8.0.tar", max compression
```

## Comparing `barcodes_uc-0.7.0.tar` & `barcodes_uc-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2205 2023-08-03 12:22:12.415990 barcodes_uc-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.7.0/barcodes_uc/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.7.0/barcodes_uc/barcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.7.0/barcodes_uc/barcodes/__main__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__init__.py
--rw-r--r--   0        0        0     3115 2023-08-03 11:22:38.779125 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__main__.py
--rw-r--r--   0        0        0      189 2023-07-13 15:35:12.454179 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      171 2023-07-14 13:34:11.240069 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4345 2023-08-03 11:22:41.098823 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0    21823 2023-08-05 07:20:03.074297 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-311.pyc
--rw-r--r--   0        0        0     8909 2023-08-03 08:10:47.508145 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-39.pyc
--rw-r--r--   0        0        0    26257 2023-07-14 13:33:49.056641 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-311.pyc
--rw-r--r--   0        0        0    15979 2023-07-25 21:47:17.851848 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-39.pyc
--rw-r--r--   0        0        0    55776 2023-08-05 07:20:03.036280 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-311.pyc
--rw-r--r--   0        0        0    20967 2023-08-03 08:54:56.822508 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-39.pyc
--rw-r--r--   0        0        0    15054 2023-08-05 07:19:23.305411 barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrgenerator.py
--rw-r--r--   0        0        0    51478 2023-08-05 07:19:58.290195 barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrutils.py
--rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.7.0/data/GF256.csv
--rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.7.0/data/alignment_locations.csv
--rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.7.0/data/capabilities.csv
--rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.7.0/data/error_correction_table.csv
--rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.7.0/data/format_table.csv
--rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.7.0/data/version_table.csv
--rw-r--r--   0        0        0      671 2023-08-05 07:20:50.235659 barcodes_uc-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10489 2023-08-05 06:51:06.168501 barcodes_uc-0.7.0/requirements.txt
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 barcodes_uc-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2205 2023-08-03 12:22:12.415990 barcodes_uc-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.8.0/barcodes_uc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.8.0/barcodes_uc/barcodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.8.0/barcodes_uc/barcodes/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__init__.py
+-rw-r--r--   0        0        0     3115 2023-08-03 11:22:38.779125 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__main__.py
+-rw-r--r--   0        0        0      189 2023-07-13 15:35:12.454179 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      171 2023-07-14 13:34:11.240069 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4345 2023-08-03 11:22:41.098823 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0    21977 2023-08-05 09:40:40.676858 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-311.pyc
+-rw-r--r--   0        0        0     8909 2023-08-03 08:10:47.508145 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-39.pyc
+-rw-r--r--   0        0        0    26257 2023-07-14 13:33:49.056641 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-311.pyc
+-rw-r--r--   0        0        0    15979 2023-07-25 21:47:17.851848 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-39.pyc
+-rw-r--r--   0        0        0    56007 2023-08-05 09:39:47.858959 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-311.pyc
+-rw-r--r--   0        0        0    20967 2023-08-03 08:54:56.822508 barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-39.pyc
+-rw-r--r--   0        0        0    15201 2023-08-05 09:40:37.457293 barcodes_uc-0.8.0/barcodes_uc/qrcodes/qrgenerator.py
+-rw-r--r--   0        0        0    51646 2023-08-05 09:36:11.381533 barcodes_uc-0.8.0/barcodes_uc/qrcodes/qrutils.py
+-rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.8.0/data/GF256.csv
+-rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.8.0/data/alignment_locations.csv
+-rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.8.0/data/capabilities.csv
+-rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.8.0/data/error_correction_table.csv
+-rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.8.0/data/format_table.csv
+-rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.8.0/data/version_table.csv
+-rw-r--r--   0        0        0      671 2023-08-05 09:51:10.283947 barcodes_uc-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10489 2023-08-05 06:51:06.168501 barcodes_uc-0.8.0/requirements.txt
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 barcodes_uc-0.8.0/PKG-INFO
```

### Comparing `barcodes_uc-0.7.0/README.md` & `barcodes_uc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__main__.py` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__main__.py`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__main__.cpython-311.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/__main__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-311.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xfbf7cd64 (Sat Aug  5 07:19:23 2023 UTC)
-files sz: 15054
+moddate:  0x1519ce64 (Sat Aug  5 09:40:37 2023 UTC)
+files sz: 15201
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a010100640264036c026d035a030100640264
@@ -145,22 +145,22 @@
                236 LOAD_CONST              20 (<code object QRGenerator, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 164>)
                238 MAKE_FUNCTION            0
                240 LOAD_CONST              21 ('QRGenerator')
                242 PRECALL                  2
                246 CALL                     2
                256 STORE_NAME              14 (QRGenerator)
    
-   364         258 LOAD_CONST              22 ('msg')
+   367         258 LOAD_CONST              22 ('msg')
                260 LOAD_NAME               15 (str)
                262 BUILD_TUPLE              2
-               264 LOAD_CONST              23 (<code object get_encoding, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 364>)
+               264 LOAD_CONST              23 (<code object get_encoding, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 367>)
                266 MAKE_FUNCTION            4 (annotations)
                268 STORE_NAME              16 (get_encoding)
    
-   379         270 LOAD_NAME                1 (qrutils)
+   382         270 LOAD_NAME                1 (qrutils)
                272 LOAD_ATTR               17 (QREncoding)
                282 LOAD_ATTR               18 (byte)
                292 LOAD_NAME                1 (qrutils)
                294 LOAD_ATTR               19 (QRErrorCorrectionLevels)
                304 LOAD_ATTR               20 (Q)
                314 BUILD_TUPLE              2
                316 LOAD_CONST              22 ('msg')
@@ -168,29 +168,29 @@
                320 LOAD_CONST              24 ('encoding')
                322 LOAD_NAME                1 (qrutils)
                324 LOAD_ATTR               17 (QREncoding)
                334 LOAD_CONST              25 ('error_correction')
                336 LOAD_NAME                1 (qrutils)
                338 LOAD_ATTR               19 (QRErrorCorrectionLevels)
                348 BUILD_TUPLE              6
-               350 LOAD_CONST              26 (<code object get_min_version, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 379>)
+               350 LOAD_CONST              26 (<code object get_min_version, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 382>)
                352 MAKE_FUNCTION            5 (defaults, annotations)
                354 STORE_NAME              21 (get_min_version)
    
-   390         356 LOAD_NAME                1 (qrutils)
+   393         356 LOAD_NAME                1 (qrutils)
                358 LOAD_ATTR               19 (QRErrorCorrectionLevels)
                368 LOAD_ATTR               20 (Q)
                378 BUILD_TUPLE              1
                380 LOAD_CONST              22 ('msg')
                382 LOAD_NAME               15 (str)
                384 LOAD_CONST              25 ('error_correction')
                386 LOAD_NAME                1 (qrutils)
                388 LOAD_ATTR               19 (QRErrorCorrectionLevels)
                398 BUILD_TUPLE              4
-               400 LOAD_CONST              27 (<code object smallest_qr, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 390>)
+               400 LOAD_CONST              27 (<code object smallest_qr, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 393>)
                402 MAKE_FUNCTION            5 (defaults, annotations)
                404 STORE_NAME              22 (smallest_qr)
                406 LOAD_CONST               4 (None)
                408 RETURN_VALUE
    consts
       1
       ('qrutils',)
@@ -1942,15 +1942,15 @@
          flags     : 0
          code
             0x970065005a0164005a02640165036a0400000000000000006a05000000
             000000000065036a0600000000000000006a07000000000000000065036a
             0800000000000000006a09000000000000000066046402650a640365036a
             040000000000000000640465036a060000000000000000640565036a0800
             000000000000006608640684055a0b640784005a0c640884005a0d640984
-            005a0e640a84005a0f640b5300
+            005a0e640e640b650f6602640c84055a10640d5300
          164           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('QRGenerator')
                        8 STORE_NAME               2 (__qualname__)
          
          165          10 LOAD_CONST               1 ('Hello World')
@@ -1988,19 +1988,23 @@
                      142 MAKE_FUNCTION            0
                      144 STORE_NAME              13 (__repr__)
          
          177         146 LOAD_CONST               9 (<code object check, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 177>)
                      148 MAKE_FUNCTION            0
                      150 STORE_NAME              14 (check)
          
-         185         152 LOAD_CONST              10 (<code object generate, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 185>)
-                     154 MAKE_FUNCTION            0
-                     156 STORE_NAME              15 (generate)
-                     158 LOAD_CONST              11 (None)
-                     160 RETURN_VALUE
+         185         152 LOAD_CONST              14 ((False,))
+                     154 LOAD_CONST              11 ('returnALL')
+                     156 LOAD_NAME               15 (bool)
+                     158 BUILD_TUPLE              2
+                     160 LOAD_CONST              12 (<code object generate, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py", line 185>)
+                     162 MAKE_FUNCTION            5 (defaults, annotations)
+                     164 STORE_NAME              16 (generate)
+                     166 LOAD_CONST              13 (None)
+                     168 RETURN_VALUE
          consts
             'QRGenerator'
             'Hello World'
             'msg'
             'encoding'
             'version'
             'error_correction'
@@ -2187,618 +2191,621 @@
                varnames   ('self', 'max_character_count')
                freevars   ()
                cellvars   ()
                filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
                name       'check'
                firstlineno 177
                lnotab 0x0201880230010402
+            False
+            'returnALL'
             code
-               argcount  : 1
-               nlocals   : 17
+               argcount  : 2
+               nlocals   : 20
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   000000000000007c006a0300000000000000007c006a0400000000000000
-                  007c006a050000000000000000a6040000ab0400000000000000007d0174
-                  01000000000000000000006a0600000000000000007c0164011900000000
-                  00000000007c016402190000000000000000007c006a0200000000000000
-                  00a6030000ab0300000000000000007d026403a007000000000000000000
-                  00000000000000000000007c02a6010000ab0100000000000000007d0274
+                  007c006a050000000000000000a6040000ab0400000000000000007d0274
+                  01000000000000000000006a0600000000000000007c0264011900000000
+                  00000000007c026402190000000000000000007c006a0200000000000000
+                  00a6030000ab0300000000000000007d036403a007000000000000000000
+                  00000000000000000000007c03a6010000ab0100000000000000007d0374
                   11000000000000000000007c006a0200000000000000007c006a03000000
                   00000000007c006a0500000000000000007c006a040000000000000000ac
-                  04a6040000ab0400000000000000007d0374130000000000000000000074
+                  04a6040000ab0400000000000000007d0474130000000000000000000074
                   1400000000000000000000a6010000ab01000000000000000044005d2a5c
-                  0200007d047d057413000000000000000000007c05a6010000ab01000000
-                  000000000044005d155c0200007d067d077c077c036a0b00000000000000
-                  007c04190000000000000000007c063c0000008c168c2b74130000000000
+                  0200007d057d067413000000000000000000007c06a6010000ab01000000
+                  000000000044005d155c0200007d077d087c087c046a0b00000000000000
+                  007c05190000000000000000007c073c0000008c168c2b74130000000000
                   0000000000741400000000000000000000a6010000ab0100000000000000
-                  0044005d355c0200007d047d057413000000000000000000007c05a60100
-                  00ab01000000000000000044005d205c0200007d067d077c077c036a0b00
-                  000000000000007c04190000000000000000007c036a0c00000000000000
-                  0064057a0a00007c067a0000003c0000008c218c36741300000000000000
+                  0044005d355c0200007d057d067413000000000000000000007c06a60100
+                  00ab01000000000000000044005d205c0200007d077d087c087c046a0b00
+                  000000000000007c05190000000000000000007c046a0c00000000000000
+                  0064057a0a00007c077a0000003c0000008c218c36741300000000000000
                   000000741400000000000000000000a6010000ab01000000000000000044
-                  005d355c0200007d047d057413000000000000000000007c05a6010000ab
-                  01000000000000000044005d205c0200007d067d077c077c036a0b000000
-                  00000000007c036a0c000000000000000064057a0a00007c047a00000019
-                  0000000000000000007c063c0000008c218c36741b000000000000000000
-                  006406a6010000ab01000000000000000044005d127d0864077c036a0b00
-                  000000000000007c081900000000000000000064053c0000008c13741b00
+                  005d355c0200007d057d067413000000000000000000007c06a6010000ab
+                  01000000000000000044005d205c0200007d077d087c087c046a0b000000
+                  00000000007c046a0c000000000000000064057a0a00007c057a00000019
+                  0000000000000000007c073c0000008c218c36741b000000000000000000
+                  006406a6010000ab01000000000000000044005d127d0964077c046a0b00
+                  000000000000007c091900000000000000000064053c0000008c13741b00
                   0000000000000000006406a6010000ab01000000000000000044005d127d
-                  0864077c036a0b00000000000000006405190000000000000000007c083c
+                  0964077c046a0b00000000000000006405190000000000000000007c093c
                   0000008c13741b000000000000000000006406a6010000ab010000000000
-                  00000044005d1a7d0864077c036a0b00000000000000007c081900000000
-                  00000000007c036a0c000000000000000064067a0a00003c0000008c1b74
+                  00000044005d1a7d0964077c046a0b00000000000000007c091900000000
+                  00000000007c046a0c000000000000000064067a0a00003c0000008c1b74
                   1b000000000000000000006406a6010000ab01000000000000000044005d
-                  1d7d0864077c036a0b00000000000000006405190000000000000000007c
-                  036a0c000000000000000064087a0a00007c087a0a00003c0000008c1e74
+                  1d7d0964077c046a0b00000000000000006405190000000000000000007c
+                  046a0c000000000000000064087a0a00007c097a0a00003c0000008c1e74
                   1b000000000000000000006406a6010000ab01000000000000000044005d
-                  1d7d0864077c036a0b00000000000000007c036a0c000000000000000064
-                  067a0a00007c087a0000001900000000000000000064053c0000008c1e74
+                  1d7d0964077c046a0b00000000000000007c046a0c000000000000000064
+                  067a0a00007c097a0000001900000000000000000064053c0000008c1e74
                   1b000000000000000000006406a6010000ab01000000000000000044005d
-                  1a7d0864077c036a0b00000000000000007c036a0c000000000000000064
-                  067a0a0000190000000000000000007c083c0000008c1b64087d09741b00
-                  00000000000000000064067c036a0c000000000000000064067a0a0000a6
-                  020000ab02000000000000000044005d1a7d087c0964097a0600007c036a
-                  0b0000000000000000640a190000000000000000007c083c0000007c0964
-                  087a0d00007d098c1b64087d09741b0000000000000000000064067c036a
+                  1a7d0964077c046a0b00000000000000007c046a0c000000000000000064
+                  067a0a0000190000000000000000007c093c0000008c1b64087d0a741b00
+                  00000000000000000064067c046a0c000000000000000064067a0a0000a6
+                  020000ab02000000000000000044005d1a7d097c0a64097a0600007c046a
+                  0b0000000000000000640a190000000000000000007c093c0000007c0a64
+                  087a0d00007d0a8c1b64087d0a741b0000000000000000000064067c046a
                   0c000000000000000064067a0a0000a6020000ab02000000000000000044
-                  005d1a7d087c0964097a0600007c036a0b00000000000000007c08190000
-                  00000000000000640a3c0000007c0964087a0d00007d098c1b7401000000
+                  005d1a7d097c0a64097a0600007c046a0b00000000000000007c09190000
+                  00000000000000640a3c0000007c0a64087a0d00007d0a8c1b7401000000
                   000000000000006a0e00000000000000007c006a020000000000000000a6
-                  010000ab0100000000000000007d0a7c0a44005d6d7d0b7c0b6407190000
-                  000000000000007d047c0b6408190000000000000000007d066700640ba2
-                  017d0c741b00000000000000000000640ca6010000ab0100000000000000
-                  0044005d477d08741b00000000000000000000640ca6010000ab01000000
-                  000000000044005d357d0d741e000000000000000000007c081900000000
-                  00000000007c0d190000000000000000007c036a0b00000000000000007c
-                  047c0c7c08190000000000000000007a000000190000000000000000007c
-                  067c0c7c0d190000000000000000007a0000003c0000008c368c488c6e64
-                  087c036a0b00000000000000007c036a0c000000000000000064067a0a00
+                  010000ab0100000000000000007d0b7c0b44005d6d7d0c7c0c6407190000
+                  000000000000007d057c0c6408190000000000000000007d076700640ba2
+                  017d0d741b00000000000000000000640ca6010000ab0100000000000000
+                  0044005d477d09741b00000000000000000000640ca6010000ab01000000
+                  000000000044005d357d0e741e000000000000000000007c091900000000
+                  00000000007c0e190000000000000000007c046a0b00000000000000007c
+                  057c0d7c09190000000000000000007a000000190000000000000000007c
+                  077c0d7c0e190000000000000000007a0000003c0000008c368c488c6e64
+                  087c046a0b00000000000000007c046a0c000000000000000064067a0a00
                   001900000000000000000064063c000000741b0000000000000000000064
-                  0da6010000ab01000000000000000044005d187d087c08640a6b03000000
-                  007210640e7c036a0b00000000000000007c081900000000000000000064
+                  0da6010000ab01000000000000000044005d187d097c09640a6b03000000
+                  007210640e7c046a0b00000000000000007c091900000000000000000064
                   063c0000008c19741b00000000000000000000640da6010000ab01000000
-                  000000000044005d187d087c08640a6b03000000007210640e7c036a0b00
-                  000000000000006406190000000000000000007c083c0000008c19741b00
+                  000000000044005d187d097c09640a6b03000000007210640e7c046a0b00
+                  000000000000006406190000000000000000007c093c0000008c19741b00
                   0000000000000000006408640da6020000ab02000000000000000044005d
-                  1a7d08640e7c036a0b00000000000000006406190000000000000000007c
-                  036a0c00000000000000007c087a0a00003c0000008c1b741b0000000000
-                  000000000064086406a6020000ab02000000000000000044005d1a7d0864
-                  0e7c036a0b00000000000000007c036a0c00000000000000007c087a0a00
+                  1a7d09640e7c046a0b00000000000000006406190000000000000000007c
+                  046a0c00000000000000007c097a0a00003c0000008c1b741b0000000000
+                  000000000064086406a6020000ab02000000000000000044005d1a7d0964
+                  0e7c046a0b00000000000000007c046a0c00000000000000007c097a0a00
                   001900000000000000000064063c0000008c1b7c006a0200000000000000
                   006a1000000000000000007400000000000000000000006a110000000000
                   0000006a1200000000000000006a1000000000000000006b050000000072
                   5a741b00000000000000000000640aa6010000ab01000000000000000044
-                  005d4a7d08741b00000000000000000000640fa6010000ab010000000000
-                  00000044005d387d0d640e7c036a0b00000000000000007c081900000000
-                  00000000007c036a0c000000000000000064107a0a00007c0d7a0000003c
-                  000000640e7c036a0b00000000000000007c036a0c000000000000000064
-                  107a0a00007c0d7a000000190000000000000000007c083c0000008c398c
-                  4b7413000000000000000000007c036a0b0000000000000000a6010000ab
-                  01000000000000000044005d305c0200007d047d05741300000000000000
-                  0000007c05a6010000ab01000000000000000044005d1b5c0200007d067d
-                  077c0764116b0300000000721064087c036a1300000000000000007c0419
-                  0000000000000000007c063c0000008c1c8c317c036a0c00000000000000
-                  0064087a0a00007d047c036a0c000000000000000064087a0a00007d0664
-                  087d0e64087d0f64077d107c107429000000000000000000007c02a60100
-                  00ab0100000000000000006b000000000072ef7c036a0b00000000000000
-                  007c04190000000000000000007c061900000000000000000064116b0200
-                  000000721b7c027c10190000000000000000007c036a0b00000000000000
-                  007c04190000000000000000007c063c0000007c1064087a0d00007d107c
-                  0e64086b0200000000720e7c0f64086b020000000072087c0664087a1700
-                  007d0664127d0f6e457c0e64086b020000000072137c0f64126b02000000
-                  00720d7c0464087a1700007d047c0664087a0d00007d0664087d0f6e2c7c
-                  0e64126b0200000000720e7c0f64086b020000000072087c0664087a1700
-                  007d0664127d0f6e187c0e64126b020000000072127c0f64126b02000000
-                  00720c7c0664087a0d00007d067c0464087a0d00007d0464087d0f7c0464
-                  126b0200000000720c64127d0e64077d0464087d0f7c0664097a1700007d
-                  066e1e7c047c036a0c00000000000000006b0200000000721364087d0e7c
-                  036a0c000000000000000064087a0a00007d0464087d0f7c0664097a1700
-                  007d067c06640a6b020000000072057c0664087a1700007d067c0664076b
+                  005d4a7d09741b00000000000000000000640fa6010000ab010000000000
+                  00000044005d387d0e640e7c046a0b00000000000000007c091900000000
+                  00000000007c046a0c000000000000000064107a0a00007c0e7a0000003c
+                  000000640e7c046a0b00000000000000007c046a0c000000000000000064
+                  107a0a00007c0e7a000000190000000000000000007c093c0000008c398c
+                  4b7413000000000000000000007c046a0b0000000000000000a6010000ab
+                  01000000000000000044005d305c0200007d057d06741300000000000000
+                  0000007c06a6010000ab01000000000000000044005d1b5c0200007d077d
+                  087c0864116b0300000000721064087c046a1300000000000000007c0519
+                  0000000000000000007c073c0000008c1c8c317c046a0c00000000000000
+                  0064087a0a00007d057c046a0c000000000000000064087a0a00007d0764
+                  087d0f64087d1064077d117c117429000000000000000000007c03a60100
+                  00ab0100000000000000006b000000000072ef7c046a0b00000000000000
+                  007c05190000000000000000007c071900000000000000000064116b0200
+                  000000721b7c037c11190000000000000000007c046a0b00000000000000
+                  007c05190000000000000000007c073c0000007c1164087a0d00007d117c
+                  0f64086b0200000000720e7c1064086b020000000072087c0764087a1700
+                  007d0764127d106e457c0f64086b020000000072137c1064126b02000000
+                  00720d7c0564087a1700007d057c0764087a0d00007d0764087d106e2c7c
+                  0f64126b0200000000720e7c1064086b020000000072087c0764087a1700
+                  007d0764127d106e187c0f64126b020000000072127c1064126b02000000
+                  00720c7c0764087a0d00007d077c0564087a0d00007d0564087d107c0564
+                  126b0200000000720c64127d0f64077d0564087d107c0764097a1700007d
+                  076e1e7c057c046a0c00000000000000006b0200000000721364087d0f7c
+                  046a0c000000000000000064087a0a00007d0564087d107c0764097a1700
+                  007d077c07640a6b020000000072057c0764087a1700007d077c0764076b
                   00000000007210742b000000000000000000006413a6010000ab01000000
-                  000000000001006e137c107429000000000000000000007c02a6010000ab
+                  000000000001006e137c117429000000000000000000007c03a6010000ab
                   0100000000000000006b0000000000b0ef7401000000000000000000006a
-                  1600000000000000007c036a0b00000000000000007c036a130000000000
+                  1600000000000000007c046a0b00000000000000007c046a130000000000
                   0000007c006a0400000000000000007c006a020000000000000000a60400
-                  00ab0400000000000000007c035f0b00000000000000007c035300
+                  00ab0400000000000000005c0300007c045f0b00000000000000007d127d
+                  137c0172057c047c127c13660353007c045300
                185           0 RESUME                   0
                
                188           2 LOAD_GLOBAL              1 (NULL + qrutils)
                             14 LOAD_ATTR                1 (qr_encode_data)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (version)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (encoding)
                             48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                4 (error_correction)
                             60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                5 (msg)
                             72 PRECALL                  4
                             76 CALL                     4
-                            86 STORE_FAST               1 (rawData)
+                            86 STORE_FAST               2 (rawData)
                
                192          88 LOAD_GLOBAL              1 (NULL + qrutils)
                            100 LOAD_ATTR                6 (interleave_blocks)
-                           110 LOAD_FAST                1 (rawData)
+                           110 LOAD_FAST                2 (rawData)
                            112 LOAD_CONST               1 ('dataBytes')
                            114 BINARY_SUBSCR
-                           124 LOAD_FAST                1 (rawData)
+                           124 LOAD_FAST                2 (rawData)
                            126 LOAD_CONST               2 ('ErrorCorrection')
                            128 BINARY_SUBSCR
                            138 LOAD_FAST                0 (self)
                            140 LOAD_ATTR                2 (version)
                            150 PRECALL                  3
                            154 CALL                     3
-                           164 STORE_FAST               2 (interleavedData)
+                           164 STORE_FAST               3 (interleavedData)
                
                194         166 LOAD_CONST               3 ('')
                            168 LOAD_METHOD              7 (join)
-                           190 LOAD_FAST                2 (interleavedData)
+                           190 LOAD_FAST                3 (interleavedData)
                            192 PRECALL                  1
                            196 CALL                     1
-                           206 STORE_FAST               2 (interleavedData)
+                           206 STORE_FAST               3 (interleavedData)
                
                197         208 LOAD_GLOBAL             17 (NULL + QR)
                            220 LOAD_FAST                0 (self)
                            222 LOAD_ATTR                2 (version)
                            232 LOAD_FAST                0 (self)
                            234 LOAD_ATTR                3 (encoding)
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                5 (msg)
                            256 LOAD_FAST                0 (self)
                            258 LOAD_ATTR                4 (error_correction)
                            268 KW_NAMES                 4
                            270 PRECALL                  4
                            274 CALL                     4
-                           284 STORE_FAST               3 (qr)
+                           284 STORE_FAST               4 (qr)
                
                202         286 LOAD_GLOBAL             19 (NULL + enumerate)
                            298 LOAD_GLOBAL             20 (finderPattern)
                            310 PRECALL                  1
                            314 CALL                     1
                            324 GET_ITER
                        >>  326 FOR_ITER                42 (to 412)
                            328 UNPACK_SEQUENCE          2
-                           332 STORE_FAST               4 (posx)
-                           334 STORE_FAST               5 (row)
+                           332 STORE_FAST               5 (posx)
+                           334 STORE_FAST               6 (row)
                
                203         336 LOAD_GLOBAL             19 (NULL + enumerate)
-                           348 LOAD_FAST                5 (row)
+                           348 LOAD_FAST                6 (row)
                            350 PRECALL                  1
                            354 CALL                     1
                            364 GET_ITER
                        >>  366 FOR_ITER                21 (to 410)
                            368 UNPACK_SEQUENCE          2
-                           372 STORE_FAST               6 (posy)
-                           374 STORE_FAST               7 (col)
+                           372 STORE_FAST               7 (posy)
+                           374 STORE_FAST               8 (col)
                
-               204         376 LOAD_FAST                7 (col)
-                           378 LOAD_FAST                3 (qr)
+               204         376 LOAD_FAST                8 (col)
+                           378 LOAD_FAST                4 (qr)
                            380 LOAD_ATTR               11 (matrix)
-                           390 LOAD_FAST                4 (posx)
+                           390 LOAD_FAST                5 (posx)
                            392 BINARY_SUBSCR
-                           402 LOAD_FAST                6 (posy)
+                           402 LOAD_FAST                7 (posy)
                            404 STORE_SUBSCR
                            408 JUMP_BACKWARD           22 (to 366)
                
                203     >>  410 JUMP_BACKWARD           43 (to 326)
                
                207     >>  412 LOAD_GLOBAL             19 (NULL + enumerate)
                            424 LOAD_GLOBAL             20 (finderPattern)
                            436 PRECALL                  1
                            440 CALL                     1
                            450 GET_ITER
                        >>  452 FOR_ITER                53 (to 560)
                            454 UNPACK_SEQUENCE          2
-                           458 STORE_FAST               4 (posx)
-                           460 STORE_FAST               5 (row)
+                           458 STORE_FAST               5 (posx)
+                           460 STORE_FAST               6 (row)
                
                208         462 LOAD_GLOBAL             19 (NULL + enumerate)
-                           474 LOAD_FAST                5 (row)
+                           474 LOAD_FAST                6 (row)
                            476 PRECALL                  1
                            480 CALL                     1
                            490 GET_ITER
                        >>  492 FOR_ITER                32 (to 558)
                            494 UNPACK_SEQUENCE          2
-                           498 STORE_FAST               6 (posy)
-                           500 STORE_FAST               7 (col)
+                           498 STORE_FAST               7 (posy)
+                           500 STORE_FAST               8 (col)
                
-               209         502 LOAD_FAST                7 (col)
-                           504 LOAD_FAST                3 (qr)
+               209         502 LOAD_FAST                8 (col)
+                           504 LOAD_FAST                4 (qr)
                            506 LOAD_ATTR               11 (matrix)
-                           516 LOAD_FAST                4 (posx)
+                           516 LOAD_FAST                5 (posx)
                            518 BINARY_SUBSCR
-                           528 LOAD_FAST                3 (qr)
+                           528 LOAD_FAST                4 (qr)
                            530 LOAD_ATTR               12 (size)
                            540 LOAD_CONST               5 (7)
                            542 BINARY_OP               10 (-)
-                           546 LOAD_FAST                6 (posy)
+                           546 LOAD_FAST                7 (posy)
                            548 BINARY_OP                0 (+)
                            552 STORE_SUBSCR
                            556 JUMP_BACKWARD           33 (to 492)
                
                208     >>  558 JUMP_BACKWARD           54 (to 452)
                
                212     >>  560 LOAD_GLOBAL             19 (NULL + enumerate)
                            572 LOAD_GLOBAL             20 (finderPattern)
                            584 PRECALL                  1
                            588 CALL                     1
                            598 GET_ITER
                        >>  600 FOR_ITER                53 (to 708)
                            602 UNPACK_SEQUENCE          2
-                           606 STORE_FAST               4 (posx)
-                           608 STORE_FAST               5 (row)
+                           606 STORE_FAST               5 (posx)
+                           608 STORE_FAST               6 (row)
                
                213         610 LOAD_GLOBAL             19 (NULL + enumerate)
-                           622 LOAD_FAST                5 (row)
+                           622 LOAD_FAST                6 (row)
                            624 PRECALL                  1
                            628 CALL                     1
                            638 GET_ITER
                        >>  640 FOR_ITER                32 (to 706)
                            642 UNPACK_SEQUENCE          2
-                           646 STORE_FAST               6 (posy)
-                           648 STORE_FAST               7 (col)
+                           646 STORE_FAST               7 (posy)
+                           648 STORE_FAST               8 (col)
                
-               214         650 LOAD_FAST                7 (col)
-                           652 LOAD_FAST                3 (qr)
+               214         650 LOAD_FAST                8 (col)
+                           652 LOAD_FAST                4 (qr)
                            654 LOAD_ATTR               11 (matrix)
-                           664 LOAD_FAST                3 (qr)
+                           664 LOAD_FAST                4 (qr)
                            666 LOAD_ATTR               12 (size)
                            676 LOAD_CONST               5 (7)
                            678 BINARY_OP               10 (-)
-                           682 LOAD_FAST                4 (posx)
+                           682 LOAD_FAST                5 (posx)
                            684 BINARY_OP                0 (+)
                            688 BINARY_SUBSCR
-                           698 LOAD_FAST                6 (posy)
+                           698 LOAD_FAST                7 (posy)
                            700 STORE_SUBSCR
                            704 JUMP_BACKWARD           33 (to 640)
                
                213     >>  706 JUMP_BACKWARD           54 (to 600)
                
                218     >>  708 LOAD_GLOBAL             27 (NULL + range)
                            720 LOAD_CONST               6 (8)
                            722 PRECALL                  1
                            726 CALL                     1
                            736 GET_ITER
                        >>  738 FOR_ITER                18 (to 776)
-                           740 STORE_FAST               8 (i)
+                           740 STORE_FAST               9 (i)
                
                219         742 LOAD_CONST               7 (0)
-                           744 LOAD_FAST                3 (qr)
+                           744 LOAD_FAST                4 (qr)
                            746 LOAD_ATTR               11 (matrix)
-                           756 LOAD_FAST                8 (i)
+                           756 LOAD_FAST                9 (i)
                            758 BINARY_SUBSCR
                            768 LOAD_CONST               5 (7)
                            770 STORE_SUBSCR
                            774 JUMP_BACKWARD           19 (to 738)
                
                220     >>  776 LOAD_GLOBAL             27 (NULL + range)
                            788 LOAD_CONST               6 (8)
                            790 PRECALL                  1
                            794 CALL                     1
                            804 GET_ITER
                        >>  806 FOR_ITER                18 (to 844)
-                           808 STORE_FAST               8 (i)
+                           808 STORE_FAST               9 (i)
                
                221         810 LOAD_CONST               7 (0)
-                           812 LOAD_FAST                3 (qr)
+                           812 LOAD_FAST                4 (qr)
                            814 LOAD_ATTR               11 (matrix)
                            824 LOAD_CONST               5 (7)
                            826 BINARY_SUBSCR
-                           836 LOAD_FAST                8 (i)
+                           836 LOAD_FAST                9 (i)
                            838 STORE_SUBSCR
                            842 JUMP_BACKWARD           19 (to 806)
                
                224     >>  844 LOAD_GLOBAL             27 (NULL + range)
                            856 LOAD_CONST               6 (8)
                            858 PRECALL                  1
                            862 CALL                     1
                            872 GET_ITER
                        >>  874 FOR_ITER                26 (to 928)
-                           876 STORE_FAST               8 (i)
+                           876 STORE_FAST               9 (i)
                
                225         878 LOAD_CONST               7 (0)
-                           880 LOAD_FAST                3 (qr)
+                           880 LOAD_FAST                4 (qr)
                            882 LOAD_ATTR               11 (matrix)
-                           892 LOAD_FAST                8 (i)
+                           892 LOAD_FAST                9 (i)
                            894 BINARY_SUBSCR
-                           904 LOAD_FAST                3 (qr)
+                           904 LOAD_FAST                4 (qr)
                            906 LOAD_ATTR               12 (size)
                            916 LOAD_CONST               6 (8)
                            918 BINARY_OP               10 (-)
                            922 STORE_SUBSCR
                            926 JUMP_BACKWARD           27 (to 874)
                
                226     >>  928 LOAD_GLOBAL             27 (NULL + range)
                            940 LOAD_CONST               6 (8)
                            942 PRECALL                  1
                            946 CALL                     1
                            956 GET_ITER
                        >>  958 FOR_ITER                29 (to 1018)
-                           960 STORE_FAST               8 (i)
+                           960 STORE_FAST               9 (i)
                
                227         962 LOAD_CONST               7 (0)
-                           964 LOAD_FAST                3 (qr)
+                           964 LOAD_FAST                4 (qr)
                            966 LOAD_ATTR               11 (matrix)
                            976 LOAD_CONST               5 (7)
                            978 BINARY_SUBSCR
-                           988 LOAD_FAST                3 (qr)
+                           988 LOAD_FAST                4 (qr)
                            990 LOAD_ATTR               12 (size)
                           1000 LOAD_CONST               8 (1)
                           1002 BINARY_OP               10 (-)
-                          1006 LOAD_FAST                8 (i)
+                          1006 LOAD_FAST                9 (i)
                           1008 BINARY_OP               10 (-)
                           1012 STORE_SUBSCR
                           1016 JUMP_BACKWARD           30 (to 958)
                
                230     >> 1018 LOAD_GLOBAL             27 (NULL + range)
                           1030 LOAD_CONST               6 (8)
                           1032 PRECALL                  1
                           1036 CALL                     1
                           1046 GET_ITER
                        >> 1048 FOR_ITER                29 (to 1108)
-                          1050 STORE_FAST               8 (i)
+                          1050 STORE_FAST               9 (i)
                
                231        1052 LOAD_CONST               7 (0)
-                          1054 LOAD_FAST                3 (qr)
+                          1054 LOAD_FAST                4 (qr)
                           1056 LOAD_ATTR               11 (matrix)
-                          1066 LOAD_FAST                3 (qr)
+                          1066 LOAD_FAST                4 (qr)
                           1068 LOAD_ATTR               12 (size)
                           1078 LOAD_CONST               6 (8)
                           1080 BINARY_OP               10 (-)
-                          1084 LOAD_FAST                8 (i)
+                          1084 LOAD_FAST                9 (i)
                           1086 BINARY_OP                0 (+)
                           1090 BINARY_SUBSCR
                           1100 LOAD_CONST               5 (7)
                           1102 STORE_SUBSCR
                           1106 JUMP_BACKWARD           30 (to 1048)
                
                232     >> 1108 LOAD_GLOBAL             27 (NULL + range)
                           1120 LOAD_CONST               6 (8)
                           1122 PRECALL                  1
                           1126 CALL                     1
                           1136 GET_ITER
                        >> 1138 FOR_ITER                26 (to 1192)
-                          1140 STORE_FAST               8 (i)
+                          1140 STORE_FAST               9 (i)
                
                233        1142 LOAD_CONST               7 (0)
-                          1144 LOAD_FAST                3 (qr)
+                          1144 LOAD_FAST                4 (qr)
                           1146 LOAD_ATTR               11 (matrix)
-                          1156 LOAD_FAST                3 (qr)
+                          1156 LOAD_FAST                4 (qr)
                           1158 LOAD_ATTR               12 (size)
                           1168 LOAD_CONST               6 (8)
                           1170 BINARY_OP               10 (-)
                           1174 BINARY_SUBSCR
-                          1184 LOAD_FAST                8 (i)
+                          1184 LOAD_FAST                9 (i)
                           1186 STORE_SUBSCR
                           1190 JUMP_BACKWARD           27 (to 1138)
                
                237     >> 1192 LOAD_CONST               8 (1)
-                          1194 STORE_FAST               9 (value)
+                          1194 STORE_FAST              10 (value)
                
                238        1196 LOAD_GLOBAL             27 (NULL + range)
                           1208 LOAD_CONST               6 (8)
-                          1210 LOAD_FAST                3 (qr)
+                          1210 LOAD_FAST                4 (qr)
                           1212 LOAD_ATTR               12 (size)
                           1222 LOAD_CONST               6 (8)
                           1224 BINARY_OP               10 (-)
                           1228 PRECALL                  2
                           1232 CALL                     2
                           1242 GET_ITER
                        >> 1244 FOR_ITER                26 (to 1298)
-                          1246 STORE_FAST               8 (i)
+                          1246 STORE_FAST               9 (i)
                
-               239        1248 LOAD_FAST                9 (value)
+               239        1248 LOAD_FAST               10 (value)
                           1250 LOAD_CONST               9 (2)
                           1252 BINARY_OP                6 (%)
-                          1256 LOAD_FAST                3 (qr)
+                          1256 LOAD_FAST                4 (qr)
                           1258 LOAD_ATTR               11 (matrix)
                           1268 LOAD_CONST              10 (6)
                           1270 BINARY_SUBSCR
-                          1280 LOAD_FAST                8 (i)
+                          1280 LOAD_FAST                9 (i)
                           1282 STORE_SUBSCR
                
-               240        1286 LOAD_FAST                9 (value)
+               240        1286 LOAD_FAST               10 (value)
                           1288 LOAD_CONST               8 (1)
                           1290 BINARY_OP               13 (+=)
-                          1294 STORE_FAST               9 (value)
+                          1294 STORE_FAST              10 (value)
                           1296 JUMP_BACKWARD           27 (to 1244)
                
                243     >> 1298 LOAD_CONST               8 (1)
-                          1300 STORE_FAST               9 (value)
+                          1300 STORE_FAST              10 (value)
                
                244        1302 LOAD_GLOBAL             27 (NULL + range)
                           1314 LOAD_CONST               6 (8)
-                          1316 LOAD_FAST                3 (qr)
+                          1316 LOAD_FAST                4 (qr)
                           1318 LOAD_ATTR               12 (size)
                           1328 LOAD_CONST               6 (8)
                           1330 BINARY_OP               10 (-)
                           1334 PRECALL                  2
                           1338 CALL                     2
                           1348 GET_ITER
                        >> 1350 FOR_ITER                26 (to 1404)
-                          1352 STORE_FAST               8 (i)
+                          1352 STORE_FAST               9 (i)
                
-               245        1354 LOAD_FAST                9 (value)
+               245        1354 LOAD_FAST               10 (value)
                           1356 LOAD_CONST               9 (2)
                           1358 BINARY_OP                6 (%)
-                          1362 LOAD_FAST                3 (qr)
+                          1362 LOAD_FAST                4 (qr)
                           1364 LOAD_ATTR               11 (matrix)
-                          1374 LOAD_FAST                8 (i)
+                          1374 LOAD_FAST                9 (i)
                           1376 BINARY_SUBSCR
                           1386 LOAD_CONST              10 (6)
                           1388 STORE_SUBSCR
                
-               246        1392 LOAD_FAST                9 (value)
+               246        1392 LOAD_FAST               10 (value)
                           1394 LOAD_CONST               8 (1)
                           1396 BINARY_OP               13 (+=)
-                          1400 STORE_FAST               9 (value)
+                          1400 STORE_FAST              10 (value)
                           1402 JUMP_BACKWARD           27 (to 1350)
                
                249     >> 1404 LOAD_GLOBAL              1 (NULL + qrutils)
                           1416 LOAD_ATTR               14 (alignment_pattern_locations)
                           1426 LOAD_FAST                0 (self)
                           1428 LOAD_ATTR                2 (version)
                           1438 PRECALL                  1
                           1442 CALL                     1
-                          1452 STORE_FAST              10 (patternLocations)
+                          1452 STORE_FAST              11 (patternLocations)
                
-               251        1454 LOAD_FAST               10 (patternLocations)
+               251        1454 LOAD_FAST               11 (patternLocations)
                           1456 GET_ITER
                        >> 1458 FOR_ITER               109 (to 1678)
-                          1460 STORE_FAST              11 (patternLocation)
+                          1460 STORE_FAST              12 (patternLocation)
                
-               252        1462 LOAD_FAST               11 (patternLocation)
+               252        1462 LOAD_FAST               12 (patternLocation)
                           1464 LOAD_CONST               7 (0)
                           1466 BINARY_SUBSCR
-                          1476 STORE_FAST               4 (posx)
+                          1476 STORE_FAST               5 (posx)
                
-               253        1478 LOAD_FAST               11 (patternLocation)
+               253        1478 LOAD_FAST               12 (patternLocation)
                           1480 LOAD_CONST               8 (1)
                           1482 BINARY_SUBSCR
-                          1492 STORE_FAST               6 (posy)
+                          1492 STORE_FAST               7 (posy)
                
                255        1494 BUILD_LIST               0
                           1496 LOAD_CONST              11 ((-2, -1, 0, 1, 2))
                           1498 LIST_EXTEND              1
-                          1500 STORE_FAST              12 (offset)
+                          1500 STORE_FAST              13 (offset)
                
                256        1502 LOAD_GLOBAL             27 (NULL + range)
                           1514 LOAD_CONST              12 (5)
                           1516 PRECALL                  1
                           1520 CALL                     1
                           1530 GET_ITER
                        >> 1532 FOR_ITER                71 (to 1676)
-                          1534 STORE_FAST               8 (i)
+                          1534 STORE_FAST               9 (i)
                
                257        1536 LOAD_GLOBAL             27 (NULL + range)
                           1548 LOAD_CONST              12 (5)
                           1550 PRECALL                  1
                           1554 CALL                     1
                           1564 GET_ITER
                        >> 1566 FOR_ITER                53 (to 1674)
-                          1568 STORE_FAST              13 (j)
+                          1568 STORE_FAST              14 (j)
                
                258        1570 LOAD_GLOBAL             30 (alignmentPattern)
-                          1582 LOAD_FAST                8 (i)
+                          1582 LOAD_FAST                9 (i)
                           1584 BINARY_SUBSCR
-                          1594 LOAD_FAST               13 (j)
+                          1594 LOAD_FAST               14 (j)
                           1596 BINARY_SUBSCR
-                          1606 LOAD_FAST                3 (qr)
+                          1606 LOAD_FAST                4 (qr)
                           1608 LOAD_ATTR               11 (matrix)
-                          1618 LOAD_FAST                4 (posx)
-                          1620 LOAD_FAST               12 (offset)
-                          1622 LOAD_FAST                8 (i)
+                          1618 LOAD_FAST                5 (posx)
+                          1620 LOAD_FAST               13 (offset)
+                          1622 LOAD_FAST                9 (i)
                           1624 BINARY_SUBSCR
                           1634 BINARY_OP                0 (+)
                           1638 BINARY_SUBSCR
-                          1648 LOAD_FAST                6 (posy)
-                          1650 LOAD_FAST               12 (offset)
-                          1652 LOAD_FAST               13 (j)
+                          1648 LOAD_FAST                7 (posy)
+                          1650 LOAD_FAST               13 (offset)
+                          1652 LOAD_FAST               14 (j)
                           1654 BINARY_SUBSCR
                           1664 BINARY_OP                0 (+)
                           1668 STORE_SUBSCR
                           1672 JUMP_BACKWARD           54 (to 1566)
                
                257     >> 1674 JUMP_BACKWARD           72 (to 1532)
                
                256     >> 1676 JUMP_BACKWARD          110 (to 1458)
                
                261     >> 1678 LOAD_CONST               8 (1)
-                          1680 LOAD_FAST                3 (qr)
+                          1680 LOAD_FAST                4 (qr)
                           1682 LOAD_ATTR               11 (matrix)
-                          1692 LOAD_FAST                3 (qr)
+                          1692 LOAD_FAST                4 (qr)
                           1694 LOAD_ATTR               12 (size)
                           1704 LOAD_CONST               6 (8)
                           1706 BINARY_OP               10 (-)
                           1710 BINARY_SUBSCR
                           1720 LOAD_CONST               6 (8)
                           1722 STORE_SUBSCR
                
                265        1726 LOAD_GLOBAL             27 (NULL + range)
                           1738 LOAD_CONST              13 (9)
                           1740 PRECALL                  1
                           1744 CALL                     1
                           1754 GET_ITER
                        >> 1756 FOR_ITER                24 (to 1806)
-                          1758 STORE_FAST               8 (i)
+                          1758 STORE_FAST               9 (i)
                
-               266        1760 LOAD_FAST                8 (i)
+               266        1760 LOAD_FAST                9 (i)
                           1762 LOAD_CONST              10 (6)
                           1764 COMPARE_OP               3 (!=)
                           1770 POP_JUMP_FORWARD_IF_FALSE    16 (to 1804)
                
                267        1772 LOAD_CONST              14 ('x')
-                          1774 LOAD_FAST                3 (qr)
+                          1774 LOAD_FAST                4 (qr)
                           1776 LOAD_ATTR               11 (matrix)
-                          1786 LOAD_FAST                8 (i)
+                          1786 LOAD_FAST                9 (i)
                           1788 BINARY_SUBSCR
                           1798 LOAD_CONST               6 (8)
                           1800 STORE_SUBSCR
                        >> 1804 JUMP_BACKWARD           25 (to 1756)
                
                268     >> 1806 LOAD_GLOBAL             27 (NULL + range)
                           1818 LOAD_CONST              13 (9)
                           1820 PRECALL                  1
                           1824 CALL                     1
                           1834 GET_ITER
                        >> 1836 FOR_ITER                24 (to 1886)
-                          1838 STORE_FAST               8 (i)
+                          1838 STORE_FAST               9 (i)
                
-               269        1840 LOAD_FAST                8 (i)
+               269        1840 LOAD_FAST                9 (i)
                           1842 LOAD_CONST              10 (6)
                           1844 COMPARE_OP               3 (!=)
                           1850 POP_JUMP_FORWARD_IF_FALSE    16 (to 1884)
                
                270        1852 LOAD_CONST              14 ('x')
-                          1854 LOAD_FAST                3 (qr)
+                          1854 LOAD_FAST                4 (qr)
                           1856 LOAD_ATTR               11 (matrix)
                           1866 LOAD_CONST               6 (8)
                           1868 BINARY_SUBSCR
-                          1878 LOAD_FAST                8 (i)
+                          1878 LOAD_FAST                9 (i)
                           1880 STORE_SUBSCR
                        >> 1884 JUMP_BACKWARD           25 (to 1836)
                
                273     >> 1886 LOAD_GLOBAL             27 (NULL + range)
                           1898 LOAD_CONST               8 (1)
                           1900 LOAD_CONST              13 (9)
                           1902 PRECALL                  2
                           1906 CALL                     2
                           1916 GET_ITER
                        >> 1918 FOR_ITER                26 (to 1972)
-                          1920 STORE_FAST               8 (i)
+                          1920 STORE_FAST               9 (i)
                
                274        1922 LOAD_CONST              14 ('x')
-                          1924 LOAD_FAST                3 (qr)
+                          1924 LOAD_FAST                4 (qr)
                           1926 LOAD_ATTR               11 (matrix)
                           1936 LOAD_CONST               6 (8)
                           1938 BINARY_SUBSCR
-                          1948 LOAD_FAST                3 (qr)
+                          1948 LOAD_FAST                4 (qr)
                           1950 LOAD_ATTR               12 (size)
-                          1960 LOAD_FAST                8 (i)
+                          1960 LOAD_FAST                9 (i)
                           1962 BINARY_OP               10 (-)
                           1966 STORE_SUBSCR
                           1970 JUMP_BACKWARD           27 (to 1918)
                
                277     >> 1972 LOAD_GLOBAL             27 (NULL + range)
                           1984 LOAD_CONST               8 (1)
                           1986 LOAD_CONST               6 (8)
                           1988 PRECALL                  2
                           1992 CALL                     2
                           2002 GET_ITER
                        >> 2004 FOR_ITER                26 (to 2058)
-                          2006 STORE_FAST               8 (i)
+                          2006 STORE_FAST               9 (i)
                
                278        2008 LOAD_CONST              14 ('x')
-                          2010 LOAD_FAST                3 (qr)
+                          2010 LOAD_FAST                4 (qr)
                           2012 LOAD_ATTR               11 (matrix)
-                          2022 LOAD_FAST                3 (qr)
+                          2022 LOAD_FAST                4 (qr)
                           2024 LOAD_ATTR               12 (size)
-                          2034 LOAD_FAST                8 (i)
+                          2034 LOAD_FAST                9 (i)
                           2036 BINARY_OP               10 (-)
                           2040 BINARY_SUBSCR
                           2050 LOAD_CONST               6 (8)
                           2052 STORE_SUBSCR
                           2056 JUMP_BACKWARD           27 (to 2004)
                
                281     >> 2058 LOAD_FAST                0 (self)
@@ -2813,316 +2820,328 @@
                
                282        2130 LOAD_GLOBAL             27 (NULL + range)
                           2142 LOAD_CONST              10 (6)
                           2144 PRECALL                  1
                           2148 CALL                     1
                           2158 GET_ITER
                        >> 2160 FOR_ITER                74 (to 2310)
-                          2162 STORE_FAST               8 (i)
+                          2162 STORE_FAST               9 (i)
                
                283        2164 LOAD_GLOBAL             27 (NULL + range)
                           2176 LOAD_CONST              15 (3)
                           2178 PRECALL                  1
                           2182 CALL                     1
                           2192 GET_ITER
                        >> 2194 FOR_ITER                56 (to 2308)
-                          2196 STORE_FAST              13 (j)
+                          2196 STORE_FAST              14 (j)
                
                284        2198 LOAD_CONST              14 ('x')
-                          2200 LOAD_FAST                3 (qr)
+                          2200 LOAD_FAST                4 (qr)
                           2202 LOAD_ATTR               11 (matrix)
-                          2212 LOAD_FAST                8 (i)
+                          2212 LOAD_FAST                9 (i)
                           2214 BINARY_SUBSCR
-                          2224 LOAD_FAST                3 (qr)
+                          2224 LOAD_FAST                4 (qr)
                           2226 LOAD_ATTR               12 (size)
                           2236 LOAD_CONST              16 (11)
                           2238 BINARY_OP               10 (-)
-                          2242 LOAD_FAST               13 (j)
+                          2242 LOAD_FAST               14 (j)
                           2244 BINARY_OP                0 (+)
                           2248 STORE_SUBSCR
                
                285        2252 LOAD_CONST              14 ('x')
-                          2254 LOAD_FAST                3 (qr)
+                          2254 LOAD_FAST                4 (qr)
                           2256 LOAD_ATTR               11 (matrix)
-                          2266 LOAD_FAST                3 (qr)
+                          2266 LOAD_FAST                4 (qr)
                           2268 LOAD_ATTR               12 (size)
                           2278 LOAD_CONST              16 (11)
                           2280 BINARY_OP               10 (-)
-                          2284 LOAD_FAST               13 (j)
+                          2284 LOAD_FAST               14 (j)
                           2286 BINARY_OP                0 (+)
                           2290 BINARY_SUBSCR
-                          2300 LOAD_FAST                8 (i)
+                          2300 LOAD_FAST                9 (i)
                           2302 STORE_SUBSCR
                           2306 JUMP_BACKWARD           57 (to 2194)
                
                283     >> 2308 JUMP_BACKWARD           75 (to 2160)
                
                288     >> 2310 LOAD_GLOBAL             19 (NULL + enumerate)
-                          2322 LOAD_FAST                3 (qr)
+                          2322 LOAD_FAST                4 (qr)
                           2324 LOAD_ATTR               11 (matrix)
                           2334 PRECALL                  1
                           2338 CALL                     1
                           2348 GET_ITER
                        >> 2350 FOR_ITER                48 (to 2448)
                           2352 UNPACK_SEQUENCE          2
-                          2356 STORE_FAST               4 (posx)
-                          2358 STORE_FAST               5 (row)
+                          2356 STORE_FAST               5 (posx)
+                          2358 STORE_FAST               6 (row)
                
                289        2360 LOAD_GLOBAL             19 (NULL + enumerate)
-                          2372 LOAD_FAST                5 (row)
+                          2372 LOAD_FAST                6 (row)
                           2374 PRECALL                  1
                           2378 CALL                     1
                           2388 GET_ITER
                        >> 2390 FOR_ITER                27 (to 2446)
                           2392 UNPACK_SEQUENCE          2
-                          2396 STORE_FAST               6 (posy)
-                          2398 STORE_FAST               7 (col)
+                          2396 STORE_FAST               7 (posy)
+                          2398 STORE_FAST               8 (col)
                
-               290        2400 LOAD_FAST                7 (col)
+               290        2400 LOAD_FAST                8 (col)
                           2402 LOAD_CONST              17 ('X')
                           2404 COMPARE_OP               3 (!=)
                           2410 POP_JUMP_FORWARD_IF_FALSE    16 (to 2444)
                
                291        2412 LOAD_CONST               8 (1)
-                          2414 LOAD_FAST                3 (qr)
+                          2414 LOAD_FAST                4 (qr)
                           2416 LOAD_ATTR               19 (reserved_positions)
-                          2426 LOAD_FAST                4 (posx)
+                          2426 LOAD_FAST                5 (posx)
                           2428 BINARY_SUBSCR
-                          2438 LOAD_FAST                6 (posy)
+                          2438 LOAD_FAST                7 (posy)
                           2440 STORE_SUBSCR
                        >> 2444 JUMP_BACKWARD           28 (to 2390)
                
                289     >> 2446 JUMP_BACKWARD           49 (to 2350)
                
-               296     >> 2448 LOAD_FAST                3 (qr)
+               296     >> 2448 LOAD_FAST                4 (qr)
                           2450 LOAD_ATTR               12 (size)
                           2460 LOAD_CONST               8 (1)
                           2462 BINARY_OP               10 (-)
-                          2466 STORE_FAST               4 (posx)
+                          2466 STORE_FAST               5 (posx)
                
-               297        2468 LOAD_FAST                3 (qr)
+               297        2468 LOAD_FAST                4 (qr)
                           2470 LOAD_ATTR               12 (size)
                           2480 LOAD_CONST               8 (1)
                           2482 BINARY_OP               10 (-)
-                          2486 STORE_FAST               6 (posy)
+                          2486 STORE_FAST               7 (posy)
                
                298        2488 LOAD_CONST               8 (1)
-                          2490 STORE_FAST              14 (directionUD)
+                          2490 STORE_FAST              15 (directionUD)
                
                299        2492 LOAD_CONST               8 (1)
-                          2494 STORE_FAST              15 (directionLR)
+                          2494 STORE_FAST              16 (directionLR)
                
                300        2496 LOAD_CONST               7 (0)
-                          2498 STORE_FAST              16 (dataPos)
+                          2498 STORE_FAST              17 (dataPos)
                
-               301        2500 LOAD_FAST               16 (dataPos)
+               301        2500 LOAD_FAST               17 (dataPos)
                           2502 LOAD_GLOBAL             41 (NULL + len)
-                          2514 LOAD_FAST                2 (interleavedData)
+                          2514 LOAD_FAST                3 (interleavedData)
                           2516 PRECALL                  1
                           2520 CALL                     1
                           2530 COMPARE_OP               0 (<)
                           2536 POP_JUMP_FORWARD_IF_FALSE   239 (to 3016)
                
-               303     >> 2538 LOAD_FAST                3 (qr)
+               303     >> 2538 LOAD_FAST                4 (qr)
                           2540 LOAD_ATTR               11 (matrix)
-                          2550 LOAD_FAST                4 (posx)
+                          2550 LOAD_FAST                5 (posx)
                           2552 BINARY_SUBSCR
-                          2562 LOAD_FAST                6 (posy)
+                          2562 LOAD_FAST                7 (posy)
                           2564 BINARY_SUBSCR
                           2574 LOAD_CONST              17 ('X')
                           2576 COMPARE_OP               2 (==)
                           2582 POP_JUMP_FORWARD_IF_FALSE    27 (to 2638)
                
-               304        2584 LOAD_FAST                2 (interleavedData)
-                          2586 LOAD_FAST               16 (dataPos)
+               304        2584 LOAD_FAST                3 (interleavedData)
+                          2586 LOAD_FAST               17 (dataPos)
                           2588 BINARY_SUBSCR
-                          2598 LOAD_FAST                3 (qr)
+                          2598 LOAD_FAST                4 (qr)
                           2600 LOAD_ATTR               11 (matrix)
-                          2610 LOAD_FAST                4 (posx)
+                          2610 LOAD_FAST                5 (posx)
                           2612 BINARY_SUBSCR
-                          2622 LOAD_FAST                6 (posy)
+                          2622 LOAD_FAST                7 (posy)
                           2624 STORE_SUBSCR
                
-               305        2628 LOAD_FAST               16 (dataPos)
+               305        2628 LOAD_FAST               17 (dataPos)
                           2630 LOAD_CONST               8 (1)
                           2632 BINARY_OP               13 (+=)
-                          2636 STORE_FAST              16 (dataPos)
+                          2636 STORE_FAST              17 (dataPos)
                
-               309     >> 2638 LOAD_FAST               14 (directionUD)
+               309     >> 2638 LOAD_FAST               15 (directionUD)
                           2640 LOAD_CONST               8 (1)
                           2642 COMPARE_OP               2 (==)
                           2648 POP_JUMP_FORWARD_IF_FALSE    14 (to 2678)
-                          2650 LOAD_FAST               15 (directionLR)
+                          2650 LOAD_FAST               16 (directionLR)
                           2652 LOAD_CONST               8 (1)
                           2654 COMPARE_OP               2 (==)
                           2660 POP_JUMP_FORWARD_IF_FALSE     8 (to 2678)
                
-               310        2662 LOAD_FAST                6 (posy)
+               310        2662 LOAD_FAST                7 (posy)
                           2664 LOAD_CONST               8 (1)
                           2666 BINARY_OP               23 (-=)
-                          2670 STORE_FAST               6 (posy)
+                          2670 STORE_FAST               7 (posy)
                
                311        2672 LOAD_CONST              18 (-1)
-                          2674 STORE_FAST              15 (directionLR)
+                          2674 STORE_FAST              16 (directionLR)
                           2676 JUMP_FORWARD            69 (to 2816)
                
-               312     >> 2678 LOAD_FAST               14 (directionUD)
+               312     >> 2678 LOAD_FAST               15 (directionUD)
                           2680 LOAD_CONST               8 (1)
                           2682 COMPARE_OP               2 (==)
                           2688 POP_JUMP_FORWARD_IF_FALSE    19 (to 2728)
-                          2690 LOAD_FAST               15 (directionLR)
+                          2690 LOAD_FAST               16 (directionLR)
                           2692 LOAD_CONST              18 (-1)
                           2694 COMPARE_OP               2 (==)
                           2700 POP_JUMP_FORWARD_IF_FALSE    13 (to 2728)
                
-               313        2702 LOAD_FAST                4 (posx)
+               313        2702 LOAD_FAST                5 (posx)
                           2704 LOAD_CONST               8 (1)
                           2706 BINARY_OP               23 (-=)
-                          2710 STORE_FAST               4 (posx)
+                          2710 STORE_FAST               5 (posx)
                
-               314        2712 LOAD_FAST                6 (posy)
+               314        2712 LOAD_FAST                7 (posy)
                           2714 LOAD_CONST               8 (1)
                           2716 BINARY_OP               13 (+=)
-                          2720 STORE_FAST               6 (posy)
+                          2720 STORE_FAST               7 (posy)
                
                315        2722 LOAD_CONST               8 (1)
-                          2724 STORE_FAST              15 (directionLR)
+                          2724 STORE_FAST              16 (directionLR)
                           2726 JUMP_FORWARD            44 (to 2816)
                
-               316     >> 2728 LOAD_FAST               14 (directionUD)
+               316     >> 2728 LOAD_FAST               15 (directionUD)
                           2730 LOAD_CONST              18 (-1)
                           2732 COMPARE_OP               2 (==)
                           2738 POP_JUMP_FORWARD_IF_FALSE    14 (to 2768)
-                          2740 LOAD_FAST               15 (directionLR)
+                          2740 LOAD_FAST               16 (directionLR)
                           2742 LOAD_CONST               8 (1)
                           2744 COMPARE_OP               2 (==)
                           2750 POP_JUMP_FORWARD_IF_FALSE     8 (to 2768)
                
-               318        2752 LOAD_FAST                6 (posy)
+               318        2752 LOAD_FAST                7 (posy)
                           2754 LOAD_CONST               8 (1)
                           2756 BINARY_OP               23 (-=)
-                          2760 STORE_FAST               6 (posy)
+                          2760 STORE_FAST               7 (posy)
                
                319        2762 LOAD_CONST              18 (-1)
-                          2764 STORE_FAST              15 (directionLR)
+                          2764 STORE_FAST              16 (directionLR)
                           2766 JUMP_FORWARD            24 (to 2816)
                
-               320     >> 2768 LOAD_FAST               14 (directionUD)
+               320     >> 2768 LOAD_FAST               15 (directionUD)
                           2770 LOAD_CONST              18 (-1)
                           2772 COMPARE_OP               2 (==)
                           2778 POP_JUMP_FORWARD_IF_FALSE    18 (to 2816)
-                          2780 LOAD_FAST               15 (directionLR)
+                          2780 LOAD_FAST               16 (directionLR)
                           2782 LOAD_CONST              18 (-1)
                           2784 COMPARE_OP               2 (==)
                           2790 POP_JUMP_FORWARD_IF_FALSE    12 (to 2816)
                
-               321        2792 LOAD_FAST                6 (posy)
+               321        2792 LOAD_FAST                7 (posy)
                           2794 LOAD_CONST               8 (1)
                           2796 BINARY_OP               13 (+=)
-                          2800 STORE_FAST               6 (posy)
+                          2800 STORE_FAST               7 (posy)
                
-               322        2802 LOAD_FAST                4 (posx)
+               322        2802 LOAD_FAST                5 (posx)
                           2804 LOAD_CONST               8 (1)
                           2806 BINARY_OP               13 (+=)
-                          2810 STORE_FAST               4 (posx)
+                          2810 STORE_FAST               5 (posx)
                
                323        2812 LOAD_CONST               8 (1)
-                          2814 STORE_FAST              15 (directionLR)
+                          2814 STORE_FAST              16 (directionLR)
                
-               326     >> 2816 LOAD_FAST                4 (posx)
+               326     >> 2816 LOAD_FAST                5 (posx)
                           2818 LOAD_CONST              18 (-1)
                           2820 COMPARE_OP               2 (==)
                           2826 POP_JUMP_FORWARD_IF_FALSE    12 (to 2852)
                
                327        2828 LOAD_CONST              18 (-1)
-                          2830 STORE_FAST              14 (directionUD)
+                          2830 STORE_FAST              15 (directionUD)
                
                328        2832 LOAD_CONST               7 (0)
-                          2834 STORE_FAST               4 (posx)
+                          2834 STORE_FAST               5 (posx)
                
                329        2836 LOAD_CONST               8 (1)
-                          2838 STORE_FAST              15 (directionLR)
+                          2838 STORE_FAST              16 (directionLR)
                
-               330        2840 LOAD_FAST                6 (posy)
+               330        2840 LOAD_FAST                7 (posy)
                           2842 LOAD_CONST               9 (2)
                           2844 BINARY_OP               23 (-=)
-                          2848 STORE_FAST               6 (posy)
+                          2848 STORE_FAST               7 (posy)
                           2850 JUMP_FORWARD            30 (to 2912)
                
-               331     >> 2852 LOAD_FAST                4 (posx)
-                          2854 LOAD_FAST                3 (qr)
+               331     >> 2852 LOAD_FAST                5 (posx)
+                          2854 LOAD_FAST                4 (qr)
                           2856 LOAD_ATTR               12 (size)
                           2866 COMPARE_OP               2 (==)
                           2872 POP_JUMP_FORWARD_IF_FALSE    19 (to 2912)
                
                332        2874 LOAD_CONST               8 (1)
-                          2876 STORE_FAST              14 (directionUD)
+                          2876 STORE_FAST              15 (directionUD)
                
-               333        2878 LOAD_FAST                3 (qr)
+               333        2878 LOAD_FAST                4 (qr)
                           2880 LOAD_ATTR               12 (size)
                           2890 LOAD_CONST               8 (1)
                           2892 BINARY_OP               10 (-)
-                          2896 STORE_FAST               4 (posx)
+                          2896 STORE_FAST               5 (posx)
                
                334        2898 LOAD_CONST               8 (1)
-                          2900 STORE_FAST              15 (directionLR)
+                          2900 STORE_FAST              16 (directionLR)
                
-               335        2902 LOAD_FAST                6 (posy)
+               335        2902 LOAD_FAST                7 (posy)
                           2904 LOAD_CONST               9 (2)
                           2906 BINARY_OP               23 (-=)
-                          2910 STORE_FAST               6 (posy)
+                          2910 STORE_FAST               7 (posy)
                
-               337     >> 2912 LOAD_FAST                6 (posy)
+               337     >> 2912 LOAD_FAST                7 (posy)
                           2914 LOAD_CONST              10 (6)
                           2916 COMPARE_OP               2 (==)
                           2922 POP_JUMP_FORWARD_IF_FALSE     5 (to 2934)
                
-               338        2924 LOAD_FAST                6 (posy)
+               338        2924 LOAD_FAST                7 (posy)
                           2926 LOAD_CONST               8 (1)
                           2928 BINARY_OP               23 (-=)
-                          2932 STORE_FAST               6 (posy)
+                          2932 STORE_FAST               7 (posy)
                
-               340     >> 2934 LOAD_FAST                6 (posy)
+               340     >> 2934 LOAD_FAST                7 (posy)
                           2936 LOAD_CONST               7 (0)
                           2938 COMPARE_OP               0 (<)
                           2944 POP_JUMP_FORWARD_IF_FALSE    16 (to 2978)
                
                341        2946 LOAD_GLOBAL             43 (NULL + print)
                           2958 LOAD_CONST              19 ('No more space for data')
                           2960 PRECALL                  1
                           2964 CALL                     1
                           2974 POP_TOP
                
                343        2976 JUMP_FORWARD            19 (to 3016)
                
-               301     >> 2978 LOAD_FAST               16 (dataPos)
+               301     >> 2978 LOAD_FAST               17 (dataPos)
                           2980 LOAD_GLOBAL             41 (NULL + len)
-                          2992 LOAD_FAST                2 (interleavedData)
+                          2992 LOAD_FAST                3 (interleavedData)
                           2994 PRECALL                  1
                           2998 CALL                     1
                           3008 COMPARE_OP               0 (<)
                           3014 POP_JUMP_BACKWARD_IF_TRUE   239 (to 2538)
                
                346     >> 3016 LOAD_GLOBAL              1 (NULL + qrutils)
                           3028 LOAD_ATTR               22 (qr_masking)
-                          3038 LOAD_FAST                3 (qr)
+                          3038 LOAD_FAST                4 (qr)
                           3040 LOAD_ATTR               11 (matrix)
-                          3050 LOAD_FAST                3 (qr)
+                          3050 LOAD_FAST                4 (qr)
                           3052 LOAD_ATTR               19 (reserved_positions)
                           3062 LOAD_FAST                0 (self)
                           3064 LOAD_ATTR                4 (error_correction)
                           3074 LOAD_FAST                0 (self)
                           3076 LOAD_ATTR                2 (version)
                           3086 PRECALL                  4
                           3090 CALL                     4
-                          3100 LOAD_FAST                3 (qr)
-                          3102 STORE_ATTR              11 (matrix)
+                          3100 UNPACK_SEQUENCE          3
+                          3104 LOAD_FAST                4 (qr)
+                          3106 STORE_ATTR              11 (matrix)
+                          3116 STORE_FAST              18 (allPaterns)
+                          3118 STORE_FAST              19 (allPenaltyScores)
+               
+               361        3120 LOAD_FAST                1 (returnALL)
+                          3122 POP_JUMP_FORWARD_IF_FALSE     5 (to 3134)
+               
+               362        3124 LOAD_FAST                4 (qr)
+                          3126 LOAD_FAST               18 (allPaterns)
+                          3128 LOAD_FAST               19 (allPenaltyScores)
+                          3130 BUILD_TUPLE              3
+                          3132 RETURN_VALUE
                
-               361        3112 LOAD_FAST                3 (qr)
-                          3114 RETURN_VALUE
+               364     >> 3134 LOAD_FAST                4 (qr)
+                          3136 RETURN_VALUE
                consts
                   None
                   'dataBytes'
                   'ErrorCorrection'
                   ''
                   ('version', 'encoding', 'message', 'error_correction')
                   7
@@ -3137,31 +3156,32 @@
                   'x'
                   3
                   11
                   'X'
                   -1
                   'No more space for data'
                names      ('qrutils', 'qr_encode_data', 'version', 'encoding', 'error_correction', 'msg', 'interleave_blocks', 'join', 'QR', 'enumerate', 'finderPattern', 'matrix', 'size', 'range', 'alignment_pattern_locations', 'alignmentPattern', 'value', 'QRVersion', 'v7', 'reserved_positions', 'len', 'print', 'qr_masking')
-               varnames   ('self', 'rawData', 'interleavedData', 'qr', 'posx', 'row', 'posy', 'col', 'i', 'value', 'patternLocations', 'patternLocation', 'offset', 'j', 'directionUD', 'directionLR', 'dataPos')
+               varnames   ('self', 'returnALL', 'rawData', 'interleavedData', 'qr', 'posx', 'row', 'posy', 'col', 'i', 'value', 'patternLocations', 'patternLocation', 'offset', 'j', 'directionUD', 'directionLR', 'dataPos', 'allPaterns', 'allPenaltyScores')
                freevars   ()
                cellvars   ()
                filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
                name       'generate'
                firstlineno 185
                lnotab
                   0x020356044e022a034e053201280122ff02043201280138ff0204320128
                   0138ff020522012201220122032201320122013803220138012201320404
                   01340126010c030401340126010c03320208011001100208012201220168
                   ff02ff0205300422010c01220122010c0122032401320324013203480122
                   012201360138fe0205320128010c0122fe02071401140104010401040126
                   022e012c010a0418010a01060118010a010a01060118020a01060118010a
                   010a0104030c010401040104010c0116010401140104010a020c010a020c
-                  011e0202d6262d600f
+                  011e0202d6262d680f04010a02
             None
-         names      ('__name__', '__module__', '__qualname__', 'qrutils', 'QREncoding', 'byte', 'QRVersion', 'v1', 'QRErrorCorrectionLevels', 'L', 'str', '__init__', '__str__', '__repr__', 'check', 'generate')
+            (False,)
+         names      ('__name__', '__module__', '__qualname__', 'qrutils', 'QREncoding', 'byte', 'QRVersion', 'v1', 'QRErrorCorrectionLevels', 'L', 'str', '__init__', '__str__', '__repr__', 'check', 'bool', 'generate')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
          name       'QRGenerator'
          firstlineno 164
          lnotab 0x0a017c06060306030608
@@ -3180,74 +3200,74 @@
             0000000000000000006a0200000000000000006a05000000000000000053
             007403000000000000000000006a0600000000000000007c00a6010000ab
             01000000000000000072117402000000000000000000006a020000000000
             0000006a07000000000000000053007403000000000000000000006a0800
             000000000000007c00a6010000ab01000000000000000072117402000000
             000000000000006a0200000000000000006a090000000000000000530064
             005300
-         364           0 RESUME                   0
+         367           0 RESUME                   0
          
-         366           2 LOAD_FAST                0 (msg)
+         369           2 LOAD_FAST                0 (msg)
                        4 LOAD_METHOD              0 (isnumeric)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 POP_JUMP_FORWARD_IF_FALSE    17 (to 76)
          
-         367          42 LOAD_GLOBAL              2 (qrutils)
+         370          42 LOAD_GLOBAL              2 (qrutils)
                       54 LOAD_ATTR                2 (QREncoding)
                       64 LOAD_ATTR                3 (numeric)
                       74 RETURN_VALUE
          
-         369     >>   76 LOAD_GLOBAL              3 (NULL + qrutils)
+         372     >>   76 LOAD_GLOBAL              3 (NULL + qrutils)
                       88 LOAD_ATTR                4 (is_alphanumeric)
                       98 LOAD_FAST                0 (msg)
                      100 PRECALL                  1
                      104 CALL                     1
                      114 POP_JUMP_FORWARD_IF_FALSE    17 (to 150)
          
-         370         116 LOAD_GLOBAL              2 (qrutils)
+         373         116 LOAD_GLOBAL              2 (qrutils)
                      128 LOAD_ATTR                2 (QREncoding)
                      138 LOAD_ATTR                5 (alphanumeric)
                      148 RETURN_VALUE
          
-         372     >>  150 LOAD_GLOBAL              3 (NULL + qrutils)
+         375     >>  150 LOAD_GLOBAL              3 (NULL + qrutils)
                      162 LOAD_ATTR                6 (is_byte)
                      172 LOAD_FAST                0 (msg)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_JUMP_FORWARD_IF_FALSE    17 (to 224)
          
-         373         190 LOAD_GLOBAL              2 (qrutils)
+         376         190 LOAD_GLOBAL              2 (qrutils)
                      202 LOAD_ATTR                2 (QREncoding)
                      212 LOAD_ATTR                7 (byte)
                      222 RETURN_VALUE
          
-         374     >>  224 LOAD_GLOBAL              3 (NULL + qrutils)
+         377     >>  224 LOAD_GLOBAL              3 (NULL + qrutils)
                      236 LOAD_ATTR                8 (is_kanji)
                      246 LOAD_FAST                0 (msg)
                      248 PRECALL                  1
                      252 CALL                     1
                      262 POP_JUMP_FORWARD_IF_FALSE    17 (to 298)
          
-         375         264 LOAD_GLOBAL              2 (qrutils)
+         378         264 LOAD_GLOBAL              2 (qrutils)
                      276 LOAD_ATTR                2 (QREncoding)
                      286 LOAD_ATTR                9 (kanji)
                      296 RETURN_VALUE
          
-         374     >>  298 LOAD_CONST               0 (None)
+         377     >>  298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          consts
             None
          names      ('isnumeric', 'qrutils', 'QREncoding', 'numeric', 'is_alphanumeric', 'alphanumeric', 'is_byte', 'byte', 'is_kanji', 'kanji')
          varnames   ('msg',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
          name       'get_encoding'
-         firstlineno 364
+         firstlineno 367
          lnotab 0x0202280122022801220228012201280122ff
       'encoding'
       'error_correction'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 6
@@ -3264,29 +3284,29 @@
             0100000000000000006a050000000000000000190000000000000000007c
             02190000000000000000007c056a06000000000000000019000000000000
             0000007c046b0000000000723c7c057d037400000000000000000000006a
             0300000000000000007401000000000000000000006a0400000000000000
             007c01a6010000ab0100000000000000006a050000000000000000190000
             000000000000007c02190000000000000000007c056a0600000000000000
             00190000000000000000007d048cc87c037c0266025300
-         379           0 RESUME                   0
+         382           0 RESUME                   0
          
-         380           2 LOAD_CONST               0 (None)
+         383           2 LOAD_CONST               0 (None)
                        4 STORE_FAST               3 (min_version)
          
-         382           6 LOAD_CONST               1 (9999999)
+         385           6 LOAD_CONST               1 (9999999)
                        8 STORE_FAST               4 (minlength)
          
-         383          10 LOAD_GLOBAL              0 (qrutils)
+         386          10 LOAD_GLOBAL              0 (qrutils)
                       22 LOAD_ATTR                1 (QRVersion)
                       32 GET_ITER
                  >>   34 FOR_ITER               199 (to 434)
                       36 STORE_FAST               5 (version)
          
-         384          38 LOAD_GLOBAL              5 (NULL + len)
+         387          38 LOAD_GLOBAL              5 (NULL + len)
                       50 LOAD_FAST                0 (msg)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 LOAD_GLOBAL              0 (qrutils)
                       78 LOAD_ATTR                3 (MAX_CHARACTERS)
                       88 LOAD_GLOBAL              1 (NULL + qrutils)
                      100 LOAD_ATTR                4 (QREncoding)
@@ -3316,18 +3336,18 @@
                      280 LOAD_FAST                5 (version)
                      282 LOAD_ATTR                6 (value)
                      292 BINARY_SUBSCR
                      302 LOAD_FAST                4 (minlength)
                      304 COMPARE_OP               0 (<)
                      310 POP_JUMP_FORWARD_IF_FALSE    60 (to 432)
          
-         385         312 LOAD_FAST                5 (version)
+         388         312 LOAD_FAST                5 (version)
                      314 STORE_FAST               3 (min_version)
          
-         386         316 LOAD_GLOBAL              0 (qrutils)
+         389         316 LOAD_GLOBAL              0 (qrutils)
                      328 LOAD_ATTR                3 (MAX_CHARACTERS)
                      338 LOAD_GLOBAL              1 (NULL + qrutils)
                      350 LOAD_ATTR                4 (QREncoding)
                      360 LOAD_FAST                1 (encoding)
                      362 PRECALL                  1
                      366 CALL                     1
                      376 LOAD_ATTR                5 (name)
@@ -3336,91 +3356,91 @@
                      398 BINARY_SUBSCR
                      408 LOAD_FAST                5 (version)
                      410 LOAD_ATTR                6 (value)
                      420 BINARY_SUBSCR
                      430 STORE_FAST               4 (minlength)
                  >>  432 JUMP_BACKWARD          200 (to 34)
          
-         388     >>  434 LOAD_FAST                3 (min_version)
+         391     >>  434 LOAD_FAST                3 (min_version)
                      436 LOAD_FAST                2 (error_correction)
                      438 BUILD_TUPLE              2
                      440 RETURN_VALUE
          consts
             None
             9999999
          names      ('qrutils', 'QRVersion', 'len', 'MAX_CHARACTERS', 'QREncoding', 'name', 'value')
          varnames   ('msg', 'encoding', 'error_correction', 'min_version', 'minlength', 'version')
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
          name       'get_min_version'
-         firstlineno 379
+         firstlineno 382
          lnotab 0x0201040204011c01ff00130104017602
       code
          argcount  : 2
          nlocals   : 7
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007d027403000000000000000000007c007c027c01a6030000ab03000000
             00000000005c0200007d037d047405000000000000000000007c007c027c
             037c04ac01a6040000ab0400000000000000007d057c05a0030000000000
             000000000000000000000000000000a6000000ab0000000000000000007d
             067c065300
-         390           0 RESUME                   0
+         393           0 RESUME                   0
          
-         392           2 LOAD_GLOBAL              1 (NULL + get_encoding)
+         395           2 LOAD_GLOBAL              1 (NULL + get_encoding)
                       14 LOAD_FAST                0 (msg)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               2 (encoding)
          
-         394          32 LOAD_GLOBAL              3 (NULL + get_min_version)
+         397          32 LOAD_GLOBAL              3 (NULL + get_min_version)
                       44 LOAD_FAST                0 (msg)
                       46 LOAD_FAST                2 (encoding)
                       48 LOAD_FAST                1 (error_correction)
                       50 PRECALL                  3
                       54 CALL                     3
                       64 UNPACK_SEQUENCE          2
                       68 STORE_FAST               3 (version)
                       70 STORE_FAST               4 (err)
          
-         396          72 LOAD_GLOBAL              5 (NULL + QRGenerator)
+         399          72 LOAD_GLOBAL              5 (NULL + QRGenerator)
                       84 LOAD_FAST                0 (msg)
                       86 LOAD_FAST                2 (encoding)
                       88 LOAD_FAST                3 (version)
                       90 LOAD_FAST                4 (err)
                       92 KW_NAMES                 1
                       94 PRECALL                  4
                       98 CALL                     4
                      108 STORE_FAST               5 (generator)
          
-         397         110 LOAD_FAST                5 (generator)
+         400         110 LOAD_FAST                5 (generator)
                      112 LOAD_METHOD              3 (generate)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 STORE_FAST               6 (qr)
          
-         399         150 LOAD_FAST                6 (qr)
+         402         150 LOAD_FAST                6 (qr)
                      152 RETURN_VALUE
          consts
             None
             ('msg', 'encoding', 'version', 'error_correction')
          names      ('get_encoding', 'get_min_version', 'QRGenerator', 'generate')
          varnames   ('msg', 'error_correction', 'encoding', 'version', 'err', 'generator', 'qr')
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
          name       'smallest_qr'
-         firstlineno 390
+         firstlineno 393
          lnotab 0x02021e02280226012802
    names      ('', 'qrutils', 'PIL', 'Image', 'numpy', 'np', 'enum', 'Enum', 'finderPattern', 'alignmentPattern', 'ModuleColors', 'NewColour', 'QRColour', 'QR', 'QRGenerator', 'str', 'get_encoding', 'QREncoding', 'byte', 'QRErrorCorrectionLevels', 'Q', 'get_min_version', 'smallest_qr')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrgenerator.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02030c010c0108010c0406010601060106010601060106f9040b06
-      0106010601060106fb04091a051a0c1c141a631a7f00490c0f560b
+      0106010601060106fb04091a051a0c1c141a631a7f004c0c0f560b
```

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-39.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-311.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-39.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-311.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1ef8cd64 (Sat Aug  5 07:19:58 2023 UTC)
-files sz: 51478
+moddate:  0x0b18ce64 (Sat Aug  5 09:36:11 2023 UTC)
+files sz: 51646
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -1236,38 +1236,38 @@
                3140 LOAD_CONST             122 ('return')
                3142 LOAD_NAME               52 (list)
                3144 BUILD_TUPLE             12
                3146 LOAD_CONST             158 (<code object qr_masking, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1486>)
                3148 MAKE_FUNCTION            5 (defaults, annotations)
                3150 STORE_NAME              69 (qr_masking)
    
-   1541        3152 LOAD_CONST             126 ('data')
+   1546        3152 LOAD_CONST             126 ('data')
                3154 LOAD_NAME               20 (str)
                3156 LOAD_CONST             122 ('return')
                3158 LOAD_NAME               70 (bool)
                3160 BUILD_TUPLE              4
-               3162 LOAD_CONST             159 (<code object is_kanji, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1541>)
+               3162 LOAD_CONST             159 (<code object is_kanji, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1546>)
                3164 MAKE_FUNCTION            4 (annotations)
                3166 STORE_NAME              71 (is_kanji)
    
-   1548        3168 LOAD_CONST             126 ('data')
+   1553        3168 LOAD_CONST             126 ('data')
                3170 LOAD_NAME               20 (str)
                3172 LOAD_CONST             122 ('return')
                3174 LOAD_NAME               70 (bool)
                3176 BUILD_TUPLE              4
-               3178 LOAD_CONST             160 (<code object is_byte, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1548>)
+               3178 LOAD_CONST             160 (<code object is_byte, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1553>)
                3180 MAKE_FUNCTION            4 (annotations)
                3182 STORE_NAME              72 (is_byte)
    
-   1555        3184 LOAD_CONST             126 ('data')
+   1560        3184 LOAD_CONST             126 ('data')
                3186 LOAD_NAME               20 (str)
                3188 LOAD_CONST             122 ('return')
                3190 LOAD_NAME               70 (bool)
                3192 BUILD_TUPLE              4
-               3194 LOAD_CONST             161 (<code object is_alphanumeric, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1555>)
+               3194 LOAD_CONST             161 (<code object is_alphanumeric, file "/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py", line 1560>)
                3196 MAKE_FUNCTION            4 (annotations)
                3198 STORE_NAME              73 (is_alphanumeric)
                3200 LOAD_CONST               3 (None)
                3202 RETURN_VALUE
    consts
       0
       ('Path',)
@@ -9078,36 +9078,40 @@
          firstlineno 1437
          lnotab
             0x0203260324010c0144023e0224016a022401640224010c014a02440316
             01240204012401240162010cfe020404012401240162010cfe020a
       'masks'
       code
          argcount  : 5
-         nlocals   : 16
+         nlocals   : 18
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007401000000000000000000007c01a6010000ab0100000000000000006b
             0300000000720f7403000000000000000000006401a6010000ab01000000
-            0000000000820164027d0564027d0667007d077405000000000000000000
-            007c00a6010000ab0100000000000000007d087407000000000000000000
-            007401000000000000000000007c04a6010000ab010000000000000000a6
-            010000ab01000000000000000044005da77d097409000000000000000000
-            007c087c027c047c09190000000000000000007c03a6040000ab04000000
-            00000000007d00740b000000000000000000007c00a6010000ab01000000
-            000000000044005d325c0200007d0a7d0b740b000000000000000000007c
-            0ba6010000ab01000000000000000044005d1d5c0200007d0c7d0d740d00
-            0000000000000000007c0da6010000ab0100000000000000007c007c0a19
-            0000000000000000007c0c3c0000008c1e8c33740f000000000000000000
-            007c007c047c09190000000000000000007c01a6030000ab030000000000
-            0000007d0e7411000000000000000000007c0ea6010000ab010000000000
-            0000007d0f7c0f7c066b000000000073067c0964026b020000000072197c
-            047c09190000000000000000007d057c0f7d067405000000000000000000
-            007c0ea6010000ab0100000000000000007d078ca87c075300
+            0000000000820164027d0564027d0667007d0767007d0867007d09740500
+            0000000000000000007c00a6010000ab0100000000000000007d0a740700
+            0000000000000000007401000000000000000000007c04a6010000ab0100
+            00000000000000a6010000ab01000000000000000044005dde7d0b740900
+            0000000000000000007c0a7c027c047c0b190000000000000000007c03a6
+            040000ab0400000000000000007d00740b000000000000000000007c00a6
+            010000ab01000000000000000044005d325c0200007d0c7d0d740b000000
+            000000000000007c0da6010000ab01000000000000000044005d1d5c0200
+            007d0e7d0f740d000000000000000000007c0fa6010000ab010000000000
+            0000007c007c0c190000000000000000007c0e3c0000008c1e8c33740f00
+            0000000000000000007c007c047c0b190000000000000000007c01a60300
+            00ab0300000000000000007d107411000000000000000000007c10a60100
+            00ab0100000000000000007d117c117c066b000000000073067c0b64026b
+            020000000072197c047c0b190000000000000000007d057c117d06740500
+            0000000000000000007c10a6010000ab0100000000000000007d077c09a0
+            0900000000000000000000000000000000000000007c11a6010000ab0100
+            0000000000000001007c08a0090000000000000000000000000000000000
+            0000007405000000000000000000007c10a6010000ab0100000000000000
+            00a6010000ab01000000000000000001008cdf7c077c087c0966035300
          1486           0 RESUME                   0
          
          1487           2 LOAD_GLOBAL              1 (NULL + len)
                        14 LOAD_FAST                0 (data)
                        16 PRECALL                  1
                        20 CALL                     1
                        30 LOAD_GLOBAL              1 (NULL + len)
@@ -9128,158 +9132,184 @@
          
          1492         100 LOAD_CONST               2 (0)
                       102 STORE_FAST               6 (penaltyScores)
          
          1493         104 BUILD_LIST               0
                       106 STORE_FAST               7 (maskedPatterns)
          
-         1501         108 LOAD_GLOBAL              5 (NULL + deepcopy)
-                      120 LOAD_FAST                0 (data)
-                      122 PRECALL                  1
-                      126 CALL                     1
-                      136 STORE_FAST               8 (originalData)
-         
-         1502         138 LOAD_GLOBAL              7 (NULL + range)
-                      150 LOAD_GLOBAL              1 (NULL + len)
-                      162 LOAD_FAST                4 (masks)
-                      164 PRECALL                  1
-                      168 CALL                     1
-                      178 PRECALL                  1
-                      182 CALL                     1
-                      192 GET_ITER
-                  >>  194 FOR_ITER               167 (to 530)
-                      196 STORE_FAST               9 (i)
-         
-         1505         198 LOAD_GLOBAL              9 (NULL + add_format_version_information)
-                      210 LOAD_FAST                8 (originalData)
-                      212 LOAD_FAST                2 (errCorrection)
-                      214 LOAD_FAST                4 (masks)
-                      216 LOAD_FAST                9 (i)
-                      218 BINARY_SUBSCR
-                      228 LOAD_FAST                3 (version)
-                      230 PRECALL                  4
-                      234 CALL                     4
-                      244 STORE_FAST               0 (data)
-         
-         1508         246 LOAD_GLOBAL             11 (NULL + enumerate)
-                      258 LOAD_FAST                0 (data)
-                      260 PRECALL                  1
-                      264 CALL                     1
-                      274 GET_ITER
-                  >>  276 FOR_ITER                50 (to 378)
-                      278 UNPACK_SEQUENCE          2
-                      282 STORE_FAST              10 (posx)
-                      284 STORE_FAST              11 (row)
-         
-         1509         286 LOAD_GLOBAL             11 (NULL + enumerate)
-                      298 LOAD_FAST               11 (row)
-                      300 PRECALL                  1
-                      304 CALL                     1
-                      314 GET_ITER
-                  >>  316 FOR_ITER                29 (to 376)
-                      318 UNPACK_SEQUENCE          2
-                      322 STORE_FAST              12 (posy)
-                      324 STORE_FAST              13 (col)
-         
-         1510         326 LOAD_GLOBAL             13 (NULL + int)
-                      338 LOAD_FAST               13 (col)
-                      340 PRECALL                  1
-                      344 CALL                     1
-                      354 LOAD_FAST                0 (data)
-                      356 LOAD_FAST               10 (posx)
-                      358 BINARY_SUBSCR
-                      368 LOAD_FAST               12 (posy)
-                      370 STORE_SUBSCR
-                      374 JUMP_BACKWARD           30 (to 316)
-         
-         1509     >>  376 JUMP_BACKWARD           51 (to 276)
-         
-         1517     >>  378 LOAD_GLOBAL             15 (NULL + apply_mask)
-                      390 LOAD_FAST                0 (data)
-                      392 LOAD_FAST                4 (masks)
-                      394 LOAD_FAST                9 (i)
-                      396 BINARY_SUBSCR
-                      406 LOAD_FAST                1 (reservedPositions)
-                      408 PRECALL                  3
-                      412 CALL                     3
-                      422 STORE_FAST              14 (maskedData)
-         
-         1524         424 LOAD_GLOBAL             17 (NULL + calculate_penalty_score)
-                      436 LOAD_FAST               14 (maskedData)
-                      438 PRECALL                  1
-                      442 CALL                     1
-                      452 STORE_FAST              15 (score)
-         
-         1525         454 LOAD_FAST               15 (score)
-                      456 LOAD_FAST                6 (penaltyScores)
-                      458 COMPARE_OP               0 (<)
-                      464 POP_JUMP_FORWARD_IF_TRUE     6 (to 478)
-                      466 LOAD_FAST                9 (i)
-                      468 LOAD_CONST               2 (0)
-                      470 COMPARE_OP               2 (==)
-                      476 POP_JUMP_FORWARD_IF_FALSE    25 (to 528)
-         
-         1526     >>  478 LOAD_FAST                4 (masks)
-                      480 LOAD_FAST                9 (i)
-                      482 BINARY_SUBSCR
-                      492 STORE_FAST               5 (maskNum)
+         1494         108 BUILD_LIST               0
+                      110 STORE_FAST               8 (allPatterns)
          
-         1527         494 LOAD_FAST               15 (score)
-                      496 STORE_FAST               6 (penaltyScores)
+         1495         112 BUILD_LIST               0
+                      114 STORE_FAST               9 (allPenaltyScores)
          
-         1528         498 LOAD_GLOBAL              5 (NULL + deepcopy)
-                      510 LOAD_FAST               14 (maskedData)
-                      512 PRECALL                  1
-                      516 CALL                     1
-                      526 STORE_FAST               7 (maskedPatterns)
-                  >>  528 JUMP_BACKWARD          168 (to 194)
+         1503         116 LOAD_GLOBAL              5 (NULL + deepcopy)
+                      128 LOAD_FAST                0 (data)
+                      130 PRECALL                  1
+                      134 CALL                     1
+                      144 STORE_FAST              10 (originalData)
+         
+         1504         146 LOAD_GLOBAL              7 (NULL + range)
+                      158 LOAD_GLOBAL              1 (NULL + len)
+                      170 LOAD_FAST                4 (masks)
+                      172 PRECALL                  1
+                      176 CALL                     1
+                      186 PRECALL                  1
+                      190 CALL                     1
+                      200 GET_ITER
+                  >>  202 FOR_ITER               222 (to 648)
+                      204 STORE_FAST              11 (i)
+         
+         1507         206 LOAD_GLOBAL              9 (NULL + add_format_version_information)
+                      218 LOAD_FAST               10 (originalData)
+                      220 LOAD_FAST                2 (errCorrection)
+                      222 LOAD_FAST                4 (masks)
+                      224 LOAD_FAST               11 (i)
+                      226 BINARY_SUBSCR
+                      236 LOAD_FAST                3 (version)
+                      238 PRECALL                  4
+                      242 CALL                     4
+                      252 STORE_FAST               0 (data)
+         
+         1510         254 LOAD_GLOBAL             11 (NULL + enumerate)
+                      266 LOAD_FAST                0 (data)
+                      268 PRECALL                  1
+                      272 CALL                     1
+                      282 GET_ITER
+                  >>  284 FOR_ITER                50 (to 386)
+                      286 UNPACK_SEQUENCE          2
+                      290 STORE_FAST              12 (posx)
+                      292 STORE_FAST              13 (row)
+         
+         1511         294 LOAD_GLOBAL             11 (NULL + enumerate)
+                      306 LOAD_FAST               13 (row)
+                      308 PRECALL                  1
+                      312 CALL                     1
+                      322 GET_ITER
+                  >>  324 FOR_ITER                29 (to 384)
+                      326 UNPACK_SEQUENCE          2
+                      330 STORE_FAST              14 (posy)
+                      332 STORE_FAST              15 (col)
+         
+         1512         334 LOAD_GLOBAL             13 (NULL + int)
+                      346 LOAD_FAST               15 (col)
+                      348 PRECALL                  1
+                      352 CALL                     1
+                      362 LOAD_FAST                0 (data)
+                      364 LOAD_FAST               12 (posx)
+                      366 BINARY_SUBSCR
+                      376 LOAD_FAST               14 (posy)
+                      378 STORE_SUBSCR
+                      382 JUMP_BACKWARD           30 (to 324)
+         
+         1511     >>  384 JUMP_BACKWARD           51 (to 284)
+         
+         1519     >>  386 LOAD_GLOBAL             15 (NULL + apply_mask)
+                      398 LOAD_FAST                0 (data)
+                      400 LOAD_FAST                4 (masks)
+                      402 LOAD_FAST               11 (i)
+                      404 BINARY_SUBSCR
+                      414 LOAD_FAST                1 (reservedPositions)
+                      416 PRECALL                  3
+                      420 CALL                     3
+                      430 STORE_FAST              16 (maskedData)
+         
+         1526         432 LOAD_GLOBAL             17 (NULL + calculate_penalty_score)
+                      444 LOAD_FAST               16 (maskedData)
+                      446 PRECALL                  1
+                      450 CALL                     1
+                      460 STORE_FAST              17 (score)
+         
+         1527         462 LOAD_FAST               17 (score)
+                      464 LOAD_FAST                6 (penaltyScores)
+                      466 COMPARE_OP               0 (<)
+                      472 POP_JUMP_FORWARD_IF_TRUE     6 (to 486)
+                      474 LOAD_FAST               11 (i)
+                      476 LOAD_CONST               2 (0)
+                      478 COMPARE_OP               2 (==)
+                      484 POP_JUMP_FORWARD_IF_FALSE    25 (to 536)
+         
+         1528     >>  486 LOAD_FAST                4 (masks)
+                      488 LOAD_FAST               11 (i)
+                      490 BINARY_SUBSCR
+                      500 STORE_FAST               5 (maskNum)
+         
+         1529         502 LOAD_FAST               17 (score)
+                      504 STORE_FAST               6 (penaltyScores)
+         
+         1530         506 LOAD_GLOBAL              5 (NULL + deepcopy)
+                      518 LOAD_FAST               16 (maskedData)
+                      520 PRECALL                  1
+                      524 CALL                     1
+                      534 STORE_FAST               7 (maskedPatterns)
+         
+         1532     >>  536 LOAD_FAST                9 (allPenaltyScores)
+                      538 LOAD_METHOD              9 (append)
+                      560 LOAD_FAST               17 (score)
+                      562 PRECALL                  1
+                      566 CALL                     1
+                      576 POP_TOP
          
-         1539     >>  530 LOAD_FAST                7 (maskedPatterns)
-                      532 RETURN_VALUE
+         1533         578 LOAD_FAST                8 (allPatterns)
+                      580 LOAD_METHOD              9 (append)
+                      602 LOAD_GLOBAL              5 (NULL + deepcopy)
+                      614 LOAD_FAST               16 (maskedData)
+                      616 PRECALL                  1
+                      620 CALL                     1
+                      630 PRECALL                  1
+                      634 CALL                     1
+                      644 POP_TOP
+                      646 JUMP_BACKWARD          223 (to 202)
+         
+         1544     >>  648 LOAD_FAST                7 (maskedPatterns)
+                      650 LOAD_FAST                8 (allPatterns)
+                      652 LOAD_FAST                9 (allPenaltyScores)
+                      654 BUILD_TUPLE              3
+                      656 RETURN_VALUE
          consts
             None
             'The data and reserved positions lists must have the same length.'
             0
-         names      ('len', 'Exception', 'deepcopy', 'range', 'add_format_version_information', 'enumerate', 'int', 'apply_mask', 'calculate_penalty_score')
-         varnames   ('data', 'reservedPositions', 'errCorrection', 'version', 'masks', 'maskNum', 'penaltyScores', 'maskedPatterns', 'originalData', 'i', 'posx', 'row', 'posy', 'col', 'maskedData', 'score')
+         names      ('len', 'Exception', 'deepcopy', 'range', 'add_format_version_information', 'enumerate', 'int', 'apply_mask', 'calculate_penalty_score', 'append')
+         varnames   ('data', 'reservedPositions', 'errCorrection', 'version', 'masks', 'maskNum', 'penaltyScores', 'maskedPatterns', 'allPatterns', 'allPenaltyScores', 'originalData', 'i', 'posx', 'row', 'posy', 'col', 'maskedData', 'score')
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py'
          name       'qr_masking'
          firstlineno 1486
          lnotab
-            0x020140011e030401040104081e013c0330032801280132ff02082e071e
-            01180110010401200b
+            0x020140011e03040104010401040104081e013c0330032801280132ff02
+            082e071e011801100104011e022a01460b
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970009007c00a000000000000000000000000000000000000000000064
             01a6010000ab010000000000000000010064025300230001005900640353
             00780359007701
-         1541           0 RESUME                   0
+         1546           0 RESUME                   0
          
-         1542           2 NOP
+         1547           2 NOP
          
-         1543           4 LOAD_FAST                0 (data)
+         1548           4 LOAD_FAST                0 (data)
                         6 LOAD_METHOD              0 (encode)
                        28 LOAD_CONST               1 ('shift-jis')
                        30 PRECALL                  1
                        34 CALL                     1
                        44 POP_TOP
          
-         1544          46 LOAD_CONST               2 (True)
+         1549          46 LOAD_CONST               2 (True)
                        48 RETURN_VALUE
                   >>   50 PUSH_EXC_INFO
          
-         1545          52 POP_TOP
+         1550          52 POP_TOP
          
-         1546          54 POP_EXCEPT
+         1551          54 POP_EXCEPT
                        56 LOAD_CONST               3 (False)
                        58 RETURN_VALUE
                   >>   60 COPY                     3
                        62 POP_EXCEPT
                        64 RERAISE                  1
          ExceptionTable:
            4 to 44 -> 50 [0]
@@ -9291,43 +9321,43 @@
             False
          names      ('encode',)
          varnames   ('data',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py'
          name       'is_kanji'
-         firstlineno 1541
+         firstlineno 1546
          lnotab 0x020102012a0106010201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970009007c00a000000000000000000000000000000000000000000064
             01a6010000ab010000000000000000010064025300230001005900640353
             00780359007701
-         1548           0 RESUME                   0
+         1553           0 RESUME                   0
          
-         1549           2 NOP
+         1554           2 NOP
          
-         1550           4 LOAD_FAST                0 (data)
+         1555           4 LOAD_FAST                0 (data)
                         6 LOAD_METHOD              0 (encode)
                        28 LOAD_CONST               1 ('ISO-8859-1')
                        30 PRECALL                  1
                        34 CALL                     1
                        44 POP_TOP
          
-         1551          46 LOAD_CONST               2 (True)
+         1556          46 LOAD_CONST               2 (True)
                        48 RETURN_VALUE
                   >>   50 PUSH_EXC_INFO
          
-         1552          52 POP_TOP
+         1557          52 POP_TOP
          
-         1553          54 POP_EXCEPT
+         1558          54 POP_EXCEPT
                        56 LOAD_CONST               3 (False)
                        58 RETURN_VALUE
                   >>   60 COPY                     3
                        62 POP_EXCEPT
                        64 RERAISE                  1
          ExceptionTable:
            4 to 44 -> 50 [0]
@@ -9339,55 +9369,55 @@
             False
          names      ('encode',)
          varnames   ('data',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py'
          name       'is_byte'
-         firstlineno 1548
+         firstlineno 1553
          lnotab 0x020102012a0106010201
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 3
          flags     : 3
          code
             0x97007c0044005d0e7d017c017400000000000000000000007601720301
             00640153008c0f64025300
-         1555           0 RESUME                   0
+         1560           0 RESUME                   0
          
-         1556           2 LOAD_FAST                0 (data)
+         1561           2 LOAD_FAST                0 (data)
                         4 GET_ITER
                   >>    6 FOR_ITER                14 (to 36)
                         8 STORE_FAST               1 (char)
          
-         1557          10 LOAD_FAST                1 (char)
+         1562          10 LOAD_FAST                1 (char)
                        12 LOAD_GLOBAL              0 (AlphanumericVals)
                        24 CONTAINS_OP              1
                        26 POP_JUMP_FORWARD_IF_FALSE     3 (to 34)
          
-         1558          28 POP_TOP
+         1563          28 POP_TOP
                        30 LOAD_CONST               1 (False)
                        32 RETURN_VALUE
          
-         1557     >>   34 JUMP_BACKWARD           15 (to 6)
+         1562     >>   34 JUMP_BACKWARD           15 (to 6)
          
-         1560     >>   36 LOAD_CONST               2 (True)
+         1565     >>   36 LOAD_CONST               2 (True)
                        38 RETURN_VALUE
          consts
             None
             False
             True
          names      ('AlphanumericVals',)
          varnames   ('data', 'char')
          freevars   ()
          cellvars   ()
          filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py'
          name       'is_alphanumeric'
-         firstlineno 1555
+         firstlineno 1560
          lnotab 0x02010801120106ff0203
    names      ('pathlib', 'Path', 'enum', 'Enum', 'numpy', 'np', 'pandas', 'pd', 'copy', 'deepcopy', '__file__', 'parent', 'FILE_PATH', 'read_csv', '__CAPABILITIES', '__ERR_CORR', 'replace', 'nan', '__GF', '__ALIGNMENT', 'str', '__FORMAT', '__VERSION', 'GF256', 'iterrows', 'index', 'row', 'append', 'MAX_CHARACTERS', 'unique', 'mode', 'error', 'version', 'DATA_CODEWORDS', 'ERR_CORR_CODEWORDS_BLOCK', 'GROUPS', 'int', 'ALIGNMENT_PATTERNS', 'split', 'locationsArray', 'FORMAT_INFORMATION', 'mask', 'VERSION_INFORMATION', 'PAD_BYTES', 'QREncoding', 'QRVersion', 'AlphanumericVals', 'QRErrorCorrectionLevels', 'qr_size', 'qr_count_indicator_size', 'qr_count_indicator', 'find_indices', 'list', 'multiply_polynomials', 'generator_polynomial', 'remainder_bits', 'interleave_blocks', 'divide_polynomials', 'dict', 'qr_encode_data_numeric', 'qr_encode_data_alphanumeric', 'qr_encode_data_byte', 'qr_encode_data_kanji', 'qr_encode_data', 'alignment_pattern_locations', 'calculate_penalty_score', 'apply_mask', 'add_format_version_information', 'range', 'qr_masking', 'bool', 'is_kanji', 'is_byte', 'is_alphanumeric')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parzival1918/Documents/GitHub/barcodes-uc/barcodes_uc/qrcodes/qrutils.py'
    name       '<module>'
@@ -9401,9 +9431,9 @@
       0130010c023201240402010201020102010201020308031c071c2b020104
       ff020204fe020304fd020404fc020504fb020604fa020704f9020804f802
       0904f7020a04f6020b04f5020c04f4020d04f3020e04f2020f04f1021004
       f0021104ef041204ee021304ed021404ec021504eb021604ea021704e902
       1804e8021904e7021a04e6021b04e5021c04e4021d04e3021e04e2021f04
       e1022004e0022104df022204de0423020102010201020102010201020102
       010201020102d308311a0710041422180806071c401445100f18231c4818
-      7f003e187f0026187f0035187f00311c0f1012106818381c315637100710
+      7f003e187f0026187f0035187f00311c0f1012106818381c31563c100710
       07
```

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-39.pyc` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrgenerator.py` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/qrgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         max_character_count = qrutils.MAX_CHARACTERS[qrutils.QREncoding(self.encoding).name][self.error_correction][self.version]
 
         if len(self.msg) >= max_character_count:
             return False
         else:
             return True
         
-    def generate(self):
+    def generate(self, returnALL: bool = False):
         # if not self.check():
         #     raise ValueError("Message is too long for the specified encoding, version and error correction level.")
         rawData = qrutils.qr_encode_data(self.version, self.encoding, self.error_correction, self.msg)
         # print(rawData)
 
         #interleave data blocks and error correction blocks if necessary
         interleavedData = qrutils.interleave_blocks(rawData['dataBytes'], rawData['ErrorCorrection'], self.version)
@@ -339,30 +339,33 @@
 
             if posy < 0:
                 print('No more space for data')
                 #exit loop
                 break
                 
         #9 - Masking
-        qr.matrix = qrutils.qr_masking(qr.matrix, qr.reserved_positions, self.error_correction, self.version)
+        qr.matrix, allPaterns, allPenaltyScores = qrutils.qr_masking(qr.matrix, qr.reserved_positions, self.error_correction, self.version)
         # originalMatrix = qr.matrix
         # for i in range(8):
         #     qr.matrix = qrutils.qr_masking(originalMatrix, qr.reserved_positions, self.error_correction, self.version, [i])
         #     #Turn every position into int 
         #     #TODO: Find a better way to do this
         #     for posx,row in enumerate(qr.matrix):
         #         for posy,col in enumerate(row):
         #             qr.matrix[posx][posy] = int(col)
             
         #     qr.show()
 
         # print(qr)
         # print(dataPos, len(interleavedData), (len(interleavedData)-dataPos))
 
-        return qr
+        if returnALL:
+            return qr, allPaterns, allPenaltyScores
+        else:
+            return qr
 
 #Function to get the correct encoding for the message
 def get_encoding(msg: str):
     #Check if message is numeric
     if msg.isnumeric():
         return qrutils.QREncoding.numeric
     #Check if message is alphanumeric
```

### Comparing `barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrutils.py` & `barcodes_uc-0.8.0/barcodes_uc/qrcodes/qrutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1487,14 +1487,16 @@
     if len(data) != len(reservedPositions):
         raise Exception('The data and reserved positions lists must have the same length.')
     
     #Apply all 8 masks and calculate the penalty score
     maskNum = 0
     penaltyScores = 0
     maskedPatterns = []
+    allPatterns = []
+    allPenaltyScores = []
 
     # for row in reservedPositions:
     #     for col in row:
     #         print(col, end='')
     #     print()
     # print()
 
@@ -1523,24 +1525,27 @@
 
         score = calculate_penalty_score(maskedData)
         if score < penaltyScores or i == 0:
             maskNum = masks[i]
             penaltyScores = score
             maskedPatterns = deepcopy(maskedData)
 
+        allPenaltyScores.append(score)
+        allPatterns.append(deepcopy(maskedData))
+
     #Choose the mask with the lowest penalty score
     # print(f"Mask {maskNum} has the lowest penalty score: {penaltyScores}")
 
     # for row in maskedPatterns:
     #         for col in row:
     #             print(col, end='')
     #         print()
     # print()
     
-    return maskedPatterns#, maskNum
+    return maskedPatterns, allPatterns, allPenaltyScores #, maskNum
 
 def is_kanji(data: str) -> bool:
     try:
         data.encode('shift-jis')
         return True
     except:
         return False
```

### Comparing `barcodes_uc-0.7.0/data/GF256.csv` & `barcodes_uc-0.8.0/data/GF256.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/data/alignment_locations.csv` & `barcodes_uc-0.8.0/data/alignment_locations.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/data/capabilities.csv` & `barcodes_uc-0.8.0/data/capabilities.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/data/error_correction_table.csv` & `barcodes_uc-0.8.0/data/error_correction_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/data/format_table.csv` & `barcodes_uc-0.8.0/data/format_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/data/version_table.csv` & `barcodes_uc-0.8.0/data/version_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/pyproject.toml` & `barcodes_uc-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "barcodes-uc"
-version = "0.7.0"
+version = "0.8.0"
 description = "A library to generate barcodes"
 authors = ["Pedro Juan Royo <pedro.juan.royo@gmail.com>"]
 readme = "README.md"
 packages = [{include = "barcodes_uc"}]
 include = ["data/*","requirements.txt"]
 exclude = ["fastapi/*"]
 repository = "https://github.com/Parzival1918/barcodes-uc"
```

### Comparing `barcodes_uc-0.7.0/requirements.txt` & `barcodes_uc-0.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.7.0/PKG-INFO` & `barcodes_uc-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barcodes-uc
-Version: 0.7.0
+Version: 0.8.0
 Summary: A library to generate barcodes
 Home-page: https://github.com/Parzival1918/barcodes-uc
 Author: Pedro Juan Royo
 Author-email: pedro.juan.royo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

