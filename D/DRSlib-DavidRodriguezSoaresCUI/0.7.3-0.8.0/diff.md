# Comparing `tmp/DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar.gz` & `tmp/DRSlib-DavidRodriguezSoaresCUI-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar", last modified: Sun Apr 23 16:04:45 2023, max compression
+gzip compressed data, was "DRSlib-DavidRodriguezSoaresCUI-0.8.0.tar", last modified: Sun Aug  6 09:47:00 2023, max compression
```

## Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3.tar` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/
--rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     3503 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/README.md
--rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0     1102 2023-04-23 16:04:45.074573 DRSlib-DavidRodriguezSoaresCUI-0.7.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.045775 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.060789 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/
--rw-rw-rw-   0        0        0      697 2023-04-22 15:27:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/__init__.py
--rw-rw-rw-   0        0        0     5046 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/banner.py
--rw-rw-rw-   0        0        0     9799 2023-04-23 16:02:46.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/cli_ui.py
--rw-rw-rw-   0        0        0     6182 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/debug.py
--rw-rw-rw-   0        0        0     9731 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/decorators.py
--rw-rw-rw-   0        0        0     3413 2023-04-23 13:58:36.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/dict_utils.py
--rw-rw-rw-   0        0        0     1370 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/execute.py
--rw-rw-rw-   0        0        0    13598 2023-04-22 15:31:18.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/fsdb.py
--rw-rw-rw-   0        0        0     4219 2023-04-23 12:12:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/hash.py
--rw-rw-rw-   0        0        0     3410 2023-04-22 08:30:58.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/interval.py
--rw-rw-rw-   0        0        0      444 2023-04-23 12:01:10.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/list_utils.py
--rw-rw-rw-   0        0        0    15553 2023-04-23 12:11:23.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/mediainfo.py
--rw-rw-rw-   0        0        0     1329 2023-04-23 14:11:24.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/multiprocessing.py
--rw-rw-rw-   0        0        0     1568 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/os_detect.py
--rw-rw-rw-   0        0        0    13957 2023-04-22 15:33:39.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/path_tools.py
--rw-rw-rw-   0        0        0     2266 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/spinner.py
--rw-rw-rw-   0        0        0     4188 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/str_utils.py
--rw-rw-rw-   0        0        0     4040 2023-04-23 12:10:40.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-23 16:04:45.073568 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
--rw-rw-rw-   0        0        0     3503 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-23 16:04:45.000000 DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 09:47:00.773156 DRSlib-DavidRodriguezSoaresCUI-0.8.0/
+-rw-rw-rw-   0        0        0     6432 2021-11-14 15:06:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     3407 2023-08-06 09:47:00.773156 DRSlib-DavidRodriguezSoaresCUI-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2497 2021-11-28 13:21:49.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/README.md
+-rw-rw-rw-   0        0        0      114 2021-10-31 10:05:27.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1090 2023-08-06 09:47:00.773156 DRSlib-DavidRodriguezSoaresCUI-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 09:47:00.757531 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 09:47:00.757531 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/
+-rw-rw-rw-   0        0        0      697 2023-04-22 15:27:12.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/__init__.py
+-rw-rw-rw-   0        0        0     5046 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/banner.py
+-rw-rw-rw-   0        0        0     9787 2023-05-06 15:21:29.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/cli_ui.py
+-rw-rw-rw-   0        0        0     6182 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/debug.py
+-rw-rw-rw-   0        0        0     8436 2023-05-06 15:06:08.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/decorators.py
+-rw-rw-rw-   0        0        0     3413 2023-04-23 13:58:36.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/dict_utils.py
+-rw-rw-rw-   0        0        0    17686 2023-08-06 09:33:37.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/execute.py
+-rw-rw-rw-   0        0        0    13598 2023-04-22 15:31:18.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/fsdb.py
+-rw-rw-rw-   0        0        0     4219 2023-04-23 12:12:03.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/hash.py
+-rw-rw-rw-   0        0        0     4611 2023-05-18 14:22:07.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/interval.py
+-rw-rw-rw-   0        0        0      444 2023-04-23 12:01:10.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/list_utils.py
+-rw-rw-rw-   0        0        0    15553 2023-04-23 12:11:23.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/mediainfo.py
+-rw-rw-rw-   0        0        0     2060 2023-08-06 09:40:35.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/multiprocessing.py
+-rw-rw-rw-   0        0        0     1568 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/os_detect.py
+-rw-rw-rw-   0        0        0    13957 2023-04-22 15:33:39.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/path_tools.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 09:12:09.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/py.typed
+-rw-rw-rw-   0        0        0     2266 2023-04-22 15:27:32.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/spinner.py
+-rw-rw-rw-   0        0        0     3633 2023-05-06 15:05:50.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/str_utils.py
+-rw-rw-rw-   0        0        0     4312 2023-05-06 15:08:57.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:47:00.773156 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-08-06 09:47:00.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-08-06 09:47:00.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:47:00.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-06 09:47:00.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 09:47:00.000000 DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/top_level.txt
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/LICENSE` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.7.3
+Version: 0.8.0
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [DRSlib - a set of utilities by DavidRodriguezSoaresCUI](https://github.com/DavidRodriguezSoaresCUI/DRSlib)
 
 DRSlib is a Python package that provides a wide range of small
 yet powerful and highly-reusable functions, classes,
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/README.md` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/setup.cfg` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 5253 6c69 622d 4461 7669 6452   = DRSlib-DavidR
 00000020: 6f64 7269 6775 657a 536f 6172 6573 4355  odriguezSoaresCU
-00000030: 490d 0a76 6572 7369 6f6e 203d 2030 2e37  I..version = 0.7
-00000040: 2e33 0d0a 6175 7468 6f72 203d 2044 6176  .3..author = Dav
+00000030: 490d 0a76 6572 7369 6f6e 203d 2030 2e38  I..version = 0.8
+00000040: 2e30 0d0a 6175 7468 6f72 203d 2044 6176  .0..author = Dav
 00000050: 6964 526f 6472 6967 7565 7a53 6f61 7265  idRodriguezSoare
 00000060: 7343 5549 0d0a 6175 7468 6f72 5f65 6d61  sCUI..author_ema
 00000070: 696c 203d 2066 6972 6562 6c61 7a65 3930  il = fireblaze90
 00000080: 342b 4452 536c 6962 4067 6d61 696c 2e63  4+DRSlib@gmail.c
 00000090: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 000000a0: 3d20 4452 536c 6962 202d 2061 2073 6574  = DRSlib - a set
 000000b0: 206f 6620 7574 696c 6974 6965 7320 6279   of utilities by
@@ -23,47 +23,47 @@
 00000160: 536c 6962 0d0a 7072 6f6a 6563 745f 7572  Slib..project_ur
 00000170: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
 00000180: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
 00000190: 7468 7562 2e63 6f6d 2f44 6176 6964 526f  thub.com/DavidRo
 000001a0: 6472 6967 7565 7a53 6f61 7265 7343 5549  driguezSoaresCUI
 000001b0: 2f44 5253 6c69 622f 6973 7375 6573 0d0a  /DRSlib/issues..
 000001c0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001d0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001e0: 7475 7320 3a3a 2033 202d 2041 6c70 6861  tus :: 3 - Alpha
-000001f0: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000200: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000210: 7273 0d0a 094c 6963 656e 7365 203a 3a20  rs...License :: 
-00000220: 4343 3020 312e 3020 556e 6976 6572 7361  CC0 1.0 Universa
-00000230: 6c20 2843 4330 2031 2e30 2920 5075 626c  l (CC0 1.0) Publ
-00000240: 6963 2044 6f6d 6169 6e20 4465 6469 6361  ic Domain Dedica
-00000250: 7469 6f6e 0d0a 094f 7065 7261 7469 6e67  tion...Operating
-00000260: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000270: 6465 7065 6e64 656e 740d 0a09 5072 6f67  dependent...Prog
-00000280: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000290: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
-000002a0: 3a3a 204f 6e6c 790d 0a09 5072 6f67 7261  :: Only...Progra
-000002b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002c0: 3a20 5079 7468 6f6e 203a 3a20 332e 360d  : Python :: 3.6.
-000002d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002f0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
-00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000310: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
-00000320: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000330: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000340: 203a 3a20 332e 390d 0a09 546f 7069 6320   :: 3.9...Topic 
-00000350: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000360: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000370: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
-00000380: 6f64 756c 6573 0d0a 0d0a 5b6f 7074 696f  odules....[optio
-00000390: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
-000003a0: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
-000003b0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-000003c0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000003d0: 203e 3d33 2e36 0d0a 696e 7374 616c 6c5f   >=3.6..install_
-000003e0: 7265 7175 6972 6573 203d 200d 0a09 7365  requires = ...se
-000003f0: 6e64 3274 7261 7368 0d0a 0d0a 5b6f 7074  nd2trash....[opt
-00000400: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000410: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-00000420: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000430: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000440: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000001d0: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000001e0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+000001f0: 0d0a 094c 6963 656e 7365 203a 3a20 4343  ...License :: CC
+00000200: 3020 312e 3020 556e 6976 6572 7361 6c20  0 1.0 Universal 
+00000210: 2843 4330 2031 2e30 2920 5075 626c 6963  (CC0 1.0) Public
+00000220: 2044 6f6d 6169 6e20 4465 6469 6361 7469   Domain Dedicati
+00000230: 6f6e 0d0a 094f 7065 7261 7469 6e67 2053  on...Operating S
+00000240: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000250: 7065 6e64 656e 740d 0a09 5072 6f67 7261  pendent...Progra
+00000260: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000270: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
+00000280: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
+00000290: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002a0: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
+000002b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002d0: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002f0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000300: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000310: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000320: 204c 6962 7261 7269 6573 203a 3a20 5079   Libraries :: Py
+00000330: 7468 6f6e 204d 6f64 756c 6573 0d0a 0d0a  thon Modules....
+00000340: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000350: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
+00000360: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
+00000370: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
+00000380: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
+00000390: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+000003a0: 200d 0a09 6e75 6d70 790d 0a09 7073 7574   ...numpy...psut
+000003b0: 696c 0d0a 0973 656e 6432 7472 6173 680d  il...send2trash.
+000003c0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+000003d0: 6167 655f 6461 7461 5d0d 0a44 5253 6c69  age_data]..DRSli
+000003e0: 6220 3d20 7079 2e74 7970 6564 0d0a 0d0a  b = py.typed....
+000003f0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000400: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000410: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
+00000420: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000430: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000440: 0d0a                                     ..
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/__init__.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/__init__.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/banner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/banner.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/cli_ui.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/cli_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 ===========================
 
 Implements convenience function for CLI user interaction.
 Useful when you need to ask the user what to do, or select one
 of many options.
 """
 
-import ast
 import os
 import sys
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, Optional, Union
 
 from .banner import one_line_banner
 from .os_detect import Os
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/debug.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/debug.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/decorators.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -289,70 +289,7 @@
     # File Extension enforcement
     if cache_file_or_args.suffix != ".cacheFS":
         cache_file = Path(f"{cache_file}.cacheFS")
 
     cached_data = load_cached_data(cache_file)
 
     return actual_decorator
-
-
-########### end of decorators ###########
-
-
-if __name__ == "__main__":
-
-    def vspace():
-        """just prints newlines"""
-        print("\n" * 2)
-
-    # Tests
-
-    # Test 01
-    vspace()
-    print("Test 01 : decorator 'timer'")
-
-    @timer
-    def wait2s() -> None:
-        """Just wait 2s"""
-        time.sleep(2)
-
-    print(wait2s)
-    print(wait2s.__doc__)
-    wait2s()
-
-    # Test 02
-    vspace()
-    print("Test 02 : decorator 'log_to_file'")
-
-    @log_to_file
-    def add(a: int, b: int) -> int:
-        """Add a and b"""
-        return a + b
-
-    print(add)
-    print(add.__doc__)
-    add(7, 13)
-    logfile = Path("add.log")
-    assertTrue(logfile.is_file(), "logfile must exist: '{}'", logfile)
-
-    # Test 03
-    vspace()
-    print("Test 03 : decorator 'cacheFS'")
-
-    # @cacheFS(Path('slow_mult'))
-    @cacheFS
-    def slow_mult(a: int, b: int) -> int:
-        """Multiply a and b"""
-        time.sleep(1)
-        return a * b
-
-    print(slow_mult)
-    print(slow_mult.__doc__)
-
-    @timer
-    def test03():
-        """tests timer decorator"""
-        for i in range(4):
-            res = slow_mult(111, 10 * i)
-            print(f"111 * {i} = {res}")
-
-    test03()  # runs in 2ms-4s depending on cache hits/misses
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/dict_utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/dict_utils.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/fsdb.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/fsdb.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/hash.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/hash.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/mediainfo.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/mediainfo.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/os_detect.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/os_detect.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/path_tools.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/path_tools.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/spinner.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/spinner.py`

 * *Files identical despite different names*

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/str_utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/str_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 Simple utils that accomplish one task well, specifically string operations.
 
 """
 
 import re
 
 
+DOUBLE_QUOTE = '"'
+
+
+def ensure_quoted_on_space(s: str) -> str:
+    """Ensures a string containing spaces is fully enclosed
+    between double quotes
+    """
+    if " " not in s:
+        return s
+    return ensure_double_quotes(s)
+
+
 def ensure_double_quotes(s: str) -> str:
     """Ensures s is double quoted in a particular way :
      - returned string must begin and end with a double quote character `"`
      - any double quote that isn't at the beginning or end must be escaped `\\"`
 
     Examples :
      - `` (empty string) -> `""`
@@ -98,37 +110,7 @@
 
     if cut_location == "right":
         return f"[...] {s[-(output_length-6):]}"
     # else
     raise ValueError(
         f"truncate_str: given parameter 'cut_location'={cut_location} is not in ['left','center','right'] !"
     )
-
-
-if __name__ == "__main__":
-    # ensure_double_quotes tests
-
-    # tests = [
-    #     '',
-    #     '.',
-    #     '"',
-    #     '"hello',
-    #     'hello"',
-    #     '"hello"',
-    #     '"he"llo"',
-    #     'he\\"llo'
-    # ]
-
-    # for test_s in tests:
-    #     res = ensure_double_quotes(test_s)
-    #     print(f"test_s={test_s}={list(test_s)} -> {list(res)} = {res}")
-
-    # truncate_str tests
-
-    tests = ["h" * 20, "h" * 21]
-    for new_len in [10, 15]:
-        for cut in ["left", "center", "right"]:
-            for test_s in tests:
-                res = truncate_str(test_s, new_len, cut)
-                print(
-                    f"new_len={new_len}, cut={cut} : test_s='{test_s}' (len={len(test_s)}) -> '{res}' (len={len(res)})"
-                )
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib/utils.py` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,7 +113,18 @@
     try:
         res = method(*args, **kwargs)
         if res is None:
             return None
         return res if mapping is None else mapping(res)
     except Exception:
         return None
+
+
+def cast_number(number: str) -> int | float | str:
+    """Attempts to cast number to int or float"""
+    try:
+        return int(number)
+    except ValueError:
+        try:
+            return float(number)
+        except ValueError:
+            return number
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: DRSlib-DavidRodriguezSoaresCUI
-Version: 0.7.3
+Version: 0.8.0
 Summary: DRSlib - a set of utilities by DavidRodriguezSoaresCUI
 Home-page: https://github.com/DavidRodriguezSoaresCUI/DRSlib
 Author: DavidRodriguezSoaresCUI
 Author-email: fireblaze904+DRSlib@gmail.com
 Project-URL: Bug Tracker, https://github.com/DavidRodriguezSoaresCUI/DRSlib/issues
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [DRSlib - a set of utilities by DavidRodriguezSoaresCUI](https://github.com/DavidRodriguezSoaresCUI/DRSlib)
 
 DRSlib is a Python package that provides a wide range of small
 yet powerful and highly-reusable functions, classes,
```

### Comparing `DRSlib-DavidRodriguezSoaresCUI-0.7.3/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt` & `DRSlib-DavidRodriguezSoaresCUI-0.8.0/src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/DRSlib/hash.py
 src/DRSlib/interval.py
 src/DRSlib/list_utils.py
 src/DRSlib/mediainfo.py
 src/DRSlib/multiprocessing.py
 src/DRSlib/os_detect.py
 src/DRSlib/path_tools.py
+src/DRSlib/py.typed
 src/DRSlib/spinner.py
 src/DRSlib/str_utils.py
 src/DRSlib/utils.py
 src/DRSlib_DavidRodriguezSoaresCUI.egg-info/PKG-INFO
 src/DRSlib_DavidRodriguezSoaresCUI.egg-info/SOURCES.txt
 src/DRSlib_DavidRodriguezSoaresCUI.egg-info/dependency_links.txt
 src/DRSlib_DavidRodriguezSoaresCUI.egg-info/requires.txt
```

