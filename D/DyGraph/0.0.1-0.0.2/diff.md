# Comparing `tmp/DyGraph-0.0.1.tar.gz` & `tmp/DyGraph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DyGraph-0.0.1.tar", last modified: Sun Apr 30 20:03:04 2023, max compression
+gzip compressed data, was "DyGraph-0.0.2.tar", last modified: Sat Aug  5 22:49:40 2023, max compression
```

## Comparing `DyGraph-0.0.1.tar` & `DyGraph-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 20:03:04.089697 DyGraph-0.0.1/
--rw-rw-rw-   0        0        0     1102 2023-04-26 16:02:16.000000 DyGraph-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1218 2023-04-30 20:03:04.090330 DyGraph-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-26 16:17:22.000000 DyGraph-0.0.1/README.md
--rw-rw-rw-   0        0        0      228 2023-04-26 11:53:06.000000 DyGraph-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1134 2023-04-30 20:03:04.091329 DyGraph-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-04-23 21:57:56.000000 DyGraph-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:03:04.033812 DyGraph-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 20:03:04.077822 DyGraph-0.0.1/src/DyGraph/
--rw-rw-rw-   0        0        0     5064 2023-04-28 10:30:15.000000 DyGraph-0.0.1/src/DyGraph/RootDygl.py
--rw-rw-rw-   0        0        0      246 2023-04-27 22:56:23.000000 DyGraph-0.0.1/src/DyGraph/__init__.py
--rw-rw-rw-   0        0        0    11329 2023-04-28 10:26:26.000000 DyGraph-0.0.1/src/DyGraph/dyg_outer_em.py
--rw-rw-rw-   0        0        0    11262 2023-04-28 10:44:48.000000 DyGraph-0.0.1/src/DyGraph/dygl_inner_em.py
--rw-rw-rw-   0        0        0    24554 2023-04-27 22:57:54.000000 DyGraph-0.0.1/src/DyGraph/dygl_utils.py
--rw-rw-rw-   0        0        0     4581 2023-04-28 10:26:56.000000 DyGraph-0.0.1/src/DyGraph/sgl_inner_em.py
--rw-rw-rw-   0        0        0     4924 2023-04-28 10:25:37.000000 DyGraph-0.0.1/src/DyGraph/sgl_outer_em.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:03:04.088825 DyGraph-0.0.1/src/DyGraph.egg-info/
--rw-rw-rw-   0        0        0     1218 2023-04-30 20:03:04.000000 DyGraph-0.0.1/src/DyGraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2023-04-30 20:03:04.000000 DyGraph-0.0.1/src/DyGraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 20:03:04.000000 DyGraph-0.0.1/src/DyGraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-29 17:35:32.000000 DyGraph-0.0.1/src/DyGraph.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2023-04-30 20:03:04.000000 DyGraph-0.0.1/src/DyGraph.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-30 20:03:04.000000 DyGraph-0.0.1/src/DyGraph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 22:49:40.465489 DyGraph-0.0.2/
+-rw-rw-rw-   0        0        0     1102 2023-06-07 13:00:07.000000 DyGraph-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3286 2023-08-05 22:49:40.466549 DyGraph-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2374 2023-06-07 13:00:07.000000 DyGraph-0.0.2/README.md
+-rw-rw-rw-   0        0        0      228 2023-06-07 13:00:07.000000 DyGraph-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1143 2023-08-05 22:49:40.475360 DyGraph-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-06-07 13:00:07.000000 DyGraph-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 22:49:40.287943 DyGraph-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 22:49:40.349377 DyGraph-0.0.2/src/CovReg/
+-rw-rw-rw-   0        0        0      334 2023-08-04 07:50:57.000000 DyGraph-0.0.2/src/CovReg/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-08-05 21:37:01.000000 DyGraph-0.0.2/src/CovReg/covreg.py
+-rw-rw-rw-   0        0        0    13227 2023-08-05 01:55:39.000000 DyGraph-0.0.2/src/CovReg/graphcovreg.py
+drwxrwxrwx   0        0        0        0 2023-08-05 22:49:40.381201 DyGraph-0.0.2/src/DyGraph/
+-rw-rw-rw-   0        0        0     5064 2023-06-07 13:00:07.000000 DyGraph-0.0.2/src/DyGraph/RootDygl.py
+-rw-rw-rw-   0        0        0      250 2023-08-04 03:06:35.000000 DyGraph-0.0.2/src/DyGraph/__init__.py
+-rw-rw-rw-   0        0        0    11758 2023-07-23 00:51:58.000000 DyGraph-0.0.2/src/DyGraph/dyg_outer_em.py
+-rw-rw-rw-   0        0        0    11690 2023-07-23 00:51:58.000000 DyGraph-0.0.2/src/DyGraph/dygl_inner_em.py
+-rw-rw-rw-   0        0        0    24554 2023-06-07 13:00:07.000000 DyGraph-0.0.2/src/DyGraph/dygl_utils.py
+-rw-rw-rw-   0        0        0     4581 2023-06-07 13:00:07.000000 DyGraph-0.0.2/src/DyGraph/sgl_inner_em.py
+-rw-rw-rw-   0        0        0     4924 2023-06-07 13:00:07.000000 DyGraph-0.0.2/src/DyGraph/sgl_outer_em.py
+drwxrwxrwx   0        0        0        0 2023-08-05 22:49:40.461760 DyGraph-0.0.2/src/DyGraph.egg-info/
+-rw-rw-rw-   0        0        0     3286 2023-08-05 22:49:40.000000 DyGraph-0.0.2/src/DyGraph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-08-05 22:49:40.000000 DyGraph-0.0.2/src/DyGraph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 22:49:40.000000 DyGraph-0.0.2/src/DyGraph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-05 22:46:00.000000 DyGraph-0.0.2/src/DyGraph.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2023-08-05 22:49:40.000000 DyGraph-0.0.2/src/DyGraph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-05 22:49:40.000000 DyGraph-0.0.2/src/DyGraph.egg-info/top_level.txt
```

### Comparing `DyGraph-0.0.1/LICENSE` & `DyGraph-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DyGraph-0.0.1/PKG-INFO` & `DyGraph-0.0.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,72 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2044 7947  : 2.1..Name: DyG
-00000020: 7261 7068 0d0a 5665 7273 696f 6e3a 2030  raph..Version: 0
-00000030: 2e30 2e31 0d0a 5375 6d6d 6172 793a 2041  .0.1..Summary: A
-00000040: 2070 6163 6b61 6765 2066 6f72 2065 7374   package for est
-00000050: 696d 6174 696e 6720 6479 6e61 6d69 6320  imating dynamic 
-00000060: 6772 6170 6869 6361 6c20 6c61 7373 6f20  graphical lasso 
-00000070: 7769 7468 2068 6561 7679 2074 6169 6c65  with heavy taile
-00000080: 6420 6469 7374 7269 6275 7469 6f6e 730d  d distributions.
-00000090: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-000000a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-000000b0: 6167 6e61 726c 6576 692f 4479 4772 6170  agnarlevi/DyGrap
-000000c0: 680d 0a41 7574 686f 723a 2072 6167 6e61  h..Author: ragna
-000000d0: 726c 6576 690d 0a4c 6963 656e 7365 3a20  rlevi..License: 
-000000e0: 4d49 540d 0a50 726f 6a65 6374 2d55 524c  MIT..Project-URL
-000000f0: 3a20 4275 6720 5472 6163 6b65 722c 2068  : Bug Tracker, h
-00000100: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000110: 6d2f 7261 676e 6172 6c65 7669 2f44 7947  m/ragnarlevi/DyG
-00000120: 7261 7068 2f69 7373 7565 730d 0a50 6c61  raph/issues..Pla
-00000130: 7466 6f72 6d3a 2075 6e69 780d 0a50 6c61  tform: unix..Pla
-00000140: 7466 6f72 6d3a 206c 696e 7578 0d0a 506c  tform: linux..Pl
-00000150: 6174 666f 726d 3a20 6f73 780d 0a50 6c61  atform: osx..Pla
-00000160: 7466 6f72 6d3a 2063 7967 7769 6e0d 0a50  tform: cygwin..P
-00000170: 6c61 7466 6f72 6d3a 2077 696e 3332 0d0a  latform: win32..
-00000180: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001e0: 203a 3a20 4f6e 6c79 0d0a 436c 6173 7369   :: Only..Classi
-000001f0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000210: 7468 6f6e 203a 3a20 332e 370d 0a43 6c61  thon :: 3.7..Cla
-00000220: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000230: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000240: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
-00000250: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000260: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000270: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000280: 390d 0a43 6c61 7373 6966 6965 723a 2050  9..Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e31 300d 0a43 6c61 7373 6966 6965   3.10..Classifie
-000002c0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-000002d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000002e0: 5420 4c69 6365 6e73 650d 0a43 6c61 7373  T License..Class
-000002f0: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000300: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000310: 6465 7065 6e64 656e 740d 0a52 6571 7569  dependent..Requi
-00000320: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00000330: 370d 0a44 6573 6372 6970 7469 6f6e 2d43  7..Description-C
-00000340: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-00000350: 742f 6d61 726b 646f 776e 0d0a 5072 6f76  t/markdown..Prov
-00000360: 6964 6573 2d45 7874 7261 3a20 7465 7374  ides-Extra: test
-00000370: 696e 670d 0a4c 6963 656e 7365 2d46 696c  ing..License-Fil
-00000380: 653a 204c 4943 454e 5345 0d0a 0d0a 0d0a  e: LICENSE......
-00000390: 215b 5465 7374 735d 2868 7474 7073 3a2f  ![Tests](https:/
-000003a0: 2f67 6974 6875 622e 636f 6d2f 7261 676e  /github.com/ragn
-000003b0: 6172 6c65 7669 2f44 7947 7261 7068 2f61  arlevi/DyGraph/a
-000003c0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-000003d0: 2f74 6573 7473 2e79 6d6c 2f62 6164 6765  /tests.yml/badge
-000003e0: 2e73 7667 290d 0a5b 215b 436f 7665 7261  .svg)..[![Covera
-000003f0: 6765 2053 7461 7475 735d 2868 7474 7073  ge Status](https
-00000400: 3a2f 2f63 6f76 6572 616c 6c73 2e69 6f2f  ://coveralls.io/
-00000410: 7265 706f 732f 6769 7468 7562 2f72 6167  repos/github/rag
-00000420: 6e61 726c 6576 692f 4479 4772 6170 682f  narlevi/DyGraph/
-00000430: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-00000440: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
-00000450: 636f 7665 7261 6c6c 732e 696f 2f67 6974  coveralls.io/git
-00000460: 6875 622f 7261 676e 6172 6c65 7669 2f44  hub/ragnarlevi/D
-00000470: 7947 7261 7068 3f62 7261 6e63 683d 6d61  yGraph?branch=ma
-00000480: 696e 290d 0a0d 0a23 2044 7947 7261 7068  in)....# DyGraph
-00000490: 0d0a 0d0a 4120 7061 636b 6167 6520 666f  ....A package fo
-000004a0: 7220 6479 6e61 6d69 6320 6772 6170 6820  r dynamic graph 
-000004b0: 6573 7469 6d61 7469 6f6e 0d0a 0d0a 0d0a  estimation......
-000004c0: 0d0a                                     ..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2044 7947 7261 7068 0d0a 6465 7363   = DyGraph..desc
+00000020: 7269 7074 696f 6e20 3d20 4120 7061 636b  ription = A pack
+00000030: 6167 6520 666f 7220 6573 7469 6d61 7469  age for estimati
+00000040: 6e67 2064 796e 616d 6963 2067 7261 7068  ng dynamic graph
+00000050: 6963 616c 206c 6173 736f 2077 6974 6820  ical lasso with 
+00000060: 6865 6176 7920 7461 696c 6564 2064 6973  heavy tailed dis
+00000070: 7472 6962 7574 696f 6e73 0d0a 6c6f 6e67  tributions..long
+00000080: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+00000090: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+000000c0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
+000000d0: 7574 686f 7220 3d20 7261 676e 6172 6c65  uthor = ragnarle
+000000e0: 7669 0d0a 7665 7273 696f 6e20 3d20 302e  vi..version = 0.
+000000f0: 302e 320d 0a6c 6963 656e 7365 203d 204d  0.2..license = M
+00000100: 4954 0d0a 6c69 6365 6e73 655f 6669 6c65  IT..license_file
+00000110: 203d 204c 4943 454e 5345 0d0a 7572 6c20   = LICENSE..url 
+00000120: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000130: 2e63 6f6d 2f72 6167 6e61 726c 6576 692f  .com/ragnarlevi/
+00000140: 4479 4772 6170 680d 0a70 6c61 7466 6f72  DyGraph..platfor
+00000150: 6d73 203d 2075 6e69 782c 206c 696e 7578  ms = unix, linux
+00000160: 2c20 6f73 782c 2063 7967 7769 6e2c 2077  , osx, cygwin, w
+00000170: 696e 3332 0d0a 636c 6173 7369 6669 6572  in32..classifier
+00000180: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001a0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
+000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000200: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000210: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000220: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
+00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000250: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000260: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000270: 6e20 3a3a 2033 2e31 300d 0a09 4c69 6365  n :: 3.10...Lice
+00000280: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000290: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000002a0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+000002b0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000002c0: 7065 6e64 656e 740d 0a70 726f 6a65 6374  pendent..project
+000002d0: 5f75 726c 7320 3d20 0d0a 0942 7567 2054  _urls = ...Bug T
+000002e0: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
+000002f0: 2f67 6974 6875 622e 636f 6d2f 7261 676e  /github.com/ragn
+00000300: 6172 6c65 7669 2f44 7947 7261 7068 2f69  arlevi/DyGraph/i
+00000310: 7373 7565 730d 0a0d 0a5b 6f70 7469 6f6e  ssues....[option
+00000320: 735d 0d0a 7061 636b 6167 6573 203d 200d  s]..packages = .
+00000330: 0a09 4479 4772 6170 680d 0a09 436f 7652  ..DyGraph...CovR
+00000340: 6567 0d0a 696e 7374 616c 6c5f 7265 7175  eg..install_requ
+00000350: 6972 6573 203d 200d 0a09 7363 6970 793e  ires = ...scipy>
+00000360: 3d31 2e36 2e31 0d0a 096e 756d 7079 3e3d  =1.6.1...numpy>=
+00000370: 312e 3230 2e31 0d0a 0974 7164 6d3e 3d34  1.20.1...tqdm>=4
+00000380: 2e36 352e 300d 0a70 7974 686f 6e5f 7265  .65.0..python_re
+00000390: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
+000003a0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000003b0: 093d 7372 630d 0a7a 6970 5f73 6166 6520  .=src..zip_safe 
+000003c0: 3d20 6e6f 0d0a 0d0a 5b6f 7074 696f 6e73  = no....[options
+000003d0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+000003e0: 0d0a 7465 7374 696e 6720 3d20 0d0a 0970  ..testing = ...p
+000003f0: 7974 6573 743e 3d37 2e33 2e30 0d0a 0970  ytest>=7.3.0...p
+00000400: 7974 6573 742d 636f 763e 3d32 2e30 0d0a  ytest-cov>=2.0..
+00000410: 0974 6f78 3e3d 332e 3234 0d0a 0d0a 5b6f  .tox>=3.24....[o
+00000420: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+00000430: 6174 615d 0d0a 736c 6170 7069 6e67 203d  ata]..slapping =
+00000440: 2070 792e 7479 7065 640d 0a0d 0a5b 6567   py.typed....[eg
+00000450: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000460: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000470: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `DyGraph-0.0.1/src/DyGraph/RootDygl.py` & `DyGraph-0.0.2/src/DyGraph/RootDygl.py`

 * *Files identical despite different names*

### Comparing `DyGraph-0.0.1/src/DyGraph/dyg_outer_em.py` & `DyGraph-0.0.2/src/DyGraph/dyg_outer_em.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         if i == self.nr_graphs-1 or i == 0:
             eta = self.obs_per_graph_used[i]/self.rho/2.0
         else:
             eta = self.obs_per_graph_used[i]/self.rho/3.0
         return eta
 
 
-    def fit(self, temporal_penalty,theta_init = None,  nr_workers = 1, verbose = True, max_admm_iter = 1, **kwargs):
+    def fit(self, temporal_penalty, theta_init = None,  nr_workers = 1, verbose = True, max_admm_iter = 1, **kwargs):
 
         self.get_nr_graphs()
         self.calc_S(kwargs.get("S_method", "empirical"))
         self.max_admm_iter = max_admm_iter
 
         if kwargs.get("nu", None) is None:
             self.nu = self.calc_nu(self.lik_type)
@@ -168,14 +168,20 @@
         
         if self.nr_graphs< nr_workers:
             nr_workers = self.nr_graphs
 
 
         if not hasattr(self.kappa, "__len__"):
             self.kappa = np.array([self.kappa for _ in range(self.nr_graphs)])
+        if not hasattr(self.lamda, "__len__"):
+            self.lamda = np.array([self.lamda for _ in range(self.nr_graphs)])  
+        elif  (len(self.lamda.shape) == 1) and (len(self.lamda) == self.nr_graphs):
+            self.lamda = self.lamda
+        elif (self.lamda.shape[0] == self.lamda.shape[1]) and len(self.lamda.shape) == 2:
+            self.lamda = np.array([self.lamda for _ in range(self.nr_graphs)])  
         if not hasattr(self.kappa_gamma, "__len__"):
             self.kappa_gamma = np.array([self.kappa_gamma for _ in range(self.nr_graphs)])
 
     
         while self.iteration < self.max_iter:
 
             # Perform E-step
@@ -217,15 +223,15 @@
                         for i in range(self.nr_graphs):
                             self.gamma[i], _ = update_gamma(i, G1[i], G2[i], self.theta[i], self.rho_gamma, self.get_A_gamma(i) )
 
 
                 # update dual in parallel
                 # update z0
                 for i in range(self.nr_graphs):
-                    self.z0[i] = soft_threshold_odd(self.theta[i]+self.u0[i], self.lamda/self.rho)
+                    self.z0[i] = soft_threshold_odd(self.theta[i]+self.u0[i], self.lamda[i]/self.rho)
 
 
                 # update z1, z2, z3, z4
                 for i in range(1,self.nr_graphs):
                     A = self.theta[i]-self.theta[i-1]+self.u2[i]-self.u1[i-1]
                     if temporal_penalty == "element-wise":
                         E = soft_threshold_odd(A, 2*self.kappa[i-1]/self.rho)
```

### Comparing `DyGraph-0.0.1/src/DyGraph/dygl_inner_em.py` & `DyGraph-0.0.2/src/DyGraph/dygl_inner_em.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,20 @@
 
         if nr_workers >1:
             pool = Pool(nr_workers)
 
 
         if not hasattr(self.kappa, "__len__"):
             self.kappa = np.array([self.kappa for _ in range(self.nr_graphs)])
+        if not hasattr(self.lamda, "__len__"):
+            self.lamda = np.array([self.lamda for _ in range(self.nr_graphs)])  
+        elif  (len(self.lamda.shape) == 1) and (len(self.lamda) == self.nr_graphs):
+            self.lamda = self.lamda
+        elif (self.lamda.shape[0] == self.lamda.shape[1]) and len(self.lamda.shape) == 2:
+            self.lamda = np.array([self.lamda for _ in range(self.nr_graphs)])  
         if not hasattr(self.kappa_gamma, "__len__"):
             self.kappa_gamma = np.array([self.kappa_gamma for _ in range(self.nr_graphs)])
 
 
         while self.iteration < self.max_iter:
 
             if self.nr_graphs< nr_workers:
@@ -209,15 +215,15 @@
                                                         kwargs.get("nr_quad", 5),
                                                         kwargs.get("pool", None)  )
 
 
             # update dual in parallel
             # update z0
             for i in range(self.nr_graphs):
-                self.z0[i] = soft_threshold_odd(self.theta[i]+self.u0[i], self.lamda/self.rho)
+                self.z0[i] = soft_threshold_odd(self.theta[i]+self.u0[i], self.lamda[i]/self.rho)
 
             # update z1, z2, z3, z4
             for i in range(1,self.nr_graphs):
                 A = self.theta[i]-self.theta[i-1]+self.u2[i]-self.u1[i-1]
                 if temporal_penalty == "element-wise":
                     E = soft_threshold_odd(A, 2*self.kappa[i-1]/self.rho)
                     self.z12_update(E,i)
```

### Comparing `DyGraph-0.0.1/src/DyGraph/dygl_utils.py` & `DyGraph-0.0.2/src/DyGraph/dygl_utils.py`

 * *Files identical despite different names*

### Comparing `DyGraph-0.0.1/src/DyGraph/sgl_inner_em.py` & `DyGraph-0.0.2/src/DyGraph/sgl_inner_em.py`

 * *Files identical despite different names*

### Comparing `DyGraph-0.0.1/src/DyGraph/sgl_outer_em.py` & `DyGraph-0.0.2/src/DyGraph/sgl_outer_em.py`

 * *Files identical despite different names*

