# Comparing `tmp/dexhub-0.6.7.tar.gz` & `tmp/dexhub-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.6.7.tar", last modified: Wed May  3 02:13:23 2023, max compression
+gzip compressed data, was "dexhub-0.6.8.tar", last modified: Wed May  3 12:57:26 2023, max compression
```

## Comparing `dexhub-0.6.7.tar` & `dexhub-0.6.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.276359 dexhub-0.6.7/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-03 02:13:23.276208 dexhub-0.6.7/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.7/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.272142 dexhub-0.6.7/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1207 2023-05-02 19:50:21.000000 dexhub-0.6.7/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.274143 dexhub-0.6.7/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.7/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.7/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.6.7/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.7/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.7/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.7/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.275387 dexhub-0.6.7/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.7/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.7/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.7/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.7/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.7/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.7/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.7/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)   142188 2023-05-03 02:13:08.000000 dexhub-0.6.7/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.275617 dexhub-0.6.7/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.7/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.7/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.276013 dexhub-0.6.7/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.6.7/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.6.7/dexhub/util/helper.py
--rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.6.7/dexhub/util/joe_v2.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 02:13:23.273085 dexhub-0.6.7/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-03 02:13:23.000000 dexhub-0.6.7/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      679 2023-05-03 02:13:23.000000 dexhub-0.6.7/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-03 02:13:23.000000 dexhub-0.6.7/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-03 02:13:23.000000 dexhub-0.6.7/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-03 02:13:23.000000 dexhub-0.6.7/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-03 02:13:23.276410 dexhub-0.6.7/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-03 02:13:16.000000 dexhub-0.6.7/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.661606 dexhub-0.6.8/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-03 12:57:26.661432 dexhub-0.6.8/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.8/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.657000 dexhub-0.6.8/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1207 2023-05-02 19:50:21.000000 dexhub-0.6.8/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.658503 dexhub-0.6.8/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.8/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.8/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.6.8/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.8/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.8/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.8/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.659525 dexhub-0.6.8/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.8/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.8/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.8/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.8/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.8/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.8/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.8/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)   142211 2023-05-03 12:57:14.000000 dexhub-0.6.8/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.659773 dexhub-0.6.8/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.8/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.8/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.661210 dexhub-0.6.8/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.6.8/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.6.8/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.6.8/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-03 12:57:26.657665 dexhub-0.6.8/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-03 12:57:26.000000 dexhub-0.6.8/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      679 2023-05-03 12:57:26.000000 dexhub-0.6.8/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-03 12:57:26.000000 dexhub-0.6.8/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-03 12:57:26.000000 dexhub-0.6.8/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-03 12:57:26.000000 dexhub-0.6.8/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-03 12:57:26.661681 dexhub-0.6.8/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-03 12:57:22.000000 dexhub-0.6.8/setup.py
```

### Comparing `dexhub-0.6.7/PKG-INFO` & `dexhub-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.7
+Version: 0.6.8
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.7/dexhub/__init__.py` & `dexhub-0.6.8/dexhub/__init__.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/abi/arbitrum_abi.py` & `dexhub-0.6.8/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/abi/avax_abi.py` & `dexhub-0.6.8/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/abi/dfk_abi.py` & `dexhub-0.6.8/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/abi/eth_abi.py` & `dexhub-0.6.8/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/abi/klay_abi.py` & `dexhub-0.6.8/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/arbitrum_address.py` & `dexhub-0.6.8/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/avax_address.py` & `dexhub-0.6.8/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/dfk_address.py` & `dexhub-0.6.8/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/eth_address.py` & `dexhub-0.6.8/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/klay_address.py` & `dexhub-0.6.8/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/address/polygon_address.py` & `dexhub-0.6.8/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/dex.py` & `dexhub-0.6.8/dexhub/dex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2815,6073 +2815,6075 @@
 0000afe0: 302c 7265 7365 7276 6531 2c62 6c6f 636b  0,reserve1,block
 0000aff0: 5469 6d65 5374 616d 703d 7061 6972 436f  TimeStamp=pairCo
 0000b000: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
 0000b010: 2e67 6574 5265 7365 7276 6573 2829 2e63  .getReserves().c
 0000b020: 616c 6c28 290a 2020 2020 2020 2020 7265  all().        re
 0000b030: 7475 726e 2072 6573 6572 7665 302c 7265  turn reserve0,re
 0000b040: 7365 7276 6531 2c62 6c6f 636b 5469 6d65  serve1,blockTime
-0000b050: 5374 616d 700a 0a20 2020 2064 6566 2067  Stamp..    def g
-0000b060: 6574 5f72 6573 6572 7665 7328 5f77 6562  et_reserves(_web
-0000b070: 333a 5765 6233 2c5f 7061 6972 5f61 6464  3:Web3,_pair_add
-0000b080: 7265 7373 2c5f 7061 6972 5f61 6269 293a  ress,_pair_abi):
-0000b090: 0a20 2020 2020 2020 2070 6169 725f 636f  .        pair_co
-0000b0a0: 6e74 7261 6374 3d5f 7765 6233 2e65 7468  ntract=_web3.eth
-0000b0b0: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
-0000b0c0: 733d 5f70 6169 725f 6164 6472 6573 732c  s=_pair_address,
-0000b0d0: 6162 693d 5f70 6169 725f 6162 6929 0a20  abi=_pair_abi). 
-0000b0e0: 2020 2020 2020 2072 6573 6572 7665 302c         reserve0,
-0000b0f0: 7265 7365 7276 6531 2c62 6c6f 636b 5469  reserve1,blockTi
-0000b100: 6d65 5374 616d 703d 7061 6972 5f63 6f6e  meStamp=pair_con
-0000b110: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-0000b120: 6765 7452 6573 6572 7665 7328 292e 6361  getReserves().ca
-0000b130: 6c6c 2829 0a20 2020 2020 2020 2072 6574  ll().        ret
-0000b140: 7572 6e20 7265 7365 7276 6530 2c72 6573  urn reserve0,res
-0000b150: 6572 7665 312c 626c 6f63 6b54 696d 6553  erve1,blockTimeS
-0000b160: 7461 6d70 0a0a 2020 2020 6465 6620 6765  tamp..    def ge
-0000b170: 745f 7061 6972 5f69 6e66 6f28 7365 6c66  t_pair_info(self
-0000b180: 2c70 6169 725f 6164 6472 6573 7329 3a0a  ,pair_address):.
-0000b190: 2020 2020 2020 2020 7061 6972 436f 6e74          pairCont
-0000b1a0: 7261 6374 3d73 656c 662e 7765 6233 2e65  ract=self.web3.e
-0000b1b0: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-0000b1c0: 6573 733d 7061 6972 5f61 6464 7265 7373  ess=pair_address
-0000b1d0: 2c20 6162 693d 7365 6c66 2e70 6169 725f  , abi=self.pair_
-0000b1e0: 6162 6929 0a20 2020 2020 2020 2074 6f6b  abi).        tok
-0000b1f0: 656e 3041 6464 7265 7373 3d70 6169 7243  en0Address=pairC
-0000b200: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
-0000b210: 732e 746f 6b65 6e30 2829 2e63 616c 6c28  s.token0().call(
-0000b220: 290a 2020 2020 2020 2020 746f 6b65 6e31  ).        token1
-0000b230: 4164 6472 6573 733d 7061 6972 436f 6e74  Address=pairCont
-0000b240: 7261 6374 2e66 756e 6374 696f 6e73 2e74  ract.functions.t
-0000b250: 6f6b 656e 3128 292e 6361 6c6c 2829 0a20  oken1().call(). 
-0000b260: 2020 2020 2020 2072 6573 6572 7665 302c         reserve0,
-0000b270: 7265 7365 7276 6531 2c62 6c6f 636b 5469  reserve1,blockTi
-0000b280: 6d65 5374 616d 703d 7061 6972 436f 6e74  meStamp=pairCont
-0000b290: 7261 6374 2e66 756e 6374 696f 6e73 2e67  ract.functions.g
-0000b2a0: 6574 5265 7365 7276 6573 2829 2e63 616c  etReserves().cal
-0000b2b0: 6c28 290a 2020 2020 2020 2020 2320 746f  l().        # to
-0000b2c0: 6b65 6e30 5f63 6f6e 7472 6163 743d 7365  ken0_contract=se
-0000b2d0: 6c66 2e77 6562 332e 6574 682e 636f 6e74  lf.web3.eth.cont
-0000b2e0: 7261 6374 2861 6464 7265 7373 3d74 6f6b  ract(address=tok
-0000b2f0: 656e 3041 6464 7265 7373 2c20 6162 693d  en0Address, abi=
-0000b300: 7365 6c66 2e65 7263 3230 5f61 6269 290a  self.erc20_abi).
-0000b310: 2020 2020 2020 2020 2320 746f 6b65 6e31          # token1
-0000b320: 5f63 6f6e 7472 6163 743d 7365 6c66 2e77  _contract=self.w
-0000b330: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
-0000b340: 2861 6464 7265 7373 3d74 6f6b 656e 3141  (address=token1A
-0000b350: 6464 7265 7373 2c20 6162 693d 7365 6c66  ddress, abi=self
-0000b360: 2e65 7263 3230 5f61 6269 290a 2020 2020  .erc20_abi).    
-0000b370: 2020 2020 2320 746f 6b65 6e30 5f6e 616d      # token0_nam
-0000b380: 653d 746f 6b65 6e30 5f63 6f6e 7472 6163  e=token0_contrac
-0000b390: 742e 6675 6e63 7469 6f6e 732e 6e61 6d65  t.functions.name
-0000b3a0: 2829 2e63 616c 6c28 290a 2020 2020 2020  ().call().      
-0000b3b0: 2020 2320 746f 6b65 6e31 5f6e 616d 653d    # token1_name=
-0000b3c0: 746f 6b65 6e31 5f63 6f6e 7472 6163 742e  token1_contract.
-0000b3d0: 6675 6e63 7469 6f6e 732e 6e61 6d65 2829  functions.name()
-0000b3e0: 2e63 616c 6c28 290a 2020 2020 2020 2020  .call().        
-0000b3f0: 7072 6963 6530 3d72 6573 6572 7665 312f  price0=reserve1/
-0000b400: 7265 7365 7276 6530 0a20 2020 2020 2020  reserve0.       
-0000b410: 2070 7269 6365 313d 7265 7365 7276 6530   price1=reserve0
-0000b420: 2f72 6573 6572 7665 310a 2020 2020 2020  /reserve1.      
-0000b430: 2020 2320 7072 696e 7428 2274 6f6b 656e    # print("token
-0000b440: 303a 222c 7374 7228 746f 6b65 6e30 4164  0:",str(token0Ad
-0000b450: 6472 6573 7329 2c22 2d2d 6e61 6d65 3a22  dress),"--name:"
-0000b460: 2c73 7472 2874 6f6b 656e 305f 6e61 6d65  ,str(token0_name
-0000b470: 292c 222d 2d70 7269 6365 3a22 2c73 7472  ),"--price:",str
-0000b480: 2870 7269 6365 3029 290a 2020 2020 2020  (price0)).      
-0000b490: 2020 2320 7072 696e 7428 2274 6f6b 656e    # print("token
-0000b4a0: 313a 222c 7374 7228 746f 6b65 6e31 4164  1:",str(token1Ad
-0000b4b0: 6472 6573 7329 2c22 2d2d 6e61 6d65 3a22  dress),"--name:"
-0000b4c0: 2c73 7472 2874 6f6b 656e 315f 6e61 6d65  ,str(token1_name
-0000b4d0: 292c 222d 2d70 7269 6365 3a22 2c73 7472  ),"--price:",str
-0000b4e0: 2870 7269 6365 3129 290a 2020 2020 2020  (price1)).      
-0000b4f0: 2020 2320 7072 696e 7428 2272 6573 6572    # print("reser
-0000b500: 7665 3022 2c73 7472 2872 6573 6572 7665  ve0",str(reserve
-0000b510: 3029 290a 2020 2020 2020 2020 2320 7072  0)).        # pr
-0000b520: 696e 7428 2272 6573 6572 7665 3122 2c73  int("reserve1",s
-0000b530: 7472 2872 6573 6572 7665 3129 290a 2020  tr(reserve1)).  
-0000b540: 2020 2020 2020 2320 7072 696e 7428 2262        # print("b
-0000b550: 6c6f 636b 5469 6d65 5374 616d 7022 2c73  lockTimeStamp",s
-0000b560: 7472 2862 6c6f 636b 5469 6d65 5374 616d  tr(blockTimeStam
-0000b570: 7029 290a 2020 2020 2020 2020 7265 7475  p)).        retu
-0000b580: 726e 2074 6f6b 656e 3041 6464 7265 7373  rn token0Address
-0000b590: 2c72 6573 6572 7665 302c 746f 6b65 6e31  ,reserve0,token1
-0000b5a0: 4164 6472 6573 732c 7265 7365 7276 6531  Address,reserve1
-0000b5b0: 2c62 6c6f 636b 5469 6d65 5374 616d 702c  ,blockTimeStamp,
-0000b5c0: 7072 6963 6530 2c70 7269 6365 310a 0a63  price0,price1..c
-0000b5d0: 6c61 7373 2055 6e69 7377 6170 5633 3a0a  lass UniswapV3:.
-0000b5e0: 2020 2020 2368 7474 7073 3a2f 2f65 7468      #https://eth
-0000b5f0: 6572 7363 616e 2e69 6f2f 6164 6472 6573  erscan.io/addres
-0000b600: 732f 3078 3166 3938 3433 3163 3861 6439  s/0x1f98431c8ad9
-0000b610: 3835 3233 3633 3161 6534 6135 3966 3236  8523631ae4a59f26
-0000b620: 3733 3436 6561 3331 6639 3834 0a20 2020  7346ea31f984.   
-0000b630: 2075 6e69 7377 6170 5f76 335f 6661 6374   uniswap_v3_fact
-0000b640: 6f72 795f 6162 693d 275b 7b22 696e 7075  ory_abi='[{"inpu
-0000b650: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
-0000b660: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-0000b670: 6162 6c65 222c 2274 7970 6522 3a22 636f  able","type":"co
-0000b680: 6e73 7472 7563 746f 7222 7d2c 7b22 616e  nstructor"},{"an
-0000b690: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
-0000b6a0: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
-0000b6b0: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
-0000b6c0: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
-0000b6d0: 2c22 6e61 6d65 223a 2266 6565 222c 2274  ,"name":"fee","t
-0000b6e0: 7970 6522 3a22 7569 6e74 3234 227d 2c7b  ype":"uint24"},{
-0000b6f0: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-0000b700: 696e 7465 726e 616c 5479 7065 223a 2269  internalType":"i
-0000b710: 6e74 3234 222c 226e 616d 6522 3a22 7469  nt24","name":"ti
-0000b720: 636b 5370 6163 696e 6722 2c22 7479 7065  ckSpacing","type
-0000b730: 223a 2269 6e74 3234 227d 5d2c 226e 616d  ":"int24"}],"nam
-0000b740: 6522 3a22 4665 6541 6d6f 756e 7445 6e61  e":"FeeAmountEna
-0000b750: 626c 6564 222c 2274 7970 6522 3a22 6576  bled","type":"ev
-0000b760: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
-0000b770: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
-0000b780: 223a 5b7b 2269 6e64 6578 6564 223a 7472  ":[{"indexed":tr
-0000b790: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-0000b7a0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000b7b0: 6522 3a22 6f6c 644f 776e 6572 222c 2274  e":"oldOwner","t
-0000b7c0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0000b7d0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-0000b7e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000b7f0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0000b800: 226e 6577 4f77 6e65 7222 2c22 7479 7065  "newOwner","type
-0000b810: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
-0000b820: 616d 6522 3a22 4f77 6e65 7243 6861 6e67  ame":"OwnerChang
-0000b830: 6564 222c 2274 7970 6522 3a22 6576 656e  ed","type":"even
-0000b840: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-0000b850: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0000b860: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-0000b870: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0000b880: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0000b890: 3a22 746f 6b65 6e30 222c 2274 7970 6522  :"token0","type"
-0000b8a0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0000b8b0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0000b8c0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000b8d0: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000b8e0: 656e 3122 2c22 7479 7065 223a 2261 6464  en1","type":"add
-0000b8f0: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
-0000b900: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
-0000b910: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-0000b920: 6e61 6d65 223a 2266 6565 222c 2274 7970  name":"fee","typ
-0000b930: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
-0000b940: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
-0000b950: 6e74 6572 6e61 6c54 7970 6522 3a22 696e  nternalType":"in
-0000b960: 7432 3422 2c22 6e61 6d65 223a 2274 6963  t24","name":"tic
-0000b970: 6b53 7061 6369 6e67 222c 2274 7970 6522  kSpacing","type"
-0000b980: 3a22 696e 7432 3422 7d2c 7b22 696e 6465  :"int24"},{"inde
-0000b990: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0000b9a0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0000b9b0: 7373 222c 226e 616d 6522 3a22 706f 6f6c  ss","name":"pool
-0000b9c0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0000b9d0: 7322 7d5d 2c22 6e61 6d65 223a 2250 6f6f  s"}],"name":"Poo
-0000b9e0: 6c43 7265 6174 6564 222c 2274 7970 6522  lCreated","type"
-0000b9f0: 3a22 6576 656e 7422 7d2c 7b22 696e 7075  :"event"},{"inpu
-0000ba00: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0000ba10: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0000ba20: 6e61 6d65 223a 2274 6f6b 656e 4122 2c22  name":"tokenA","
-0000ba30: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0000ba40: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000ba50: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0000ba60: 223a 2274 6f6b 656e 4222 2c22 7479 7065  ":"tokenB","type
-0000ba70: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0000ba80: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000ba90: 6e74 3234 222c 226e 616d 6522 3a22 6665  nt24","name":"fe
-0000baa0: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
-0000bab0: 3422 7d5d 2c22 6e61 6d65 223a 2263 7265  4"}],"name":"cre
-0000bac0: 6174 6550 6f6f 6c22 2c22 6f75 7470 7574  atePool","output
-0000bad0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000bae0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0000baf0: 616d 6522 3a22 706f 6f6c 222c 2274 7970  ame":"pool","typ
-0000bb00: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-0000bb10: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0000bb20: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-0000bb30: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0000bb40: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0000bb50: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0000bb60: 7432 3422 2c22 6e61 6d65 223a 2266 6565  t24","name":"fee
-0000bb70: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
-0000bb80: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0000bb90: 6522 3a22 696e 7432 3422 2c22 6e61 6d65  e":"int24","name
-0000bba0: 223a 2274 6963 6b53 7061 6369 6e67 222c  ":"tickSpacing",
-0000bbb0: 2274 7970 6522 3a22 696e 7432 3422 7d5d  "type":"int24"}]
-0000bbc0: 2c22 6e61 6d65 223a 2265 6e61 626c 6546  ,"name":"enableF
-0000bbd0: 6565 416d 6f75 6e74 222c 226f 7574 7075  eeAmount","outpu
-0000bbe0: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
-0000bbf0: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-0000bc00: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-0000bc10: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-0000bc20: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000bc30: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
-0000bc40: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
-0000bc50: 696e 7432 3422 7d5d 2c22 6e61 6d65 223a  int24"}],"name":
-0000bc60: 2266 6565 416d 6f75 6e74 5469 636b 5370  "feeAmountTickSp
-0000bc70: 6163 696e 6722 2c22 6f75 7470 7574 7322  acing","outputs"
-0000bc80: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0000bc90: 223a 2269 6e74 3234 222c 226e 616d 6522  ":"int24","name"
-0000bca0: 3a22 222c 2274 7970 6522 3a22 696e 7432  :"","type":"int2
-0000bcb0: 3422 7d5d 2c22 7374 6174 654d 7574 6162  4"}],"stateMutab
-0000bcc0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
-0000bcd0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0000bce0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0000bcf0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000bd00: 7265 7373 222c 226e 616d 6522 3a22 222c  ress","name":"",
-0000bd10: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0000bd20: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000bd30: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000bd40: 6522 3a22 222c 2274 7970 6522 3a22 6164  e":"","type":"ad
-0000bd50: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0000bd60: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
-0000bd70: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-0000bd80: 223a 2275 696e 7432 3422 7d5d 2c22 6e61  ":"uint24"}],"na
-0000bd90: 6d65 223a 2267 6574 506f 6f6c 222c 226f  me":"getPool","o
-0000bda0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-0000bdb0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0000bdc0: 7322 2c22 6e61 6d65 223a 2222 2c22 7479  s","name":"","ty
-0000bdd0: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-0000bde0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000bdf0: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-0000be00: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-0000be10: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0000be20: 226f 776e 6572 222c 226f 7574 7075 7473  "owner","outputs
-0000be30: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000be40: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000be50: 6d65 223a 2222 2c22 7479 7065 223a 2261  me":"","type":"a
-0000be60: 6464 7265 7373 227d 5d2c 2273 7461 7465  ddress"}],"state
-0000be70: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-0000be80: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-0000be90: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0000bea0: 5b5d 2c22 6e61 6d65 223a 2270 6172 616d  [],"name":"param
-0000beb0: 6574 6572 7322 2c22 6f75 7470 7574 7322  eters","outputs"
-0000bec0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0000bed0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000bee0: 6522 3a22 6661 6374 6f72 7922 2c22 7479  e":"factory","ty
-0000bef0: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0000bf00: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000bf10: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0000bf20: 2274 6f6b 656e 3022 2c22 7479 7065 223a  "token0","type":
-0000bf30: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0000bf40: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000bf50: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000bf60: 656e 3122 2c22 7479 7065 223a 2261 6464  en1","type":"add
-0000bf70: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0000bf80: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-0000bf90: 226e 616d 6522 3a22 6665 6522 2c22 7479  "name":"fee","ty
-0000bfa0: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
-0000bfb0: 696e 7465 726e 616c 5479 7065 223a 2269  internalType":"i
-0000bfc0: 6e74 3234 222c 226e 616d 6522 3a22 7469  nt24","name":"ti
-0000bfd0: 636b 5370 6163 696e 6722 2c22 7479 7065  ckSpacing","type
-0000bfe0: 223a 2269 6e74 3234 227d 5d2c 2273 7461  ":"int24"}],"sta
-0000bff0: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
-0000c000: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
-0000c010: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-0000c020: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000c030: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000c040: 6d65 223a 225f 6f77 6e65 7222 2c22 7479  me":"_owner","ty
-0000c050: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-0000c060: 226e 616d 6522 3a22 7365 744f 776e 6572  "name":"setOwner
-0000c070: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
-0000c080: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0000c090: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-0000c0a0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0000c0b0: 5d27 0a20 2020 2075 6e69 7377 6170 5f76  ]'.    uniswap_v
-0000c0c0: 335f 7061 6972 5f61 6269 3d27 5b20 7b20  3_pair_abi='[ { 
-0000c0d0: 2261 6e6f 6e79 6d6f 7573 223a 2066 616c  "anonymous": fal
-0000c0e0: 7365 2c20 2269 6e70 7574 7322 3a20 5b20  se, "inputs": [ 
-0000c0f0: 7b20 2269 6e64 6578 6564 223a 2074 7275  { "indexed": tru
-0000c100: 652c 2022 696e 7465 726e 616c 5479 7065  e, "internalType
-0000c110: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000c120: 616d 6522 3a20 226f 776e 6572 222c 2022  ame": "owner", "
-0000c130: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
-0000c140: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
-0000c150: 2074 7275 652c 2022 696e 7465 726e 616c   true, "internal
-0000c160: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000c170: 2c20 226e 616d 6522 3a20 2273 7065 6e64  , "name": "spend
-0000c180: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
-0000c190: 6472 6573 7322 207d 2c20 7b20 2269 6e64  dress" }, { "ind
-0000c1a0: 6578 6564 223a 2066 616c 7365 2c20 2269  exed": false, "i
-0000c1b0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000c1c0: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
-0000c1d0: 2022 7661 6c75 6522 2c20 2274 7970 6522   "value", "type"
-0000c1e0: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
-0000c1f0: 2022 6e61 6d65 223a 2022 4170 7072 6f76   "name": "Approv
-0000c200: 616c 222c 2022 7479 7065 223a 2022 6576  al", "type": "ev
-0000c210: 656e 7422 207d 2c20 7b20 2261 6e6f 6e79  ent" }, { "anony
-0000c220: 6d6f 7573 223a 2066 616c 7365 2c20 2269  mous": false, "i
-0000c230: 6e70 7574 7322 3a20 5b20 7b20 2269 6e64  nputs": [ { "ind
-0000c240: 6578 6564 223a 2074 7275 652c 2022 696e  exed": true, "in
-0000c250: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000c260: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000c270: 2273 656e 6465 7222 2c20 2274 7970 6522  "sender", "type"
-0000c280: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
-0000c290: 2022 696e 6465 7865 6422 3a20 6661 6c73   "indexed": fals
-0000c2a0: 652c 2022 696e 7465 726e 616c 5479 7065  e, "internalType
-0000c2b0: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
-0000c2c0: 616d 6522 3a20 2261 6d6f 756e 7430 222c  ame": "amount0",
-0000c2d0: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
-0000c2e0: 3622 207d 2c20 7b20 2269 6e64 6578 6564  6" }, { "indexed
-0000c2f0: 223a 2066 616c 7365 2c20 2269 6e74 6572  ": false, "inter
-0000c300: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000c310: 3536 222c 2022 6e61 6d65 223a 2022 616d  56", "name": "am
-0000c320: 6f75 6e74 3122 2c20 2274 7970 6522 3a20  ount1", "type": 
-0000c330: 2275 696e 7432 3536 2220 7d2c 207b 2022  "uint256" }, { "
-0000c340: 696e 6465 7865 6422 3a20 7472 7565 2c20  indexed": true, 
-0000c350: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000c360: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
-0000c370: 223a 2022 746f 222c 2022 7479 7065 223a  ": "to", "type":
-0000c380: 2022 6164 6472 6573 7322 207d 205d 2c20   "address" } ], 
-0000c390: 226e 616d 6522 3a20 2242 7572 6e22 2c20  "name": "Burn", 
-0000c3a0: 2274 7970 6522 3a20 2265 7665 6e74 2220  "type": "event" 
-0000c3b0: 7d2c 207b 2022 616e 6f6e 796d 6f75 7322  }, { "anonymous"
-0000c3c0: 3a20 6661 6c73 652c 2022 696e 7075 7473  : false, "inputs
-0000c3d0: 223a 205b 207b 2022 696e 6465 7865 6422  ": [ { "indexed"
-0000c3e0: 3a20 7472 7565 2c20 2269 6e74 6572 6e61  : true, "interna
-0000c3f0: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-0000c400: 222c 2022 6e61 6d65 223a 2022 7365 6e64  ", "name": "send
-0000c410: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
-0000c420: 6472 6573 7322 207d 2c20 7b20 2269 6e64  dress" }, { "ind
-0000c430: 6578 6564 223a 2066 616c 7365 2c20 2269  exed": false, "i
-0000c440: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000c450: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
-0000c460: 2022 616d 6f75 6e74 3022 2c20 2274 7970   "amount0", "typ
-0000c470: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
-0000c480: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
-0000c490: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
-0000c4a0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000c4b0: 226e 616d 6522 3a20 2261 6d6f 756e 7431  "name": "amount1
-0000c4c0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-0000c4d0: 3235 3622 207d 205d 2c20 226e 616d 6522  256" } ], "name"
-0000c4e0: 3a20 224d 696e 7422 2c20 2274 7970 6522  : "Mint", "type"
-0000c4f0: 3a20 2265 7665 6e74 2220 7d2c 207b 2022  : "event" }, { "
-0000c500: 616e 6f6e 796d 6f75 7322 3a20 6661 6c73  anonymous": fals
-0000c510: 652c 2022 696e 7075 7473 223a 205b 207b  e, "inputs": [ {
-0000c520: 2022 696e 6465 7865 6422 3a20 7472 7565   "indexed": true
-0000c530: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
-0000c540: 3a20 2261 6464 7265 7373 222c 2022 6e61  : "address", "na
-0000c550: 6d65 223a 2022 7365 6e64 6572 222c 2022  me": "sender", "
-0000c560: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
-0000c570: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
-0000c580: 2066 616c 7365 2c20 2269 6e74 6572 6e61   false, "interna
-0000c590: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000c5a0: 222c 2022 6e61 6d65 223a 2022 616d 6f75  ", "name": "amou
-0000c5b0: 6e74 3049 6e22 2c20 2274 7970 6522 3a20  nt0In", "type": 
-0000c5c0: 2275 696e 7432 3536 2220 7d2c 207b 2022  "uint256" }, { "
-0000c5d0: 696e 6465 7865 6422 3a20 6661 6c73 652c  indexed": false,
-0000c5e0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000c5f0: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-0000c600: 6522 3a20 2261 6d6f 756e 7431 496e 222c  e": "amount1In",
-0000c610: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
-0000c620: 3622 207d 2c20 7b20 2269 6e64 6578 6564  6" }, { "indexed
-0000c630: 223a 2066 616c 7365 2c20 2269 6e74 6572  ": false, "inter
-0000c640: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000c650: 3536 222c 2022 6e61 6d65 223a 2022 616d  56", "name": "am
-0000c660: 6f75 6e74 304f 7574 222c 2022 7479 7065  ount0Out", "type
-0000c670: 223a 2022 7569 6e74 3235 3622 207d 2c20  ": "uint256" }, 
-0000c680: 7b20 2269 6e64 6578 6564 223a 2066 616c  { "indexed": fal
-0000c690: 7365 2c20 2269 6e74 6572 6e61 6c54 7970  se, "internalTyp
-0000c6a0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
-0000c6b0: 6e61 6d65 223a 2022 616d 6f75 6e74 314f  name": "amount1O
-0000c6c0: 7574 222c 2022 7479 7065 223a 2022 7569  ut", "type": "ui
-0000c6d0: 6e74 3235 3622 207d 2c20 7b20 2269 6e64  nt256" }, { "ind
-0000c6e0: 6578 6564 223a 2074 7275 652c 2022 696e  exed": true, "in
-0000c6f0: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000c700: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000c710: 2274 6f22 2c20 2274 7970 6522 3a20 2261  "to", "type": "a
-0000c720: 6464 7265 7373 2220 7d20 5d2c 2022 6e61  ddress" } ], "na
-0000c730: 6d65 223a 2022 5377 6170 222c 2022 7479  me": "Swap", "ty
-0000c740: 7065 223a 2022 6576 656e 7422 207d 2c20  pe": "event" }, 
-0000c750: 7b20 2261 6e6f 6e79 6d6f 7573 223a 2066  { "anonymous": f
-0000c760: 616c 7365 2c20 2269 6e70 7574 7322 3a20  alse, "inputs": 
-0000c770: 5b20 7b20 2269 6e64 6578 6564 223a 2066  [ { "indexed": f
-0000c780: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
-0000c790: 7970 6522 3a20 2275 696e 7431 3132 222c  ype": "uint112",
-0000c7a0: 2022 6e61 6d65 223a 2022 7265 7365 7276   "name": "reserv
-0000c7b0: 6530 222c 2022 7479 7065 223a 2022 7569  e0", "type": "ui
-0000c7c0: 6e74 3131 3222 207d 2c20 7b20 2269 6e64  nt112" }, { "ind
-0000c7d0: 6578 6564 223a 2066 616c 7365 2c20 2269  exed": false, "i
-0000c7e0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000c7f0: 696e 7431 3132 222c 2022 6e61 6d65 223a  int112", "name":
-0000c800: 2022 7265 7365 7276 6531 222c 2022 7479   "reserve1", "ty
-0000c810: 7065 223a 2022 7569 6e74 3131 3222 207d  pe": "uint112" }
-0000c820: 205d 2c20 226e 616d 6522 3a20 2253 796e   ], "name": "Syn
-0000c830: 6322 2c20 2274 7970 6522 3a20 2265 7665  c", "type": "eve
-0000c840: 6e74 2220 7d2c 207b 2022 616e 6f6e 796d  nt" }, { "anonym
-0000c850: 6f75 7322 3a20 6661 6c73 652c 2022 696e  ous": false, "in
-0000c860: 7075 7473 223a 205b 207b 2022 696e 6465  puts": [ { "inde
-0000c870: 7865 6422 3a20 7472 7565 2c20 2269 6e74  xed": true, "int
-0000c880: 6572 6e61 6c54 7970 6522 3a20 2261 6464  ernalType": "add
-0000c890: 7265 7373 222c 2022 6e61 6d65 223a 2022  ress", "name": "
-0000c8a0: 6672 6f6d 222c 2022 7479 7065 223a 2022  from", "type": "
-0000c8b0: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-0000c8c0: 6e64 6578 6564 223a 2074 7275 652c 2022  ndexed": true, "
-0000c8d0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000c8e0: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
-0000c8f0: 3a20 2274 6f22 2c20 2274 7970 6522 3a20  : "to", "type": 
-0000c900: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
-0000c910: 696e 6465 7865 6422 3a20 6661 6c73 652c  indexed": false,
-0000c920: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000c930: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-0000c940: 6522 3a20 2276 616c 7565 222c 2022 7479  e": "value", "ty
-0000c950: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-0000c960: 205d 2c20 226e 616d 6522 3a20 2254 7261   ], "name": "Tra
-0000c970: 6e73 6665 7222 2c20 2274 7970 6522 3a20  nsfer", "type": 
-0000c980: 2265 7665 6e74 2220 7d2c 207b 2022 696e  "event" }, { "in
-0000c990: 7075 7473 223a 205b 5d2c 2022 6e61 6d65  puts": [], "name
-0000c9a0: 223a 2022 444f 4d41 494e 5f53 4550 4152  ": "DOMAIN_SEPAR
-0000c9b0: 4154 4f52 222c 2022 6f75 7470 7574 7322  ATOR", "outputs"
-0000c9c0: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000c9d0: 7970 6522 3a20 2262 7974 6573 3332 222c  ype": "bytes32",
-0000c9e0: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000c9f0: 7065 223a 2022 6279 7465 7333 3222 207d  pe": "bytes32" }
-0000ca00: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-0000ca10: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
-0000ca20: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-0000ca30: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-0000ca40: 205b 5d2c 2022 6e61 6d65 223a 2022 4d49   [], "name": "MI
-0000ca50: 4e49 4d55 4d5f 4c49 5155 4944 4954 5922  NIMUM_LIQUIDITY"
-0000ca60: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-0000ca70: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000ca80: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-0000ca90: 6522 3a20 2222 2c20 2274 7970 6522 3a20  e": "", "type": 
-0000caa0: 2275 696e 7432 3536 2220 7d20 5d2c 2022  "uint256" } ], "
-0000cab0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0000cac0: 3a20 2270 7572 6522 2c20 2274 7970 6522  : "pure", "type"
-0000cad0: 3a20 2266 756e 6374 696f 6e22 207d 2c20  : "function" }, 
-0000cae0: 7b20 2269 6e70 7574 7322 3a20 5b5d 2c20  { "inputs": [], 
-0000caf0: 226e 616d 6522 3a20 2250 4552 4d49 545f  "name": "PERMIT_
-0000cb00: 5459 5045 4841 5348 222c 2022 6f75 7470  TYPEHASH", "outp
-0000cb10: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000cb20: 6e61 6c54 7970 6522 3a20 2262 7974 6573  nalType": "bytes
-0000cb30: 3332 222c 2022 6e61 6d65 223a 2022 222c  32", "name": "",
-0000cb40: 2022 7479 7065 223a 2022 6279 7465 7333   "type": "bytes3
-0000cb50: 3222 207d 205d 2c20 2273 7461 7465 4d75  2" } ], "stateMu
-0000cb60: 7461 6269 6c69 7479 223a 2022 7075 7265  tability": "pure
-0000cb70: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
-0000cb80: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
-0000cb90: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000cba0: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
-0000cbb0: 7322 2c20 226e 616d 6522 3a20 226f 776e  s", "name": "own
-0000cbc0: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
-0000cbd0: 6472 6573 7322 207d 2c20 7b20 2269 6e74  dress" }, { "int
-0000cbe0: 6572 6e61 6c54 7970 6522 3a20 2261 6464  ernalType": "add
-0000cbf0: 7265 7373 222c 2022 6e61 6d65 223a 2022  ress", "name": "
-0000cc00: 7370 656e 6465 7222 2c20 2274 7970 6522  spender", "type"
-0000cc10: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000cc20: 2022 6e61 6d65 223a 2022 616c 6c6f 7761   "name": "allowa
-0000cc30: 6e63 6522 2c20 226f 7574 7075 7473 223a  nce", "outputs":
-0000cc40: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-0000cc50: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000cc60: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000cc70: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-0000cc80: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000cc90: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-0000cca0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000ccb0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000ccc0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000ccd0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000cce0: 6e61 6d65 223a 2022 7370 656e 6465 7222  name": "spender"
-0000ccf0: 2c20 2274 7970 6522 3a20 2261 6464 7265  , "type": "addre
-0000cd00: 7373 2220 7d2c 207b 2022 696e 7465 726e  ss" }, { "intern
-0000cd10: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-0000cd20: 3622 2c20 226e 616d 6522 3a20 2276 616c  6", "name": "val
-0000cd30: 7565 222c 2022 7479 7065 223a 2022 7569  ue", "type": "ui
-0000cd40: 6e74 3235 3622 207d 205d 2c20 226e 616d  nt256" } ], "nam
-0000cd50: 6522 3a20 2261 7070 726f 7665 222c 2022  e": "approve", "
-0000cd60: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
-0000cd70: 6e74 6572 6e61 6c54 7970 6522 3a20 2262  nternalType": "b
-0000cd80: 6f6f 6c22 2c20 226e 616d 6522 3a20 2222  ool", "name": ""
-0000cd90: 2c20 2274 7970 6522 3a20 2262 6f6f 6c22  , "type": "bool"
-0000cda0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000cdb0: 6269 6c69 7479 223a 2022 6e6f 6e70 6179  bility": "nonpay
-0000cdc0: 6162 6c65 222c 2022 7479 7065 223a 2022  able", "type": "
-0000cdd0: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-0000cde0: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
-0000cdf0: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000ce00: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000ce10: 226f 776e 6572 222c 2022 7479 7065 223a  "owner", "type":
-0000ce20: 2022 6164 6472 6573 7322 207d 205d 2c20   "address" } ], 
-0000ce30: 226e 616d 6522 3a20 2262 616c 616e 6365  "name": "balance
-0000ce40: 4f66 222c 2022 6f75 7470 7574 7322 3a20  Of", "outputs": 
-0000ce50: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000ce60: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
-0000ce70: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000ce80: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
-0000ce90: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000cea0: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-0000ceb0: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000cec0: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000ced0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000cee0: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000cef0: 616d 6522 3a20 2274 6f22 2c20 2274 7970  ame": "to", "typ
-0000cf00: 6522 3a20 2261 6464 7265 7373 2220 7d20  e": "address" } 
-0000cf10: 5d2c 2022 6e61 6d65 223a 2022 6275 726e  ], "name": "burn
-0000cf20: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
-0000cf30: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000cf40: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000cf50: 6d65 223a 2022 616d 6f75 6e74 3022 2c20  me": "amount0", 
-0000cf60: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
-0000cf70: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-0000cf80: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
-0000cf90: 2c20 226e 616d 6522 3a20 2261 6d6f 756e  , "name": "amoun
-0000cfa0: 7431 222c 2022 7479 7065 223a 2022 7569  t1", "type": "ui
-0000cfb0: 6e74 3235 3622 207d 205d 2c20 2273 7461  nt256" } ], "sta
-0000cfc0: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
-0000cfd0: 6e6f 6e70 6179 6162 6c65 222c 2022 7479  nonpayable", "ty
-0000cfe0: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000cff0: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000d000: 5d2c 2022 6e61 6d65 223a 2022 6465 6369  ], "name": "deci
-0000d010: 6d61 6c73 222c 2022 6f75 7470 7574 7322  mals", "outputs"
-0000d020: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000d030: 7970 6522 3a20 2275 696e 7438 222c 2022  ype": "uint8", "
-0000d040: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000d050: 223a 2022 7569 6e74 3822 207d 205d 2c20  ": "uint8" } ], 
-0000d060: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000d070: 223a 2022 7075 7265 222c 2022 7479 7065  ": "pure", "type
-0000d080: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
-0000d090: 207b 2022 696e 7075 7473 223a 205b 5d2c   { "inputs": [],
-0000d0a0: 2022 6e61 6d65 223a 2022 6661 6374 6f72   "name": "factor
-0000d0b0: 7922 2c20 226f 7574 7075 7473 223a 205b  y", "outputs": [
-0000d0c0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000d0d0: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000d0e0: 616d 6522 3a20 2222 2c20 2274 7970 6522  ame": "", "type"
-0000d0f0: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000d100: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000d110: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
-0000d120: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-0000d130: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-0000d140: 2c20 226e 616d 6522 3a20 2267 6574 5265  , "name": "getRe
-0000d150: 7365 7276 6573 222c 2022 6f75 7470 7574  serves", "output
-0000d160: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000d170: 6c54 7970 6522 3a20 2275 696e 7431 3132  lType": "uint112
-0000d180: 222c 2022 6e61 6d65 223a 2022 7265 7365  ", "name": "rese
-0000d190: 7276 6530 222c 2022 7479 7065 223a 2022  rve0", "type": "
-0000d1a0: 7569 6e74 3131 3222 207d 2c20 7b20 2269  uint112" }, { "i
-0000d1b0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000d1c0: 696e 7431 3132 222c 2022 6e61 6d65 223a  int112", "name":
-0000d1d0: 2022 7265 7365 7276 6531 222c 2022 7479   "reserve1", "ty
-0000d1e0: 7065 223a 2022 7569 6e74 3131 3222 207d  pe": "uint112" }
-0000d1f0: 2c20 7b20 2269 6e74 6572 6e61 6c54 7970  , { "internalTyp
-0000d200: 6522 3a20 2275 696e 7433 3222 2c20 226e  e": "uint32", "n
-0000d210: 616d 6522 3a20 2262 6c6f 636b 5469 6d65  ame": "blockTime
-0000d220: 7374 616d 704c 6173 7422 2c20 2274 7970  stampLast", "typ
-0000d230: 6522 3a20 2275 696e 7433 3222 207d 205d  e": "uint32" } ]
-0000d240: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000d250: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-0000d260: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000d270: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000d280: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000d290: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000d2a0: 616d 6522 3a20 2222 2c20 2274 7970 6522  ame": "", "type"
-0000d2b0: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
-0000d2c0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000d2d0: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
-0000d2e0: 6522 3a20 2222 2c20 2274 7970 6522 3a20  e": "", "type": 
-0000d2f0: 2261 6464 7265 7373 2220 7d20 5d2c 2022  "address" } ], "
-0000d300: 6e61 6d65 223a 2022 696e 6974 6961 6c69  name": "initiali
-0000d310: 7a65 222c 2022 6f75 7470 7574 7322 3a20  ze", "outputs": 
-0000d320: 5b5d 2c20 2273 7461 7465 4d75 7461 6269  [], "stateMutabi
-0000d330: 6c69 7479 223a 2022 6e6f 6e70 6179 6162  lity": "nonpayab
-0000d340: 6c65 222c 2022 7479 7065 223a 2022 6675  le", "type": "fu
-0000d350: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-0000d360: 7075 7473 223a 205b 5d2c 2022 6e61 6d65  puts": [], "name
-0000d370: 223a 2022 6b4c 6173 7422 2c20 226f 7574  ": "kLast", "out
-0000d380: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000d390: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000d3a0: 3235 3622 2c20 226e 616d 6522 3a20 2222  256", "name": ""
-0000d3b0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
-0000d3c0: 3536 2220 7d20 5d2c 2022 7374 6174 654d  56" } ], "stateM
-0000d3d0: 7574 6162 696c 6974 7922 3a20 2276 6965  utability": "vie
-0000d3e0: 7722 2c20 2274 7970 6522 3a20 2266 756e  w", "type": "fun
-0000d3f0: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
-0000d400: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000d410: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000d420: 7373 222c 2022 6e61 6d65 223a 2022 746f  ss", "name": "to
-0000d430: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000d440: 6573 7322 207d 205d 2c20 226e 616d 6522  ess" } ], "name"
-0000d450: 3a20 226d 696e 7422 2c20 226f 7574 7075  : "mint", "outpu
-0000d460: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000d470: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-0000d480: 3622 2c20 226e 616d 6522 3a20 226c 6971  6", "name": "liq
-0000d490: 7569 6469 7479 222c 2022 7479 7065 223a  uidity", "type":
-0000d4a0: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
-0000d4b0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000d4c0: 223a 2022 6e6f 6e70 6179 6162 6c65 222c  ": "nonpayable",
-0000d4d0: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000d4e0: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000d4f0: 223a 205b 5d2c 2022 6e61 6d65 223a 2022  ": [], "name": "
-0000d500: 6e61 6d65 222c 2022 6f75 7470 7574 7322  name", "outputs"
-0000d510: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000d520: 7970 6522 3a20 2273 7472 696e 6722 2c20  ype": "string", 
-0000d530: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000d540: 6522 3a20 2273 7472 696e 6722 207d 205d  e": "string" } ]
-0000d550: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000d560: 7479 223a 2022 7075 7265 222c 2022 7479  ty": "pure", "ty
-0000d570: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000d580: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000d590: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000d5a0: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000d5b0: 616d 6522 3a20 226f 776e 6572 222c 2022  ame": "owner", "
-0000d5c0: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
-0000d5d0: 207d 205d 2c20 226e 616d 6522 3a20 226e   } ], "name": "n
-0000d5e0: 6f6e 6365 7322 2c20 226f 7574 7075 7473  onces", "outputs
-0000d5f0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000d600: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
-0000d610: 2c20 226e 616d 6522 3a20 2222 2c20 2274  , "name": "", "t
-0000d620: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
-0000d630: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
-0000d640: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
-0000d650: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
-0000d660: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
-0000d670: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000d680: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
-0000d690: 2022 6e61 6d65 223a 2022 6f77 6e65 7222   "name": "owner"
-0000d6a0: 2c20 2274 7970 6522 3a20 2261 6464 7265  , "type": "addre
-0000d6b0: 7373 2220 7d2c 207b 2022 696e 7465 726e  ss" }, { "intern
-0000d6c0: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
-0000d6d0: 7322 2c20 226e 616d 6522 3a20 2273 7065  s", "name": "spe
-0000d6e0: 6e64 6572 222c 2022 7479 7065 223a 2022  nder", "type": "
-0000d6f0: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-0000d700: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000d710: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
-0000d720: 2022 7661 6c75 6522 2c20 2274 7970 6522   "value", "type"
-0000d730: 3a20 2275 696e 7432 3536 2220 7d2c 207b  : "uint256" }, {
-0000d740: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000d750: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-0000d760: 6522 3a20 2264 6561 646c 696e 6522 2c20  e": "deadline", 
-0000d770: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
-0000d780: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-0000d790: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
-0000d7a0: 226e 616d 6522 3a20 2276 222c 2022 7479  "name": "v", "ty
-0000d7b0: 7065 223a 2022 7569 6e74 3822 207d 2c20  pe": "uint8" }, 
-0000d7c0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000d7d0: 3a20 2262 7974 6573 3332 222c 2022 6e61  : "bytes32", "na
-0000d7e0: 6d65 223a 2022 7222 2c20 2274 7970 6522  me": "r", "type"
-0000d7f0: 3a20 2262 7974 6573 3332 2220 7d2c 207b  : "bytes32" }, {
-0000d800: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000d810: 2022 6279 7465 7333 3222 2c20 226e 616d   "bytes32", "nam
-0000d820: 6522 3a20 2273 222c 2022 7479 7065 223a  e": "s", "type":
-0000d830: 2022 6279 7465 7333 3222 207d 205d 2c20   "bytes32" } ], 
-0000d840: 226e 616d 6522 3a20 2270 6572 6d69 7422  "name": "permit"
-0000d850: 2c20 226f 7574 7075 7473 223a 205b 5d2c  , "outputs": [],
-0000d860: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000d870: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
-0000d880: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000d890: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
-0000d8a0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
-0000d8b0: 2270 7269 6365 3043 756d 756c 6174 6976  "price0Cumulativ
-0000d8c0: 654c 6173 7422 2c20 226f 7574 7075 7473  eLast", "outputs
-0000d8d0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000d8e0: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
-0000d8f0: 2c20 226e 616d 6522 3a20 2222 2c20 2274  , "name": "", "t
-0000d900: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
-0000d910: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
-0000d920: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
-0000d930: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
-0000d940: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
-0000d950: 3a20 5b5d 2c20 226e 616d 6522 3a20 2270  : [], "name": "p
-0000d960: 7269 6365 3143 756d 756c 6174 6976 654c  rice1CumulativeL
-0000d970: 6173 7422 2c20 226f 7574 7075 7473 223a  ast", "outputs":
-0000d980: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-0000d990: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000d9a0: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000d9b0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-0000d9c0: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000d9d0: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-0000d9e0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000d9f0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000da00: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000da10: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000da20: 6e61 6d65 223a 2022 746f 222c 2022 7479  name": "to", "ty
-0000da30: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
-0000da40: 205d 2c20 226e 616d 6522 3a20 2273 6b69   ], "name": "ski
-0000da50: 6d22 2c20 226f 7574 7075 7473 223a 205b  m", "outputs": [
-0000da60: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000da70: 6974 7922 3a20 226e 6f6e 7061 7961 626c  ity": "nonpayabl
-0000da80: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
-0000da90: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
-0000daa0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000dab0: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000dac0: 3536 222c 2022 6e61 6d65 223a 2022 616d  56", "name": "am
-0000dad0: 6f75 6e74 304f 7574 222c 2022 7479 7065  ount0Out", "type
-0000dae0: 223a 2022 7569 6e74 3235 3622 207d 2c20  ": "uint256" }, 
-0000daf0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000db00: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000db10: 6d65 223a 2022 616d 6f75 6e74 314f 7574  me": "amount1Out
-0000db20: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-0000db30: 3235 3622 207d 2c20 7b20 2269 6e74 6572  256" }, { "inter
-0000db40: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000db50: 7373 222c 2022 6e61 6d65 223a 2022 746f  ss", "name": "to
-0000db60: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000db70: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
-0000db80: 6e61 6c54 7970 6522 3a20 2262 7974 6573  nalType": "bytes
-0000db90: 222c 2022 6e61 6d65 223a 2022 6461 7461  ", "name": "data
-0000dba0: 222c 2022 7479 7065 223a 2022 6279 7465  ", "type": "byte
-0000dbb0: 7322 207d 205d 2c20 226e 616d 6522 3a20  s" } ], "name": 
-0000dbc0: 2273 7761 7022 2c20 226f 7574 7075 7473  "swap", "outputs
-0000dbd0: 223a 205b 5d2c 2022 7374 6174 654d 7574  ": [], "stateMut
-0000dbe0: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
-0000dbf0: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
-0000dc00: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-0000dc10: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
-0000dc20: 616d 6522 3a20 2273 796d 626f 6c22 2c20  ame": "symbol", 
-0000dc30: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-0000dc40: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000dc50: 7374 7269 6e67 222c 2022 6e61 6d65 223a  string", "name":
-0000dc60: 2022 222c 2022 7479 7065 223a 2022 7374   "", "type": "st
-0000dc70: 7269 6e67 2220 7d20 5d2c 2022 7374 6174  ring" } ], "stat
-0000dc80: 654d 7574 6162 696c 6974 7922 3a20 2270  eMutability": "p
-0000dc90: 7572 6522 2c20 2274 7970 6522 3a20 2266  ure", "type": "f
-0000dca0: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
-0000dcb0: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
-0000dcc0: 6522 3a20 2273 796e 6322 2c20 226f 7574  e": "sync", "out
-0000dcd0: 7075 7473 223a 205b 5d2c 2022 7374 6174  puts": [], "stat
-0000dce0: 654d 7574 6162 696c 6974 7922 3a20 226e  eMutability": "n
-0000dcf0: 6f6e 7061 7961 626c 6522 2c20 2274 7970  onpayable", "typ
-0000dd00: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-0000dd10: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-0000dd20: 2c20 226e 616d 6522 3a20 2274 6f6b 656e  , "name": "token
-0000dd30: 3022 2c20 226f 7574 7075 7473 223a 205b  0", "outputs": [
-0000dd40: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000dd50: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000dd60: 616d 6522 3a20 2222 2c20 2274 7970 6522  ame": "", "type"
-0000dd70: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000dd80: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000dd90: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
-0000dda0: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-0000ddb0: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-0000ddc0: 2c20 226e 616d 6522 3a20 2274 6f6b 656e  , "name": "token
-0000ddd0: 3122 2c20 226f 7574 7075 7473 223a 205b  1", "outputs": [
-0000dde0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000ddf0: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000de00: 616d 6522 3a20 2222 2c20 2274 7970 6522  ame": "", "type"
-0000de10: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000de20: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000de30: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
-0000de40: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-0000de50: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-0000de60: 2c20 226e 616d 6522 3a20 2274 6f74 616c  , "name": "total
-0000de70: 5375 7070 6c79 222c 2022 6f75 7470 7574  Supply", "output
-0000de80: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000de90: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000dea0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
-0000deb0: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
-0000dec0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000ded0: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
-0000dee0: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000def0: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000df00: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000df10: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000df20: 2c20 226e 616d 6522 3a20 2274 6f22 2c20  , "name": "to", 
-0000df30: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000df40: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-0000df50: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
-0000df60: 2c20 226e 616d 6522 3a20 2276 616c 7565  , "name": "value
-0000df70: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-0000df80: 3235 3622 207d 205d 2c20 226e 616d 6522  256" } ], "name"
-0000df90: 3a20 2274 7261 6e73 6665 7222 2c20 226f  : "transfer", "o
-0000dfa0: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
-0000dfb0: 7465 726e 616c 5479 7065 223a 2022 626f  ternalType": "bo
-0000dfc0: 6f6c 222c 2022 6e61 6d65 223a 2022 222c  ol", "name": "",
-0000dfd0: 2022 7479 7065 223a 2022 626f 6f6c 2220   "type": "bool" 
-0000dfe0: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
-0000dff0: 696c 6974 7922 3a20 226e 6f6e 7061 7961  ility": "nonpaya
-0000e000: 626c 6522 2c20 2274 7970 6522 3a20 2266  ble", "type": "f
-0000e010: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
-0000e020: 6e70 7574 7322 3a20 5b20 7b20 2269 6e74  nputs": [ { "int
-0000e030: 6572 6e61 6c54 7970 6522 3a20 2261 6464  ernalType": "add
-0000e040: 7265 7373 222c 2022 6e61 6d65 223a 2022  ress", "name": "
-0000e050: 6672 6f6d 222c 2022 7479 7065 223a 2022  from", "type": "
-0000e060: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-0000e070: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000e080: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000e090: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
-0000e0a0: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-0000e0b0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000e0c0: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
-0000e0d0: 2022 7661 6c75 6522 2c20 2274 7970 6522   "value", "type"
-0000e0e0: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
-0000e0f0: 2022 6e61 6d65 223a 2022 7472 616e 7366   "name": "transf
-0000e100: 6572 4672 6f6d 222c 2022 6f75 7470 7574  erFrom", "output
-0000e110: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000e120: 6c54 7970 6522 3a20 2262 6f6f 6c22 2c20  lType": "bool", 
-0000e130: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000e140: 6522 3a20 2262 6f6f 6c22 207d 205d 2c20  e": "bool" } ], 
-0000e150: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000e160: 223a 2022 6e6f 6e70 6179 6162 6c65 222c  ": "nonpayable",
-0000e170: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000e180: 6f6e 2220 7d20 5d27 0a20 2020 2075 6e69  on" } ]'.    uni
-0000e190: 7377 6170 5f76 335f 6572 6332 305f 6162  swap_v3_erc20_ab
-0000e1a0: 693d 275b 207b 2022 616e 6f6e 796d 6f75  i='[ { "anonymou
-0000e1b0: 7322 3a20 6661 6c73 652c 2022 696e 7075  s": false, "inpu
-0000e1c0: 7473 223a 205b 207b 2022 696e 6465 7865  ts": [ { "indexe
-0000e1d0: 6422 3a20 7472 7565 2c20 2269 6e74 6572  d": true, "inter
-0000e1e0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000e1f0: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
-0000e200: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
-0000e210: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-0000e220: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
-0000e230: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000e240: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000e250: 2022 7370 656e 6465 7222 2c20 2274 7970   "spender", "typ
-0000e260: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
-0000e270: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
-0000e280: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
-0000e290: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000e2a0: 226e 616d 6522 3a20 2276 616c 7565 222c  "name": "value",
-0000e2b0: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
-0000e2c0: 3622 207d 205d 2c20 226e 616d 6522 3a20  6" } ], "name": 
-0000e2d0: 2241 7070 726f 7661 6c22 2c20 2274 7970  "Approval", "typ
-0000e2e0: 6522 3a20 2265 7665 6e74 2220 7d2c 207b  e": "event" }, {
-0000e2f0: 2022 616e 6f6e 796d 6f75 7322 3a20 6661   "anonymous": fa
-0000e300: 6c73 652c 2022 696e 7075 7473 223a 205b  lse, "inputs": [
-0000e310: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
-0000e320: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
-0000e330: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000e340: 6e61 6d65 223a 2022 6672 6f6d 222c 2022  name": "from", "
-0000e350: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
-0000e360: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
-0000e370: 2074 7275 652c 2022 696e 7465 726e 616c   true, "internal
-0000e380: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000e390: 2c20 226e 616d 6522 3a20 2274 6f22 2c20  , "name": "to", 
-0000e3a0: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000e3b0: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
-0000e3c0: 3a20 6661 6c73 652c 2022 696e 7465 726e  : false, "intern
-0000e3d0: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-0000e3e0: 3622 2c20 226e 616d 6522 3a20 2276 616c  6", "name": "val
-0000e3f0: 7565 222c 2022 7479 7065 223a 2022 7569  ue", "type": "ui
-0000e400: 6e74 3235 3622 207d 205d 2c20 226e 616d  nt256" } ], "nam
-0000e410: 6522 3a20 2254 7261 6e73 6665 7222 2c20  e": "Transfer", 
-0000e420: 2274 7970 6522 3a20 2265 7665 6e74 2220  "type": "event" 
-0000e430: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000e440: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000e450: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000e460: 616d 6522 3a20 226f 776e 6572 222c 2022  ame": "owner", "
-0000e470: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
-0000e480: 207d 2c20 7b20 2269 6e74 6572 6e61 6c54   }, { "internalT
-0000e490: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
-0000e4a0: 2022 6e61 6d65 223a 2022 7370 656e 6465   "name": "spende
-0000e4b0: 7222 2c20 2274 7970 6522 3a20 2261 6464  r", "type": "add
-0000e4c0: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
-0000e4d0: 223a 2022 616c 6c6f 7761 6e63 6522 2c20  ": "allowance", 
-0000e4e0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-0000e4f0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000e500: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000e510: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
-0000e520: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
-0000e530: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
-0000e540: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
-0000e550: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-0000e560: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
-0000e570: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000e580: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000e590: 2022 7370 656e 6465 7222 2c20 2274 7970   "spender", "typ
-0000e5a0: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
-0000e5b0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000e5c0: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
-0000e5d0: 616d 6522 3a20 2276 616c 7565 222c 2022  ame": "value", "
-0000e5e0: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
-0000e5f0: 207d 205d 2c20 226e 616d 6522 3a20 2261   } ], "name": "a
-0000e600: 7070 726f 7665 222c 2022 6f75 7470 7574  pprove", "output
-0000e610: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000e620: 6c54 7970 6522 3a20 2262 6f6f 6c22 2c20  lType": "bool", 
-0000e630: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000e640: 6522 3a20 2262 6f6f 6c22 207d 205d 2c20  e": "bool" } ], 
-0000e650: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000e660: 223a 2022 6e6f 6e70 6179 6162 6c65 222c  ": "nonpayable",
-0000e670: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000e680: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000e690: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000e6a0: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000e6b0: 2c20 226e 616d 6522 3a20 226f 776e 6572  , "name": "owner
-0000e6c0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000e6d0: 6573 7322 207d 205d 2c20 226e 616d 6522  ess" } ], "name"
-0000e6e0: 3a20 2262 616c 616e 6365 4f66 222c 2022  : "balanceOf", "
-0000e6f0: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
-0000e700: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
-0000e710: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
-0000e720: 2022 222c 2022 7479 7065 223a 2022 7569   "", "type": "ui
-0000e730: 6e74 3235 3622 207d 205d 2c20 2273 7461  nt256" } ], "sta
-0000e740: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
-0000e750: 7669 6577 222c 2022 7479 7065 223a 2022  view", "type": "
-0000e760: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-0000e770: 696e 7075 7473 223a 205b 5d2c 2022 6e61  inputs": [], "na
-0000e780: 6d65 223a 2022 6465 6369 6d61 6c73 222c  me": "decimals",
-0000e790: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
-0000e7a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000e7b0: 2275 696e 7438 222c 2022 6e61 6d65 223a  "uint8", "name":
-0000e7c0: 2022 222c 2022 7479 7065 223a 2022 7569   "", "type": "ui
-0000e7d0: 6e74 3822 207d 205d 2c20 2273 7461 7465  nt8" } ], "state
-0000e7e0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
-0000e7f0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
-0000e800: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-0000e810: 7075 7473 223a 205b 5d2c 2022 6e61 6d65  puts": [], "name
-0000e820: 223a 2022 6e61 6d65 222c 2022 6f75 7470  ": "name", "outp
-0000e830: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000e840: 6e61 6c54 7970 6522 3a20 2273 7472 696e  nalType": "strin
-0000e850: 6722 2c20 226e 616d 6522 3a20 2222 2c20  g", "name": "", 
-0000e860: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-0000e870: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000e880: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
-0000e890: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000e8a0: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000e8b0: 223a 205b 5d2c 2022 6e61 6d65 223a 2022  ": [], "name": "
-0000e8c0: 7379 6d62 6f6c 222c 2022 6f75 7470 7574  symbol", "output
-0000e8d0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000e8e0: 6c54 7970 6522 3a20 2273 7472 696e 6722  lType": "string"
-0000e8f0: 2c20 226e 616d 6522 3a20 2222 2c20 2274  , "name": "", "t
-0000e900: 7970 6522 3a20 2273 7472 696e 6722 207d  ype": "string" }
-0000e910: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-0000e920: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
-0000e930: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-0000e940: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-0000e950: 205b 5d2c 2022 6e61 6d65 223a 2022 746f   [], "name": "to
-0000e960: 7461 6c53 7570 706c 7922 2c20 226f 7574  talSupply", "out
-0000e970: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000e980: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000e990: 3235 3622 2c20 226e 616d 6522 3a20 2222  256", "name": ""
-0000e9a0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
-0000e9b0: 3536 2220 7d20 5d2c 2022 7374 6174 654d  56" } ], "stateM
-0000e9c0: 7574 6162 696c 6974 7922 3a20 2276 6965  utability": "vie
-0000e9d0: 7722 2c20 2274 7970 6522 3a20 2266 756e  w", "type": "fun
-0000e9e0: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
-0000e9f0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000ea00: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000ea10: 7373 222c 2022 6e61 6d65 223a 2022 746f  ss", "name": "to
-0000ea20: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000ea30: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
-0000ea40: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000ea50: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
-0000ea60: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
-0000ea70: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
-0000ea80: 6d65 223a 2022 7472 616e 7366 6572 222c  me": "transfer",
-0000ea90: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
-0000eaa0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000eab0: 2262 6f6f 6c22 2c20 226e 616d 6522 3a20  "bool", "name": 
-0000eac0: 2222 2c20 2274 7970 6522 3a20 2262 6f6f  "", "type": "boo
-0000ead0: 6c22 207d 205d 2c20 2273 7461 7465 4d75  l" } ], "stateMu
-0000eae0: 7461 6269 6c69 7479 223a 2022 6e6f 6e70  tability": "nonp
-0000eaf0: 6179 6162 6c65 222c 2022 7479 7065 223a  ayable", "type":
-0000eb00: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
-0000eb10: 2022 696e 7075 7473 223a 205b 207b 2022   "inputs": [ { "
-0000eb20: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000eb30: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
-0000eb40: 3a20 2266 726f 6d22 2c20 2274 7970 6522  : "from", "type"
-0000eb50: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
-0000eb60: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000eb70: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
-0000eb80: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
-0000eb90: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
-0000eba0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000ebb0: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-0000ebc0: 6522 3a20 2276 616c 7565 222c 2022 7479  e": "value", "ty
-0000ebd0: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-0000ebe0: 205d 2c20 226e 616d 6522 3a20 2274 7261   ], "name": "tra
-0000ebf0: 6e73 6665 7246 726f 6d22 2c20 226f 7574  nsferFrom", "out
-0000ec00: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000ec10: 726e 616c 5479 7065 223a 2022 626f 6f6c  rnalType": "bool
-0000ec20: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
-0000ec30: 7479 7065 223a 2022 626f 6f6c 2220 7d20  type": "bool" } 
-0000ec40: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000ec50: 6974 7922 3a20 226e 6f6e 7061 7961 626c  ity": "nonpayabl
-0000ec60: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
-0000ec70: 6374 696f 6e22 207d 205d 270a 2020 2020  ction" } ]'.    
-0000ec80: 2368 7474 7073 3a2f 2f65 7468 6572 7363  #https://ethersc
-0000ec90: 616e 2e69 6f2f 6164 6472 6573 732f 3078  an.io/address/0x
-0000eca0: 6535 3932 3432 3761 3061 6563 6539 3264  e592427a0aece92d
-0000ecb0: 6533 6564 6565 3166 3138 6530 3135 3763  e3edee1f18e0157c
-0000ecc0: 3035 3836 3135 3634 2363 6f64 650a 2020  05861564#code.  
-0000ecd0: 2020 756e 6973 7761 705f 7633 5f72 6f75    uniswap_v3_rou
-0000ece0: 7465 5f61 6269 3d27 5b7b 2269 6e70 7574  te_abi='[{"input
-0000ecf0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000ed00: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0000ed10: 616d 6522 3a22 5f66 6163 746f 7279 222c  ame":"_factory",
-0000ed20: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0000ed30: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000ed40: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000ed50: 6522 3a22 5f57 4554 4839 222c 2274 7970  e":"_WETH9","typ
-0000ed60: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-0000ed70: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0000ed80: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-0000ed90: 7970 6522 3a22 636f 6e73 7472 7563 746f  ype":"constructo
-0000eda0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0000edb0: 2c22 6e61 6d65 223a 2257 4554 4839 222c  ,"name":"WETH9",
-0000edc0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-0000edd0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000ede0: 6573 7322 2c22 6e61 6d65 223a 2222 2c22  ess","name":"","
-0000edf0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0000ee00: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-0000ee10: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
-0000ee20: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-0000ee30: 696e 7075 7473 223a 5b7b 2263 6f6d 706f  inputs":[{"compo
-0000ee40: 6e65 6e74 7322 3a5b 7b22 696e 7465 726e  nents":[{"intern
-0000ee50: 616c 5479 7065 223a 2262 7974 6573 222c  alType":"bytes",
-0000ee60: 226e 616d 6522 3a22 7061 7468 222c 2274  "name":"path","t
-0000ee70: 7970 6522 3a22 6279 7465 7322 7d2c 7b22  ype":"bytes"},{"
-0000ee80: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0000ee90: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0000eea0: 7265 6369 7069 656e 7422 2c22 7479 7065  recipient","type
-0000eeb0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0000eec0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000eed0: 6e74 3235 3622 2c22 6e61 6d65 223a 2264  nt256","name":"d
-0000eee0: 6561 646c 696e 6522 2c22 7479 7065 223a  eadline","type":
-0000eef0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0000ef00: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0000ef10: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0000ef20: 756e 7449 6e22 2c22 7479 7065 223a 2275  untIn","type":"u
-0000ef30: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0000ef40: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0000ef50: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0000ef60: 744f 7574 4d69 6e69 6d75 6d22 2c22 7479  tOutMinimum","ty
-0000ef70: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0000ef80: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000ef90: 7374 7275 6374 2049 5377 6170 526f 7574  struct ISwapRout
-0000efa0: 6572 2e45 7861 6374 496e 7075 7450 6172  er.ExactInputPar
-0000efb0: 616d 7322 2c22 6e61 6d65 223a 2270 6172  ams","name":"par
-0000efc0: 616d 7322 2c22 7479 7065 223a 2274 7570  ams","type":"tup
-0000efd0: 6c65 227d 5d2c 226e 616d 6522 3a22 6578  le"}],"name":"ex
-0000efe0: 6163 7449 6e70 7574 222c 226f 7574 7075  actInput","outpu
-0000eff0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0000f000: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0000f010: 6e61 6d65 223a 2261 6d6f 756e 744f 7574  name":"amountOut
-0000f020: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0000f030: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
-0000f040: 696c 6974 7922 3a22 7061 7961 626c 6522  ility":"payable"
-0000f050: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-0000f060: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-0000f070: 2263 6f6d 706f 6e65 6e74 7322 3a5b 7b22  "components":[{"
-0000f080: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0000f090: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0000f0a0: 746f 6b65 6e49 6e22 2c22 7479 7065 223a  tokenIn","type":
-0000f0b0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0000f0c0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000f0d0: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000f0e0: 656e 4f75 7422 2c22 7479 7065 223a 2261  enOut","type":"a
-0000f0f0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-0000f100: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
-0000f110: 222c 226e 616d 6522 3a22 6665 6522 2c22  ","name":"fee","
-0000f120: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
-0000f130: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000f140: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0000f150: 3a22 7265 6369 7069 656e 7422 2c22 7479  :"recipient","ty
-0000f160: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0000f170: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000f180: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0000f190: 2264 6561 646c 696e 6522 2c22 7479 7065  "deadline","type
-0000f1a0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0000f1b0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000f1c0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0000f1d0: 6d6f 756e 7449 6e22 2c22 7479 7065 223a  mountIn","type":
-0000f1e0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0000f1f0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0000f200: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0000f210: 756e 744f 7574 4d69 6e69 6d75 6d22 2c22  untOutMinimum","
-0000f220: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0000f230: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000f240: 3a22 7569 6e74 3136 3022 2c22 6e61 6d65  :"uint160","name
-0000f250: 223a 2273 7172 7450 7269 6365 4c69 6d69  ":"sqrtPriceLimi
-0000f260: 7458 3936 222c 2274 7970 6522 3a22 7569  tX96","type":"ui
-0000f270: 6e74 3136 3022 7d5d 2c22 696e 7465 726e  nt160"}],"intern
-0000f280: 616c 5479 7065 223a 2273 7472 7563 7420  alType":"struct 
-0000f290: 4953 7761 7052 6f75 7465 722e 4578 6163  ISwapRouter.Exac
-0000f2a0: 7449 6e70 7574 5369 6e67 6c65 5061 7261  tInputSinglePara
-0000f2b0: 6d73 222c 226e 616d 6522 3a22 7061 7261  ms","name":"para
-0000f2c0: 6d73 222c 2274 7970 6522 3a22 7475 706c  ms","type":"tupl
-0000f2d0: 6522 7d5d 2c22 6e61 6d65 223a 2265 7861  e"}],"name":"exa
-0000f2e0: 6374 496e 7075 7453 696e 676c 6522 2c22  ctInputSingle","
-0000f2f0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0000f300: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0000f310: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0000f320: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0000f330: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0000f340: 4d75 7461 6269 6c69 7479 223a 2270 6179  Mutability":"pay
-0000f350: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-0000f360: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-0000f370: 7322 3a5b 7b22 636f 6d70 6f6e 656e 7473  s":[{"components
-0000f380: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000f390: 6522 3a22 6279 7465 7322 2c22 6e61 6d65  e":"bytes","name
-0000f3a0: 223a 2270 6174 6822 2c22 7479 7065 223a  ":"path","type":
-0000f3b0: 2262 7974 6573 227d 2c7b 2269 6e74 6572  "bytes"},{"inter
-0000f3c0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0000f3d0: 7322 2c22 6e61 6d65 223a 2272 6563 6970  s","name":"recip
-0000f3e0: 6965 6e74 222c 2274 7970 6522 3a22 6164  ient","type":"ad
-0000f3f0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0000f400: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0000f410: 222c 226e 616d 6522 3a22 6465 6164 6c69  ","name":"deadli
-0000f420: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
-0000f430: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0000f440: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0000f450: 226e 616d 6522 3a22 616d 6f75 6e74 4f75  "name":"amountOu
-0000f460: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-0000f470: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0000f480: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0000f490: 6e61 6d65 223a 2261 6d6f 756e 7449 6e4d  name":"amountInM
-0000f4a0: 6178 696d 756d 222c 2274 7970 6522 3a22  aximum","type":"
-0000f4b0: 7569 6e74 3235 3622 7d5d 2c22 696e 7465  uint256"}],"inte
-0000f4c0: 726e 616c 5479 7065 223a 2273 7472 7563  rnalType":"struc
-0000f4d0: 7420 4953 7761 7052 6f75 7465 722e 4578  t ISwapRouter.Ex
-0000f4e0: 6163 744f 7574 7075 7450 6172 616d 7322  actOutputParams"
-0000f4f0: 2c22 6e61 6d65 223a 2270 6172 616d 7322  ,"name":"params"
-0000f500: 2c22 7479 7065 223a 2274 7570 6c65 227d  ,"type":"tuple"}
-0000f510: 5d2c 226e 616d 6522 3a22 6578 6163 744f  ],"name":"exactO
-0000f520: 7574 7075 7422 2c22 6f75 7470 7574 7322  utput","outputs"
-0000f530: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0000f540: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0000f550: 6522 3a22 616d 6f75 6e74 496e 222c 2274  e":"amountIn","t
-0000f560: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0000f570: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-0000f580: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
-0000f590: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0000f5a0: 7b22 696e 7075 7473 223a 5b7b 2263 6f6d  {"inputs":[{"com
-0000f5b0: 706f 6e65 6e74 7322 3a5b 7b22 696e 7465  ponents":[{"inte
-0000f5c0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0000f5d0: 7373 222c 226e 616d 6522 3a22 746f 6b65  ss","name":"toke
-0000f5e0: 6e49 6e22 2c22 7479 7065 223a 2261 6464  nIn","type":"add
-0000f5f0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0000f600: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-0000f610: 2c22 6e61 6d65 223a 2274 6f6b 656e 4f75  ,"name":"tokenOu
-0000f620: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
-0000f630: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0000f640: 7970 6522 3a22 7569 6e74 3234 222c 226e  ype":"uint24","n
-0000f650: 616d 6522 3a22 6665 6522 2c22 7479 7065  ame":"fee","type
-0000f660: 223a 2275 696e 7432 3422 7d2c 7b22 696e  ":"uint24"},{"in
-0000f670: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000f680: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
-0000f690: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-0000f6a0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0000f6b0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0000f6c0: 3235 3622 2c22 6e61 6d65 223a 2264 6561  256","name":"dea
-0000f6d0: 646c 696e 6522 2c22 7479 7065 223a 2275  dline","type":"u
-0000f6e0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0000f6f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0000f700: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0000f710: 744f 7574 222c 2274 7970 6522 3a22 7569  tOut","type":"ui
-0000f720: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0000f730: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0000f740: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-0000f750: 496e 4d61 7869 6d75 6d22 2c22 7479 7065  InMaximum","type
-0000f760: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0000f770: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000f780: 6e74 3136 3022 2c22 6e61 6d65 223a 2273  nt160","name":"s
-0000f790: 7172 7450 7269 6365 4c69 6d69 7458 3936  qrtPriceLimitX96
-0000f7a0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-0000f7b0: 3022 7d5d 2c22 696e 7465 726e 616c 5479  0"}],"internalTy
-0000f7c0: 7065 223a 2273 7472 7563 7420 4953 7761  pe":"struct ISwa
-0000f7d0: 7052 6f75 7465 722e 4578 6163 744f 7574  pRouter.ExactOut
-0000f7e0: 7075 7453 696e 676c 6550 6172 616d 7322  putSingleParams"
-0000f7f0: 2c22 6e61 6d65 223a 2270 6172 616d 7322  ,"name":"params"
-0000f800: 2c22 7479 7065 223a 2274 7570 6c65 227d  ,"type":"tuple"}
-0000f810: 5d2c 226e 616d 6522 3a22 6578 6163 744f  ],"name":"exactO
-0000f820: 7574 7075 7453 696e 676c 6522 2c22 6f75  utputSingle","ou
-0000f830: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-0000f840: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0000f850: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-0000f860: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
-0000f870: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
-0000f880: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
-0000f890: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-0000f8a0: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0000f8b0: 5b5d 2c22 6e61 6d65 223a 2266 6163 746f  [],"name":"facto
-0000f8c0: 7279 222c 226f 7574 7075 7473 223a 5b7b  ry","outputs":[{
-0000f8d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000f8e0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0000f8f0: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-0000f900: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-0000f910: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-0000f920: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0000f930: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0000f940: 6e74 6572 6e61 6c54 7970 6522 3a22 6279  nternalType":"by
-0000f950: 7465 735b 5d22 2c22 6e61 6d65 223a 2264  tes[]","name":"d
-0000f960: 6174 6122 2c22 7479 7065 223a 2262 7974  ata","type":"byt
-0000f970: 6573 5b5d 227d 5d2c 226e 616d 6522 3a22  es[]"}],"name":"
-0000f980: 6d75 6c74 6963 616c 6c22 2c22 6f75 7470  multicall","outp
-0000f990: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0000f9a0: 5479 7065 223a 2262 7974 6573 5b5d 222c  Type":"bytes[]",
-0000f9b0: 226e 616d 6522 3a22 7265 7375 6c74 7322  "name":"results"
-0000f9c0: 2c22 7479 7065 223a 2262 7974 6573 5b5d  ,"type":"bytes[]
-0000f9d0: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-0000f9e0: 6c69 7479 223a 2270 6179 6162 6c65 222c  lity":"payable",
-0000f9f0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-0000fa00: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-0000fa10: 226e 616d 6522 3a22 7265 6675 6e64 4554  "name":"refundET
-0000fa20: 4822 2c22 6f75 7470 7574 7322 3a5b 5d2c  H","outputs":[],
-0000fa30: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000fa40: 223a 2270 6179 6162 6c65 222c 2274 7970  ":"payable","typ
-0000fa50: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-0000fa60: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0000fa70: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0000fa80: 7373 222c 226e 616d 6522 3a22 746f 6b65  ss","name":"toke
-0000fa90: 6e22 2c22 7479 7065 223a 2261 6464 7265  n","type":"addre
-0000faa0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0000fab0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0000fac0: 6e61 6d65 223a 2276 616c 7565 222c 2274  name":"value","t
-0000fad0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0000fae0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000faf0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0000fb00: 3a22 6465 6164 6c69 6e65 222c 2274 7970  :"deadline","typ
-0000fb10: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0000fb20: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000fb30: 696e 7438 222c 226e 616d 6522 3a22 7622  int8","name":"v"
-0000fb40: 2c22 7479 7065 223a 2275 696e 7438 227d  ,"type":"uint8"}
-0000fb50: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000fb60: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
-0000fb70: 223a 2272 222c 2274 7970 6522 3a22 6279  ":"r","type":"by
-0000fb80: 7465 7333 3222 7d2c 7b22 696e 7465 726e  tes32"},{"intern
-0000fb90: 616c 5479 7065 223a 2262 7974 6573 3332  alType":"bytes32
-0000fba0: 222c 226e 616d 6522 3a22 7322 2c22 7479  ","name":"s","ty
-0000fbb0: 7065 223a 2262 7974 6573 3332 227d 5d2c  pe":"bytes32"}],
-0000fbc0: 226e 616d 6522 3a22 7365 6c66 5065 726d  "name":"selfPerm
-0000fbd0: 6974 222c 226f 7574 7075 7473 223a 5b5d  it","outputs":[]
-0000fbe0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-0000fbf0: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
-0000fc00: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0000fc10: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0000fc20: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000fc30: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000fc40: 656e 222c 2274 7970 6522 3a22 6164 6472  en","type":"addr
-0000fc50: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0000fc60: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0000fc70: 226e 616d 6522 3a22 6e6f 6e63 6522 2c22  "name":"nonce","
-0000fc80: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0000fc90: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000fca0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0000fcb0: 223a 2265 7870 6972 7922 2c22 7479 7065  ":"expiry","type
-0000fcc0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0000fcd0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000fce0: 6e74 3822 2c22 6e61 6d65 223a 2276 222c  nt8","name":"v",
-0000fcf0: 2274 7970 6522 3a22 7569 6e74 3822 7d2c  "type":"uint8"},
-0000fd00: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000fd10: 2262 7974 6573 3332 222c 226e 616d 6522  "bytes32","name"
-0000fd20: 3a22 7222 2c22 7479 7065 223a 2262 7974  :"r","type":"byt
-0000fd30: 6573 3332 227d 2c7b 2269 6e74 6572 6e61  es32"},{"interna
-0000fd40: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
-0000fd50: 2c22 6e61 6d65 223a 2273 222c 2274 7970  ,"name":"s","typ
-0000fd60: 6522 3a22 6279 7465 7333 3222 7d5d 2c22  e":"bytes32"}],"
-0000fd70: 6e61 6d65 223a 2273 656c 6650 6572 6d69  name":"selfPermi
-0000fd80: 7441 6c6c 6f77 6564 222c 226f 7574 7075  tAllowed","outpu
-0000fd90: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
-0000fda0: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
-0000fdb0: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-0000fdc0: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0000fdd0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0000fde0: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0000fdf0: 223a 2274 6f6b 656e 222c 2274 7970 6522  ":"token","type"
-0000fe00: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0000fe10: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0000fe20: 7432 3536 222c 226e 616d 6522 3a22 6e6f  t256","name":"no
-0000fe30: 6e63 6522 2c22 7479 7065 223a 2275 696e  nce","type":"uin
-0000fe40: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0000fe50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0000fe60: 2c22 6e61 6d65 223a 2265 7870 6972 7922  ,"name":"expiry"
-0000fe70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0000fe80: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0000fe90: 6522 3a22 7569 6e74 3822 2c22 6e61 6d65  e":"uint8","name
-0000fea0: 223a 2276 222c 2274 7970 6522 3a22 7569  ":"v","type":"ui
-0000feb0: 6e74 3822 7d2c 7b22 696e 7465 726e 616c  nt8"},{"internal
-0000fec0: 5479 7065 223a 2262 7974 6573 3332 222c  Type":"bytes32",
-0000fed0: 226e 616d 6522 3a22 7222 2c22 7479 7065  "name":"r","type
-0000fee0: 223a 2262 7974 6573 3332 227d 2c7b 2269  ":"bytes32"},{"i
-0000fef0: 6e74 6572 6e61 6c54 7970 6522 3a22 6279  nternalType":"by
-0000ff00: 7465 7333 3222 2c22 6e61 6d65 223a 2273  tes32","name":"s
-0000ff10: 222c 2274 7970 6522 3a22 6279 7465 7333  ","type":"bytes3
-0000ff20: 3222 7d5d 2c22 6e61 6d65 223a 2273 656c  2"}],"name":"sel
-0000ff30: 6650 6572 6d69 7441 6c6c 6f77 6564 4966  fPermitAllowedIf
-0000ff40: 4e65 6365 7373 6172 7922 2c22 6f75 7470  Necessary","outp
-0000ff50: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-0000ff60: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
-0000ff70: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
-0000ff80: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0000ff90: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0000ffa0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000ffb0: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
-0000ffc0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0000ffd0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000ffe0: 6e74 3235 3622 2c22 6e61 6d65 223a 2276  nt256","name":"v
-0000fff0: 616c 7565 222c 2274 7970 6522 3a22 7569  alue","type":"ui
-00010000: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-00010010: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00010020: 222c 226e 616d 6522 3a22 6465 6164 6c69  ","name":"deadli
-00010030: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
-00010040: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00010050: 5479 7065 223a 2275 696e 7438 222c 226e  Type":"uint8","n
-00010060: 616d 6522 3a22 7622 2c22 7479 7065 223a  ame":"v","type":
-00010070: 2275 696e 7438 227d 2c7b 2269 6e74 6572  "uint8"},{"inter
-00010080: 6e61 6c54 7970 6522 3a22 6279 7465 7333  nalType":"bytes3
-00010090: 3222 2c22 6e61 6d65 223a 2272 222c 2274  2","name":"r","t
-000100a0: 7970 6522 3a22 6279 7465 7333 3222 7d2c  ype":"bytes32"},
-000100b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000100c0: 2262 7974 6573 3332 222c 226e 616d 6522  "bytes32","name"
-000100d0: 3a22 7322 2c22 7479 7065 223a 2262 7974  :"s","type":"byt
-000100e0: 6573 3332 227d 5d2c 226e 616d 6522 3a22  es32"}],"name":"
-000100f0: 7365 6c66 5065 726d 6974 4966 4e65 6365  selfPermitIfNece
-00010100: 7373 6172 7922 2c22 6f75 7470 7574 7322  ssary","outputs"
-00010110: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
-00010120: 6c69 7479 223a 2270 6179 6162 6c65 222c  lity":"payable",
-00010130: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00010140: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00010150: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-00010160: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-00010170: 746f 6b65 6e22 2c22 7479 7065 223a 2261  token","type":"a
-00010180: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00010190: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-000101a0: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-000101b0: 744d 696e 696d 756d 222c 2274 7970 6522  tMinimum","type"
-000101c0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-000101d0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-000101e0: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
-000101f0: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-00010200: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
-00010210: 6522 3a22 7377 6565 7054 6f6b 656e 222c  e":"sweepToken",
-00010220: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-00010230: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00010240: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-00010250: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00010260: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00010270: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00010280: 2c22 6e61 6d65 223a 2274 6f6b 656e 222c  ,"name":"token",
-00010290: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-000102a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000102b0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-000102c0: 6522 3a22 616d 6f75 6e74 4d69 6e69 6d75  e":"amountMinimu
-000102d0: 6d22 2c22 7479 7065 223a 2275 696e 7432  m","type":"uint2
-000102e0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-000102f0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-00010300: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
-00010310: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00010320: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00010330: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00010340: 616d 6522 3a22 6665 6542 6970 7322 2c22  ame":"feeBips","
-00010350: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00010360: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00010370: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-00010380: 223a 2266 6565 5265 6369 7069 656e 7422  ":"feeRecipient"
-00010390: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-000103a0: 227d 5d2c 226e 616d 6522 3a22 7377 6565  "}],"name":"swee
-000103b0: 7054 6f6b 656e 5769 7468 4665 6522 2c22  pTokenWithFee","
-000103c0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-000103d0: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
-000103e0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-000103f0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00010400: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00010410: 5479 7065 223a 2269 6e74 3235 3622 2c22  Type":"int256","
-00010420: 6e61 6d65 223a 2261 6d6f 756e 7430 4465  name":"amount0De
-00010430: 6c74 6122 2c22 7479 7065 223a 2269 6e74  lta","type":"int
-00010440: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00010450: 5479 7065 223a 2269 6e74 3235 3622 2c22  Type":"int256","
-00010460: 6e61 6d65 223a 2261 6d6f 756e 7431 4465  name":"amount1De
-00010470: 6c74 6122 2c22 7479 7065 223a 2269 6e74  lta","type":"int
-00010480: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00010490: 5479 7065 223a 2262 7974 6573 222c 226e  Type":"bytes","n
-000104a0: 616d 6522 3a22 5f64 6174 6122 2c22 7479  ame":"_data","ty
-000104b0: 7065 223a 2262 7974 6573 227d 5d2c 226e  pe":"bytes"}],"n
-000104c0: 616d 6522 3a22 756e 6973 7761 7056 3353  ame":"uniswapV3S
-000104d0: 7761 7043 616c 6c62 6163 6b22 2c22 6f75  wapCallback","ou
-000104e0: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
-000104f0: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-00010500: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-00010510: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00010520: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00010530: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00010540: 2c22 6e61 6d65 223a 2261 6d6f 756e 744d  ,"name":"amountM
-00010550: 696e 696d 756d 222c 2274 7970 6522 3a22  inimum","type":"
-00010560: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00010570: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00010580: 7373 222c 226e 616d 6522 3a22 7265 6369  ss","name":"reci
-00010590: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
-000105a0: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
-000105b0: 3a22 756e 7772 6170 5745 5448 3922 2c22  :"unwrapWETH9","
-000105c0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-000105d0: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
-000105e0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-000105f0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00010600: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00010610: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00010620: 226e 616d 6522 3a22 616d 6f75 6e74 4d69  "name":"amountMi
-00010630: 6e69 6d75 6d22 2c22 7479 7065 223a 2275  nimum","type":"u
-00010640: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00010650: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00010660: 7322 2c22 6e61 6d65 223a 2272 6563 6970  s","name":"recip
-00010670: 6965 6e74 222c 2274 7970 6522 3a22 6164  ient","type":"ad
-00010680: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-00010690: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000106a0: 222c 226e 616d 6522 3a22 6665 6542 6970  ","name":"feeBip
-000106b0: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-000106c0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-000106d0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-000106e0: 6e61 6d65 223a 2266 6565 5265 6369 7069  name":"feeRecipi
-000106f0: 656e 7422 2c22 7479 7065 223a 2261 6464  ent","type":"add
-00010700: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-00010710: 756e 7772 6170 5745 5448 3957 6974 6846  unwrapWETH9WithF
-00010720: 6565 222c 226f 7574 7075 7473 223a 5b5d  ee","outputs":[]
-00010730: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00010740: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
-00010750: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00010760: 7b22 7374 6174 654d 7574 6162 696c 6974  {"stateMutabilit
-00010770: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
-00010780: 7065 223a 2272 6563 6569 7665 227d 5d27  pe":"receive"}]'
-00010790: 0a0a 2020 2020 2727 270a 2020 2020 2020  ..    '''.      
-000107a0: 2020 7573 6564 2066 6f72 2075 6e69 7377    used for unisw
-000107b0: 6170 2076 3320 6261 7365 6420 6465 780a  ap v3 based dex.
-000107c0: 2020 2020 2727 270a 2020 2020 6465 6620      '''.    def 
-000107d0: 5f5f 696e 6974 5f5f 2873 656c 662c 5f77  __init__(self,_w
-000107e0: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
-000107f0: 7265 7373 2c5f 726f 7574 655f 6164 6472  ress,_route_addr
-00010800: 6573 732c 5f70 7562 6c69 635f 6b65 792c  ess,_public_key,
-00010810: 5f70 7269 7661 7465 5f6b 6579 293a 0a20  _private_key):. 
-00010820: 2020 2020 2020 2073 656c 662e 6d79 5f70         self.my_p
-00010830: 7562 6c69 635f 6b65 793d 5f70 7562 6c69  ublic_key=_publi
-00010840: 635f 6b65 790a 2020 2020 2020 2020 7365  c_key.        se
-00010850: 6c66 2e6d 795f 7072 6976 6174 655f 6b65  lf.my_private_ke
-00010860: 793d 5f70 7269 7661 7465 5f6b 6579 0a20  y=_private_key. 
-00010870: 2020 2020 2020 2073 656c 662e 6661 6374         self.fact
-00010880: 6f72 795f 6164 6472 6573 733d 5f66 6163  ory_address=_fac
-00010890: 746f 7279 5f61 6464 7265 7373 0a20 2020  tory_address.   
-000108a0: 2020 2020 2073 656c 662e 726f 7574 655f       self.route_
-000108b0: 6164 6472 6573 733d 5f72 6f75 7465 5f61  address=_route_a
-000108c0: 6464 7265 7373 0a20 2020 2020 2020 2073  ddress.        s
-000108d0: 656c 662e 7765 6233 203d 205f 7765 6233  elf.web3 = _web3
-000108e0: 0a20 2020 2020 2020 2073 656c 662e 7765  .        self.we
-000108f0: 6233 2e6d 6964 646c 6577 6172 655f 6f6e  b3.middleware_on
-00010900: 696f 6e2e 696e 6a65 6374 2867 6574 685f  ion.inject(geth_
-00010910: 706f 615f 6d69 6464 6c65 7761 7265 2c20  poa_middleware, 
-00010920: 6c61 7965 723d 3029 0a20 2020 2020 2020  layer=0).       
-00010930: 2070 7269 6e74 2827 2323 2323 2323 2323   print('########
-00010940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010950: 2323 2323 2729 0a20 2020 2020 2020 2070  ####').        p
-00010960: 7269 6e74 2822 636f 6e74 7261 6374 2063  rint("contract c
-00010970: 6f6e 6e65 6374 696f 6e20 6973 2022 2b73  onnection is "+s
-00010980: 7472 2873 656c 662e 7765 6233 2e69 7343  tr(self.web3.isC
-00010990: 6f6e 6e65 6374 6564 2829 2929 0a20 2020  onnected())).   
-000109a0: 2020 2020 2069 6620 7365 6c66 2e77 6562       if self.web
-000109b0: 332e 6973 436f 6e6e 6563 7465 6428 293a  3.isConnected():
-000109c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000109d0: 662e 6e6f 6e63 653d 7365 6c66 2e77 6562  f.nonce=self.web
-000109e0: 332e 6574 682e 6765 745f 7472 616e 7361  3.eth.get_transa
-000109f0: 6374 696f 6e5f 636f 756e 7428 7365 6c66  ction_count(self
-00010a00: 2e6d 795f 7075 626c 6963 5f6b 6579 290a  .my_public_key).
-00010a10: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010a20: 7428 226e 6f6e 6365 203d 2022 2c73 656c  t("nonce = ",sel
-00010a30: 662e 6e6f 6e63 6529 0a20 2020 2020 2020  f.nonce).       
-00010a40: 2070 7269 6e74 2827 2323 2323 2323 2323   print('########
-00010a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010a60: 2323 2323 2729 0a20 2020 2020 2020 2023  ####').        #
-00010a70: 2075 6e69 7377 6170 5f46 6163 746f 7279   uniswap_Factory
-00010a80: 0a20 2020 2020 2020 2073 656c 662e 6661  .        self.fa
-00010a90: 6374 6f72 795f 6162 6920 3d20 6a73 6f6e  ctory_abi = json
-00010aa0: 2e6c 6f61 6473 2873 656c 662e 756e 6973  .loads(self.unis
-00010ab0: 7761 705f 7633 5f66 6163 746f 7279 5f61  wap_v3_factory_a
-00010ac0: 6269 290a 2020 2020 2020 2020 7365 6c66  bi).        self
-00010ad0: 2e70 6169 725f 6162 693d 6a73 6f6e 2e6c  .pair_abi=json.l
-00010ae0: 6f61 6473 2873 656c 662e 756e 6973 7761  oads(self.uniswa
-00010af0: 705f 7633 5f70 6169 725f 6162 6929 0a20  p_v3_pair_abi). 
-00010b00: 2020 2020 2020 2073 656c 662e 6572 6332         self.erc2
-00010b10: 305f 6162 693d 6a73 6f6e 2e6c 6f61 6473  0_abi=json.loads
-00010b20: 2873 656c 662e 756e 6973 7761 705f 7633  (self.uniswap_v3
-00010b30: 5f65 7263 3230 5f61 6269 290a 2020 2020  _erc20_abi).    
-00010b40: 2020 2020 7365 6c66 2e72 6f75 7465 5f61      self.route_a
-00010b50: 6269 3d6a 736f 6e2e 6c6f 6164 7328 7365  bi=json.loads(se
-00010b60: 6c66 2e75 6e69 7377 6170 5f76 335f 726f  lf.uniswap_v3_ro
-00010b70: 7574 655f 6162 6929 0a0a 2020 2020 2020  ute_abi)..      
-00010b80: 2020 7365 6c66 2e66 6163 746f 7279 5f63    self.factory_c
-00010b90: 6f6e 7472 6163 7420 3d20 7365 6c66 2e77  ontract = self.w
-00010ba0: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
-00010bb0: 2861 6464 7265 7373 3d73 656c 662e 6661  (address=self.fa
-00010bc0: 6374 6f72 795f 6164 6472 6573 732c 2061  ctory_address, a
-00010bd0: 6269 3d73 656c 662e 6661 6374 6f72 795f  bi=self.factory_
-00010be0: 6162 6929 0a20 2020 2020 2020 2073 656c  abi).        sel
-00010bf0: 662e 726f 7574 655f 636f 6e74 7261 6374  f.route_contract
-00010c00: 3d73 656c 662e 7765 6233 2e65 7468 2e63  =self.web3.eth.c
-00010c10: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
-00010c20: 7365 6c66 2e72 6f75 7465 5f61 6464 7265  self.route_addre
-00010c30: 7373 2c61 6269 3d73 656c 662e 726f 7574  ss,abi=self.rout
-00010c40: 655f 6162 6929 0a63 6c61 7373 2055 6e69  e_abi).class Uni
-00010c50: 7377 6170 5633 4661 6374 6f72 793a 0a0a  swapV3Factory:..
-00010c60: 2020 2020 2366 6163 746f 7279 0a20 2020      #factory.   
-00010c70: 2023 7265 7475 726e 2061 6464 7265 7373   #return address
-00010c80: 206f 6620 706f 6f6c 2066 6f72 2074 6f6b   of pool for tok
-00010c90: 656e 4120 616e 6420 746f 6b65 6e42 2077  enA and tokenB w
-00010ca0: 6974 6820 7370 6563 6966 6963 2066 6565  ith specific fee
-00010cb0: 0a20 2020 2023 3130 3030 3020 666f 7220  .    #10000 for 
-00010cc0: 3125 2066 6565 2c20 3330 3030 2066 6f72  1% fee, 3000 for
-00010cd0: 2030 2e33 252c 2061 6e64 2035 3030 2066   0.3%, and 500 f
-00010ce0: 6f72 2030 2e30 3525 0a20 2020 2064 6566  or 0.05%.    def
-00010cf0: 2067 6574 506f 6f6c 285f 7765 6233 3a57   getPool(_web3:W
-00010d00: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
-00010d10: 7265 7373 2c5f 6162 692c 5f74 6f6b 656e  ress,_abi,_token
-00010d20: 413a 7374 722c 5f74 6f6b 656e 423a 7374  A:str,_tokenB:st
-00010d30: 722c 5f66 6565 3a69 6e74 293a 0a20 2020  r,_fee:int):.   
-00010d40: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-00010d50: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-00010d60: 6464 7265 7373 3d5f 6661 6374 6f72 795f  ddress=_factory_
-00010d70: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
-00010d80: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
-00010d90: 506f 6f6c 285f 746f 6b65 6e41 2c5f 746f  Pool(_tokenA,_to
-00010da0: 6b65 6e42 2c5f 6665 6529 2e63 616c 6c28  kenB,_fee).call(
-00010db0: 290a 2020 2020 0a63 6c61 7373 2055 6e69  ).    .class Uni
-00010dc0: 7377 6170 5633 5175 6f74 6572 3a0a 2020  swapV3Quoter:.  
-00010dd0: 2020 2372 6574 7572 6e20 6164 6472 6573    #return addres
-00010de0: 7320 6f66 2070 6f6f 6c20 666f 7220 746f  s of pool for to
-00010df0: 6b65 6e41 2061 6e64 2074 6f6b 656e 4220  kenA and tokenB 
-00010e00: 7769 7468 2073 7065 6369 6669 6320 6665  with specific fe
-00010e10: 650a 2020 2020 2331 3030 3030 2066 6f72  e.    #10000 for
-00010e20: 2031 2520 6665 652c 2033 3030 3020 666f   1% fee, 3000 fo
-00010e30: 7220 302e 3325 2c20 616e 6420 3530 3020  r 0.3%, and 500 
-00010e40: 666f 7220 302e 3035 250a 2020 2020 6465  for 0.05%.    de
-00010e50: 6620 6765 7450 6f6f 6c28 5f77 6562 333a  f getPool(_web3:
-00010e60: 5765 6233 2c5f 7175 6f74 6572 5f61 6464  Web3,_quoter_add
-00010e70: 7265 7373 2c5f 6162 692c 5f74 6f6b 656e  ress,_abi,_token
-00010e80: 413a 7374 722c 5f74 6f6b 656e 423a 7374  A:str,_tokenB:st
-00010e90: 722c 5f66 6565 3a69 6e74 293a 0a20 2020  r,_fee:int):.   
-00010ea0: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-00010eb0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-00010ec0: 6464 7265 7373 3d5f 7175 6f74 6572 5f61  ddress=_quoter_a
-00010ed0: 6464 7265 7373 2c20 6162 693d 5f61 6269  ddress, abi=_abi
-00010ee0: 292e 6675 6e63 7469 6f6e 732e 6765 7450  ).functions.getP
-00010ef0: 6f6f 6c28 5f74 6f6b 656e 412c 5f74 6f6b  ool(_tokenA,_tok
-00010f00: 656e 422c 5f66 6565 292e 6361 6c6c 2829  enB,_fee).call()
-00010f10: 0a20 2020 200a 2020 2020 2320 7374 7275  .    .    # stru
-00010f20: 6374 2051 756f 7465 4578 6163 7449 6e70  ct QuoteExactInp
-00010f30: 7574 5369 6e67 6c65 5061 7261 6d73 207b  utSingleParams {
-00010f40: 0a20 2020 2023 2020 2020 2061 6464 7265  .    #     addre
-00010f50: 7373 2074 6f6b 656e 496e 3b0a 2020 2020  ss tokenIn;.    
-00010f60: 2320 2020 2020 6164 6472 6573 7320 746f  #     address to
-00010f70: 6b65 6e4f 7574 3b0a 2020 2020 2320 2020  kenOut;.    #   
-00010f80: 2020 7569 6e74 3235 3620 616d 6f75 6e74    uint256 amount
-00010f90: 496e 3b0a 2020 2020 2320 2020 2020 7569  In;.    #     ui
-00010fa0: 6e74 3234 2066 6565 3b0a 2020 2020 2320  nt24 fee;.    # 
-00010fb0: 2020 2020 7569 6e74 3136 3020 7371 7274      uint160 sqrt
-00010fc0: 5072 6963 654c 696d 6974 5839 363b 0a20  PriceLimitX96;. 
-00010fd0: 2020 2023 207d 0a20 2020 2064 6566 2071     # }.    def q
-00010fe0: 756f 7465 4578 6163 7449 6e70 7574 5369  uoteExactInputSi
-00010ff0: 6e67 6c65 285f 7765 6233 3a57 6562 332c  ngle(_web3:Web3,
-00011000: 5f71 756f 7465 725f 6164 6472 6573 732c  _quoter_address,
-00011010: 5f61 6269 2c5f 7061 7261 6d29 3a0a 2020  _abi,_param):.  
-00011020: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00011030: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-00011040: 6164 6472 6573 733d 5f71 756f 7465 725f  address=_quoter_
-00011050: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
-00011060: 6929 2e66 756e 6374 696f 6e73 2e71 756f  i).functions.quo
-00011070: 7465 4578 6163 7449 6e70 7574 5369 6e67  teExactInputSing
-00011080: 6c65 285f 7061 7261 6d29 2e63 616c 6c28  le(_param).call(
-00011090: 290a 0a20 2020 2023 7061 7468 2073 7461  )..    #path sta
-000110a0: 7274 7769 7468 2069 6e70 7574 2074 6f6b  rtwith input tok
-000110b0: 656e 0a20 2020 2064 6566 2071 756f 7465  en.    def quote
-000110c0: 4578 6163 7449 6e70 7574 285f 7765 6233  ExactInput(_web3
-000110d0: 3a57 6562 332c 5f71 756f 7465 725f 6164  :Web3,_quoter_ad
-000110e0: 6472 6573 732c 5f61 6269 2c70 6174 682c  dress,_abi,path,
-000110f0: 5f61 6d6f 756e 745f 696e 293a 0a20 2020  _amount_in):.   
-00011100: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-00011110: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-00011120: 6464 7265 7373 3d5f 7175 6f74 6572 5f61  ddress=_quoter_a
-00011130: 6464 7265 7373 2c20 6162 693d 5f61 6269  ddress, abi=_abi
-00011140: 292e 6675 6e63 7469 6f6e 732e 7175 6f74  ).functions.quot
-00011150: 6545 7861 6374 496e 7075 7428 7061 7468  eExactInput(path
-00011160: 2c5f 616d 6f75 6e74 5f69 6e29 2e63 616c  ,_amount_in).cal
-00011170: 6c28 290a 2020 2020 0a20 2020 2023 2073  l().    .    # s
-00011180: 7472 7563 7420 5175 6f74 6545 7861 6374  truct QuoteExact
-00011190: 4f75 7470 7574 5369 6e67 6c65 5061 7261  OutputSinglePara
-000111a0: 6d73 207b 0a20 2020 2023 2020 2020 2061  ms {.    #     a
-000111b0: 6464 7265 7373 2074 6f6b 656e 496e 3b0a  ddress tokenIn;.
-000111c0: 2020 2020 2320 2020 2020 6164 6472 6573      #     addres
-000111d0: 7320 746f 6b65 6e4f 7574 3b0a 2020 2020  s tokenOut;.    
-000111e0: 2320 2020 2020 7569 6e74 3235 3620 616d  #     uint256 am
-000111f0: 6f75 6e74 3b0a 2020 2020 2320 2020 2020  ount;.    #     
-00011200: 7569 6e74 3234 2066 6565 3b0a 2020 2020  uint24 fee;.    
-00011210: 2320 2020 2020 7569 6e74 3136 3020 7371  #     uint160 sq
-00011220: 7274 5072 6963 654c 696d 6974 5839 363b  rtPriceLimitX96;
-00011230: 0a20 2020 2023 207d 0a20 2020 2064 6566  .    # }.    def
-00011240: 2071 756f 7465 4578 6163 744f 7574 7075   quoteExactOutpu
-00011250: 7453 696e 676c 6528 5f77 6562 333a 5765  tSingle(_web3:We
-00011260: 6233 2c5f 7175 6f74 6572 5f61 6464 7265  b3,_quoter_addre
-00011270: 7373 2c5f 6162 692c 5f70 6172 616d 293a  ss,_abi,_param):
-00011280: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011290: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
-000112a0: 6374 2861 6464 7265 7373 3d5f 7175 6f74  ct(address=_quot
-000112b0: 6572 5f61 6464 7265 7373 2c20 6162 693d  er_address, abi=
-000112c0: 5f61 6269 292e 6675 6e63 7469 6f6e 732e  _abi).functions.
-000112d0: 7175 6f74 6545 7861 6374 4f75 7470 7574  quoteExactOutput
-000112e0: 5369 6e67 6c65 285f 7061 7261 6d29 2e63  Single(_param).c
-000112f0: 616c 6c28 290a 2020 2020 0a20 2020 2023  all().    .    #
-00011300: 7061 7468 2073 7461 7274 2077 6974 6820  path start with 
-00011310: 6f75 7470 7574 2074 6f6b 656e 0a20 2020  output token.   
-00011320: 2064 6566 2071 756f 7465 4578 6163 744f   def quoteExactO
-00011330: 7574 7075 7428 5f77 6562 333a 5765 6233  utput(_web3:Web3
-00011340: 2c5f 7175 6f74 6572 5f61 6464 7265 7373  ,_quoter_address
-00011350: 2c5f 6162 692c 7061 7468 2c5f 616d 6f75  ,_abi,path,_amou
-00011360: 6e74 5f6f 7574 293a 0a20 2020 2020 2020  nt_out):.       
-00011370: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
-00011380: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
-00011390: 7373 3d5f 7175 6f74 6572 5f61 6464 7265  ss=_quoter_addre
-000113a0: 7373 2c20 6162 693d 5f61 6269 292e 6675  ss, abi=_abi).fu
-000113b0: 6e63 7469 6f6e 732e 7175 6f74 6545 7861  nctions.quoteExa
-000113c0: 6374 4f75 7470 7574 2870 6174 682c 5f61  ctOutput(path,_a
-000113d0: 6d6f 756e 745f 6f75 7429 2e63 616c 6c28  mount_out).call(
-000113e0: 290a 0a63 6c61 7373 2055 6e69 7377 6170  )..class Uniswap
-000113f0: 5633 526f 7574 6572 3a0a 0a20 2020 2023  V3Router:..    #
-00011400: 2073 7472 7563 7420 4578 6163 7449 6e70   struct ExactInp
-00011410: 7574 5369 6e67 6c65 5061 7261 6d73 207b  utSingleParams {
-00011420: 0a20 2020 2023 2020 2020 2061 6464 7265  .    #     addre
-00011430: 7373 2074 6f6b 656e 496e 3b0a 2020 2020  ss tokenIn;.    
-00011440: 2320 2020 2020 6164 6472 6573 7320 746f  #     address to
-00011450: 6b65 6e4f 7574 3b0a 2020 2020 2320 2020  kenOut;.    #   
-00011460: 2020 7569 6e74 3234 2066 6565 3b0a 2020    uint24 fee;.  
-00011470: 2020 2320 2020 2020 6164 6472 6573 7320    #     address 
-00011480: 7265 6369 7069 656e 743b 0a20 2020 2023  recipient;.    #
-00011490: 2020 2020 2075 696e 7432 3536 2064 6561       uint256 dea
-000114a0: 646c 696e 653b 0a20 2020 2023 2020 2020  dline;.    #    
-000114b0: 2075 696e 7432 3536 2061 6d6f 756e 7449   uint256 amountI
-000114c0: 6e3b 0a20 2020 2023 2020 2020 2075 696e  n;.    #     uin
-000114d0: 7432 3536 2061 6d6f 756e 744f 7574 4d69  t256 amountOutMi
-000114e0: 6e69 6d75 6d3b 0a20 2020 2023 2020 2020  nimum;.    #    
-000114f0: 2075 696e 7431 3630 2073 7172 7450 7269   uint160 sqrtPri
-00011500: 6365 4c69 6d69 7458 3936 3b0a 2020 2020  ceLimitX96;.    
-00011510: 2320 7d0a 2020 2020 6465 6620 6578 6163  # }.    def exac
-00011520: 7449 6e70 7574 5369 6e67 6c65 285f 7765  tInputSingle(_we
-00011530: 6233 3a57 6562 332c 5f72 6f75 7465 5f61  b3:Web3,_route_a
-00011540: 6464 7265 7373 2c5f 6162 692c 5f6e 6f6e  ddress,_abi,_non
-00011550: 6365 2c5f 7075 626c 6963 5f6b 6579 2c5f  ce,_public_key,_
-00011560: 7072 6976 6174 655f 6b65 792c 0a20 2020  private_key,.   
-00011570: 2020 2020 205f 746f 6b65 6e5f 696e 2c5f       _token_in,_
-00011580: 746f 6b65 6e5f 6f75 742c 5f66 6565 2c5f  token_out,_fee,_
-00011590: 7265 6369 7069 656e 742c 5f64 6561 646c  recipient,_deadl
-000115a0: 696e 652c 5f61 6d6f 756e 745f 696e 2c5f  ine,_amount_in,_
-000115b0: 616d 6f75 6e74 5f6f 7574 5f6d 696e 2c5f  amount_out_min,_
-000115c0: 7371 7274 5f70 7269 6365 5f6c 696d 6974  sqrt_price_limit
-000115d0: 293a 0a20 2020 2020 2020 2072 6f75 7465  ):.        route
-000115e0: 5f63 6f6e 7472 6163 743d 5f77 6562 332e  _contract=_web3.
-000115f0: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-00011600: 7265 7373 3d5f 726f 7574 655f 6164 6472  ress=_route_addr
-00011610: 6573 732c 2061 6269 3d5f 6162 6929 0a20  ess, abi=_abi). 
-00011620: 2020 2020 2020 2066 756e 6374 696f 6e5f         function_
-00011630: 7061 7261 6d73 3d7b 0a20 2020 2020 2020  params={.       
-00011640: 2020 2020 2027 746f 6b65 6e49 6e27 3a5f       'tokenIn':_
-00011650: 746f 6b65 6e5f 696e 2c0a 2020 2020 2020  token_in,.      
-00011660: 2020 2020 2020 2774 6f6b 656e 4f75 7427        'tokenOut'
-00011670: 3a5f 746f 6b65 6e5f 6f75 742c 0a20 2020  :_token_out,.   
-00011680: 2020 2020 2020 2020 2027 6665 6527 3a5f           'fee':_
-00011690: 6665 652c 0a20 2020 2020 2020 2020 2020  fee,.           
-000116a0: 2027 7265 6369 7069 656e 7427 3a5f 7265   'recipient':_re
-000116b0: 6369 7069 656e 742c 0a20 2020 2020 2020  cipient,.       
-000116c0: 2020 2020 2027 6465 6164 6c69 6e65 273a       'deadline':
-000116d0: 5f64 6561 646c 696e 652c 0a20 2020 2020  _deadline,.     
-000116e0: 2020 2020 2020 2027 616d 6f75 6e74 496e         'amountIn
-000116f0: 273a 5f61 6d6f 756e 745f 696e 2c0a 2020  ':_amount_in,.  
-00011700: 2020 2020 2020 2020 2020 2761 6d6f 756e            'amoun
-00011710: 744f 7574 4d69 6e69 6d75 6d27 3a5f 616d  tOutMinimum':_am
-00011720: 6f75 6e74 5f6f 7574 5f6d 696e 2c0a 2020  ount_out_min,.  
-00011730: 2020 2020 2020 2020 2020 2773 7172 7450            'sqrtP
-00011740: 7269 6365 4c69 6d69 7458 3936 273a 5f73  riceLimitX96':_s
-00011750: 7172 745f 7072 6963 655f 6c69 6d69 740a  qrt_price_limit.
-00011760: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00011770: 2020 2320 6675 6e63 7469 6f6e 5f70 6172    # function_par
-00011780: 616d 733d 285f 746f 6b65 6e5f 696e 2c5f  ams=(_token_in,_
-00011790: 746f 6b65 6e5f 6f75 742c 5f66 6565 2c5f  token_out,_fee,_
-000117a0: 7265 6369 7069 656e 742c 5f64 6561 646c  recipient,_deadl
-000117b0: 696e 652c 5f61 6d6f 756e 745f 696e 2c5f  ine,_amount_in,_
-000117c0: 616d 6f75 6e74 5f6f 7574 5f6d 696e 2c5f  amount_out_min,_
-000117d0: 7371 7274 5f70 7269 6365 5f6c 696d 6974  sqrt_price_limit
-000117e0: 290a 2020 2020 2020 2020 7377 6170 5f66  ).        swap_f
-000117f0: 756e 6374 696f 6e3d 726f 7574 655f 636f  unction=route_co
-00011800: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
-00011810: 2e65 7861 6374 496e 7075 7453 696e 676c  .exactInputSingl
-00011820: 6528 6675 6e63 7469 6f6e 5f70 6172 616d  e(function_param
-00011830: 7329 0a20 2020 2020 2020 2074 785f 7061  s).        tx_pa
-00011840: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
-00011850: 2020 2027 6672 6f6d 273a 205f 7075 626c     'from': _publ
-00011860: 6963 5f6b 6579 2c0a 2020 2020 2020 2020  ic_key,.        
-00011870: 2020 2020 2776 616c 7565 273a 2030 2c0a      'value': 0,.
-00011880: 2020 2020 2020 2020 2020 2020 276e 6f6e              'non
-00011890: 6365 273a 205f 6e6f 6e63 652c 0a20 2020  ce': _nonce,.   
-000118a0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-000118b0: 2027 3078 3227 0a20 2020 2020 2020 207d   '0x2'.        }
-000118c0: 0a20 2020 2020 2020 2074 7261 6e73 6163  .        transac
-000118d0: 7469 6f6e 3d73 7761 705f 6675 6e63 7469  tion=swap_functi
-000118e0: 6f6e 2e62 7569 6c64 5472 616e 7361 6374  on.buildTransact
-000118f0: 696f 6e28 7478 5f70 6172 616d 7329 0a20  ion(tx_params). 
-00011900: 2020 2020 2020 2073 6967 6e65 645f 7472         signed_tr
-00011910: 616e 7361 6374 696f 6e3d 5f77 6562 332e  ansaction=_web3.
-00011920: 6574 682e 6163 636f 756e 742e 7369 676e  eth.account.sign
-00011930: 5f74 7261 6e73 6163 7469 6f6e 2874 7261  _transaction(tra
-00011940: 6e73 6163 7469 6f6e 2c20 7072 6976 6174  nsaction, privat
-00011950: 655f 6b65 793d 5f70 7269 7661 7465 5f6b  e_key=_private_k
-00011960: 6579 290a 2020 2020 2020 2020 7265 7475  ey).        retu
-00011970: 726e 205f 7765 6233 2e74 6f48 6578 285f  rn _web3.toHex(_
-00011980: 7765 6233 2e65 7468 2e73 656e 645f 7261  web3.eth.send_ra
-00011990: 775f 7472 616e 7361 6374 696f 6e28 7369  w_transaction(si
-000119a0: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
-000119b0: 2e72 6177 5472 616e 7361 6374 696f 6e29  .rawTransaction)
-000119c0: 290a 0a20 2020 2023 2073 7472 7563 7420  )..    # struct 
-000119d0: 4578 6163 7449 6e70 7574 5061 7261 6d73  ExactInputParams
-000119e0: 207b 0a20 2020 2023 2020 2020 2062 7974   {.    #     byt
-000119f0: 6573 2070 6174 683b 0a20 2020 2023 2020  es path;.    #  
-00011a00: 2020 2061 6464 7265 7373 2072 6563 6970     address recip
-00011a10: 6965 6e74 3b0a 2020 2020 2320 2020 2020  ient;.    #     
-00011a20: 7569 6e74 3235 3620 6465 6164 6c69 6e65  uint256 deadline
-00011a30: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
-00011a40: 3235 3620 616d 6f75 6e74 496e 3b0a 2020  256 amountIn;.  
-00011a50: 2020 2320 2020 2020 7569 6e74 3235 3620    #     uint256 
-00011a60: 616d 6f75 6e74 4f75 744d 696e 696d 756d  amountOutMinimum
-00011a70: 3b0a 2020 2020 2320 7d0a 2020 2020 6465  ;.    # }.    de
-00011a80: 6620 6578 6163 7449 6e70 7574 285f 7765  f exactInput(_we
-00011a90: 6233 3a57 6562 332c 5f72 6f75 7465 5f61  b3:Web3,_route_a
-00011aa0: 6464 7265 7373 2c5f 6162 692c 5f6e 6f6e  ddress,_abi,_non
-00011ab0: 6365 2c5f 7075 626c 6963 5f6b 6579 2c5f  ce,_public_key,_
-00011ac0: 7072 6976 6174 655f 6b65 792c 0a20 2020  private_key,.   
-00011ad0: 2020 2020 205f 7061 7468 2c5f 7265 6369       _path,_reci
-00011ae0: 7069 656e 742c 5f64 6561 646c 696e 652c  pient,_deadline,
-00011af0: 5f61 6d6f 756e 7449 6e2c 5f61 6d6f 756e  _amountIn,_amoun
-00011b00: 744f 7574 4d69 6e29 3a0a 2020 2020 2020  tOutMin):.      
-00011b10: 2020 726f 7574 655f 636f 6e74 7261 6374    route_contract
-00011b20: 3d5f 7765 6233 2e65 7468 2e63 6f6e 7472  =_web3.eth.contr
-00011b30: 6163 7428 6164 6472 6573 733d 5f72 6f75  act(address=_rou
-00011b40: 7465 5f61 6464 7265 7373 2c20 6162 693d  te_address, abi=
-00011b50: 5f61 6269 290a 0a20 2020 2020 2020 2023  _abi)..        #
-00011b60: 2074 7970 653d 5b27 6279 7465 7327 2c27   type=['bytes','
-00011b70: 6164 6472 6573 7327 2c27 7569 6e74 3235  address','uint25
-00011b80: 3627 2c27 7569 6e74 3235 3627 2c27 7569  6','uint256','ui
-00011b90: 6e74 3235 3627 5d0a 2020 2020 2020 2020  nt256'].        
-00011ba0: 2320 6461 7461 3d5b 5f70 6174 682c 5f72  # data=[_path,_r
-00011bb0: 6563 6970 6965 6e74 2c5f 6465 6164 6c69  ecipient,_deadli
-00011bc0: 6e65 2c5f 616d 6f75 6e74 496e 2c5f 616d  ne,_amountIn,_am
-00011bd0: 6f75 6e74 4f75 744d 696e 5d0a 2020 2020  ountOutMin].    
-00011be0: 2020 2020 2320 6675 6e63 7469 6f6e 5f70      # function_p
-00011bf0: 6172 616d 733d 656e 636f 6465 5f61 6269  arams=encode_abi
-00011c00: 2874 7970 652c 6461 7461 290a 2020 2020  (type,data).    
-00011c10: 2020 2020 6675 6e63 7469 6f6e 5f70 6172      function_par
-00011c20: 616d 733d 7b0a 2020 2020 2020 2020 2020  ams={.          
-00011c30: 2020 2770 6174 6827 3a5f 7061 7468 2c0a    'path':_path,.
-00011c40: 2020 2020 2020 2020 2020 2020 2772 6563              'rec
-00011c50: 6970 6965 6e74 273a 5f72 6563 6970 6965  ipient':_recipie
-00011c60: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00011c70: 2764 6561 646c 696e 6527 3a5f 6465 6164  'deadline':_dead
-00011c80: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
-00011c90: 2020 2761 6d6f 756e 7449 6e27 3a5f 616d    'amountIn':_am
-00011ca0: 6f75 6e74 496e 2c0a 2020 2020 2020 2020  ountIn,.        
-00011cb0: 2020 2020 2761 6d6f 756e 744f 7574 4d69      'amountOutMi
-00011cc0: 6e69 6d75 6d27 3a5f 616d 6f75 6e74 4f75  nimum':_amountOu
-00011cd0: 744d 696e 0a20 2020 2020 2020 207d 0a20  tMin.        }. 
-00011ce0: 2020 2020 2020 2023 2066 756e 6374 696f         # functio
-00011cf0: 6e5f 7061 7261 6d73 3d28 5f70 6174 682c  n_params=(_path,
-00011d00: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
-00011d10: 6c69 6e65 2c5f 616d 6f75 6e74 496e 2c5f  line,_amountIn,_
-00011d20: 616d 6f75 6e74 4f75 744d 696e 290a 2020  amountOutMin).  
-00011d30: 2020 2020 2020 7377 6170 5f66 756e 6374        swap_funct
-00011d40: 696f 6e3d 726f 7574 655f 636f 6e74 7261  ion=route_contra
-00011d50: 6374 2e66 756e 6374 696f 6e73 2e65 7861  ct.functions.exa
-00011d60: 6374 496e 7075 7428 6675 6e63 7469 6f6e  ctInput(function
-00011d70: 5f70 6172 616d 7329 0a20 2020 2020 2020  _params).       
-00011d80: 2074 785f 7061 7261 6d73 3d7b 0a20 2020   tx_params={.   
-00011d90: 2020 2020 2020 2020 2027 6672 6f6d 273a           'from':
-00011da0: 205f 7075 626c 6963 5f6b 6579 2c0a 2020   _public_key,.  
-00011db0: 2020 2020 2020 2020 2020 2776 616c 7565            'value
-00011dc0: 273a 2030 2c0a 2020 2020 2020 2020 2020  ': 0,.          
-00011dd0: 2020 276e 6f6e 6365 273a 205f 6e6f 6e63    'nonce': _nonc
-00011de0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-00011df0: 7479 7065 273a 2027 3078 3227 2c0a 2020  type': '0x2',.  
-00011e00: 2020 2020 2020 2020 2020 2320 2767 6173            # 'gas
-00011e10: 273a 5f67 6173 0a20 2020 2020 2020 207d  ':_gas.        }
-00011e20: 0a20 2020 2020 2020 2074 7261 6e73 6163  .        transac
-00011e30: 7469 6f6e 3d73 7761 705f 6675 6e63 7469  tion=swap_functi
-00011e40: 6f6e 2e62 7569 6c64 5472 616e 7361 6374  on.buildTransact
-00011e50: 696f 6e28 7478 5f70 6172 616d 7329 0a20  ion(tx_params). 
-00011e60: 2020 2020 2020 2073 6967 6e65 645f 7472         signed_tr
-00011e70: 616e 7361 6374 696f 6e3d 5f77 6562 332e  ansaction=_web3.
-00011e80: 6574 682e 6163 636f 756e 742e 7369 676e  eth.account.sign
-00011e90: 5f74 7261 6e73 6163 7469 6f6e 2874 7261  _transaction(tra
-00011ea0: 6e73 6163 7469 6f6e 2c20 7072 6976 6174  nsaction, privat
-00011eb0: 655f 6b65 793d 5f70 7269 7661 7465 5f6b  e_key=_private_k
-00011ec0: 6579 290a 2020 2020 2020 2020 7265 7475  ey).        retu
-00011ed0: 726e 205f 7765 6233 2e74 6f48 6578 285f  rn _web3.toHex(_
-00011ee0: 7765 6233 2e65 7468 2e73 656e 645f 7261  web3.eth.send_ra
-00011ef0: 775f 7472 616e 7361 6374 696f 6e28 7369  w_transaction(si
-00011f00: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
-00011f10: 2e72 6177 5472 616e 7361 6374 696f 6e29  .rawTransaction)
-00011f20: 290a 0a20 2020 2023 2073 7472 7563 7420  )..    # struct 
-00011f30: 4578 6163 744f 7574 7075 7453 696e 676c  ExactOutputSingl
-00011f40: 6550 6172 616d 7320 7b0a 2020 2020 2320  eParams {.    # 
-00011f50: 2020 2020 6164 6472 6573 7320 746f 6b65      address toke
-00011f60: 6e49 6e3b 0a20 2020 2023 2020 2020 2061  nIn;.    #     a
-00011f70: 6464 7265 7373 2074 6f6b 656e 4f75 743b  ddress tokenOut;
-00011f80: 0a20 2020 2023 2020 2020 2075 696e 7432  .    #     uint2
-00011f90: 3420 6665 653b 0a20 2020 2023 2020 2020  4 fee;.    #    
-00011fa0: 2061 6464 7265 7373 2072 6563 6970 6965   address recipie
-00011fb0: 6e74 3b0a 2020 2020 2320 2020 2020 7569  nt;.    #     ui
-00011fc0: 6e74 3235 3620 6465 6164 6c69 6e65 3b0a  nt256 deadline;.
-00011fd0: 2020 2020 2320 2020 2020 7569 6e74 3235      #     uint25
-00011fe0: 3620 616d 6f75 6e74 4f75 743b 0a20 2020  6 amountOut;.   
-00011ff0: 2023 2020 2020 2075 696e 7432 3536 2061   #     uint256 a
-00012000: 6d6f 756e 7449 6e4d 6178 696d 756d 3b0a  mountInMaximum;.
-00012010: 2020 2020 2320 2020 2020 7569 6e74 3136      #     uint16
-00012020: 3020 7371 7274 5072 6963 654c 696d 6974  0 sqrtPriceLimit
-00012030: 5839 363b 0a20 2020 2023 207d 0a20 2020  X96;.    # }.   
-00012040: 2064 6566 2065 7861 6374 4f75 7470 7574   def exactOutput
-00012050: 5369 6e67 6c65 285f 7765 6233 3a57 6562  Single(_web3:Web
-00012060: 332c 5f72 6f75 7465 5f61 6464 7265 7373  3,_route_address
-00012070: 2c5f 6162 692c 5f6e 6f6e 6365 2c5f 7075  ,_abi,_nonce,_pu
-00012080: 626c 6963 5f6b 6579 2c5f 7072 6976 6174  blic_key,_privat
-00012090: 655f 6b65 792c 0a20 2020 2020 2020 205f  e_key,.        _
-000120a0: 746f 6b65 6e5f 696e 2c5f 746f 6b65 6e5f  token_in,_token_
-000120b0: 6f75 742c 5f66 6565 2c5f 7265 6369 7069  out,_fee,_recipi
-000120c0: 656e 742c 5f64 6561 646c 696e 652c 5f61  ent,_deadline,_a
-000120d0: 6d6f 756e 745f 6f75 742c 5f61 6d6f 756e  mount_out,_amoun
-000120e0: 745f 696e 5f6d 6178 2c5f 7371 7274 5f70  t_in_max,_sqrt_p
-000120f0: 7269 6365 5f6c 696d 6974 293a 0a20 2020  rice_limit):.   
-00012100: 2020 2020 2072 6f75 7465 5f63 6f6e 7472       route_contr
-00012110: 6163 743d 5f77 6562 332e 6574 682e 636f  act=_web3.eth.co
-00012120: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
-00012130: 726f 7574 655f 6164 6472 6573 732c 2061  route_address, a
-00012140: 6269 3d5f 6162 6929 0a20 2020 2020 2020  bi=_abi).       
-00012150: 2066 756e 6374 696f 6e5f 7061 7261 6d3d   function_param=
-00012160: 7b0a 2020 2020 2020 2020 2020 2020 2774  {.            't
-00012170: 6f6b 656e 496e 273a 5f74 6f6b 656e 5f69  okenIn':_token_i
-00012180: 6e2c 0a20 2020 2020 2020 2020 2020 2027  n,.            '
-00012190: 746f 6b65 6e4f 7574 273a 5f74 6f6b 656e  tokenOut':_token
-000121a0: 5f6f 7574 2c0a 2020 2020 2020 2020 2020  _out,.          
-000121b0: 2020 2766 6565 273a 5f66 6565 2c0a 2020    'fee':_fee,.  
-000121c0: 2020 2020 2020 2020 2020 2772 6563 6970            'recip
-000121d0: 6965 6e74 273a 5f72 6563 6970 6965 6e74  ient':_recipient
-000121e0: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
-000121f0: 6561 646c 696e 6527 3a5f 6465 6164 6c69  eadline':_deadli
-00012200: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00012210: 2761 6d6f 756e 744f 7574 273a 5f61 6d6f  'amountOut':_amo
-00012220: 756e 745f 6f75 742c 0a20 2020 2020 2020  unt_out,.       
-00012230: 2020 2020 2027 616d 6f75 6e74 496e 4d61       'amountInMa
-00012240: 7869 6d75 6d27 3a5f 616d 6f75 6e74 5f69  ximum':_amount_i
-00012250: 6e5f 6d61 782c 0a20 2020 2020 2020 2020  n_max,.         
-00012260: 2020 2027 7371 7274 5072 6963 654c 696d     'sqrtPriceLim
-00012270: 6974 5839 3627 3a5f 7371 7274 5f70 7269  itX96':_sqrt_pri
-00012280: 6365 5f6c 696d 6974 0a20 2020 2020 2020  ce_limit.       
-00012290: 207d 0a20 2020 2020 2020 2073 7761 705f   }.        swap_
-000122a0: 6675 6e63 7469 6f6e 3d72 6f75 7465 5f63  function=route_c
-000122b0: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
-000122c0: 732e 6578 6163 744f 7574 7075 7453 696e  s.exactOutputSin
-000122d0: 676c 6528 6675 6e63 7469 6f6e 5f70 6172  gle(function_par
-000122e0: 616d 290a 2020 2020 2020 2020 7478 5f70  am).        tx_p
-000122f0: 6172 616d 733d 7b0a 2020 2020 2020 2020  arams={.        
-00012300: 2020 2020 2766 726f 6d27 3a20 5f70 7562      'from': _pub
-00012310: 6c69 635f 6b65 792c 0a20 2020 2020 2020  lic_key,.       
-00012320: 2020 2020 2027 7661 6c75 6527 3a20 302c       'value': 0,
-00012330: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
-00012340: 6e63 6527 3a20 5f6e 6f6e 6365 2c0a 2020  nce': _nonce,.  
-00012350: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-00012360: 3a20 2730 7832 270a 2020 2020 2020 2020  : '0x2'.        
-00012370: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
-00012380: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
-00012390: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
-000123a0: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
-000123b0: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
-000123c0: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
-000123d0: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
-000123e0: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
-000123f0: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
-00012400: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
-00012410: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
-00012420: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
-00012430: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
-00012440: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
-00012450: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
-00012460: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
-00012470: 2929 0a0a 0a20 2020 2023 2073 7472 7563  ))...    # struc
-00012480: 7420 4578 6163 744f 7574 7075 7450 6172  t ExactOutputPar
-00012490: 616d 7320 7b0a 2020 2020 2320 2020 2020  ams {.    #     
-000124a0: 6279 7465 7320 7061 7468 3b0a 2020 2020  bytes path;.    
-000124b0: 2320 2020 2020 6164 6472 6573 7320 7265  #     address re
-000124c0: 6369 7069 656e 743b 0a20 2020 2023 2020  cipient;.    #  
-000124d0: 2020 2075 696e 7432 3536 2064 6561 646c     uint256 deadl
-000124e0: 696e 653b 0a20 2020 2023 2020 2020 2075  ine;.    #     u
-000124f0: 696e 7432 3536 2061 6d6f 756e 744f 7574  int256 amountOut
-00012500: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
-00012510: 3235 3620 616d 6f75 6e74 496e 4d61 7869  256 amountInMaxi
-00012520: 6d75 6d3b 0a20 2020 2023 207d 0a20 2020  mum;.    # }.   
-00012530: 2064 6566 2065 7861 6374 4f75 7470 7574   def exactOutput
-00012540: 285f 7765 6233 3a57 6562 332c 5f72 6f75  (_web3:Web3,_rou
-00012550: 7465 5f61 6464 7265 7373 2c5f 6162 692c  te_address,_abi,
-00012560: 5f6e 6f6e 6365 2c5f 7075 626c 6963 5f6b  _nonce,_public_k
-00012570: 6579 2c5f 7072 6976 6174 655f 6b65 792c  ey,_private_key,
-00012580: 0a20 2020 2020 2020 205f 7061 7468 2c5f  .        _path,_
-00012590: 7265 6369 7069 656e 742c 5f64 6561 646c  recipient,_deadl
-000125a0: 696e 652c 5f61 6d6f 756e 745f 6f75 742c  ine,_amount_out,
-000125b0: 5f61 6d6f 756e 745f 696e 5f6d 6178 293a  _amount_in_max):
-000125c0: 0a20 2020 2020 2020 2072 6f75 7465 5f63  .        route_c
-000125d0: 6f6e 7472 6163 743d 5f77 6562 332e 6574  ontract=_web3.et
-000125e0: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
-000125f0: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
-00012600: 732c 2061 6269 3d5f 6162 6929 0a20 2020  s, abi=_abi).   
-00012610: 2020 2020 2066 756e 6374 696f 6e5f 7061       function_pa
-00012620: 7261 6d3d 7b0a 2020 2020 2020 2020 2020  ram={.          
-00012630: 2020 2770 6174 6827 3a5f 7061 7468 2c0a    'path':_path,.
-00012640: 2020 2020 2020 2020 2020 2020 2772 6563              'rec
-00012650: 6970 6965 6e74 273a 5f72 6563 6970 6965  ipient':_recipie
-00012660: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
-00012670: 2764 6561 646c 696e 6527 3a5f 6465 6164  'deadline':_dead
-00012680: 6c69 6e65 2c0a 2020 2020 2020 2020 2020  line,.          
-00012690: 2020 2761 6d6f 756e 744f 7574 273a 5f61    'amountOut':_a
-000126a0: 6d6f 756e 745f 6f75 742c 0a20 2020 2020  mount_out,.     
-000126b0: 2020 2020 2020 2027 616d 6f75 6e74 496e         'amountIn
-000126c0: 4d61 7869 6d75 6d27 3a5f 616d 6f75 6e74  Maximum':_amount
-000126d0: 5f69 6e5f 6d61 780a 2020 2020 2020 2020  _in_max.        
-000126e0: 7d0a 2020 2020 2020 2020 7377 6170 5f66  }.        swap_f
-000126f0: 756e 6374 696f 6e3d 726f 7574 655f 636f  unction=route_co
-00012700: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
-00012710: 2e65 7861 6374 4f75 7470 7574 2866 756e  .exactOutput(fun
-00012720: 6374 696f 6e5f 7061 7261 6d29 0a20 2020  ction_param).   
-00012730: 2020 2020 2074 785f 7061 7261 6d73 3d7b       tx_params={
-00012740: 0a20 2020 2020 2020 2020 2020 2027 6672  .            'fr
-00012750: 6f6d 273a 205f 7075 626c 6963 5f6b 6579  om': _public_key
-00012760: 2c0a 2020 2020 2020 2020 2020 2020 2776  ,.            'v
-00012770: 616c 7565 273a 2030 2c0a 2020 2020 2020  alue': 0,.      
-00012780: 2020 2020 2020 276e 6f6e 6365 273a 205f        'nonce': _
-00012790: 6e6f 6e63 652c 0a20 2020 2020 2020 2020  nonce,.         
-000127a0: 2020 2027 7479 7065 273a 2027 3078 3227     'type': '0x2'
-000127b0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-000127c0: 2020 2074 7261 6e73 6163 7469 6f6e 3d73     transaction=s
-000127d0: 7761 705f 6675 6e63 7469 6f6e 2e62 7569  wap_function.bui
-000127e0: 6c64 5472 616e 7361 6374 696f 6e28 7478  ldTransaction(tx
-000127f0: 5f70 6172 616d 7329 0a20 2020 2020 2020  _params).       
-00012800: 2073 6967 6e65 645f 7472 616e 7361 6374   signed_transact
-00012810: 696f 6e3d 5f77 6562 332e 6574 682e 6163  ion=_web3.eth.ac
-00012820: 636f 756e 742e 7369 676e 5f74 7261 6e73  count.sign_trans
-00012830: 6163 7469 6f6e 2874 7261 6e73 6163 7469  action(transacti
-00012840: 6f6e 2c20 7072 6976 6174 655f 6b65 793d  on, private_key=
-00012850: 5f70 7269 7661 7465 5f6b 6579 290a 2020  _private_key).  
-00012860: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00012870: 6233 2e74 6f48 6578 285f 7765 6233 2e65  b3.toHex(_web3.e
-00012880: 7468 2e73 656e 645f 7261 775f 7472 616e  th.send_raw_tran
-00012890: 7361 6374 696f 6e28 7369 676e 6564 5f74  saction(signed_t
-000128a0: 7261 6e73 6163 7469 6f6e 2e72 6177 5472  ransaction.rawTr
-000128b0: 616e 7361 6374 696f 6e29 290a 636c 6173  ansaction)).clas
-000128c0: 7320 4a6f 6556 3246 6163 746f 7279 3a0a  s JoeV2Factory:.
-000128d0: 2020 2020 6a6f 655f 6661 6374 6f72 795f      joe_factory_
-000128e0: 7632 5f61 6269 3d6a 736f 6e2e 6c6f 6164  v2_abi=json.load
-000128f0: 7328 275b 7b22 696e 7075 7473 223a 5b7b  s('[{"inputs":[{
-00012900: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00012910: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00012920: 225f 6665 6552 6563 6970 6965 6e74 222c  "_feeRecipient",
-00012930: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-00012940: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00012950: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00012960: 6522 3a22 5f66 6c61 7368 4c6f 616e 4665  e":"_flashLoanFe
-00012970: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
-00012980: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
-00012990: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
-000129a0: 626c 6522 2c22 7479 7065 223a 2263 6f6e  ble","type":"con
-000129b0: 7374 7275 6374 6f72 227d 2c7b 2269 6e70  structor"},{"inp
-000129c0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-000129d0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-000129e0: 226e 616d 6522 3a22 6270 222c 2274 7970  "name":"bp","typ
-000129f0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00012a00: 6e61 6d65 223a 2242 696e 4865 6c70 6572  name":"BinHelper
-00012a10: 5f5f 4269 6e53 7465 704f 7665 7266 6c6f  __BinStepOverflo
-00012a20: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
-00012a30: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-00012a40: 2c22 6e61 6d65 223a 2242 696e 4865 6c70  ,"name":"BinHelp
-00012a50: 6572 5f5f 4964 4f76 6572 666c 6f77 7322  er__IdOverflows"
-00012a60: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00012a70: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00012a80: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
-00012a90: 5f41 6464 7265 7373 5a65 726f 222c 2274  _AddressZero","t
-00012aa0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00012ab0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00012ac0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00012ad0: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
-00012ae0: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-00012af0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
-00012b00: 4246 6163 746f 7279 5f5f 4269 6e53 7465  BFactory__BinSte
-00012b10: 7048 6173 4e6f 5072 6573 6574 222c 2274  pHasNoPreset","t
-00012b20: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00012b30: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00012b40: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00012b50: 3622 2c22 6e61 6d65 223a 226c 6f77 6572  6","name":"lower
-00012b60: 426f 756e 6422 2c22 7479 7065 223a 2275  Bound","type":"u
-00012b70: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00012b80: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
-00012b90: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
-00012ba0: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
-00012bb0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00012bc0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00012bd0: 616d 6522 3a22 6869 6768 6572 426f 756e  ame":"higherBoun
-00012be0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00012bf0: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
-00012c00: 4661 6374 6f72 795f 5f42 696e 5374 6570  Factory__BinStep
-00012c10: 5265 7175 6972 656d 656e 7473 4272 6561  RequirementsBrea
-00012c20: 6368 6564 222c 2274 7970 6522 3a22 6572  ched","type":"er
-00012c30: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-00012c40: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00012c50: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00012c60: 3a22 6669 6c74 6572 5065 7269 6f64 222c  :"filterPeriod",
-00012c70: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-00012c80: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00012c90: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00012ca0: 3a22 6465 6361 7950 6572 696f 6422 2c22  :"decayPeriod","
-00012cb0: 7479 7065 223a 2275 696e 7431 3622 7d5d  type":"uint16"}]
-00012cc0: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
-00012cd0: 7279 5f5f 4465 6372 6561 7369 6e67 5065  ry__DecreasingPe
-00012ce0: 7269 6f64 7322 2c22 7479 7065 223a 2265  riods","type":"e
-00012cf0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00012d00: 3a5b 5d2c 226e 616d 6522 3a22 4c42 4661  :[],"name":"LBFa
-00012d10: 6374 6f72 795f 5f46 6163 746f 7279 4c6f  ctory__FactoryLo
-00012d20: 636b 4973 416c 7265 6164 7949 6e54 6865  ckIsAlreadyInThe
-00012d30: 5361 6d65 5374 6174 6522 2c22 7479 7065  SameState","type
-00012d40: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-00012d50: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00012d60: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00012d70: 226e 616d 6522 3a22 6665 6573 222c 2274  "name":"fees","t
-00012d80: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00012d90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00012da0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00012db0: 3a22 6d61 7846 6565 7322 2c22 7479 7065  :"maxFees","type
-00012dc0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00012dd0: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
-00012de0: 5f46 6565 7341 626f 7665 4d61 7822 2c22  _FeesAboveMax","
-00012df0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00012e00: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00012e10: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00012e20: 3536 222c 226e 616d 6522 3a22 6665 6573  56","name":"fees
-00012e30: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00012e40: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00012e50: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00012e60: 616d 6522 3a22 6d61 7846 6565 7322 2c22  ame":"maxFees","
-00012e70: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00012e80: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00012e90: 6f72 795f 5f46 6c61 7368 4c6f 616e 4665  ory__FlashLoanFe
-00012ea0: 6541 626f 7665 4d61 7822 2c22 7479 7065  eAboveMax","type
-00012eb0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-00012ec0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00012ed0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-00012ee0: 226e 616d 6522 3a22 7573 6572 222c 2274  "name":"user","t
-00012ef0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-00012f00: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
-00012f10: 7279 5f5f 4675 6e63 7469 6f6e 4973 4c6f  ry__FunctionIsLo
-00012f20: 636b 6564 466f 7255 7365 7273 222c 2274  ckedForUsers","t
-00012f30: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00012f40: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00012f50: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-00012f60: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
-00012f70: 223a 2274 6f6b 656e 222c 2274 7970 6522  ":"token","type"
-00012f80: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-00012f90: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
-00012fa0: 4964 656e 7469 6361 6c41 6464 7265 7373  IdenticalAddress
-00012fb0: 6573 222c 2274 7970 6522 3a22 6572 726f  es","type":"erro
-00012fc0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-00012fd0: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
-00012fe0: 7279 5f5f 496d 706c 656d 656e 7461 7469  ry__Implementati
-00012ff0: 6f6e 4e6f 7453 6574 222c 2274 7970 6522  onNotSet","type"
-00013000: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00013010: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00013020: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00013030: 4552 4332 3022 2c22 6e61 6d65 223a 2274  ERC20","name":"t
-00013040: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
-00013050: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00013060: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-00013070: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
-00013080: 223a 2274 6f6b 656e 5922 2c22 7479 7065  ":"tokenY","type
-00013090: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-000130a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000130b0: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-000130c0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-000130d0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-000130e0: 6522 3a22 4c42 4661 6374 6f72 795f 5f4c  e":"LBFactory__L
-000130f0: 4250 6169 7241 6c72 6561 6479 4578 6973  BPairAlreadyExis
-00013100: 7473 222c 2274 7970 6522 3a22 6572 726f  ts","type":"erro
-00013110: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-00013120: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
-00013130: 7279 5f5f 4c42 5061 6972 4967 6e6f 7265  ry__LBPairIgnore
-00013140: 6449 7341 6c72 6561 6479 496e 5468 6553  dIsAlreadyInTheS
-00013150: 616d 6553 7461 7465 222c 2274 7970 6522  ameState","type"
-00013160: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00013170: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00013180: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00013190: 4552 4332 3022 2c22 6e61 6d65 223a 2274  ERC20","name":"t
-000131a0: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
-000131b0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-000131c0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-000131d0: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
-000131e0: 223a 2274 6f6b 656e 5922 2c22 7479 7065  ":"tokenY","type
-000131f0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00013200: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00013210: 6e74 3235 3622 2c22 6e61 6d65 223a 2262  nt256","name":"b
-00013220: 696e 5374 6570 222c 2274 7970 6522 3a22  inStep","type":"
-00013230: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00013240: 223a 224c 4246 6163 746f 7279 5f5f 4c42  ":"LBFactory__LB
-00013250: 5061 6972 4e6f 7443 7265 6174 6564 222c  PairNotCreated",
-00013260: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-00013270: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-00013280: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00013290: 6573 7322 2c22 6e61 6d65 223a 224c 4250  ess","name":"LBP
-000132a0: 6169 7249 6d70 6c65 6d65 6e74 6174 696f  airImplementatio
-000132b0: 6e22 2c22 7479 7065 223a 2261 6464 7265  n","type":"addre
-000132c0: 7373 227d 5d2c 226e 616d 6522 3a22 4c42  ss"}],"name":"LB
-000132d0: 4661 6374 6f72 795f 5f4c 4250 6169 7253  Factory__LBPairS
-000132e0: 6166 6574 7943 6865 636b 4661 696c 6564  afetyCheckFailed
-000132f0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00013300: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00013310: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00013320: 6e74 3136 222c 226e 616d 6522 3a22 7072  nt16","name":"pr
-00013330: 6f74 6f63 6f6c 5368 6172 6522 2c22 7479  otocolShare","ty
-00013340: 7065 223a 2275 696e 7431 3622 7d2c 7b22  pe":"uint16"},{"
-00013350: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013360: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00013370: 6d61 7822 2c22 7479 7065 223a 2275 696e  max","type":"uin
-00013380: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00013390: 4c42 4661 6374 6f72 795f 5f50 726f 746f  LBFactory__Proto
-000133a0: 636f 6c53 6861 7265 4f76 6572 666c 6f77  colShareOverflow
-000133b0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-000133c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-000133d0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-000133e0: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
-000133f0: 226e 616d 6522 3a22 7175 6f74 6541 7373  "name":"quoteAss
-00013400: 6574 222c 2274 7970 6522 3a22 6164 6472  et","type":"addr
-00013410: 6573 7322 7d5d 2c22 6e61 6d65 223a 224c  ess"}],"name":"L
-00013420: 4246 6163 746f 7279 5f5f 5175 6f74 6541  BFactory__QuoteA
-00013430: 7373 6574 416c 7265 6164 7957 6869 7465  ssetAlreadyWhite
-00013440: 6c69 7374 6564 222c 2274 7970 6522 3a22  listed","type":"
-00013450: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00013460: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00013470: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-00013480: 4332 3022 2c22 6e61 6d65 223a 2271 756f  C20","name":"quo
-00013490: 7465 4173 7365 7422 2c22 7479 7065 223a  teAsset","type":
-000134a0: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
-000134b0: 6522 3a22 4c42 4661 6374 6f72 795f 5f51  e":"LBFactory__Q
-000134c0: 756f 7465 4173 7365 744e 6f74 5768 6974  uoteAssetNotWhit
-000134d0: 656c 6973 7465 6422 2c22 7479 7065 223a  elisted","type":
-000134e0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-000134f0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00013500: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
-00013510: 6d65 223a 2272 6564 7563 7469 6f6e 4661  me":"reductionFa
-00013520: 6374 6f72 222c 2274 7970 6522 3a22 7569  ctor","type":"ui
-00013530: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
-00013540: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00013550: 2c22 6e61 6d65 223a 226d 6178 222c 2274  ,"name":"max","t
-00013560: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00013570: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
-00013580: 7279 5f5f 5265 6475 6374 696f 6e46 6163  ry__ReductionFac
-00013590: 746f 724f 7665 7266 6c6f 7773 222c 2274  torOverflows","t
-000135a0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-000135b0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-000135c0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-000135d0: 7322 2c22 6e61 6d65 223a 2266 6565 5265  s","name":"feeRe
-000135e0: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-000135f0: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
-00013600: 6522 3a22 4c42 4661 6374 6f72 795f 5f53  e":"LBFactory__S
-00013610: 616d 6546 6565 5265 6369 7069 656e 7422  ameFeeRecipient"
-00013620: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00013630: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00013640: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00013650: 7432 3536 222c 226e 616d 6522 3a22 666c  t256","name":"fl
-00013660: 6173 684c 6f61 6e46 6565 222c 2274 7970  ashLoanFee","typ
-00013670: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00013680: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
-00013690: 5f5f 5361 6d65 466c 6173 684c 6f61 6e46  __SameFlashLoanF
-000136a0: 6565 222c 2274 7970 6522 3a22 6572 726f  ee","type":"erro
-000136b0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-000136c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000136d0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-000136e0: 224c 4250 6169 7249 6d70 6c65 6d65 6e74  "LBPairImplement
-000136f0: 6174 696f 6e22 2c22 7479 7065 223a 2261  ation","type":"a
-00013700: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
-00013710: 3a22 4c42 4661 6374 6f72 795f 5f53 616d  :"LBFactory__Sam
-00013720: 6549 6d70 6c65 6d65 6e74 6174 696f 6e22  eImplementation"
-00013730: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00013740: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00013750: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00013760: 7432 3536 222c 226e 616d 6522 3a22 7822  t256","name":"x"
-00013770: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00013780: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00013790: 6522 3a22 696e 7432 3536 222c 226e 616d  e":"int256","nam
-000137a0: 6522 3a22 7922 2c22 7479 7065 223a 2269  e":"y","type":"i
-000137b0: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-000137c0: 224d 6174 6831 3238 7831 3238 5f5f 506f  "Math128x128__Po
-000137d0: 7765 7255 6e64 6572 666c 6f77 222c 2274  werUnderflow","t
-000137e0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-000137f0: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00013800: 223a 2250 656e 6469 6e67 4f77 6e61 626c  ":"PendingOwnabl
-00013810: 655f 5f41 6464 7265 7373 5a65 726f 222c  e__AddressZero",
-00013820: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-00013830: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00013840: 6d65 223a 2250 656e 6469 6e67 4f77 6e61  me":"PendingOwna
-00013850: 626c 655f 5f4e 6f50 656e 6469 6e67 4f77  ble__NoPendingOw
-00013860: 6e65 7222 2c22 7479 7065 223a 2265 7272  ner","type":"err
-00013870: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00013880: 5d2c 226e 616d 6522 3a22 5065 6e64 696e  ],"name":"Pendin
-00013890: 674f 776e 6162 6c65 5f5f 4e6f 744f 776e  gOwnable__NotOwn
-000138a0: 6572 222c 2274 7970 6522 3a22 6572 726f  er","type":"erro
-000138b0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-000138c0: 2c22 6e61 6d65 223a 2250 656e 6469 6e67  ,"name":"Pending
-000138d0: 4f77 6e61 626c 655f 5f4e 6f74 5065 6e64  Ownable__NotPend
-000138e0: 696e 674f 776e 6572 222c 2274 7970 6522  ingOwner","type"
-000138f0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00013900: 7473 223a 5b5d 2c22 6e61 6d65 223a 2250  ts":[],"name":"P
-00013910: 656e 6469 6e67 4f77 6e61 626c 655f 5f50  endingOwnable__P
-00013920: 656e 6469 6e67 4f77 6e65 7241 6c72 6561  endingOwnerAlrea
-00013930: 6479 5365 7422 2c22 7479 7065 223a 2265  dySet","type":"e
-00013940: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00013950: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00013960: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00013970: 6522 3a22 7822 2c22 7479 7065 223a 2275  e":"x","type":"u
-00013980: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00013990: 3a22 5361 6665 4361 7374 5f5f 4578 6365  :"SafeCast__Exce
-000139a0: 6564 7331 3642 6974 7322 2c22 7479 7065  eds16Bits","type
-000139b0: 223a 2265 7272 6f72 227d 2c7b 2261 6e6f  ":"error"},{"ano
-000139c0: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
-000139d0: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
-000139e0: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-000139f0: 616c 5479 7065 223a 2262 6f6f 6c22 2c22  alType":"bool","
-00013a00: 6e61 6d65 223a 2275 6e6c 6f63 6b65 6422  name":"unlocked"
-00013a10: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
-00013a20: 2c22 6e61 6d65 223a 2246 6163 746f 7279  ,"name":"Factory
-00013a30: 4c6f 636b 6564 5374 6174 7573 5570 6461  LockedStatusUpda
-00013a40: 7465 6422 2c22 7479 7065 223a 2265 7665  ted","type":"eve
-00013a50: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
-00013a60: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
-00013a70: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
-00013a80: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00013a90: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-00013aa0: 223a 2273 656e 6465 7222 2c22 7479 7065  ":"sender","type
-00013ab0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00013ac0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-00013ad0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-00013ae0: 7472 6163 7420 494c 4250 6169 7222 2c22  tract ILBPair","
-00013af0: 6e61 6d65 223a 224c 4250 6169 7222 2c22  name":"LBPair","
-00013b00: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-00013b10: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-00013b20: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00013b30: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00013b40: 223a 2262 696e 5374 6570 222c 2274 7970  ":"binStep","typ
-00013b50: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00013b60: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-00013b70: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013b80: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00013b90: 6261 7365 4661 6374 6f72 222c 2274 7970  baseFactor","typ
-00013ba0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00013bb0: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-00013bc0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013bd0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00013be0: 6669 6c74 6572 5065 7269 6f64 222c 2274  filterPeriod","t
-00013bf0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00013c00: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-00013c10: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-00013c20: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00013c30: 3a22 6465 6361 7950 6572 696f 6422 2c22  :"decayPeriod","
-00013c40: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00013c50: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-00013c60: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00013c70: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00013c80: 223a 2272 6564 7563 7469 6f6e 4661 6374  ":"reductionFact
-00013c90: 6f72 222c 2274 7970 6522 3a22 7569 6e74  or","type":"uint
-00013ca0: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
-00013cb0: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
-00013cc0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00013cd0: 226e 616d 6522 3a22 7661 7269 6162 6c65  "name":"variable
-00013ce0: 4665 6543 6f6e 7472 6f6c 222c 2274 7970  FeeControl","typ
-00013cf0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00013d00: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-00013d10: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013d20: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00013d30: 7072 6f74 6f63 6f6c 5368 6172 6522 2c22  protocolShare","
-00013d40: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00013d50: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-00013d60: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00013d70: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00013d80: 223a 226d 6178 566f 6c61 7469 6c69 7479  ":"maxVolatility
-00013d90: 4163 6375 6d75 6c61 7465 6422 2c22 7479  Accumulated","ty
-00013da0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00013db0: 226e 616d 6522 3a22 4665 6550 6172 616d  "name":"FeeParam
-00013dc0: 6574 6572 7353 6574 222c 2274 7970 6522  etersSet","type"
-00013dd0: 3a22 6576 656e 7422 7d2c 7b22 616e 6f6e  :"event"},{"anon
-00013de0: 796d 6f75 7322 3a66 616c 7365 2c22 696e  ymous":false,"in
-00013df0: 7075 7473 223a 5b7b 2269 6e64 6578 6564  puts":[{"indexed
-00013e00: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-00013e10: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00013e20: 2c22 6e61 6d65 223a 226f 6c64 5265 6369  ,"name":"oldReci
-00013e30: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
-00013e40: 6464 7265 7373 227d 2c7b 2269 6e64 6578  ddress"},{"index
-00013e50: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
-00013e60: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00013e70: 7322 2c22 6e61 6d65 223a 226e 6577 5265  s","name":"newRe
-00013e80: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-00013e90: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
-00013ea0: 6522 3a22 4665 6552 6563 6970 6965 6e74  e":"FeeRecipient
-00013eb0: 5365 7422 2c22 7479 7065 223a 2265 7665  Set","type":"eve
-00013ec0: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
-00013ed0: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
-00013ee0: 3a5b 7b22 696e 6465 7865 6422 3a66 616c  :[{"indexed":fal
-00013ef0: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00013f00: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00013f10: 6522 3a22 6f6c 6446 6c61 7368 4c6f 616e  e":"oldFlashLoan
-00013f20: 4665 6522 2c22 7479 7065 223a 2275 696e  Fee","type":"uin
-00013f30: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
-00013f40: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-00013f50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00013f60: 2c22 6e61 6d65 223a 226e 6577 466c 6173  ,"name":"newFlas
-00013f70: 684c 6f61 6e46 6565 222c 2274 7970 6522  hLoanFee","type"
-00013f80: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00013f90: 6d65 223a 2246 6c61 7368 4c6f 616e 4665  me":"FlashLoanFe
-00013fa0: 6553 6574 222c 2274 7970 6522 3a22 6576  eSet","type":"ev
-00013fb0: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
-00013fc0: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
-00013fd0: 223a 5b7b 2269 6e64 6578 6564 223a 7472  ":[{"indexed":tr
-00013fe0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-00013ff0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-00014000: 3230 222c 226e 616d 6522 3a22 746f 6b65  20","name":"toke
-00014010: 6e58 222c 2274 7970 6522 3a22 6164 6472  nX","type":"addr
-00014020: 6573 7322 7d2c 7b22 696e 6465 7865 6422  ess"},{"indexed"
-00014030: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
-00014040: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00014050: 4552 4332 3022 2c22 6e61 6d65 223a 2274  ERC20","name":"t
-00014060: 6f6b 656e 5922 2c22 7479 7065 223a 2261  okenY","type":"a
-00014070: 6464 7265 7373 227d 2c7b 2269 6e64 6578  ddress"},{"index
-00014080: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
-00014090: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000140a0: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
-000140b0: 7022 2c22 7479 7065 223a 2275 696e 7432  p","type":"uint2
-000140c0: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
-000140d0: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
-000140e0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-000140f0: 4c42 5061 6972 222c 226e 616d 6522 3a22  LBPair","name":"
-00014100: 4c42 5061 6972 222c 2274 7970 6522 3a22  LBPair","type":"
-00014110: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-00014120: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-00014130: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00014140: 3536 222c 226e 616d 6522 3a22 7069 6422  56","name":"pid"
-00014150: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00014160: 227d 5d2c 226e 616d 6522 3a22 4c42 5061  "}],"name":"LBPa
-00014170: 6972 4372 6561 7465 6422 2c22 7479 7065  irCreated","type
-00014180: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
-00014190: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
-000141a0: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
-000141b0: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
-000141c0: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-000141d0: 2049 4c42 5061 6972 222c 226e 616d 6522   ILBPair","name"
-000141e0: 3a22 4c42 5061 6972 222c 2274 7970 6522  :"LBPair","type"
-000141f0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-00014200: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
-00014210: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
-00014220: 6c22 2c22 6e61 6d65 223a 2269 676e 6f72  l","name":"ignor
-00014230: 6564 222c 2274 7970 6522 3a22 626f 6f6c  ed","type":"bool
-00014240: 227d 5d2c 226e 616d 6522 3a22 4c42 5061  "}],"name":"LBPa
-00014250: 6972 4967 6e6f 7265 6453 7461 7465 4368  irIgnoredStateCh
-00014260: 616e 6765 6422 2c22 7479 7065 223a 2265  anged","type":"e
-00014270: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
-00014280: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
-00014290: 7322 3a5b 7b22 696e 6465 7865 6422 3a66  s":[{"indexed":f
-000142a0: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
-000142b0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-000142c0: 616d 6522 3a22 6f6c 644c 4250 6169 7249  ame":"oldLBPairI
-000142d0: 6d70 6c65 6d65 6e74 6174 696f 6e22 2c22  mplementation","
-000142e0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-000142f0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-00014300: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00014310: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-00014320: 223a 224c 4250 6169 7249 6d70 6c65 6d65  ":"LBPairImpleme
-00014330: 6e74 6174 696f 6e22 2c22 7479 7065 223a  ntation","type":
-00014340: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
-00014350: 6522 3a22 4c42 5061 6972 496d 706c 656d  e":"LBPairImplem
-00014360: 656e 7461 7469 6f6e 5365 7422 2c22 7479  entationSet","ty
-00014370: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
-00014380: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
-00014390: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
-000143a0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-000143b0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-000143c0: 7322 2c22 6e61 6d65 223a 2270 7265 7669  s","name":"previ
-000143d0: 6f75 734f 776e 6572 222c 2274 7970 6522  ousOwner","type"
-000143e0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-000143f0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-00014400: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00014410: 6573 7322 2c22 6e61 6d65 223a 226e 6577  ess","name":"new
-00014420: 4f77 6e65 7222 2c22 7479 7065 223a 2261  Owner","type":"a
-00014430: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
-00014440: 3a22 4f77 6e65 7273 6869 7054 7261 6e73  :"OwnershipTrans
-00014450: 6665 7272 6564 222c 2274 7970 6522 3a22  ferred","type":"
-00014460: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
-00014470: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
-00014480: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
-00014490: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-000144a0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-000144b0: 616d 6522 3a22 7065 6e64 696e 674f 776e  ame":"pendingOwn
-000144c0: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-000144d0: 6573 7322 7d5d 2c22 6e61 6d65 223a 2250  ess"}],"name":"P
-000144e0: 656e 6469 6e67 4f77 6e65 7253 6574 222c  endingOwnerSet",
-000144f0: 2274 7970 6522 3a22 6576 656e 7422 7d2c  "type":"event"},
-00014500: 7b22 616e 6f6e 796d 6f75 7322 3a66 616c  {"anonymous":fal
-00014510: 7365 2c22 696e 7075 7473 223a 5b7b 2269  se,"inputs":[{"i
-00014520: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-00014530: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00014540: 7432 3536 222c 226e 616d 6522 3a22 6269  t256","name":"bi
-00014550: 6e53 7465 7022 2c22 7479 7065 223a 2275  nStep","type":"u
-00014560: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00014570: 3a22 5072 6573 6574 5265 6d6f 7665 6422  :"PresetRemoved"
-00014580: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
-00014590: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
-000145a0: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
-000145b0: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-000145c0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000145d0: 6e74 3235 3622 2c22 6e61 6d65 223a 2262  nt256","name":"b
-000145e0: 696e 5374 6570 222c 2274 7970 6522 3a22  inStep","type":"
-000145f0: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
-00014600: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-00014610: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00014620: 3536 222c 226e 616d 6522 3a22 6261 7365  56","name":"base
-00014630: 4661 6374 6f72 222c 2274 7970 6522 3a22  Factor","type":"
-00014640: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
-00014650: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-00014660: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00014670: 3536 222c 226e 616d 6522 3a22 6669 6c74  56","name":"filt
-00014680: 6572 5065 7269 6f64 222c 2274 7970 6522  erPeriod","type"
-00014690: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-000146a0: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
-000146b0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-000146c0: 7432 3536 222c 226e 616d 6522 3a22 6465  t256","name":"de
-000146d0: 6361 7950 6572 696f 6422 2c22 7479 7065  cayPeriod","type
-000146e0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-000146f0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
-00014700: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00014710: 6e74 3235 3622 2c22 6e61 6d65 223a 2272  nt256","name":"r
-00014720: 6564 7563 7469 6f6e 4661 6374 6f72 222c  eductionFactor",
-00014730: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00014740: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-00014750: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00014760: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00014770: 6522 3a22 7661 7269 6162 6c65 4665 6543  e":"variableFeeC
-00014780: 6f6e 7472 6f6c 222c 2274 7970 6522 3a22  ontrol","type":"
-00014790: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
-000147a0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-000147b0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000147c0: 3536 222c 226e 616d 6522 3a22 7072 6f74  56","name":"prot
-000147d0: 6f63 6f6c 5368 6172 6522 2c22 7479 7065  ocolShare","type
-000147e0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-000147f0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
-00014800: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00014810: 6e74 3235 3622 2c22 6e61 6d65 223a 226d  nt256","name":"m
-00014820: 6178 566f 6c61 7469 6c69 7479 4163 6375  axVolatilityAccu
-00014830: 6d75 6c61 7465 6422 2c22 7479 7065 223a  mulated","type":
-00014840: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-00014850: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-00014860: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014870: 3235 3622 2c22 6e61 6d65 223a 2273 616d  256","name":"sam
-00014880: 706c 654c 6966 6574 696d 6522 2c22 7479  pleLifetime","ty
-00014890: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-000148a0: 226e 616d 6522 3a22 5072 6573 6574 5365  "name":"PresetSe
-000148b0: 7422 2c22 7479 7065 223a 2265 7665 6e74  t","type":"event
-000148c0: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
-000148d0: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
-000148e0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-000148f0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00014900: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
-00014910: 2c22 6e61 6d65 223a 2271 756f 7465 4173  ,"name":"quoteAs
-00014920: 7365 7422 2c22 7479 7065 223a 2261 6464  set","type":"add
-00014930: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-00014940: 5175 6f74 6541 7373 6574 4164 6465 6422  QuoteAssetAdded"
-00014950: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
-00014960: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
-00014970: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
-00014980: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-00014990: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-000149a0: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
-000149b0: 6e61 6d65 223a 2271 756f 7465 4173 7365  name":"quoteAsse
-000149c0: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
-000149d0: 7373 227d 5d2c 226e 616d 6522 3a22 5175  ss"}],"name":"Qu
-000149e0: 6f74 6541 7373 6574 5265 6d6f 7665 6422  oteAssetRemoved"
-000149f0: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
-00014a00: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00014a10: 616d 6522 3a22 4c42 5061 6972 496d 706c  ame":"LBPairImpl
-00014a20: 656d 656e 7461 7469 6f6e 222c 226f 7574  ementation","out
-00014a30: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00014a40: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00014a50: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-00014a60: 223a 2261 6464 7265 7373 227d 5d2c 2273  ":"address"}],"s
-00014a70: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00014a80: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00014a90: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00014aa0: 7473 223a 5b5d 2c22 6e61 6d65 223a 224d  ts":[],"name":"M
-00014ab0: 4158 5f42 494e 5f53 5445 5022 2c22 6f75  AX_BIN_STEP","ou
-00014ac0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-00014ad0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00014ae0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00014af0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00014b00: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00014b10: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00014b20: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00014b30: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-00014b40: 4d41 585f 4645 4522 2c22 6f75 7470 7574  MAX_FEE","output
-00014b50: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00014b60: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00014b70: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
-00014b80: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-00014b90: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-00014ba0: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-00014bb0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-00014bc0: 3a5b 5d2c 226e 616d 6522 3a22 4d41 585f  :[],"name":"MAX_
-00014bd0: 5052 4f54 4f43 4f4c 5f53 4841 5245 222c  PROTOCOL_SHARE",
-00014be0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00014bf0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014c00: 3235 3622 2c22 6e61 6d65 223a 2222 2c22  256","name":"","
-00014c10: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00014c20: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00014c30: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
-00014c40: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00014c50: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00014c60: 223a 224d 494e 5f42 494e 5f53 5445 5022  ":"MIN_BIN_STEP"
-00014c70: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00014c80: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00014c90: 7432 3536 222c 226e 616d 6522 3a22 222c  t256","name":"",
-00014ca0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00014cb0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-00014cc0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-00014cd0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00014ce0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00014cf0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-00014d00: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-00014d10: 6522 3a22 5f71 756f 7465 4173 7365 7422  e":"_quoteAsset"
-00014d20: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00014d30: 227d 5d2c 226e 616d 6522 3a22 6164 6451  "}],"name":"addQ
-00014d40: 756f 7465 4173 7365 7422 2c22 6f75 7470  uoteAsset","outp
-00014d50: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-00014d60: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-00014d70: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-00014d80: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00014d90: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00014da0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00014db0: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
-00014dc0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-00014dd0: 6522 3a22 616c 6c4c 4250 6169 7273 222c  e":"allLBPairs",
-00014de0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00014df0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-00014e00: 7261 6374 2049 4c42 5061 6972 222c 226e  ract ILBPair","n
-00014e10: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
-00014e20: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
-00014e30: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-00014e40: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-00014e50: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-00014e60: 3a5b 5d2c 226e 616d 6522 3a22 6265 636f  :[],"name":"beco
-00014e70: 6d65 4f77 6e65 7222 2c22 6f75 7470 7574  meOwner","output
-00014e80: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
-00014e90: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
-00014ea0: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
-00014eb0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-00014ec0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00014ed0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-00014ee0: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
-00014ef0: 6b65 6e58 222c 2274 7970 6522 3a22 6164  kenX","type":"ad
-00014f00: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-00014f10: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-00014f20: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
-00014f30: 3a22 5f74 6f6b 656e 5922 2c22 7479 7065  :"_tokenY","type
-00014f40: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00014f50: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00014f60: 6e74 3234 222c 226e 616d 6522 3a22 5f61  nt24","name":"_a
-00014f70: 6374 6976 6549 6422 2c22 7479 7065 223a  ctiveId","type":
-00014f80: 2275 696e 7432 3422 7d2c 7b22 696e 7465  "uint24"},{"inte
-00014f90: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
-00014fa0: 3622 2c22 6e61 6d65 223a 225f 6269 6e53  6","name":"_binS
-00014fb0: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
-00014fc0: 7431 3622 7d5d 2c22 6e61 6d65 223a 2263  t16"}],"name":"c
-00014fd0: 7265 6174 654c 4250 6169 7222 2c22 6f75  reateLBPair","ou
-00014fe0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-00014ff0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-00015000: 7420 494c 4250 6169 7222 2c22 6e61 6d65  t ILBPair","name
-00015010: 223a 225f 4c42 5061 6972 222c 2274 7970  ":"_LBPair","typ
-00015020: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-00015030: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00015040: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-00015050: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00015060: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00015070: 616d 6522 3a22 6372 6561 7469 6f6e 556e  ame":"creationUn
-00015080: 6c6f 636b 6564 222c 226f 7574 7075 7473  locked","outputs
-00015090: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-000150a0: 6522 3a22 626f 6f6c 222c 226e 616d 6522  e":"bool","name"
-000150b0: 3a22 222c 2274 7970 6522 3a22 626f 6f6c  :"","type":"bool
-000150c0: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-000150d0: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
-000150e0: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-000150f0: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00015100: 6d65 223a 2266 6565 5265 6369 7069 656e  me":"feeRecipien
-00015110: 7422 2c22 6f75 7470 7574 7322 3a5b 7b22  t","outputs":[{"
-00015120: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-00015130: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-00015140: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00015150: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
-00015160: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
-00015170: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00015180: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00015190: 616d 6522 3a22 666c 6173 684c 6f61 6e46  ame":"flashLoanF
-000151a0: 6565 222c 226f 7574 7075 7473 223a 5b7b  ee","outputs":[{
-000151b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000151c0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-000151d0: 2222 2c22 7479 7065 223a 2275 696e 7432  "","type":"uint2
-000151e0: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
-000151f0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-00015200: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00015210: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00015220: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-00015230: 6e74 7261 6374 2049 4c42 5061 6972 222c  ntract ILBPair",
-00015240: 226e 616d 6522 3a22 5f4c 4250 6169 7222  "name":"_LBPair"
-00015250: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00015260: 227d 5d2c 226e 616d 6522 3a22 666f 7263  "}],"name":"forc
-00015270: 6544 6563 6179 222c 226f 7574 7075 7473  eDecay","outputs
-00015280: 223a 5b5d 2c22 7374 6174 654d 7574 6162  ":[],"stateMutab
-00015290: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
-000152a0: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
-000152b0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-000152c0: 3a5b 5d2c 226e 616d 6522 3a22 6765 7441  :[],"name":"getA
-000152d0: 6c6c 4269 6e53 7465 7073 222c 226f 7574  llBinSteps","out
-000152e0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000152f0: 6c54 7970 6522 3a22 7569 6e74 3235 365b  lType":"uint256[
-00015300: 5d22 2c22 6e61 6d65 223a 2270 7265 7365  ]","name":"prese
-00015310: 7473 4269 6e53 7465 7022 2c22 7479 7065  tsBinStep","type
-00015320: 223a 2275 696e 7432 3536 5b5d 227d 5d2c  ":"uint256[]"}],
-00015330: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00015340: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00015350: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00015360: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00015370: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-00015380: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-00015390: 225f 746f 6b65 6e58 222c 2274 7970 6522  "_tokenX","type"
-000153a0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-000153b0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-000153c0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
-000153d0: 616d 6522 3a22 5f74 6f6b 656e 5922 2c22  ame":"_tokenY","
-000153e0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-000153f0: 5d2c 226e 616d 6522 3a22 6765 7441 6c6c  ],"name":"getAll
-00015400: 4c42 5061 6972 7322 2c22 6f75 7470 7574  LBPairs","output
-00015410: 7322 3a5b 7b22 636f 6d70 6f6e 656e 7473  s":[{"components
-00015420: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00015430: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
-00015440: 6522 3a22 6269 6e53 7465 7022 2c22 7479  e":"binStep","ty
-00015450: 7065 223a 2275 696e 7431 3622 7d2c 7b22  pe":"uint16"},{"
-00015460: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-00015470: 6f6e 7472 6163 7420 494c 4250 6169 7222  ontract ILBPair"
-00015480: 2c22 6e61 6d65 223a 224c 4250 6169 7222  ,"name":"LBPair"
-00015490: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-000154a0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000154b0: 6522 3a22 626f 6f6c 222c 226e 616d 6522  e":"bool","name"
-000154c0: 3a22 6372 6561 7465 6442 794f 776e 6572  :"createdByOwner
-000154d0: 222c 2274 7970 6522 3a22 626f 6f6c 227d  ","type":"bool"}
-000154e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000154f0: 3a22 626f 6f6c 222c 226e 616d 6522 3a22  :"bool","name":"
-00015500: 6967 6e6f 7265 6446 6f72 526f 7574 696e  ignoredForRoutin
-00015510: 6722 2c22 7479 7065 223a 2262 6f6f 6c22  g","type":"bool"
-00015520: 7d5d 2c22 696e 7465 726e 616c 5479 7065  }],"internalType
-00015530: 223a 2273 7472 7563 7420 494c 4246 6163  ":"struct ILBFac
-00015540: 746f 7279 2e4c 4250 6169 7249 6e66 6f72  tory.LBPairInfor
-00015550: 6d61 7469 6f6e 5b5d 222c 226e 616d 6522  mation[]","name"
-00015560: 3a22 4c42 5061 6972 7341 7661 696c 6162  :"LBPairsAvailab
-00015570: 6c65 222c 2274 7970 6522 3a22 7475 706c  le","type":"tupl
-00015580: 655b 5d22 7d5d 2c22 7374 6174 654d 7574  e[]"}],"stateMut
-00015590: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-000155a0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-000155b0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-000155c0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-000155d0: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
-000155e0: 226e 616d 6522 3a22 5f74 6f6b 656e 4122  "name":"_tokenA"
-000155f0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00015600: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00015610: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-00015620: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
-00015630: 6b65 6e42 222c 2274 7970 6522 3a22 6164  kenB","type":"ad
-00015640: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-00015650: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00015660: 222c 226e 616d 6522 3a22 5f62 696e 5374  ","name":"_binSt
-00015670: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-00015680: 3235 3622 7d5d 2c22 6e61 6d65 223a 2267  256"}],"name":"g
-00015690: 6574 4c42 5061 6972 496e 666f 726d 6174  etLBPairInformat
-000156a0: 696f 6e22 2c22 6f75 7470 7574 7322 3a5b  ion","outputs":[
-000156b0: 7b22 636f 6d70 6f6e 656e 7473 223a 5b7b  {"components":[{
-000156c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000156d0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
-000156e0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-000156f0: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
-00015700: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-00015710: 6163 7420 494c 4250 6169 7222 2c22 6e61  act ILBPair","na
-00015720: 6d65 223a 224c 4250 6169 7222 2c22 7479  me":"LBPair","ty
-00015730: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-00015740: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015750: 626f 6f6c 222c 226e 616d 6522 3a22 6372  bool","name":"cr
-00015760: 6561 7465 6442 794f 776e 6572 222c 2274  eatedByOwner","t
-00015770: 7970 6522 3a22 626f 6f6c 227d 2c7b 2269  ype":"bool"},{"i
-00015780: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
-00015790: 6f6c 222c 226e 616d 6522 3a22 6967 6e6f  ol","name":"igno
-000157a0: 7265 6446 6f72 526f 7574 696e 6722 2c22  redForRouting","
-000157b0: 7479 7065 223a 2262 6f6f 6c22 7d5d 2c22  type":"bool"}],"
-000157c0: 696e 7465 726e 616c 5479 7065 223a 2273  internalType":"s
-000157d0: 7472 7563 7420 494c 4246 6163 746f 7279  truct ILBFactory
-000157e0: 2e4c 4250 6169 7249 6e66 6f72 6d61 7469  .LBPairInformati
-000157f0: 6f6e 222c 226e 616d 6522 3a22 222c 2274  on","name":"","t
-00015800: 7970 6522 3a22 7475 706c 6522 7d5d 2c22  ype":"tuple"}],"
-00015810: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00015820: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00015830: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00015840: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-00015850: 6765 744e 756d 6265 724f 664c 4250 6169  getNumberOfLBPai
-00015860: 7273 222c 226f 7574 7075 7473 223a 5b7b  rs","outputs":[{
-00015870: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015880: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00015890: 2222 2c22 7479 7065 223a 2275 696e 7432  "","type":"uint2
-000158a0: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
-000158b0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-000158c0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-000158d0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-000158e0: 6e61 6d65 223a 2267 6574 4e75 6d62 6572  name":"getNumber
-000158f0: 4f66 5175 6f74 6541 7373 6574 7322 2c22  OfQuoteAssets","
-00015900: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-00015910: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00015920: 3536 222c 226e 616d 6522 3a22 222c 2274  56","name":"","t
-00015930: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00015940: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00015950: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-00015960: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00015970: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00015980: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
-00015990: 2c22 6e61 6d65 223a 225f 6269 6e53 7465  ,"name":"_binSte
-000159a0: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
-000159b0: 3622 7d5d 2c22 6e61 6d65 223a 2267 6574  6"}],"name":"get
-000159c0: 5072 6573 6574 222c 226f 7574 7075 7473  Preset","outputs
-000159d0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-000159e0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-000159f0: 6d65 223a 2262 6173 6546 6163 746f 7222  me":"baseFactor"
-00015a00: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00015a10: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00015a20: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00015a30: 6d65 223a 2266 696c 7465 7250 6572 696f  me":"filterPerio
-00015a40: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00015a50: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-00015a60: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00015a70: 6e61 6d65 223a 2264 6563 6179 5065 7269  name":"decayPeri
-00015a80: 6f64 222c 2274 7970 6522 3a22 7569 6e74  od","type":"uint
-00015a90: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00015aa0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00015ab0: 226e 616d 6522 3a22 7265 6475 6374 696f  "name":"reductio
-00015ac0: 6e46 6163 746f 7222 2c22 7479 7065 223a  nFactor","type":
-00015ad0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00015ae0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00015af0: 3235 3622 2c22 6e61 6d65 223a 2276 6172  256","name":"var
-00015b00: 6961 626c 6546 6565 436f 6e74 726f 6c22  iableFeeControl"
-00015b10: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00015b20: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00015b30: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00015b40: 6d65 223a 2270 726f 746f 636f 6c53 6861  me":"protocolSha
-00015b50: 7265 222c 2274 7970 6522 3a22 7569 6e74  re","type":"uint
-00015b60: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00015b70: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00015b80: 226e 616d 6522 3a22 6d61 7856 6f6c 6174  "name":"maxVolat
-00015b90: 696c 6974 7941 6363 756d 756c 6174 6564  ilityAccumulated
-00015ba0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00015bb0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00015bc0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00015bd0: 616d 6522 3a22 7361 6d70 6c65 4c69 6665  ame":"sampleLife
-00015be0: 7469 6d65 222c 2274 7970 6522 3a22 7569  time","type":"ui
-00015bf0: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-00015c00: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
-00015c10: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00015c20: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-00015c30: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015c40: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00015c50: 3a22 5f69 6e64 6578 222c 2274 7970 6522  :"_index","type"
-00015c60: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00015c70: 6d65 223a 2267 6574 5175 6f74 6541 7373  me":"getQuoteAss
-00015c80: 6574 222c 226f 7574 7075 7473 223a 5b7b  et","outputs":[{
-00015c90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015ca0: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
-00015cb0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-00015cc0: 223a 2261 6464 7265 7373 227d 5d2c 2273  ":"address"}],"s
-00015cd0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00015ce0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00015cf0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00015d00: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00015d10: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00015d20: 4552 4332 3022 2c22 6e61 6d65 223a 225f  ERC20","name":"_
-00015d30: 746f 6b65 6e22 2c22 7479 7065 223a 2261  token","type":"a
-00015d40: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
-00015d50: 3a22 6973 5175 6f74 6541 7373 6574 222c  :"isQuoteAsset",
-00015d60: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00015d70: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
-00015d80: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00015d90: 6522 3a22 626f 6f6c 227d 5d2c 2273 7461  e":"bool"}],"sta
-00015da0: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
-00015db0: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
-00015dc0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-00015dd0: 223a 5b5d 2c22 6e61 6d65 223a 226f 776e  ":[],"name":"own
-00015de0: 6572 222c 226f 7574 7075 7473 223a 5b7b  er","outputs":[{
-00015df0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015e00: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00015e10: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-00015e20: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-00015e30: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-00015e40: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00015e50: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00015e60: 6e61 6d65 223a 2270 656e 6469 6e67 4f77  name":"pendingOw
-00015e70: 6e65 7222 2c22 6f75 7470 7574 7322 3a5b  ner","outputs":[
-00015e80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015e90: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00015ea0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-00015eb0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-00015ec0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-00015ed0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00015ee0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00015ef0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00015f00: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
-00015f10: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-00015f20: 2275 696e 7431 3622 7d5d 2c22 6e61 6d65  "uint16"}],"name
-00015f30: 223a 2272 656d 6f76 6550 7265 7365 7422  ":"removePreset"
-00015f40: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
-00015f50: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00015f60: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
-00015f70: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00015f80: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-00015f90: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-00015fa0: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-00015fb0: 6d65 223a 225f 7175 6f74 6541 7373 6574  me":"_quoteAsset
-00015fc0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00015fd0: 7322 7d5d 2c22 6e61 6d65 223a 2272 656d  s"}],"name":"rem
-00015fe0: 6f76 6551 756f 7465 4173 7365 7422 2c22  oveQuoteAsset","
-00015ff0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00016000: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00016010: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00016020: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00016030: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00016040: 223a 2272 656e 6f75 6e63 654f 776e 6572  ":"renounceOwner
-00016050: 7368 6970 222c 226f 7574 7075 7473 223a  ship","outputs":
-00016060: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
-00016070: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
-00016080: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00016090: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-000160a0: 5d2c 226e 616d 6522 3a22 7265 766f 6b65  ],"name":"revoke
-000160b0: 5065 6e64 696e 674f 776e 6572 222c 226f  PendingOwner","o
-000160c0: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
-000160d0: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-000160e0: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-000160f0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00016100: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00016110: 616c 5479 7065 223a 2262 6f6f 6c22 2c22  alType":"bool","
-00016120: 6e61 6d65 223a 225f 6c6f 636b 6564 222c  name":"_locked",
-00016130: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-00016140: 226e 616d 6522 3a22 7365 7446 6163 746f  "name":"setFacto
-00016150: 7279 4c6f 636b 6564 5374 6174 6522 2c22  ryLockedState","
-00016160: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00016170: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00016180: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00016190: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-000161a0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-000161b0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-000161c0: 7322 2c22 6e61 6d65 223a 225f 6665 6552  s","name":"_feeR
-000161d0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-000161e0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-000161f0: 6d65 223a 2273 6574 4665 6552 6563 6970  me":"setFeeRecip
-00016200: 6965 6e74 222c 226f 7574 7075 7473 223a  ient","outputs":
-00016210: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
-00016220: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
-00016230: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00016240: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-00016250: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00016260: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
-00016270: 222c 226e 616d 6522 3a22 5f74 6f6b 656e  ","name":"_token
-00016280: 5822 2c22 7479 7065 223a 2261 6464 7265  X","type":"addre
-00016290: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-000162a0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-000162b0: 4552 4332 3022 2c22 6e61 6d65 223a 225f  ERC20","name":"_
-000162c0: 746f 6b65 6e59 222c 2274 7970 6522 3a22  tokenY","type":"
-000162d0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-000162e0: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
-000162f0: 3622 2c22 6e61 6d65 223a 225f 6269 6e53  6","name":"_binS
-00016300: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
-00016310: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
-00016320: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
-00016330: 6e61 6d65 223a 225f 6261 7365 4661 6374  name":"_baseFact
-00016340: 6f72 222c 2274 7970 6522 3a22 7569 6e74  or","type":"uint
-00016350: 3136 227d 2c7b 2269 6e74 6572 6e61 6c54  16"},{"internalT
-00016360: 7970 6522 3a22 7569 6e74 3136 222c 226e  ype":"uint16","n
-00016370: 616d 6522 3a22 5f66 696c 7465 7250 6572  ame":"_filterPer
-00016380: 696f 6422 2c22 7479 7065 223a 2275 696e  iod","type":"uin
-00016390: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
-000163a0: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
-000163b0: 6e61 6d65 223a 225f 6465 6361 7950 6572  name":"_decayPer
-000163c0: 696f 6422 2c22 7479 7065 223a 2275 696e  iod","type":"uin
-000163d0: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
-000163e0: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
-000163f0: 6e61 6d65 223a 225f 7265 6475 6374 696f  name":"_reductio
-00016400: 6e46 6163 746f 7222 2c22 7479 7065 223a  nFactor","type":
-00016410: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
-00016420: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00016430: 3422 2c22 6e61 6d65 223a 225f 7661 7269  4","name":"_vari
-00016440: 6162 6c65 4665 6543 6f6e 7472 6f6c 222c  ableFeeControl",
-00016450: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
-00016460: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00016470: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00016480: 3a22 5f70 726f 746f 636f 6c53 6861 7265  :"_protocolShare
-00016490: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-000164a0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000164b0: 6522 3a22 7569 6e74 3234 222c 226e 616d  e":"uint24","nam
-000164c0: 6522 3a22 5f6d 6178 566f 6c61 7469 6c69  e":"_maxVolatili
-000164d0: 7479 4163 6375 6d75 6c61 7465 6422 2c22  tyAccumulated","
-000164e0: 7479 7065 223a 2275 696e 7432 3422 7d5d  type":"uint24"}]
-000164f0: 2c22 6e61 6d65 223a 2273 6574 4665 6573  ,"name":"setFees
-00016500: 5061 7261 6d65 7465 7273 4f6e 5061 6972  ParametersOnPair
-00016510: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
-00016520: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00016530: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-00016540: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00016550: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00016560: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00016570: 7432 3536 222c 226e 616d 6522 3a22 5f66  t256","name":"_f
-00016580: 6c61 7368 4c6f 616e 4665 6522 2c22 7479  lashLoanFee","ty
-00016590: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-000165a0: 226e 616d 6522 3a22 7365 7446 6c61 7368  "name":"setFlash
-000165b0: 4c6f 616e 4665 6522 2c22 6f75 7470 7574  LoanFee","output
-000165c0: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
-000165d0: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
-000165e0: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
-000165f0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-00016600: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00016610: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-00016620: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
-00016630: 6b65 6e58 222c 2274 7970 6522 3a22 6164  kenX","type":"ad
-00016640: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-00016650: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-00016660: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
-00016670: 3a22 5f74 6f6b 656e 5922 2c22 7479 7065  :"_tokenY","type
-00016680: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00016690: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000166a0: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-000166b0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-000166c0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-000166d0: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
-000166e0: 222c 226e 616d 6522 3a22 5f69 676e 6f72  ","name":"_ignor
-000166f0: 6564 222c 2274 7970 6522 3a22 626f 6f6c  ed","type":"bool
-00016700: 227d 5d2c 226e 616d 6522 3a22 7365 744c  "}],"name":"setL
-00016710: 4250 6169 7249 676e 6f72 6564 222c 226f  BPairIgnored","o
-00016720: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
-00016730: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-00016740: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-00016750: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00016760: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00016770: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00016780: 222c 226e 616d 6522 3a22 5f4c 4250 6169  ","name":"_LBPai
-00016790: 7249 6d70 6c65 6d65 6e74 6174 696f 6e22  rImplementation"
-000167a0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-000167b0: 227d 5d2c 226e 616d 6522 3a22 7365 744c  "}],"name":"setL
-000167c0: 4250 6169 7249 6d70 6c65 6d65 6e74 6174  BPairImplementat
-000167d0: 696f 6e22 2c22 6f75 7470 7574 7322 3a5b  ion","outputs":[
-000167e0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-000167f0: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
-00016800: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-00016810: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-00016820: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00016830: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00016840: 2270 656e 6469 6e67 4f77 6e65 725f 222c  "pendingOwner_",
-00016850: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-00016860: 7d5d 2c22 6e61 6d65 223a 2273 6574 5065  }],"name":"setPe
-00016870: 6e64 696e 674f 776e 6572 222c 226f 7574  ndingOwner","out
-00016880: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-00016890: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-000168a0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-000168b0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-000168c0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-000168d0: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
-000168e0: 6e61 6d65 223a 225f 6269 6e53 7465 7022  name":"_binStep"
-000168f0: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-00016900: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00016910: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00016920: 223a 225f 6261 7365 4661 6374 6f72 222c  ":"_baseFactor",
-00016930: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-00016940: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00016950: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00016960: 3a22 5f66 696c 7465 7250 6572 696f 6422  :"_filterPeriod"
-00016970: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-00016980: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00016990: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-000169a0: 223a 225f 6465 6361 7950 6572 696f 6422  ":"_decayPeriod"
-000169b0: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-000169c0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000169d0: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-000169e0: 223a 225f 7265 6475 6374 696f 6e46 6163  ":"_reductionFac
-000169f0: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
-00016a00: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
-00016a10: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-00016a20: 6e61 6d65 223a 225f 7661 7269 6162 6c65  name":"_variable
-00016a30: 4665 6543 6f6e 7472 6f6c 222c 2274 7970  FeeControl","typ
-00016a40: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
-00016a50: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00016a60: 6e74 3136 222c 226e 616d 6522 3a22 5f70  nt16","name":"_p
-00016a70: 726f 746f 636f 6c53 6861 7265 222c 2274  rotocolShare","t
-00016a80: 7970 6522 3a22 7569 6e74 3136 227d 2c7b  ype":"uint16"},{
-00016a90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00016aa0: 7569 6e74 3234 222c 226e 616d 6522 3a22  uint24","name":"
-00016ab0: 5f6d 6178 566f 6c61 7469 6c69 7479 4163  _maxVolatilityAc
-00016ac0: 6375 6d75 6c61 7465 6422 2c22 7479 7065  cumulated","type
-00016ad0: 223a 2275 696e 7432 3422 7d2c 7b22 696e  ":"uint24"},{"in
-00016ae0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00016af0: 7431 3622 2c22 6e61 6d65 223a 225f 7361  t16","name":"_sa
-00016b00: 6d70 6c65 4c69 6665 7469 6d65 222c 2274  mpleLifetime","t
-00016b10: 7970 6522 3a22 7569 6e74 3136 227d 5d2c  ype":"uint16"}],
-00016b20: 226e 616d 6522 3a22 7365 7450 7265 7365  "name":"setPrese
-00016b30: 7422 2c22 6f75 7470 7574 7322 3a5b 5d2c  t","outputs":[],
-00016b40: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00016b50: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-00016b60: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00016b70: 7d5d 2729 0a0a 2020 2020 236a 6f65 2066  }]')..    #joe f
-00016b80: 6163 6f74 7279 0a20 2020 2064 6566 2067  acotry.    def g
-00016b90: 6574 5f6e 756d 6265 725f 6f66 5f6c 625f  et_number_of_lb_
-00016ba0: 7061 6972 7328 5f77 6562 333a 5765 6233  pairs(_web3:Web3
-00016bb0: 2c5f 6661 6374 6f72 795f 6164 6472 6573  ,_factory_addres
-00016bc0: 7329 3a0a 2020 2020 2020 2020 7265 7475  s):.        retu
-00016bd0: 726e 205f 7765 6233 2e65 7468 2e63 6f6e  rn _web3.eth.con
-00016be0: 7472 6163 7428 6164 6472 6573 733d 5f66  tract(address=_f
-00016bf0: 6163 746f 7279 5f61 6464 7265 7373 2c20  actory_address, 
-00016c00: 6162 693d 4a6f 6556 3246 6163 746f 7279  abi=JoeV2Factory
-00016c10: 2e6a 6f65 5f66 6163 746f 7279 5f76 325f  .joe_factory_v2_
-00016c20: 6162 6929 2e66 756e 6374 696f 6e73 2e67  abi).functions.g
-00016c30: 6574 4e75 6d62 6572 4f66 4c42 5061 6972  etNumberOfLBPair
-00016c40: 7328 292e 6361 6c6c 2829 0a0a 2020 2020  s().call()..    
-00016c50: 6465 6620 6765 745f 6e75 6d62 6572 5f6f  def get_number_o
-00016c60: 665f 7175 6f74 655f 6173 7365 7473 285f  f_quote_assets(_
-00016c70: 7765 6233 3a57 6562 332c 5f66 6163 746f  web3:Web3,_facto
-00016c80: 7279 5f61 6464 7265 7373 293a 0a20 2020  ry_address):.   
-00016c90: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-00016ca0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-00016cb0: 6464 7265 7373 3d5f 6661 6374 6f72 795f  ddress=_factory_
-00016cc0: 6164 6472 6573 732c 2061 6269 3d4a 6f65  address, abi=Joe
-00016cd0: 5632 4661 6374 6f72 792e 6a6f 655f 6661  V2Factory.joe_fa
-00016ce0: 6374 6f72 795f 7632 5f61 6269 292e 6675  ctory_v2_abi).fu
-00016cf0: 6e63 7469 6f6e 732e 6765 744e 756d 6265  nctions.getNumbe
-00016d00: 724f 6651 756f 7465 4173 7365 7473 2829  rOfQuoteAssets()
-00016d10: 2e63 616c 6c28 290a 0a20 2020 2064 6566  .call()..    def
-00016d20: 2067 6574 5f71 756f 7465 5f61 7373 6574   get_quote_asset
-00016d30: 285f 7765 6233 3a57 6562 332c 5f66 6163  (_web3:Web3,_fac
-00016d40: 746f 7279 5f61 6464 7265 7373 2c5f 696e  tory_address,_in
-00016d50: 6465 7829 3a0a 2020 2020 2020 2020 7265  dex):.        re
-00016d60: 7475 726e 205f 7765 6233 2e65 7468 2e63  turn _web3.eth.c
-00016d70: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
-00016d80: 5f66 6163 746f 7279 5f61 6464 7265 7373  _factory_address
-00016d90: 2c20 6162 693d 4a6f 6556 3246 6163 746f  , abi=JoeV2Facto
-00016da0: 7279 2e6a 6f65 5f66 6163 746f 7279 5f76  ry.joe_factory_v
-00016db0: 325f 6162 6929 2e66 756e 6374 696f 6e73  2_abi).functions
-00016dc0: 2e67 6574 5175 6f74 6541 7373 6574 285f  .getQuoteAsset(_
-00016dd0: 696e 6465 7829 2e63 616c 6c28 290a 0a20  index).call().. 
-00016de0: 2020 2064 6566 2069 735f 7175 6f74 655f     def is_quote_
-00016df0: 6173 7365 7428 5f77 6562 333a 5765 6233  asset(_web3:Web3
-00016e00: 2c5f 6661 6374 6f72 795f 6164 6472 6573  ,_factory_addres
-00016e10: 732c 5f61 6464 7265 7373 3a73 7472 293a  s,_address:str):
-00016e20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016e30: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
-00016e40: 6374 2861 6464 7265 7373 3d5f 6661 6374  ct(address=_fact
-00016e50: 6f72 795f 6164 6472 6573 732c 2061 6269  ory_address, abi
-00016e60: 3d4a 6f65 5632 4661 6374 6f72 792e 6a6f  =JoeV2Factory.jo
-00016e70: 655f 6661 6374 6f72 795f 7632 5f61 6269  e_factory_v2_abi
-00016e80: 292e 6675 6e63 7469 6f6e 732e 6973 5175  ).functions.isQu
-00016e90: 6f74 6541 7373 6574 285f 6164 6472 6573  oteAsset(_addres
-00016ea0: 7329 2e63 616c 6c28 290a 0a20 2020 2064  s).call()..    d
-00016eb0: 6566 2067 6574 5f70 6169 725f 696e 666f  ef get_pair_info
-00016ec0: 726d 6174 696f 6e28 5f77 6562 333a 5765  rmation(_web3:We
-00016ed0: 6233 2c5f 6661 6374 6f72 795f 6164 6472  b3,_factory_addr
-00016ee0: 6573 732c 5f74 6f6b 656e 5f61 3a73 7472  ess,_token_a:str
-00016ef0: 2c5f 746f 6b65 6e5f 623a 7374 722c 5f62  ,_token_b:str,_b
-00016f00: 696e 5f73 7465 7029 3a0a 2020 2020 2020  in_step):.      
-00016f10: 2020 7265 7475 726e 205f 7765 6233 2e65    return _web3.e
-00016f20: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-00016f30: 6573 733d 5f66 6163 746f 7279 5f61 6464  ess=_factory_add
-00016f40: 7265 7373 2c20 6162 693d 4a6f 6556 3246  ress, abi=JoeV2F
-00016f50: 6163 746f 7279 2e6a 6f65 5f66 6163 746f  actory.joe_facto
-00016f60: 7279 5f76 325f 6162 6929 2e66 756e 6374  ry_v2_abi).funct
-00016f70: 696f 6e73 2e67 6574 4c42 5061 6972 496e  ions.getLBPairIn
-00016f80: 666f 726d 6174 696f 6e28 5f74 6f6b 656e  formation(_token
-00016f90: 5f61 2c5f 746f 6b65 6e5f 622c 5f62 696e  _a,_token_b,_bin
-00016fa0: 5f73 7465 7029 2e63 616c 6c28 290a 0a20  _step).call().. 
-00016fb0: 2020 2064 6566 2067 6574 5f61 6c6c 5f6c     def get_all_l
-00016fc0: 625f 7061 6972 7328 5f77 6562 333a 5765  b_pairs(_web3:We
-00016fd0: 6233 2c5f 6661 6374 6f72 795f 6164 6472  b3,_factory_addr
-00016fe0: 6573 732c 5f74 6f6b 656e 5f61 3a73 7472  ess,_token_a:str
-00016ff0: 2c5f 746f 6b65 6e5f 623a 7374 7229 3a0a  ,_token_b:str):.
-00017000: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00017010: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
-00017020: 7428 6164 6472 6573 733d 5f66 6163 746f  t(address=_facto
-00017030: 7279 5f61 6464 7265 7373 2c20 6162 693d  ry_address, abi=
-00017040: 4a6f 6556 3246 6163 746f 7279 2e6a 6f65  JoeV2Factory.joe
-00017050: 5f66 6163 746f 7279 5f76 325f 6162 6929  _factory_v2_abi)
-00017060: 2e66 756e 6374 696f 6e73 2e67 6574 416c  .functions.getAl
-00017070: 6c4c 4250 6169 7273 285f 746f 6b65 6e5f  lLBPairs(_token_
-00017080: 612c 5f74 6f6b 656e 5f62 292e 6361 6c6c  a,_token_b).call
-00017090: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
-000170a0: 616c 6c5f 6269 6e5f 7374 6570 7328 5f77  all_bin_steps(_w
-000170b0: 6562 333a 5765 6233 2c5f 6661 6374 6f72  eb3:Web3,_factor
-000170c0: 795f 6164 6472 6573 7329 3a0a 2020 2020  y_address):.    
-000170d0: 2020 2020 7265 7475 726e 205f 7765 6233      return _web3
-000170e0: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
-000170f0: 6472 6573 733d 5f66 6163 746f 7279 5f61  dress=_factory_a
-00017100: 6464 7265 7373 2c20 6162 693d 4a6f 6556  ddress, abi=JoeV
-00017110: 3246 6163 746f 7279 2e6a 6f65 5f66 6163  2Factory.joe_fac
-00017120: 746f 7279 5f76 325f 6162 6929 2e66 756e  tory_v2_abi).fun
-00017130: 6374 696f 6e73 2e67 6574 416c 6c42 696e  ctions.getAllBin
-00017140: 5374 6570 7328 292e 6361 6c6c 2829 0a0a  Steps().call()..
-00017150: 636c 6173 7320 4a6f 6556 3251 756f 7465  class JoeV2Quote
-00017160: 3a0a 2020 2020 6a6f 655f 7175 6f74 655f  :.    joe_quote_
-00017170: 7632 5f61 6269 3d27 5b7b 2269 6e70 7574  v2_abi='[{"input
-00017180: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00017190: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-000171a0: 616d 6522 3a22 5f72 6f75 7465 7256 3222  ame":"_routerV2"
-000171b0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-000171c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000171d0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-000171e0: 6d65 223a 225f 6661 6374 6f72 7956 3122  me":"_factoryV1"
-000171f0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00017200: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00017210: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-00017220: 6d65 223a 225f 6661 6374 6f72 7956 3222  me":"_factoryV2"
-00017230: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00017240: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-00017250: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
-00017260: 6522 2c22 7479 7065 223a 2263 6f6e 7374  e","type":"const
-00017270: 7275 6374 6f72 227d 2c7b 2269 6e70 7574  ructor"},{"input
-00017280: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00017290: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-000172a0: 616d 6522 3a22 6270 222c 2274 7970 6522  ame":"bp","type"
-000172b0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-000172c0: 6d65 223a 2242 696e 4865 6c70 6572 5f5f  me":"BinHelper__
-000172d0: 4269 6e53 7465 704f 7665 7266 6c6f 7773  BinStepOverflows
-000172e0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-000172f0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00017300: 6e61 6d65 223a 2242 696e 4865 6c70 6572  name":"BinHelper
-00017310: 5f5f 4964 4f76 6572 666c 6f77 7322 2c22  __IdOverflows","
-00017320: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00017330: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00017340: 6522 3a22 4a6f 654c 6962 7261 7279 5f5f  e":"JoeLibrary__
-00017350: 4164 6472 6573 735a 6572 6f22 2c22 7479  AddressZero","ty
-00017360: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00017370: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-00017380: 3a22 4a6f 654c 6962 7261 7279 5f5f 4964  :"JoeLibrary__Id
-00017390: 656e 7469 6361 6c41 6464 7265 7373 6573  enticalAddresses
-000173a0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-000173b0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-000173c0: 6e61 6d65 223a 224a 6f65 4c69 6272 6172  name":"JoeLibrar
-000173d0: 795f 5f49 6e73 7566 6669 6369 656e 7441  y__InsufficientA
-000173e0: 6d6f 756e 7422 2c22 7479 7065 223a 2265  mount","type":"e
-000173f0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00017400: 3a5b 5d2c 226e 616d 6522 3a22 4a6f 654c  :[],"name":"JoeL
-00017410: 6962 7261 7279 5f5f 496e 7375 6666 6963  ibrary__Insuffic
-00017420: 6965 6e74 4c69 7175 6964 6974 7922 2c22  ientLiquidity","
-00017430: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00017440: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00017450: 6522 3a22 4c42 5175 6f74 6572 5f49 6e76  e":"LBQuoter_Inv
-00017460: 616c 6964 4c65 6e67 7468 222c 2274 7970  alidLength","typ
-00017470: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-00017480: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00017490: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-000174a0: 2c22 6e61 6d65 223a 2278 222c 2274 7970  ,"name":"x","typ
-000174b0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-000174c0: 696e 7465 726e 616c 5479 7065 223a 2269  internalType":"i
-000174d0: 6e74 3235 3622 2c22 6e61 6d65 223a 2279  nt256","name":"y
-000174e0: 222c 2274 7970 6522 3a22 696e 7432 3536  ","type":"int256
-000174f0: 227d 5d2c 226e 616d 6522 3a22 4d61 7468  "}],"name":"Math
-00017500: 3132 3878 3132 385f 5f50 6f77 6572 556e  128x128__PowerUn
-00017510: 6465 7266 6c6f 7722 2c22 7479 7065 223a  derflow","type":
-00017520: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00017530: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00017540: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00017550: 616d 6522 3a22 7072 6f64 3122 2c22 7479  ame":"prod1","ty
-00017560: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00017570: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00017580: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00017590: 2264 656e 6f6d 696e 6174 6f72 222c 2274  "denominator","t
-000175a0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-000175b0: 2c22 6e61 6d65 223a 224d 6174 6835 3132  ,"name":"Math512
-000175c0: 4269 7473 5f5f 4d75 6c44 6976 4f76 6572  Bits__MulDivOver
-000175d0: 666c 6f77 222c 2274 7970 6522 3a22 6572  flow","type":"er
-000175e0: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-000175f0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00017600: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00017610: 223a 2270 726f 6431 222c 2274 7970 6522  ":"prod1","type"
-00017620: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00017630: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00017640: 7432 3536 222c 226e 616d 6522 3a22 6f66  t256","name":"of
-00017650: 6673 6574 222c 2274 7970 6522 3a22 7569  fset","type":"ui
-00017660: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00017670: 224d 6174 6835 3132 4269 7473 5f5f 4d75  "Math512Bits__Mu
-00017680: 6c53 6869 6674 4f76 6572 666c 6f77 222c  lShiftOverflow",
-00017690: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-000176a0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-000176b0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000176c0: 3235 3622 2c22 6e61 6d65 223a 226f 6666  256","name":"off
-000176d0: 7365 7422 2c22 7479 7065 223a 2275 696e  set","type":"uin
-000176e0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-000176f0: 4d61 7468 3531 3242 6974 735f 5f4f 6666  Math512Bits__Off
-00017700: 7365 744f 7665 7266 6c6f 7773 222c 2274  setOverflows","t
-00017710: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00017720: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00017730: 223a 2266 6163 746f 7279 5631 222c 226f  ":"factoryV1","o
-00017740: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00017750: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00017760: 7322 2c22 6e61 6d65 223a 2222 2c22 7479  s","name":"","ty
-00017770: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-00017780: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00017790: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-000177a0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000177b0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-000177c0: 2266 6163 746f 7279 5632 222c 226f 7574  "factoryV2","out
-000177d0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000177e0: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-000177f0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-00017800: 223a 2261 6464 7265 7373 227d 5d2c 2273  ":"address"}],"s
-00017810: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00017820: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00017830: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00017840: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00017850: 7970 6522 3a22 6164 6472 6573 735b 5d22  ype":"address[]"
-00017860: 2c22 6e61 6d65 223a 225f 726f 7574 6522  ,"name":"_route"
-00017870: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00017880: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
-00017890: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-000178a0: 6e61 6d65 223a 225f 616d 6f75 6e74 496e  name":"_amountIn
-000178b0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-000178c0: 3622 7d5d 2c22 6e61 6d65 223a 2266 696e  6"}],"name":"fin
-000178d0: 6442 6573 7450 6174 6846 726f 6d41 6d6f  dBestPathFromAmo
-000178e0: 756e 7449 6e22 2c22 6f75 7470 7574 7322  untIn","outputs"
-000178f0: 3a5b 7b22 636f 6d70 6f6e 656e 7473 223a  :[{"components":
-00017900: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00017910: 3a22 6164 6472 6573 735b 5d22 2c22 6e61  :"address[]","na
-00017920: 6d65 223a 2272 6f75 7465 222c 2274 7970  me":"route","typ
-00017930: 6522 3a22 6164 6472 6573 735b 5d22 7d2c  e":"address[]"},
-00017940: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00017950: 2261 6464 7265 7373 5b5d 222c 226e 616d  "address[]","nam
-00017960: 6522 3a22 7061 6972 7322 2c22 7479 7065  e":"pairs","type
-00017970: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
-00017980: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00017990: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
-000179a0: 223a 2262 696e 5374 6570 7322 2c22 7479  ":"binSteps","ty
-000179b0: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
-000179c0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000179d0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-000179e0: 6d65 223a 2261 6d6f 756e 7473 222c 2274  me":"amounts","t
-000179f0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-00017a00: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00017a10: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-00017a20: 616d 6522 3a22 7669 7274 7561 6c41 6d6f  ame":"virtualAmo
-00017a30: 756e 7473 5769 7468 6f75 7453 6c69 7070  untsWithoutSlipp
-00017a40: 6167 6522 2c22 7479 7065 223a 2275 696e  age","type":"uin
-00017a50: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
-00017a60: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00017a70: 365b 5d22 2c22 6e61 6d65 223a 2266 6565  6[]","name":"fee
-00017a80: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-00017a90: 3536 5b5d 227d 5d2c 2269 6e74 6572 6e61  56[]"}],"interna
-00017aa0: 6c54 7970 6522 3a22 7374 7275 6374 204c  lType":"struct L
-00017ab0: 4251 756f 7465 722e 5175 6f74 6522 2c22  BQuoter.Quote","
-00017ac0: 6e61 6d65 223a 2271 756f 7465 222c 2274  name":"quote","t
-00017ad0: 7970 6522 3a22 7475 706c 6522 7d5d 2c22  ype":"tuple"}],"
-00017ae0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00017af0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00017b00: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00017b10: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00017b20: 5479 7065 223a 2261 6464 7265 7373 5b5d  Type":"address[]
-00017b30: 222c 226e 616d 6522 3a22 5f72 6f75 7465  ","name":"_route
-00017b40: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00017b50: 735b 5d22 7d2c 7b22 696e 7465 726e 616c  s[]"},{"internal
-00017b60: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00017b70: 226e 616d 6522 3a22 5f61 6d6f 756e 744f  "name":"_amountO
-00017b80: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
-00017b90: 3235 3622 7d5d 2c22 6e61 6d65 223a 2266  256"}],"name":"f
-00017ba0: 696e 6442 6573 7450 6174 6846 726f 6d41  indBestPathFromA
-00017bb0: 6d6f 756e 744f 7574 222c 226f 7574 7075  mountOut","outpu
-00017bc0: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
-00017bd0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00017be0: 7065 223a 2261 6464 7265 7373 5b5d 222c  pe":"address[]",
-00017bf0: 226e 616d 6522 3a22 726f 7574 6522 2c22  "name":"route","
-00017c00: 7479 7065 223a 2261 6464 7265 7373 5b5d  type":"address[]
-00017c10: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00017c20: 6522 3a22 6164 6472 6573 735b 5d22 2c22  e":"address[]","
-00017c30: 6e61 6d65 223a 2270 6169 7273 222c 2274  name":"pairs","t
-00017c40: 7970 6522 3a22 6164 6472 6573 735b 5d22  ype":"address[]"
-00017c50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00017c60: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-00017c70: 616d 6522 3a22 6269 6e53 7465 7073 222c  ame":"binSteps",
-00017c80: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
-00017c90: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-00017ca0: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-00017cb0: 226e 616d 6522 3a22 616d 6f75 6e74 7322  "name":"amounts"
-00017cc0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00017cd0: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
-00017ce0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-00017cf0: 2c22 6e61 6d65 223a 2276 6972 7475 616c  ,"name":"virtual
-00017d00: 416d 6f75 6e74 7357 6974 686f 7574 536c  AmountsWithoutSl
-00017d10: 6970 7061 6765 222c 2274 7970 6522 3a22  ippage","type":"
-00017d20: 7569 6e74 3235 365b 5d22 7d2c 7b22 696e  uint256[]"},{"in
-00017d30: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00017d40: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-00017d50: 6665 6573 222c 2274 7970 6522 3a22 7569  fees","type":"ui
-00017d60: 6e74 3235 365b 5d22 7d5d 2c22 696e 7465  nt256[]"}],"inte
-00017d70: 726e 616c 5479 7065 223a 2273 7472 7563  rnalType":"struc
-00017d80: 7420 4c42 5175 6f74 6572 2e51 756f 7465  t LBQuoter.Quote
-00017d90: 222c 226e 616d 6522 3a22 7175 6f74 6522  ","name":"quote"
-00017da0: 2c22 7479 7065 223a 2274 7570 6c65 227d  ,"type":"tuple"}
-00017db0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00017dc0: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
-00017dd0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00017de0: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00017df0: 223a 2272 6f75 7465 7256 3222 2c22 6f75  ":"routerV2","ou
-00017e00: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-00017e10: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00017e20: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00017e30: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-00017e40: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00017e50: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00017e60: 6675 6e63 7469 6f6e 227d 5d27 0a0a 2020  function"}]'..  
-00017e70: 2020 2372 6574 7572 6e20 7175 6f74 650a    #return quote.
-00017e80: 2020 2020 2320 2020 2073 7472 7563 7420      #    struct 
-00017e90: 5175 6f74 6520 7b0a 2020 2020 2320 2020  Quote {.    #   
-00017ea0: 2020 6164 6472 6573 735b 5d20 726f 7574    address[] rout
-00017eb0: 653b 2069 6e20 746f 6b65 6e20 e59c a8e5  e; in token ....
-00017ec0: 898d 0a20 2020 2023 2020 2020 2061 6464  ...    #     add
-00017ed0: 7265 7373 5b5d 2070 6169 7273 3b0a 2020  ress[] pairs;.  
-00017ee0: 2020 2320 2020 2020 7569 6e74 3235 365b    #     uint256[
-00017ef0: 5d20 6269 6e53 7465 7073 3b0a 2020 2020  ] binSteps;.    
-00017f00: 2320 2020 2020 7569 6e74 3235 365b 5d20  #     uint256[] 
-00017f10: 616d 6f75 6e74 733b 20e6 95b0 e7bb 842c  amounts; ......,
-00017f20: e9a1 bae5 ba8f e4b8 8ee8 b7af e5be 84e4  ................
-00017f30: b880 e887 b40a 2020 2020 2320 2020 2020  ......    #     
-00017f40: 7569 6e74 3235 365b 5d20 7669 7274 7561  uint256[] virtua
-00017f50: 6c41 6d6f 756e 7473 5769 7468 6f75 7453  lAmountsWithoutS
-00017f60: 6c69 7070 6167 653b 0a20 2020 2023 2020  lippage;.    #  
-00017f70: 2020 2075 696e 7432 3536 5b5d 2066 6565     uint256[] fee
-00017f80: 733b 0a20 2020 2023 207d 0a20 2020 2064  s;.    # }.    d
-00017f90: 6566 2066 696e 645f 6265 7374 5f70 6174  ef find_best_pat
-00017fa0: 685f 666f 725f 616d 6f75 6e74 5f69 6e28  h_for_amount_in(
-00017fb0: 5f77 6562 333a 5765 6233 2c5f 7175 6f74  _web3:Web3,_quot
-00017fc0: 655f 6164 6472 6573 732c 5f71 756f 7465  e_address,_quote
-00017fd0: 5f61 6269 2c5f 7061 7468 2c5f 616d 6f75  _abi,_path,_amou
-00017fe0: 6e74 5f69 6e29 3a0a 2020 2020 2020 2020  nt_in):.        
-00017ff0: 7265 7475 726e 205f 7765 6233 2e65 7468  return _web3.eth
-00018000: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
-00018010: 733d 5f71 756f 7465 5f61 6464 7265 7373  s=_quote_address
-00018020: 2c61 6269 3d5f 7175 6f74 655f 6162 6929  ,abi=_quote_abi)
-00018030: 2e66 756e 6374 696f 6e73 2e66 696e 6442  .functions.findB
-00018040: 6573 7450 6174 6846 726f 6d41 6d6f 756e  estPathFromAmoun
-00018050: 7449 6e28 5f70 6174 682c 5f61 6d6f 756e  tIn(_path,_amoun
-00018060: 745f 696e 292e 6361 6c6c 2829 0a20 2020  t_in).call().   
-00018070: 2023 7265 7475 726e 2071 756f 7465 0a20   #return quote. 
-00018080: 2020 2023 2020 2020 7374 7275 6374 2051     #    struct Q
-00018090: 756f 7465 207b 0a20 2020 2023 2020 2020  uote {.    #    
-000180a0: 2061 6464 7265 7373 5b5d 2072 6f75 7465   address[] route
-000180b0: 3b20 6f75 7420 746f 6b65 6ee5 9ca8 e589  ; out token.....
-000180c0: 8d0a 2020 2020 2320 2020 2020 6164 6472  ..    #     addr
-000180d0: 6573 735b 5d20 7061 6972 733b 0a20 2020  ess[] pairs;.   
-000180e0: 2023 2020 2020 2075 696e 7432 3536 5b5d   #     uint256[]
-000180f0: 2062 696e 5374 6570 733b 0a20 2020 2023   binSteps;.    #
-00018100: 2020 2020 2075 696e 7432 3536 5b5d 2061       uint256[] a
-00018110: 6d6f 756e 7473 3b0a 2020 2020 2320 2020  mounts;.    #   
-00018120: 2020 7569 6e74 3235 365b 5d20 7669 7274    uint256[] virt
-00018130: 7561 6c41 6d6f 756e 7473 5769 7468 6f75  ualAmountsWithou
-00018140: 7453 6c69 7070 6167 653b 0a20 2020 2023  tSlippage;.    #
-00018150: 2020 2020 2075 696e 7432 3536 5b5d 2066       uint256[] f
-00018160: 6565 733b 0a20 2020 2023 207d 0a20 2020  ees;.    # }.   
-00018170: 2064 6566 2066 696e 645f 6265 7374 5f70   def find_best_p
-00018180: 6174 685f 666f 725f 616d 6f75 6e74 5f6f  ath_for_amount_o
-00018190: 7574 285f 7765 6233 3a57 6562 332c 5f71  ut(_web3:Web3,_q
-000181a0: 756f 7465 5f61 6464 7265 7373 2c5f 7175  uote_address,_qu
-000181b0: 6f74 655f 6162 692c 5f70 6174 682c 5f61  ote_abi,_path,_a
-000181c0: 6d6f 756e 745f 6f75 7429 3a0a 2020 2020  mount_out):.    
-000181d0: 2020 2020 7265 7475 726e 205f 7765 6233      return _web3
-000181e0: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
-000181f0: 6472 6573 733d 5f71 756f 7465 5f61 6464  dress=_quote_add
-00018200: 7265 7373 2c61 6269 3d5f 7175 6f74 655f  ress,abi=_quote_
-00018210: 6162 6929 2e66 756e 6374 696f 6e73 2e66  abi).functions.f
-00018220: 696e 6442 6573 7450 6174 6846 726f 6d41  indBestPathFromA
-00018230: 6d6f 756e 7449 6e28 5f70 6174 682c 5f61  mountIn(_path,_a
-00018240: 6d6f 756e 745f 6f75 7429 2e63 616c 6c28  mount_out).call(
-00018250: 290a 0a0a 636c 6173 7320 4a6f 6556 3245  )...class JoeV2E
-00018260: 7263 3230 3a0a 2020 2020 6a6f 655f 6572  rc20:.    joe_er
-00018270: 6332 305f 6162 693d 275b 207b 2022 616e  c20_abi='[ { "an
-00018280: 6f6e 796d 6f75 7322 3a20 6661 6c73 652c  onymous": false,
-00018290: 2022 696e 7075 7473 223a 205b 207b 2022   "inputs": [ { "
-000182a0: 696e 6465 7865 6422 3a20 7472 7565 2c20  indexed": true, 
-000182b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-000182c0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
-000182d0: 223a 2022 6f77 6e65 7222 2c20 2274 7970  ": "owner", "typ
-000182e0: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
-000182f0: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
-00018300: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
-00018310: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-00018320: 6e61 6d65 223a 2022 7370 656e 6465 7222  name": "spender"
-00018330: 2c20 2274 7970 6522 3a20 2261 6464 7265  , "type": "addre
-00018340: 7373 2220 7d2c 207b 2022 696e 6465 7865  ss" }, { "indexe
-00018350: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
-00018360: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-00018370: 3235 3622 2c20 226e 616d 6522 3a20 2276  256", "name": "v
-00018380: 616c 7565 222c 2022 7479 7065 223a 2022  alue", "type": "
-00018390: 7569 6e74 3235 3622 207d 205d 2c20 226e  uint256" } ], "n
-000183a0: 616d 6522 3a20 2241 7070 726f 7661 6c22  ame": "Approval"
-000183b0: 2c20 2274 7970 6522 3a20 2265 7665 6e74  , "type": "event
-000183c0: 2220 7d2c 207b 2022 616e 6f6e 796d 6f75  " }, { "anonymou
-000183d0: 7322 3a20 6661 6c73 652c 2022 696e 7075  s": false, "inpu
-000183e0: 7473 223a 205b 207b 2022 696e 6465 7865  ts": [ { "indexe
-000183f0: 6422 3a20 7472 7565 2c20 2269 6e74 6572  d": true, "inter
-00018400: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-00018410: 7373 222c 2022 6e61 6d65 223a 2022 6672  ss", "name": "fr
-00018420: 6f6d 222c 2022 7479 7065 223a 2022 6164  om", "type": "ad
-00018430: 6472 6573 7322 207d 2c20 7b20 2269 6e64  dress" }, { "ind
-00018440: 6578 6564 223a 2074 7275 652c 2022 696e  exed": true, "in
-00018450: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-00018460: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-00018470: 2274 6f22 2c20 2274 7970 6522 3a20 2261  "to", "type": "a
-00018480: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-00018490: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
-000184a0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-000184b0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-000184c0: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
-000184d0: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
-000184e0: 2c20 226e 616d 6522 3a20 2254 7261 6e73  , "name": "Trans
-000184f0: 6665 7222 2c20 2274 7970 6522 3a20 2265  fer", "type": "e
-00018500: 7665 6e74 2220 7d2c 207b 2022 696e 7075  vent" }, { "inpu
-00018510: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-00018520: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
-00018530: 7322 2c20 226e 616d 6522 3a20 226f 776e  s", "name": "own
-00018540: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
-00018550: 6472 6573 7322 207d 2c20 7b20 2269 6e74  dress" }, { "int
-00018560: 6572 6e61 6c54 7970 6522 3a20 2261 6464  ernalType": "add
-00018570: 7265 7373 222c 2022 6e61 6d65 223a 2022  ress", "name": "
-00018580: 7370 656e 6465 7222 2c20 2274 7970 6522  spender", "type"
-00018590: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-000185a0: 2022 6e61 6d65 223a 2022 616c 6c6f 7761   "name": "allowa
-000185b0: 6e63 6522 2c20 226f 7574 7075 7473 223a  nce", "outputs":
-000185c0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-000185d0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-000185e0: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-000185f0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-00018600: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-00018610: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-00018620: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-00018630: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-00018640: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-00018650: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-00018660: 6e61 6d65 223a 2022 7370 656e 6465 7222  name": "spender"
-00018670: 2c20 2274 7970 6522 3a20 2261 6464 7265  , "type": "addre
-00018680: 7373 2220 7d2c 207b 2022 696e 7465 726e  ss" }, { "intern
-00018690: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-000186a0: 3622 2c20 226e 616d 6522 3a20 2276 616c  6", "name": "val
-000186b0: 7565 222c 2022 7479 7065 223a 2022 7569  ue", "type": "ui
-000186c0: 6e74 3235 3622 207d 205d 2c20 226e 616d  nt256" } ], "nam
-000186d0: 6522 3a20 2261 7070 726f 7665 222c 2022  e": "approve", "
-000186e0: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
-000186f0: 6e74 6572 6e61 6c54 7970 6522 3a20 2262  nternalType": "b
-00018700: 6f6f 6c22 2c20 226e 616d 6522 3a20 2222  ool", "name": ""
-00018710: 2c20 2274 7970 6522 3a20 2262 6f6f 6c22  , "type": "bool"
-00018720: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-00018730: 6269 6c69 7479 223a 2022 6e6f 6e70 6179  bility": "nonpay
-00018740: 6162 6c65 222c 2022 7479 7065 223a 2022  able", "type": "
-00018750: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-00018760: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
-00018770: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-00018780: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-00018790: 226f 776e 6572 222c 2022 7479 7065 223a  "owner", "type":
-000187a0: 2022 6164 6472 6573 7322 207d 205d 2c20   "address" } ], 
-000187b0: 226e 616d 6522 3a20 2262 616c 616e 6365  "name": "balance
-000187c0: 4f66 222c 2022 6f75 7470 7574 7322 3a20  Of", "outputs": 
-000187d0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-000187e0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
-000187f0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-00018800: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
-00018810: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-00018820: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-00018830: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-00018840: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-00018850: 5d2c 2022 6e61 6d65 223a 2022 6465 6369  ], "name": "deci
-00018860: 6d61 6c73 222c 2022 6f75 7470 7574 7322  mals", "outputs"
-00018870: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-00018880: 7970 6522 3a20 2275 696e 7438 222c 2022  ype": "uint8", "
-00018890: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-000188a0: 223a 2022 7569 6e74 3822 207d 205d 2c20  ": "uint8" } ], 
-000188b0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-000188c0: 223a 2022 7669 6577 222c 2022 7479 7065  ": "view", "type
-000188d0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
-000188e0: 207b 2022 696e 7075 7473 223a 205b 5d2c   { "inputs": [],
-000188f0: 2022 6e61 6d65 223a 2022 6e61 6d65 222c   "name": "name",
-00018900: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
-00018910: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-00018920: 2273 7472 696e 6722 2c20 226e 616d 6522  "string", "name"
-00018930: 3a20 2222 2c20 2274 7970 6522 3a20 2273  : "", "type": "s
-00018940: 7472 696e 6722 207d 205d 2c20 2273 7461  tring" } ], "sta
-00018950: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
-00018960: 7669 6577 222c 2022 7479 7065 223a 2022  view", "type": "
-00018970: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-00018980: 696e 7075 7473 223a 205b 5d2c 2022 6e61  inputs": [], "na
-00018990: 6d65 223a 2022 7379 6d62 6f6c 222c 2022  me": "symbol", "
-000189a0: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
-000189b0: 6e74 6572 6e61 6c54 7970 6522 3a20 2273  nternalType": "s
-000189c0: 7472 696e 6722 2c20 226e 616d 6522 3a20  tring", "name": 
-000189d0: 2222 2c20 2274 7970 6522 3a20 2273 7472  "", "type": "str
-000189e0: 696e 6722 207d 205d 2c20 2273 7461 7465  ing" } ], "state
-000189f0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
-00018a00: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
-00018a10: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-00018a20: 7075 7473 223a 205b 5d2c 2022 6e61 6d65  puts": [], "name
-00018a30: 223a 2022 746f 7461 6c53 7570 706c 7922  ": "totalSupply"
-00018a40: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-00018a50: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-00018a60: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-00018a70: 6522 3a20 2222 2c20 2274 7970 6522 3a20  e": "", "type": 
-00018a80: 2275 696e 7432 3536 2220 7d20 5d2c 2022  "uint256" } ], "
-00018a90: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00018aa0: 3a20 2276 6965 7722 2c20 2274 7970 6522  : "view", "type"
-00018ab0: 3a20 2266 756e 6374 696f 6e22 207d 2c20  : "function" }, 
-00018ac0: 7b20 2269 6e70 7574 7322 3a20 5b20 7b20  { "inputs": [ { 
-00018ad0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-00018ae0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
-00018af0: 223a 2022 746f 222c 2022 7479 7065 223a  ": "to", "type":
-00018b00: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
-00018b10: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-00018b20: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
-00018b30: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
-00018b40: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-00018b50: 5d2c 2022 6e61 6d65 223a 2022 7472 616e  ], "name": "tran
-00018b60: 7366 6572 222c 2022 6f75 7470 7574 7322  sfer", "outputs"
-00018b70: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-00018b80: 7970 6522 3a20 2262 6f6f 6c22 2c20 226e  ype": "bool", "n
-00018b90: 616d 6522 3a20 2222 2c20 2274 7970 6522  ame": "", "type"
-00018ba0: 3a20 2262 6f6f 6c22 207d 205d 2c20 2273  : "bool" } ], "s
-00018bb0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00018bc0: 2022 6e6f 6e70 6179 6162 6c65 222c 2022   "nonpayable", "
-00018bd0: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-00018be0: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-00018bf0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-00018c00: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-00018c10: 226e 616d 6522 3a20 2266 726f 6d22 2c20  "name": "from", 
-00018c20: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-00018c30: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-00018c40: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-00018c50: 2c20 226e 616d 6522 3a20 2274 6f22 2c20  , "name": "to", 
-00018c60: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-00018c70: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-00018c80: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
-00018c90: 2c20 226e 616d 6522 3a20 2276 616c 7565  , "name": "value
-00018ca0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-00018cb0: 3235 3622 207d 205d 2c20 226e 616d 6522  256" } ], "name"
-00018cc0: 3a20 2274 7261 6e73 6665 7246 726f 6d22  : "transferFrom"
-00018cd0: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-00018ce0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-00018cf0: 2022 626f 6f6c 222c 2022 6e61 6d65 223a   "bool", "name":
-00018d00: 2022 222c 2022 7479 7065 223a 2022 626f   "", "type": "bo
-00018d10: 6f6c 2220 7d20 5d2c 2022 7374 6174 654d  ol" } ], "stateM
-00018d20: 7574 6162 696c 6974 7922 3a20 226e 6f6e  utability": "non
-00018d30: 7061 7961 626c 6522 2c20 2274 7970 6522  payable", "type"
-00018d40: 3a20 2266 756e 6374 696f 6e22 207d 205d  : "function" } ]
-00018d50: 2720 200a 0a63 6c61 7373 204a 6f65 5632  '  ..class JoeV2
-00018d60: 526f 7574 653a 0a20 2020 206a 6f65 5f72  Route:.    joe_r
-00018d70: 6f75 7465 5f76 325f 6162 693d 6a73 6f6e  oute_v2_abi=json
-00018d80: 2e6c 6f61 6473 2827 5b7b 2269 6e70 7574  .loads('[{"input
-00018d90: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00018da0: 7065 223a 2263 6f6e 7472 6163 7420 494c  pe":"contract IL
-00018db0: 4246 6163 746f 7279 222c 226e 616d 6522  BFactory","name"
-00018dc0: 3a22 5f66 6163 746f 7279 222c 2274 7970  :"_factory","typ
-00018dd0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00018de0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-00018df0: 6f6e 7472 6163 7420 494a 6f65 4661 6374  ontract IJoeFact
-00018e00: 6f72 7922 2c22 6e61 6d65 223a 225f 6f6c  ory","name":"_ol
-00018e10: 6446 6163 746f 7279 222c 2274 7970 6522  dFactory","type"
-00018e20: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-00018e30: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-00018e40: 7472 6163 7420 4957 4156 4158 222c 226e  tract IWAVAX","n
-00018e50: 616d 6522 3a22 5f77 6176 6178 222c 2274  ame":"_wavax","t
-00018e60: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-00018e70: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00018e80: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
-00018e90: 2274 7970 6522 3a22 636f 6e73 7472 7563  "type":"construc
-00018ea0: 746f 7222 7d2c 7b22 696e 7075 7473 223a  tor"},{"inputs":
-00018eb0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00018ec0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00018ed0: 223a 2262 7022 2c22 7479 7065 223a 2275  ":"bp","type":"u
-00018ee0: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00018ef0: 3a22 4269 6e48 656c 7065 725f 5f42 696e  :"BinHelper__Bin
-00018f00: 5374 6570 4f76 6572 666c 6f77 7322 2c22  StepOverflows","
-00018f10: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00018f20: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00018f30: 6522 3a22 4269 6e48 656c 7065 725f 5f49  e":"BinHelper__I
-00018f40: 644f 7665 7266 6c6f 7773 222c 2274 7970  dOverflows","typ
-00018f50: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-00018f60: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-00018f70: 224a 6f65 4c69 6272 6172 795f 5f49 6e73  "JoeLibrary__Ins
-00018f80: 7566 6669 6369 656e 7441 6d6f 756e 7422  ufficientAmount"
-00018f90: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00018fa0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00018fb0: 616d 6522 3a22 4a6f 654c 6962 7261 7279  ame":"JoeLibrary
-00018fc0: 5f5f 496e 7375 6666 6963 6965 6e74 4c69  __InsufficientLi
-00018fd0: 7175 6964 6974 7922 2c22 7479 7065 223a  quidity","type":
-00018fe0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00018ff0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00019000: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019010: 616d 6522 3a22 616d 6f75 6e74 584d 696e  ame":"amountXMin
-00019020: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00019030: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00019040: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019050: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
-00019060: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00019070: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00019080: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00019090: 223a 2261 6d6f 756e 7459 4d69 6e22 2c22  ":"amountYMin","
-000190a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-000190b0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000190c0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-000190d0: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
-000190e0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-000190f0: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
-00019100: 5f41 6d6f 756e 7453 6c69 7070 6167 6543  _AmountSlippageC
-00019110: 6175 6768 7422 2c22 7479 7065 223a 2265  aught","type":"e
-00019120: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00019130: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00019140: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00019150: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
-00019160: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00019170: 223a 224c 4252 6f75 7465 725f 5f42 696e  ":"LBRouter__Bin
-00019180: 5265 7365 7276 654f 7665 7266 6c6f 7773  ReserveOverflows
-00019190: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-000191a0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-000191b0: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
-000191c0: 5f42 726f 6b65 6e53 7761 7053 6166 6574  _BrokenSwapSafet
-000191d0: 7943 6865 636b 222c 2274 7970 6522 3a22  yCheck","type":"
-000191e0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-000191f0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019200: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00019210: 6d65 223a 2264 6561 646c 696e 6522 2c22  me":"deadline","
-00019220: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00019230: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00019240: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00019250: 223a 2263 7572 7265 6e74 5469 6d65 7374  ":"currentTimest
-00019260: 616d 7022 2c22 7479 7065 223a 2275 696e  amp","type":"uin
-00019270: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00019280: 4c42 526f 7574 6572 5f5f 4465 6164 6c69  LBRouter__Deadli
-00019290: 6e65 4578 6365 6564 6564 222c 2274 7970  neExceeded","typ
-000192a0: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-000192b0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000192c0: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-000192d0: 2c22 6e61 6d65 223a 2272 6563 6970 6965  ,"name":"recipie
-000192e0: 6e74 222c 2274 7970 6522 3a22 6164 6472  nt","type":"addr
-000192f0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-00019300: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00019310: 226e 616d 6522 3a22 616d 6f75 6e74 222c  "name":"amount",
-00019320: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00019330: 7d5d 2c22 6e61 6d65 223a 224c 4252 6f75  }],"name":"LBRou
-00019340: 7465 725f 5f46 6169 6c65 6454 6f53 656e  ter__FailedToSen
-00019350: 6441 5641 5822 2c22 7479 7065 223a 2265  dAVAX","type":"e
-00019360: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00019370: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00019380: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00019390: 6522 3a22 6964 4465 7369 7265 6422 2c22  e":"idDesired","
-000193a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-000193b0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000193c0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-000193d0: 223a 2269 6453 6c69 7070 6167 6522 2c22  ":"idSlippage","
-000193e0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-000193f0: 5d2c 226e 616d 6522 3a22 4c42 526f 7574  ],"name":"LBRout
-00019400: 6572 5f5f 4964 4465 7369 7265 644f 7665  er__IdDesiredOve
-00019410: 7266 6c6f 7773 222c 2274 7970 6522 3a22  rflows","type":"
-00019420: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019430: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019440: 6522 3a22 696e 7432 3536 222c 226e 616d  e":"int256","nam
-00019450: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
-00019460: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00019470: 3a22 4c42 526f 7574 6572 5f5f 4964 4f76  :"LBRouter__IdOv
-00019480: 6572 666c 6f77 7322 2c22 7479 7065 223a  erflows","type":
-00019490: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-000194a0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-000194b0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-000194c0: 616d 6522 3a22 6163 7469 7665 4964 4465  ame":"activeIdDe
-000194d0: 7369 7265 6422 2c22 7479 7065 223a 2275  sired","type":"u
-000194e0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-000194f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00019500: 3622 2c22 6e61 6d65 223a 2269 6453 6c69  6","name":"idSli
-00019510: 7070 6167 6522 2c22 7479 7065 223a 2275  ppage","type":"u
-00019520: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00019530: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00019540: 3622 2c22 6e61 6d65 223a 2261 6374 6976  6","name":"activ
-00019550: 6549 6422 2c22 7479 7065 223a 2275 696e  eId","type":"uin
-00019560: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00019570: 4c42 526f 7574 6572 5f5f 4964 536c 6970  LBRouter__IdSlip
-00019580: 7061 6765 4361 7567 6874 222c 2274 7970  pageCaught","typ
-00019590: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-000195a0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000195b0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-000195c0: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
-000195d0: 7574 4d69 6e22 2c22 7479 7065 223a 2275  utMin","type":"u
-000195e0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-000195f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00019600: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-00019610: 744f 7574 222c 2274 7970 6522 3a22 7569  tOut","type":"ui
-00019620: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00019630: 224c 4252 6f75 7465 725f 5f49 6e73 7566  "LBRouter__Insuf
-00019640: 6669 6369 656e 7441 6d6f 756e 744f 7574  ficientAmountOut
-00019650: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00019660: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00019670: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-00019680: 6472 6573 7322 2c22 6e61 6d65 223a 2277  dress","name":"w
-00019690: 726f 6e67 546f 6b65 6e22 2c22 7479 7065  rongToken","type
-000196a0: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
-000196b0: 616d 6522 3a22 4c42 526f 7574 6572 5f5f  ame":"LBRouter__
-000196c0: 496e 7661 6c69 6454 6f6b 656e 5061 7468  InvalidTokenPath
-000196d0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-000196e0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-000196f0: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
-00019700: 5f4c 656e 6774 6873 4d69 736d 6174 6368  _LengthsMismatch
-00019710: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00019720: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00019730: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00019740: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-00019750: 6d6f 756e 7449 6e4d 6178 222c 2274 7970  mountInMax","typ
-00019760: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00019770: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00019780: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00019790: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
-000197a0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-000197b0: 6d65 223a 224c 4252 6f75 7465 725f 5f4d  me":"LBRouter__M
-000197c0: 6178 416d 6f75 6e74 496e 4578 6365 6564  axAmountInExceed
-000197d0: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
-000197e0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-000197f0: 2c22 6e61 6d65 223a 224c 4252 6f75 7465  ,"name":"LBRoute
-00019800: 725f 5f4e 6f74 4661 6374 6f72 794f 776e  r__NotFactoryOwn
-00019810: 6572 222c 2274 7970 6522 3a22 6572 726f  er","type":"erro
-00019820: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-00019830: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00019840: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00019850: 2274 6f6b 656e 5822 2c22 7479 7065 223a  "tokenX","type":
-00019860: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-00019870: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00019880: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-00019890: 656e 5922 2c22 7479 7065 223a 2261 6464  enY","type":"add
-000198a0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-000198b0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-000198c0: 2c22 6e61 6d65 223a 2262 696e 5374 6570  ,"name":"binStep
-000198d0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-000198e0: 3622 7d5d 2c22 6e61 6d65 223a 224c 4252  6"}],"name":"LBR
-000198f0: 6f75 7465 725f 5f50 6169 724e 6f74 4372  outer__PairNotCr
-00019900: 6561 7465 6422 2c22 7479 7065 223a 2265  eated","type":"e
-00019910: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00019920: 3a5b 5d2c 226e 616d 6522 3a22 4c42 526f  :[],"name":"LBRo
-00019930: 7574 6572 5f5f 5365 6e64 6572 4973 4e6f  uter__SenderIsNo
-00019940: 7457 4156 4158 222c 2274 7970 6522 3a22  tWAVAX","type":"
-00019950: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019960: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019970: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00019980: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
-00019990: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-000199a0: 6522 3a22 4c42 526f 7574 6572 5f5f 5377  e":"LBRouter__Sw
-000199b0: 6170 4f76 6572 666c 6f77 7322 2c22 7479  apOverflows","ty
-000199c0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-000199d0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-000199e0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000199f0: 222c 226e 616d 6522 3a22 6578 6365 7373  ","name":"excess
-00019a00: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00019a10: 3622 7d5d 2c22 6e61 6d65 223a 224c 4252  6"}],"name":"LBR
-00019a20: 6f75 7465 725f 5f54 6f6f 4d75 6368 546f  outer__TooMuchTo
-00019a30: 6b65 6e73 496e 222c 2274 7970 6522 3a22  kensIn","type":"
-00019a40: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019a50: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019a60: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00019a70: 6d65 223a 2261 6d6f 756e 7422 2c22 7479  me":"amount","ty
-00019a80: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00019a90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00019aa0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00019ab0: 2272 6573 6572 7665 222c 2274 7970 6522  "reserve","type"
-00019ac0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00019ad0: 6d65 223a 224c 4252 6f75 7465 725f 5f57  me":"LBRouter__W
-00019ae0: 726f 6e67 416d 6f75 6e74 7322 2c22 7479  rongAmounts","ty
-00019af0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00019b00: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00019b10: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00019b20: 222c 226e 616d 6522 3a22 746f 6b65 6e58  ","name":"tokenX
-00019b30: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00019b40: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00019b50: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-00019b60: 616d 6522 3a22 746f 6b65 6e59 222c 2274  ame":"tokenY","t
-00019b70: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-00019b80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00019b90: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00019ba0: 3a22 616d 6f75 6e74 5822 2c22 7479 7065  :"amountX","type
-00019bb0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00019bc0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00019bd0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-00019be0: 6d6f 756e 7459 222c 2274 7970 6522 3a22  mountY","type":"
-00019bf0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00019c00: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00019c10: 3536 222c 226e 616d 6522 3a22 6d73 6756  56","name":"msgV
-00019c20: 616c 7565 222c 2274 7970 6522 3a22 7569  alue","type":"ui
-00019c30: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00019c40: 224c 4252 6f75 7465 725f 5f57 726f 6e67  "LBRouter__Wrong
-00019c50: 4176 6178 4c69 7175 6964 6974 7950 6172  AvaxLiquidityPar
-00019c60: 616d 6574 6572 7322 2c22 7479 7065 223a  ameters","type":
-00019c70: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019c80: 7322 3a5b 5d2c 226e 616d 6522 3a22 4c42  s":[],"name":"LB
-00019c90: 526f 7574 6572 5f5f 5772 6f6e 6754 6f6b  Router__WrongTok
-00019ca0: 656e 4f72 6465 7222 2c22 7479 7065 223a  enOrder","type":
-00019cb0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019cc0: 7322 3a5b 5d2c 226e 616d 6522 3a22 4d61  s":[],"name":"Ma
-00019cd0: 7468 3132 3878 3132 385f 5f4c 6f67 556e  th128x128__LogUn
-00019ce0: 6465 7266 6c6f 7722 2c22 7479 7065 223a  derflow","type":
-00019cf0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019d00: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00019d10: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019d20: 616d 6522 3a22 7822 2c22 7479 7065 223a  ame":"x","type":
-00019d30: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00019d40: 6572 6e61 6c54 7970 6522 3a22 696e 7432  ernalType":"int2
-00019d50: 3536 222c 226e 616d 6522 3a22 7922 2c22  56","name":"y","
-00019d60: 7479 7065 223a 2269 6e74 3235 3622 7d5d  type":"int256"}]
-00019d70: 2c22 6e61 6d65 223a 224d 6174 6831 3238  ,"name":"Math128
-00019d80: 7831 3238 5f5f 506f 7765 7255 6e64 6572  x128__PowerUnder
-00019d90: 666c 6f77 222c 2274 7970 6522 3a22 6572  flow","type":"er
-00019da0: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-00019db0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00019dc0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00019dd0: 223a 2270 726f 6431 222c 2274 7970 6522  ":"prod1","type"
-00019de0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00019df0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00019e00: 7432 3536 222c 226e 616d 6522 3a22 6465  t256","name":"de
-00019e10: 6e6f 6d69 6e61 746f 7222 2c22 7479 7065  nominator","type
-00019e20: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00019e30: 616d 6522 3a22 4d61 7468 3531 3242 6974  ame":"Math512Bit
-00019e40: 735f 5f4d 756c 4469 764f 7665 7266 6c6f  s__MulDivOverflo
-00019e50: 7722 2c22 7479 7065 223a 2265 7272 6f72  w","type":"error
-00019e60: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00019e70: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00019e80: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00019e90: 7072 6f64 3122 2c22 7479 7065 223a 2275  prod1","type":"u
-00019ea0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00019eb0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00019ec0: 3622 2c22 6e61 6d65 223a 226f 6666 7365  6","name":"offse
-00019ed0: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-00019ee0: 3536 227d 5d2c 226e 616d 6522 3a22 4d61  56"}],"name":"Ma
-00019ef0: 7468 3531 3242 6974 735f 5f4d 756c 5368  th512Bits__MulSh
-00019f00: 6966 744f 7665 7266 6c6f 7722 2c22 7479  iftOverflow","ty
-00019f10: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00019f20: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00019f30: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00019f40: 222c 226e 616d 6522 3a22 6f66 6673 6574  ","name":"offset
-00019f50: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00019f60: 3622 7d5d 2c22 6e61 6d65 223a 224d 6174  6"}],"name":"Mat
-00019f70: 6835 3132 4269 7473 5f5f 4f66 6673 6574  h512Bits__Offset
-00019f80: 4f76 6572 666c 6f77 7322 2c22 7479 7065  Overflows","type
-00019f90: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-00019fa0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00019fb0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00019fc0: 226e 616d 6522 3a22 7822 2c22 7479 7065  "name":"x","type
-00019fd0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00019fe0: 616d 6522 3a22 5361 6665 4361 7374 5f5f  ame":"SafeCast__
-00019ff0: 4578 6365 6564 7331 3238 4269 7473 222c  Exceeds128Bits",
-0001a000: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001a010: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001a020: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001a030: 3235 3622 2c22 6e61 6d65 223a 2278 222c  256","name":"x",
-0001a040: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001a050: 7d5d 2c22 6e61 6d65 223a 2253 6166 6543  }],"name":"SafeC
-0001a060: 6173 745f 5f45 7863 6565 6473 3430 4269  ast__Exceeds40Bi
-0001a070: 7473 222c 2274 7970 6522 3a22 6572 726f  ts","type":"erro
-0001a080: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0001a090: 2c22 6e61 6d65 223a 2254 6f6b 656e 4865  ,"name":"TokenHe
-0001a0a0: 6c70 6572 5f5f 4361 6c6c 4661 696c 6564  lper__CallFailed
-0001a0b0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001a0c0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001a0d0: 6e61 6d65 223a 2254 6f6b 656e 4865 6c70  name":"TokenHelp
-0001a0e0: 6572 5f5f 4e6f 6e43 6f6e 7472 6163 7422  er__NonContract"
-0001a0f0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001a100: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001a110: 616d 6522 3a22 546f 6b65 6e48 656c 7065  ame":"TokenHelpe
-0001a120: 725f 5f54 7261 6e73 6665 7246 6169 6c65  r__TransferFaile
-0001a130: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
-0001a140: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001a150: 636f 6d70 6f6e 656e 7473 223a 5b7b 2269  components":[{"i
-0001a160: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-0001a170: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
-0001a180: 6e61 6d65 223a 2274 6f6b 656e 5822 2c22  name":"tokenX","
-0001a190: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001a1a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a1b0: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
-0001a1c0: 3022 2c22 6e61 6d65 223a 2274 6f6b 656e  0","name":"token
-0001a1d0: 5922 2c22 7479 7065 223a 2261 6464 7265  Y","type":"addre
-0001a1e0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0001a1f0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001a200: 6e61 6d65 223a 2262 696e 5374 6570 222c  name":"binStep",
-0001a210: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001a220: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a230: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001a240: 6522 3a22 616d 6f75 6e74 5822 2c22 7479  e":"amountX","ty
-0001a250: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0001a260: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001a270: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001a280: 2261 6d6f 756e 7459 222c 2274 7970 6522  "amountY","type"
-0001a290: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001a2a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001a2b0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0001a2c0: 6f75 6e74 584d 696e 222c 2274 7970 6522  ountXMin","type"
-0001a2d0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001a2e0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001a2f0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0001a300: 6f75 6e74 594d 696e 222c 2274 7970 6522  ountYMin","type"
-0001a310: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001a320: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001a330: 7432 3536 222c 226e 616d 6522 3a22 6163  t256","name":"ac
-0001a340: 7469 7665 4964 4465 7369 7265 6422 2c22  tiveIdDesired","
-0001a350: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001a360: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a370: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001a380: 223a 2269 6453 6c69 7070 6167 6522 2c22  ":"idSlippage","
-0001a390: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001a3a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a3b0: 3a22 696e 7432 3536 5b5d 222c 226e 616d  :"int256[]","nam
-0001a3c0: 6522 3a22 6465 6c74 6149 6473 222c 2274  e":"deltaIds","t
-0001a3d0: 7970 6522 3a22 696e 7432 3536 5b5d 227d  ype":"int256[]"}
-0001a3e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a3f0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-0001a400: 6d65 223a 2264 6973 7472 6962 7574 696f  me":"distributio
-0001a410: 6e58 222c 2274 7970 6522 3a22 7569 6e74  nX","type":"uint
-0001a420: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
-0001a430: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001a440: 5b5d 222c 226e 616d 6522 3a22 6469 7374  []","name":"dist
-0001a450: 7269 6275 7469 6f6e 5922 2c22 7479 7065  ributionY","type
-0001a460: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
-0001a470: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001a480: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001a490: 2274 6f22 2c22 7479 7065 223a 2261 6464  "to","type":"add
-0001a4a0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001a4b0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001a4c0: 2c22 6e61 6d65 223a 2264 6561 646c 696e  ,"name":"deadlin
-0001a4d0: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
-0001a4e0: 3536 227d 5d2c 2269 6e74 6572 6e61 6c54  56"}],"internalT
-0001a4f0: 7970 6522 3a22 7374 7275 6374 2049 4c42  ype":"struct ILB
-0001a500: 526f 7574 6572 2e4c 6971 7569 6469 7479  Router.Liquidity
-0001a510: 5061 7261 6d65 7465 7273 222c 226e 616d  Parameters","nam
-0001a520: 6522 3a22 5f6c 6971 7569 6469 7479 5061  e":"_liquidityPa
-0001a530: 7261 6d65 7465 7273 222c 2274 7970 6522  rameters","type"
-0001a540: 3a22 7475 706c 6522 7d5d 2c22 6e61 6d65  :"tuple"}],"name
-0001a550: 223a 2261 6464 4c69 7175 6964 6974 7922  ":"addLiquidity"
-0001a560: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-0001a570: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001a580: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-0001a590: 6465 706f 7369 7449 6473 222c 2274 7970  depositIds","typ
-0001a5a0: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-0001a5b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001a5c0: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
-0001a5d0: 6522 3a22 6c69 7175 6964 6974 794d 696e  e":"liquidityMin
-0001a5e0: 7465 6422 2c22 7479 7065 223a 2275 696e  ted","type":"uin
-0001a5f0: 7432 3536 5b5d 227d 5d2c 2273 7461 7465  t256[]"}],"state
-0001a600: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-0001a610: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-0001a620: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-0001a630: 7075 7473 223a 5b7b 2263 6f6d 706f 6e65  puts":[{"compone
-0001a640: 6e74 7322 3a5b 7b22 696e 7465 726e 616c  nts":[{"internal
-0001a650: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-0001a660: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-0001a670: 746f 6b65 6e58 222c 2274 7970 6522 3a22  tokenX","type":"
-0001a680: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-0001a690: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-0001a6a0: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-0001a6b0: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
-0001a6c0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001a6d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001a6e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001a6f0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-0001a700: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001a710: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001a720: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001a730: 756e 7458 222c 2274 7970 6522 3a22 7569  untX","type":"ui
-0001a740: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0001a750: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001a760: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-0001a770: 5922 2c22 7479 7065 223a 2275 696e 7432  Y","type":"uint2
-0001a780: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001a790: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001a7a0: 6e61 6d65 223a 2261 6d6f 756e 7458 4d69  name":"amountXMi
-0001a7b0: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001a7c0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001a7d0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001a7e0: 6e61 6d65 223a 2261 6d6f 756e 7459 4d69  name":"amountYMi
-0001a7f0: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001a800: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001a810: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001a820: 6e61 6d65 223a 2261 6374 6976 6549 6444  name":"activeIdD
-0001a830: 6573 6972 6564 222c 2274 7970 6522 3a22  esired","type":"
-0001a840: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001a850: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001a860: 3536 222c 226e 616d 6522 3a22 6964 536c  56","name":"idSl
-0001a870: 6970 7061 6765 222c 2274 7970 6522 3a22  ippage","type":"
-0001a880: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001a890: 726e 616c 5479 7065 223a 2269 6e74 3235  rnalType":"int25
-0001a8a0: 365b 5d22 2c22 6e61 6d65 223a 2264 656c  6[]","name":"del
-0001a8b0: 7461 4964 7322 2c22 7479 7065 223a 2269  taIds","type":"i
-0001a8c0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
-0001a8d0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001a8e0: 3536 5b5d 222c 226e 616d 6522 3a22 6469  56[]","name":"di
-0001a8f0: 7374 7269 6275 7469 6f6e 5822 2c22 7479  stributionX","ty
-0001a900: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
-0001a910: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a920: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-0001a930: 6d65 223a 2264 6973 7472 6962 7574 696f  me":"distributio
-0001a940: 6e59 222c 2274 7970 6522 3a22 7569 6e74  nY","type":"uint
-0001a950: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
-0001a960: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-0001a970: 222c 226e 616d 6522 3a22 746f 222c 2274  ","name":"to","t
-0001a980: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0001a990: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001a9a0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001a9b0: 3a22 6465 6164 6c69 6e65 222c 2274 7970  :"deadline","typ
-0001a9c0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001a9d0: 696e 7465 726e 616c 5479 7065 223a 2273  internalType":"s
-0001a9e0: 7472 7563 7420 494c 4252 6f75 7465 722e  truct ILBRouter.
-0001a9f0: 4c69 7175 6964 6974 7950 6172 616d 6574  LiquidityParamet
-0001aa00: 6572 7322 2c22 6e61 6d65 223a 225f 6c69  ers","name":"_li
-0001aa10: 7175 6964 6974 7950 6172 616d 6574 6572  quidityParameter
-0001aa20: 7322 2c22 7479 7065 223a 2274 7570 6c65  s","type":"tuple
-0001aa30: 227d 5d2c 226e 616d 6522 3a22 6164 644c  "}],"name":"addL
-0001aa40: 6971 7569 6469 7479 4156 4158 222c 226f  iquidityAVAX","o
-0001aa50: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-0001aa60: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001aa70: 365b 5d22 2c22 6e61 6d65 223a 2264 6570  6[]","name":"dep
-0001aa80: 6f73 6974 4964 7322 2c22 7479 7065 223a  ositIds","type":
-0001aa90: 2275 696e 7432 3536 5b5d 227d 2c7b 2269  "uint256[]"},{"i
-0001aaa0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001aab0: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-0001aac0: 226c 6971 7569 6469 7479 4d69 6e74 6564  "liquidityMinted
-0001aad0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001aae0: 365b 5d22 7d5d 2c22 7374 6174 654d 7574  6[]"}],"stateMut
-0001aaf0: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
-0001ab00: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-0001ab10: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001ab20: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001ab30: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
-0001ab40: 3022 2c22 6e61 6d65 223a 225f 746f 6b65  0","name":"_toke
-0001ab50: 6e58 222c 2274 7970 6522 3a22 6164 6472  nX","type":"addr
-0001ab60: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001ab70: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-0001ab80: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-0001ab90: 5f74 6f6b 656e 5922 2c22 7479 7065 223a  _tokenY","type":
-0001aba0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0001abb0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001abc0: 3234 222c 226e 616d 6522 3a22 5f61 6374  24","name":"_act
-0001abd0: 6976 6549 6422 2c22 7479 7065 223a 2275  iveId","type":"u
-0001abe0: 696e 7432 3422 7d2c 7b22 696e 7465 726e  int24"},{"intern
-0001abf0: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
-0001ac00: 2c22 6e61 6d65 223a 225f 6269 6e53 7465  ,"name":"_binSte
-0001ac10: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
-0001ac20: 3622 7d5d 2c22 6e61 6d65 223a 2263 7265  6"}],"name":"cre
-0001ac30: 6174 654c 4250 6169 7222 2c22 6f75 7470  ateLBPair","outp
-0001ac40: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001ac50: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-0001ac60: 494c 4250 6169 7222 2c22 6e61 6d65 223a  ILBPair","name":
-0001ac70: 2270 6169 7222 2c22 7479 7065 223a 2261  "pair","type":"a
-0001ac80: 6464 7265 7373 227d 5d2c 2273 7461 7465  ddress"}],"state
-0001ac90: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-0001aca0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-0001acb0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-0001acc0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001acd0: 2266 6163 746f 7279 222c 226f 7574 7075  "factory","outpu
-0001ace0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001acf0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-0001ad00: 4c42 4661 6374 6f72 7922 2c22 6e61 6d65  LBFactory","name
-0001ad10: 223a 2222 2c22 7479 7065 223a 2261 6464  ":"","type":"add
-0001ad20: 7265 7373 227d 5d2c 2273 7461 7465 4d75  ress"}],"stateMu
-0001ad30: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
-0001ad40: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-0001ad50: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-0001ad60: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001ad70: 636f 6e74 7261 6374 2049 4c42 5061 6972  contract ILBPair
-0001ad80: 222c 226e 616d 6522 3a22 5f4c 4250 6169  ","name":"_LBPai
-0001ad90: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-0001ada0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0001adb0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001adc0: 6e61 6d65 223a 225f 7072 6963 6522 2c22  name":"_price","
-0001add0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001ade0: 5d2c 226e 616d 6522 3a22 6765 7449 6446  ],"name":"getIdF
-0001adf0: 726f 6d50 7269 6365 222c 226f 7574 7075  romPrice","outpu
-0001ae00: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001ae10: 7970 6522 3a22 7569 6e74 3234 222c 226e  ype":"uint24","n
-0001ae20: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
-0001ae30: 7569 6e74 3234 227d 5d2c 2273 7461 7465  uint24"}],"state
-0001ae40: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-0001ae50: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-0001ae60: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001ae70: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001ae80: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
-0001ae90: 6972 222c 226e 616d 6522 3a22 5f4c 4250  ir","name":"_LBP
-0001aea0: 6169 7222 2c22 7479 7065 223a 2261 6464  air","type":"add
-0001aeb0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001aec0: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-0001aed0: 226e 616d 6522 3a22 5f69 6422 2c22 7479  "name":"_id","ty
-0001aee0: 7065 223a 2275 696e 7432 3422 7d5d 2c22  pe":"uint24"}],"
-0001aef0: 6e61 6d65 223a 2267 6574 5072 6963 6546  name":"getPriceF
-0001af00: 726f 6d49 6422 2c22 6f75 7470 7574 7322  romId","outputs"
-0001af10: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001af20: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001af30: 6522 3a22 222c 2274 7970 6522 3a22 7569  e":"","type":"ui
-0001af40: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-0001af50: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
-0001af60: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-0001af70: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-0001af80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001af90: 2263 6f6e 7472 6163 7420 494c 4250 6169  "contract ILBPai
-0001afa0: 7222 2c22 6e61 6d65 223a 225f 4c42 5061  r","name":"_LBPa
-0001afb0: 6972 222c 2274 7970 6522 3a22 6164 6472  ir","type":"addr
-0001afc0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001afd0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001afe0: 226e 616d 6522 3a22 5f61 6d6f 756e 744f  "name":"_amountO
-0001aff0: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
-0001b000: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001b010: 5479 7065 223a 2262 6f6f 6c22 2c22 6e61  Type":"bool","na
-0001b020: 6d65 223a 225f 7377 6170 466f 7259 222c  me":"_swapForY",
-0001b030: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-0001b040: 226e 616d 6522 3a22 6765 7453 7761 7049  "name":"getSwapI
-0001b050: 6e22 2c22 6f75 7470 7574 7322 3a5b 7b22  n","outputs":[{"
-0001b060: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b070: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001b080: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
-0001b090: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001b0a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001b0b0: 7432 3536 222c 226e 616d 6522 3a22 6665  t256","name":"fe
-0001b0c0: 6573 496e 222c 2274 7970 6522 3a22 7569  esIn","type":"ui
-0001b0d0: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-0001b0e0: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
-0001b0f0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-0001b100: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-0001b110: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001b120: 2263 6f6e 7472 6163 7420 494c 4250 6169  "contract ILBPai
-0001b130: 7222 2c22 6e61 6d65 223a 225f 4c42 5061  r","name":"_LBPa
-0001b140: 6972 222c 2274 7970 6522 3a22 6164 6472  ir","type":"addr
-0001b150: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001b160: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001b170: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
-0001b180: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001b190: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001b1a0: 7970 6522 3a22 626f 6f6c 222c 226e 616d  ype":"bool","nam
-0001b1b0: 6522 3a22 5f73 7761 7046 6f72 5922 2c22  e":"_swapForY","
-0001b1c0: 7479 7065 223a 2262 6f6f 6c22 7d5d 2c22  type":"bool"}],"
-0001b1d0: 6e61 6d65 223a 2267 6574 5377 6170 4f75  name":"getSwapOu
-0001b1e0: 7422 2c22 6f75 7470 7574 7322 3a5b 7b22  t","outputs":[{"
-0001b1f0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b200: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001b210: 616d 6f75 6e74 4f75 7422 2c22 7479 7065  amountOut","type
-0001b220: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001b230: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001b240: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
-0001b250: 6565 7349 6e22 2c22 7479 7065 223a 2275  eesIn","type":"u
-0001b260: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001b270: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-0001b280: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-0001b290: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001b2a0: 5b5d 2c22 6e61 6d65 223a 226f 6c64 4661  [],"name":"oldFa
-0001b2b0: 6374 6f72 7922 2c22 6f75 7470 7574 7322  ctory","outputs"
-0001b2c0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001b2d0: 223a 2263 6f6e 7472 6163 7420 494a 6f65  ":"contract IJoe
-0001b2e0: 4661 6374 6f72 7922 2c22 6e61 6d65 223a  Factory","name":
-0001b2f0: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-0001b300: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-0001b310: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-0001b320: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0001b330: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0001b340: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-0001b350: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
-0001b360: 6e61 6d65 223a 225f 746f 6b65 6e58 222c  name":"_tokenX",
-0001b370: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001b380: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001b390: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001b3a0: 3230 222c 226e 616d 6522 3a22 5f74 6f6b  20","name":"_tok
-0001b3b0: 656e 5922 2c22 7479 7065 223a 2261 6464  enY","type":"add
-0001b3c0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001b3d0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
-0001b3e0: 226e 616d 6522 3a22 5f62 696e 5374 6570  "name":"_binStep
-0001b3f0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-0001b400: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b410: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001b420: 6d65 223a 225f 616d 6f75 6e74 584d 696e  me":"_amountXMin
-0001b430: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001b440: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001b450: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001b460: 616d 6522 3a22 5f61 6d6f 756e 7459 4d69  ame":"_amountYMi
-0001b470: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001b480: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001b490: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001b4a0: 2c22 6e61 6d65 223a 225f 6964 7322 2c22  ,"name":"_ids","
-0001b4b0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-0001b4c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b4d0: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-0001b4e0: 6e61 6d65 223a 225f 616d 6f75 6e74 7322  name":"_amounts"
-0001b4f0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001b500: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
-0001b510: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001b520: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
-0001b530: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001b540: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b550: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001b560: 5f64 6561 646c 696e 6522 2c22 7479 7065  _deadline","type
-0001b570: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001b580: 616d 6522 3a22 7265 6d6f 7665 4c69 7175  ame":"removeLiqu
-0001b590: 6964 6974 7922 2c22 6f75 7470 7574 7322  idity","outputs"
-0001b5a0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001b5b0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001b5c0: 6522 3a22 616d 6f75 6e74 5822 2c22 7479  e":"amountX","ty
-0001b5d0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0001b5e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b5f0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001b600: 2261 6d6f 756e 7459 222c 2274 7970 6522  "amountY","type"
-0001b610: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
-0001b620: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-0001b630: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-0001b640: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-0001b650: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001b660: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-0001b670: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-0001b680: 6522 3a22 5f74 6f6b 656e 222c 2274 7970  e":"_token","typ
-0001b690: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001b6a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b6b0: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
-0001b6c0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-0001b6d0: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
-0001b6e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001b6f0: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
-0001b700: 756e 7454 6f6b 656e 4d69 6e22 2c22 7479  untTokenMin","ty
-0001b710: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0001b720: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b730: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001b740: 225f 616d 6f75 6e74 4156 4158 4d69 6e22  "_amountAVAXMin"
-0001b750: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001b760: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b770: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-0001b780: 6e61 6d65 223a 225f 6964 7322 2c22 7479  name":"_ids","ty
-0001b790: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
-0001b7a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001b7b0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-0001b7c0: 6d65 223a 225f 616d 6f75 6e74 7322 2c22  me":"_amounts","
-0001b7d0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-0001b7e0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b7f0: 6522 3a22 6164 6472 6573 7320 7061 7961  e":"address paya
-0001b800: 626c 6522 2c22 6e61 6d65 223a 225f 746f  ble","name":"_to
-0001b810: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001b820: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-0001b830: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001b840: 616d 6522 3a22 5f64 6561 646c 696e 6522  ame":"_deadline"
-0001b850: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001b860: 227d 5d2c 226e 616d 6522 3a22 7265 6d6f  "}],"name":"remo
-0001b870: 7665 4c69 7175 6964 6974 7941 5641 5822  veLiquidityAVAX"
-0001b880: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-0001b890: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001b8a0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0001b8b0: 6f75 6e74 546f 6b65 6e22 2c22 7479 7065  ountToken","type
-0001b8c0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001b8d0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001b8e0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0001b8f0: 6d6f 756e 7441 5641 5822 2c22 7479 7065  mountAVAX","type
-0001b900: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
-0001b910: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-0001b920: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
-0001b930: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0001b940: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001b950: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001b960: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
-0001b970: 6f75 6e74 4f75 7422 2c22 7479 7065 223a  ountOut","type":
-0001b980: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001b990: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001b9a0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-0001b9b0: 7061 6972 4269 6e53 7465 7073 222c 2274  pairBinSteps","t
-0001b9c0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001b9d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001b9e0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001b9f0: 3230 5b5d 222c 226e 616d 6522 3a22 5f74  20[]","name":"_t
-0001ba00: 6f6b 656e 5061 7468 222c 2274 7970 6522  okenPath","type"
-0001ba10: 3a22 6164 6472 6573 735b 5d22 7d2c 7b22  :"address[]"},{"
-0001ba20: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0001ba30: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0001ba40: 5f74 6f22 2c22 7479 7065 223a 2261 6464  _to","type":"add
-0001ba50: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001ba60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001ba70: 2c22 6e61 6d65 223a 225f 6465 6164 6c69  ,"name":"_deadli
-0001ba80: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
-0001ba90: 3235 3622 7d5d 2c22 6e61 6d65 223a 2273  256"}],"name":"s
-0001baa0: 7761 7041 5641 5846 6f72 4578 6163 7454  wapAVAXForExactT
-0001bab0: 6f6b 656e 7322 2c22 6f75 7470 7574 7322  okens","outputs"
-0001bac0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001bad0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-0001bae0: 616d 6522 3a22 616d 6f75 6e74 7349 6e22  ame":"amountsIn"
-0001baf0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001bb00: 5b5d 227d 5d2c 2273 7461 7465 4d75 7461  []"}],"stateMuta
-0001bb10: 6269 6c69 7479 223a 2270 6179 6162 6c65  bility":"payable
-0001bb20: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-0001bb30: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-0001bb40: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001bb50: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001bb60: 3a22 5f61 6d6f 756e 744f 7574 4d69 6e22  :"_amountOutMin"
-0001bb70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001bb80: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001bb90: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-0001bba0: 6e61 6d65 223a 225f 7061 6972 4269 6e53  name":"_pairBinS
-0001bbb0: 7465 7073 222c 2274 7970 6522 3a22 7569  teps","type":"ui
-0001bbc0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
-0001bbd0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-0001bbe0: 6163 7420 4945 5243 3230 5b5d 222c 226e  act IERC20[]","n
-0001bbf0: 616d 6522 3a22 5f74 6f6b 656e 5061 7468  ame":"_tokenPath
-0001bc00: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001bc10: 735b 5d22 7d2c 7b22 696e 7465 726e 616c  s[]"},{"internal
-0001bc20: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-0001bc30: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
-0001bc40: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001bc50: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001bc60: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001bc70: 225f 6465 6164 6c69 6e65 222c 2274 7970  "_deadline","typ
-0001bc80: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001bc90: 6e61 6d65 223a 2273 7761 7045 7861 6374  name":"swapExact
-0001bca0: 4156 4158 466f 7254 6f6b 656e 7322 2c22  AVAXForTokens","
-0001bcb0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0001bcc0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001bcd0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001bce0: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0001bcf0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001bd00: 4d75 7461 6269 6c69 7479 223a 2270 6179  Mutability":"pay
-0001bd10: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-0001bd20: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-0001bd30: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001bd40: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001bd50: 616d 6522 3a22 5f61 6d6f 756e 744f 7574  ame":"_amountOut
-0001bd60: 4d69 6e22 2c22 7479 7065 223a 2275 696e  Min","type":"uin
-0001bd70: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0001bd80: 6c54 7970 6522 3a22 7569 6e74 3235 365b  lType":"uint256[
-0001bd90: 5d22 2c22 6e61 6d65 223a 225f 7061 6972  ]","name":"_pair
-0001bda0: 4269 6e53 7465 7073 222c 2274 7970 6522  BinSteps","type"
-0001bdb0: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
-0001bdc0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-0001bdd0: 6f6e 7472 6163 7420 4945 5243 3230 5b5d  ontract IERC20[]
-0001bde0: 222c 226e 616d 6522 3a22 5f74 6f6b 656e  ","name":"_token
-0001bdf0: 5061 7468 222c 2274 7970 6522 3a22 6164  Path","type":"ad
-0001be00: 6472 6573 735b 5d22 7d2c 7b22 696e 7465  dress[]"},{"inte
-0001be10: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001be20: 7373 222c 226e 616d 6522 3a22 5f74 6f22  ss","name":"_to"
-0001be30: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001be40: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001be50: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001be60: 6d65 223a 225f 6465 6164 6c69 6e65 222c  me":"_deadline",
-0001be70: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001be80: 7d5d 2c22 6e61 6d65 223a 2273 7761 7045  }],"name":"swapE
-0001be90: 7861 6374 4156 4158 466f 7254 6f6b 656e  xactAVAXForToken
-0001bea0: 7353 7570 706f 7274 696e 6746 6565 4f6e  sSupportingFeeOn
-0001beb0: 5472 616e 7366 6572 546f 6b65 6e73 222c  TransferTokens",
-0001bec0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-0001bed0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001bee0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001bef0: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
-0001bf00: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-0001bf10: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
-0001bf20: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-0001bf30: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-0001bf40: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001bf50: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001bf60: 6e61 6d65 223a 225f 616d 6f75 6e74 496e  name":"_amountIn
-0001bf70: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001bf80: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001bf90: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001bfa0: 616d 6522 3a22 5f61 6d6f 756e 744f 7574  ame":"_amountOut
-0001bfb0: 4d69 6e41 5641 5822 2c22 7479 7065 223a  MinAVAX","type":
-0001bfc0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001bfd0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001bfe0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-0001bff0: 7061 6972 4269 6e53 7465 7073 222c 2274  pairBinSteps","t
-0001c000: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001c010: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001c020: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001c030: 3230 5b5d 222c 226e 616d 6522 3a22 5f74  20[]","name":"_t
-0001c040: 6f6b 656e 5061 7468 222c 2274 7970 6522  okenPath","type"
-0001c050: 3a22 6164 6472 6573 735b 5d22 7d2c 7b22  :"address[]"},{"
-0001c060: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0001c070: 6464 7265 7373 2070 6179 6162 6c65 222c  ddress payable",
-0001c080: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
-0001c090: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001c0a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001c0b0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001c0c0: 225f 6465 6164 6c69 6e65 222c 2274 7970  "_deadline","typ
-0001c0d0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001c0e0: 6e61 6d65 223a 2273 7761 7045 7861 6374  name":"swapExact
-0001c0f0: 546f 6b65 6e73 466f 7241 5641 5822 2c22  TokensForAVAX","
-0001c100: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0001c110: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001c120: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001c130: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0001c140: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001c150: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-0001c160: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-0001c170: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-0001c180: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001c190: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001c1a0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001c1b0: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
-0001c1c0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001c1d0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001c1e0: 226e 616d 6522 3a22 5f61 6d6f 756e 744f  "name":"_amountO
-0001c1f0: 7574 4d69 6e41 5641 5822 2c22 7479 7065  utMinAVAX","type
-0001c200: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001c210: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001c220: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-0001c230: 225f 7061 6972 4269 6e53 7465 7073 222c  "_pairBinSteps",
-0001c240: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
-0001c250: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-0001c260: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-0001c270: 5243 3230 5b5d 222c 226e 616d 6522 3a22  RC20[]","name":"
-0001c280: 5f74 6f6b 656e 5061 7468 222c 2274 7970  _tokenPath","typ
-0001c290: 6522 3a22 6164 6472 6573 735b 5d22 7d2c  e":"address[]"},
-0001c2a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001c2b0: 2261 6464 7265 7373 2070 6179 6162 6c65  "address payable
-0001c2c0: 222c 226e 616d 6522 3a22 5f74 6f22 2c22  ","name":"_to","
-0001c2d0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001c2e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001c2f0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001c300: 223a 225f 6465 6164 6c69 6e65 222c 2274  ":"_deadline","t
-0001c310: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0001c320: 2c22 6e61 6d65 223a 2273 7761 7045 7861  ,"name":"swapExa
-0001c330: 6374 546f 6b65 6e73 466f 7241 5641 5853  ctTokensForAVAXS
-0001c340: 7570 706f 7274 696e 6746 6565 4f6e 5472  upportingFeeOnTr
-0001c350: 616e 7366 6572 546f 6b65 6e73 222c 226f  ansferTokens","o
-0001c360: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-0001c370: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001c380: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0001c390: 744f 7574 222c 2274 7970 6522 3a22 7569  tOut","type":"ui
-0001c3a0: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-0001c3b0: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-0001c3c0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-0001c3d0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-0001c3e0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001c3f0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001c400: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
-0001c410: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001c420: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001c430: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001c440: 6e61 6d65 223a 225f 616d 6f75 6e74 4f75  name":"_amountOu
-0001c450: 744d 696e 222c 2274 7970 6522 3a22 7569  tMin","type":"ui
-0001c460: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0001c470: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001c480: 5b5d 222c 226e 616d 6522 3a22 5f70 6169  []","name":"_pai
-0001c490: 7242 696e 5374 6570 7322 2c22 7479 7065  rBinSteps","type
-0001c4a0: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
-0001c4b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001c4c0: 636f 6e74 7261 6374 2049 4552 4332 305b  contract IERC20[
-0001c4d0: 5d22 2c22 6e61 6d65 223a 225f 746f 6b65  ]","name":"_toke
-0001c4e0: 6e50 6174 6822 2c22 7479 7065 223a 2261  nPath","type":"a
-0001c4f0: 6464 7265 7373 5b5d 227d 2c7b 2269 6e74  ddress[]"},{"int
-0001c500: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001c510: 6573 7322 2c22 6e61 6d65 223a 225f 746f  ess","name":"_to
-0001c520: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001c530: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-0001c540: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001c550: 616d 6522 3a22 5f64 6561 646c 696e 6522  ame":"_deadline"
-0001c560: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001c570: 227d 5d2c 226e 616d 6522 3a22 7377 6170  "}],"name":"swap
-0001c580: 4578 6163 7454 6f6b 656e 7346 6f72 546f  ExactTokensForTo
-0001c590: 6b65 6e73 222c 226f 7574 7075 7473 223a  kens","outputs":
-0001c5a0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001c5b0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001c5c0: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
-0001c5d0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0001c5e0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-0001c5f0: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
-0001c600: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-0001c610: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001c620: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001c630: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001c640: 5f61 6d6f 756e 7449 6e22 2c22 7479 7065  _amountIn","type
-0001c650: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001c660: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001c670: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-0001c680: 616d 6f75 6e74 4f75 744d 696e 222c 2274  amountOutMin","t
-0001c690: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001c6a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001c6b0: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
-0001c6c0: 6522 3a22 5f70 6169 7242 696e 5374 6570  e":"_pairBinStep
-0001c6d0: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-0001c6e0: 3536 5b5d 227d 2c7b 2269 6e74 6572 6e61  56[]"},{"interna
-0001c6f0: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001c700: 2049 4552 4332 305b 5d22 2c22 6e61 6d65   IERC20[]","name
-0001c710: 223a 225f 746f 6b65 6e50 6174 6822 2c22  ":"_tokenPath","
-0001c720: 7479 7065 223a 2261 6464 7265 7373 5b5d  type":"address[]
-0001c730: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001c740: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0001c750: 6d65 223a 225f 746f 222c 2274 7970 6522  me":"_to","type"
-0001c760: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001c770: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001c780: 7432 3536 222c 226e 616d 6522 3a22 5f64  t256","name":"_d
-0001c790: 6561 646c 696e 6522 2c22 7479 7065 223a  eadline","type":
-0001c7a0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-0001c7b0: 6522 3a22 7377 6170 4578 6163 7454 6f6b  e":"swapExactTok
-0001c7c0: 656e 7346 6f72 546f 6b65 6e73 5375 7070  ensForTokensSupp
-0001c7d0: 6f72 7469 6e67 4665 654f 6e54 7261 6e73  ortingFeeOnTrans
-0001c7e0: 6665 7254 6f6b 656e 7322 2c22 6f75 7470  ferTokens","outp
-0001c7f0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001c800: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001c810: 226e 616d 6522 3a22 616d 6f75 6e74 4f75  "name":"amountOu
-0001c820: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-0001c830: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
-0001c840: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
-0001c850: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
-0001c860: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-0001c870: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001c880: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001c890: 6d65 223a 225f 616d 6f75 6e74 4156 4158  me":"_amountAVAX
-0001c8a0: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
-0001c8b0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0001c8c0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001c8d0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001c8e0: 496e 4d61 7822 2c22 7479 7065 223a 2275  InMax","type":"u
-0001c8f0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001c900: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001c910: 365b 5d22 2c22 6e61 6d65 223a 225f 7061  6[]","name":"_pa
-0001c920: 6972 4269 6e53 7465 7073 222c 2274 7970  irBinSteps","typ
-0001c930: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-0001c940: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001c950: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
-0001c960: 5b5d 222c 226e 616d 6522 3a22 5f74 6f6b  []","name":"_tok
-0001c970: 656e 5061 7468 222c 2274 7970 6522 3a22  enPath","type":"
-0001c980: 6164 6472 6573 735b 5d22 7d2c 7b22 696e  address[]"},{"in
-0001c990: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001c9a0: 7265 7373 2070 6179 6162 6c65 222c 226e  ress payable","n
-0001c9b0: 616d 6522 3a22 5f74 6f22 2c22 7479 7065  ame":"_to","type
-0001c9c0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001c9d0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001c9e0: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-0001c9f0: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
-0001ca00: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-0001ca10: 6d65 223a 2273 7761 7054 6f6b 656e 7346  me":"swapTokensF
-0001ca20: 6f72 4578 6163 7441 5641 5822 2c22 6f75  orExactAVAX","ou
-0001ca30: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-0001ca40: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001ca50: 5b5d 222c 226e 616d 6522 3a22 616d 6f75  []","name":"amou
-0001ca60: 6e74 7349 6e22 2c22 7479 7065 223a 2275  ntsIn","type":"u
-0001ca70: 696e 7432 3536 5b5d 227d 5d2c 2273 7461  int256[]"}],"sta
-0001ca80: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-0001ca90: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-0001caa0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-0001cab0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-0001cac0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001cad0: 3622 2c22 6e61 6d65 223a 225f 616d 6f75  6","name":"_amou
-0001cae0: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0001caf0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001cb00: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001cb10: 3622 2c22 6e61 6d65 223a 225f 616d 6f75  6","name":"_amou
-0001cb20: 6e74 496e 4d61 7822 2c22 7479 7065 223a  ntInMax","type":
-0001cb30: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001cb40: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001cb50: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-0001cb60: 7061 6972 4269 6e53 7465 7073 222c 2274  pairBinSteps","t
-0001cb70: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001cb80: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001cb90: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001cba0: 3230 5b5d 222c 226e 616d 6522 3a22 5f74  20[]","name":"_t
-0001cbb0: 6f6b 656e 5061 7468 222c 2274 7970 6522  okenPath","type"
-0001cbc0: 3a22 6164 6472 6573 735b 5d22 7d2c 7b22  :"address[]"},{"
-0001cbd0: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0001cbe0: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0001cbf0: 5f74 6f22 2c22 7479 7065 223a 2261 6464  _to","type":"add
-0001cc00: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001cc10: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001cc20: 2c22 6e61 6d65 223a 225f 6465 6164 6c69  ,"name":"_deadli
-0001cc30: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
-0001cc40: 3235 3622 7d5d 2c22 6e61 6d65 223a 2273  256"}],"name":"s
-0001cc50: 7761 7054 6f6b 656e 7346 6f72 4578 6163  wapTokensForExac
-0001cc60: 7454 6f6b 656e 7322 2c22 6f75 7470 7574  tTokens","output
-0001cc70: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001cc80: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-0001cc90: 226e 616d 6522 3a22 616d 6f75 6e74 7349  "name":"amountsI
-0001cca0: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001ccb0: 3536 5b5d 227d 5d2c 2273 7461 7465 4d75  56[]"}],"stateMu
-0001ccc0: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-0001ccd0: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-0001cce0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-0001ccf0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001cd00: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-0001cd10: 4552 4332 3022 2c22 6e61 6d65 223a 225f  ERC20","name":"_
-0001cd20: 746f 6b65 6e22 2c22 7479 7065 223a 2261  token","type":"a
-0001cd30: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-0001cd40: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001cd50: 7322 2c22 6e61 6d65 223a 225f 746f 222c  s","name":"_to",
-0001cd60: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001cd70: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001cd80: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001cd90: 6522 3a22 5f61 6d6f 756e 7422 2c22 7479  e":"_amount","ty
-0001cda0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001cdb0: 226e 616d 6522 3a22 7377 6565 7022 2c22  "name":"sweep","
-0001cdc0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-0001cdd0: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-0001cde0: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-0001cdf0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-0001ce00: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-0001ce10: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-0001ce20: 6374 2049 4c42 546f 6b65 6e22 2c22 6e61  ct ILBToken","na
-0001ce30: 6d65 223a 225f 6c62 546f 6b65 6e22 2c22  me":"_lbToken","
-0001ce40: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001ce50: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001ce60: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0001ce70: 223a 225f 746f 222c 2274 7970 6522 3a22  ":"_to","type":"
-0001ce80: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-0001ce90: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001cea0: 3536 5b5d 222c 226e 616d 6522 3a22 5f69  56[]","name":"_i
-0001ceb0: 6473 222c 2274 7970 6522 3a22 7569 6e74  ds","type":"uint
-0001cec0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
-0001ced0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001cee0: 5b5d 222c 226e 616d 6522 3a22 5f61 6d6f  []","name":"_amo
-0001cef0: 756e 7473 222c 2274 7970 6522 3a22 7569  unts","type":"ui
-0001cf00: 6e74 3235 365b 5d22 7d5d 2c22 6e61 6d65  nt256[]"}],"name
-0001cf10: 223a 2273 7765 6570 4c42 546f 6b65 6e22  ":"sweepLBToken"
-0001cf20: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
-0001cf30: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-0001cf40: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
-0001cf50: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0001cf60: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-0001cf70: 6d65 223a 2277 6176 6178 222c 226f 7574  me":"wavax","out
-0001cf80: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001cf90: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001cfa0: 2049 5741 5641 5822 2c22 6e61 6d65 223a   IWAVAX","name":
-0001cfb0: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-0001cfc0: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-0001cfd0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-0001cfe0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0001cff0: 7d2c 7b22 7374 6174 654d 7574 6162 696c  },{"stateMutabil
-0001d000: 6974 7922 3a22 7061 7961 626c 6522 2c22  ity":"payable","
-0001d010: 7479 7065 223a 2272 6563 6569 7665 227d  type":"receive"}
-0001d020: 5d27 290a 0a20 2020 2064 6566 2067 6574  ]')..    def get
-0001d030: 5f69 645f 6672 6f6d 5f70 7269 6365 285f  _id_from_price(_
-0001d040: 7765 6233 3a57 6562 332c 5f72 6f75 7465  web3:Web3,_route
-0001d050: 5f61 6464 7265 7373 3a73 7472 2c5f 726f  _address:str,_ro
-0001d060: 7574 655f 6162 692c 5f6c 625f 7061 6972  ute_abi,_lb_pair
-0001d070: 2c5f 7072 6963 6529 3a0a 2020 2020 2020  ,_price):.      
-0001d080: 2020 7265 7475 726e 205f 7765 6233 2e65    return _web3.e
-0001d090: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-0001d0a0: 6573 733d 5f72 6f75 7465 5f61 6464 7265  ess=_route_addre
-0001d0b0: 7373 2c20 6162 693d 5f72 6f75 7465 5f61  ss, abi=_route_a
-0001d0c0: 6269 292e 6675 6e63 7469 6f6e 732e 6765  bi).functions.ge
-0001d0d0: 7449 6446 726f 6d50 7269 6365 285f 6c62  tIdFromPrice(_lb
-0001d0e0: 5f70 6169 722c 5f70 7269 6365 292e 6361  _pair,_price).ca
-0001d0f0: 6c6c 2829 0a0a 2020 2020 6465 6620 6765  ll()..    def ge
-0001d100: 745f 7072 6963 655f 6672 6f6d 5f69 6428  t_price_from_id(
-0001d110: 5f77 6562 333a 5765 6233 2c5f 726f 7574  _web3:Web3,_rout
-0001d120: 655f 6164 6472 6573 733a 7374 722c 5f72  e_address:str,_r
-0001d130: 6f75 7465 5f61 6269 2c5f 6c62 5f70 6169  oute_abi,_lb_pai
-0001d140: 722c 5f69 6429 3a0a 2020 2020 2020 2020  r,_id):.        
-0001d150: 7265 7475 726e 205f 7765 6233 2e65 7468  return _web3.eth
-0001d160: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
-0001d170: 733d 5f72 6f75 7465 5f61 6464 7265 7373  s=_route_address
-0001d180: 2c20 6162 693d 5f72 6f75 7465 5f61 6269  , abi=_route_abi
-0001d190: 292e 6675 6e63 7469 6f6e 732e 6765 7450  ).functions.getP
-0001d1a0: 7269 6365 4672 6f6d 4964 285f 6c62 5f70  riceFromId(_lb_p
-0001d1b0: 6169 722c 5f69 6429 2e63 616c 6c28 290a  air,_id).call().
-0001d1c0: 0a20 2020 2023 7265 7475 726e 205b 616d  .    #return [am
-0001d1d0: 6f75 6e74 5f69 6e2c 6665 655d 0a20 2020  ount_in,fee].   
-0001d1e0: 2064 6566 2067 6574 5f73 7761 705f 696e   def get_swap_in
-0001d1f0: 285f 7765 6233 3a57 6562 332c 5f72 6f75  (_web3:Web3,_rou
-0001d200: 7465 5f61 6464 7265 7373 3a73 7472 2c5f  te_address:str,_
-0001d210: 726f 7574 655f 6162 693a 7374 722c 5f6c  route_abi:str,_l
-0001d220: 625f 7061 6972 2c5f 616d 6f75 6e74 5f6f  b_pair,_amount_o
-0001d230: 7574 2c5f 7377 6170 5f66 6f72 5f79 3a62  ut,_swap_for_y:b
-0001d240: 6f6f 6c29 3a0a 2020 2020 2020 2020 7265  ool):.        re
-0001d250: 7475 726e 205f 7765 6233 2e65 7468 2e63  turn _web3.eth.c
-0001d260: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
-0001d270: 5f72 6f75 7465 5f61 6464 7265 7373 2c20  _route_address, 
-0001d280: 6162 693d 5f72 6f75 7465 5f61 6269 292e  abi=_route_abi).
-0001d290: 6675 6e63 7469 6f6e 732e 6765 7453 7761  functions.getSwa
-0001d2a0: 7049 6e28 5f6c 625f 7061 6972 2c5f 616d  pIn(_lb_pair,_am
-0001d2b0: 6f75 6e74 5f6f 7574 2c5f 7377 6170 5f66  ount_out,_swap_f
-0001d2c0: 6f72 5f79 292e 6361 6c6c 2829 0a20 2020  or_y).call().   
-0001d2d0: 200a 2020 2020 2372 6574 7572 6e20 5b61   .    #return [a
-0001d2e0: 6d6f 756e 745f 6f75 742c 6665 655d 0a20  mount_out,fee]. 
-0001d2f0: 2020 2064 6566 2067 6574 5f73 7761 705f     def get_swap_
-0001d300: 6f75 7428 5f77 6562 333a 5765 6233 2c5f  out(_web3:Web3,_
-0001d310: 726f 7574 655f 6164 6472 6573 733a 7374  route_address:st
-0001d320: 722c 5f72 6f75 7465 5f61 6269 3a73 7472  r,_route_abi:str
-0001d330: 2c5f 6c62 5f70 6169 722c 5f61 6d6f 756e  ,_lb_pair,_amoun
-0001d340: 745f 696e 2c5f 7377 6170 5f66 6f72 5f79  t_in,_swap_for_y
-0001d350: 3a62 6f6f 6c29 3a0a 2020 2020 2020 2020  :bool):.        
-0001d360: 7265 7475 726e 205f 7765 6233 2e65 7468  return _web3.eth
-0001d370: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
-0001d380: 733d 5f72 6f75 7465 5f61 6464 7265 7373  s=_route_address
-0001d390: 2c20 6162 693d 5f72 6f75 7465 5f61 6269  , abi=_route_abi
-0001d3a0: 292e 6675 6e63 7469 6f6e 732e 6765 7453  ).functions.getS
-0001d3b0: 7761 704f 7574 285f 6c62 5f70 6169 722c  wapOut(_lb_pair,
-0001d3c0: 5f61 6d6f 756e 745f 696e 2c5f 7377 6170  _amount_in,_swap
-0001d3d0: 5f66 6f72 5f79 292e 6361 6c6c 2829 0a0a  _for_y).call()..
-0001d3e0: 2020 2020 6465 6620 7377 6170 5f65 7861      def swap_exa
-0001d3f0: 6374 5f74 6f6b 656e 735f 666f 725f 746f  ct_tokens_for_to
-0001d400: 6b65 6e73 285f 7765 6233 3a57 6562 332c  kens(_web3:Web3,
-0001d410: 5f72 6f75 7465 5f61 6464 7265 7373 3a73  _route_address:s
-0001d420: 7472 2c5f 726f 7574 655f 6162 692c 0a20  tr,_route_abi,. 
-0001d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d450: 2020 2020 5f61 6d6f 756e 745f 696e 2c5f      _amount_in,_
-0001d460: 616d 6f75 6e74 5f6f 7574 5f6d 696e 2c5f  amount_out_min,_
-0001d470: 7061 6972 5f62 696e 5f73 7465 7073 2c5f  pair_bin_steps,_
-0001d480: 746f 6b65 6e5f 7061 7468 2c5f 746f 2c5f  token_path,_to,_
-0001d490: 6465 6164 6c69 6e65 2c0a 2020 2020 2020  deadline,.      
-0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4b0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0001d4c0: 7075 626c 6963 5f6b 6579 2c5f 7072 6976  public_key,_priv
-0001d4d0: 6174 655f 6b65 7929 3a0a 2020 2020 2020  ate_key):.      
-0001d4e0: 2020 6e6f 6e63 653d 5f77 6562 332e 6574    nonce=_web3.et
-0001d4f0: 682e 6765 745f 7472 616e 7361 6374 696f  h.get_transactio
-0001d500: 6e5f 636f 756e 7428 5f70 7562 6c69 635f  n_count(_public_
-0001d510: 6b65 7929 0a20 2020 2020 2020 2072 6f75  key).        rou
-0001d520: 7465 5f63 6f6e 7472 6163 743d 5f77 6562  te_contract=_web
-0001d530: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-0001d540: 6464 7265 7373 3d5f 726f 7574 655f 6164  ddress=_route_ad
-0001d550: 6472 6573 732c 2061 6269 3d5f 726f 7574  dress, abi=_rout
-0001d560: 655f 6162 6929 0a20 2020 2020 2020 2073  e_abi).        s
-0001d570: 7761 705f 6675 6e63 7469 6f6e 3d72 6f75  wap_function=rou
-0001d580: 7465 5f63 6f6e 7472 6163 742e 6675 6e63  te_contract.func
-0001d590: 7469 6f6e 732e 7377 6170 4578 6163 7454  tions.swapExactT
-0001d5a0: 6f6b 656e 7346 6f72 546f 6b65 6e73 285f  okensForTokens(_
-0001d5b0: 616d 6f75 6e74 5f69 6e2c 5f61 6d6f 756e  amount_in,_amoun
-0001d5c0: 745f 6f75 745f 6d69 6e2c 5f70 6169 725f  t_out_min,_pair_
-0001d5d0: 6269 6e5f 7374 6570 732c 5f74 6f6b 656e  bin_steps,_token
-0001d5e0: 5f70 6174 682c 5f74 6f2c 5f64 6561 646c  _path,_to,_deadl
-0001d5f0: 696e 6529 0a20 2020 2020 2020 2070 6172  ine).        par
-0001d600: 616d 733d 7b0a 2020 2020 2020 2020 2020  ams={.          
-0001d610: 2020 2766 726f 6d27 3a20 5f70 7562 6c69    'from': _publi
-0001d620: 635f 6b65 792c 0a20 2020 2020 2020 2020  c_key,.         
-0001d630: 2020 2027 7661 6c75 6527 3a20 302c 0a20     'value': 0,. 
-0001d640: 2020 2020 2020 2020 2020 2027 6e6f 6e63             'nonc
-0001d650: 6527 3a20 6e6f 6e63 652c 0a20 2020 2020  e': nonce,.     
-0001d660: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
-0001d670: 3078 3227 0a20 2020 2020 2020 207d 0a20  0x2'.        }. 
-0001d680: 2020 2020 2020 2073 6967 6e65 645f 7472         signed_tr
-0001d690: 616e 7361 6374 696f 6e3d 5f77 6562 332e  ansaction=_web3.
-0001d6a0: 6574 682e 6163 636f 756e 742e 7369 676e  eth.account.sign
-0001d6b0: 5f74 7261 6e73 6163 7469 6f6e 2873 7761  _transaction(swa
-0001d6c0: 705f 6675 6e63 7469 6f6e 2e62 7569 6c64  p_function.build
-0001d6d0: 5472 616e 7361 6374 696f 6e28 7061 7261  Transaction(para
-0001d6e0: 6d73 292c 7072 6976 6174 655f 6b65 793d  ms),private_key=
-0001d6f0: 5f70 7269 7661 7465 5f6b 6579 290a 2020  _private_key).  
-0001d700: 2020 2020 2020 7265 7370 6f6e 7365 3d5f        response=_
-0001d710: 7765 6233 2e65 7468 2e73 656e 645f 7261  web3.eth.send_ra
-0001d720: 775f 7472 616e 7361 6374 696f 6e28 7369  w_transaction(si
-0001d730: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
-0001d740: 2e72 6177 5472 616e 7361 6374 696f 6e29  .rawTransaction)
-0001d750: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001d760: 5765 6233 2e74 6f48 6578 2872 6573 706f  Web3.toHex(respo
-0001d770: 6e73 6529 0a20 2020 200a 2020 2020 6465  nse).    .    de
-0001d780: 6620 7377 6170 5f74 6f6b 656e 735f 666f  f swap_tokens_fo
-0001d790: 725f 6578 6163 745f 746f 6b65 6e73 285f  r_exact_tokens(_
-0001d7a0: 7765 6233 3a57 6562 332c 5f72 6f75 7465  web3:Web3,_route
-0001d7b0: 5f61 6464 7265 7373 3a73 7472 2c5f 726f  _address:str,_ro
-0001d7c0: 7574 655f 6162 692c 0a20 2020 2020 2020  ute_abi,.       
-0001d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7e0: 2020 2020 2020 2020 2020 2020 2020 5f61                _a
-0001d7f0: 6d6f 756e 745f 6f75 742c 5f61 6d6f 756e  mount_out,_amoun
-0001d800: 745f 696e 5f6d 6178 2c5f 7061 6972 5f62  t_in_max,_pair_b
-0001d810: 696e 5f73 7465 7073 2c5f 746f 6b65 6e5f  in_steps,_token_
-0001d820: 7061 7468 2c5f 746f 2c5f 6465 6164 6c69  path,_to,_deadli
-0001d830: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d850: 2020 2020 2020 2020 205f 7075 626c 6963           _public
-0001d860: 5f6b 6579 2c5f 7072 6976 6174 655f 6b65  _key,_private_ke
-0001d870: 7929 3a0a 2020 2020 2020 2020 6e6f 6e63  y):.        nonc
-0001d880: 653d 5f77 6562 332e 6574 682e 6765 745f  e=_web3.eth.get_
-0001d890: 7472 616e 7361 6374 696f 6e5f 636f 756e  transaction_coun
-0001d8a0: 7428 5f70 7562 6c69 635f 6b65 7929 0a20  t(_public_key). 
-0001d8b0: 2020 2020 2020 2072 6f75 7465 5f63 6f6e         route_con
-0001d8c0: 7472 6163 743d 5f77 6562 332e 6574 682e  tract=_web3.eth.
-0001d8d0: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
-0001d8e0: 3d5f 726f 7574 655f 6164 6472 6573 732c  =_route_address,
-0001d8f0: 2061 6269 3d5f 726f 7574 655f 6162 6929   abi=_route_abi)
-0001d900: 0a20 2020 2020 2020 2073 7761 705f 6675  .        swap_fu
-0001d910: 6e63 7469 6f6e 3d72 6f75 7465 5f63 6f6e  nction=route_con
-0001d920: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-0001d930: 7377 6170 546f 6b65 6e73 466f 7245 7861  swapTokensForExa
-0001d940: 6374 546f 6b65 6e73 285f 616d 6f75 6e74  ctTokens(_amount
-0001d950: 5f6f 7574 2c5f 616d 6f75 6e74 5f69 6e5f  _out,_amount_in_
-0001d960: 6d61 782c 5f70 6169 725f 6269 6e5f 7374  max,_pair_bin_st
-0001d970: 6570 732c 5f74 6f6b 656e 5f70 6174 682c  eps,_token_path,
-0001d980: 5f74 6f2c 5f64 6561 646c 696e 6529 0a20  _to,_deadline). 
-0001d990: 2020 2020 2020 2070 6172 616d 733d 7b0a         params={.
-0001d9a0: 2020 2020 2020 2020 2020 2020 2766 726f              'fro
-0001d9b0: 6d27 3a20 5f70 7562 6c69 635f 6b65 792c  m': _public_key,
-0001d9c0: 0a20 2020 2020 2020 2020 2020 2027 7661  .            'va
-0001d9d0: 6c75 6527 3a20 302c 0a20 2020 2020 2020  lue': 0,.       
-0001d9e0: 2020 2020 2027 6e6f 6e63 6527 3a20 6e6f       'nonce': no
-0001d9f0: 6e63 652c 0a20 2020 2020 2020 2020 2020  nce,.           
-0001da00: 2027 7479 7065 273a 2027 3078 3227 0a20   'type': '0x2'. 
-0001da10: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0001da20: 2073 6967 6e65 645f 7472 616e 7361 6374   signed_transact
-0001da30: 696f 6e3d 5f77 6562 332e 6574 682e 6163  ion=_web3.eth.ac
-0001da40: 636f 756e 742e 7369 676e 5f74 7261 6e73  count.sign_trans
-0001da50: 6163 7469 6f6e 2873 7761 705f 6675 6e63  action(swap_func
-0001da60: 7469 6f6e 2e62 7569 6c64 5472 616e 7361  tion.buildTransa
-0001da70: 6374 696f 6e28 7061 7261 6d73 292c 7072  ction(params),pr
-0001da80: 6976 6174 655f 6b65 793d 5f70 7269 7661  ivate_key=_priva
-0001da90: 7465 5f6b 6579 290a 2020 2020 2020 2020  te_key).        
-0001daa0: 7265 7370 6f6e 7365 3d5f 7765 6233 2e65  response=_web3.e
-0001dab0: 7468 2e73 656e 645f 7261 775f 7472 616e  th.send_raw_tran
-0001dac0: 7361 6374 696f 6e28 7369 676e 6564 5f74  saction(signed_t
-0001dad0: 7261 6e73 6163 7469 6f6e 2e72 6177 5472  ransaction.rawTr
-0001dae0: 616e 7361 6374 696f 6e29 0a20 2020 2020  ansaction).     
-0001daf0: 2020 2072 6574 7572 6e20 5765 6233 2e74     return Web3.t
-0001db00: 6f48 6578 2872 6573 706f 6e73 6529 0a0a  oHex(response)..
-0001db10: 636c 6173 7320 4a6f 6556 3250 6169 723a  class JoeV2Pair:
-0001db20: 0a0a 2020 2020 6a6f 655f 7061 6972 5f76  ..    joe_pair_v
-0001db30: 325f 6162 693d 6a73 6f6e 2e6c 6f61 6473  2_abi=json.loads
-0001db40: 2827 5b7b 2269 6e70 7574 7322 3a5b 7b22  ('[{"inputs":[{"
-0001db50: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-0001db60: 6f6e 7472 6163 7420 494c 4246 6163 746f  ontract ILBFacto
-0001db70: 7279 222c 226e 616d 6522 3a22 5f66 6163  ry","name":"_fac
-0001db80: 746f 7279 222c 2274 7970 6522 3a22 6164  tory","type":"ad
-0001db90: 6472 6573 7322 7d5d 2c22 7374 6174 654d  dress"}],"stateM
-0001dba0: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-0001dbb0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-0001dbc0: 636f 6e73 7472 7563 746f 7222 7d2c 7b22  constructor"},{"
-0001dbd0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-0001dbe0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001dbf0: 3622 2c22 6e61 6d65 223a 2262 7022 2c22  6","name":"bp","
-0001dc00: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001dc10: 5d2c 226e 616d 6522 3a22 4269 6e48 656c  ],"name":"BinHel
-0001dc20: 7065 725f 5f42 696e 5374 6570 4f76 6572  per__BinStepOver
-0001dc30: 666c 6f77 7322 2c22 7479 7065 223a 2265  flows","type":"e
-0001dc40: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-0001dc50: 3a5b 5d2c 226e 616d 6522 3a22 4269 6e48  :[],"name":"BinH
-0001dc60: 656c 7065 725f 5f49 644f 7665 7266 6c6f  elper__IdOverflo
-0001dc70: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
-0001dc80: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0001dc90: 2c22 6e61 6d65 223a 224c 4250 6169 725f  ,"name":"LBPair_
-0001dca0: 5f41 6464 7265 7373 5a65 726f 222c 2274  _AddressZero","t
-0001dcb0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-0001dcc0: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-0001dcd0: 223a 224c 4250 6169 725f 5f41 6464 7265  ":"LBPair__Addre
-0001dce0: 7373 5a65 726f 4f72 5468 6973 222c 2274  ssZeroOrThis","t
-0001dcf0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-0001dd00: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-0001dd10: 223a 224c 4250 6169 725f 5f41 6c72 6561  ":"LBPair__Alrea
-0001dd20: 6479 496e 6974 6961 6c69 7a65 6422 2c22  dyInitialized","
-0001dd30: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001dd40: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001dd50: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001dd60: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
-0001dd70: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001dd80: 7d5d 2c22 6e61 6d65 223a 224c 4250 6169  }],"name":"LBPai
-0001dd90: 725f 5f43 6f6d 706f 7369 7469 6f6e 4661  r__CompositionFa
-0001dda0: 6374 6f72 466c 6177 6564 222c 2274 7970  ctorFlawed","typ
-0001ddb0: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001ddc0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001ddd0: 224c 4250 6169 725f 5f44 6973 7472 6962  "LBPair__Distrib
-0001dde0: 7574 696f 6e73 4f76 6572 666c 6f77 222c  utionsOverflow",
-0001ddf0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001de00: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-0001de10: 6d65 223a 224c 4250 6169 725f 5f46 6c61  me":"LBPair__Fla
-0001de20: 7368 4c6f 616e 4361 6c6c 6261 636b 4661  shLoanCallbackFa
-0001de30: 696c 6564 222c 2274 7970 6522 3a22 6572  iled","type":"er
-0001de40: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-0001de50: 5b5d 2c22 6e61 6d65 223a 224c 4250 6169  [],"name":"LBPai
-0001de60: 725f 5f46 6c61 7368 4c6f 616e 496e 7661  r__FlashLoanInva
-0001de70: 6c69 6442 616c 616e 6365 222c 2274 7970  lidBalance","typ
-0001de80: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001de90: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001dea0: 224c 4250 6169 725f 5f46 6c61 7368 4c6f  "LBPair__FlashLo
-0001deb0: 616e 496e 7661 6c69 6454 6f6b 656e 222c  anInvalidToken",
-0001dec0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001ded0: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-0001dee0: 6d65 223a 224c 4250 6169 725f 5f49 6e73  me":"LBPair__Ins
-0001def0: 7566 6669 6369 656e 7441 6d6f 756e 7473  ufficientAmounts
-0001df00: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001df10: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0001df20: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001df30: 6e74 3235 3622 2c22 6e61 6d65 223a 2269  nt256","name":"i
-0001df40: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-0001df50: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
-0001df60: 5061 6972 5f5f 496e 7375 6666 6963 6965  Pair__Insufficie
-0001df70: 6e74 4c69 7175 6964 6974 7942 7572 6e65  ntLiquidityBurne
-0001df80: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
-0001df90: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001dfa0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001dfb0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001dfc0: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-0001dfd0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
-0001dfe0: 4250 6169 725f 5f49 6e73 7566 6669 6369  BPair__Insuffici
-0001dff0: 656e 744c 6971 7569 6469 7479 4d69 6e74  entLiquidityMint
-0001e000: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
-0001e010: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0001e020: 2c22 6e61 6d65 223a 224c 4250 6169 725f  ,"name":"LBPair_
-0001e030: 5f4f 6e6c 7946 6163 746f 7279 222c 2274  _OnlyFactory","t
-0001e040: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-0001e050: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-0001e060: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001e070: 7322 2c22 6e61 6d65 223a 2266 6565 5265  s","name":"feeRe
-0001e080: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-0001e090: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0001e0a0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001e0b0: 6573 7322 2c22 6e61 6d65 223a 2273 656e  ess","name":"sen
-0001e0c0: 6465 7222 2c22 7479 7065 223a 2261 6464  der","type":"add
-0001e0d0: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-0001e0e0: 4c42 5061 6972 5f5f 4f6e 6c79 4665 6552  LBPair__OnlyFeeR
-0001e0f0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-0001e100: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-0001e110: 7473 223a 5b5d 2c22 6e61 6d65 223a 224c  ts":[],"name":"L
-0001e120: 4250 6169 725f 5f4f 6e6c 7953 7472 6963  BPair__OnlyStric
-0001e130: 746c 7949 6e63 7265 6173 696e 6749 6422  tlyIncreasingId"
-0001e140: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001e150: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0001e160: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001e170: 7432 3536 222c 226e 616d 6522 3a22 6e65  t256","name":"ne
-0001e180: 7753 697a 6522 2c22 7479 7065 223a 2275  wSize","type":"u
-0001e190: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001e1a0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001e1b0: 3622 2c22 6e61 6d65 223a 226f 7261 636c  6","name":"oracl
-0001e1c0: 6553 697a 6522 2c22 7479 7065 223a 2275  eSize","type":"u
-0001e1d0: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-0001e1e0: 3a22 4c42 5061 6972 5f5f 4f72 6163 6c65  :"LBPair__Oracle
-0001e1f0: 4e65 7753 697a 6554 6f6f 536d 616c 6c22  NewSizeTooSmall"
-0001e200: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001e210: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001e220: 616d 6522 3a22 4c42 5061 6972 5f5f 5772  ame":"LBPair__Wr
-0001e230: 6f6e 674c 656e 6774 6873 222c 2274 7970  ongLengths","typ
-0001e240: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e250: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001e260: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-0001e270: 2c22 6e61 6d65 223a 2266 726f 6d22 2c22  ,"name":"from","
-0001e280: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001e290: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001e2a0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001e2b0: 223a 2269 6422 2c22 7479 7065 223a 2275  ":"id","type":"u
-0001e2c0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001e2d0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001e2e0: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0001e2f0: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-0001e300: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
-0001e310: 546f 6b65 6e5f 5f42 7572 6e45 7863 6565  Token__BurnExcee
-0001e320: 6473 4261 6c61 6e63 6522 2c22 7479 7065  dsBalance","type
-0001e330: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e340: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-0001e350: 4c42 546f 6b65 6e5f 5f42 7572 6e46 726f  LBToken__BurnFro
-0001e360: 6d41 6464 7265 7373 3022 2c22 7479 7065  mAddress0","type
-0001e370: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e380: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001e390: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001e3a0: 226e 616d 6522 3a22 6163 636f 756e 7473  "name":"accounts
-0001e3b0: 4c65 6e67 7468 222c 2274 7970 6522 3a22  Length","type":"
-0001e3c0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001e3d0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001e3e0: 3536 222c 226e 616d 6522 3a22 6964 734c  56","name":"idsL
-0001e3f0: 656e 6774 6822 2c22 7479 7065 223a 2275  ength","type":"u
-0001e400: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-0001e410: 3a22 4c42 546f 6b65 6e5f 5f4c 656e 6774  :"LBToken__Lengt
-0001e420: 684d 6973 6d61 7463 6822 2c22 7479 7065  hMismatch","type
-0001e430: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e440: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-0001e450: 4c42 546f 6b65 6e5f 5f4d 696e 7454 6f41  LBToken__MintToA
-0001e460: 6464 7265 7373 3022 2c22 7479 7065 223a  ddress0","type":
-0001e470: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-0001e480: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001e490: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001e4a0: 616d 6522 3a22 6f77 6e65 7222 2c22 7479  ame":"owner","ty
-0001e4b0: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-0001e4c0: 226e 616d 6522 3a22 4c42 546f 6b65 6e5f  "name":"LBToken_
-0001e4d0: 5f53 656c 6641 7070 726f 7661 6c22 2c22  _SelfApproval","
-0001e4e0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001e4f0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001e500: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001e510: 7373 222c 226e 616d 6522 3a22 6f77 6e65  ss","name":"owne
-0001e520: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-0001e530: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0001e540: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001e550: 6e61 6d65 223a 2273 7065 6e64 6572 222c  name":"spender",
-0001e560: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001e570: 7d5d 2c22 6e61 6d65 223a 224c 4254 6f6b  }],"name":"LBTok
-0001e580: 656e 5f5f 5370 656e 6465 724e 6f74 4170  en__SpenderNotAp
-0001e590: 7072 6f76 6564 222c 2274 7970 6522 3a22  proved","type":"
-0001e5a0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-0001e5b0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001e5c0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0001e5d0: 6d65 223a 2266 726f 6d22 2c22 7479 7065  me":"from","type
-0001e5e0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001e5f0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001e600: 6e74 3235 3622 2c22 6e61 6d65 223a 2269  nt256","name":"i
-0001e610: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-0001e620: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001e630: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001e640: 6e61 6d65 223a 2261 6d6f 756e 7422 2c22  name":"amount","
-0001e650: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001e660: 5d2c 226e 616d 6522 3a22 4c42 546f 6b65  ],"name":"LBToke
-0001e670: 6e5f 5f54 7261 6e73 6665 7245 7863 6565  n__TransferExcee
-0001e680: 6473 4261 6c61 6e63 6522 2c22 7479 7065  dsBalance","type
-0001e690: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e6a0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-0001e6b0: 4c42 546f 6b65 6e5f 5f54 7261 6e73 6665  LBToken__Transfe
-0001e6c0: 7246 726f 6d4f 7254 6f41 6464 7265 7373  rFromOrToAddress
-0001e6d0: 3022 2c22 7479 7065 223a 2265 7272 6f72  0","type":"error
-0001e6e0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-0001e6f0: 226e 616d 6522 3a22 4c42 546f 6b65 6e5f  "name":"LBToken_
-0001e700: 5f54 7261 6e73 6665 7254 6f53 656c 6622  _TransferToSelf"
-0001e710: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001e720: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0001e730: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001e740: 7432 3536 222c 226e 616d 6522 3a22 7822  t256","name":"x"
-0001e750: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001e760: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001e770: 6522 3a22 696e 7432 3536 222c 226e 616d  e":"int256","nam
-0001e780: 6522 3a22 7922 2c22 7479 7065 223a 2269  e":"y","type":"i
-0001e790: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-0001e7a0: 224d 6174 6831 3238 7831 3238 5f5f 506f  "Math128x128__Po
-0001e7b0: 7765 7255 6e64 6572 666c 6f77 222c 2274  werUnderflow","t
-0001e7c0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-0001e7d0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-0001e7e0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001e7f0: 3622 2c22 6e61 6d65 223a 2270 726f 6431  6","name":"prod1
-0001e800: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001e810: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001e820: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001e830: 616d 6522 3a22 6465 6e6f 6d69 6e61 746f  ame":"denominato
-0001e840: 7222 2c22 7479 7065 223a 2275 696e 7432  r","type":"uint2
-0001e850: 3536 227d 5d2c 226e 616d 6522 3a22 4d61  56"}],"name":"Ma
-0001e860: 7468 3531 3242 6974 735f 5f4d 756c 4469  th512Bits__MulDi
-0001e870: 764f 7665 7266 6c6f 7722 2c22 7479 7065  vOverflow","type
-0001e880: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e890: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001e8a0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001e8b0: 226e 616d 6522 3a22 7072 6f64 3122 2c22  "name":"prod1","
-0001e8c0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001e8d0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001e8e0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001e8f0: 223a 226f 6666 7365 7422 2c22 7479 7065  ":"offset","type
-0001e900: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001e910: 616d 6522 3a22 4d61 7468 3531 3242 6974  ame":"Math512Bit
-0001e920: 735f 5f4d 756c 5368 6966 744f 7665 7266  s__MulShiftOverf
-0001e930: 6c6f 7722 2c22 7479 7065 223a 2265 7272  low","type":"err
-0001e940: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-0001e950: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001e960: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001e970: 3a22 6f66 6673 6574 222c 2274 7970 6522  :"offset","type"
-0001e980: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-0001e990: 6d65 223a 224d 6174 6835 3132 4269 7473  me":"Math512Bits
-0001e9a0: 5f5f 4f66 6673 6574 4f76 6572 666c 6f77  __OffsetOverflow
-0001e9b0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-0001e9c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001e9d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001e9e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001e9f0: 5f6d 696e 5469 6d65 7374 616d 7022 2c22  _minTimestamp","
-0001ea00: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001ea10: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001ea20: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001ea30: 223a 225f 6c6f 6f6b 5570 5469 6d65 7374  ":"_lookUpTimest
-0001ea40: 616d 7022 2c22 7479 7065 223a 2275 696e  amp","type":"uin
-0001ea50: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-0001ea60: 4f72 6163 6c65 5f5f 4c6f 6f6b 5570 5469  Oracle__LookUpTi
-0001ea70: 6d65 7374 616d 7054 6f6f 4f6c 6422 2c22  mestampTooOld","
-0001ea80: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001ea90: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-0001eaa0: 6522 3a22 4f72 6163 6c65 5f5f 4e6f 7449  e":"Oracle__NotI
-0001eab0: 6e69 7469 616c 697a 6564 222c 2274 7970  nitialized","typ
-0001eac0: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001ead0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001eae0: 2252 6565 6e74 7261 6e63 7947 7561 7264  "ReentrancyGuard
-0001eaf0: 5570 6772 6164 6561 626c 655f 5f41 6c72  Upgradeable__Alr
-0001eb00: 6561 6479 496e 6974 6961 6c69 7a65 6422  eadyInitialized"
-0001eb10: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001eb20: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001eb30: 616d 6522 3a22 5265 656e 7472 616e 6379  ame":"Reentrancy
-0001eb40: 4775 6172 6455 7067 7261 6465 6162 6c65  GuardUpgradeable
-0001eb50: 5f5f 5265 656e 7472 616e 7443 616c 6c22  __ReentrantCall"
-0001eb60: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001eb70: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0001eb80: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001eb90: 7432 3536 222c 226e 616d 6522 3a22 7822  t256","name":"x"
-0001eba0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001ebb0: 227d 5d2c 226e 616d 6522 3a22 5361 6665  "}],"name":"Safe
-0001ebc0: 4361 7374 5f5f 4578 6365 6564 7331 3132  Cast__Exceeds112
-0001ebd0: 4269 7473 222c 2274 7970 6522 3a22 6572  Bits","type":"er
-0001ebe0: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-0001ebf0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001ec00: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001ec10: 223a 2278 222c 2274 7970 6522 3a22 7569  ":"x","type":"ui
-0001ec20: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-0001ec30: 2253 6166 6543 6173 745f 5f45 7863 6565  "SafeCast__Excee
-0001ec40: 6473 3132 3842 6974 7322 2c22 7479 7065  ds128Bits","type
-0001ec50: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001ec60: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001ec70: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001ec80: 226e 616d 6522 3a22 7822 2c22 7479 7065  "name":"x","type
-0001ec90: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001eca0: 616d 6522 3a22 5361 6665 4361 7374 5f5f  ame":"SafeCast__
-0001ecb0: 4578 6365 6564 7332 3442 6974 7322 2c22  Exceeds24Bits","
-0001ecc0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001ecd0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001ece0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001ecf0: 3536 222c 226e 616d 6522 3a22 7822 2c22  56","name":"x","
-0001ed00: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001ed10: 5d2c 226e 616d 6522 3a22 5361 6665 4361  ],"name":"SafeCa
-0001ed20: 7374 5f5f 4578 6365 6564 7334 3042 6974  st__Exceeds40Bit
-0001ed30: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-0001ed40: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-0001ed50: 226e 616d 6522 3a22 546f 6b65 6e48 656c  "name":"TokenHel
-0001ed60: 7065 725f 5f43 616c 6c46 6169 6c65 6422  per__CallFailed"
-0001ed70: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001ed80: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001ed90: 616d 6522 3a22 546f 6b65 6e48 656c 7065  ame":"TokenHelpe
-0001eda0: 725f 5f4e 6f6e 436f 6e74 7261 6374 222c  r__NonContract",
-0001edb0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001edc0: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-0001edd0: 6d65 223a 2254 6f6b 656e 4865 6c70 6572  me":"TokenHelper
-0001ede0: 5f5f 5472 616e 7366 6572 4661 696c 6564  __TransferFailed
-0001edf0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001ee00: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001ee10: 6e61 6d65 223a 2254 7265 654d 6174 685f  name":"TreeMath_
-0001ee20: 5f45 7272 6f72 4465 7074 6853 6561 7263  _ErrorDepthSearc
-0001ee30: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
-0001ee40: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
-0001ee50: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
-0001ee60: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-0001ee70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001ee80: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001ee90: 2261 6363 6f75 6e74 222c 2274 7970 6522  "account","type"
-0001eea0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001eeb0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0001eec0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001eed0: 6573 7322 2c22 6e61 6d65 223a 2273 656e  ess","name":"sen
-0001eee0: 6465 7222 2c22 7479 7065 223a 2261 6464  der","type":"add
-0001eef0: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
-0001ef00: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-0001ef10: 6c54 7970 6522 3a22 626f 6f6c 222c 226e  lType":"bool","n
-0001ef20: 616d 6522 3a22 6170 7072 6f76 6564 222c  ame":"approved",
-0001ef30: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-0001ef40: 226e 616d 6522 3a22 4170 7072 6f76 616c  "name":"Approval
-0001ef50: 466f 7241 6c6c 222c 2274 7970 6522 3a22  ForAll","type":"
-0001ef60: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
-0001ef70: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
-0001ef80: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
-0001ef90: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-0001efa0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001efb0: 616d 6522 3a22 7365 6e64 6572 222c 2274  ame":"sender","t
-0001efc0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0001efd0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-0001efe0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001eff0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001f000: 2272 6563 6970 6965 6e74 222c 2274 7970  "recipient","typ
-0001f010: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001f020: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-0001f030: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001f040: 6e74 3235 3622 2c22 6e61 6d65 223a 2269  nt256","name":"i
-0001f050: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-0001f060: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
-0001f070: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
-0001f080: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001f090: 6e61 6d65 223a 2266 6565 7358 222c 2274  name":"feesX","t
-0001f0a0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001f0b0: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-0001f0c0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f0d0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001f0e0: 3a22 6665 6573 5922 2c22 7479 7065 223a  :"feesY","type":
-0001f0f0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-0001f100: 6522 3a22 436f 6d70 6f73 6974 696f 6e46  e":"CompositionF
-0001f110: 6565 222c 2274 7970 6522 3a22 6576 656e  ee","type":"even
-0001f120: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-0001f130: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0001f140: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-0001f150: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f160: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001f170: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
-0001f180: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001f190: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0001f1a0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001f1b0: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
-0001f1c0: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
-0001f1d0: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-0001f1e0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0001f1f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001f200: 3622 2c22 6e61 6d65 223a 2269 6422 2c22  6","name":"id","
-0001f210: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001f220: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001f230: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f240: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001f250: 223a 2261 6d6f 756e 7458 222c 2274 7970  ":"amountX","typ
-0001f260: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0001f270: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-0001f280: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001f290: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001f2a0: 616d 6f75 6e74 5922 2c22 7479 7065 223a  amountY","type":
-0001f2b0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-0001f2c0: 6522 3a22 4465 706f 7369 7465 6454 6f42  e":"DepositedToB
-0001f2d0: 696e 222c 2274 7970 6522 3a22 6576 656e  in","type":"even
-0001f2e0: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-0001f2f0: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0001f300: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-0001f310: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f320: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001f330: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
-0001f340: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001f350: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0001f360: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001f370: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
-0001f380: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
-0001f390: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-0001f3a0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0001f3b0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001f3c0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001f3d0: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
-0001f3e0: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
-0001f3f0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-0001f400: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001f410: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
-0001f420: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001f430: 3622 7d5d 2c22 6e61 6d65 223a 2246 6565  6"}],"name":"Fee
-0001f440: 7343 6f6c 6c65 6374 6564 222c 2274 7970  sCollected","typ
-0001f450: 6522 3a22 6576 656e 7422 7d2c 7b22 616e  e":"event"},{"an
-0001f460: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
-0001f470: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
-0001f480: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
-0001f490: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-0001f4a0: 222c 226e 616d 6522 3a22 7365 6e64 6572  ","name":"sender
-0001f4b0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001f4c0: 7322 7d2c 7b22 696e 6465 7865 6422 3a74  s"},{"indexed":t
-0001f4d0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-0001f4e0: 6522 3a22 636f 6e74 7261 6374 2049 4c42  e":"contract ILB
-0001f4f0: 466c 6173 684c 6f61 6e43 616c 6c62 6163  FlashLoanCallbac
-0001f500: 6b22 2c22 6e61 6d65 223a 2272 6563 6569  k","name":"recei
-0001f510: 7665 7222 2c22 7479 7065 223a 2261 6464  ver","type":"add
-0001f520: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
-0001f530: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-0001f540: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001f550: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-0001f560: 2274 6f6b 656e 222c 2274 7970 6522 3a22  "token","type":"
-0001f570: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-0001f580: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0001f590: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001f5a0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001f5b0: 6e74 222c 2274 7970 6522 3a22 7569 6e74  nt","type":"uint
-0001f5c0: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
-0001f5d0: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
-0001f5e0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001f5f0: 226e 616d 6522 3a22 6665 6522 2c22 7479  "name":"fee","ty
-0001f600: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001f610: 226e 616d 6522 3a22 466c 6173 684c 6f61  "name":"FlashLoa
-0001f620: 6e22 2c22 7479 7065 223a 2265 7665 6e74  n","type":"event
-0001f630: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
-0001f640: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
-0001f650: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-0001f660: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f670: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001f680: 3a22 7072 6576 696f 7573 5369 7a65 222c  :"previousSize",
-0001f690: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001f6a0: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-0001f6b0: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-0001f6c0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001f6d0: 6522 3a22 6e65 7753 697a 6522 2c22 7479  e":"newSize","ty
-0001f6e0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001f6f0: 226e 616d 6522 3a22 4f72 6163 6c65 5369  "name":"OracleSi
-0001f700: 7a65 496e 6372 6561 7365 6422 2c22 7479  zeIncreased","ty
-0001f710: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
-0001f720: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
-0001f730: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
-0001f740: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0001f750: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001f760: 7322 2c22 6e61 6d65 223a 2273 656e 6465  s","name":"sende
-0001f770: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-0001f780: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
-0001f790: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-0001f7a0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001f7b0: 616d 6522 3a22 7265 6369 7069 656e 7422  ame":"recipient"
-0001f7c0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001f7d0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
-0001f7e0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-0001f7f0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001f800: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
-0001f810: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001f820: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-0001f830: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f840: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001f850: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
-0001f860: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001f870: 616d 6522 3a22 5072 6f74 6f63 6f6c 4665  ame":"ProtocolFe
-0001f880: 6573 436f 6c6c 6563 7465 6422 2c22 7479  esCollected","ty
-0001f890: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
-0001f8a0: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
-0001f8b0: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
-0001f8c0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0001f8d0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001f8e0: 7322 2c22 6e61 6d65 223a 2273 656e 6465  s","name":"sende
-0001f8f0: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-0001f900: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
-0001f910: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-0001f920: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001f930: 616d 6522 3a22 7265 6369 7069 656e 7422  ame":"recipient"
-0001f940: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001f950: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
-0001f960: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-0001f970: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001f980: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
-0001f990: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
-0001f9a0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0001f9b0: 726e 616c 5479 7065 223a 2262 6f6f 6c22  rnalType":"bool"
-0001f9c0: 2c22 6e61 6d65 223a 2273 7761 7046 6f72  ,"name":"swapFor
-0001f9d0: 5922 2c22 7479 7065 223a 2262 6f6f 6c22  Y","type":"bool"
-0001f9e0: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-0001f9f0: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-0001fa00: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001fa10: 6522 3a22 616d 6f75 6e74 496e 222c 2274  e":"amountIn","t
-0001fa20: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001fa30: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-0001fa40: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001fa50: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001fa60: 3a22 616d 6f75 6e74 4f75 7422 2c22 7479  :"amountOut","ty
-0001fa70: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0001fa80: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
-0001fa90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001faa0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001fab0: 2276 6f6c 6174 696c 6974 7941 6363 756d  "volatilityAccum
-0001fac0: 756c 6174 6564 222c 2274 7970 6522 3a22  ulated","type":"
-0001fad0: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
-0001fae0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0001faf0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001fb00: 3536 222c 226e 616d 6522 3a22 6665 6573  56","name":"fees
-0001fb10: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001fb20: 3622 7d5d 2c22 6e61 6d65 223a 2253 7761  6"}],"name":"Swa
-0001fb30: 7022 2c22 7479 7065 223a 2265 7665 6e74  p","type":"event
-0001fb40: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
-0001fb50: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
-0001fb60: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-0001fb70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001fb80: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001fb90: 2273 656e 6465 7222 2c22 7479 7065 223a  "sender","type":
-0001fba0: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-0001fbb0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
-0001fbc0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001fbd0: 7373 222c 226e 616d 6522 3a22 6672 6f6d  ss","name":"from
-0001fbe0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001fbf0: 7322 7d2c 7b22 696e 6465 7865 6422 3a74  s"},{"indexed":t
-0001fc00: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-0001fc10: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0001fc20: 6d65 223a 2274 6f22 2c22 7479 7065 223a  me":"to","type":
-0001fc30: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-0001fc40: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0001fc50: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001fc60: 3235 365b 5d22 2c22 6e61 6d65 223a 2269  256[]","name":"i
-0001fc70: 6473 222c 2274 7970 6522 3a22 7569 6e74  ds","type":"uint
-0001fc80: 3235 365b 5d22 7d2c 7b22 696e 6465 7865  256[]"},{"indexe
-0001fc90: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-0001fca0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001fcb0: 5b5d 222c 226e 616d 6522 3a22 616d 6f75  []","name":"amou
-0001fcc0: 6e74 7322 2c22 7479 7065 223a 2275 696e  nts","type":"uin
-0001fcd0: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
-0001fce0: 3a22 5472 616e 7366 6572 4261 7463 6822  :"TransferBatch"
-0001fcf0: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
-0001fd00: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
-0001fd10: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
-0001fd20: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-0001fd30: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-0001fd40: 6472 6573 7322 2c22 6e61 6d65 223a 2273  dress","name":"s
-0001fd50: 656e 6465 7222 2c22 7479 7065 223a 2261  ender","type":"a
-0001fd60: 6464 7265 7373 227d 2c7b 2269 6e64 6578  ddress"},{"index
-0001fd70: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
-0001fd80: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-0001fd90: 222c 226e 616d 6522 3a22 6672 6f6d 222c  ","name":"from",
-0001fda0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001fdb0: 7d2c 7b22 696e 6465 7865 6422 3a74 7275  },{"indexed":tru
-0001fdc0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001fdd0: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0001fde0: 223a 2274 6f22 2c22 7479 7065 223a 2261  ":"to","type":"a
-0001fdf0: 6464 7265 7373 227d 2c7b 2269 6e64 6578  ddress"},{"index
-0001fe00: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
-0001fe10: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001fe20: 3622 2c22 6e61 6d65 223a 2269 6422 2c22  6","name":"id","
-0001fe30: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001fe40: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001fe50: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001fe60: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001fe70: 223a 2261 6d6f 756e 7422 2c22 7479 7065  ":"amount","type
-0001fe80: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001fe90: 616d 6522 3a22 5472 616e 7366 6572 5369  ame":"TransferSi
-0001fea0: 6e67 6c65 222c 2274 7970 6522 3a22 6576  ngle","type":"ev
-0001feb0: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
-0001fec0: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
-0001fed0: 223a 5b7b 2269 6e64 6578 6564 223a 7472  ":[{"indexed":tr
-0001fee0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-0001fef0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0001ff00: 6522 3a22 7365 6e64 6572 222c 2274 7970  e":"sender","typ
-0001ff10: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001ff20: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-0001ff30: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-0001ff40: 6472 6573 7322 2c22 6e61 6d65 223a 2272  dress","name":"r
-0001ff50: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-0001ff60: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001ff70: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0001ff80: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001ff90: 3235 3622 2c22 6e61 6d65 223a 2269 6422  256","name":"id"
-0001ffa0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001ffb0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
-0001ffc0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-0001ffd0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001ffe0: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
-0001fff0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00020000: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-00020010: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-00020020: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00020030: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
-00020040: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00020050: 616d 6522 3a22 5769 7468 6472 6177 6e46  ame":"WithdrawnF
-00020060: 726f 6d42 696e 222c 2274 7970 6522 3a22  romBin","type":"
-00020070: 6576 656e 7422 7d2c 7b22 696e 7075 7473  event"},{"inputs
-00020080: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00020090: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-000200a0: 6d65 223a 225f 6163 636f 756e 7422 2c22  me":"_account","
-000200b0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-000200c0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000200d0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-000200e0: 223a 225f 6964 222c 2274 7970 6522 3a22  ":"_id","type":"
-000200f0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00020100: 223a 2262 616c 616e 6365 4f66 222c 226f  ":"balanceOf","o
-00020110: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00020120: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00020130: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
-00020140: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00020150: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00020160: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00020170: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00020180: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00020190: 6c54 7970 6522 3a22 6164 6472 6573 735b  lType":"address[
-000201a0: 5d22 2c22 6e61 6d65 223a 225f 6163 636f  ]","name":"_acco
-000201b0: 756e 7473 222c 2274 7970 6522 3a22 6164  unts","type":"ad
-000201c0: 6472 6573 735b 5d22 7d2c 7b22 696e 7465  dress[]"},{"inte
-000201d0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000201e0: 3536 5b5d 222c 226e 616d 6522 3a22 5f69  56[]","name":"_i
-000201f0: 6473 222c 2274 7970 6522 3a22 7569 6e74  ds","type":"uint
-00020200: 3235 365b 5d22 7d5d 2c22 6e61 6d65 223a  256[]"}],"name":
-00020210: 2262 616c 616e 6365 4f66 4261 7463 6822  "balanceOfBatch"
-00020220: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00020230: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00020240: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-00020250: 6261 7463 6842 616c 616e 6365 7322 2c22  batchBalances","
-00020260: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-00020270: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-00020280: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
-00020290: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-000202a0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-000202b0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000202c0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-000202d0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
-000202e0: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
-000202f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00020300: 365b 5d22 2c22 6e61 6d65 223a 225f 616d  6[]","name":"_am
-00020310: 6f75 6e74 7322 2c22 7479 7065 223a 2275  ounts","type":"u
-00020320: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
-00020330: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00020340: 6573 7322 2c22 6e61 6d65 223a 225f 746f  ess","name":"_to
-00020350: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00020360: 7322 7d5d 2c22 6e61 6d65 223a 2262 7572  s"}],"name":"bur
-00020370: 6e22 2c22 6f75 7470 7574 7322 3a5b 7b22  n","outputs":[{"
-00020380: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00020390: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000203a0: 616d 6f75 6e74 5822 2c22 7479 7065 223a  amountX","type":
-000203b0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-000203c0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000203d0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-000203e0: 756e 7459 222c 2274 7970 6522 3a22 7569  untY","type":"ui
-000203f0: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-00020400: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00020410: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00020420: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00020430: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00020440: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-00020450: 226e 616d 6522 3a22 5f61 6363 6f75 6e74  "name":"_account
-00020460: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00020470: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00020480: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-00020490: 226e 616d 6522 3a22 5f69 6473 222c 2274  "name":"_ids","t
-000204a0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-000204b0: 7d5d 2c22 6e61 6d65 223a 2263 6f6c 6c65  }],"name":"colle
-000204c0: 6374 4665 6573 222c 226f 7574 7075 7473  ctFees","outputs
-000204d0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-000204e0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-000204f0: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
-00020500: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00020510: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00020520: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00020530: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
-00020540: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
-00020550: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00020560: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
-00020570: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00020580: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00020590: 6d65 223a 2263 6f6c 6c65 6374 5072 6f74  me":"collectProt
-000205a0: 6f63 6f6c 4665 6573 222c 226f 7574 7075  ocolFees","outpu
-000205b0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-000205c0: 7970 6522 3a22 7569 6e74 3132 3822 2c22  ype":"uint128","
-000205d0: 6e61 6d65 223a 2261 6d6f 756e 7458 222c  name":"amountX",
-000205e0: 2274 7970 6522 3a22 7569 6e74 3132 3822  "type":"uint128"
-000205f0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00020600: 223a 2275 696e 7431 3238 222c 226e 616d  ":"uint128","nam
-00020610: 6522 3a22 616d 6f75 6e74 5922 2c22 7479  e":"amountY","ty
-00020620: 7065 223a 2275 696e 7431 3238 227d 5d2c  pe":"uint128"}],
-00020630: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00020640: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-00020650: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00020660: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00020670: 6e61 6d65 223a 2266 6163 746f 7279 222c  name":"factory",
-00020680: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00020690: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-000206a0: 7261 6374 2049 4c42 4661 6374 6f72 7922  ract ILBFactory"
-000206b0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-000206c0: 223a 2261 6464 7265 7373 227d 5d2c 2273  ":"address"}],"s
-000206d0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-000206e0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-000206f0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00020700: 7473 223a 5b5d 2c22 6e61 6d65 223a 2266  ts":[],"name":"f
-00020710: 6565 5061 7261 6d65 7465 7273 222c 226f  eeParameters","o
-00020720: 7574 7075 7473 223a 5b7b 2263 6f6d 706f  utputs":[{"compo
-00020730: 6e65 6e74 7322 3a5b 7b22 696e 7465 726e  nents":[{"intern
-00020740: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
-00020750: 2c22 6e61 6d65 223a 2262 696e 5374 6570  ,"name":"binStep
-00020760: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-00020770: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00020780: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
-00020790: 6522 3a22 6261 7365 4661 6374 6f72 222c  e":"baseFactor",
-000207a0: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-000207b0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000207c0: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-000207d0: 3a22 6669 6c74 6572 5065 7269 6f64 222c  :"filterPeriod",
-000207e0: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-000207f0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00020800: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00020810: 3a22 6465 6361 7950 6572 696f 6422 2c22  :"decayPeriod","
-00020820: 7479 7065 223a 2275 696e 7431 3622 7d2c  type":"uint16"},
-00020830: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00020840: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
-00020850: 2272 6564 7563 7469 6f6e 4661 6374 6f72  "reductionFactor
-00020860: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-00020870: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00020880: 6522 3a22 7569 6e74 3234 222c 226e 616d  e":"uint24","nam
-00020890: 6522 3a22 7661 7269 6162 6c65 4665 6543  e":"variableFeeC
-000208a0: 6f6e 7472 6f6c 222c 2274 7970 6522 3a22  ontrol","type":"
-000208b0: 7569 6e74 3234 227d 2c7b 2269 6e74 6572  uint24"},{"inter
-000208c0: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
-000208d0: 222c 226e 616d 6522 3a22 7072 6f74 6f63  ","name":"protoc
-000208e0: 6f6c 5368 6172 6522 2c22 7479 7065 223a  olShare","type":
-000208f0: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
-00020900: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00020910: 3422 2c22 6e61 6d65 223a 226d 6178 566f  4","name":"maxVo
-00020920: 6c61 7469 6c69 7479 4163 6375 6d75 6c61  latilityAccumula
-00020930: 7465 6422 2c22 7479 7065 223a 2275 696e  ted","type":"uin
-00020940: 7432 3422 7d2c 7b22 696e 7465 726e 616c  t24"},{"internal
-00020950: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-00020960: 6e61 6d65 223a 2276 6f6c 6174 696c 6974  name":"volatilit
-00020970: 7941 6363 756d 756c 6174 6564 222c 2274  yAccumulated","t
-00020980: 7970 6522 3a22 7569 6e74 3234 227d 2c7b  ype":"uint24"},{
-00020990: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000209a0: 7569 6e74 3234 222c 226e 616d 6522 3a22  uint24","name":"
-000209b0: 766f 6c61 7469 6c69 7479 5265 6665 7265  volatilityRefere
-000209c0: 6e63 6522 2c22 7479 7065 223a 2275 696e  nce","type":"uin
-000209d0: 7432 3422 7d2c 7b22 696e 7465 726e 616c  t24"},{"internal
-000209e0: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-000209f0: 6e61 6d65 223a 2269 6e64 6578 5265 6622  name":"indexRef"
-00020a00: 2c22 7479 7065 223a 2275 696e 7432 3422  ,"type":"uint24"
-00020a10: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00020a20: 223a 2275 696e 7434 3022 2c22 6e61 6d65  ":"uint40","name
-00020a30: 223a 2274 696d 6522 2c22 7479 7065 223a  ":"time","type":
-00020a40: 2275 696e 7434 3022 7d5d 2c22 696e 7465  "uint40"}],"inte
-00020a50: 726e 616c 5479 7065 223a 2273 7472 7563  rnalType":"struc
-00020a60: 7420 4665 6548 656c 7065 722e 4665 6550  t FeeHelper.FeeP
-00020a70: 6172 616d 6574 6572 7322 2c22 6e61 6d65  arameters","name
-00020a80: 223a 2222 2c22 7479 7065 223a 2274 7570  ":"","type":"tup
-00020a90: 6c65 227d 5d2c 2273 7461 7465 4d75 7461  le"}],"stateMuta
-00020aa0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-00020ab0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00020ac0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00020ad0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00020ae0: 6e74 3234 222c 226e 616d 6522 3a22 5f69  nt24","name":"_i
-00020af0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00020b00: 3422 7d2c 7b22 696e 7465 726e 616c 5479  4"},{"internalTy
-00020b10: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
-00020b20: 223a 225f 7377 6170 466f 7259 222c 2274  ":"_swapForY","t
-00020b30: 7970 6522 3a22 626f 6f6c 227d 5d2c 226e  ype":"bool"}],"n
-00020b40: 616d 6522 3a22 6669 6e64 4669 7273 744e  ame":"findFirstN
-00020b50: 6f6e 456d 7074 7942 696e 4964 222c 226f  onEmptyBinId","o
-00020b60: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00020b70: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
-00020b80: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00020b90: 6522 3a22 7569 6e74 3234 227d 5d2c 2273  e":"uint24"}],"s
-00020ba0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00020bb0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00020bc0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00020bd0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00020be0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00020bf0: 4c42 466c 6173 684c 6f61 6e43 616c 6c62  LBFlashLoanCallb
-00020c00: 6163 6b22 2c22 6e61 6d65 223a 225f 7265  ack","name":"_re
-00020c10: 6365 6976 6572 222c 2274 7970 6522 3a22  ceiver","type":"
-00020c20: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-00020c30: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-00020c40: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-00020c50: 6522 3a22 5f74 6f6b 656e 222c 2274 7970  e":"_token","typ
-00020c60: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00020c70: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00020c80: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00020c90: 5f61 6d6f 756e 7422 2c22 7479 7065 223a  _amount","type":
-00020ca0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00020cb0: 6572 6e61 6c54 7970 6522 3a22 6279 7465  ernalType":"byte
-00020cc0: 7322 2c22 6e61 6d65 223a 225f 6461 7461  s","name":"_data
-00020cd0: 222c 2274 7970 6522 3a22 6279 7465 7322  ","type":"bytes"
-00020ce0: 7d5d 2c22 6e61 6d65 223a 2266 6c61 7368  }],"name":"flash
-00020cf0: 4c6f 616e 222c 226f 7574 7075 7473 223a  Loan","outputs":
-00020d00: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
-00020d10: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
-00020d20: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00020d30: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-00020d40: 5d2c 226e 616d 6522 3a22 666f 7263 6544  ],"name":"forceD
-00020d50: 6563 6179 222c 226f 7574 7075 7473 223a  ecay","outputs":
-00020d60: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
-00020d70: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
-00020d80: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00020d90: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-00020da0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00020db0: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
-00020dc0: 225f 6964 222c 2274 7970 6522 3a22 7569  "_id","type":"ui
-00020dd0: 6e74 3234 227d 5d2c 226e 616d 6522 3a22  nt24"}],"name":"
-00020de0: 6765 7442 696e 222c 226f 7574 7075 7473  getBin","outputs
-00020df0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00020e00: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00020e10: 6d65 223a 2272 6573 6572 7665 5822 2c22  me":"reserveX","
-00020e20: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00020e30: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00020e40: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00020e50: 223a 2272 6573 6572 7665 5922 2c22 7479  ":"reserveY","ty
-00020e60: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00020e70: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00020e80: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00020e90: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00020ea0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-00020eb0: 2267 6574 476c 6f62 616c 4665 6573 222c  "getGlobalFees",
-00020ec0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00020ed0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00020ee0: 3132 3822 2c22 6e61 6d65 223a 2266 6565  128","name":"fee
-00020ef0: 7358 546f 7461 6c22 2c22 7479 7065 223a  sXTotal","type":
-00020f00: 2275 696e 7431 3238 227d 2c7b 2269 6e74  "uint128"},{"int
-00020f10: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00020f20: 3132 3822 2c22 6e61 6d65 223a 2266 6565  128","name":"fee
-00020f30: 7359 546f 7461 6c22 2c22 7479 7065 223a  sYTotal","type":
-00020f40: 2275 696e 7431 3238 227d 2c7b 2269 6e74  "uint128"},{"int
-00020f50: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00020f60: 3132 3822 2c22 6e61 6d65 223a 2266 6565  128","name":"fee
-00020f70: 7358 5072 6f74 6f63 6f6c 222c 2274 7970  sXProtocol","typ
-00020f80: 6522 3a22 7569 6e74 3132 3822 7d2c 7b22  e":"uint128"},{"
-00020f90: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00020fa0: 696e 7431 3238 222c 226e 616d 6522 3a22  int128","name":"
-00020fb0: 6665 6573 5950 726f 746f 636f 6c22 2c22  feesYProtocol","
-00020fc0: 7479 7065 223a 2275 696e 7431 3238 227d  type":"uint128"}
-00020fd0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00020fe0: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
-00020ff0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00021000: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00021010: 223a 2267 6574 4f72 6163 6c65 5061 7261  ":"getOraclePara
-00021020: 6d65 7465 7273 222c 226f 7574 7075 7473  meters","outputs
-00021030: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00021040: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00021050: 6d65 223a 226f 7261 636c 6553 616d 706c  me":"oracleSampl
-00021060: 654c 6966 6574 696d 6522 2c22 7479 7065  eLifetime","type
-00021070: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00021080: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00021090: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
-000210a0: 7261 636c 6553 697a 6522 2c22 7479 7065  racleSize","type
-000210b0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-000210c0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000210d0: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
-000210e0: 7261 636c 6541 6374 6976 6553 697a 6522  racleActiveSize"
-000210f0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00021100: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00021110: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00021120: 6d65 223a 226f 7261 636c 654c 6173 7454  me":"oracleLastT
-00021130: 696d 6573 7461 6d70 222c 2274 7970 6522  imestamp","type"
-00021140: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00021150: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00021160: 7432 3536 222c 226e 616d 6522 3a22 6f72  t256","name":"or
-00021170: 6163 6c65 4964 222c 2274 7970 6522 3a22  acleId","type":"
-00021180: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00021190: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000211a0: 3536 222c 226e 616d 6522 3a22 6d69 6e22  56","name":"min"
-000211b0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-000211c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000211d0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-000211e0: 6d65 223a 226d 6178 222c 2274 7970 6522  me":"max","type"
-000211f0: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
-00021200: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00021210: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
-00021220: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-00021230: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00021240: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00021250: 616d 6522 3a22 5f74 696d 6544 656c 7461  ame":"_timeDelta
-00021260: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00021270: 3622 7d5d 2c22 6e61 6d65 223a 2267 6574  6"}],"name":"get
-00021280: 4f72 6163 6c65 5361 6d70 6c65 4672 6f6d  OracleSampleFrom
-00021290: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-000212a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000212b0: 6e74 3235 3622 2c22 6e61 6d65 223a 2263  nt256","name":"c
-000212c0: 756d 756c 6174 6976 6549 6422 2c22 7479  umulativeId","ty
-000212d0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-000212e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000212f0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00021300: 2263 756d 756c 6174 6976 6556 6f6c 6174  "cumulativeVolat
-00021310: 696c 6974 7941 6363 756d 756c 6174 6564  ilityAccumulated
-00021320: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00021330: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00021340: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00021350: 616d 6522 3a22 6375 6d75 6c61 7469 7665  ame":"cumulative
-00021360: 4269 6e43 726f 7373 6564 222c 2274 7970  BinCrossed","typ
-00021370: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00021380: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00021390: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-000213a0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-000213b0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-000213c0: 6765 7452 6573 6572 7665 7341 6e64 4964  getReservesAndId
-000213d0: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-000213e0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000213f0: 6e74 3235 3622 2c22 6e61 6d65 223a 2272  nt256","name":"r
-00021400: 6573 6572 7665 5822 2c22 7479 7065 223a  eserveX","type":
-00021410: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00021420: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00021430: 3235 3622 2c22 6e61 6d65 223a 2272 6573  256","name":"res
-00021440: 6572 7665 5922 2c22 7479 7065 223a 2275  erveY","type":"u
-00021450: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00021460: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00021470: 3622 2c22 6e61 6d65 223a 2261 6374 6976  6","name":"activ
-00021480: 6549 6422 2c22 7479 7065 223a 2275 696e  eId","type":"uin
-00021490: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
-000214a0: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
-000214b0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-000214c0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-000214d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000214e0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
-000214f0: 5f6e 6577 4c65 6e67 7468 222c 2274 7970  _newLength","typ
-00021500: 6522 3a22 7569 6e74 3136 227d 5d2c 226e  e":"uint16"}],"n
-00021510: 616d 6522 3a22 696e 6372 6561 7365 4f72  ame":"increaseOr
-00021520: 6163 6c65 4c65 6e67 7468 222c 226f 7574  acleLength","out
-00021530: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-00021540: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00021550: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00021560: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00021570: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00021580: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00021590: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-000215a0: 5f74 6f6b 656e 5822 2c22 7479 7065 223a  _tokenX","type":
-000215b0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-000215c0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-000215d0: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-000215e0: 6d65 223a 225f 746f 6b65 6e59 222c 2274  me":"_tokenY","t
-000215f0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-00021600: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021610: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
-00021620: 225f 6163 7469 7665 4964 222c 2274 7970  "_activeId","typ
-00021630: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
-00021640: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00021650: 6e74 3136 222c 226e 616d 6522 3a22 5f73  nt16","name":"_s
-00021660: 616d 706c 654c 6966 6574 696d 6522 2c22  ampleLifetime","
-00021670: 7479 7065 223a 2275 696e 7431 3622 7d2c  type":"uint16"},
-00021680: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021690: 2262 7974 6573 3332 222c 226e 616d 6522  "bytes32","name"
-000216a0: 3a22 5f70 6163 6b65 6446 6565 5061 7261  :"_packedFeePara
-000216b0: 6d65 7465 7273 222c 2274 7970 6522 3a22  meters","type":"
-000216c0: 6279 7465 7333 3222 7d5d 2c22 6e61 6d65  bytes32"}],"name
-000216d0: 223a 2269 6e69 7469 616c 697a 6522 2c22  ":"initialize","
-000216e0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-000216f0: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00021700: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00021710: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00021720: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00021730: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00021740: 7322 2c22 6e61 6d65 223a 225f 6f77 6e65  s","name":"_owne
-00021750: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-00021760: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-00021770: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-00021780: 6e61 6d65 223a 225f 7370 656e 6465 7222  name":"_spender"
-00021790: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-000217a0: 227d 5d2c 226e 616d 6522 3a22 6973 4170  "}],"name":"isAp
-000217b0: 7072 6f76 6564 466f 7241 6c6c 222c 226f  provedForAll","o
-000217c0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-000217d0: 6e61 6c54 7970 6522 3a22 626f 6f6c 222c  nalType":"bool",
-000217e0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
-000217f0: 3a22 626f 6f6c 227d 5d2c 2273 7461 7465  :"bool"}],"state
-00021800: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-00021810: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-00021820: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00021830: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00021840: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-00021850: 6d65 223a 225f 6964 7322 2c22 7479 7065  me":"_ids","type
-00021860: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
-00021870: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00021880: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
-00021890: 223a 225f 6469 7374 7269 6275 7469 6f6e  ":"_distribution
-000218a0: 5822 2c22 7479 7065 223a 2275 696e 7432  X","type":"uint2
-000218b0: 3536 5b5d 227d 2c7b 2269 6e74 6572 6e61  56[]"},{"interna
-000218c0: 6c54 7970 6522 3a22 7569 6e74 3235 365b  lType":"uint256[
-000218d0: 5d22 2c22 6e61 6d65 223a 225f 6469 7374  ]","name":"_dist
-000218e0: 7269 6275 7469 6f6e 5922 2c22 7479 7065  ributionY","type
-000218f0: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
-00021900: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00021910: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00021920: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
-00021930: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
-00021940: 226d 696e 7422 2c22 6f75 7470 7574 7322  "mint","outputs"
-00021950: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00021960: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00021970: 6522 3a22 222c 2274 7970 6522 3a22 7569  e":"","type":"ui
-00021980: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-00021990: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000219a0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-000219b0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-000219c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-000219d0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
-000219e0: 3a22 6c69 7175 6964 6974 794d 696e 7465  :"liquidityMinte
-000219f0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00021a00: 3536 5b5d 227d 5d2c 2273 7461 7465 4d75  56[]"}],"stateMu
-00021a10: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-00021a20: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-00021a30: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00021a40: 7473 223a 5b5d 2c22 6e61 6d65 223a 226e  ts":[],"name":"n
-00021a50: 616d 6522 2c22 6f75 7470 7574 7322 3a5b  ame","outputs":[
-00021a60: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021a70: 2273 7472 696e 6722 2c22 6e61 6d65 223a  "string","name":
-00021a80: 2222 2c22 7479 7065 223a 2273 7472 696e  "","type":"strin
-00021a90: 6722 7d5d 2c22 7374 6174 654d 7574 6162  g"}],"stateMutab
-00021aa0: 696c 6974 7922 3a22 7075 7265 222c 2274  ility":"pure","t
-00021ab0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00021ac0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00021ad0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00021ae0: 7265 7373 222c 226e 616d 6522 3a22 5f61  ress","name":"_a
-00021af0: 6363 6f75 6e74 222c 2274 7970 6522 3a22  ccount","type":"
-00021b00: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-00021b10: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00021b20: 3536 5b5d 222c 226e 616d 6522 3a22 5f69  56[]","name":"_i
-00021b30: 6473 222c 2274 7970 6522 3a22 7569 6e74  ds","type":"uint
-00021b40: 3235 365b 5d22 7d5d 2c22 6e61 6d65 223a  256[]"}],"name":
-00021b50: 2270 656e 6469 6e67 4665 6573 222c 226f  "pendingFees","o
-00021b60: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00021b70: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00021b80: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-00021b90: 7458 222c 2274 7970 6522 3a22 7569 6e74  tX","type":"uint
-00021ba0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00021bb0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00021bc0: 226e 616d 6522 3a22 616d 6f75 6e74 5922  "name":"amountY"
-00021bd0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00021be0: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-00021bf0: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
-00021c00: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00021c10: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-00021c20: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00021c30: 6573 7322 2c22 6e61 6d65 223a 225f 6672  ess","name":"_fr
-00021c40: 6f6d 222c 2274 7970 6522 3a22 6164 6472  om","type":"addr
-00021c50: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-00021c60: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-00021c70: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
-00021c80: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-00021c90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00021ca0: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
-00021cb0: 223a 225f 6964 7322 2c22 7479 7065 223a  ":"_ids","type":
-00021cc0: 2275 696e 7432 3536 5b5d 227d 2c7b 2269  "uint256[]"},{"i
-00021cd0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00021ce0: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-00021cf0: 225f 616d 6f75 6e74 7322 2c22 7479 7065  "_amounts","type
-00021d00: 223a 2275 696e 7432 3536 5b5d 227d 5d2c  ":"uint256[]"}],
-00021d10: 226e 616d 6522 3a22 7361 6665 4261 7463  "name":"safeBatc
-00021d20: 6854 7261 6e73 6665 7246 726f 6d22 2c22  hTransferFrom","
-00021d30: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00021d40: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00021d50: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00021d60: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00021d70: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00021d80: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00021d90: 7322 2c22 6e61 6d65 223a 225f 6672 6f6d  s","name":"_from
-00021da0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00021db0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00021dc0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-00021dd0: 616d 6522 3a22 5f74 6f22 2c22 7479 7065  ame":"_to","type
-00021de0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00021df0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00021e00: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-00021e10: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-00021e20: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00021e30: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00021e40: 226e 616d 6522 3a22 5f61 6d6f 756e 7422  "name":"_amount"
-00021e50: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00021e60: 227d 5d2c 226e 616d 6522 3a22 7361 6665  "}],"name":"safe
-00021e70: 5472 616e 7366 6572 4672 6f6d 222c 226f  TransferFrom","o
-00021e80: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
-00021e90: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-00021ea0: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-00021eb0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00021ec0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00021ed0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00021ee0: 222c 226e 616d 6522 3a22 5f73 7065 6e64  ","name":"_spend
-00021ef0: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-00021f00: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-00021f10: 5479 7065 223a 2262 6f6f 6c22 2c22 6e61  Type":"bool","na
-00021f20: 6d65 223a 225f 6170 7072 6f76 6564 222c  me":"_approved",
-00021f30: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-00021f40: 226e 616d 6522 3a22 7365 7441 7070 726f  "name":"setAppro
-00021f50: 7661 6c46 6f72 416c 6c22 2c22 6f75 7470  valForAll","outp
-00021f60: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-00021f70: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-00021f80: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-00021f90: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00021fa0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00021fb0: 7970 6522 3a22 6279 7465 7333 3222 2c22  ype":"bytes32","
-00021fc0: 6e61 6d65 223a 225f 7061 636b 6564 4665  name":"_packedFe
-00021fd0: 6550 6172 616d 6574 6572 7322 2c22 7479  eParameters","ty
-00021fe0: 7065 223a 2262 7974 6573 3332 227d 5d2c  pe":"bytes32"}],
-00021ff0: 226e 616d 6522 3a22 7365 7446 6565 7350  "name":"setFeesP
-00022000: 6172 616d 6574 6572 7322 2c22 6f75 7470  arameters","outp
-00022010: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-00022020: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-00022030: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-00022040: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00022050: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00022060: 7970 6522 3a22 6279 7465 7334 222c 226e  ype":"bytes4","n
-00022070: 616d 6522 3a22 5f69 6e74 6572 6661 6365  ame":"_interface
-00022080: 4964 222c 2274 7970 6522 3a22 6279 7465  Id","type":"byte
-00022090: 7334 227d 5d2c 226e 616d 6522 3a22 7375  s4"}],"name":"su
-000220a0: 7070 6f72 7473 496e 7465 7266 6163 6522  pportsInterface"
-000220b0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-000220c0: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
-000220d0: 6c22 2c22 6e61 6d65 223a 2222 2c22 7479  l","name":"","ty
-000220e0: 7065 223a 2262 6f6f 6c22 7d5d 2c22 7374  pe":"bool"}],"st
-000220f0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00022100: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
-00022110: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-00022120: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00022130: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
-00022140: 223a 225f 7377 6170 466f 7259 222c 2274  ":"_swapForY","t
-00022150: 7970 6522 3a22 626f 6f6c 227d 2c7b 2269  ype":"bool"},{"i
-00022160: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-00022170: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
-00022180: 746f 222c 2274 7970 6522 3a22 6164 6472  to","type":"addr
-00022190: 6573 7322 7d5d 2c22 6e61 6d65 223a 2273  ess"}],"name":"s
-000221a0: 7761 7022 2c22 6f75 7470 7574 7322 3a5b  wap","outputs":[
-000221b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000221c0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-000221d0: 3a22 616d 6f75 6e74 584f 7574 222c 2274  :"amountXOut","t
-000221e0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-000221f0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00022200: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00022210: 3a22 616d 6f75 6e74 594f 7574 222c 2274  :"amountYOut","t
-00022220: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00022230: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00022240: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
-00022250: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00022260: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-00022270: 226e 616d 6522 3a22 7379 6d62 6f6c 222c  "name":"symbol",
-00022280: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00022290: 6572 6e61 6c54 7970 6522 3a22 7374 7269  ernalType":"stri
-000222a0: 6e67 222c 226e 616d 6522 3a22 222c 2274  ng","name":"","t
-000222b0: 7970 6522 3a22 7374 7269 6e67 227d 5d2c  ype":"string"}],
-000222c0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-000222d0: 223a 2270 7572 6522 2c22 7479 7065 223a  ":"pure","type":
-000222e0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000222f0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-00022300: 2274 6f6b 656e 5822 2c22 6f75 7470 7574  "tokenX","output
-00022310: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00022320: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-00022330: 5243 3230 222c 226e 616d 6522 3a22 222c  RC20","name":"",
-00022340: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-00022350: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-00022360: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-00022370: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00022380: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00022390: 6522 3a22 746f 6b65 6e59 222c 226f 7574  e":"tokenY","out
-000223a0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000223b0: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-000223c0: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-000223d0: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-000223e0: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-000223f0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-00022400: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00022410: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00022420: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00022430: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-00022440: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-00022450: 3235 3622 7d5d 2c22 6e61 6d65 223a 2274  256"}],"name":"t
-00022460: 6f74 616c 5375 7070 6c79 222c 226f 7574  otalSupply","out
-00022470: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00022480: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00022490: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-000224a0: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
-000224b0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-000224c0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-000224d0: 756e 6374 696f 6e22 7d5d 2729 0a0a 2020  unction"}]')..  
-000224e0: 2020 2320 7265 7475 726e 7320 2875 696e    # returns (uin
-000224f0: 7432 3536 2072 6573 6572 7665 582c 2075  t256 reserveX, u
-00022500: 696e 7432 3536 2072 6573 6572 7665 592c  int256 reserveY,
-00022510: 2075 696e 7432 3536 2061 6374 6976 6549   uint256 activeI
-00022520: 6429 0a20 2020 2064 6566 2067 6574 5f72  d).    def get_r
-00022530: 6573 6572 7665 5f61 6e64 5f69 6428 5f77  eserve_and_id(_w
-00022540: 6562 333a 5765 6233 2c5f 7061 6972 5f61  eb3:Web3,_pair_a
-00022550: 6464 7265 7373 3a73 7472 293a 0a20 2020  ddress:str):.   
-00022560: 2020 2020 2070 6169 725f 636f 6e74 7261       pair_contra
-00022570: 6374 3d5f 7765 6233 2e65 7468 2e63 6f6e  ct=_web3.eth.con
-00022580: 7472 6163 7428 6164 6472 6573 733d 5f70  tract(address=_p
-00022590: 6169 725f 6164 6472 6573 732c 2061 6269  air_address, abi
-000225a0: 3d4a 6f65 5632 5061 6972 2e6a 6f65 5f70  =JoeV2Pair.joe_p
-000225b0: 6169 725f 7632 5f61 6269 290a 2020 2020  air_v2_abi).    
-000225c0: 2020 2020 7265 7475 726e 2070 6169 725f      return pair_
-000225d0: 636f 6e74 7261 6374 2e66 756e 6374 696f  contract.functio
-000225e0: 6e73 2e67 6574 5265 7365 7276 6573 416e  ns.getReservesAn
-000225f0: 6449 6428 292e 6361 6c6c 2829 0a0a 2020  dId().call()..  
-00022600: 2020 2320 6675 6e63 7469 6f6e 2067 6574    # function get
-00022610: 476c 6f62 616c 4665 6573 2829 2065 7874  GlobalFees() ext
-00022620: 6572 6e61 6c20 7669 6577 206f 7665 7272  ernal view overr
-00022630: 6964 6520 7265 7475 726e 7320 2875 696e  ide returns (uin
-00022640: 7432 3536 2066 6565 7358 546f 7461 6c2c  t256 feesXTotal,
-00022650: 2075 696e 7432 3536 2066 6565 7359 546f   uint256 feesYTo
-00022660: 7461 6c2c 2075 696e 7432 3536 2066 6565  tal, uint256 fee
-00022670: 7358 5072 6f74 6f63 6f6c 2c20 7569 6e74  sXProtocol, uint
-00022680: 3235 3620 6665 6573 5950 726f 746f 636f  256 feesYProtoco
-00022690: 6c29 0a20 2020 2064 6566 2067 6574 5f67  l).    def get_g
-000226a0: 6c6f 6261 6c5f 6665 6528 5f77 6562 333a  lobal_fee(_web3:
-000226b0: 5765 6233 2c5f 7061 6972 5f61 6464 7265  Web3,_pair_addre
-000226c0: 7373 3a73 7472 293a 0a20 2020 2020 2020  ss:str):.       
-000226d0: 2070 6169 725f 636f 6e74 7261 6374 3d5f   pair_contract=_
-000226e0: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
-000226f0: 7428 6164 6472 6573 733d 5f70 6169 725f  t(address=_pair_
-00022700: 6164 6472 6573 732c 2061 6269 3d4a 6f65  address, abi=Joe
-00022710: 5632 5061 6972 2e6a 6f65 5f70 6169 725f  V2Pair.joe_pair_
-00022720: 7632 5f61 6269 290a 2020 2020 2020 2020  v2_abi).        
-00022730: 7265 7475 726e 2070 6169 725f 636f 6e74  return pair_cont
-00022740: 7261 6374 2e66 756e 6374 696f 6e73 2e67  ract.functions.g
-00022750: 6574 476c 6f62 616c 4665 6573 2829 2e63  etGlobalFees().c
-00022760: 616c 6c28 290a 0a20 2020 2023 2066 756e  all()..    # fun
-00022770: 6374 696f 6e20 6669 6e64 4669 7273 744e  ction findFirstN
-00022780: 6f6e 456d 7074 7942 696e 4964 2875 696e  onEmptyBinId(uin
-00022790: 7432 3420 5f69 642c 2062 6f6f 6c20 5f73  t24 _id, bool _s
-000227a0: 7761 7046 6f72 5929 2065 7874 6572 6e61  wapForY) externa
-000227b0: 6c20 7669 6577 206f 7665 7272 6964 6520  l view override 
-000227c0: 7265 7475 726e 7320 2875 696e 7432 3429  returns (uint24)
-000227d0: 0a20 2020 2064 6566 2066 696e 645f 6669  .    def find_fi
-000227e0: 7273 745f 6e6f 6e5f 656d 7074 795f 6269  rst_non_empty_bi
-000227f0: 6e5f 6964 285f 7765 6233 3a57 6562 332c  n_id(_web3:Web3,
-00022800: 5f70 6169 725f 6164 6472 6573 733a 7374  _pair_address:st
-00022810: 722c 5f69 642c 5f73 7761 705f 666f 725f  r,_id,_swap_for_
-00022820: 7929 3a0a 2020 2020 2020 2020 7061 6972  y):.        pair
-00022830: 5f63 6f6e 7472 6163 743d 5f77 6562 332e  _contract=_web3.
-00022840: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-00022850: 7265 7373 3d5f 7061 6972 5f61 6464 7265  ress=_pair_addre
-00022860: 7373 2c20 6162 693d 4a6f 6556 3250 6169  ss, abi=JoeV2Pai
-00022870: 722e 6a6f 655f 7061 6972 5f76 325f 6162  r.joe_pair_v2_ab
-00022880: 6929 0a20 2020 2020 2020 2072 6574 7572  i).        retur
-00022890: 6e20 7061 6972 5f63 6f6e 7472 6163 742e  n pair_contract.
-000228a0: 6675 6e63 7469 6f6e 732e 6669 6e64 4669  functions.findFi
-000228b0: 7273 744e 6f6e 456d 7074 7942 696e 4964  rstNonEmptyBinId
-000228c0: 285f 6964 2c5f 7377 6170 5f66 6f72 5f79  (_id,_swap_for_y
-000228d0: 292e 6361 6c6c 2829 0a0a 2020 2020 2320  ).call()..    # 
-000228e0: 6675 6e63 7469 6f6e 2067 6574 4269 6e28  function getBin(
-000228f0: 7569 6e74 3234 205f 6964 2920 6578 7465  uint24 _id) exte
-00022900: 726e 616c 2076 6965 7720 6f76 6572 7269  rnal view overri
-00022910: 6465 2072 6574 7572 6e73 2028 7569 6e74  de returns (uint
-00022920: 3235 3620 7265 7365 7276 6558 2c20 7569  256 reserveX, ui
-00022930: 6e74 3235 3620 7265 7365 7276 6559 290a  nt256 reserveY).
-00022940: 2020 2020 6465 6620 6765 745f 6269 6e28      def get_bin(
-00022950: 5f77 6562 333a 5765 6233 2c5f 7061 6972  _web3:Web3,_pair
-00022960: 5f61 6464 7265 7373 3a73 7472 2c5f 6964  _address:str,_id
-00022970: 293a 0a20 2020 2020 2020 2070 6169 725f  ):.        pair_
-00022980: 636f 6e74 7261 6374 3d5f 7765 6233 2e65  contract=_web3.e
-00022990: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-000229a0: 6573 733d 5f70 6169 725f 6164 6472 6573  ess=_pair_addres
-000229b0: 732c 2061 6269 3d4a 6f65 5632 5061 6972  s, abi=JoeV2Pair
-000229c0: 2e6a 6f65 5f70 6169 725f 7632 5f61 6269  .joe_pair_v2_abi
-000229d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000229e0: 2070 6169 725f 636f 6e74 7261 6374 2e66   pair_contract.f
-000229f0: 756e 6374 696f 6e73 2e67 6574 4269 6e28  unctions.getBin(
-00022a00: 5f69 6429 2e63 616c 6c28 290a 0a20 2020  _id).call()..   
-00022a10: 2023 2066 756e 6374 696f 6e20 7377 6170   # function swap
-00022a20: 2862 6f6f 6c20 5f73 7761 7046 6f72 592c  (bool _swapForY,
-00022a30: 2061 6464 7265 7373 205f 746f 2920 6578   address _to) ex
-00022a40: 7465 726e 616c 206f 7665 7272 6964 6520  ternal override 
-00022a50: 6e6f 6e52 6565 6e74 7261 6e74 2072 6574  nonReentrant ret
-00022a60: 7572 6e73 2028 7569 6e74 3235 3620 616d  urns (uint256 am
-00022a70: 6f75 6e74 584f 7574 2c20 7569 6e74 3235  ountXOut, uint25
-00022a80: 3620 616d 6f75 6e74 594f 7574 290a 2020  6 amountYOut).  
-00022a90: 2020 6465 6620 7377 6170 285f 7765 6233    def swap(_web3
-00022aa0: 3a57 6562 332c 5f70 6169 725f 6164 6472  :Web3,_pair_addr
-00022ab0: 6573 733a 7374 722c 5f73 7761 705f 666f  ess:str,_swap_fo
-00022ac0: 725f 792c 5f74 6f29 3a0a 2020 2020 2020  r_y,_to):.      
-00022ad0: 2020 7061 6972 5f63 6f6e 7472 6163 743d    pair_contract=
-00022ae0: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
-00022af0: 6374 2861 6464 7265 7373 3d5f 7061 6972  ct(address=_pair
-00022b00: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
-00022b10: 6556 3250 6169 722e 6a6f 655f 7061 6972  eV2Pair.joe_pair
-00022b20: 5f76 325f 6162 6929 0a20 2020 2020 2020  _v2_abi).       
-00022b30: 2072 6574 7572 6e20 7061 6972 5f63 6f6e   return pair_con
-00022b40: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-00022b50: 7377 6170 285f 7377 6170 5f66 6f72 5f79  swap(_swap_for_y
-00022b60: 2c5f 746f 292e 6361 6c6c 2829            ,_to).call()
+0000b050: 5374 616d 700a 0a0a 2020 2020 6465 6620  Stamp...    def 
+0000b060: 6765 745f 7061 6972 5f69 6e66 6f28 7365  get_pair_info(se
+0000b070: 6c66 2c70 6169 725f 6164 6472 6573 7329  lf,pair_address)
+0000b080: 3a0a 2020 2020 2020 2020 7061 6972 436f  :.        pairCo
+0000b090: 6e74 7261 6374 3d73 656c 662e 7765 6233  ntract=self.web3
+0000b0a0: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
+0000b0b0: 6472 6573 733d 7061 6972 5f61 6464 7265  dress=pair_addre
+0000b0c0: 7373 2c20 6162 693d 7365 6c66 2e70 6169  ss, abi=self.pai
+0000b0d0: 725f 6162 6929 0a20 2020 2020 2020 2074  r_abi).        t
+0000b0e0: 6f6b 656e 3041 6464 7265 7373 3d70 6169  oken0Address=pai
+0000b0f0: 7243 6f6e 7472 6163 742e 6675 6e63 7469  rContract.functi
+0000b100: 6f6e 732e 746f 6b65 6e30 2829 2e63 616c  ons.token0().cal
+0000b110: 6c28 290a 2020 2020 2020 2020 746f 6b65  l().        toke
+0000b120: 6e31 4164 6472 6573 733d 7061 6972 436f  n1Address=pairCo
+0000b130: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+0000b140: 2e74 6f6b 656e 3128 292e 6361 6c6c 2829  .token1().call()
+0000b150: 0a20 2020 2020 2020 2072 6573 6572 7665  .        reserve
+0000b160: 302c 7265 7365 7276 6531 2c62 6c6f 636b  0,reserve1,block
+0000b170: 5469 6d65 5374 616d 703d 7061 6972 436f  TimeStamp=pairCo
+0000b180: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+0000b190: 2e67 6574 5265 7365 7276 6573 2829 2e63  .getReserves().c
+0000b1a0: 616c 6c28 290a 2020 2020 2020 2020 2320  all().        # 
+0000b1b0: 746f 6b65 6e30 5f63 6f6e 7472 6163 743d  token0_contract=
+0000b1c0: 7365 6c66 2e77 6562 332e 6574 682e 636f  self.web3.eth.co
+0000b1d0: 6e74 7261 6374 2861 6464 7265 7373 3d74  ntract(address=t
+0000b1e0: 6f6b 656e 3041 6464 7265 7373 2c20 6162  oken0Address, ab
+0000b1f0: 693d 7365 6c66 2e65 7263 3230 5f61 6269  i=self.erc20_abi
+0000b200: 290a 2020 2020 2020 2020 2320 746f 6b65  ).        # toke
+0000b210: 6e31 5f63 6f6e 7472 6163 743d 7365 6c66  n1_contract=self
+0000b220: 2e77 6562 332e 6574 682e 636f 6e74 7261  .web3.eth.contra
+0000b230: 6374 2861 6464 7265 7373 3d74 6f6b 656e  ct(address=token
+0000b240: 3141 6464 7265 7373 2c20 6162 693d 7365  1Address, abi=se
+0000b250: 6c66 2e65 7263 3230 5f61 6269 290a 2020  lf.erc20_abi).  
+0000b260: 2020 2020 2020 2320 746f 6b65 6e30 5f6e        # token0_n
+0000b270: 616d 653d 746f 6b65 6e30 5f63 6f6e 7472  ame=token0_contr
+0000b280: 6163 742e 6675 6e63 7469 6f6e 732e 6e61  act.functions.na
+0000b290: 6d65 2829 2e63 616c 6c28 290a 2020 2020  me().call().    
+0000b2a0: 2020 2020 2320 746f 6b65 6e31 5f6e 616d      # token1_nam
+0000b2b0: 653d 746f 6b65 6e31 5f63 6f6e 7472 6163  e=token1_contrac
+0000b2c0: 742e 6675 6e63 7469 6f6e 732e 6e61 6d65  t.functions.name
+0000b2d0: 2829 2e63 616c 6c28 290a 2020 2020 2020  ().call().      
+0000b2e0: 2020 7072 6963 6530 3d72 6573 6572 7665    price0=reserve
+0000b2f0: 312f 7265 7365 7276 6530 0a20 2020 2020  1/reserve0.     
+0000b300: 2020 2070 7269 6365 313d 7265 7365 7276     price1=reserv
+0000b310: 6530 2f72 6573 6572 7665 310a 2020 2020  e0/reserve1.    
+0000b320: 2020 2020 2320 7072 696e 7428 2274 6f6b      # print("tok
+0000b330: 656e 303a 222c 7374 7228 746f 6b65 6e30  en0:",str(token0
+0000b340: 4164 6472 6573 7329 2c22 2d2d 6e61 6d65  Address),"--name
+0000b350: 3a22 2c73 7472 2874 6f6b 656e 305f 6e61  :",str(token0_na
+0000b360: 6d65 292c 222d 2d70 7269 6365 3a22 2c73  me),"--price:",s
+0000b370: 7472 2870 7269 6365 3029 290a 2020 2020  tr(price0)).    
+0000b380: 2020 2020 2320 7072 696e 7428 2274 6f6b      # print("tok
+0000b390: 656e 313a 222c 7374 7228 746f 6b65 6e31  en1:",str(token1
+0000b3a0: 4164 6472 6573 7329 2c22 2d2d 6e61 6d65  Address),"--name
+0000b3b0: 3a22 2c73 7472 2874 6f6b 656e 315f 6e61  :",str(token1_na
+0000b3c0: 6d65 292c 222d 2d70 7269 6365 3a22 2c73  me),"--price:",s
+0000b3d0: 7472 2870 7269 6365 3129 290a 2020 2020  tr(price1)).    
+0000b3e0: 2020 2020 2320 7072 696e 7428 2272 6573      # print("res
+0000b3f0: 6572 7665 3022 2c73 7472 2872 6573 6572  erve0",str(reser
+0000b400: 7665 3029 290a 2020 2020 2020 2020 2320  ve0)).        # 
+0000b410: 7072 696e 7428 2272 6573 6572 7665 3122  print("reserve1"
+0000b420: 2c73 7472 2872 6573 6572 7665 3129 290a  ,str(reserve1)).
+0000b430: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
+0000b440: 2262 6c6f 636b 5469 6d65 5374 616d 7022  "blockTimeStamp"
+0000b450: 2c73 7472 2862 6c6f 636b 5469 6d65 5374  ,str(blockTimeSt
+0000b460: 616d 7029 290a 2020 2020 2020 2020 7265  amp)).        re
+0000b470: 7475 726e 2074 6f6b 656e 3041 6464 7265  turn token0Addre
+0000b480: 7373 2c72 6573 6572 7665 302c 746f 6b65  ss,reserve0,toke
+0000b490: 6e31 4164 6472 6573 732c 7265 7365 7276  n1Address,reserv
+0000b4a0: 6531 2c62 6c6f 636b 5469 6d65 5374 616d  e1,blockTimeStam
+0000b4b0: 702c 7072 6963 6530 2c70 7269 6365 310a  p,price0,price1.
+0000b4c0: 0a63 6c61 7373 2055 6e69 7377 6170 5632  .class UniswapV2
+0000b4d0: 5061 6972 3a0a 0a20 2020 2064 6566 2067  Pair:..    def g
+0000b4e0: 6574 5f72 6573 6572 7665 7328 5f77 6562  et_reserves(_web
+0000b4f0: 333a 5765 6233 2c5f 7061 6972 5f61 6464  3:Web3,_pair_add
+0000b500: 7265 7373 2c5f 7061 6972 5f61 6269 293a  ress,_pair_abi):
+0000b510: 0a20 2020 2020 2020 2070 6169 725f 636f  .        pair_co
+0000b520: 6e74 7261 6374 3d5f 7765 6233 2e65 7468  ntract=_web3.eth
+0000b530: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
+0000b540: 733d 5f70 6169 725f 6164 6472 6573 732c  s=_pair_address,
+0000b550: 6162 693d 5f70 6169 725f 6162 6929 0a20  abi=_pair_abi). 
+0000b560: 2020 2020 2020 2072 6573 6572 7665 302c         reserve0,
+0000b570: 7265 7365 7276 6531 2c62 6c6f 636b 5469  reserve1,blockTi
+0000b580: 6d65 5374 616d 703d 7061 6972 5f63 6f6e  meStamp=pair_con
+0000b590: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
+0000b5a0: 6765 7452 6573 6572 7665 7328 292e 6361  getReserves().ca
+0000b5b0: 6c6c 2829 0a20 2020 2020 2020 2072 6574  ll().        ret
+0000b5c0: 7572 6e20 7265 7365 7276 6530 2c72 6573  urn reserve0,res
+0000b5d0: 6572 7665 312c 626c 6f63 6b54 696d 6553  erve1,blockTimeS
+0000b5e0: 7461 6d70 0a0a 636c 6173 7320 556e 6973  tamp..class Unis
+0000b5f0: 7761 7056 333a 0a20 2020 2023 6874 7470  wapV3:.    #http
+0000b600: 733a 2f2f 6574 6865 7273 6361 6e2e 696f  s://etherscan.io
+0000b610: 2f61 6464 7265 7373 2f30 7831 6639 3834  /address/0x1f984
+0000b620: 3331 6338 6164 3938 3532 3336 3331 6165  31c8ad98523631ae
+0000b630: 3461 3539 6632 3637 3334 3665 6133 3166  4a59f267346ea31f
+0000b640: 3938 340a 2020 2020 756e 6973 7761 705f  984.    uniswap_
+0000b650: 7633 5f66 6163 746f 7279 5f61 6269 3d27  v3_factory_abi='
+0000b660: 5b7b 2269 6e70 7574 7322 3a5b 5d2c 2273  [{"inputs":[],"s
+0000b670: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000b680: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
+0000b690: 7065 223a 2263 6f6e 7374 7275 6374 6f72  pe":"constructor
+0000b6a0: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
+0000b6b0: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
+0000b6c0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
+0000b6d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000b6e0: 7569 6e74 3234 222c 226e 616d 6522 3a22  uint24","name":"
+0000b6f0: 6665 6522 2c22 7479 7065 223a 2275 696e  fee","type":"uin
+0000b700: 7432 3422 7d2c 7b22 696e 6465 7865 6422  t24"},{"indexed"
+0000b710: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
+0000b720: 7970 6522 3a22 696e 7432 3422 2c22 6e61  ype":"int24","na
+0000b730: 6d65 223a 2274 6963 6b53 7061 6369 6e67  me":"tickSpacing
+0000b740: 222c 2274 7970 6522 3a22 696e 7432 3422  ","type":"int24"
+0000b750: 7d5d 2c22 6e61 6d65 223a 2246 6565 416d  }],"name":"FeeAm
+0000b760: 6f75 6e74 456e 6162 6c65 6422 2c22 7479  ountEnabled","ty
+0000b770: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
+0000b780: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
+0000b790: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
+0000b7a0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0000b7b0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0000b7c0: 7322 2c22 6e61 6d65 223a 226f 6c64 4f77  s","name":"oldOw
+0000b7d0: 6e65 7222 2c22 7479 7065 223a 2261 6464  ner","type":"add
+0000b7e0: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
+0000b7f0: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+0000b800: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0000b810: 226e 616d 6522 3a22 6e65 774f 776e 6572  "name":"newOwner
+0000b820: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0000b830: 7322 7d5d 2c22 6e61 6d65 223a 224f 776e  s"}],"name":"Own
+0000b840: 6572 4368 616e 6765 6422 2c22 7479 7065  erChanged","type
+0000b850: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
+0000b860: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
+0000b870: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
+0000b880: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
+0000b890: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+0000b8a0: 2c22 6e61 6d65 223a 2274 6f6b 656e 3022  ,"name":"token0"
+0000b8b0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0000b8c0: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0000b8d0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0000b8e0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000b8f0: 6522 3a22 746f 6b65 6e31 222c 2274 7970  e":"token1","typ
+0000b900: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000b910: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
+0000b920: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0000b930: 6e74 3234 222c 226e 616d 6522 3a22 6665  nt24","name":"fe
+0000b940: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0000b950: 3422 7d2c 7b22 696e 6465 7865 6422 3a66  4"},{"indexed":f
+0000b960: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
+0000b970: 7065 223a 2269 6e74 3234 222c 226e 616d  pe":"int24","nam
+0000b980: 6522 3a22 7469 636b 5370 6163 696e 6722  e":"tickSpacing"
+0000b990: 2c22 7479 7065 223a 2269 6e74 3234 227d  ,"type":"int24"}
+0000b9a0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0000b9b0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0000b9c0: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0000b9d0: 223a 2270 6f6f 6c22 2c22 7479 7065 223a  ":"pool","type":
+0000b9e0: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
+0000b9f0: 6522 3a22 506f 6f6c 4372 6561 7465 6422  e":"PoolCreated"
+0000ba00: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
+0000ba10: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0000ba20: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000ba30: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+0000ba40: 6b65 6e41 222c 2274 7970 6522 3a22 6164  kenA","type":"ad
+0000ba50: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0000ba60: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0000ba70: 222c 226e 616d 6522 3a22 746f 6b65 6e42  ","name":"tokenB
+0000ba80: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0000ba90: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0000baa0: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
+0000bab0: 6d65 223a 2266 6565 222c 2274 7970 6522  me":"fee","type"
+0000bac0: 3a22 7569 6e74 3234 227d 5d2c 226e 616d  :"uint24"}],"nam
+0000bad0: 6522 3a22 6372 6561 7465 506f 6f6c 222c  e":"createPool",
+0000bae0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+0000baf0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0000bb00: 6573 7322 2c22 6e61 6d65 223a 2270 6f6f  ess","name":"poo
+0000bb10: 6c22 2c22 7479 7065 223a 2261 6464 7265  l","type":"addre
+0000bb20: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
+0000bb30: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+0000bb40: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+0000bb50: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+0000bb60: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000bb70: 6522 3a22 7569 6e74 3234 222c 226e 616d  e":"uint24","nam
+0000bb80: 6522 3a22 6665 6522 2c22 7479 7065 223a  e":"fee","type":
+0000bb90: 2275 696e 7432 3422 7d2c 7b22 696e 7465  "uint24"},{"inte
+0000bba0: 726e 616c 5479 7065 223a 2269 6e74 3234  rnalType":"int24
+0000bbb0: 222c 226e 616d 6522 3a22 7469 636b 5370  ","name":"tickSp
+0000bbc0: 6163 696e 6722 2c22 7479 7065 223a 2269  acing","type":"i
+0000bbd0: 6e74 3234 227d 5d2c 226e 616d 6522 3a22  nt24"}],"name":"
+0000bbe0: 656e 6162 6c65 4665 6541 6d6f 756e 7422  enableFeeAmount"
+0000bbf0: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
+0000bc00: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000bc10: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
+0000bc20: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+0000bc30: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0000bc40: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0000bc50: 3234 222c 226e 616d 6522 3a22 222c 2274  24","name":"","t
+0000bc60: 7970 6522 3a22 7569 6e74 3234 227d 5d2c  ype":"uint24"}],
+0000bc70: 226e 616d 6522 3a22 6665 6541 6d6f 756e  "name":"feeAmoun
+0000bc80: 7454 6963 6b53 7061 6369 6e67 222c 226f  tTickSpacing","o
+0000bc90: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0000bca0: 6e61 6c54 7970 6522 3a22 696e 7432 3422  nalType":"int24"
+0000bcb0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
+0000bcc0: 223a 2269 6e74 3234 227d 5d2c 2273 7461  ":"int24"}],"sta
+0000bcd0: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
+0000bce0: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
+0000bcf0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+0000bd00: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000bd10: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000bd20: 6d65 223a 2222 2c22 7479 7065 223a 2261  me":"","type":"a
+0000bd30: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0000bd40: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0000bd50: 7322 2c22 6e61 6d65 223a 2222 2c22 7479  s","name":"","ty
+0000bd60: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0000bd70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000bd80: 7569 6e74 3234 222c 226e 616d 6522 3a22  uint24","name":"
+0000bd90: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
+0000bda0: 227d 5d2c 226e 616d 6522 3a22 6765 7450  "}],"name":"getP
+0000bdb0: 6f6f 6c22 2c22 6f75 7470 7574 7322 3a5b  ool","outputs":[
+0000bdc0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000bdd0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0000bde0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+0000bdf0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+0000be00: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+0000be10: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0000be20: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0000be30: 226e 616d 6522 3a22 6f77 6e65 7222 2c22  "name":"owner","
+0000be40: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+0000be50: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0000be60: 7373 222c 226e 616d 6522 3a22 222c 2274  ss","name":"","t
+0000be70: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+0000be80: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0000be90: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+0000bea0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0000beb0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0000bec0: 3a22 7061 7261 6d65 7465 7273 222c 226f  :"parameters","o
+0000bed0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0000bee0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0000bef0: 7322 2c22 6e61 6d65 223a 2266 6163 746f  s","name":"facto
+0000bf00: 7279 222c 2274 7970 6522 3a22 6164 6472  ry","type":"addr
+0000bf10: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0000bf20: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0000bf30: 226e 616d 6522 3a22 746f 6b65 6e30 222c  "name":"token0",
+0000bf40: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0000bf50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000bf60: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000bf70: 6522 3a22 746f 6b65 6e31 222c 2274 7970  e":"token1","typ
+0000bf80: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000bf90: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000bfa0: 696e 7432 3422 2c22 6e61 6d65 223a 2266  int24","name":"f
+0000bfb0: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
+0000bfc0: 3234 227d 2c7b 2269 6e74 6572 6e61 6c54  24"},{"internalT
+0000bfd0: 7970 6522 3a22 696e 7432 3422 2c22 6e61  ype":"int24","na
+0000bfe0: 6d65 223a 2274 6963 6b53 7061 6369 6e67  me":"tickSpacing
+0000bff0: 222c 2274 7970 6522 3a22 696e 7432 3422  ","type":"int24"
+0000c000: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+0000c010: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+0000c020: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+0000c030: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0000c040: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0000c050: 7373 222c 226e 616d 6522 3a22 5f6f 776e  ss","name":"_own
+0000c060: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+0000c070: 6573 7322 7d5d 2c22 6e61 6d65 223a 2273  ess"}],"name":"s
+0000c080: 6574 4f77 6e65 7222 2c22 6f75 7470 7574  etOwner","output
+0000c090: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
+0000c0a0: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+0000c0b0: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+0000c0c0: 6374 696f 6e22 7d5d 270a 2020 2020 756e  ction"}]'.    un
+0000c0d0: 6973 7761 705f 7633 5f70 6169 725f 6162  iswap_v3_pair_ab
+0000c0e0: 693d 275b 207b 2022 616e 6f6e 796d 6f75  i='[ { "anonymou
+0000c0f0: 7322 3a20 6661 6c73 652c 2022 696e 7075  s": false, "inpu
+0000c100: 7473 223a 205b 207b 2022 696e 6465 7865  ts": [ { "indexe
+0000c110: 6422 3a20 7472 7565 2c20 2269 6e74 6572  d": true, "inter
+0000c120: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000c130: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
+0000c140: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
+0000c150: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000c160: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
+0000c170: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000c180: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000c190: 2022 7370 656e 6465 7222 2c20 2274 7970   "spender", "typ
+0000c1a0: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
+0000c1b0: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
+0000c1c0: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
+0000c1d0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000c1e0: 226e 616d 6522 3a20 2276 616c 7565 222c  "name": "value",
+0000c1f0: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
+0000c200: 3622 207d 205d 2c20 226e 616d 6522 3a20  6" } ], "name": 
+0000c210: 2241 7070 726f 7661 6c22 2c20 2274 7970  "Approval", "typ
+0000c220: 6522 3a20 2265 7665 6e74 2220 7d2c 207b  e": "event" }, {
+0000c230: 2022 616e 6f6e 796d 6f75 7322 3a20 6661   "anonymous": fa
+0000c240: 6c73 652c 2022 696e 7075 7473 223a 205b  lse, "inputs": [
+0000c250: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
+0000c260: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
+0000c270: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000c280: 6e61 6d65 223a 2022 7365 6e64 6572 222c  name": "sender",
+0000c290: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000c2a0: 7322 207d 2c20 7b20 2269 6e64 6578 6564  s" }, { "indexed
+0000c2b0: 223a 2066 616c 7365 2c20 2269 6e74 6572  ": false, "inter
+0000c2c0: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+0000c2d0: 3536 222c 2022 6e61 6d65 223a 2022 616d  56", "name": "am
+0000c2e0: 6f75 6e74 3022 2c20 2274 7970 6522 3a20  ount0", "type": 
+0000c2f0: 2275 696e 7432 3536 2220 7d2c 207b 2022  "uint256" }, { "
+0000c300: 696e 6465 7865 6422 3a20 6661 6c73 652c  indexed": false,
+0000c310: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000c320: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
+0000c330: 6522 3a20 2261 6d6f 756e 7431 222c 2022  e": "amount1", "
+0000c340: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+0000c350: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
+0000c360: 2074 7275 652c 2022 696e 7465 726e 616c   true, "internal
+0000c370: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
+0000c380: 2c20 226e 616d 6522 3a20 2274 6f22 2c20  , "name": "to", 
+0000c390: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000c3a0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+0000c3b0: 4275 726e 222c 2022 7479 7065 223a 2022  Burn", "type": "
+0000c3c0: 6576 656e 7422 207d 2c20 7b20 2261 6e6f  event" }, { "ano
+0000c3d0: 6e79 6d6f 7573 223a 2066 616c 7365 2c20  nymous": false, 
+0000c3e0: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
+0000c3f0: 6e64 6578 6564 223a 2074 7275 652c 2022  ndexed": true, "
+0000c400: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000c410: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
+0000c420: 3a20 2273 656e 6465 7222 2c20 2274 7970  : "sender", "typ
+0000c430: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
+0000c440: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
+0000c450: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
+0000c460: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000c470: 226e 616d 6522 3a20 2261 6d6f 756e 7430  "name": "amount0
+0000c480: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000c490: 3235 3622 207d 2c20 7b20 2269 6e64 6578  256" }, { "index
+0000c4a0: 6564 223a 2066 616c 7365 2c20 2269 6e74  ed": false, "int
+0000c4b0: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000c4c0: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000c4d0: 616d 6f75 6e74 3122 2c20 2274 7970 6522  amount1", "type"
+0000c4e0: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
+0000c4f0: 2022 6e61 6d65 223a 2022 4d69 6e74 222c   "name": "Mint",
+0000c500: 2022 7479 7065 223a 2022 6576 656e 7422   "type": "event"
+0000c510: 207d 2c20 7b20 2261 6e6f 6e79 6d6f 7573   }, { "anonymous
+0000c520: 223a 2066 616c 7365 2c20 2269 6e70 7574  ": false, "input
+0000c530: 7322 3a20 5b20 7b20 2269 6e64 6578 6564  s": [ { "indexed
+0000c540: 223a 2074 7275 652c 2022 696e 7465 726e  ": true, "intern
+0000c550: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
+0000c560: 7322 2c20 226e 616d 6522 3a20 2273 656e  s", "name": "sen
+0000c570: 6465 7222 2c20 2274 7970 6522 3a20 2261  der", "type": "a
+0000c580: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000c590: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
+0000c5a0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000c5b0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000c5c0: 3a20 2261 6d6f 756e 7430 496e 222c 2022  : "amount0In", "
+0000c5d0: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+0000c5e0: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
+0000c5f0: 2066 616c 7365 2c20 2269 6e74 6572 6e61   false, "interna
+0000c600: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000c610: 222c 2022 6e61 6d65 223a 2022 616d 6f75  ", "name": "amou
+0000c620: 6e74 3149 6e22 2c20 2274 7970 6522 3a20  nt1In", "type": 
+0000c630: 2275 696e 7432 3536 2220 7d2c 207b 2022  "uint256" }, { "
+0000c640: 696e 6465 7865 6422 3a20 6661 6c73 652c  indexed": false,
+0000c650: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000c660: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
+0000c670: 6522 3a20 2261 6d6f 756e 7430 4f75 7422  e": "amount0Out"
+0000c680: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000c690: 3536 2220 7d2c 207b 2022 696e 6465 7865  56" }, { "indexe
+0000c6a0: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
+0000c6b0: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000c6c0: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
+0000c6d0: 6d6f 756e 7431 4f75 7422 2c20 2274 7970  mount1Out", "typ
+0000c6e0: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
+0000c6f0: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
+0000c700: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
+0000c710: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000c720: 6e61 6d65 223a 2022 746f 222c 2022 7479  name": "to", "ty
+0000c730: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+0000c740: 205d 2c20 226e 616d 6522 3a20 2253 7761   ], "name": "Swa
+0000c750: 7022 2c20 2274 7970 6522 3a20 2265 7665  p", "type": "eve
+0000c760: 6e74 2220 7d2c 207b 2022 616e 6f6e 796d  nt" }, { "anonym
+0000c770: 6f75 7322 3a20 6661 6c73 652c 2022 696e  ous": false, "in
+0000c780: 7075 7473 223a 205b 207b 2022 696e 6465  puts": [ { "inde
+0000c790: 7865 6422 3a20 6661 6c73 652c 2022 696e  xed": false, "in
+0000c7a0: 7465 726e 616c 5479 7065 223a 2022 7569  ternalType": "ui
+0000c7b0: 6e74 3131 3222 2c20 226e 616d 6522 3a20  nt112", "name": 
+0000c7c0: 2272 6573 6572 7665 3022 2c20 2274 7970  "reserve0", "typ
+0000c7d0: 6522 3a20 2275 696e 7431 3132 2220 7d2c  e": "uint112" },
+0000c7e0: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
+0000c7f0: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
+0000c800: 7065 223a 2022 7569 6e74 3131 3222 2c20  pe": "uint112", 
+0000c810: 226e 616d 6522 3a20 2272 6573 6572 7665  "name": "reserve
+0000c820: 3122 2c20 2274 7970 6522 3a20 2275 696e  1", "type": "uin
+0000c830: 7431 3132 2220 7d20 5d2c 2022 6e61 6d65  t112" } ], "name
+0000c840: 223a 2022 5379 6e63 222c 2022 7479 7065  ": "Sync", "type
+0000c850: 223a 2022 6576 656e 7422 207d 2c20 7b20  ": "event" }, { 
+0000c860: 2261 6e6f 6e79 6d6f 7573 223a 2066 616c  "anonymous": fal
+0000c870: 7365 2c20 2269 6e70 7574 7322 3a20 5b20  se, "inputs": [ 
+0000c880: 7b20 2269 6e64 6578 6564 223a 2074 7275  { "indexed": tru
+0000c890: 652c 2022 696e 7465 726e 616c 5479 7065  e, "internalType
+0000c8a0: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
+0000c8b0: 616d 6522 3a20 2266 726f 6d22 2c20 2274  ame": "from", "t
+0000c8c0: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
+0000c8d0: 7d2c 207b 2022 696e 6465 7865 6422 3a20  }, { "indexed": 
+0000c8e0: 7472 7565 2c20 2269 6e74 6572 6e61 6c54  true, "internalT
+0000c8f0: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
+0000c900: 2022 6e61 6d65 223a 2022 746f 222c 2022   "name": "to", "
+0000c910: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
+0000c920: 207d 2c20 7b20 2269 6e64 6578 6564 223a   }, { "indexed":
+0000c930: 2066 616c 7365 2c20 2269 6e74 6572 6e61   false, "interna
+0000c940: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000c950: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
+0000c960: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
+0000c970: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
+0000c980: 223a 2022 5472 616e 7366 6572 222c 2022  ": "Transfer", "
+0000c990: 7479 7065 223a 2022 6576 656e 7422 207d  type": "event" }
+0000c9a0: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+0000c9b0: 2c20 226e 616d 6522 3a20 2244 4f4d 4149  , "name": "DOMAI
+0000c9c0: 4e5f 5345 5041 5241 544f 5222 2c20 226f  N_SEPARATOR", "o
+0000c9d0: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
+0000c9e0: 7465 726e 616c 5479 7065 223a 2022 6279  ternalType": "by
+0000c9f0: 7465 7333 3222 2c20 226e 616d 6522 3a20  tes32", "name": 
+0000ca00: 2222 2c20 2274 7970 6522 3a20 2262 7974  "", "type": "byt
+0000ca10: 6573 3332 2220 7d20 5d2c 2022 7374 6174  es32" } ], "stat
+0000ca20: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
+0000ca30: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
+0000ca40: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+0000ca50: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+0000ca60: 6522 3a20 224d 494e 494d 554d 5f4c 4951  e": "MINIMUM_LIQ
+0000ca70: 5549 4449 5459 222c 2022 6f75 7470 7574  UIDITY", "output
+0000ca80: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+0000ca90: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000caa0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+0000cab0: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+0000cac0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
+0000cad0: 6269 6c69 7479 223a 2022 7075 7265 222c  bility": "pure",
+0000cae0: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
+0000caf0: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
+0000cb00: 223a 205b 5d2c 2022 6e61 6d65 223a 2022  ": [], "name": "
+0000cb10: 5045 524d 4954 5f54 5950 4548 4153 4822  PERMIT_TYPEHASH"
+0000cb20: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
+0000cb30: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000cb40: 2022 6279 7465 7333 3222 2c20 226e 616d   "bytes32", "nam
+0000cb50: 6522 3a20 2222 2c20 2274 7970 6522 3a20  e": "", "type": 
+0000cb60: 2262 7974 6573 3332 2220 7d20 5d2c 2022  "bytes32" } ], "
+0000cb70: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0000cb80: 3a20 2270 7572 6522 2c20 2274 7970 6522  : "pure", "type"
+0000cb90: 3a20 2266 756e 6374 696f 6e22 207d 2c20  : "function" }, 
+0000cba0: 7b20 2269 6e70 7574 7322 3a20 5b20 7b20  { "inputs": [ { 
+0000cbb0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000cbc0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
+0000cbd0: 223a 2022 6f77 6e65 7222 2c20 2274 7970  ": "owner", "typ
+0000cbe0: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
+0000cbf0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+0000cc00: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
+0000cc10: 616d 6522 3a20 2273 7065 6e64 6572 222c  ame": "spender",
+0000cc20: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000cc30: 7322 207d 205d 2c20 226e 616d 6522 3a20  s" } ], "name": 
+0000cc40: 2261 6c6c 6f77 616e 6365 222c 2022 6f75  "allowance", "ou
+0000cc50: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+0000cc60: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000cc70: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000cc80: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000cc90: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
+0000cca0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
+0000ccb0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
+0000ccc0: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+0000ccd0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000cce0: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000ccf0: 6573 7322 2c20 226e 616d 6522 3a20 2273  ess", "name": "s
+0000cd00: 7065 6e64 6572 222c 2022 7479 7065 223a  pender", "type":
+0000cd10: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
+0000cd20: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000cd30: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+0000cd40: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
+0000cd50: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+0000cd60: 5d2c 2022 6e61 6d65 223a 2022 6170 7072  ], "name": "appr
+0000cd70: 6f76 6522 2c20 226f 7574 7075 7473 223a  ove", "outputs":
+0000cd80: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000cd90: 7065 223a 2022 626f 6f6c 222c 2022 6e61  pe": "bool", "na
+0000cda0: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+0000cdb0: 2022 626f 6f6c 2220 7d20 5d2c 2022 7374   "bool" } ], "st
+0000cdc0: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+0000cdd0: 226e 6f6e 7061 7961 626c 6522 2c20 2274  "nonpayable", "t
+0000cde0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000cdf0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000ce00: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000ce10: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000ce20: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
+0000ce30: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000ce40: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+0000ce50: 6261 6c61 6e63 654f 6622 2c20 226f 7574  balanceOf", "out
+0000ce60: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000ce70: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000ce80: 3235 3622 2c20 226e 616d 6522 3a20 2222  256", "name": ""
+0000ce90: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000cea0: 3536 2220 7d20 5d2c 2022 7374 6174 654d  56" } ], "stateM
+0000ceb0: 7574 6162 696c 6974 7922 3a20 2276 6965  utability": "vie
+0000cec0: 7722 2c20 2274 7970 6522 3a20 2266 756e  w", "type": "fun
+0000ced0: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+0000cee0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000cef0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000cf00: 7373 222c 2022 6e61 6d65 223a 2022 746f  ss", "name": "to
+0000cf10: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+0000cf20: 6573 7322 207d 205d 2c20 226e 616d 6522  ess" } ], "name"
+0000cf30: 3a20 2262 7572 6e22 2c20 226f 7574 7075  : "burn", "outpu
+0000cf40: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000cf50: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
+0000cf60: 3622 2c20 226e 616d 6522 3a20 2261 6d6f  6", "name": "amo
+0000cf70: 756e 7430 222c 2022 7479 7065 223a 2022  unt0", "type": "
+0000cf80: 7569 6e74 3235 3622 207d 2c20 7b20 2269  uint256" }, { "i
+0000cf90: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+0000cfa0: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
+0000cfb0: 2022 616d 6f75 6e74 3122 2c20 2274 7970   "amount1", "typ
+0000cfc0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+0000cfd0: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+0000cfe0: 6974 7922 3a20 226e 6f6e 7061 7961 626c  ity": "nonpayabl
+0000cff0: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
+0000d000: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+0000d010: 7574 7322 3a20 5b5d 2c20 226e 616d 6522  uts": [], "name"
+0000d020: 3a20 2264 6563 696d 616c 7322 2c20 226f  : "decimals", "o
+0000d030: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
+0000d040: 7465 726e 616c 5479 7065 223a 2022 7569  ternalType": "ui
+0000d050: 6e74 3822 2c20 226e 616d 6522 3a20 2222  nt8", "name": ""
+0000d060: 2c20 2274 7970 6522 3a20 2275 696e 7438  , "type": "uint8
+0000d070: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000d080: 6162 696c 6974 7922 3a20 2270 7572 6522  ability": "pure"
+0000d090: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000d0a0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+0000d0b0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
+0000d0c0: 2266 6163 746f 7279 222c 2022 6f75 7470  "factory", "outp
+0000d0d0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000d0e0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000d0f0: 7373 222c 2022 6e61 6d65 223a 2022 222c  ss", "name": "",
+0000d100: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000d110: 7322 207d 205d 2c20 2273 7461 7465 4d75  s" } ], "stateMu
+0000d120: 7461 6269 6c69 7479 223a 2022 7669 6577  tability": "view
+0000d130: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
+0000d140: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
+0000d150: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
+0000d160: 2022 6765 7452 6573 6572 7665 7322 2c20   "getReserves", 
+0000d170: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000d180: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000d190: 7569 6e74 3131 3222 2c20 226e 616d 6522  uint112", "name"
+0000d1a0: 3a20 2272 6573 6572 7665 3022 2c20 2274  : "reserve0", "t
+0000d1b0: 7970 6522 3a20 2275 696e 7431 3132 2220  ype": "uint112" 
+0000d1c0: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
+0000d1d0: 7065 223a 2022 7569 6e74 3131 3222 2c20  pe": "uint112", 
+0000d1e0: 226e 616d 6522 3a20 2272 6573 6572 7665  "name": "reserve
+0000d1f0: 3122 2c20 2274 7970 6522 3a20 2275 696e  1", "type": "uin
+0000d200: 7431 3132 2220 7d2c 207b 2022 696e 7465  t112" }, { "inte
+0000d210: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000d220: 3332 222c 2022 6e61 6d65 223a 2022 626c  32", "name": "bl
+0000d230: 6f63 6b54 696d 6573 7461 6d70 4c61 7374  ockTimestampLast
+0000d240: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000d250: 3332 2220 7d20 5d2c 2022 7374 6174 654d  32" } ], "stateM
+0000d260: 7574 6162 696c 6974 7922 3a20 2276 6965  utability": "vie
+0000d270: 7722 2c20 2274 7970 6522 3a20 2266 756e  w", "type": "fun
+0000d280: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+0000d290: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000d2a0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000d2b0: 7373 222c 2022 6e61 6d65 223a 2022 222c  ss", "name": "",
+0000d2c0: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000d2d0: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+0000d2e0: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000d2f0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+0000d300: 7479 7065 223a 2022 6164 6472 6573 7322  type": "address"
+0000d310: 207d 205d 2c20 226e 616d 6522 3a20 2269   } ], "name": "i
+0000d320: 6e69 7469 616c 697a 6522 2c20 226f 7574  nitialize", "out
+0000d330: 7075 7473 223a 205b 5d2c 2022 7374 6174  puts": [], "stat
+0000d340: 654d 7574 6162 696c 6974 7922 3a20 226e  eMutability": "n
+0000d350: 6f6e 7061 7961 626c 6522 2c20 2274 7970  onpayable", "typ
+0000d360: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
+0000d370: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+0000d380: 2c20 226e 616d 6522 3a20 226b 4c61 7374  , "name": "kLast
+0000d390: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+0000d3a0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000d3b0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000d3c0: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+0000d3d0: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
+0000d3e0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000d3f0: 223a 2022 7669 6577 222c 2022 7479 7065  ": "view", "type
+0000d400: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
+0000d410: 207b 2022 696e 7075 7473 223a 205b 207b   { "inputs": [ {
+0000d420: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000d430: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+0000d440: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
+0000d450: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
+0000d460: 2022 6e61 6d65 223a 2022 6d69 6e74 222c   "name": "mint",
+0000d470: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
+0000d480: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000d490: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+0000d4a0: 223a 2022 6c69 7175 6964 6974 7922 2c20  ": "liquidity", 
+0000d4b0: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
+0000d4c0: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000d4d0: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
+0000d4e0: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
+0000d4f0: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000d500: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
+0000d510: 616d 6522 3a20 226e 616d 6522 2c20 226f  ame": "name", "o
+0000d520: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
+0000d530: 7465 726e 616c 5479 7065 223a 2022 7374  ternalType": "st
+0000d540: 7269 6e67 222c 2022 6e61 6d65 223a 2022  ring", "name": "
+0000d550: 222c 2022 7479 7065 223a 2022 7374 7269  ", "type": "stri
+0000d560: 6e67 2220 7d20 5d2c 2022 7374 6174 654d  ng" } ], "stateM
+0000d570: 7574 6162 696c 6974 7922 3a20 2270 7572  utability": "pur
+0000d580: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
+0000d590: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+0000d5a0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000d5b0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000d5c0: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
+0000d5d0: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
+0000d5e0: 6464 7265 7373 2220 7d20 5d2c 2022 6e61  ddress" } ], "na
+0000d5f0: 6d65 223a 2022 6e6f 6e63 6573 222c 2022  me": "nonces", "
+0000d600: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
+0000d610: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+0000d620: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
+0000d630: 2022 222c 2022 7479 7065 223a 2022 7569   "", "type": "ui
+0000d640: 6e74 3235 3622 207d 205d 2c20 2273 7461  nt256" } ], "sta
+0000d650: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
+0000d660: 7669 6577 222c 2022 7479 7065 223a 2022  view", "type": "
+0000d670: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
+0000d680: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
+0000d690: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+0000d6a0: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+0000d6b0: 226f 776e 6572 222c 2022 7479 7065 223a  "owner", "type":
+0000d6c0: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
+0000d6d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000d6e0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
+0000d6f0: 223a 2022 7370 656e 6465 7222 2c20 2274  ": "spender", "t
+0000d700: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
+0000d710: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
+0000d720: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000d730: 226e 616d 6522 3a20 2276 616c 7565 222c  "name": "value",
+0000d740: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
+0000d750: 3622 207d 2c20 7b20 2269 6e74 6572 6e61  6" }, { "interna
+0000d760: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000d770: 222c 2022 6e61 6d65 223a 2022 6465 6164  ", "name": "dead
+0000d780: 6c69 6e65 222c 2022 7479 7065 223a 2022  line", "type": "
+0000d790: 7569 6e74 3235 3622 207d 2c20 7b20 2269  uint256" }, { "i
+0000d7a0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+0000d7b0: 696e 7438 222c 2022 6e61 6d65 223a 2022  int8", "name": "
+0000d7c0: 7622 2c20 2274 7970 6522 3a20 2275 696e  v", "type": "uin
+0000d7d0: 7438 2220 7d2c 207b 2022 696e 7465 726e  t8" }, { "intern
+0000d7e0: 616c 5479 7065 223a 2022 6279 7465 7333  alType": "bytes3
+0000d7f0: 3222 2c20 226e 616d 6522 3a20 2272 222c  2", "name": "r",
+0000d800: 2022 7479 7065 223a 2022 6279 7465 7333   "type": "bytes3
+0000d810: 3222 207d 2c20 7b20 2269 6e74 6572 6e61  2" }, { "interna
+0000d820: 6c54 7970 6522 3a20 2262 7974 6573 3332  lType": "bytes32
+0000d830: 222c 2022 6e61 6d65 223a 2022 7322 2c20  ", "name": "s", 
+0000d840: 2274 7970 6522 3a20 2262 7974 6573 3332  "type": "bytes32
+0000d850: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+0000d860: 7065 726d 6974 222c 2022 6f75 7470 7574  permit", "output
+0000d870: 7322 3a20 5b5d 2c20 2273 7461 7465 4d75  s": [], "stateMu
+0000d880: 7461 6269 6c69 7479 223a 2022 6e6f 6e70  tability": "nonp
+0000d890: 6179 6162 6c65 222c 2022 7479 7065 223a  ayable", "type":
+0000d8a0: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
+0000d8b0: 2022 696e 7075 7473 223a 205b 5d2c 2022   "inputs": [], "
+0000d8c0: 6e61 6d65 223a 2022 7072 6963 6530 4375  name": "price0Cu
+0000d8d0: 6d75 6c61 7469 7665 4c61 7374 222c 2022  mulativeLast", "
+0000d8e0: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
+0000d8f0: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+0000d900: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
+0000d910: 2022 222c 2022 7479 7065 223a 2022 7569   "", "type": "ui
+0000d920: 6e74 3235 3622 207d 205d 2c20 2273 7461  nt256" } ], "sta
+0000d930: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
+0000d940: 7669 6577 222c 2022 7479 7065 223a 2022  view", "type": "
+0000d950: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
+0000d960: 696e 7075 7473 223a 205b 5d2c 2022 6e61  inputs": [], "na
+0000d970: 6d65 223a 2022 7072 6963 6531 4375 6d75  me": "price1Cumu
+0000d980: 6c61 7469 7665 4c61 7374 222c 2022 6f75  lativeLast", "ou
+0000d990: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+0000d9a0: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000d9b0: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000d9c0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000d9d0: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
+0000d9e0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
+0000d9f0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
+0000da00: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+0000da10: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000da20: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000da30: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
+0000da40: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
+0000da50: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
+0000da60: 223a 2022 736b 696d 222c 2022 6f75 7470  ": "skim", "outp
+0000da70: 7574 7322 3a20 5b5d 2c20 2273 7461 7465  uts": [], "state
+0000da80: 4d75 7461 6269 6c69 7479 223a 2022 6e6f  Mutability": "no
+0000da90: 6e70 6179 6162 6c65 222c 2022 7479 7065  npayable", "type
+0000daa0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
+0000dab0: 207b 2022 696e 7075 7473 223a 205b 207b   { "inputs": [ {
+0000dac0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000dad0: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
+0000dae0: 6522 3a20 2261 6d6f 756e 7430 4f75 7422  e": "amount0Out"
+0000daf0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000db00: 3536 2220 7d2c 207b 2022 696e 7465 726e  56" }, { "intern
+0000db10: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
+0000db20: 3622 2c20 226e 616d 6522 3a20 2261 6d6f  6", "name": "amo
+0000db30: 756e 7431 4f75 7422 2c20 2274 7970 6522  unt1Out", "type"
+0000db40: 3a20 2275 696e 7432 3536 2220 7d2c 207b  : "uint256" }, {
+0000db50: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000db60: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+0000db70: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
+0000db80: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
+0000db90: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000dba0: 2022 6279 7465 7322 2c20 226e 616d 6522   "bytes", "name"
+0000dbb0: 3a20 2264 6174 6122 2c20 2274 7970 6522  : "data", "type"
+0000dbc0: 3a20 2262 7974 6573 2220 7d20 5d2c 2022  : "bytes" } ], "
+0000dbd0: 6e61 6d65 223a 2022 7377 6170 222c 2022  name": "swap", "
+0000dbe0: 6f75 7470 7574 7322 3a20 5b5d 2c20 2273  outputs": [], "s
+0000dbf0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000dc00: 2022 6e6f 6e70 6179 6162 6c65 222c 2022   "nonpayable", "
+0000dc10: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
+0000dc20: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
+0000dc30: 205b 5d2c 2022 6e61 6d65 223a 2022 7379   [], "name": "sy
+0000dc40: 6d62 6f6c 222c 2022 6f75 7470 7574 7322  mbol", "outputs"
+0000dc50: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+0000dc60: 7970 6522 3a20 2273 7472 696e 6722 2c20  ype": "string", 
+0000dc70: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+0000dc80: 6522 3a20 2273 7472 696e 6722 207d 205d  e": "string" } ]
+0000dc90: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000dca0: 7479 223a 2022 7075 7265 222c 2022 7479  ty": "pure", "ty
+0000dcb0: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000dcc0: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000dcd0: 5d2c 2022 6e61 6d65 223a 2022 7379 6e63  ], "name": "sync
+0000dce0: 222c 2022 6f75 7470 7574 7322 3a20 5b5d  ", "outputs": []
+0000dcf0: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000dd00: 7479 223a 2022 6e6f 6e70 6179 6162 6c65  ty": "nonpayable
+0000dd10: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
+0000dd20: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
+0000dd30: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
+0000dd40: 2022 746f 6b65 6e30 222c 2022 6f75 7470   "token0", "outp
+0000dd50: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000dd60: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000dd70: 7373 222c 2022 6e61 6d65 223a 2022 222c  ss", "name": "",
+0000dd80: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000dd90: 7322 207d 205d 2c20 2273 7461 7465 4d75  s" } ], "stateMu
+0000dda0: 7461 6269 6c69 7479 223a 2022 7669 6577  tability": "view
+0000ddb0: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
+0000ddc0: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
+0000ddd0: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
+0000dde0: 2022 746f 6b65 6e31 222c 2022 6f75 7470   "token1", "outp
+0000ddf0: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000de00: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000de10: 7373 222c 2022 6e61 6d65 223a 2022 222c  ss", "name": "",
+0000de20: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000de30: 7322 207d 205d 2c20 2273 7461 7465 4d75  s" } ], "stateMu
+0000de40: 7461 6269 6c69 7479 223a 2022 7669 6577  tability": "view
+0000de50: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
+0000de60: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
+0000de70: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
+0000de80: 2022 746f 7461 6c53 7570 706c 7922 2c20   "totalSupply", 
+0000de90: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000dea0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000deb0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000dec0: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
+0000ded0: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
+0000dee0: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+0000def0: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
+0000df00: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000df10: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
+0000df20: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000df30: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000df40: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
+0000df50: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+0000df60: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+0000df70: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
+0000df80: 2022 7661 6c75 6522 2c20 2274 7970 6522   "value", "type"
+0000df90: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
+0000dfa0: 2022 6e61 6d65 223a 2022 7472 616e 7366   "name": "transf
+0000dfb0: 6572 222c 2022 6f75 7470 7574 7322 3a20  er", "outputs": 
+0000dfc0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000dfd0: 6522 3a20 2262 6f6f 6c22 2c20 226e 616d  e": "bool", "nam
+0000dfe0: 6522 3a20 2222 2c20 2274 7970 6522 3a20  e": "", "type": 
+0000dff0: 2262 6f6f 6c22 207d 205d 2c20 2273 7461  "bool" } ], "sta
+0000e000: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
+0000e010: 6e6f 6e70 6179 6162 6c65 222c 2022 7479  nonpayable", "ty
+0000e020: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000e030: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000e040: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+0000e050: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
+0000e060: 616d 6522 3a20 2266 726f 6d22 2c20 2274  ame": "from", "t
+0000e070: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
+0000e080: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
+0000e090: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000e0a0: 226e 616d 6522 3a20 2274 6f22 2c20 2274  "name": "to", "t
+0000e0b0: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
+0000e0c0: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
+0000e0d0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000e0e0: 226e 616d 6522 3a20 2276 616c 7565 222c  "name": "value",
+0000e0f0: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
+0000e100: 3622 207d 205d 2c20 226e 616d 6522 3a20  6" } ], "name": 
+0000e110: 2274 7261 6e73 6665 7246 726f 6d22 2c20  "transferFrom", 
+0000e120: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000e130: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e140: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
+0000e150: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
+0000e160: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000e170: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
+0000e180: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
+0000e190: 2266 756e 6374 696f 6e22 207d 205d 270a  "function" } ]'.
+0000e1a0: 2020 2020 756e 6973 7761 705f 7633 5f65      uniswap_v3_e
+0000e1b0: 7263 3230 5f61 6269 3d27 5b20 7b20 2261  rc20_abi='[ { "a
+0000e1c0: 6e6f 6e79 6d6f 7573 223a 2066 616c 7365  nonymous": false
+0000e1d0: 2c20 2269 6e70 7574 7322 3a20 5b20 7b20  , "inputs": [ { 
+0000e1e0: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
+0000e1f0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000e200: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+0000e210: 6522 3a20 226f 776e 6572 222c 2022 7479  e": "owner", "ty
+0000e220: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+0000e230: 2c20 7b20 2269 6e64 6578 6564 223a 2074  , { "indexed": t
+0000e240: 7275 652c 2022 696e 7465 726e 616c 5479  rue, "internalTy
+0000e250: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000e260: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
+0000e270: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+0000e280: 6573 7322 207d 2c20 7b20 2269 6e64 6578  ess" }, { "index
+0000e290: 6564 223a 2066 616c 7365 2c20 2269 6e74  ed": false, "int
+0000e2a0: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000e2b0: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000e2c0: 7661 6c75 6522 2c20 2274 7970 6522 3a20  value", "type": 
+0000e2d0: 2275 696e 7432 3536 2220 7d20 5d2c 2022  "uint256" } ], "
+0000e2e0: 6e61 6d65 223a 2022 4170 7072 6f76 616c  name": "Approval
+0000e2f0: 222c 2022 7479 7065 223a 2022 6576 656e  ", "type": "even
+0000e300: 7422 207d 2c20 7b20 2261 6e6f 6e79 6d6f  t" }, { "anonymo
+0000e310: 7573 223a 2066 616c 7365 2c20 2269 6e70  us": false, "inp
+0000e320: 7574 7322 3a20 5b20 7b20 2269 6e64 6578  uts": [ { "index
+0000e330: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
+0000e340: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000e350: 6573 7322 2c20 226e 616d 6522 3a20 2266  ess", "name": "f
+0000e360: 726f 6d22 2c20 2274 7970 6522 3a20 2261  rom", "type": "a
+0000e370: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000e380: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
+0000e390: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000e3a0: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000e3b0: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
+0000e3c0: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+0000e3d0: 6e64 6578 6564 223a 2066 616c 7365 2c20  ndexed": false, 
+0000e3e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000e3f0: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+0000e400: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
+0000e410: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+0000e420: 5d2c 2022 6e61 6d65 223a 2022 5472 616e  ], "name": "Tran
+0000e430: 7366 6572 222c 2022 7479 7065 223a 2022  sfer", "type": "
+0000e440: 6576 656e 7422 207d 2c20 7b20 2269 6e70  event" }, { "inp
+0000e450: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000e460: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000e470: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
+0000e480: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
+0000e490: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000e4a0: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+0000e4b0: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+0000e4c0: 2273 7065 6e64 6572 222c 2022 7479 7065  "spender", "type
+0000e4d0: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+0000e4e0: 2c20 226e 616d 6522 3a20 2261 6c6c 6f77  , "name": "allow
+0000e4f0: 616e 6365 222c 2022 6f75 7470 7574 7322  ance", "outputs"
+0000e500: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+0000e510: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+0000e520: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000e530: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+0000e540: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
+0000e550: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
+0000e560: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
+0000e570: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
+0000e580: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000e590: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000e5a0: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
+0000e5b0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+0000e5c0: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
+0000e5d0: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+0000e5e0: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
+0000e5f0: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
+0000e600: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
+0000e610: 6d65 223a 2022 6170 7072 6f76 6522 2c20  me": "approve", 
+0000e620: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000e630: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e640: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
+0000e650: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
+0000e660: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000e670: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
+0000e680: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
+0000e690: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000e6a0: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
+0000e6b0: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000e6c0: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000e6d0: 2022 6f77 6e65 7222 2c20 2274 7970 6522   "owner", "type"
+0000e6e0: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
+0000e6f0: 2022 6e61 6d65 223a 2022 6261 6c61 6e63   "name": "balanc
+0000e700: 654f 6622 2c20 226f 7574 7075 7473 223a  eOf", "outputs":
+0000e710: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000e720: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000e730: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+0000e740: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+0000e750: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+0000e760: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
+0000e770: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000e780: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000e790: 5b5d 2c20 226e 616d 6522 3a20 2264 6563  [], "name": "dec
+0000e7a0: 696d 616c 7322 2c20 226f 7574 7075 7473  imals", "outputs
+0000e7b0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000e7c0: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
+0000e7d0: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+0000e7e0: 6522 3a20 2275 696e 7438 2220 7d20 5d2c  e": "uint8" } ],
+0000e7f0: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+0000e800: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
+0000e810: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
+0000e820: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+0000e830: 2c20 226e 616d 6522 3a20 226e 616d 6522  , "name": "name"
+0000e840: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
+0000e850: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000e860: 2022 7374 7269 6e67 222c 2022 6e61 6d65   "string", "name
+0000e870: 223a 2022 222c 2022 7479 7065 223a 2022  ": "", "type": "
+0000e880: 7374 7269 6e67 2220 7d20 5d2c 2022 7374  string" } ], "st
+0000e890: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+0000e8a0: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
+0000e8b0: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000e8c0: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
+0000e8d0: 616d 6522 3a20 2273 796d 626f 6c22 2c20  ame": "symbol", 
+0000e8e0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000e8f0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e900: 7374 7269 6e67 222c 2022 6e61 6d65 223a  string", "name":
+0000e910: 2022 222c 2022 7479 7065 223a 2022 7374   "", "type": "st
+0000e920: 7269 6e67 2220 7d20 5d2c 2022 7374 6174  ring" } ], "stat
+0000e930: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
+0000e940: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
+0000e950: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+0000e960: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+0000e970: 6522 3a20 2274 6f74 616c 5375 7070 6c79  e": "totalSupply
+0000e980: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+0000e990: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000e9a0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000e9b0: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+0000e9c0: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
+0000e9d0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000e9e0: 223a 2022 7669 6577 222c 2022 7479 7065  ": "view", "type
+0000e9f0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
+0000ea00: 207b 2022 696e 7075 7473 223a 205b 207b   { "inputs": [ {
+0000ea10: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000ea20: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+0000ea30: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
+0000ea40: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
+0000ea50: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000ea60: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
+0000ea70: 6522 3a20 2276 616c 7565 222c 2022 7479  e": "value", "ty
+0000ea80: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+0000ea90: 205d 2c20 226e 616d 6522 3a20 2274 7261   ], "name": "tra
+0000eaa0: 6e73 6665 7222 2c20 226f 7574 7075 7473  nsfer", "outputs
+0000eab0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000eac0: 5479 7065 223a 2022 626f 6f6c 222c 2022  Type": "bool", "
+0000ead0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+0000eae0: 223a 2022 626f 6f6c 2220 7d20 5d2c 2022  ": "bool" } ], "
+0000eaf0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0000eb00: 3a20 226e 6f6e 7061 7961 626c 6522 2c20  : "nonpayable", 
+0000eb10: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
+0000eb20: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
+0000eb30: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+0000eb40: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
+0000eb50: 2022 6e61 6d65 223a 2022 6672 6f6d 222c   "name": "from",
+0000eb60: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000eb70: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+0000eb80: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000eb90: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
+0000eba0: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000ebb0: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+0000ebc0: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000ebd0: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
+0000ebe0: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
+0000ebf0: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
+0000ec00: 223a 2022 7472 616e 7366 6572 4672 6f6d  ": "transferFrom
+0000ec10: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+0000ec20: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000ec30: 3a20 2262 6f6f 6c22 2c20 226e 616d 6522  : "bool", "name"
+0000ec40: 3a20 2222 2c20 2274 7970 6522 3a20 2262  : "", "type": "b
+0000ec50: 6f6f 6c22 207d 205d 2c20 2273 7461 7465  ool" } ], "state
+0000ec60: 4d75 7461 6269 6c69 7479 223a 2022 6e6f  Mutability": "no
+0000ec70: 6e70 6179 6162 6c65 222c 2022 7479 7065  npayable", "type
+0000ec80: 223a 2022 6675 6e63 7469 6f6e 2220 7d20  ": "function" } 
+0000ec90: 5d27 0a20 2020 2023 6874 7470 733a 2f2f  ]'.    #https://
+0000eca0: 6574 6865 7273 6361 6e2e 696f 2f61 6464  etherscan.io/add
+0000ecb0: 7265 7373 2f30 7865 3539 3234 3237 6130  ress/0xe592427a0
+0000ecc0: 6165 6365 3932 6465 3365 6465 6531 6631  aece92de3edee1f1
+0000ecd0: 3865 3031 3537 6330 3538 3631 3536 3423  8e0157c05861564#
+0000ece0: 636f 6465 0a20 2020 2075 6e69 7377 6170  code.    uniswap
+0000ecf0: 5f76 335f 726f 7574 655f 6162 693d 275b  _v3_route_abi='[
+0000ed00: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0000ed10: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0000ed20: 6573 7322 2c22 6e61 6d65 223a 225f 6661  ess","name":"_fa
+0000ed30: 6374 6f72 7922 2c22 7479 7065 223a 2261  ctory","type":"a
+0000ed40: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0000ed50: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0000ed60: 7322 2c22 6e61 6d65 223a 225f 5745 5448  s","name":"_WETH
+0000ed70: 3922 2c22 7479 7065 223a 2261 6464 7265  9","type":"addre
+0000ed80: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
+0000ed90: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+0000eda0: 626c 6522 2c22 7479 7065 223a 2263 6f6e  ble","type":"con
+0000edb0: 7374 7275 6374 6f72 227d 2c7b 2269 6e70  structor"},{"inp
+0000edc0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+0000edd0: 5745 5448 3922 2c22 6f75 7470 7574 7322  WETH9","outputs"
+0000ede0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0000edf0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000ee00: 6522 3a22 222c 2274 7970 6522 3a22 6164  e":"","type":"ad
+0000ee10: 6472 6573 7322 7d5d 2c22 7374 6174 654d  dress"}],"stateM
+0000ee20: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+0000ee30: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+0000ee40: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+0000ee50: 7b22 636f 6d70 6f6e 656e 7473 223a 5b7b  {"components":[{
+0000ee60: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000ee70: 6279 7465 7322 2c22 6e61 6d65 223a 2270  bytes","name":"p
+0000ee80: 6174 6822 2c22 7479 7065 223a 2262 7974  ath","type":"byt
+0000ee90: 6573 227d 2c7b 2269 6e74 6572 6e61 6c54  es"},{"internalT
+0000eea0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0000eeb0: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
+0000eec0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0000eed0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0000eee0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0000eef0: 616d 6522 3a22 6465 6164 6c69 6e65 222c  ame":"deadline",
+0000ef00: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0000ef10: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000ef20: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0000ef30: 6522 3a22 616d 6f75 6e74 496e 222c 2274  e":"amountIn","t
+0000ef40: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0000ef50: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000ef60: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0000ef70: 3a22 616d 6f75 6e74 4f75 744d 696e 696d  :"amountOutMinim
+0000ef80: 756d 222c 2274 7970 6522 3a22 7569 6e74  um","type":"uint
+0000ef90: 3235 3622 7d5d 2c22 696e 7465 726e 616c  256"}],"internal
+0000efa0: 5479 7065 223a 2273 7472 7563 7420 4953  Type":"struct IS
+0000efb0: 7761 7052 6f75 7465 722e 4578 6163 7449  wapRouter.ExactI
+0000efc0: 6e70 7574 5061 7261 6d73 222c 226e 616d  nputParams","nam
+0000efd0: 6522 3a22 7061 7261 6d73 222c 2274 7970  e":"params","typ
+0000efe0: 6522 3a22 7475 706c 6522 7d5d 2c22 6e61  e":"tuple"}],"na
+0000eff0: 6d65 223a 2265 7861 6374 496e 7075 7422  me":"exactInput"
+0000f000: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+0000f010: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000f020: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0000f030: 6f75 6e74 4f75 7422 2c22 7479 7065 223a  ountOut","type":
+0000f040: 2275 696e 7432 3536 227d 5d2c 2273 7461  "uint256"}],"sta
+0000f050: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
+0000f060: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+0000f070: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+0000f080: 7574 7322 3a5b 7b22 636f 6d70 6f6e 656e  uts":[{"componen
+0000f090: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0000f0a0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0000f0b0: 6e61 6d65 223a 2274 6f6b 656e 496e 222c  name":"tokenIn",
+0000f0c0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0000f0d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000f0e0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000f0f0: 6522 3a22 746f 6b65 6e4f 7574 222c 2274  e":"tokenOut","t
+0000f100: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0000f110: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000f120: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
+0000f130: 2266 6565 222c 2274 7970 6522 3a22 7569  "fee","type":"ui
+0000f140: 6e74 3234 227d 2c7b 2269 6e74 6572 6e61  nt24"},{"interna
+0000f150: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+0000f160: 2c22 6e61 6d65 223a 2272 6563 6970 6965  ,"name":"recipie
+0000f170: 6e74 222c 2274 7970 6522 3a22 6164 6472  nt","type":"addr
+0000f180: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0000f190: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0000f1a0: 226e 616d 6522 3a22 6465 6164 6c69 6e65  "name":"deadline
+0000f1b0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0000f1c0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0000f1d0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0000f1e0: 616d 6522 3a22 616d 6f75 6e74 496e 222c  ame":"amountIn",
+0000f1f0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0000f200: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000f210: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0000f220: 6522 3a22 616d 6f75 6e74 4f75 744d 696e  e":"amountOutMin
+0000f230: 696d 756d 222c 2274 7970 6522 3a22 7569  imum","type":"ui
+0000f240: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0000f250: 616c 5479 7065 223a 2275 696e 7431 3630  alType":"uint160
+0000f260: 222c 226e 616d 6522 3a22 7371 7274 5072  ","name":"sqrtPr
+0000f270: 6963 654c 696d 6974 5839 3622 2c22 7479  iceLimitX96","ty
+0000f280: 7065 223a 2275 696e 7431 3630 227d 5d2c  pe":"uint160"}],
+0000f290: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000f2a0: 7374 7275 6374 2049 5377 6170 526f 7574  struct ISwapRout
+0000f2b0: 6572 2e45 7861 6374 496e 7075 7453 696e  er.ExactInputSin
+0000f2c0: 676c 6550 6172 616d 7322 2c22 6e61 6d65  gleParams","name
+0000f2d0: 223a 2270 6172 616d 7322 2c22 7479 7065  ":"params","type
+0000f2e0: 223a 2274 7570 6c65 227d 5d2c 226e 616d  ":"tuple"}],"nam
+0000f2f0: 6522 3a22 6578 6163 7449 6e70 7574 5369  e":"exactInputSi
+0000f300: 6e67 6c65 222c 226f 7574 7075 7473 223a  ngle","outputs":
+0000f310: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0000f320: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0000f330: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
+0000f340: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0000f350: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0000f360: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
+0000f370: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+0000f380: 7b22 696e 7075 7473 223a 5b7b 2263 6f6d  {"inputs":[{"com
+0000f390: 706f 6e65 6e74 7322 3a5b 7b22 696e 7465  ponents":[{"inte
+0000f3a0: 726e 616c 5479 7065 223a 2262 7974 6573  rnalType":"bytes
+0000f3b0: 222c 226e 616d 6522 3a22 7061 7468 222c  ","name":"path",
+0000f3c0: 2274 7970 6522 3a22 6279 7465 7322 7d2c  "type":"bytes"},
+0000f3d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000f3e0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0000f3f0: 3a22 7265 6369 7069 656e 7422 2c22 7479  :"recipient","ty
+0000f400: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0000f410: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000f420: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0000f430: 2264 6561 646c 696e 6522 2c22 7479 7065  "deadline","type
+0000f440: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0000f450: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0000f460: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0000f470: 6d6f 756e 744f 7574 222c 2274 7970 6522  mountOut","type"
+0000f480: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0000f490: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000f4a0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0000f4b0: 6f75 6e74 496e 4d61 7869 6d75 6d22 2c22  ountInMaximum","
+0000f4c0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0000f4d0: 5d2c 2269 6e74 6572 6e61 6c54 7970 6522  ],"internalType"
+0000f4e0: 3a22 7374 7275 6374 2049 5377 6170 526f  :"struct ISwapRo
+0000f4f0: 7574 6572 2e45 7861 6374 4f75 7470 7574  uter.ExactOutput
+0000f500: 5061 7261 6d73 222c 226e 616d 6522 3a22  Params","name":"
+0000f510: 7061 7261 6d73 222c 2274 7970 6522 3a22  params","type":"
+0000f520: 7475 706c 6522 7d5d 2c22 6e61 6d65 223a  tuple"}],"name":
+0000f530: 2265 7861 6374 4f75 7470 7574 222c 226f  "exactOutput","o
+0000f540: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0000f550: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0000f560: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0000f570: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
+0000f580: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
+0000f590: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+0000f5a0: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0000f5b0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0000f5c0: 3a5b 7b22 636f 6d70 6f6e 656e 7473 223a  :[{"components":
+0000f5d0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0000f5e0: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0000f5f0: 223a 2274 6f6b 656e 496e 222c 2274 7970  ":"tokenIn","typ
+0000f600: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000f610: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+0000f620: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+0000f630: 746f 6b65 6e4f 7574 222c 2274 7970 6522  tokenOut","type"
+0000f640: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0000f650: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000f660: 7432 3422 2c22 6e61 6d65 223a 2266 6565  t24","name":"fee
+0000f670: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
+0000f680: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0000f690: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000f6a0: 6d65 223a 2272 6563 6970 6965 6e74 222c  me":"recipient",
+0000f6b0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0000f6c0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000f6d0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0000f6e0: 6522 3a22 6465 6164 6c69 6e65 222c 2274  e":"deadline","t
+0000f6f0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0000f700: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000f710: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0000f720: 3a22 616d 6f75 6e74 4f75 7422 2c22 7479  :"amountOut","ty
+0000f730: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+0000f740: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000f750: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0000f760: 2261 6d6f 756e 7449 6e4d 6178 696d 756d  "amountInMaximum
+0000f770: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0000f780: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0000f790: 7065 223a 2275 696e 7431 3630 222c 226e  pe":"uint160","n
+0000f7a0: 616d 6522 3a22 7371 7274 5072 6963 654c  ame":"sqrtPriceL
+0000f7b0: 696d 6974 5839 3622 2c22 7479 7065 223a  imitX96","type":
+0000f7c0: 2275 696e 7431 3630 227d 5d2c 2269 6e74  "uint160"}],"int
+0000f7d0: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
+0000f7e0: 6374 2049 5377 6170 526f 7574 6572 2e45  ct ISwapRouter.E
+0000f7f0: 7861 6374 4f75 7470 7574 5369 6e67 6c65  xactOutputSingle
+0000f800: 5061 7261 6d73 222c 226e 616d 6522 3a22  Params","name":"
+0000f810: 7061 7261 6d73 222c 2274 7970 6522 3a22  params","type":"
+0000f820: 7475 706c 6522 7d5d 2c22 6e61 6d65 223a  tuple"}],"name":
+0000f830: 2265 7861 6374 4f75 7470 7574 5369 6e67  "exactOutputSing
+0000f840: 6c65 222c 226f 7574 7075 7473 223a 5b7b  le","outputs":[{
+0000f850: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000f860: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0000f870: 2261 6d6f 756e 7449 6e22 2c22 7479 7065  "amountIn","type
+0000f880: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
+0000f890: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000f8a0: 2270 6179 6162 6c65 222c 2274 7970 6522  "payable","type"
+0000f8b0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0000f8c0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0000f8d0: 3a22 6661 6374 6f72 7922 2c22 6f75 7470  :"factory","outp
+0000f8e0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0000f8f0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0000f900: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+0000f910: 3a22 6164 6472 6573 7322 7d5d 2c22 7374  :"address"}],"st
+0000f920: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0000f930: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+0000f940: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+0000f950: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0000f960: 7065 223a 2262 7974 6573 5b5d 222c 226e  pe":"bytes[]","n
+0000f970: 616d 6522 3a22 6461 7461 222c 2274 7970  ame":"data","typ
+0000f980: 6522 3a22 6279 7465 735b 5d22 7d5d 2c22  e":"bytes[]"}],"
+0000f990: 6e61 6d65 223a 226d 756c 7469 6361 6c6c  name":"multicall
+0000f9a0: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+0000f9b0: 6e74 6572 6e61 6c54 7970 6522 3a22 6279  nternalType":"by
+0000f9c0: 7465 735b 5d22 2c22 6e61 6d65 223a 2272  tes[]","name":"r
+0000f9d0: 6573 756c 7473 222c 2274 7970 6522 3a22  esults","type":"
+0000f9e0: 6279 7465 735b 5d22 7d5d 2c22 7374 6174  bytes[]"}],"stat
+0000f9f0: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
+0000fa00: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+0000fa10: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+0000fa20: 7473 223a 5b5d 2c22 6e61 6d65 223a 2272  ts":[],"name":"r
+0000fa30: 6566 756e 6445 5448 222c 226f 7574 7075  efundETH","outpu
+0000fa40: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
+0000fa50: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
+0000fa60: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+0000fa70: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+0000fa80: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0000fa90: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0000faa0: 223a 2274 6f6b 656e 222c 2274 7970 6522  ":"token","type"
+0000fab0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0000fac0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000fad0: 7432 3536 222c 226e 616d 6522 3a22 7661  t256","name":"va
+0000fae0: 6c75 6522 2c22 7479 7065 223a 2275 696e  lue","type":"uin
+0000faf0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+0000fb00: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0000fb10: 2c22 6e61 6d65 223a 2264 6561 646c 696e  ,"name":"deadlin
+0000fb20: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0000fb30: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+0000fb40: 7970 6522 3a22 7569 6e74 3822 2c22 6e61  ype":"uint8","na
+0000fb50: 6d65 223a 2276 222c 2274 7970 6522 3a22  me":"v","type":"
+0000fb60: 7569 6e74 3822 7d2c 7b22 696e 7465 726e  uint8"},{"intern
+0000fb70: 616c 5479 7065 223a 2262 7974 6573 3332  alType":"bytes32
+0000fb80: 222c 226e 616d 6522 3a22 7222 2c22 7479  ","name":"r","ty
+0000fb90: 7065 223a 2262 7974 6573 3332 227d 2c7b  pe":"bytes32"},{
+0000fba0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000fbb0: 6279 7465 7333 3222 2c22 6e61 6d65 223a  bytes32","name":
+0000fbc0: 2273 222c 2274 7970 6522 3a22 6279 7465  "s","type":"byte
+0000fbd0: 7333 3222 7d5d 2c22 6e61 6d65 223a 2273  s32"}],"name":"s
+0000fbe0: 656c 6650 6572 6d69 7422 2c22 6f75 7470  elfPermit","outp
+0000fbf0: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
+0000fc00: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+0000fc10: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0000fc20: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0000fc30: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0000fc40: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000fc50: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
+0000fc60: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0000fc70: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0000fc80: 6e74 3235 3622 2c22 6e61 6d65 223a 226e  nt256","name":"n
+0000fc90: 6f6e 6365 222c 2274 7970 6522 3a22 7569  once","type":"ui
+0000fca0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0000fcb0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0000fcc0: 222c 226e 616d 6522 3a22 6578 7069 7279  ","name":"expiry
+0000fcd0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0000fce0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0000fcf0: 7065 223a 2275 696e 7438 222c 226e 616d  pe":"uint8","nam
+0000fd00: 6522 3a22 7622 2c22 7479 7065 223a 2275  e":"v","type":"u
+0000fd10: 696e 7438 227d 2c7b 2269 6e74 6572 6e61  int8"},{"interna
+0000fd20: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
+0000fd30: 2c22 6e61 6d65 223a 2272 222c 2274 7970  ,"name":"r","typ
+0000fd40: 6522 3a22 6279 7465 7333 3222 7d2c 7b22  e":"bytes32"},{"
+0000fd50: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
+0000fd60: 7974 6573 3332 222c 226e 616d 6522 3a22  ytes32","name":"
+0000fd70: 7322 2c22 7479 7065 223a 2262 7974 6573  s","type":"bytes
+0000fd80: 3332 227d 5d2c 226e 616d 6522 3a22 7365  32"}],"name":"se
+0000fd90: 6c66 5065 726d 6974 416c 6c6f 7765 6422  lfPermitAllowed"
+0000fda0: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
+0000fdb0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000fdc0: 2270 6179 6162 6c65 222c 2274 7970 6522  "payable","type"
+0000fdd0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0000fde0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0000fdf0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0000fe00: 222c 226e 616d 6522 3a22 746f 6b65 6e22  ","name":"token"
+0000fe10: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0000fe20: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0000fe30: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0000fe40: 6d65 223a 226e 6f6e 6365 222c 2274 7970  me":"nonce","typ
+0000fe50: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0000fe60: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000fe70: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0000fe80: 6578 7069 7279 222c 2274 7970 6522 3a22  expiry","type":"
+0000fe90: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0000fea0: 726e 616c 5479 7065 223a 2275 696e 7438  rnalType":"uint8
+0000feb0: 222c 226e 616d 6522 3a22 7622 2c22 7479  ","name":"v","ty
+0000fec0: 7065 223a 2275 696e 7438 227d 2c7b 2269  pe":"uint8"},{"i
+0000fed0: 6e74 6572 6e61 6c54 7970 6522 3a22 6279  nternalType":"by
+0000fee0: 7465 7333 3222 2c22 6e61 6d65 223a 2272  tes32","name":"r
+0000fef0: 222c 2274 7970 6522 3a22 6279 7465 7333  ","type":"bytes3
+0000ff00: 3222 7d2c 7b22 696e 7465 726e 616c 5479  2"},{"internalTy
+0000ff10: 7065 223a 2262 7974 6573 3332 222c 226e  pe":"bytes32","n
+0000ff20: 616d 6522 3a22 7322 2c22 7479 7065 223a  ame":"s","type":
+0000ff30: 2262 7974 6573 3332 227d 5d2c 226e 616d  "bytes32"}],"nam
+0000ff40: 6522 3a22 7365 6c66 5065 726d 6974 416c  e":"selfPermitAl
+0000ff50: 6c6f 7765 6449 664e 6563 6573 7361 7279  lowedIfNecessary
+0000ff60: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+0000ff70: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0000ff80: 3a22 7061 7961 626c 6522 2c22 7479 7065  :"payable","type
+0000ff90: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+0000ffa0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+0000ffb0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0000ffc0: 7322 2c22 6e61 6d65 223a 2274 6f6b 656e  s","name":"token
+0000ffd0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0000ffe0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0000fff0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00010000: 616d 6522 3a22 7661 6c75 6522 2c22 7479  ame":"value","ty
+00010010: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+00010020: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00010030: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00010040: 2264 6561 646c 696e 6522 2c22 7479 7065  "deadline","type
+00010050: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00010060: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00010070: 6e74 3822 2c22 6e61 6d65 223a 2276 222c  nt8","name":"v",
+00010080: 2274 7970 6522 3a22 7569 6e74 3822 7d2c  "type":"uint8"},
+00010090: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000100a0: 2262 7974 6573 3332 222c 226e 616d 6522  "bytes32","name"
+000100b0: 3a22 7222 2c22 7479 7065 223a 2262 7974  :"r","type":"byt
+000100c0: 6573 3332 227d 2c7b 2269 6e74 6572 6e61  es32"},{"interna
+000100d0: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
+000100e0: 2c22 6e61 6d65 223a 2273 222c 2274 7970  ,"name":"s","typ
+000100f0: 6522 3a22 6279 7465 7333 3222 7d5d 2c22  e":"bytes32"}],"
+00010100: 6e61 6d65 223a 2273 656c 6650 6572 6d69  name":"selfPermi
+00010110: 7449 664e 6563 6573 7361 7279 222c 226f  tIfNecessary","o
+00010120: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
+00010130: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
+00010140: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+00010150: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+00010160: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00010170: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+00010180: 6e61 6d65 223a 2274 6f6b 656e 222c 2274  name":"token","t
+00010190: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+000101a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000101b0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+000101c0: 3a22 616d 6f75 6e74 4d69 6e69 6d75 6d22  :"amountMinimum"
+000101d0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+000101e0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+000101f0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+00010200: 6d65 223a 2272 6563 6970 6965 6e74 222c  me":"recipient",
+00010210: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00010220: 7d5d 2c22 6e61 6d65 223a 2273 7765 6570  }],"name":"sweep
+00010230: 546f 6b65 6e22 2c22 6f75 7470 7574 7322  Token","outputs"
+00010240: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
+00010250: 6c69 7479 223a 2270 6179 6162 6c65 222c  lity":"payable",
+00010260: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00010270: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00010280: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00010290: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+000102a0: 746f 6b65 6e22 2c22 7479 7065 223a 2261  token","type":"a
+000102b0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+000102c0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000102d0: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+000102e0: 744d 696e 696d 756d 222c 2274 7970 6522  tMinimum","type"
+000102f0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00010300: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00010310: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
+00010320: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
+00010330: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00010340: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00010350: 3235 3622 2c22 6e61 6d65 223a 2266 6565  256","name":"fee
+00010360: 4269 7073 222c 2274 7970 6522 3a22 7569  Bips","type":"ui
+00010370: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+00010380: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00010390: 222c 226e 616d 6522 3a22 6665 6552 6563  ","name":"feeRec
+000103a0: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+000103b0: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+000103c0: 223a 2273 7765 6570 546f 6b65 6e57 6974  ":"sweepTokenWit
+000103d0: 6846 6565 222c 226f 7574 7075 7473 223a  hFee","outputs":
+000103e0: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+000103f0: 6974 7922 3a22 7061 7961 626c 6522 2c22  ity":"payable","
+00010400: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00010410: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00010420: 6e74 6572 6e61 6c54 7970 6522 3a22 696e  nternalType":"in
+00010430: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+00010440: 6f75 6e74 3044 656c 7461 222c 2274 7970  ount0Delta","typ
+00010450: 6522 3a22 696e 7432 3536 227d 2c7b 2269  e":"int256"},{"i
+00010460: 6e74 6572 6e61 6c54 7970 6522 3a22 696e  nternalType":"in
+00010470: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+00010480: 6f75 6e74 3144 656c 7461 222c 2274 7970  ount1Delta","typ
+00010490: 6522 3a22 696e 7432 3536 227d 2c7b 2269  e":"int256"},{"i
+000104a0: 6e74 6572 6e61 6c54 7970 6522 3a22 6279  nternalType":"by
+000104b0: 7465 7322 2c22 6e61 6d65 223a 225f 6461  tes","name":"_da
+000104c0: 7461 222c 2274 7970 6522 3a22 6279 7465  ta","type":"byte
+000104d0: 7322 7d5d 2c22 6e61 6d65 223a 2275 6e69  s"}],"name":"uni
+000104e0: 7377 6170 5633 5377 6170 4361 6c6c 6261  swapV3SwapCallba
+000104f0: 636b 222c 226f 7574 7075 7473 223a 5b5d  ck","outputs":[]
+00010500: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00010510: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+00010520: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00010530: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00010540: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00010550: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00010560: 616d 6f75 6e74 4d69 6e69 6d75 6d22 2c22  amountMinimum","
+00010570: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00010580: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00010590: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+000105a0: 223a 2272 6563 6970 6965 6e74 222c 2274  ":"recipient","t
+000105b0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+000105c0: 2c22 6e61 6d65 223a 2275 6e77 7261 7057  ,"name":"unwrapW
+000105d0: 4554 4839 222c 226f 7574 7075 7473 223a  ETH9","outputs":
+000105e0: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+000105f0: 6974 7922 3a22 7061 7961 626c 6522 2c22  ity":"payable","
+00010600: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00010610: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00010620: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00010630: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+00010640: 6d6f 756e 744d 696e 696d 756d 222c 2274  mountMinimum","t
+00010650: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00010660: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00010670: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00010680: 3a22 7265 6369 7069 656e 7422 2c22 7479  :"recipient","ty
+00010690: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+000106a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000106b0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+000106c0: 2266 6565 4269 7073 222c 2274 7970 6522  "feeBips","type"
+000106d0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+000106e0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+000106f0: 7265 7373 222c 226e 616d 6522 3a22 6665  ress","name":"fe
+00010700: 6552 6563 6970 6965 6e74 222c 2274 7970  eRecipient","typ
+00010710: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+00010720: 6e61 6d65 223a 2275 6e77 7261 7057 4554  name":"unwrapWET
+00010730: 4839 5769 7468 4665 6522 2c22 6f75 7470  H9WithFee","outp
+00010740: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
+00010750: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+00010760: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+00010770: 7469 6f6e 227d 2c7b 2273 7461 7465 4d75  tion"},{"stateMu
+00010780: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+00010790: 6c65 222c 2274 7970 6522 3a22 7265 6365  le","type":"rece
+000107a0: 6976 6522 7d5d 270a 0a20 2020 2027 2727  ive"}]'..    '''
+000107b0: 0a20 2020 2020 2020 2075 7365 6420 666f  .        used fo
+000107c0: 7220 756e 6973 7761 7020 7633 2062 6173  r uniswap v3 bas
+000107d0: 6564 2064 6578 0a20 2020 2027 2727 0a20  ed dex.    '''. 
+000107e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000107f0: 7365 6c66 2c5f 7765 6233 2c5f 6661 6374  self,_web3,_fact
+00010800: 6f72 795f 6164 6472 6573 732c 5f72 6f75  ory_address,_rou
+00010810: 7465 5f61 6464 7265 7373 2c5f 7075 626c  te_address,_publ
+00010820: 6963 5f6b 6579 2c5f 7072 6976 6174 655f  ic_key,_private_
+00010830: 6b65 7929 3a0a 2020 2020 2020 2020 7365  key):.        se
+00010840: 6c66 2e6d 795f 7075 626c 6963 5f6b 6579  lf.my_public_key
+00010850: 3d5f 7075 626c 6963 5f6b 6579 0a20 2020  =_public_key.   
+00010860: 2020 2020 2073 656c 662e 6d79 5f70 7269       self.my_pri
+00010870: 7661 7465 5f6b 6579 3d5f 7072 6976 6174  vate_key=_privat
+00010880: 655f 6b65 790a 2020 2020 2020 2020 7365  e_key.        se
+00010890: 6c66 2e66 6163 746f 7279 5f61 6464 7265  lf.factory_addre
+000108a0: 7373 3d5f 6661 6374 6f72 795f 6164 6472  ss=_factory_addr
+000108b0: 6573 730a 2020 2020 2020 2020 7365 6c66  ess.        self
+000108c0: 2e72 6f75 7465 5f61 6464 7265 7373 3d5f  .route_address=_
+000108d0: 726f 7574 655f 6164 6472 6573 730a 2020  route_address.  
+000108e0: 2020 2020 2020 7365 6c66 2e77 6562 3320        self.web3 
+000108f0: 3d20 5f77 6562 330a 2020 2020 2020 2020  = _web3.        
+00010900: 7365 6c66 2e77 6562 332e 6d69 6464 6c65  self.web3.middle
+00010910: 7761 7265 5f6f 6e69 6f6e 2e69 6e6a 6563  ware_onion.injec
+00010920: 7428 6765 7468 5f70 6f61 5f6d 6964 646c  t(geth_poa_middl
+00010930: 6577 6172 652c 206c 6179 6572 3d30 290a  eware, layer=0).
+00010940: 2020 2020 2020 2020 7072 696e 7428 2723          print('#
+00010950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010960: 2323 2323 2323 2323 2323 2327 290a 2020  ###########').  
+00010970: 2020 2020 2020 7072 696e 7428 2263 6f6e        print("con
+00010980: 7472 6163 7420 636f 6e6e 6563 7469 6f6e  tract connection
+00010990: 2069 7320 222b 7374 7228 7365 6c66 2e77   is "+str(self.w
+000109a0: 6562 332e 6973 436f 6e6e 6563 7465 6428  eb3.isConnected(
+000109b0: 2929 290a 2020 2020 2020 2020 6966 2073  ))).        if s
+000109c0: 656c 662e 7765 6233 2e69 7343 6f6e 6e65  elf.web3.isConne
+000109d0: 6374 6564 2829 3a0a 2020 2020 2020 2020  cted():.        
+000109e0: 2020 2020 7365 6c66 2e6e 6f6e 6365 3d73      self.nonce=s
+000109f0: 656c 662e 7765 6233 2e65 7468 2e67 6574  elf.web3.eth.get
+00010a00: 5f74 7261 6e73 6163 7469 6f6e 5f63 6f75  _transaction_cou
+00010a10: 6e74 2873 656c 662e 6d79 5f70 7562 6c69  nt(self.my_publi
+00010a20: 635f 6b65 7929 0a20 2020 2020 2020 2020  c_key).         
+00010a30: 2020 2070 7269 6e74 2822 6e6f 6e63 6520     print("nonce 
+00010a40: 3d20 222c 7365 6c66 2e6e 6f6e 6365 290a  = ",self.nonce).
+00010a50: 2020 2020 2020 2020 7072 696e 7428 2723          print('#
+00010a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010a70: 2323 2323 2323 2323 2323 2327 290a 2020  ###########').  
+00010a80: 2020 2020 2020 2320 756e 6973 7761 705f        # uniswap_
+00010a90: 4661 6374 6f72 790a 2020 2020 2020 2020  Factory.        
+00010aa0: 7365 6c66 2e66 6163 746f 7279 5f61 6269  self.factory_abi
+00010ab0: 203d 206a 736f 6e2e 6c6f 6164 7328 7365   = json.loads(se
+00010ac0: 6c66 2e75 6e69 7377 6170 5f76 335f 6661  lf.uniswap_v3_fa
+00010ad0: 6374 6f72 795f 6162 6929 0a20 2020 2020  ctory_abi).     
+00010ae0: 2020 2073 656c 662e 7061 6972 5f61 6269     self.pair_abi
+00010af0: 3d6a 736f 6e2e 6c6f 6164 7328 7365 6c66  =json.loads(self
+00010b00: 2e75 6e69 7377 6170 5f76 335f 7061 6972  .uniswap_v3_pair
+00010b10: 5f61 6269 290a 2020 2020 2020 2020 7365  _abi).        se
+00010b20: 6c66 2e65 7263 3230 5f61 6269 3d6a 736f  lf.erc20_abi=jso
+00010b30: 6e2e 6c6f 6164 7328 7365 6c66 2e75 6e69  n.loads(self.uni
+00010b40: 7377 6170 5f76 335f 6572 6332 305f 6162  swap_v3_erc20_ab
+00010b50: 6929 0a20 2020 2020 2020 2073 656c 662e  i).        self.
+00010b60: 726f 7574 655f 6162 693d 6a73 6f6e 2e6c  route_abi=json.l
+00010b70: 6f61 6473 2873 656c 662e 756e 6973 7761  oads(self.uniswa
+00010b80: 705f 7633 5f72 6f75 7465 5f61 6269 290a  p_v3_route_abi).
+00010b90: 0a20 2020 2020 2020 2073 656c 662e 6661  .        self.fa
+00010ba0: 6374 6f72 795f 636f 6e74 7261 6374 203d  ctory_contract =
+00010bb0: 2073 656c 662e 7765 6233 2e65 7468 2e63   self.web3.eth.c
+00010bc0: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
+00010bd0: 7365 6c66 2e66 6163 746f 7279 5f61 6464  self.factory_add
+00010be0: 7265 7373 2c20 6162 693d 7365 6c66 2e66  ress, abi=self.f
+00010bf0: 6163 746f 7279 5f61 6269 290a 2020 2020  actory_abi).    
+00010c00: 2020 2020 7365 6c66 2e72 6f75 7465 5f63      self.route_c
+00010c10: 6f6e 7472 6163 743d 7365 6c66 2e77 6562  ontract=self.web
+00010c20: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
+00010c30: 6464 7265 7373 3d73 656c 662e 726f 7574  ddress=self.rout
+00010c40: 655f 6164 6472 6573 732c 6162 693d 7365  e_address,abi=se
+00010c50: 6c66 2e72 6f75 7465 5f61 6269 290a 636c  lf.route_abi).cl
+00010c60: 6173 7320 556e 6973 7761 7056 3346 6163  ass UniswapV3Fac
+00010c70: 746f 7279 3a0a 0a20 2020 2023 6661 6374  tory:..    #fact
+00010c80: 6f72 790a 2020 2020 2372 6574 7572 6e20  ory.    #return 
+00010c90: 6164 6472 6573 7320 6f66 2070 6f6f 6c20  address of pool 
+00010ca0: 666f 7220 746f 6b65 6e41 2061 6e64 2074  for tokenA and t
+00010cb0: 6f6b 656e 4220 7769 7468 2073 7065 6369  okenB with speci
+00010cc0: 6669 6320 6665 650a 2020 2020 2331 3030  fic fee.    #100
+00010cd0: 3030 2066 6f72 2031 2520 6665 652c 2033  00 for 1% fee, 3
+00010ce0: 3030 3020 666f 7220 302e 3325 2c20 616e  000 for 0.3%, an
+00010cf0: 6420 3530 3020 666f 7220 302e 3035 250a  d 500 for 0.05%.
+00010d00: 2020 2020 6465 6620 6765 7450 6f6f 6c28      def getPool(
+00010d10: 5f77 6562 333a 5765 6233 2c5f 6661 6374  _web3:Web3,_fact
+00010d20: 6f72 795f 6164 6472 6573 732c 5f61 6269  ory_address,_abi
+00010d30: 2c5f 746f 6b65 6e41 3a73 7472 2c5f 746f  ,_tokenA:str,_to
+00010d40: 6b65 6e42 3a73 7472 2c5f 6665 653a 696e  kenB:str,_fee:in
+00010d50: 7429 3a0a 2020 2020 2020 2020 7265 7475  t):.        retu
+00010d60: 726e 205f 7765 6233 2e65 7468 2e63 6f6e  rn _web3.eth.con
+00010d70: 7472 6163 7428 6164 6472 6573 733d 5f66  tract(address=_f
+00010d80: 6163 746f 7279 5f61 6464 7265 7373 2c20  actory_address, 
+00010d90: 6162 693d 5f61 6269 292e 6675 6e63 7469  abi=_abi).functi
+00010da0: 6f6e 732e 6765 7450 6f6f 6c28 5f74 6f6b  ons.getPool(_tok
+00010db0: 656e 412c 5f74 6f6b 656e 422c 5f66 6565  enA,_tokenB,_fee
+00010dc0: 292e 6361 6c6c 2829 0a20 2020 200a 636c  ).call().    .cl
+00010dd0: 6173 7320 556e 6973 7761 7056 3351 756f  ass UniswapV3Quo
+00010de0: 7465 723a 0a20 2020 2023 7265 7475 726e  ter:.    #return
+00010df0: 2061 6464 7265 7373 206f 6620 706f 6f6c   address of pool
+00010e00: 2066 6f72 2074 6f6b 656e 4120 616e 6420   for tokenA and 
+00010e10: 746f 6b65 6e42 2077 6974 6820 7370 6563  tokenB with spec
+00010e20: 6966 6963 2066 6565 0a20 2020 2023 3130  ific fee.    #10
+00010e30: 3030 3020 666f 7220 3125 2066 6565 2c20  000 for 1% fee, 
+00010e40: 3330 3030 2066 6f72 2030 2e33 252c 2061  3000 for 0.3%, a
+00010e50: 6e64 2035 3030 2066 6f72 2030 2e30 3525  nd 500 for 0.05%
+00010e60: 0a20 2020 2064 6566 2067 6574 506f 6f6c  .    def getPool
+00010e70: 285f 7765 6233 3a57 6562 332c 5f71 756f  (_web3:Web3,_quo
+00010e80: 7465 725f 6164 6472 6573 732c 5f61 6269  ter_address,_abi
+00010e90: 2c5f 746f 6b65 6e41 3a73 7472 2c5f 746f  ,_tokenA:str,_to
+00010ea0: 6b65 6e42 3a73 7472 2c5f 6665 653a 696e  kenB:str,_fee:in
+00010eb0: 7429 3a0a 2020 2020 2020 2020 7265 7475  t):.        retu
+00010ec0: 726e 205f 7765 6233 2e65 7468 2e63 6f6e  rn _web3.eth.con
+00010ed0: 7472 6163 7428 6164 6472 6573 733d 5f71  tract(address=_q
+00010ee0: 756f 7465 725f 6164 6472 6573 732c 2061  uoter_address, a
+00010ef0: 6269 3d5f 6162 6929 2e66 756e 6374 696f  bi=_abi).functio
+00010f00: 6e73 2e67 6574 506f 6f6c 285f 746f 6b65  ns.getPool(_toke
+00010f10: 6e41 2c5f 746f 6b65 6e42 2c5f 6665 6529  nA,_tokenB,_fee)
+00010f20: 2e63 616c 6c28 290a 2020 2020 0a20 2020  .call().    .   
+00010f30: 2023 2073 7472 7563 7420 5175 6f74 6545   # struct QuoteE
+00010f40: 7861 6374 496e 7075 7453 696e 676c 6550  xactInputSingleP
+00010f50: 6172 616d 7320 7b0a 2020 2020 2320 2020  arams {.    #   
+00010f60: 2020 6164 6472 6573 7320 746f 6b65 6e49    address tokenI
+00010f70: 6e3b 0a20 2020 2023 2020 2020 2061 6464  n;.    #     add
+00010f80: 7265 7373 2074 6f6b 656e 4f75 743b 0a20  ress tokenOut;. 
+00010f90: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
+00010fa0: 2061 6d6f 756e 7449 6e3b 0a20 2020 2023   amountIn;.    #
+00010fb0: 2020 2020 2075 696e 7432 3420 6665 653b       uint24 fee;
+00010fc0: 0a20 2020 2023 2020 2020 2075 696e 7431  .    #     uint1
+00010fd0: 3630 2073 7172 7450 7269 6365 4c69 6d69  60 sqrtPriceLimi
+00010fe0: 7458 3936 3b0a 2020 2020 2320 7d0a 2020  tX96;.    # }.  
+00010ff0: 2020 6465 6620 7175 6f74 6545 7861 6374    def quoteExact
+00011000: 496e 7075 7453 696e 676c 6528 5f77 6562  InputSingle(_web
+00011010: 333a 5765 6233 2c5f 7175 6f74 6572 5f61  3:Web3,_quoter_a
+00011020: 6464 7265 7373 2c5f 6162 692c 5f70 6172  ddress,_abi,_par
+00011030: 616d 293a 0a20 2020 2020 2020 2072 6574  am):.        ret
+00011040: 7572 6e20 5f77 6562 332e 6574 682e 636f  urn _web3.eth.co
+00011050: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
+00011060: 7175 6f74 6572 5f61 6464 7265 7373 2c20  quoter_address, 
+00011070: 6162 693d 5f61 6269 292e 6675 6e63 7469  abi=_abi).functi
+00011080: 6f6e 732e 7175 6f74 6545 7861 6374 496e  ons.quoteExactIn
+00011090: 7075 7453 696e 676c 6528 5f70 6172 616d  putSingle(_param
+000110a0: 292e 6361 6c6c 2829 0a0a 2020 2020 2370  ).call()..    #p
+000110b0: 6174 6820 7374 6172 7477 6974 6820 696e  ath startwith in
+000110c0: 7075 7420 746f 6b65 6e0a 2020 2020 6465  put token.    de
+000110d0: 6620 7175 6f74 6545 7861 6374 496e 7075  f quoteExactInpu
+000110e0: 7428 5f77 6562 333a 5765 6233 2c5f 7175  t(_web3:Web3,_qu
+000110f0: 6f74 6572 5f61 6464 7265 7373 2c5f 6162  oter_address,_ab
+00011100: 692c 7061 7468 2c5f 616d 6f75 6e74 5f69  i,path,_amount_i
+00011110: 6e29 3a0a 2020 2020 2020 2020 7265 7475  n):.        retu
+00011120: 726e 205f 7765 6233 2e65 7468 2e63 6f6e  rn _web3.eth.con
+00011130: 7472 6163 7428 6164 6472 6573 733d 5f71  tract(address=_q
+00011140: 756f 7465 725f 6164 6472 6573 732c 2061  uoter_address, a
+00011150: 6269 3d5f 6162 6929 2e66 756e 6374 696f  bi=_abi).functio
+00011160: 6e73 2e71 756f 7465 4578 6163 7449 6e70  ns.quoteExactInp
+00011170: 7574 2870 6174 682c 5f61 6d6f 756e 745f  ut(path,_amount_
+00011180: 696e 292e 6361 6c6c 2829 0a20 2020 200a  in).call().    .
+00011190: 2020 2020 2320 7374 7275 6374 2051 756f      # struct Quo
+000111a0: 7465 4578 6163 744f 7574 7075 7453 696e  teExactOutputSin
+000111b0: 676c 6550 6172 616d 7320 7b0a 2020 2020  gleParams {.    
+000111c0: 2320 2020 2020 6164 6472 6573 7320 746f  #     address to
+000111d0: 6b65 6e49 6e3b 0a20 2020 2023 2020 2020  kenIn;.    #    
+000111e0: 2061 6464 7265 7373 2074 6f6b 656e 4f75   address tokenOu
+000111f0: 743b 0a20 2020 2023 2020 2020 2075 696e  t;.    #     uin
+00011200: 7432 3536 2061 6d6f 756e 743b 0a20 2020  t256 amount;.   
+00011210: 2023 2020 2020 2075 696e 7432 3420 6665   #     uint24 fe
+00011220: 653b 0a20 2020 2023 2020 2020 2075 696e  e;.    #     uin
+00011230: 7431 3630 2073 7172 7450 7269 6365 4c69  t160 sqrtPriceLi
+00011240: 6d69 7458 3936 3b0a 2020 2020 2320 7d0a  mitX96;.    # }.
+00011250: 2020 2020 6465 6620 7175 6f74 6545 7861      def quoteExa
+00011260: 6374 4f75 7470 7574 5369 6e67 6c65 285f  ctOutputSingle(_
+00011270: 7765 6233 3a57 6562 332c 5f71 756f 7465  web3:Web3,_quote
+00011280: 725f 6164 6472 6573 732c 5f61 6269 2c5f  r_address,_abi,_
+00011290: 7061 7261 6d29 3a0a 2020 2020 2020 2020  param):.        
+000112a0: 7265 7475 726e 205f 7765 6233 2e65 7468  return _web3.eth
+000112b0: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
+000112c0: 733d 5f71 756f 7465 725f 6164 6472 6573  s=_quoter_addres
+000112d0: 732c 2061 6269 3d5f 6162 6929 2e66 756e  s, abi=_abi).fun
+000112e0: 6374 696f 6e73 2e71 756f 7465 4578 6163  ctions.quoteExac
+000112f0: 744f 7574 7075 7453 696e 676c 6528 5f70  tOutputSingle(_p
+00011300: 6172 616d 292e 6361 6c6c 2829 0a20 2020  aram).call().   
+00011310: 200a 2020 2020 2370 6174 6820 7374 6172   .    #path star
+00011320: 7420 7769 7468 206f 7574 7075 7420 746f  t with output to
+00011330: 6b65 6e0a 2020 2020 6465 6620 7175 6f74  ken.    def quot
+00011340: 6545 7861 6374 4f75 7470 7574 285f 7765  eExactOutput(_we
+00011350: 6233 3a57 6562 332c 5f71 756f 7465 725f  b3:Web3,_quoter_
+00011360: 6164 6472 6573 732c 5f61 6269 2c70 6174  address,_abi,pat
+00011370: 682c 5f61 6d6f 756e 745f 6f75 7429 3a0a  h,_amount_out):.
+00011380: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00011390: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
+000113a0: 7428 6164 6472 6573 733d 5f71 756f 7465  t(address=_quote
+000113b0: 725f 6164 6472 6573 732c 2061 6269 3d5f  r_address, abi=_
+000113c0: 6162 6929 2e66 756e 6374 696f 6e73 2e71  abi).functions.q
+000113d0: 756f 7465 4578 6163 744f 7574 7075 7428  uoteExactOutput(
+000113e0: 7061 7468 2c5f 616d 6f75 6e74 5f6f 7574  path,_amount_out
+000113f0: 292e 6361 6c6c 2829 0a0a 636c 6173 7320  ).call()..class 
+00011400: 556e 6973 7761 7056 3352 6f75 7465 723a  UniswapV3Router:
+00011410: 0a0a 2020 2020 2320 7374 7275 6374 2045  ..    # struct E
+00011420: 7861 6374 496e 7075 7453 696e 676c 6550  xactInputSingleP
+00011430: 6172 616d 7320 7b0a 2020 2020 2320 2020  arams {.    #   
+00011440: 2020 6164 6472 6573 7320 746f 6b65 6e49    address tokenI
+00011450: 6e3b 0a20 2020 2023 2020 2020 2061 6464  n;.    #     add
+00011460: 7265 7373 2074 6f6b 656e 4f75 743b 0a20  ress tokenOut;. 
+00011470: 2020 2023 2020 2020 2075 696e 7432 3420     #     uint24 
+00011480: 6665 653b 0a20 2020 2023 2020 2020 2061  fee;.    #     a
+00011490: 6464 7265 7373 2072 6563 6970 6965 6e74  ddress recipient
+000114a0: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
+000114b0: 3235 3620 6465 6164 6c69 6e65 3b0a 2020  256 deadline;.  
+000114c0: 2020 2320 2020 2020 7569 6e74 3235 3620    #     uint256 
+000114d0: 616d 6f75 6e74 496e 3b0a 2020 2020 2320  amountIn;.    # 
+000114e0: 2020 2020 7569 6e74 3235 3620 616d 6f75      uint256 amou
+000114f0: 6e74 4f75 744d 696e 696d 756d 3b0a 2020  ntOutMinimum;.  
+00011500: 2020 2320 2020 2020 7569 6e74 3136 3020    #     uint160 
+00011510: 7371 7274 5072 6963 654c 696d 6974 5839  sqrtPriceLimitX9
+00011520: 363b 0a20 2020 2023 207d 0a20 2020 2064  6;.    # }.    d
+00011530: 6566 2065 7861 6374 496e 7075 7453 696e  ef exactInputSin
+00011540: 676c 6528 5f77 6562 333a 5765 6233 2c5f  gle(_web3:Web3,_
+00011550: 726f 7574 655f 6164 6472 6573 732c 5f61  route_address,_a
+00011560: 6269 2c5f 6e6f 6e63 652c 5f70 7562 6c69  bi,_nonce,_publi
+00011570: 635f 6b65 792c 5f70 7269 7661 7465 5f6b  c_key,_private_k
+00011580: 6579 2c0a 2020 2020 2020 2020 5f74 6f6b  ey,.        _tok
+00011590: 656e 5f69 6e2c 5f74 6f6b 656e 5f6f 7574  en_in,_token_out
+000115a0: 2c5f 6665 652c 5f72 6563 6970 6965 6e74  ,_fee,_recipient
+000115b0: 2c5f 6465 6164 6c69 6e65 2c5f 616d 6f75  ,_deadline,_amou
+000115c0: 6e74 5f69 6e2c 5f61 6d6f 756e 745f 6f75  nt_in,_amount_ou
+000115d0: 745f 6d69 6e2c 5f73 7172 745f 7072 6963  t_min,_sqrt_pric
+000115e0: 655f 6c69 6d69 7429 3a0a 2020 2020 2020  e_limit):.      
+000115f0: 2020 726f 7574 655f 636f 6e74 7261 6374    route_contract
+00011600: 3d5f 7765 6233 2e65 7468 2e63 6f6e 7472  =_web3.eth.contr
+00011610: 6163 7428 6164 6472 6573 733d 5f72 6f75  act(address=_rou
+00011620: 7465 5f61 6464 7265 7373 2c20 6162 693d  te_address, abi=
+00011630: 5f61 6269 290a 2020 2020 2020 2020 6675  _abi).        fu
+00011640: 6e63 7469 6f6e 5f70 6172 616d 733d 7b0a  nction_params={.
+00011650: 2020 2020 2020 2020 2020 2020 2774 6f6b              'tok
+00011660: 656e 496e 273a 5f74 6f6b 656e 5f69 6e2c  enIn':_token_in,
+00011670: 0a20 2020 2020 2020 2020 2020 2027 746f  .            'to
+00011680: 6b65 6e4f 7574 273a 5f74 6f6b 656e 5f6f  kenOut':_token_o
+00011690: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
+000116a0: 2766 6565 273a 5f66 6565 2c0a 2020 2020  'fee':_fee,.    
+000116b0: 2020 2020 2020 2020 2772 6563 6970 6965          'recipie
+000116c0: 6e74 273a 5f72 6563 6970 6965 6e74 2c0a  nt':_recipient,.
+000116d0: 2020 2020 2020 2020 2020 2020 2764 6561              'dea
+000116e0: 646c 696e 6527 3a5f 6465 6164 6c69 6e65  dline':_deadline
+000116f0: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
+00011700: 6d6f 756e 7449 6e27 3a5f 616d 6f75 6e74  mountIn':_amount
+00011710: 5f69 6e2c 0a20 2020 2020 2020 2020 2020  _in,.           
+00011720: 2027 616d 6f75 6e74 4f75 744d 696e 696d   'amountOutMinim
+00011730: 756d 273a 5f61 6d6f 756e 745f 6f75 745f  um':_amount_out_
+00011740: 6d69 6e2c 0a20 2020 2020 2020 2020 2020  min,.           
+00011750: 2027 7371 7274 5072 6963 654c 696d 6974   'sqrtPriceLimit
+00011760: 5839 3627 3a5f 7371 7274 5f70 7269 6365  X96':_sqrt_price
+00011770: 5f6c 696d 6974 0a20 2020 2020 2020 207d  _limit.        }
+00011780: 0a20 2020 2020 2020 2023 2066 756e 6374  .        # funct
+00011790: 696f 6e5f 7061 7261 6d73 3d28 5f74 6f6b  ion_params=(_tok
+000117a0: 656e 5f69 6e2c 5f74 6f6b 656e 5f6f 7574  en_in,_token_out
+000117b0: 2c5f 6665 652c 5f72 6563 6970 6965 6e74  ,_fee,_recipient
+000117c0: 2c5f 6465 6164 6c69 6e65 2c5f 616d 6f75  ,_deadline,_amou
+000117d0: 6e74 5f69 6e2c 5f61 6d6f 756e 745f 6f75  nt_in,_amount_ou
+000117e0: 745f 6d69 6e2c 5f73 7172 745f 7072 6963  t_min,_sqrt_pric
+000117f0: 655f 6c69 6d69 7429 0a20 2020 2020 2020  e_limit).       
+00011800: 2073 7761 705f 6675 6e63 7469 6f6e 3d72   swap_function=r
+00011810: 6f75 7465 5f63 6f6e 7472 6163 742e 6675  oute_contract.fu
+00011820: 6e63 7469 6f6e 732e 6578 6163 7449 6e70  nctions.exactInp
+00011830: 7574 5369 6e67 6c65 2866 756e 6374 696f  utSingle(functio
+00011840: 6e5f 7061 7261 6d73 290a 2020 2020 2020  n_params).      
+00011850: 2020 7478 5f70 6172 616d 733d 7b0a 2020    tx_params={.  
+00011860: 2020 2020 2020 2020 2020 2766 726f 6d27            'from'
+00011870: 3a20 5f70 7562 6c69 635f 6b65 792c 0a20  : _public_key,. 
+00011880: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
+00011890: 6527 3a20 302c 0a20 2020 2020 2020 2020  e': 0,.         
+000118a0: 2020 2027 6e6f 6e63 6527 3a20 5f6e 6f6e     'nonce': _non
+000118b0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+000118c0: 2774 7970 6527 3a20 2730 7832 270a 2020  'type': '0x2'.  
+000118d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000118e0: 7472 616e 7361 6374 696f 6e3d 7377 6170  transaction=swap
+000118f0: 5f66 756e 6374 696f 6e2e 6275 696c 6454  _function.buildT
+00011900: 7261 6e73 6163 7469 6f6e 2874 785f 7061  ransaction(tx_pa
+00011910: 7261 6d73 290a 2020 2020 2020 2020 7369  rams).        si
+00011920: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
+00011930: 3d5f 7765 6233 2e65 7468 2e61 6363 6f75  =_web3.eth.accou
+00011940: 6e74 2e73 6967 6e5f 7472 616e 7361 6374  nt.sign_transact
+00011950: 696f 6e28 7472 616e 7361 6374 696f 6e2c  ion(transaction,
+00011960: 2070 7269 7661 7465 5f6b 6579 3d5f 7072   private_key=_pr
+00011970: 6976 6174 655f 6b65 7929 0a20 2020 2020  ivate_key).     
+00011980: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
+00011990: 746f 4865 7828 5f77 6562 332e 6574 682e  toHex(_web3.eth.
+000119a0: 7365 6e64 5f72 6177 5f74 7261 6e73 6163  send_raw_transac
+000119b0: 7469 6f6e 2873 6967 6e65 645f 7472 616e  tion(signed_tran
+000119c0: 7361 6374 696f 6e2e 7261 7754 7261 6e73  saction.rawTrans
+000119d0: 6163 7469 6f6e 2929 0a0a 2020 2020 2320  action))..    # 
+000119e0: 7374 7275 6374 2045 7861 6374 496e 7075  struct ExactInpu
+000119f0: 7450 6172 616d 7320 7b0a 2020 2020 2320  tParams {.    # 
+00011a00: 2020 2020 6279 7465 7320 7061 7468 3b0a      bytes path;.
+00011a10: 2020 2020 2320 2020 2020 6164 6472 6573      #     addres
+00011a20: 7320 7265 6369 7069 656e 743b 0a20 2020  s recipient;.   
+00011a30: 2023 2020 2020 2075 696e 7432 3536 2064   #     uint256 d
+00011a40: 6561 646c 696e 653b 0a20 2020 2023 2020  eadline;.    #  
+00011a50: 2020 2075 696e 7432 3536 2061 6d6f 756e     uint256 amoun
+00011a60: 7449 6e3b 0a20 2020 2023 2020 2020 2075  tIn;.    #     u
+00011a70: 696e 7432 3536 2061 6d6f 756e 744f 7574  int256 amountOut
+00011a80: 4d69 6e69 6d75 6d3b 0a20 2020 2023 207d  Minimum;.    # }
+00011a90: 0a20 2020 2064 6566 2065 7861 6374 496e  .    def exactIn
+00011aa0: 7075 7428 5f77 6562 333a 5765 6233 2c5f  put(_web3:Web3,_
+00011ab0: 726f 7574 655f 6164 6472 6573 732c 5f61  route_address,_a
+00011ac0: 6269 2c5f 6e6f 6e63 652c 5f70 7562 6c69  bi,_nonce,_publi
+00011ad0: 635f 6b65 792c 5f70 7269 7661 7465 5f6b  c_key,_private_k
+00011ae0: 6579 2c0a 2020 2020 2020 2020 5f70 6174  ey,.        _pat
+00011af0: 682c 5f72 6563 6970 6965 6e74 2c5f 6465  h,_recipient,_de
+00011b00: 6164 6c69 6e65 2c5f 616d 6f75 6e74 496e  adline,_amountIn
+00011b10: 2c5f 616d 6f75 6e74 4f75 744d 696e 293a  ,_amountOutMin):
+00011b20: 0a20 2020 2020 2020 2072 6f75 7465 5f63  .        route_c
+00011b30: 6f6e 7472 6163 743d 5f77 6562 332e 6574  ontract=_web3.et
+00011b40: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
+00011b50: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
+00011b60: 732c 2061 6269 3d5f 6162 6929 0a0a 2020  s, abi=_abi)..  
+00011b70: 2020 2020 2020 2320 7479 7065 3d5b 2762        # type=['b
+00011b80: 7974 6573 272c 2761 6464 7265 7373 272c  ytes','address',
+00011b90: 2775 696e 7432 3536 272c 2775 696e 7432  'uint256','uint2
+00011ba0: 3536 272c 2775 696e 7432 3536 275d 0a20  56','uint256']. 
+00011bb0: 2020 2020 2020 2023 2064 6174 613d 5b5f         # data=[_
+00011bc0: 7061 7468 2c5f 7265 6369 7069 656e 742c  path,_recipient,
+00011bd0: 5f64 6561 646c 696e 652c 5f61 6d6f 756e  _deadline,_amoun
+00011be0: 7449 6e2c 5f61 6d6f 756e 744f 7574 4d69  tIn,_amountOutMi
+00011bf0: 6e5d 0a20 2020 2020 2020 2023 2066 756e  n].        # fun
+00011c00: 6374 696f 6e5f 7061 7261 6d73 3d65 6e63  ction_params=enc
+00011c10: 6f64 655f 6162 6928 7479 7065 2c64 6174  ode_abi(type,dat
+00011c20: 6129 0a20 2020 2020 2020 2066 756e 6374  a).        funct
+00011c30: 696f 6e5f 7061 7261 6d73 3d7b 0a20 2020  ion_params={.   
+00011c40: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
+00011c50: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+00011c60: 2020 2027 7265 6369 7069 656e 7427 3a5f     'recipient':_
+00011c70: 7265 6369 7069 656e 742c 0a20 2020 2020  recipient,.     
+00011c80: 2020 2020 2020 2027 6465 6164 6c69 6e65         'deadline
+00011c90: 273a 5f64 6561 646c 696e 652c 0a20 2020  ':_deadline,.   
+00011ca0: 2020 2020 2020 2020 2027 616d 6f75 6e74           'amount
+00011cb0: 496e 273a 5f61 6d6f 756e 7449 6e2c 0a20  In':_amountIn,. 
+00011cc0: 2020 2020 2020 2020 2020 2027 616d 6f75             'amou
+00011cd0: 6e74 4f75 744d 696e 696d 756d 273a 5f61  ntOutMinimum':_a
+00011ce0: 6d6f 756e 744f 7574 4d69 6e0a 2020 2020  mountOutMin.    
+00011cf0: 2020 2020 7d0a 2020 2020 2020 2020 2320      }.        # 
+00011d00: 6675 6e63 7469 6f6e 5f70 6172 616d 733d  function_params=
+00011d10: 285f 7061 7468 2c5f 7265 6369 7069 656e  (_path,_recipien
+00011d20: 742c 5f64 6561 646c 696e 652c 5f61 6d6f  t,_deadline,_amo
+00011d30: 756e 7449 6e2c 5f61 6d6f 756e 744f 7574  untIn,_amountOut
+00011d40: 4d69 6e29 0a20 2020 2020 2020 2073 7761  Min).        swa
+00011d50: 705f 6675 6e63 7469 6f6e 3d72 6f75 7465  p_function=route
+00011d60: 5f63 6f6e 7472 6163 742e 6675 6e63 7469  _contract.functi
+00011d70: 6f6e 732e 6578 6163 7449 6e70 7574 2866  ons.exactInput(f
+00011d80: 756e 6374 696f 6e5f 7061 7261 6d73 290a  unction_params).
+00011d90: 2020 2020 2020 2020 7478 5f70 6172 616d          tx_param
+00011da0: 733d 7b0a 2020 2020 2020 2020 2020 2020  s={.            
+00011db0: 2766 726f 6d27 3a20 5f70 7562 6c69 635f  'from': _public_
+00011dc0: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
+00011dd0: 2027 7661 6c75 6527 3a20 302c 0a20 2020   'value': 0,.   
+00011de0: 2020 2020 2020 2020 2027 6e6f 6e63 6527           'nonce'
+00011df0: 3a20 5f6e 6f6e 6365 2c0a 2020 2020 2020  : _nonce,.      
+00011e00: 2020 2020 2020 2774 7970 6527 3a20 2730        'type': '0
+00011e10: 7832 272c 0a20 2020 2020 2020 2020 2020  x2',.           
+00011e20: 2023 2027 6761 7327 3a5f 6761 730a 2020   # 'gas':_gas.  
+00011e30: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00011e40: 7472 616e 7361 6374 696f 6e3d 7377 6170  transaction=swap
+00011e50: 5f66 756e 6374 696f 6e2e 6275 696c 6454  _function.buildT
+00011e60: 7261 6e73 6163 7469 6f6e 2874 785f 7061  ransaction(tx_pa
+00011e70: 7261 6d73 290a 2020 2020 2020 2020 7369  rams).        si
+00011e80: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
+00011e90: 3d5f 7765 6233 2e65 7468 2e61 6363 6f75  =_web3.eth.accou
+00011ea0: 6e74 2e73 6967 6e5f 7472 616e 7361 6374  nt.sign_transact
+00011eb0: 696f 6e28 7472 616e 7361 6374 696f 6e2c  ion(transaction,
+00011ec0: 2070 7269 7661 7465 5f6b 6579 3d5f 7072   private_key=_pr
+00011ed0: 6976 6174 655f 6b65 7929 0a20 2020 2020  ivate_key).     
+00011ee0: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
+00011ef0: 746f 4865 7828 5f77 6562 332e 6574 682e  toHex(_web3.eth.
+00011f00: 7365 6e64 5f72 6177 5f74 7261 6e73 6163  send_raw_transac
+00011f10: 7469 6f6e 2873 6967 6e65 645f 7472 616e  tion(signed_tran
+00011f20: 7361 6374 696f 6e2e 7261 7754 7261 6e73  saction.rawTrans
+00011f30: 6163 7469 6f6e 2929 0a0a 2020 2020 2320  action))..    # 
+00011f40: 7374 7275 6374 2045 7861 6374 4f75 7470  struct ExactOutp
+00011f50: 7574 5369 6e67 6c65 5061 7261 6d73 207b  utSingleParams {
+00011f60: 0a20 2020 2023 2020 2020 2061 6464 7265  .    #     addre
+00011f70: 7373 2074 6f6b 656e 496e 3b0a 2020 2020  ss tokenIn;.    
+00011f80: 2320 2020 2020 6164 6472 6573 7320 746f  #     address to
+00011f90: 6b65 6e4f 7574 3b0a 2020 2020 2320 2020  kenOut;.    #   
+00011fa0: 2020 7569 6e74 3234 2066 6565 3b0a 2020    uint24 fee;.  
+00011fb0: 2020 2320 2020 2020 6164 6472 6573 7320    #     address 
+00011fc0: 7265 6369 7069 656e 743b 0a20 2020 2023  recipient;.    #
+00011fd0: 2020 2020 2075 696e 7432 3536 2064 6561       uint256 dea
+00011fe0: 646c 696e 653b 0a20 2020 2023 2020 2020  dline;.    #    
+00011ff0: 2075 696e 7432 3536 2061 6d6f 756e 744f   uint256 amountO
+00012000: 7574 3b0a 2020 2020 2320 2020 2020 7569  ut;.    #     ui
+00012010: 6e74 3235 3620 616d 6f75 6e74 496e 4d61  nt256 amountInMa
+00012020: 7869 6d75 6d3b 0a20 2020 2023 2020 2020  ximum;.    #    
+00012030: 2075 696e 7431 3630 2073 7172 7450 7269   uint160 sqrtPri
+00012040: 6365 4c69 6d69 7458 3936 3b0a 2020 2020  ceLimitX96;.    
+00012050: 2320 7d0a 2020 2020 6465 6620 6578 6163  # }.    def exac
+00012060: 744f 7574 7075 7453 696e 676c 6528 5f77  tOutputSingle(_w
+00012070: 6562 333a 5765 6233 2c5f 726f 7574 655f  eb3:Web3,_route_
+00012080: 6164 6472 6573 732c 5f61 6269 2c5f 6e6f  address,_abi,_no
+00012090: 6e63 652c 5f70 7562 6c69 635f 6b65 792c  nce,_public_key,
+000120a0: 5f70 7269 7661 7465 5f6b 6579 2c0a 2020  _private_key,.  
+000120b0: 2020 2020 2020 5f74 6f6b 656e 5f69 6e2c        _token_in,
+000120c0: 5f74 6f6b 656e 5f6f 7574 2c5f 6665 652c  _token_out,_fee,
+000120d0: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
+000120e0: 6c69 6e65 2c5f 616d 6f75 6e74 5f6f 7574  line,_amount_out
+000120f0: 2c5f 616d 6f75 6e74 5f69 6e5f 6d61 782c  ,_amount_in_max,
+00012100: 5f73 7172 745f 7072 6963 655f 6c69 6d69  _sqrt_price_limi
+00012110: 7429 3a0a 2020 2020 2020 2020 726f 7574  t):.        rout
+00012120: 655f 636f 6e74 7261 6374 3d5f 7765 6233  e_contract=_web3
+00012130: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
+00012140: 6472 6573 733d 5f72 6f75 7465 5f61 6464  dress=_route_add
+00012150: 7265 7373 2c20 6162 693d 5f61 6269 290a  ress, abi=_abi).
+00012160: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+00012170: 5f70 6172 616d 3d7b 0a20 2020 2020 2020  _param={.       
+00012180: 2020 2020 2027 746f 6b65 6e49 6e27 3a5f       'tokenIn':_
+00012190: 746f 6b65 6e5f 696e 2c0a 2020 2020 2020  token_in,.      
+000121a0: 2020 2020 2020 2774 6f6b 656e 4f75 7427        'tokenOut'
+000121b0: 3a5f 746f 6b65 6e5f 6f75 742c 0a20 2020  :_token_out,.   
+000121c0: 2020 2020 2020 2020 2027 6665 6527 3a5f           'fee':_
+000121d0: 6665 652c 0a20 2020 2020 2020 2020 2020  fee,.           
+000121e0: 2027 7265 6369 7069 656e 7427 3a5f 7265   'recipient':_re
+000121f0: 6369 7069 656e 742c 0a20 2020 2020 2020  cipient,.       
+00012200: 2020 2020 2027 6465 6164 6c69 6e65 273a       'deadline':
+00012210: 5f64 6561 646c 696e 652c 0a20 2020 2020  _deadline,.     
+00012220: 2020 2020 2020 2027 616d 6f75 6e74 4f75         'amountOu
+00012230: 7427 3a5f 616d 6f75 6e74 5f6f 7574 2c0a  t':_amount_out,.
+00012240: 2020 2020 2020 2020 2020 2020 2761 6d6f              'amo
+00012250: 756e 7449 6e4d 6178 696d 756d 273a 5f61  untInMaximum':_a
+00012260: 6d6f 756e 745f 696e 5f6d 6178 2c0a 2020  mount_in_max,.  
+00012270: 2020 2020 2020 2020 2020 2773 7172 7450            'sqrtP
+00012280: 7269 6365 4c69 6d69 7458 3936 273a 5f73  riceLimitX96':_s
+00012290: 7172 745f 7072 6963 655f 6c69 6d69 740a  qrt_price_limit.
+000122a0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+000122b0: 2020 7377 6170 5f66 756e 6374 696f 6e3d    swap_function=
+000122c0: 726f 7574 655f 636f 6e74 7261 6374 2e66  route_contract.f
+000122d0: 756e 6374 696f 6e73 2e65 7861 6374 4f75  unctions.exactOu
+000122e0: 7470 7574 5369 6e67 6c65 2866 756e 6374  tputSingle(funct
+000122f0: 696f 6e5f 7061 7261 6d29 0a20 2020 2020  ion_param).     
+00012300: 2020 2074 785f 7061 7261 6d73 3d7b 0a20     tx_params={. 
+00012310: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
+00012320: 273a 205f 7075 626c 6963 5f6b 6579 2c0a  ': _public_key,.
+00012330: 2020 2020 2020 2020 2020 2020 2776 616c              'val
+00012340: 7565 273a 2030 2c0a 2020 2020 2020 2020  ue': 0,.        
+00012350: 2020 2020 276e 6f6e 6365 273a 205f 6e6f      'nonce': _no
+00012360: 6e63 652c 0a20 2020 2020 2020 2020 2020  nce,.           
+00012370: 2027 7479 7065 273a 2027 3078 3227 0a20   'type': '0x2'. 
+00012380: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00012390: 2074 7261 6e73 6163 7469 6f6e 3d73 7761   transaction=swa
+000123a0: 705f 6675 6e63 7469 6f6e 2e62 7569 6c64  p_function.build
+000123b0: 5472 616e 7361 6374 696f 6e28 7478 5f70  Transaction(tx_p
+000123c0: 6172 616d 7329 0a20 2020 2020 2020 2073  arams).        s
+000123d0: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+000123e0: 6e3d 5f77 6562 332e 6574 682e 6163 636f  n=_web3.eth.acco
+000123f0: 756e 742e 7369 676e 5f74 7261 6e73 6163  unt.sign_transac
+00012400: 7469 6f6e 2874 7261 6e73 6163 7469 6f6e  tion(transaction
+00012410: 2c20 7072 6976 6174 655f 6b65 793d 5f70  , private_key=_p
+00012420: 7269 7661 7465 5f6b 6579 290a 2020 2020  rivate_key).    
+00012430: 2020 2020 7265 7475 726e 205f 7765 6233      return _web3
+00012440: 2e74 6f48 6578 285f 7765 6233 2e65 7468  .toHex(_web3.eth
+00012450: 2e73 656e 645f 7261 775f 7472 616e 7361  .send_raw_transa
+00012460: 6374 696f 6e28 7369 676e 6564 5f74 7261  ction(signed_tra
+00012470: 6e73 6163 7469 6f6e 2e72 6177 5472 616e  nsaction.rawTran
+00012480: 7361 6374 696f 6e29 290a 0a0a 2020 2020  saction))...    
+00012490: 2320 7374 7275 6374 2045 7861 6374 4f75  # struct ExactOu
+000124a0: 7470 7574 5061 7261 6d73 207b 0a20 2020  tputParams {.   
+000124b0: 2023 2020 2020 2062 7974 6573 2070 6174   #     bytes pat
+000124c0: 683b 0a20 2020 2023 2020 2020 2061 6464  h;.    #     add
+000124d0: 7265 7373 2072 6563 6970 6965 6e74 3b0a  ress recipient;.
+000124e0: 2020 2020 2320 2020 2020 7569 6e74 3235      #     uint25
+000124f0: 3620 6465 6164 6c69 6e65 3b0a 2020 2020  6 deadline;.    
+00012500: 2320 2020 2020 7569 6e74 3235 3620 616d  #     uint256 am
+00012510: 6f75 6e74 4f75 743b 0a20 2020 2023 2020  ountOut;.    #  
+00012520: 2020 2075 696e 7432 3536 2061 6d6f 756e     uint256 amoun
+00012530: 7449 6e4d 6178 696d 756d 3b0a 2020 2020  tInMaximum;.    
+00012540: 2320 7d0a 2020 2020 6465 6620 6578 6163  # }.    def exac
+00012550: 744f 7574 7075 7428 5f77 6562 333a 5765  tOutput(_web3:We
+00012560: 6233 2c5f 726f 7574 655f 6164 6472 6573  b3,_route_addres
+00012570: 732c 5f61 6269 2c5f 6e6f 6e63 652c 5f70  s,_abi,_nonce,_p
+00012580: 7562 6c69 635f 6b65 792c 5f70 7269 7661  ublic_key,_priva
+00012590: 7465 5f6b 6579 2c0a 2020 2020 2020 2020  te_key,.        
+000125a0: 5f70 6174 682c 5f72 6563 6970 6965 6e74  _path,_recipient
+000125b0: 2c5f 6465 6164 6c69 6e65 2c5f 616d 6f75  ,_deadline,_amou
+000125c0: 6e74 5f6f 7574 2c5f 616d 6f75 6e74 5f69  nt_out,_amount_i
+000125d0: 6e5f 6d61 7829 3a0a 2020 2020 2020 2020  n_max):.        
+000125e0: 726f 7574 655f 636f 6e74 7261 6374 3d5f  route_contract=_
+000125f0: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
+00012600: 7428 6164 6472 6573 733d 5f72 6f75 7465  t(address=_route
+00012610: 5f61 6464 7265 7373 2c20 6162 693d 5f61  _address, abi=_a
+00012620: 6269 290a 2020 2020 2020 2020 6675 6e63  bi).        func
+00012630: 7469 6f6e 5f70 6172 616d 3d7b 0a20 2020  tion_param={.   
+00012640: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
+00012650: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+00012660: 2020 2027 7265 6369 7069 656e 7427 3a5f     'recipient':_
+00012670: 7265 6369 7069 656e 742c 0a20 2020 2020  recipient,.     
+00012680: 2020 2020 2020 2027 6465 6164 6c69 6e65         'deadline
+00012690: 273a 5f64 6561 646c 696e 652c 0a20 2020  ':_deadline,.   
+000126a0: 2020 2020 2020 2020 2027 616d 6f75 6e74           'amount
+000126b0: 4f75 7427 3a5f 616d 6f75 6e74 5f6f 7574  Out':_amount_out
+000126c0: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
+000126d0: 6d6f 756e 7449 6e4d 6178 696d 756d 273a  mountInMaximum':
+000126e0: 5f61 6d6f 756e 745f 696e 5f6d 6178 0a20  _amount_in_max. 
+000126f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00012700: 2073 7761 705f 6675 6e63 7469 6f6e 3d72   swap_function=r
+00012710: 6f75 7465 5f63 6f6e 7472 6163 742e 6675  oute_contract.fu
+00012720: 6e63 7469 6f6e 732e 6578 6163 744f 7574  nctions.exactOut
+00012730: 7075 7428 6675 6e63 7469 6f6e 5f70 6172  put(function_par
+00012740: 616d 290a 2020 2020 2020 2020 7478 5f70  am).        tx_p
+00012750: 6172 616d 733d 7b0a 2020 2020 2020 2020  arams={.        
+00012760: 2020 2020 2766 726f 6d27 3a20 5f70 7562      'from': _pub
+00012770: 6c69 635f 6b65 792c 0a20 2020 2020 2020  lic_key,.       
+00012780: 2020 2020 2027 7661 6c75 6527 3a20 302c       'value': 0,
+00012790: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
+000127a0: 6e63 6527 3a20 5f6e 6f6e 6365 2c0a 2020  nce': _nonce,.  
+000127b0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+000127c0: 3a20 2730 7832 270a 2020 2020 2020 2020  : '0x2'.        
+000127d0: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
+000127e0: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
+000127f0: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
+00012800: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
+00012810: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
+00012820: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
+00012830: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
+00012840: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
+00012850: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
+00012860: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
+00012870: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
+00012880: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
+00012890: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
+000128a0: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
+000128b0: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+000128c0: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
+000128d0: 2929 0a63 6c61 7373 204a 6f65 5632 4661  )).class JoeV2Fa
+000128e0: 6374 6f72 793a 0a20 2020 206a 6f65 5f66  ctory:.    joe_f
+000128f0: 6163 746f 7279 5f76 325f 6162 693d 6a73  actory_v2_abi=js
+00012900: 6f6e 2e6c 6f61 6473 2827 5b7b 2269 6e70  on.loads('[{"inp
+00012910: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00012920: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00012930: 226e 616d 6522 3a22 5f66 6565 5265 6369  "name":"_feeReci
+00012940: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
+00012950: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+00012960: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00012970: 3622 2c22 6e61 6d65 223a 225f 666c 6173  6","name":"_flas
+00012980: 684c 6f61 6e46 6565 222c 2274 7970 6522  hLoanFee","type"
+00012990: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
+000129a0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+000129b0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+000129c0: 6522 3a22 636f 6e73 7472 7563 746f 7222  e":"constructor"
+000129d0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+000129e0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+000129f0: 6e74 3235 3622 2c22 6e61 6d65 223a 2262  nt256","name":"b
+00012a00: 7022 2c22 7479 7065 223a 2275 696e 7432  p","type":"uint2
+00012a10: 3536 227d 5d2c 226e 616d 6522 3a22 4269  56"}],"name":"Bi
+00012a20: 6e48 656c 7065 725f 5f42 696e 5374 6570  nHelper__BinStep
+00012a30: 4f76 6572 666c 6f77 7322 2c22 7479 7065  Overflows","type
+00012a40: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00012a50: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00012a60: 4269 6e48 656c 7065 725f 5f49 644f 7665  BinHelper__IdOve
+00012a70: 7266 6c6f 7773 222c 2274 7970 6522 3a22  rflows","type":"
+00012a80: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00012a90: 223a 5b5d 2c22 6e61 6d65 223a 224c 4246  ":[],"name":"LBF
+00012aa0: 6163 746f 7279 5f5f 4164 6472 6573 735a  actory__AddressZ
+00012ab0: 6572 6f22 2c22 7479 7065 223a 2265 7272  ero","type":"err
+00012ac0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00012ad0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00012ae0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00012af0: 3a22 6269 6e53 7465 7022 2c22 7479 7065  :"binStep","type
+00012b00: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00012b10: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
+00012b20: 5f42 696e 5374 6570 4861 734e 6f50 7265  _BinStepHasNoPre
+00012b30: 7365 7422 2c22 7479 7065 223a 2265 7272  set","type":"err
+00012b40: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00012b50: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00012b60: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00012b70: 3a22 6c6f 7765 7242 6f75 6e64 222c 2274  :"lowerBound","t
+00012b80: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00012b90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00012ba0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
+00012bb0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
+00012bc0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
+00012bd0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00012be0: 3235 3622 2c22 6e61 6d65 223a 2268 6967  256","name":"hig
+00012bf0: 6865 7242 6f75 6e64 222c 2274 7970 6522  herBound","type"
+00012c00: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+00012c10: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
+00012c20: 4269 6e53 7465 7052 6571 7569 7265 6d65  BinStepRequireme
+00012c30: 6e74 7342 7265 6163 6865 6422 2c22 7479  ntsBreached","ty
+00012c40: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+00012c50: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00012c60: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+00012c70: 2c22 6e61 6d65 223a 2266 696c 7465 7250  ,"name":"filterP
+00012c80: 6572 696f 6422 2c22 7479 7065 223a 2275  eriod","type":"u
+00012c90: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
+00012ca0: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+00012cb0: 2c22 6e61 6d65 223a 2264 6563 6179 5065  ,"name":"decayPe
+00012cc0: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
+00012cd0: 6e74 3136 227d 5d2c 226e 616d 6522 3a22  nt16"}],"name":"
+00012ce0: 4c42 4661 6374 6f72 795f 5f44 6563 7265  LBFactory__Decre
+00012cf0: 6173 696e 6750 6572 696f 6473 222c 2274  asingPeriods","t
+00012d00: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00012d10: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00012d20: 223a 224c 4246 6163 746f 7279 5f5f 4661  ":"LBFactory__Fa
+00012d30: 6374 6f72 794c 6f63 6b49 7341 6c72 6561  ctoryLockIsAlrea
+00012d40: 6479 496e 5468 6553 616d 6553 7461 7465  dyInTheSameState
+00012d50: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00012d60: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00012d70: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00012d80: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
+00012d90: 6565 7322 2c22 7479 7065 223a 2275 696e  ees","type":"uin
+00012da0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00012db0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00012dc0: 2c22 6e61 6d65 223a 226d 6178 4665 6573  ,"name":"maxFees
+00012dd0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00012de0: 3622 7d5d 2c22 6e61 6d65 223a 224c 4246  6"}],"name":"LBF
+00012df0: 6163 746f 7279 5f5f 4665 6573 4162 6f76  actory__FeesAbov
+00012e00: 654d 6178 222c 2274 7970 6522 3a22 6572  eMax","type":"er
+00012e10: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+00012e20: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00012e30: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00012e40: 223a 2266 6565 7322 2c22 7479 7065 223a  ":"fees","type":
+00012e50: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00012e60: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00012e70: 3235 3622 2c22 6e61 6d65 223a 226d 6178  256","name":"max
+00012e80: 4665 6573 222c 2274 7970 6522 3a22 7569  Fees","type":"ui
+00012e90: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+00012ea0: 224c 4246 6163 746f 7279 5f5f 466c 6173  "LBFactory__Flas
+00012eb0: 684c 6f61 6e46 6565 4162 6f76 654d 6178  hLoanFeeAboveMax
+00012ec0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00012ed0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00012ee0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+00012ef0: 6472 6573 7322 2c22 6e61 6d65 223a 2275  dress","name":"u
+00012f00: 7365 7222 2c22 7479 7065 223a 2261 6464  ser","type":"add
+00012f10: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
+00012f20: 4c42 4661 6374 6f72 795f 5f46 756e 6374  LBFactory__Funct
+00012f30: 696f 6e49 734c 6f63 6b65 6446 6f72 5573  ionIsLockedForUs
+00012f40: 6572 7322 2c22 7479 7065 223a 2265 7272  ers","type":"err
+00012f50: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00012f60: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00012f70: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+00012f80: 222c 226e 616d 6522 3a22 746f 6b65 6e22  ","name":"token"
+00012f90: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00012fa0: 227d 5d2c 226e 616d 6522 3a22 4c42 4661  "}],"name":"LBFa
+00012fb0: 6374 6f72 795f 5f49 6465 6e74 6963 616c  ctory__Identical
+00012fc0: 4164 6472 6573 7365 7322 2c22 7479 7065  Addresses","type
+00012fd0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00012fe0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00012ff0: 4c42 4661 6374 6f72 795f 5f49 6d70 6c65  LBFactory__Imple
+00013000: 6d65 6e74 6174 696f 6e4e 6f74 5365 7422  mentationNotSet"
+00013010: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+00013020: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00013030: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00013040: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+00013050: 616d 6522 3a22 746f 6b65 6e58 222c 2274  ame":"tokenX","t
+00013060: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+00013070: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00013080: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+00013090: 222c 226e 616d 6522 3a22 746f 6b65 6e59  ","name":"tokenY
+000130a0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000130b0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+000130c0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000130d0: 616d 6522 3a22 5f62 696e 5374 6570 222c  ame":"_binStep",
+000130e0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000130f0: 7d5d 2c22 6e61 6d65 223a 224c 4246 6163  }],"name":"LBFac
+00013100: 746f 7279 5f5f 4c42 5061 6972 416c 7265  tory__LBPairAlre
+00013110: 6164 7945 7869 7374 7322 2c22 7479 7065  adyExists","type
+00013120: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00013130: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00013140: 4c42 4661 6374 6f72 795f 5f4c 4250 6169  LBFactory__LBPai
+00013150: 7249 676e 6f72 6564 4973 416c 7265 6164  rIgnoredIsAlread
+00013160: 7949 6e54 6865 5361 6d65 5374 6174 6522  yInTheSameState"
+00013170: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+00013180: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00013190: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+000131a0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+000131b0: 616d 6522 3a22 746f 6b65 6e58 222c 2274  ame":"tokenX","t
+000131c0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+000131d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000131e0: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+000131f0: 222c 226e 616d 6522 3a22 746f 6b65 6e59  ","name":"tokenY
+00013200: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00013210: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+00013220: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00013230: 616d 6522 3a22 6269 6e53 7465 7022 2c22  ame":"binStep","
+00013240: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00013250: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00013260: 6f72 795f 5f4c 4250 6169 724e 6f74 4372  ory__LBPairNotCr
+00013270: 6561 7465 6422 2c22 7479 7065 223a 2265  eated","type":"e
+00013280: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+00013290: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+000132a0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+000132b0: 6522 3a22 4c42 5061 6972 496d 706c 656d  e":"LBPairImplem
+000132c0: 656e 7461 7469 6f6e 222c 2274 7970 6522  entation","type"
+000132d0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+000132e0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
+000132f0: 4c42 5061 6972 5361 6665 7479 4368 6563  LBPairSafetyChec
+00013300: 6b46 6169 6c65 6422 2c22 7479 7065 223a  kFailed","type":
+00013310: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00013320: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00013330: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
+00013340: 6d65 223a 2270 726f 746f 636f 6c53 6861  me":"protocolSha
+00013350: 7265 222c 2274 7970 6522 3a22 7569 6e74  re","type":"uint
+00013360: 3136 227d 2c7b 2269 6e74 6572 6e61 6c54  16"},{"internalT
+00013370: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00013380: 6e61 6d65 223a 226d 6178 222c 2274 7970  name":"max","typ
+00013390: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+000133a0: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
+000133b0: 5f5f 5072 6f74 6f63 6f6c 5368 6172 654f  __ProtocolShareO
+000133c0: 7665 7266 6c6f 7773 222c 2274 7970 6522  verflows","type"
+000133d0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+000133e0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+000133f0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+00013400: 4552 4332 3022 2c22 6e61 6d65 223a 2271  ERC20","name":"q
+00013410: 756f 7465 4173 7365 7422 2c22 7479 7065  uoteAsset","type
+00013420: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
+00013430: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
+00013440: 5f51 756f 7465 4173 7365 7441 6c72 6561  _QuoteAssetAlrea
+00013450: 6479 5768 6974 656c 6973 7465 6422 2c22  dyWhitelisted","
+00013460: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00013470: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00013480: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+00013490: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+000134a0: 6522 3a22 7175 6f74 6541 7373 6574 222c  e":"quoteAsset",
+000134b0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+000134c0: 7d5d 2c22 6e61 6d65 223a 224c 4246 6163  }],"name":"LBFac
+000134d0: 746f 7279 5f5f 5175 6f74 6541 7373 6574  tory__QuoteAsset
+000134e0: 4e6f 7457 6869 7465 6c69 7374 6564 222c  NotWhitelisted",
+000134f0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00013500: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00013510: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00013520: 3136 222c 226e 616d 6522 3a22 7265 6475  16","name":"redu
+00013530: 6374 696f 6e46 6163 746f 7222 2c22 7479  ctionFactor","ty
+00013540: 7065 223a 2275 696e 7431 3622 7d2c 7b22  pe":"uint16"},{"
+00013550: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00013560: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00013570: 6d61 7822 2c22 7479 7065 223a 2275 696e  max","type":"uin
+00013580: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00013590: 4c42 4661 6374 6f72 795f 5f52 6564 7563  LBFactory__Reduc
+000135a0: 7469 6f6e 4661 6374 6f72 4f76 6572 666c  tionFactorOverfl
+000135b0: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
+000135c0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+000135d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000135e0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+000135f0: 3a22 6665 6552 6563 6970 6965 6e74 222c  :"feeRecipient",
+00013600: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00013610: 7d5d 2c22 6e61 6d65 223a 224c 4246 6163  }],"name":"LBFac
+00013620: 746f 7279 5f5f 5361 6d65 4665 6552 6563  tory__SameFeeRec
+00013630: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+00013640: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00013650: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00013660: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00013670: 6d65 223a 2266 6c61 7368 4c6f 616e 4665  me":"flashLoanFe
+00013680: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+00013690: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
+000136a0: 4661 6374 6f72 795f 5f53 616d 6546 6c61  Factory__SameFla
+000136b0: 7368 4c6f 616e 4665 6522 2c22 7479 7065  shLoanFee","type
+000136c0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+000136d0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+000136e0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+000136f0: 226e 616d 6522 3a22 4c42 5061 6972 496d  "name":"LBPairIm
+00013700: 706c 656d 656e 7461 7469 6f6e 222c 2274  plementation","t
+00013710: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+00013720: 2c22 6e61 6d65 223a 224c 4246 6163 746f  ,"name":"LBFacto
+00013730: 7279 5f5f 5361 6d65 496d 706c 656d 656e  ry__SameImplemen
+00013740: 7461 7469 6f6e 222c 2274 7970 6522 3a22  tation","type":"
+00013750: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00013760: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00013770: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00013780: 6d65 223a 2278 222c 2274 7970 6522 3a22  me":"x","type":"
+00013790: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+000137a0: 726e 616c 5479 7065 223a 2269 6e74 3235  rnalType":"int25
+000137b0: 3622 2c22 6e61 6d65 223a 2279 222c 2274  6","name":"y","t
+000137c0: 7970 6522 3a22 696e 7432 3536 227d 5d2c  ype":"int256"}],
+000137d0: 226e 616d 6522 3a22 4d61 7468 3132 3878  "name":"Math128x
+000137e0: 3132 385f 5f50 6f77 6572 556e 6465 7266  128__PowerUnderf
+000137f0: 6c6f 7722 2c22 7479 7065 223a 2265 7272  low","type":"err
+00013800: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00013810: 5d2c 226e 616d 6522 3a22 5065 6e64 696e  ],"name":"Pendin
+00013820: 674f 776e 6162 6c65 5f5f 4164 6472 6573  gOwnable__Addres
+00013830: 735a 6572 6f22 2c22 7479 7065 223a 2265  sZero","type":"e
+00013840: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+00013850: 3a5b 5d2c 226e 616d 6522 3a22 5065 6e64  :[],"name":"Pend
+00013860: 696e 674f 776e 6162 6c65 5f5f 4e6f 5065  ingOwnable__NoPe
+00013870: 6e64 696e 674f 776e 6572 222c 2274 7970  ndingOwner","typ
+00013880: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+00013890: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+000138a0: 2250 656e 6469 6e67 4f77 6e61 626c 655f  "PendingOwnable_
+000138b0: 5f4e 6f74 4f77 6e65 7222 2c22 7479 7065  _NotOwner","type
+000138c0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+000138d0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+000138e0: 5065 6e64 696e 674f 776e 6162 6c65 5f5f  PendingOwnable__
+000138f0: 4e6f 7450 656e 6469 6e67 4f77 6e65 7222  NotPendingOwner"
+00013900: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+00013910: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00013920: 616d 6522 3a22 5065 6e64 696e 674f 776e  ame":"PendingOwn
+00013930: 6162 6c65 5f5f 5065 6e64 696e 674f 776e  able__PendingOwn
+00013940: 6572 416c 7265 6164 7953 6574 222c 2274  erAlreadySet","t
+00013950: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00013960: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00013970: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00013980: 3622 2c22 6e61 6d65 223a 2278 222c 2274  6","name":"x","t
+00013990: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+000139a0: 2c22 6e61 6d65 223a 2253 6166 6543 6173  ,"name":"SafeCas
+000139b0: 745f 5f45 7863 6565 6473 3136 4269 7473  t__Exceeds16Bits
+000139c0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+000139d0: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
+000139e0: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
+000139f0: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+00013a00: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00013a10: 626f 6f6c 222c 226e 616d 6522 3a22 756e  bool","name":"un
+00013a20: 6c6f 636b 6564 222c 2274 7970 6522 3a22  locked","type":"
+00013a30: 626f 6f6c 227d 5d2c 226e 616d 6522 3a22  bool"}],"name":"
+00013a40: 4661 6374 6f72 794c 6f63 6b65 6453 7461  FactoryLockedSta
+00013a50: 7475 7355 7064 6174 6564 222c 2274 7970  tusUpdated","typ
+00013a60: 6522 3a22 6576 656e 7422 7d2c 7b22 616e  e":"event"},{"an
+00013a70: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
+00013a80: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
+00013a90: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
+00013aa0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00013ab0: 222c 226e 616d 6522 3a22 7365 6e64 6572  ","name":"sender
+00013ac0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00013ad0: 7322 7d2c 7b22 696e 6465 7865 6422 3a74  s"},{"indexed":t
+00013ae0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+00013af0: 6522 3a22 636f 6e74 7261 6374 2049 4c42  e":"contract ILB
+00013b00: 5061 6972 222c 226e 616d 6522 3a22 4c42  Pair","name":"LB
+00013b10: 5061 6972 222c 2274 7970 6522 3a22 6164  Pair","type":"ad
+00013b20: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
+00013b30: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00013b40: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00013b50: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
+00013b60: 7022 2c22 7479 7065 223a 2275 696e 7432  p","type":"uint2
+00013b70: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
+00013b80: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
+00013b90: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00013ba0: 6e61 6d65 223a 2262 6173 6546 6163 746f  name":"baseFacto
+00013bb0: 7222 2c22 7479 7065 223a 2275 696e 7432  r","type":"uint2
+00013bc0: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
+00013bd0: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
+00013be0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00013bf0: 6e61 6d65 223a 2266 696c 7465 7250 6572  name":"filterPer
+00013c00: 696f 6422 2c22 7479 7065 223a 2275 696e  iod","type":"uin
+00013c10: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+00013c20: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+00013c30: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00013c40: 2c22 6e61 6d65 223a 2264 6563 6179 5065  ,"name":"decayPe
+00013c50: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
+00013c60: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+00013c70: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00013c80: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00013c90: 222c 226e 616d 6522 3a22 7265 6475 6374  ","name":"reduct
+00013ca0: 696f 6e46 6163 746f 7222 2c22 7479 7065  ionFactor","type
+00013cb0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00013cc0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
+00013cd0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00013ce0: 6e74 3235 3622 2c22 6e61 6d65 223a 2276  nt256","name":"v
+00013cf0: 6172 6961 626c 6546 6565 436f 6e74 726f  ariableFeeContro
+00013d00: 6c22 2c22 7479 7065 223a 2275 696e 7432  l","type":"uint2
+00013d10: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
+00013d20: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
+00013d30: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00013d40: 6e61 6d65 223a 2270 726f 746f 636f 6c53  name":"protocolS
+00013d50: 6861 7265 222c 2274 7970 6522 3a22 7569  hare","type":"ui
+00013d60: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+00013d70: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00013d80: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00013d90: 222c 226e 616d 6522 3a22 6d61 7856 6f6c  ","name":"maxVol
+00013da0: 6174 696c 6974 7941 6363 756d 756c 6174  atilityAccumulat
+00013db0: 6564 222c 2274 7970 6522 3a22 7569 6e74  ed","type":"uint
+00013dc0: 3235 3622 7d5d 2c22 6e61 6d65 223a 2246  256"}],"name":"F
+00013dd0: 6565 5061 7261 6d65 7465 7273 5365 7422  eeParametersSet"
+00013de0: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
+00013df0: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
+00013e00: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
+00013e10: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+00013e20: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00013e30: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+00013e40: 6f6c 6452 6563 6970 6965 6e74 222c 2274  oldRecipient","t
+00013e50: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+00013e60: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
+00013e70: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+00013e80: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00013e90: 3a22 6e65 7752 6563 6970 6965 6e74 222c  :"newRecipient",
+00013ea0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00013eb0: 7d5d 2c22 6e61 6d65 223a 2246 6565 5265  }],"name":"FeeRe
+00013ec0: 6369 7069 656e 7453 6574 222c 2274 7970  cipientSet","typ
+00013ed0: 6522 3a22 6576 656e 7422 7d2c 7b22 616e  e":"event"},{"an
+00013ee0: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
+00013ef0: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
+00013f00: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+00013f10: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00013f20: 3622 2c22 6e61 6d65 223a 226f 6c64 466c  6","name":"oldFl
+00013f30: 6173 684c 6f61 6e46 6565 222c 2274 7970  ashLoanFee","typ
+00013f40: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+00013f50: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+00013f60: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00013f70: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00013f80: 6e65 7746 6c61 7368 4c6f 616e 4665 6522  newFlashLoanFee"
+00013f90: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00013fa0: 227d 5d2c 226e 616d 6522 3a22 466c 6173  "}],"name":"Flas
+00013fb0: 684c 6f61 6e46 6565 5365 7422 2c22 7479  hLoanFeeSet","ty
+00013fc0: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
+00013fd0: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
+00013fe0: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
+00013ff0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+00014000: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+00014010: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
+00014020: 223a 2274 6f6b 656e 5822 2c22 7479 7065  ":"tokenX","type
+00014030: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00014040: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+00014050: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00014060: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+00014070: 616d 6522 3a22 746f 6b65 6e59 222c 2274  ame":"tokenY","t
+00014080: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+00014090: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
+000140a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000140b0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+000140c0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
+000140d0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+000140e0: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
+000140f0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00014100: 7472 6163 7420 494c 4250 6169 7222 2c22  tract ILBPair","
+00014110: 6e61 6d65 223a 224c 4250 6169 7222 2c22  name":"LBPair","
+00014120: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00014130: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+00014140: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+00014150: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00014160: 223a 2270 6964 222c 2274 7970 6522 3a22  ":"pid","type":"
+00014170: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+00014180: 223a 224c 4250 6169 7243 7265 6174 6564  ":"LBPairCreated
+00014190: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
+000141a0: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
+000141b0: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
+000141c0: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+000141d0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+000141e0: 6f6e 7472 6163 7420 494c 4250 6169 7222  ontract ILBPair"
+000141f0: 2c22 6e61 6d65 223a 224c 4250 6169 7222  ,"name":"LBPair"
+00014200: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00014210: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
+00014220: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+00014230: 6522 3a22 626f 6f6c 222c 226e 616d 6522  e":"bool","name"
+00014240: 3a22 6967 6e6f 7265 6422 2c22 7479 7065  :"ignored","type
+00014250: 223a 2262 6f6f 6c22 7d5d 2c22 6e61 6d65  ":"bool"}],"name
+00014260: 223a 224c 4250 6169 7249 676e 6f72 6564  ":"LBPairIgnored
+00014270: 5374 6174 6543 6861 6e67 6564 222c 2274  StateChanged","t
+00014280: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
+00014290: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
+000142a0: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
+000142b0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+000142c0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+000142d0: 6573 7322 2c22 6e61 6d65 223a 226f 6c64  ess","name":"old
+000142e0: 4c42 5061 6972 496d 706c 656d 656e 7461  LBPairImplementa
+000142f0: 7469 6f6e 222c 2274 7970 6522 3a22 6164  tion","type":"ad
+00014300: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
+00014310: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00014320: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00014330: 222c 226e 616d 6522 3a22 4c42 5061 6972  ","name":"LBPair
+00014340: 496d 706c 656d 656e 7461 7469 6f6e 222c  Implementation",
+00014350: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00014360: 7d5d 2c22 6e61 6d65 223a 224c 4250 6169  }],"name":"LBPai
+00014370: 7249 6d70 6c65 6d65 6e74 6174 696f 6e53  rImplementationS
+00014380: 6574 222c 2274 7970 6522 3a22 6576 656e  et","type":"even
+00014390: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+000143a0: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+000143b0: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+000143c0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+000143d0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+000143e0: 3a22 7072 6576 696f 7573 4f77 6e65 7222  :"previousOwner"
+000143f0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00014400: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+00014410: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+00014420: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00014430: 6522 3a22 6e65 774f 776e 6572 222c 2274  e":"newOwner","t
+00014440: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+00014450: 2c22 6e61 6d65 223a 224f 776e 6572 7368  ,"name":"Ownersh
+00014460: 6970 5472 616e 7366 6572 7265 6422 2c22  ipTransferred","
+00014470: 7479 7065 223a 2265 7665 6e74 227d 2c7b  type":"event"},{
+00014480: 2261 6e6f 6e79 6d6f 7573 223a 6661 6c73  "anonymous":fals
+00014490: 652c 2269 6e70 7574 7322 3a5b 7b22 696e  e,"inputs":[{"in
+000144a0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
+000144b0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+000144c0: 6573 7322 2c22 6e61 6d65 223a 2270 656e  ess","name":"pen
+000144d0: 6469 6e67 4f77 6e65 7222 2c22 7479 7065  dingOwner","type
+000144e0: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
+000144f0: 616d 6522 3a22 5065 6e64 696e 674f 776e  ame":"PendingOwn
+00014500: 6572 5365 7422 2c22 7479 7065 223a 2265  erSet","type":"e
+00014510: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
+00014520: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
+00014530: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
+00014540: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+00014550: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00014560: 6d65 223a 2262 696e 5374 6570 222c 2274  me":"binStep","t
+00014570: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+00014580: 2c22 6e61 6d65 223a 2250 7265 7365 7452  ,"name":"PresetR
+00014590: 656d 6f76 6564 222c 2274 7970 6522 3a22  emoved","type":"
+000145a0: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
+000145b0: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
+000145c0: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
+000145d0: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+000145e0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000145f0: 616d 6522 3a22 6269 6e53 7465 7022 2c22  ame":"binStep","
+00014600: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00014610: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+00014620: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+00014630: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00014640: 223a 2262 6173 6546 6163 746f 7222 2c22  ":"baseFactor","
+00014650: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00014660: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+00014670: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+00014680: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00014690: 223a 2266 696c 7465 7250 6572 696f 6422  ":"filterPeriod"
+000146a0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+000146b0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
+000146c0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+000146d0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+000146e0: 6d65 223a 2264 6563 6179 5065 7269 6f64  me":"decayPeriod
+000146f0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00014700: 3622 7d2c 7b22 696e 6465 7865 6422 3a66  6"},{"indexed":f
+00014710: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
+00014720: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00014730: 616d 6522 3a22 7265 6475 6374 696f 6e46  ame":"reductionF
+00014740: 6163 746f 7222 2c22 7479 7065 223a 2275  actor","type":"u
+00014750: 696e 7432 3536 227d 2c7b 2269 6e64 6578  int256"},{"index
+00014760: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+00014770: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00014780: 3622 2c22 6e61 6d65 223a 2276 6172 6961  6","name":"varia
+00014790: 626c 6546 6565 436f 6e74 726f 6c22 2c22  bleFeeControl","
+000147a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+000147b0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+000147c0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+000147d0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+000147e0: 223a 2270 726f 746f 636f 6c53 6861 7265  ":"protocolShare
+000147f0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00014800: 3622 7d2c 7b22 696e 6465 7865 6422 3a66  6"},{"indexed":f
+00014810: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
+00014820: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00014830: 616d 6522 3a22 6d61 7856 6f6c 6174 696c  ame":"maxVolatil
+00014840: 6974 7941 6363 756d 756c 6174 6564 222c  ityAccumulated",
+00014850: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00014860: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+00014870: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+00014880: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00014890: 6522 3a22 7361 6d70 6c65 4c69 6665 7469  e":"sampleLifeti
+000148a0: 6d65 222c 2274 7970 6522 3a22 7569 6e74  me","type":"uint
+000148b0: 3235 3622 7d5d 2c22 6e61 6d65 223a 2250  256"}],"name":"P
+000148c0: 7265 7365 7453 6574 222c 2274 7970 6522  resetSet","type"
+000148d0: 3a22 6576 656e 7422 7d2c 7b22 616e 6f6e  :"event"},{"anon
+000148e0: 796d 6f75 7322 3a66 616c 7365 2c22 696e  ymous":false,"in
+000148f0: 7075 7473 223a 5b7b 2269 6e64 6578 6564  puts":[{"indexed
+00014900: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+00014910: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00014920: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+00014930: 7175 6f74 6541 7373 6574 222c 2274 7970  quoteAsset","typ
+00014940: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+00014950: 6e61 6d65 223a 2251 756f 7465 4173 7365  name":"QuoteAsse
+00014960: 7441 6464 6564 222c 2274 7970 6522 3a22  tAdded","type":"
+00014970: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
+00014980: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
+00014990: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
+000149a0: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+000149b0: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+000149c0: 5243 3230 222c 226e 616d 6522 3a22 7175  RC20","name":"qu
+000149d0: 6f74 6541 7373 6574 222c 2274 7970 6522  oteAsset","type"
+000149e0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+000149f0: 6d65 223a 2251 756f 7465 4173 7365 7452  me":"QuoteAssetR
+00014a00: 656d 6f76 6564 222c 2274 7970 6522 3a22  emoved","type":"
+00014a10: 6576 656e 7422 7d2c 7b22 696e 7075 7473  event"},{"inputs
+00014a20: 223a 5b5d 2c22 6e61 6d65 223a 224c 4250  ":[],"name":"LBP
+00014a30: 6169 7249 6d70 6c65 6d65 6e74 6174 696f  airImplementatio
+00014a40: 6e22 2c22 6f75 7470 7574 7322 3a5b 7b22  n","outputs":[{"
+00014a50: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00014a60: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+00014a70: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00014a80: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
+00014a90: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00014aa0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00014ab0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00014ac0: 616d 6522 3a22 4d41 585f 4249 4e5f 5354  ame":"MAX_BIN_ST
+00014ad0: 4550 222c 226f 7574 7075 7473 223a 5b7b  EP","outputs":[{
+00014ae0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00014af0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00014b00: 2222 2c22 7479 7065 223a 2275 696e 7432  "","type":"uint2
+00014b10: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
+00014b20: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+00014b30: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00014b40: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00014b50: 6e61 6d65 223a 224d 4158 5f46 4545 222c  name":"MAX_FEE",
+00014b60: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+00014b70: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00014b80: 3235 3622 2c22 6e61 6d65 223a 2222 2c22  256","name":"","
+00014b90: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00014ba0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00014bb0: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
+00014bc0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00014bd0: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00014be0: 223a 224d 4158 5f50 524f 544f 434f 4c5f  ":"MAX_PROTOCOL_
+00014bf0: 5348 4152 4522 2c22 6f75 7470 7574 7322  SHARE","outputs"
+00014c00: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00014c10: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00014c20: 6522 3a22 222c 2274 7970 6522 3a22 7569  e":"","type":"ui
+00014c30: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
+00014c40: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+00014c50: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00014c60: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00014c70: 5d2c 226e 616d 6522 3a22 4d49 4e5f 4249  ],"name":"MIN_BI
+00014c80: 4e5f 5354 4550 222c 226f 7574 7075 7473  N_STEP","outputs
+00014c90: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00014ca0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00014cb0: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
+00014cc0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+00014cd0: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
+00014ce0: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
+00014cf0: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+00014d00: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00014d10: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+00014d20: 3022 2c22 6e61 6d65 223a 225f 7175 6f74  0","name":"_quot
+00014d30: 6541 7373 6574 222c 2274 7970 6522 3a22  eAsset","type":"
+00014d40: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+00014d50: 223a 2261 6464 5175 6f74 6541 7373 6574  ":"addQuoteAsset
+00014d60: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+00014d70: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00014d80: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00014d90: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00014da0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00014db0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00014dc0: 7432 3536 222c 226e 616d 6522 3a22 222c  t256","name":"",
+00014dd0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00014de0: 7d5d 2c22 6e61 6d65 223a 2261 6c6c 4c42  }],"name":"allLB
+00014df0: 5061 6972 7322 2c22 6f75 7470 7574 7322  Pairs","outputs"
+00014e00: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00014e10: 223a 2263 6f6e 7472 6163 7420 494c 4250  ":"contract ILBP
+00014e20: 6169 7222 2c22 6e61 6d65 223a 2222 2c22  air","name":"","
+00014e30: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00014e40: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00014e50: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
+00014e60: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00014e70: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00014e80: 223a 2262 6563 6f6d 654f 776e 6572 222c  ":"becomeOwner",
+00014e90: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+00014ea0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00014eb0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00014ec0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00014ed0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00014ee0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+00014ef0: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+00014f00: 6522 3a22 5f74 6f6b 656e 5822 2c22 7479  e":"_tokenX","ty
+00014f10: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+00014f20: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00014f30: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
+00014f40: 2c22 6e61 6d65 223a 225f 746f 6b65 6e59  ,"name":"_tokenY
+00014f50: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00014f60: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+00014f70: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
+00014f80: 6d65 223a 225f 6163 7469 7665 4964 222c  me":"_activeId",
+00014f90: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
+00014fa0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00014fb0: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
+00014fc0: 3a22 5f62 696e 5374 6570 222c 2274 7970  :"_binStep","typ
+00014fd0: 6522 3a22 7569 6e74 3136 227d 5d2c 226e  e":"uint16"}],"n
+00014fe0: 616d 6522 3a22 6372 6561 7465 4c42 5061  ame":"createLBPa
+00014ff0: 6972 222c 226f 7574 7075 7473 223a 5b7b  ir","outputs":[{
+00015000: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00015010: 636f 6e74 7261 6374 2049 4c42 5061 6972  contract ILBPair
+00015020: 222c 226e 616d 6522 3a22 5f4c 4250 6169  ","name":"_LBPai
+00015030: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
+00015040: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
+00015050: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+00015060: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+00015070: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+00015080: 223a 5b5d 2c22 6e61 6d65 223a 2263 7265  ":[],"name":"cre
+00015090: 6174 696f 6e55 6e6c 6f63 6b65 6422 2c22  ationUnlocked","
+000150a0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+000150b0: 726e 616c 5479 7065 223a 2262 6f6f 6c22  rnalType":"bool"
+000150c0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
+000150d0: 223a 2262 6f6f 6c22 7d5d 2c22 7374 6174  ":"bool"}],"stat
+000150e0: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+000150f0: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+00015100: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+00015110: 3a5b 5d2c 226e 616d 6522 3a22 6665 6552  :[],"name":"feeR
+00015120: 6563 6970 6965 6e74 222c 226f 7574 7075  ecipient","outpu
+00015130: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00015140: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+00015150: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
+00015160: 2261 6464 7265 7373 227d 5d2c 2273 7461  "address"}],"sta
+00015170: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
+00015180: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
+00015190: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+000151a0: 223a 5b5d 2c22 6e61 6d65 223a 2266 6c61  ":[],"name":"fla
+000151b0: 7368 4c6f 616e 4665 6522 2c22 6f75 7470  shLoanFee","outp
+000151c0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+000151d0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+000151e0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+000151f0: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
+00015200: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00015210: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+00015220: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00015230: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00015240: 7065 223a 2263 6f6e 7472 6163 7420 494c  pe":"contract IL
+00015250: 4250 6169 7222 2c22 6e61 6d65 223a 225f  BPair","name":"_
+00015260: 4c42 5061 6972 222c 2274 7970 6522 3a22  LBPair","type":"
+00015270: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+00015280: 223a 2266 6f72 6365 4465 6361 7922 2c22  ":"forceDecay","
+00015290: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
+000152a0: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
+000152b0: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
+000152c0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+000152d0: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+000152e0: 223a 2267 6574 416c 6c42 696e 5374 6570  ":"getAllBinStep
+000152f0: 7322 2c22 6f75 7470 7574 7322 3a5b 7b22  s","outputs":[{"
+00015300: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00015310: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+00015320: 3a22 7072 6573 6574 7342 696e 5374 6570  :"presetsBinStep
+00015330: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00015340: 365b 5d22 7d5d 2c22 7374 6174 654d 7574  6[]"}],"stateMut
+00015350: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00015360: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00015370: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00015380: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+00015390: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+000153a0: 226e 616d 6522 3a22 5f74 6f6b 656e 5822  "name":"_tokenX"
+000153b0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+000153c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+000153d0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+000153e0: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
+000153f0: 6b65 6e59 222c 2274 7970 6522 3a22 6164  kenY","type":"ad
+00015400: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
+00015410: 2267 6574 416c 6c4c 4250 6169 7273 222c  "getAllLBPairs",
+00015420: 226f 7574 7075 7473 223a 5b7b 2263 6f6d  "outputs":[{"com
+00015430: 706f 6e65 6e74 7322 3a5b 7b22 696e 7465  ponents":[{"inte
+00015440: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
+00015450: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
+00015460: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
+00015470: 3136 227d 2c7b 2269 6e74 6572 6e61 6c54  16"},{"internalT
+00015480: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+00015490: 4c42 5061 6972 222c 226e 616d 6522 3a22  LBPair","name":"
+000154a0: 4c42 5061 6972 222c 2274 7970 6522 3a22  LBPair","type":"
+000154b0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+000154c0: 726e 616c 5479 7065 223a 2262 6f6f 6c22  rnalType":"bool"
+000154d0: 2c22 6e61 6d65 223a 2263 7265 6174 6564  ,"name":"created
+000154e0: 4279 4f77 6e65 7222 2c22 7479 7065 223a  ByOwner","type":
+000154f0: 2262 6f6f 6c22 7d2c 7b22 696e 7465 726e  "bool"},{"intern
+00015500: 616c 5479 7065 223a 2262 6f6f 6c22 2c22  alType":"bool","
+00015510: 6e61 6d65 223a 2269 676e 6f72 6564 466f  name":"ignoredFo
+00015520: 7252 6f75 7469 6e67 222c 2274 7970 6522  rRouting","type"
+00015530: 3a22 626f 6f6c 227d 5d2c 2269 6e74 6572  :"bool"}],"inter
+00015540: 6e61 6c54 7970 6522 3a22 7374 7275 6374  nalType":"struct
+00015550: 2049 4c42 4661 6374 6f72 792e 4c42 5061   ILBFactory.LBPa
+00015560: 6972 496e 666f 726d 6174 696f 6e5b 5d22  irInformation[]"
+00015570: 2c22 6e61 6d65 223a 224c 4250 6169 7273  ,"name":"LBPairs
+00015580: 4176 6169 6c61 626c 6522 2c22 7479 7065  Available","type
+00015590: 223a 2274 7570 6c65 5b5d 227d 5d2c 2273  ":"tuple[]"}],"s
+000155a0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+000155b0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
+000155c0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+000155d0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+000155e0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+000155f0: 4552 4332 3022 2c22 6e61 6d65 223a 225f  ERC20","name":"_
+00015600: 746f 6b65 6e41 222c 2274 7970 6522 3a22  tokenA","type":"
+00015610: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+00015620: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+00015630: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+00015640: 6522 3a22 5f74 6f6b 656e 4222 2c22 7479  e":"_tokenB","ty
+00015650: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+00015660: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00015670: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00015680: 225f 6269 6e53 7465 7022 2c22 7479 7065  "_binStep","type
+00015690: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+000156a0: 616d 6522 3a22 6765 744c 4250 6169 7249  ame":"getLBPairI
+000156b0: 6e66 6f72 6d61 7469 6f6e 222c 226f 7574  nformation","out
+000156c0: 7075 7473 223a 5b7b 2263 6f6d 706f 6e65  puts":[{"compone
+000156d0: 6e74 7322 3a5b 7b22 696e 7465 726e 616c  nts":[{"internal
+000156e0: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
+000156f0: 6e61 6d65 223a 2262 696e 5374 6570 222c  name":"binStep",
+00015700: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00015710: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00015720: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
+00015730: 6972 222c 226e 616d 6522 3a22 4c42 5061  ir","name":"LBPa
+00015740: 6972 222c 2274 7970 6522 3a22 6164 6472  ir","type":"addr
+00015750: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+00015760: 5479 7065 223a 2262 6f6f 6c22 2c22 6e61  Type":"bool","na
+00015770: 6d65 223a 2263 7265 6174 6564 4279 4f77  me":"createdByOw
+00015780: 6e65 7222 2c22 7479 7065 223a 2262 6f6f  ner","type":"boo
+00015790: 6c22 7d2c 7b22 696e 7465 726e 616c 5479  l"},{"internalTy
+000157a0: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
+000157b0: 223a 2269 676e 6f72 6564 466f 7252 6f75  ":"ignoredForRou
+000157c0: 7469 6e67 222c 2274 7970 6522 3a22 626f  ting","type":"bo
+000157d0: 6f6c 227d 5d2c 2269 6e74 6572 6e61 6c54  ol"}],"internalT
+000157e0: 7970 6522 3a22 7374 7275 6374 2049 4c42  ype":"struct ILB
+000157f0: 4661 6374 6f72 792e 4c42 5061 6972 496e  Factory.LBPairIn
+00015800: 666f 726d 6174 696f 6e22 2c22 6e61 6d65  formation","name
+00015810: 223a 2222 2c22 7479 7065 223a 2274 7570  ":"","type":"tup
+00015820: 6c65 227d 5d2c 2273 7461 7465 4d75 7461  le"}],"stateMuta
+00015830: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+00015840: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00015850: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00015860: 6e61 6d65 223a 2267 6574 4e75 6d62 6572  name":"getNumber
+00015870: 4f66 4c42 5061 6972 7322 2c22 6f75 7470  OfLBPairs","outp
+00015880: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00015890: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+000158a0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+000158b0: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
+000158c0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+000158d0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+000158e0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+000158f0: 7322 3a5b 5d2c 226e 616d 6522 3a22 6765  s":[],"name":"ge
+00015900: 744e 756d 6265 724f 6651 756f 7465 4173  tNumberOfQuoteAs
+00015910: 7365 7473 222c 226f 7574 7075 7473 223a  sets","outputs":
+00015920: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00015930: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00015940: 223a 2222 2c22 7479 7065 223a 2275 696e  ":"","type":"uin
+00015950: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
+00015960: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
+00015970: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00015980: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00015990: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000159a0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
+000159b0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+000159c0: 3a22 7569 6e74 3136 227d 5d2c 226e 616d  :"uint16"}],"nam
+000159d0: 6522 3a22 6765 7450 7265 7365 7422 2c22  e":"getPreset","
+000159e0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+000159f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00015a00: 3536 222c 226e 616d 6522 3a22 6261 7365  56","name":"base
+00015a10: 4661 6374 6f72 222c 2274 7970 6522 3a22  Factor","type":"
+00015a20: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00015a30: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00015a40: 3536 222c 226e 616d 6522 3a22 6669 6c74  56","name":"filt
+00015a50: 6572 5065 7269 6f64 222c 2274 7970 6522  erPeriod","type"
+00015a60: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00015a70: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00015a80: 7432 3536 222c 226e 616d 6522 3a22 6465  t256","name":"de
+00015a90: 6361 7950 6572 696f 6422 2c22 7479 7065  cayPeriod","type
+00015aa0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00015ab0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00015ac0: 6e74 3235 3622 2c22 6e61 6d65 223a 2272  nt256","name":"r
+00015ad0: 6564 7563 7469 6f6e 4661 6374 6f72 222c  eductionFactor",
+00015ae0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00015af0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00015b00: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00015b10: 6522 3a22 7661 7269 6162 6c65 4665 6543  e":"variableFeeC
+00015b20: 6f6e 7472 6f6c 222c 2274 7970 6522 3a22  ontrol","type":"
+00015b30: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00015b40: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00015b50: 3536 222c 226e 616d 6522 3a22 7072 6f74  56","name":"prot
+00015b60: 6f63 6f6c 5368 6172 6522 2c22 7479 7065  ocolShare","type
+00015b70: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00015b80: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00015b90: 6e74 3235 3622 2c22 6e61 6d65 223a 226d  nt256","name":"m
+00015ba0: 6178 566f 6c61 7469 6c69 7479 4163 6375  axVolatilityAccu
+00015bb0: 6d75 6c61 7465 6422 2c22 7479 7065 223a  mulated","type":
+00015bc0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00015bd0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00015be0: 3235 3622 2c22 6e61 6d65 223a 2273 616d  256","name":"sam
+00015bf0: 706c 654c 6966 6574 696d 6522 2c22 7479  pleLifetime","ty
+00015c00: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00015c10: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00015c20: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+00015c30: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00015c40: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00015c50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00015c60: 2c22 6e61 6d65 223a 225f 696e 6465 7822  ,"name":"_index"
+00015c70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00015c80: 227d 5d2c 226e 616d 6522 3a22 6765 7451  "}],"name":"getQ
+00015c90: 756f 7465 4173 7365 7422 2c22 6f75 7470  uoteAsset","outp
+00015ca0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00015cb0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00015cc0: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+00015cd0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00015ce0: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
+00015cf0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00015d00: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00015d10: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00015d20: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00015d30: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+00015d40: 616d 6522 3a22 5f74 6f6b 656e 222c 2274  ame":"_token","t
+00015d50: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+00015d60: 2c22 6e61 6d65 223a 2269 7351 756f 7465  ,"name":"isQuote
+00015d70: 4173 7365 7422 2c22 6f75 7470 7574 7322  Asset","outputs"
+00015d80: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00015d90: 223a 2262 6f6f 6c22 2c22 6e61 6d65 223a  ":"bool","name":
+00015da0: 2222 2c22 7479 7065 223a 2262 6f6f 6c22  "","type":"bool"
+00015db0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+00015dc0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+00015dd0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00015de0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00015df0: 6522 3a22 6f77 6e65 7222 2c22 6f75 7470  e":"owner","outp
+00015e00: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00015e10: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00015e20: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+00015e30: 3a22 6164 6472 6573 7322 7d5d 2c22 7374  :"address"}],"st
+00015e40: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00015e50: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+00015e60: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00015e70: 7322 3a5b 5d2c 226e 616d 6522 3a22 7065  s":[],"name":"pe
+00015e80: 6e64 696e 674f 776e 6572 222c 226f 7574  ndingOwner","out
+00015e90: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00015ea0: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+00015eb0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
+00015ec0: 223a 2261 6464 7265 7373 227d 5d2c 2273  ":"address"}],"s
+00015ed0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+00015ee0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
+00015ef0: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+00015f00: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00015f10: 7970 6522 3a22 7569 6e74 3136 222c 226e  ype":"uint16","n
+00015f20: 616d 6522 3a22 5f62 696e 5374 6570 222c  ame":"_binStep",
+00015f30: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00015f40: 5d2c 226e 616d 6522 3a22 7265 6d6f 7665  ],"name":"remove
+00015f50: 5072 6573 6574 222c 226f 7574 7075 7473  Preset","outputs
+00015f60: 223a 5b5d 2c22 7374 6174 654d 7574 6162  ":[],"stateMutab
+00015f70: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
+00015f80: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+00015f90: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+00015fa0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00015fb0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
+00015fc0: 3230 222c 226e 616d 6522 3a22 5f71 756f  20","name":"_quo
+00015fd0: 7465 4173 7365 7422 2c22 7479 7065 223a  teAsset","type":
+00015fe0: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
+00015ff0: 6522 3a22 7265 6d6f 7665 5175 6f74 6541  e":"removeQuoteA
+00016000: 7373 6574 222c 226f 7574 7075 7473 223a  sset","outputs":
+00016010: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+00016020: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+00016030: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00016040: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00016050: 5d2c 226e 616d 6522 3a22 7265 6e6f 756e  ],"name":"renoun
+00016060: 6365 4f77 6e65 7273 6869 7022 2c22 6f75  ceOwnership","ou
+00016070: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00016080: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00016090: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+000160a0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+000160b0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+000160c0: 2272 6576 6f6b 6550 656e 6469 6e67 4f77  "revokePendingOw
+000160d0: 6e65 7222 2c22 6f75 7470 7574 7322 3a5b  ner","outputs":[
+000160e0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+000160f0: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+00016100: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00016110: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00016120: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00016130: 626f 6f6c 222c 226e 616d 6522 3a22 5f6c  bool","name":"_l
+00016140: 6f63 6b65 6422 2c22 7479 7065 223a 2262  ocked","type":"b
+00016150: 6f6f 6c22 7d5d 2c22 6e61 6d65 223a 2273  ool"}],"name":"s
+00016160: 6574 4661 6374 6f72 794c 6f63 6b65 6453  etFactoryLockedS
+00016170: 7461 7465 222c 226f 7574 7075 7473 223a  tate","outputs":
+00016180: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+00016190: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+000161a0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+000161b0: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+000161c0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000161d0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+000161e0: 3a22 5f66 6565 5265 6369 7069 656e 7422  :"_feeRecipient"
+000161f0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00016200: 227d 5d2c 226e 616d 6522 3a22 7365 7446  "}],"name":"setF
+00016210: 6565 5265 6369 7069 656e 7422 2c22 6f75  eeRecipient","ou
+00016220: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00016230: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00016240: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+00016250: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00016260: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00016270: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+00016280: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
+00016290: 225f 746f 6b65 6e58 222c 2274 7970 6522  "_tokenX","type"
+000162a0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+000162b0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+000162c0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+000162d0: 616d 6522 3a22 5f74 6f6b 656e 5922 2c22  ame":"_tokenY","
+000162e0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+000162f0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00016300: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
+00016310: 3a22 5f62 696e 5374 6570 222c 2274 7970  :"_binStep","typ
+00016320: 6522 3a22 7569 6e74 3136 227d 2c7b 2269  e":"uint16"},{"i
+00016330: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00016340: 6e74 3136 222c 226e 616d 6522 3a22 5f62  nt16","name":"_b
+00016350: 6173 6546 6163 746f 7222 2c22 7479 7065  aseFactor","type
+00016360: 223a 2275 696e 7431 3622 7d2c 7b22 696e  ":"uint16"},{"in
+00016370: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00016380: 7431 3622 2c22 6e61 6d65 223a 225f 6669  t16","name":"_fi
+00016390: 6c74 6572 5065 7269 6f64 222c 2274 7970  lterPeriod","typ
+000163a0: 6522 3a22 7569 6e74 3136 227d 2c7b 2269  e":"uint16"},{"i
+000163b0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+000163c0: 6e74 3136 222c 226e 616d 6522 3a22 5f64  nt16","name":"_d
+000163d0: 6563 6179 5065 7269 6f64 222c 2274 7970  ecayPeriod","typ
+000163e0: 6522 3a22 7569 6e74 3136 227d 2c7b 2269  e":"uint16"},{"i
+000163f0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00016400: 6e74 3136 222c 226e 616d 6522 3a22 5f72  nt16","name":"_r
+00016410: 6564 7563 7469 6f6e 4661 6374 6f72 222c  eductionFactor",
+00016420: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00016430: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00016440: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
+00016450: 3a22 5f76 6172 6961 626c 6546 6565 436f  :"_variableFeeCo
+00016460: 6e74 726f 6c22 2c22 7479 7065 223a 2275  ntrol","type":"u
+00016470: 696e 7432 3422 7d2c 7b22 696e 7465 726e  int24"},{"intern
+00016480: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+00016490: 2c22 6e61 6d65 223a 225f 7072 6f74 6f63  ,"name":"_protoc
+000164a0: 6f6c 5368 6172 6522 2c22 7479 7065 223a  olShare","type":
+000164b0: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
+000164c0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+000164d0: 3422 2c22 6e61 6d65 223a 225f 6d61 7856  4","name":"_maxV
+000164e0: 6f6c 6174 696c 6974 7941 6363 756d 756c  olatilityAccumul
+000164f0: 6174 6564 222c 2274 7970 6522 3a22 7569  ated","type":"ui
+00016500: 6e74 3234 227d 5d2c 226e 616d 6522 3a22  nt24"}],"name":"
+00016510: 7365 7446 6565 7350 6172 616d 6574 6572  setFeesParameter
+00016520: 734f 6e50 6169 7222 2c22 6f75 7470 7574  sOnPair","output
+00016530: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
+00016540: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+00016550: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+00016560: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+00016570: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00016580: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00016590: 6d65 223a 225f 666c 6173 684c 6f61 6e46  me":"_flashLoanF
+000165a0: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
+000165b0: 3235 3622 7d5d 2c22 6e61 6d65 223a 2273  256"}],"name":"s
+000165c0: 6574 466c 6173 684c 6f61 6e46 6565 222c  etFlashLoanFee",
+000165d0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+000165e0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+000165f0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00016600: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00016610: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00016620: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+00016630: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+00016640: 6522 3a22 5f74 6f6b 656e 5822 2c22 7479  e":"_tokenX","ty
+00016650: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+00016660: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00016670: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
+00016680: 2c22 6e61 6d65 223a 225f 746f 6b65 6e59  ,"name":"_tokenY
+00016690: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000166a0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+000166b0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000166c0: 616d 6522 3a22 5f62 696e 5374 6570 222c  ame":"_binStep",
+000166d0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000166e0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000166f0: 223a 2262 6f6f 6c22 2c22 6e61 6d65 223a  ":"bool","name":
+00016700: 225f 6967 6e6f 7265 6422 2c22 7479 7065  "_ignored","type
+00016710: 223a 2262 6f6f 6c22 7d5d 2c22 6e61 6d65  ":"bool"}],"name
+00016720: 223a 2273 6574 4c42 5061 6972 4967 6e6f  ":"setLBPairIgno
+00016730: 7265 6422 2c22 6f75 7470 7574 7322 3a5b  red","outputs":[
+00016740: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00016750: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+00016760: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00016770: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00016780: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00016790: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+000167a0: 225f 4c42 5061 6972 496d 706c 656d 656e  "_LBPairImplemen
+000167b0: 7461 7469 6f6e 222c 2274 7970 6522 3a22  tation","type":"
+000167c0: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+000167d0: 223a 2273 6574 4c42 5061 6972 496d 706c  ":"setLBPairImpl
+000167e0: 656d 656e 7461 7469 6f6e 222c 226f 7574  ementation","out
+000167f0: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
+00016800: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+00016810: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+00016820: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00016830: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00016840: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00016850: 226e 616d 6522 3a22 7065 6e64 696e 674f  "name":"pendingO
+00016860: 776e 6572 5f22 2c22 7479 7065 223a 2261  wner_","type":"a
+00016870: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
+00016880: 3a22 7365 7450 656e 6469 6e67 4f77 6e65  :"setPendingOwne
+00016890: 7222 2c22 6f75 7470 7574 7322 3a5b 5d2c  r","outputs":[],
+000168a0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+000168b0: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+000168c0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+000168d0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+000168e0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+000168f0: 6e74 3136 222c 226e 616d 6522 3a22 5f62  nt16","name":"_b
+00016900: 696e 5374 6570 222c 2274 7970 6522 3a22  inStep","type":"
+00016910: 7569 6e74 3136 227d 2c7b 2269 6e74 6572  uint16"},{"inter
+00016920: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+00016930: 222c 226e 616d 6522 3a22 5f62 6173 6546  ","name":"_baseF
+00016940: 6163 746f 7222 2c22 7479 7065 223a 2275  actor","type":"u
+00016950: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
+00016960: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+00016970: 2c22 6e61 6d65 223a 225f 6669 6c74 6572  ,"name":"_filter
+00016980: 5065 7269 6f64 222c 2274 7970 6522 3a22  Period","type":"
+00016990: 7569 6e74 3136 227d 2c7b 2269 6e74 6572  uint16"},{"inter
+000169a0: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+000169b0: 222c 226e 616d 6522 3a22 5f64 6563 6179  ","name":"_decay
+000169c0: 5065 7269 6f64 222c 2274 7970 6522 3a22  Period","type":"
+000169d0: 7569 6e74 3136 227d 2c7b 2269 6e74 6572  uint16"},{"inter
+000169e0: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+000169f0: 222c 226e 616d 6522 3a22 5f72 6564 7563  ","name":"_reduc
+00016a00: 7469 6f6e 4661 6374 6f72 222c 2274 7970  tionFactor","typ
+00016a10: 6522 3a22 7569 6e74 3136 227d 2c7b 2269  e":"uint16"},{"i
+00016a20: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00016a30: 6e74 3234 222c 226e 616d 6522 3a22 5f76  nt24","name":"_v
+00016a40: 6172 6961 626c 6546 6565 436f 6e74 726f  ariableFeeContro
+00016a50: 6c22 2c22 7479 7065 223a 2275 696e 7432  l","type":"uint2
+00016a60: 3422 7d2c 7b22 696e 7465 726e 616c 5479  4"},{"internalTy
+00016a70: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
+00016a80: 6d65 223a 225f 7072 6f74 6f63 6f6c 5368  me":"_protocolSh
+00016a90: 6172 6522 2c22 7479 7065 223a 2275 696e  are","type":"uin
+00016aa0: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
+00016ab0: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
+00016ac0: 6e61 6d65 223a 225f 6d61 7856 6f6c 6174  name":"_maxVolat
+00016ad0: 696c 6974 7941 6363 756d 756c 6174 6564  ilityAccumulated
+00016ae0: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
+00016af0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00016b00: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
+00016b10: 6522 3a22 5f73 616d 706c 654c 6966 6574  e":"_sampleLifet
+00016b20: 696d 6522 2c22 7479 7065 223a 2275 696e  ime","type":"uin
+00016b30: 7431 3622 7d5d 2c22 6e61 6d65 223a 2273  t16"}],"name":"s
+00016b40: 6574 5072 6573 6574 222c 226f 7574 7075  etPreset","outpu
+00016b50: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
+00016b60: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+00016b70: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
+00016b80: 6e63 7469 6f6e 227d 5d27 290a 0a20 2020  nction"}]')..   
+00016b90: 2023 6a6f 6520 6661 636f 7472 790a 2020   #joe facotry.  
+00016ba0: 2020 6465 6620 6765 745f 6e75 6d62 6572    def get_number
+00016bb0: 5f6f 665f 6c62 5f70 6169 7273 285f 7765  _of_lb_pairs(_we
+00016bc0: 6233 3a57 6562 332c 5f66 6163 746f 7279  b3:Web3,_factory
+00016bd0: 5f61 6464 7265 7373 293a 0a20 2020 2020  _address):.     
+00016be0: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
+00016bf0: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+00016c00: 7265 7373 3d5f 6661 6374 6f72 795f 6164  ress=_factory_ad
+00016c10: 6472 6573 732c 2061 6269 3d4a 6f65 5632  dress, abi=JoeV2
+00016c20: 4661 6374 6f72 792e 6a6f 655f 6661 6374  Factory.joe_fact
+00016c30: 6f72 795f 7632 5f61 6269 292e 6675 6e63  ory_v2_abi).func
+00016c40: 7469 6f6e 732e 6765 744e 756d 6265 724f  tions.getNumberO
+00016c50: 664c 4250 6169 7273 2829 2e63 616c 6c28  fLBPairs().call(
+00016c60: 290a 0a20 2020 2064 6566 2067 6574 5f6e  )..    def get_n
+00016c70: 756d 6265 725f 6f66 5f71 756f 7465 5f61  umber_of_quote_a
+00016c80: 7373 6574 7328 5f77 6562 333a 5765 6233  ssets(_web3:Web3
+00016c90: 2c5f 6661 6374 6f72 795f 6164 6472 6573  ,_factory_addres
+00016ca0: 7329 3a0a 2020 2020 2020 2020 7265 7475  s):.        retu
+00016cb0: 726e 205f 7765 6233 2e65 7468 2e63 6f6e  rn _web3.eth.con
+00016cc0: 7472 6163 7428 6164 6472 6573 733d 5f66  tract(address=_f
+00016cd0: 6163 746f 7279 5f61 6464 7265 7373 2c20  actory_address, 
+00016ce0: 6162 693d 4a6f 6556 3246 6163 746f 7279  abi=JoeV2Factory
+00016cf0: 2e6a 6f65 5f66 6163 746f 7279 5f76 325f  .joe_factory_v2_
+00016d00: 6162 6929 2e66 756e 6374 696f 6e73 2e67  abi).functions.g
+00016d10: 6574 4e75 6d62 6572 4f66 5175 6f74 6541  etNumberOfQuoteA
+00016d20: 7373 6574 7328 292e 6361 6c6c 2829 0a0a  ssets().call()..
+00016d30: 2020 2020 6465 6620 6765 745f 7175 6f74      def get_quot
+00016d40: 655f 6173 7365 7428 5f77 6562 333a 5765  e_asset(_web3:We
+00016d50: 6233 2c5f 6661 6374 6f72 795f 6164 6472  b3,_factory_addr
+00016d60: 6573 732c 5f69 6e64 6578 293a 0a20 2020  ess,_index):.   
+00016d70: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
+00016d80: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
+00016d90: 6464 7265 7373 3d5f 6661 6374 6f72 795f  ddress=_factory_
+00016da0: 6164 6472 6573 732c 2061 6269 3d4a 6f65  address, abi=Joe
+00016db0: 5632 4661 6374 6f72 792e 6a6f 655f 6661  V2Factory.joe_fa
+00016dc0: 6374 6f72 795f 7632 5f61 6269 292e 6675  ctory_v2_abi).fu
+00016dd0: 6e63 7469 6f6e 732e 6765 7451 756f 7465  nctions.getQuote
+00016de0: 4173 7365 7428 5f69 6e64 6578 292e 6361  Asset(_index).ca
+00016df0: 6c6c 2829 0a0a 2020 2020 6465 6620 6973  ll()..    def is
+00016e00: 5f71 756f 7465 5f61 7373 6574 285f 7765  _quote_asset(_we
+00016e10: 6233 3a57 6562 332c 5f66 6163 746f 7279  b3:Web3,_factory
+00016e20: 5f61 6464 7265 7373 2c5f 6164 6472 6573  _address,_addres
+00016e30: 733a 7374 7229 3a0a 2020 2020 2020 2020  s:str):.        
+00016e40: 7265 7475 726e 205f 7765 6233 2e65 7468  return _web3.eth
+00016e50: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
+00016e60: 733d 5f66 6163 746f 7279 5f61 6464 7265  s=_factory_addre
+00016e70: 7373 2c20 6162 693d 4a6f 6556 3246 6163  ss, abi=JoeV2Fac
+00016e80: 746f 7279 2e6a 6f65 5f66 6163 746f 7279  tory.joe_factory
+00016e90: 5f76 325f 6162 6929 2e66 756e 6374 696f  _v2_abi).functio
+00016ea0: 6e73 2e69 7351 756f 7465 4173 7365 7428  ns.isQuoteAsset(
+00016eb0: 5f61 6464 7265 7373 292e 6361 6c6c 2829  _address).call()
+00016ec0: 0a0a 2020 2020 6465 6620 6765 745f 7061  ..    def get_pa
+00016ed0: 6972 5f69 6e66 6f72 6d61 7469 6f6e 285f  ir_information(_
+00016ee0: 7765 6233 3a57 6562 332c 5f66 6163 746f  web3:Web3,_facto
+00016ef0: 7279 5f61 6464 7265 7373 2c5f 746f 6b65  ry_address,_toke
+00016f00: 6e5f 613a 7374 722c 5f74 6f6b 656e 5f62  n_a:str,_token_b
+00016f10: 3a73 7472 2c5f 6269 6e5f 7374 6570 293a  :str,_bin_step):
+00016f20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016f30: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
+00016f40: 6374 2861 6464 7265 7373 3d5f 6661 6374  ct(address=_fact
+00016f50: 6f72 795f 6164 6472 6573 732c 2061 6269  ory_address, abi
+00016f60: 3d4a 6f65 5632 4661 6374 6f72 792e 6a6f  =JoeV2Factory.jo
+00016f70: 655f 6661 6374 6f72 795f 7632 5f61 6269  e_factory_v2_abi
+00016f80: 292e 6675 6e63 7469 6f6e 732e 6765 744c  ).functions.getL
+00016f90: 4250 6169 7249 6e66 6f72 6d61 7469 6f6e  BPairInformation
+00016fa0: 285f 746f 6b65 6e5f 612c 5f74 6f6b 656e  (_token_a,_token
+00016fb0: 5f62 2c5f 6269 6e5f 7374 6570 292e 6361  _b,_bin_step).ca
+00016fc0: 6c6c 2829 0a0a 2020 2020 6465 6620 6765  ll()..    def ge
+00016fd0: 745f 616c 6c5f 6c62 5f70 6169 7273 285f  t_all_lb_pairs(_
+00016fe0: 7765 6233 3a57 6562 332c 5f66 6163 746f  web3:Web3,_facto
+00016ff0: 7279 5f61 6464 7265 7373 2c5f 746f 6b65  ry_address,_toke
+00017000: 6e5f 613a 7374 722c 5f74 6f6b 656e 5f62  n_a:str,_token_b
+00017010: 3a73 7472 293a 0a20 2020 2020 2020 2072  :str):.        r
+00017020: 6574 7572 6e20 5f77 6562 332e 6574 682e  eturn _web3.eth.
+00017030: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
+00017040: 3d5f 6661 6374 6f72 795f 6164 6472 6573  =_factory_addres
+00017050: 732c 2061 6269 3d4a 6f65 5632 4661 6374  s, abi=JoeV2Fact
+00017060: 6f72 792e 6a6f 655f 6661 6374 6f72 795f  ory.joe_factory_
+00017070: 7632 5f61 6269 292e 6675 6e63 7469 6f6e  v2_abi).function
+00017080: 732e 6765 7441 6c6c 4c42 5061 6972 7328  s.getAllLBPairs(
+00017090: 5f74 6f6b 656e 5f61 2c5f 746f 6b65 6e5f  _token_a,_token_
+000170a0: 6229 2e63 616c 6c28 290a 0a20 2020 2064  b).call()..    d
+000170b0: 6566 2067 6574 5f61 6c6c 5f62 696e 5f73  ef get_all_bin_s
+000170c0: 7465 7073 285f 7765 6233 3a57 6562 332c  teps(_web3:Web3,
+000170d0: 5f66 6163 746f 7279 5f61 6464 7265 7373  _factory_address
+000170e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000170f0: 6e20 5f77 6562 332e 6574 682e 636f 6e74  n _web3.eth.cont
+00017100: 7261 6374 2861 6464 7265 7373 3d5f 6661  ract(address=_fa
+00017110: 6374 6f72 795f 6164 6472 6573 732c 2061  ctory_address, a
+00017120: 6269 3d4a 6f65 5632 4661 6374 6f72 792e  bi=JoeV2Factory.
+00017130: 6a6f 655f 6661 6374 6f72 795f 7632 5f61  joe_factory_v2_a
+00017140: 6269 292e 6675 6e63 7469 6f6e 732e 6765  bi).functions.ge
+00017150: 7441 6c6c 4269 6e53 7465 7073 2829 2e63  tAllBinSteps().c
+00017160: 616c 6c28 290a 0a63 6c61 7373 204a 6f65  all()..class Joe
+00017170: 5632 5175 6f74 653a 0a20 2020 206a 6f65  V2Quote:.    joe
+00017180: 5f71 756f 7465 5f76 325f 6162 693d 275b  _quote_v2_abi='[
+00017190: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+000171a0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+000171b0: 6573 7322 2c22 6e61 6d65 223a 225f 726f  ess","name":"_ro
+000171c0: 7574 6572 5632 222c 2274 7970 6522 3a22  uterV2","type":"
+000171d0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+000171e0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+000171f0: 7373 222c 226e 616d 6522 3a22 5f66 6163  ss","name":"_fac
+00017200: 746f 7279 5631 222c 2274 7970 6522 3a22  toryV1","type":"
+00017210: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+00017220: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00017230: 7373 222c 226e 616d 6522 3a22 5f66 6163  ss","name":"_fac
+00017240: 746f 7279 5632 222c 2274 7970 6522 3a22  toryV2","type":"
+00017250: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
+00017260: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
+00017270: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
+00017280: 3a22 636f 6e73 7472 7563 746f 7222 7d2c  :"constructor"},
+00017290: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+000172a0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000172b0: 3235 3622 2c22 6e61 6d65 223a 2262 7022  256","name":"bp"
+000172c0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+000172d0: 227d 5d2c 226e 616d 6522 3a22 4269 6e48  "}],"name":"BinH
+000172e0: 656c 7065 725f 5f42 696e 5374 6570 4f76  elper__BinStepOv
+000172f0: 6572 666c 6f77 7322 2c22 7479 7065 223a  erflows","type":
+00017300: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00017310: 7322 3a5b 5d2c 226e 616d 6522 3a22 4269  s":[],"name":"Bi
+00017320: 6e48 656c 7065 725f 5f49 644f 7665 7266  nHelper__IdOverf
+00017330: 6c6f 7773 222c 2274 7970 6522 3a22 6572  lows","type":"er
+00017340: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+00017350: 5b5d 2c22 6e61 6d65 223a 224a 6f65 4c69  [],"name":"JoeLi
+00017360: 6272 6172 795f 5f41 6464 7265 7373 5a65  brary__AddressZe
+00017370: 726f 222c 2274 7970 6522 3a22 6572 726f  ro","type":"erro
+00017380: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
+00017390: 2c22 6e61 6d65 223a 224a 6f65 4c69 6272  ,"name":"JoeLibr
+000173a0: 6172 795f 5f49 6465 6e74 6963 616c 4164  ary__IdenticalAd
+000173b0: 6472 6573 7365 7322 2c22 7479 7065 223a  dresses","type":
+000173c0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+000173d0: 7322 3a5b 5d2c 226e 616d 6522 3a22 4a6f  s":[],"name":"Jo
+000173e0: 654c 6962 7261 7279 5f5f 496e 7375 6666  eLibrary__Insuff
+000173f0: 6963 6965 6e74 416d 6f75 6e74 222c 2274  icientAmount","t
+00017400: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00017410: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00017420: 223a 224a 6f65 4c69 6272 6172 795f 5f49  ":"JoeLibrary__I
+00017430: 6e73 7566 6669 6369 656e 744c 6971 7569  nsufficientLiqui
+00017440: 6469 7479 222c 2274 7970 6522 3a22 6572  dity","type":"er
+00017450: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+00017460: 5b5d 2c22 6e61 6d65 223a 224c 4251 756f  [],"name":"LBQuo
+00017470: 7465 725f 496e 7661 6c69 644c 656e 6774  ter_InvalidLengt
+00017480: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
+00017490: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+000174a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000174b0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000174c0: 7822 2c22 7479 7065 223a 2275 696e 7432  x","type":"uint2
+000174d0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+000174e0: 7970 6522 3a22 696e 7432 3536 222c 226e  ype":"int256","n
+000174f0: 616d 6522 3a22 7922 2c22 7479 7065 223a  ame":"y","type":
+00017500: 2269 6e74 3235 3622 7d5d 2c22 6e61 6d65  "int256"}],"name
+00017510: 223a 224d 6174 6831 3238 7831 3238 5f5f  ":"Math128x128__
+00017520: 506f 7765 7255 6e64 6572 666c 6f77 222c  PowerUnderflow",
+00017530: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00017540: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00017550: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00017560: 3235 3622 2c22 6e61 6d65 223a 2270 726f  256","name":"pro
+00017570: 6431 222c 2274 7970 6522 3a22 7569 6e74  d1","type":"uint
+00017580: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+00017590: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+000175a0: 226e 616d 6522 3a22 6465 6e6f 6d69 6e61  "name":"denomina
+000175b0: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
+000175c0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+000175d0: 4d61 7468 3531 3242 6974 735f 5f4d 756c  Math512Bits__Mul
+000175e0: 4469 764f 7665 7266 6c6f 7722 2c22 7479  DivOverflow","ty
+000175f0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+00017600: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00017610: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00017620: 222c 226e 616d 6522 3a22 7072 6f64 3122  ","name":"prod1"
+00017630: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00017640: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00017650: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00017660: 6d65 223a 226f 6666 7365 7422 2c22 7479  me":"offset","ty
+00017670: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00017680: 226e 616d 6522 3a22 4d61 7468 3531 3242  "name":"Math512B
+00017690: 6974 735f 5f4d 756c 5368 6966 744f 7665  its__MulShiftOve
+000176a0: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
+000176b0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+000176c0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+000176d0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+000176e0: 6522 3a22 6f66 6673 6574 222c 2274 7970  e":"offset","typ
+000176f0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00017700: 6e61 6d65 223a 224d 6174 6835 3132 4269  name":"Math512Bi
+00017710: 7473 5f5f 4f66 6673 6574 4f76 6572 666c  ts__OffsetOverfl
+00017720: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
+00017730: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00017740: 5d2c 226e 616d 6522 3a22 6661 6374 6f72  ],"name":"factor
+00017750: 7956 3122 2c22 6f75 7470 7574 7322 3a5b  yV1","outputs":[
+00017760: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00017770: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00017780: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+00017790: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+000177a0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+000177b0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+000177c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+000177d0: 226e 616d 6522 3a22 6661 6374 6f72 7956  "name":"factoryV
+000177e0: 3222 2c22 6f75 7470 7574 7322 3a5b 7b22  2","outputs":[{"
+000177f0: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00017800: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+00017810: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00017820: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
+00017830: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00017840: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00017850: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00017860: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00017870: 7265 7373 5b5d 222c 226e 616d 6522 3a22  ress[]","name":"
+00017880: 5f72 6f75 7465 222c 2274 7970 6522 3a22  _route","type":"
+00017890: 6164 6472 6573 735b 5d22 7d2c 7b22 696e  address[]"},{"in
+000178a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+000178b0: 7432 3536 222c 226e 616d 6522 3a22 5f61  t256","name":"_a
+000178c0: 6d6f 756e 7449 6e22 2c22 7479 7065 223a  mountIn","type":
+000178d0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+000178e0: 6522 3a22 6669 6e64 4265 7374 5061 7468  e":"findBestPath
+000178f0: 4672 6f6d 416d 6f75 6e74 496e 222c 226f  FromAmountIn","o
+00017900: 7574 7075 7473 223a 5b7b 2263 6f6d 706f  utputs":[{"compo
+00017910: 6e65 6e74 7322 3a5b 7b22 696e 7465 726e  nents":[{"intern
+00017920: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00017930: 5b5d 222c 226e 616d 6522 3a22 726f 7574  []","name":"rout
+00017940: 6522 2c22 7479 7065 223a 2261 6464 7265  e","type":"addre
+00017950: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
+00017960: 6c54 7970 6522 3a22 6164 6472 6573 735b  lType":"address[
+00017970: 5d22 2c22 6e61 6d65 223a 2270 6169 7273  ]","name":"pairs
+00017980: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00017990: 735b 5d22 7d2c 7b22 696e 7465 726e 616c  s[]"},{"internal
+000179a0: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
+000179b0: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
+000179c0: 7073 222c 2274 7970 6522 3a22 7569 6e74  ps","type":"uint
+000179d0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+000179e0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000179f0: 5b5d 222c 226e 616d 6522 3a22 616d 6f75  []","name":"amou
+00017a00: 6e74 7322 2c22 7479 7065 223a 2275 696e  nts","type":"uin
+00017a10: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+00017a20: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00017a30: 365b 5d22 2c22 6e61 6d65 223a 2276 6972  6[]","name":"vir
+00017a40: 7475 616c 416d 6f75 6e74 7357 6974 686f  tualAmountsWitho
+00017a50: 7574 536c 6970 7061 6765 222c 2274 7970  utSlippage","typ
+00017a60: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+00017a70: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00017a80: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+00017a90: 6522 3a22 6665 6573 222c 2274 7970 6522  e":"fees","type"
+00017aa0: 3a22 7569 6e74 3235 365b 5d22 7d5d 2c22  :"uint256[]"}],"
+00017ab0: 696e 7465 726e 616c 5479 7065 223a 2273  internalType":"s
+00017ac0: 7472 7563 7420 4c42 5175 6f74 6572 2e51  truct LBQuoter.Q
+00017ad0: 756f 7465 222c 226e 616d 6522 3a22 7175  uote","name":"qu
+00017ae0: 6f74 6522 2c22 7479 7065 223a 2274 7570  ote","type":"tup
+00017af0: 6c65 227d 5d2c 2273 7461 7465 4d75 7461  le"}],"stateMuta
+00017b00: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+00017b10: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00017b20: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00017b30: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+00017b40: 6472 6573 735b 5d22 2c22 6e61 6d65 223a  dress[]","name":
+00017b50: 225f 726f 7574 6522 2c22 7479 7065 223a  "_route","type":
+00017b60: 2261 6464 7265 7373 5b5d 227d 2c7b 2269  "address[]"},{"i
+00017b70: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00017b80: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+00017b90: 616d 6f75 6e74 4f75 7422 2c22 7479 7065  amountOut","type
+00017ba0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00017bb0: 616d 6522 3a22 6669 6e64 4265 7374 5061  ame":"findBestPa
+00017bc0: 7468 4672 6f6d 416d 6f75 6e74 4f75 7422  thFromAmountOut"
+00017bd0: 2c22 6f75 7470 7574 7322 3a5b 7b22 636f  ,"outputs":[{"co
+00017be0: 6d70 6f6e 656e 7473 223a 5b7b 2269 6e74  mponents":[{"int
+00017bf0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+00017c00: 6573 735b 5d22 2c22 6e61 6d65 223a 2272  ess[]","name":"r
+00017c10: 6f75 7465 222c 2274 7970 6522 3a22 6164  oute","type":"ad
+00017c20: 6472 6573 735b 5d22 7d2c 7b22 696e 7465  dress[]"},{"inte
+00017c30: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00017c40: 7373 5b5d 222c 226e 616d 6522 3a22 7061  ss[]","name":"pa
+00017c50: 6972 7322 2c22 7479 7065 223a 2261 6464  irs","type":"add
+00017c60: 7265 7373 5b5d 227d 2c7b 2269 6e74 6572  ress[]"},{"inter
+00017c70: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00017c80: 365b 5d22 2c22 6e61 6d65 223a 2262 696e  6[]","name":"bin
+00017c90: 5374 6570 7322 2c22 7479 7065 223a 2275  Steps","type":"u
+00017ca0: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
+00017cb0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00017cc0: 3235 365b 5d22 2c22 6e61 6d65 223a 2261  256[]","name":"a
+00017cd0: 6d6f 756e 7473 222c 2274 7970 6522 3a22  mounts","type":"
+00017ce0: 7569 6e74 3235 365b 5d22 7d2c 7b22 696e  uint256[]"},{"in
+00017cf0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00017d00: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+00017d10: 7669 7274 7561 6c41 6d6f 756e 7473 5769  virtualAmountsWi
+00017d20: 7468 6f75 7453 6c69 7070 6167 6522 2c22  thoutSlippage","
+00017d30: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+00017d40: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00017d50: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+00017d60: 6e61 6d65 223a 2266 6565 7322 2c22 7479  name":"fees","ty
+00017d70: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
+00017d80: 5d2c 2269 6e74 6572 6e61 6c54 7970 6522  ],"internalType"
+00017d90: 3a22 7374 7275 6374 204c 4251 756f 7465  :"struct LBQuote
+00017da0: 722e 5175 6f74 6522 2c22 6e61 6d65 223a  r.Quote","name":
+00017db0: 2271 756f 7465 222c 2274 7970 6522 3a22  "quote","type":"
+00017dc0: 7475 706c 6522 7d5d 2c22 7374 6174 654d  tuple"}],"stateM
+00017dd0: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+00017de0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00017df0: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00017e00: 5d2c 226e 616d 6522 3a22 726f 7574 6572  ],"name":"router
+00017e10: 5632 222c 226f 7574 7075 7473 223a 5b7b  V2","outputs":[{
+00017e20: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00017e30: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+00017e40: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
+00017e50: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
+00017e60: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+00017e70: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00017e80: 7d5d 270a 0a20 2020 2023 7265 7475 726e  }]'..    #return
+00017e90: 2071 756f 7465 0a20 2020 2023 2020 2020   quote.    #    
+00017ea0: 7374 7275 6374 2051 756f 7465 207b 0a20  struct Quote {. 
+00017eb0: 2020 2023 2020 2020 2061 6464 7265 7373     #     address
+00017ec0: 5b5d 2072 6f75 7465 3b20 696e 2074 6f6b  [] route; in tok
+00017ed0: 656e 20e5 9ca8 e589 8d0a 2020 2020 2320  en .......    # 
+00017ee0: 2020 2020 6164 6472 6573 735b 5d20 7061      address[] pa
+00017ef0: 6972 733b 0a20 2020 2023 2020 2020 2075  irs;.    #     u
+00017f00: 696e 7432 3536 5b5d 2062 696e 5374 6570  int256[] binStep
+00017f10: 733b 0a20 2020 2023 2020 2020 2075 696e  s;.    #     uin
+00017f20: 7432 3536 5b5d 2061 6d6f 756e 7473 3b20  t256[] amounts; 
+00017f30: e695 b0e7 bb84 2ce9 a1ba e5ba 8fe4 b88e  ......,.........
+00017f40: e8b7 afe5 be84 e4b8 80e8 87b4 0a20 2020  .............   
+00017f50: 2023 2020 2020 2075 696e 7432 3536 5b5d   #     uint256[]
+00017f60: 2076 6972 7475 616c 416d 6f75 6e74 7357   virtualAmountsW
+00017f70: 6974 686f 7574 536c 6970 7061 6765 3b0a  ithoutSlippage;.
+00017f80: 2020 2020 2320 2020 2020 7569 6e74 3235      #     uint25
+00017f90: 365b 5d20 6665 6573 3b0a 2020 2020 2320  6[] fees;.    # 
+00017fa0: 7d0a 2020 2020 6465 6620 6669 6e64 5f62  }.    def find_b
+00017fb0: 6573 745f 7061 7468 5f66 6f72 5f61 6d6f  est_path_for_amo
+00017fc0: 756e 745f 696e 285f 7765 6233 3a57 6562  unt_in(_web3:Web
+00017fd0: 332c 5f71 756f 7465 5f61 6464 7265 7373  3,_quote_address
+00017fe0: 2c5f 7175 6f74 655f 6162 692c 5f70 6174  ,_quote_abi,_pat
+00017ff0: 682c 5f61 6d6f 756e 745f 696e 293a 0a20  h,_amount_in):. 
+00018000: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
+00018010: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
+00018020: 2861 6464 7265 7373 3d5f 7175 6f74 655f  (address=_quote_
+00018030: 6164 6472 6573 732c 6162 693d 5f71 756f  address,abi=_quo
+00018040: 7465 5f61 6269 292e 6675 6e63 7469 6f6e  te_abi).function
+00018050: 732e 6669 6e64 4265 7374 5061 7468 4672  s.findBestPathFr
+00018060: 6f6d 416d 6f75 6e74 496e 285f 7061 7468  omAmountIn(_path
+00018070: 2c5f 616d 6f75 6e74 5f69 6e29 2e63 616c  ,_amount_in).cal
+00018080: 6c28 290a 2020 2020 2372 6574 7572 6e20  l().    #return 
+00018090: 7175 6f74 650a 2020 2020 2320 2020 2073  quote.    #    s
+000180a0: 7472 7563 7420 5175 6f74 6520 7b0a 2020  truct Quote {.  
+000180b0: 2020 2320 2020 2020 6164 6472 6573 735b    #     address[
+000180c0: 5d20 726f 7574 653b 206f 7574 2074 6f6b  ] route; out tok
+000180d0: 656e e59c a8e5 898d 0a20 2020 2023 2020  en.......    #  
+000180e0: 2020 2061 6464 7265 7373 5b5d 2070 6169     address[] pai
+000180f0: 7273 3b0a 2020 2020 2320 2020 2020 7569  rs;.    #     ui
+00018100: 6e74 3235 365b 5d20 6269 6e53 7465 7073  nt256[] binSteps
+00018110: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
+00018120: 3235 365b 5d20 616d 6f75 6e74 733b 0a20  256[] amounts;. 
+00018130: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
+00018140: 5b5d 2076 6972 7475 616c 416d 6f75 6e74  [] virtualAmount
+00018150: 7357 6974 686f 7574 536c 6970 7061 6765  sWithoutSlippage
+00018160: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
+00018170: 3235 365b 5d20 6665 6573 3b0a 2020 2020  256[] fees;.    
+00018180: 2320 7d0a 2020 2020 6465 6620 6669 6e64  # }.    def find
+00018190: 5f62 6573 745f 7061 7468 5f66 6f72 5f61  _best_path_for_a
+000181a0: 6d6f 756e 745f 6f75 7428 5f77 6562 333a  mount_out(_web3:
+000181b0: 5765 6233 2c5f 7175 6f74 655f 6164 6472  Web3,_quote_addr
+000181c0: 6573 732c 5f71 756f 7465 5f61 6269 2c5f  ess,_quote_abi,_
+000181d0: 7061 7468 2c5f 616d 6f75 6e74 5f6f 7574  path,_amount_out
+000181e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000181f0: 6e20 5f77 6562 332e 6574 682e 636f 6e74  n _web3.eth.cont
+00018200: 7261 6374 2861 6464 7265 7373 3d5f 7175  ract(address=_qu
+00018210: 6f74 655f 6164 6472 6573 732c 6162 693d  ote_address,abi=
+00018220: 5f71 756f 7465 5f61 6269 292e 6675 6e63  _quote_abi).func
+00018230: 7469 6f6e 732e 6669 6e64 4265 7374 5061  tions.findBestPa
+00018240: 7468 4672 6f6d 416d 6f75 6e74 496e 285f  thFromAmountIn(_
+00018250: 7061 7468 2c5f 616d 6f75 6e74 5f6f 7574  path,_amount_out
+00018260: 292e 6361 6c6c 2829 0a0a 0a63 6c61 7373  ).call()...class
+00018270: 204a 6f65 5632 4572 6332 303a 0a20 2020   JoeV2Erc20:.   
+00018280: 206a 6f65 5f65 7263 3230 5f61 6269 3d27   joe_erc20_abi='
+00018290: 5b20 7b20 2261 6e6f 6e79 6d6f 7573 223a  [ { "anonymous":
+000182a0: 2066 616c 7365 2c20 2269 6e70 7574 7322   false, "inputs"
+000182b0: 3a20 5b20 7b20 2269 6e64 6578 6564 223a  : [ { "indexed":
+000182c0: 2074 7275 652c 2022 696e 7465 726e 616c   true, "internal
+000182d0: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
+000182e0: 2c20 226e 616d 6522 3a20 226f 776e 6572  , "name": "owner
+000182f0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+00018300: 6573 7322 207d 2c20 7b20 2269 6e64 6578  ess" }, { "index
+00018310: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
+00018320: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+00018330: 6573 7322 2c20 226e 616d 6522 3a20 2273  ess", "name": "s
+00018340: 7065 6e64 6572 222c 2022 7479 7065 223a  pender", "type":
+00018350: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
+00018360: 2269 6e64 6578 6564 223a 2066 616c 7365  "indexed": false
+00018370: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
+00018380: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+00018390: 6d65 223a 2022 7661 6c75 6522 2c20 2274  me": "value", "t
+000183a0: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
+000183b0: 7d20 5d2c 2022 6e61 6d65 223a 2022 4170  } ], "name": "Ap
+000183c0: 7072 6f76 616c 222c 2022 7479 7065 223a  proval", "type":
+000183d0: 2022 6576 656e 7422 207d 2c20 7b20 2261   "event" }, { "a
+000183e0: 6e6f 6e79 6d6f 7573 223a 2066 616c 7365  nonymous": false
+000183f0: 2c20 2269 6e70 7574 7322 3a20 5b20 7b20  , "inputs": [ { 
+00018400: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
+00018410: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+00018420: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+00018430: 6522 3a20 2266 726f 6d22 2c20 2274 7970  e": "from", "typ
+00018440: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
+00018450: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
+00018460: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
+00018470: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+00018480: 6e61 6d65 223a 2022 746f 222c 2022 7479  name": "to", "ty
+00018490: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+000184a0: 2c20 7b20 2269 6e64 6578 6564 223a 2066  , { "indexed": f
+000184b0: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
+000184c0: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+000184d0: 2022 6e61 6d65 223a 2022 7661 6c75 6522   "name": "value"
+000184e0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+000184f0: 3536 2220 7d20 5d2c 2022 6e61 6d65 223a  56" } ], "name":
+00018500: 2022 5472 616e 7366 6572 222c 2022 7479   "Transfer", "ty
+00018510: 7065 223a 2022 6576 656e 7422 207d 2c20  pe": "event" }, 
+00018520: 7b20 2269 6e70 7574 7322 3a20 5b20 7b20  { "inputs": [ { 
+00018530: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+00018540: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
+00018550: 223a 2022 6f77 6e65 7222 2c20 2274 7970  ": "owner", "typ
+00018560: 6522 3a20 2261 6464 7265 7373 2220 7d2c  e": "address" },
+00018570: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+00018580: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
+00018590: 616d 6522 3a20 2273 7065 6e64 6572 222c  ame": "spender",
+000185a0: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+000185b0: 7322 207d 205d 2c20 226e 616d 6522 3a20  s" } ], "name": 
+000185c0: 2261 6c6c 6f77 616e 6365 222c 2022 6f75  "allowance", "ou
+000185d0: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+000185e0: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+000185f0: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+00018600: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+00018610: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
+00018620: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
+00018630: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
+00018640: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+00018650: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+00018660: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+00018670: 6573 7322 2c20 226e 616d 6522 3a20 2273  ess", "name": "s
+00018680: 7065 6e64 6572 222c 2022 7479 7065 223a  pender", "type":
+00018690: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
+000186a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+000186b0: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+000186c0: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
+000186d0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+000186e0: 5d2c 2022 6e61 6d65 223a 2022 6170 7072  ], "name": "appr
+000186f0: 6f76 6522 2c20 226f 7574 7075 7473 223a  ove", "outputs":
+00018700: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+00018710: 7065 223a 2022 626f 6f6c 222c 2022 6e61  pe": "bool", "na
+00018720: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+00018730: 2022 626f 6f6c 2220 7d20 5d2c 2022 7374   "bool" } ], "st
+00018740: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+00018750: 226e 6f6e 7061 7961 626c 6522 2c20 2274  "nonpayable", "t
+00018760: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+00018770: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+00018780: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+00018790: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+000187a0: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
+000187b0: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+000187c0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+000187d0: 6261 6c61 6e63 654f 6622 2c20 226f 7574  balanceOf", "out
+000187e0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+000187f0: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+00018800: 3235 3622 2c20 226e 616d 6522 3a20 2222  256", "name": ""
+00018810: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+00018820: 3536 2220 7d20 5d2c 2022 7374 6174 654d  56" } ], "stateM
+00018830: 7574 6162 696c 6974 7922 3a20 2276 6965  utability": "vie
+00018840: 7722 2c20 2274 7970 6522 3a20 2266 756e  w", "type": "fun
+00018850: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+00018860: 7574 7322 3a20 5b5d 2c20 226e 616d 6522  uts": [], "name"
+00018870: 3a20 2264 6563 696d 616c 7322 2c20 226f  : "decimals", "o
+00018880: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
+00018890: 7465 726e 616c 5479 7065 223a 2022 7569  ternalType": "ui
+000188a0: 6e74 3822 2c20 226e 616d 6522 3a20 2222  nt8", "name": ""
+000188b0: 2c20 2274 7970 6522 3a20 2275 696e 7438  , "type": "uint8
+000188c0: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+000188d0: 6162 696c 6974 7922 3a20 2276 6965 7722  ability": "view"
+000188e0: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+000188f0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+00018900: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
+00018910: 226e 616d 6522 2c20 226f 7574 7075 7473  "name", "outputs
+00018920: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+00018930: 5479 7065 223a 2022 7374 7269 6e67 222c  Type": "string",
+00018940: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+00018950: 7065 223a 2022 7374 7269 6e67 2220 7d20  pe": "string" } 
+00018960: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+00018970: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
+00018980: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+00018990: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+000189a0: 5b5d 2c20 226e 616d 6522 3a20 2273 796d  [], "name": "sym
+000189b0: 626f 6c22 2c20 226f 7574 7075 7473 223a  bol", "outputs":
+000189c0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+000189d0: 7065 223a 2022 7374 7269 6e67 222c 2022  pe": "string", "
+000189e0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+000189f0: 223a 2022 7374 7269 6e67 2220 7d20 5d2c  ": "string" } ],
+00018a00: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+00018a10: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
+00018a20: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
+00018a30: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+00018a40: 2c20 226e 616d 6522 3a20 2274 6f74 616c  , "name": "total
+00018a50: 5375 7070 6c79 222c 2022 6f75 7470 7574  Supply", "output
+00018a60: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+00018a70: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+00018a80: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+00018a90: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+00018aa0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
+00018ab0: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
+00018ac0: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
+00018ad0: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
+00018ae0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+00018af0: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
+00018b00: 2c20 226e 616d 6522 3a20 2274 6f22 2c20  , "name": "to", 
+00018b10: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+00018b20: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
+00018b30: 5479 7065 223a 2022 7569 6e74 3235 3622  Type": "uint256"
+00018b40: 2c20 226e 616d 6522 3a20 2276 616c 7565  , "name": "value
+00018b50: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+00018b60: 3235 3622 207d 205d 2c20 226e 616d 6522  256" } ], "name"
+00018b70: 3a20 2274 7261 6e73 6665 7222 2c20 226f  : "transfer", "o
+00018b80: 7574 7075 7473 223a 205b 207b 2022 696e  utputs": [ { "in
+00018b90: 7465 726e 616c 5479 7065 223a 2022 626f  ternalType": "bo
+00018ba0: 6f6c 222c 2022 6e61 6d65 223a 2022 222c  ol", "name": "",
+00018bb0: 2022 7479 7065 223a 2022 626f 6f6c 2220   "type": "bool" 
+00018bc0: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
+00018bd0: 696c 6974 7922 3a20 226e 6f6e 7061 7961  ility": "nonpaya
+00018be0: 626c 6522 2c20 2274 7970 6522 3a20 2266  ble", "type": "f
+00018bf0: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+00018c00: 6e70 7574 7322 3a20 5b20 7b20 2269 6e74  nputs": [ { "int
+00018c10: 6572 6e61 6c54 7970 6522 3a20 2261 6464  ernalType": "add
+00018c20: 7265 7373 222c 2022 6e61 6d65 223a 2022  ress", "name": "
+00018c30: 6672 6f6d 222c 2022 7479 7065 223a 2022  from", "type": "
+00018c40: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+00018c50: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+00018c60: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+00018c70: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
+00018c80: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+00018c90: 6e74 6572 6e61 6c54 7970 6522 3a20 2275  nternalType": "u
+00018ca0: 696e 7432 3536 222c 2022 6e61 6d65 223a  int256", "name":
+00018cb0: 2022 7661 6c75 6522 2c20 2274 7970 6522   "value", "type"
+00018cc0: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
+00018cd0: 2022 6e61 6d65 223a 2022 7472 616e 7366   "name": "transf
+00018ce0: 6572 4672 6f6d 222c 2022 6f75 7470 7574  erFrom", "output
+00018cf0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+00018d00: 6c54 7970 6522 3a20 2262 6f6f 6c22 2c20  lType": "bool", 
+00018d10: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+00018d20: 6522 3a20 2262 6f6f 6c22 207d 205d 2c20  e": "bool" } ], 
+00018d30: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00018d40: 223a 2022 6e6f 6e70 6179 6162 6c65 222c  ": "nonpayable",
+00018d50: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
+00018d60: 6f6e 2220 7d20 5d27 2020 0a0a 636c 6173  on" } ]'  ..clas
+00018d70: 7320 4a6f 6556 3252 6f75 7465 3a0a 2020  s JoeV2Route:.  
+00018d80: 2020 6a6f 655f 726f 7574 655f 7632 5f61    joe_route_v2_a
+00018d90: 6269 3d6a 736f 6e2e 6c6f 6164 7328 275b  bi=json.loads('[
+00018da0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00018db0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+00018dc0: 7261 6374 2049 4c42 4661 6374 6f72 7922  ract ILBFactory"
+00018dd0: 2c22 6e61 6d65 223a 225f 6661 6374 6f72  ,"name":"_factor
+00018de0: 7922 2c22 7479 7065 223a 2261 6464 7265  y","type":"addre
+00018df0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00018e00: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+00018e10: 4a6f 6546 6163 746f 7279 222c 226e 616d  JoeFactory","nam
+00018e20: 6522 3a22 5f6f 6c64 4661 6374 6f72 7922  e":"_oldFactory"
+00018e30: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00018e40: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00018e50: 6522 3a22 636f 6e74 7261 6374 2049 5741  e":"contract IWA
+00018e60: 5641 5822 2c22 6e61 6d65 223a 225f 7761  VAX","name":"_wa
+00018e70: 7661 7822 2c22 7479 7065 223a 2261 6464  vax","type":"add
+00018e80: 7265 7373 227d 5d2c 2273 7461 7465 4d75  ress"}],"stateMu
+00018e90: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
+00018ea0: 7961 626c 6522 2c22 7479 7065 223a 2263  yable","type":"c
+00018eb0: 6f6e 7374 7275 6374 6f72 227d 2c7b 2269  onstructor"},{"i
+00018ec0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00018ed0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00018ee0: 222c 226e 616d 6522 3a22 6270 222c 2274  ","name":"bp","t
+00018ef0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+00018f00: 2c22 6e61 6d65 223a 2242 696e 4865 6c70  ,"name":"BinHelp
+00018f10: 6572 5f5f 4269 6e53 7465 704f 7665 7266  er__BinStepOverf
+00018f20: 6c6f 7773 222c 2274 7970 6522 3a22 6572  lows","type":"er
+00018f30: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+00018f40: 5b5d 2c22 6e61 6d65 223a 2242 696e 4865  [],"name":"BinHe
+00018f50: 6c70 6572 5f5f 4964 4f76 6572 666c 6f77  lper__IdOverflow
+00018f60: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+00018f70: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00018f80: 226e 616d 6522 3a22 4a6f 654c 6962 7261  "name":"JoeLibra
+00018f90: 7279 5f5f 496e 7375 6666 6963 6965 6e74  ry__Insufficient
+00018fa0: 416d 6f75 6e74 222c 2274 7970 6522 3a22  Amount","type":"
+00018fb0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00018fc0: 223a 5b5d 2c22 6e61 6d65 223a 224a 6f65  ":[],"name":"Joe
+00018fd0: 4c69 6272 6172 795f 5f49 6e73 7566 6669  Library__Insuffi
+00018fe0: 6369 656e 744c 6971 7569 6469 7479 222c  cientLiquidity",
+00018ff0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00019000: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00019010: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00019020: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+00019030: 756e 7458 4d69 6e22 2c22 7479 7065 223a  untXMin","type":
+00019040: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00019050: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00019060: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+00019070: 756e 7458 222c 2274 7970 6522 3a22 7569  untX","type":"ui
+00019080: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+00019090: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000190a0: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+000190b0: 594d 696e 222c 2274 7970 6522 3a22 7569  YMin","type":"ui
+000190c0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+000190d0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000190e0: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+000190f0: 5922 2c22 7479 7065 223a 2275 696e 7432  Y","type":"uint2
+00019100: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
+00019110: 526f 7574 6572 5f5f 416d 6f75 6e74 536c  Router__AmountSl
+00019120: 6970 7061 6765 4361 7567 6874 222c 2274  ippageCaught","t
+00019130: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00019140: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00019150: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00019160: 3622 2c22 6e61 6d65 223a 2269 6422 2c22  6","name":"id","
+00019170: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00019180: 5d2c 226e 616d 6522 3a22 4c42 526f 7574  ],"name":"LBRout
+00019190: 6572 5f5f 4269 6e52 6573 6572 7665 4f76  er__BinReserveOv
+000191a0: 6572 666c 6f77 7322 2c22 7479 7065 223a  erflows","type":
+000191b0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+000191c0: 7322 3a5b 5d2c 226e 616d 6522 3a22 4c42  s":[],"name":"LB
+000191d0: 526f 7574 6572 5f5f 4272 6f6b 656e 5377  Router__BrokenSw
+000191e0: 6170 5361 6665 7479 4368 6563 6b22 2c22  apSafetyCheck","
+000191f0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00019200: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00019210: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019220: 3536 222c 226e 616d 6522 3a22 6465 6164  56","name":"dead
+00019230: 6c69 6e65 222c 2274 7970 6522 3a22 7569  line","type":"ui
+00019240: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+00019250: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00019260: 222c 226e 616d 6522 3a22 6375 7272 656e  ","name":"curren
+00019270: 7454 696d 6573 7461 6d70 222c 2274 7970  tTimestamp","typ
+00019280: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00019290: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
+000192a0: 5f44 6561 646c 696e 6545 7863 6565 6465  _DeadlineExceede
+000192b0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+000192c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+000192d0: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+000192e0: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+000192f0: 7265 6369 7069 656e 7422 2c22 7479 7065  recipient","type
+00019300: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00019310: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00019320: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+00019330: 6d6f 756e 7422 2c22 7479 7065 223a 2275  mount","type":"u
+00019340: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+00019350: 3a22 4c42 526f 7574 6572 5f5f 4661 696c  :"LBRouter__Fail
+00019360: 6564 546f 5365 6e64 4156 4158 222c 2274  edToSendAVAX","t
+00019370: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00019380: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00019390: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000193a0: 3622 2c22 6e61 6d65 223a 2269 6444 6573  6","name":"idDes
+000193b0: 6972 6564 222c 2274 7970 6522 3a22 7569  ired","type":"ui
+000193c0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+000193d0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000193e0: 222c 226e 616d 6522 3a22 6964 536c 6970  ","name":"idSlip
+000193f0: 7061 6765 222c 2274 7970 6522 3a22 7569  page","type":"ui
+00019400: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+00019410: 224c 4252 6f75 7465 725f 5f49 6444 6573  "LBRouter__IdDes
+00019420: 6972 6564 4f76 6572 666c 6f77 7322 2c22  iredOverflows","
+00019430: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00019440: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00019450: 726e 616c 5479 7065 223a 2269 6e74 3235  rnalType":"int25
+00019460: 3622 2c22 6e61 6d65 223a 2269 6422 2c22  6","name":"id","
+00019470: 7479 7065 223a 2269 6e74 3235 3622 7d5d  type":"int256"}]
+00019480: 2c22 6e61 6d65 223a 224c 4252 6f75 7465  ,"name":"LBRoute
+00019490: 725f 5f49 644f 7665 7266 6c6f 7773 222c  r__IdOverflows",
+000194a0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+000194b0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+000194c0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000194d0: 3235 3622 2c22 6e61 6d65 223a 2261 6374  256","name":"act
+000194e0: 6976 6549 6444 6573 6972 6564 222c 2274  iveIdDesired","t
+000194f0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00019500: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019510: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00019520: 3a22 6964 536c 6970 7061 6765 222c 2274  :"idSlippage","t
+00019530: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00019540: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019550: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00019560: 3a22 6163 7469 7665 4964 222c 2274 7970  :"activeId","typ
+00019570: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00019580: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
+00019590: 5f49 6453 6c69 7070 6167 6543 6175 6768  _IdSlippageCaugh
+000195a0: 7422 2c22 7479 7065 223a 2265 7272 6f72  t","type":"error
+000195b0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+000195c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000195d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000195e0: 616d 6f75 6e74 4f75 744d 696e 222c 2274  amountOutMin","t
+000195f0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00019600: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019610: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00019620: 3a22 616d 6f75 6e74 4f75 7422 2c22 7479  :"amountOut","ty
+00019630: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00019640: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
+00019650: 5f5f 496e 7375 6666 6963 6965 6e74 416d  __InsufficientAm
+00019660: 6f75 6e74 4f75 7422 2c22 7479 7065 223a  ountOut","type":
+00019670: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019680: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019690: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+000196a0: 616d 6522 3a22 7772 6f6e 6754 6f6b 656e  ame":"wrongToken
+000196b0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000196c0: 7322 7d5d 2c22 6e61 6d65 223a 224c 4252  s"}],"name":"LBR
+000196d0: 6f75 7465 725f 5f49 6e76 616c 6964 546f  outer__InvalidTo
+000196e0: 6b65 6e50 6174 6822 2c22 7479 7065 223a  kenPath","type":
+000196f0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019700: 7322 3a5b 5d2c 226e 616d 6522 3a22 4c42  s":[],"name":"LB
+00019710: 526f 7574 6572 5f5f 4c65 6e67 7468 734d  Router__LengthsM
+00019720: 6973 6d61 7463 6822 2c22 7479 7065 223a  ismatch","type":
+00019730: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019740: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019750: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00019760: 616d 6522 3a22 616d 6f75 6e74 496e 4d61  ame":"amountInMa
+00019770: 7822 2c22 7479 7065 223a 2275 696e 7432  x","type":"uint2
+00019780: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+00019790: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+000197a0: 6e61 6d65 223a 2261 6d6f 756e 7449 6e22  name":"amountIn"
+000197b0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+000197c0: 227d 5d2c 226e 616d 6522 3a22 4c42 526f  "}],"name":"LBRo
+000197d0: 7574 6572 5f5f 4d61 7841 6d6f 756e 7449  uter__MaxAmountI
+000197e0: 6e45 7863 6565 6465 6422 2c22 7479 7065  nExceeded","type
+000197f0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00019800: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00019810: 4c42 526f 7574 6572 5f5f 4e6f 7446 6163  LBRouter__NotFac
+00019820: 746f 7279 4f77 6e65 7222 2c22 7479 7065  toryOwner","type
+00019830: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00019840: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00019850: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00019860: 226e 616d 6522 3a22 746f 6b65 6e58 222c  "name":"tokenX",
+00019870: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00019880: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00019890: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+000198a0: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
+000198b0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+000198c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000198d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000198e0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
+000198f0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00019900: 6522 3a22 4c42 526f 7574 6572 5f5f 5061  e":"LBRouter__Pa
+00019910: 6972 4e6f 7443 7265 6174 6564 222c 2274  irNotCreated","t
+00019920: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00019930: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00019940: 223a 224c 4252 6f75 7465 725f 5f53 656e  ":"LBRouter__Sen
+00019950: 6465 7249 734e 6f74 5741 5641 5822 2c22  derIsNotWAVAX","
+00019960: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00019970: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00019980: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019990: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
+000199a0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000199b0: 7d5d 2c22 6e61 6d65 223a 224c 4252 6f75  }],"name":"LBRou
+000199c0: 7465 725f 5f53 7761 704f 7665 7266 6c6f  ter__SwapOverflo
+000199d0: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
+000199e0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+000199f0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00019a00: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00019a10: 2265 7863 6573 7322 2c22 7479 7065 223a  "excess","type":
+00019a20: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00019a30: 6522 3a22 4c42 526f 7574 6572 5f5f 546f  e":"LBRouter__To
+00019a40: 6f4d 7563 6854 6f6b 656e 7349 6e22 2c22  oMuchTokensIn","
+00019a50: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00019a60: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00019a70: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019a80: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+00019a90: 6e74 222c 2274 7970 6522 3a22 7569 6e74  nt","type":"uint
+00019aa0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+00019ab0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+00019ac0: 226e 616d 6522 3a22 7265 7365 7276 6522  "name":"reserve"
+00019ad0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00019ae0: 227d 5d2c 226e 616d 6522 3a22 4c42 526f  "}],"name":"LBRo
+00019af0: 7574 6572 5f5f 5772 6f6e 6741 6d6f 756e  uter__WrongAmoun
+00019b00: 7473 222c 2274 7970 6522 3a22 6572 726f  ts","type":"erro
+00019b10: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+00019b20: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00019b30: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+00019b40: 2274 6f6b 656e 5822 2c22 7479 7065 223a  "tokenX","type":
+00019b50: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00019b60: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+00019b70: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
+00019b80: 656e 5922 2c22 7479 7065 223a 2261 6464  enY","type":"add
+00019b90: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+00019ba0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00019bb0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7458  ,"name":"amountX
+00019bc0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00019bd0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00019be0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00019bf0: 616d 6522 3a22 616d 6f75 6e74 5922 2c22  ame":"amountY","
+00019c00: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00019c10: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00019c20: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00019c30: 223a 226d 7367 5661 6c75 6522 2c22 7479  ":"msgValue","ty
+00019c40: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00019c50: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
+00019c60: 5f5f 5772 6f6e 6741 7661 784c 6971 7569  __WrongAvaxLiqui
+00019c70: 6469 7479 5061 7261 6d65 7465 7273 222c  dityParameters",
+00019c80: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00019c90: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+00019ca0: 6d65 223a 224c 4252 6f75 7465 725f 5f57  me":"LBRouter__W
+00019cb0: 726f 6e67 546f 6b65 6e4f 7264 6572 222c  rongTokenOrder",
+00019cc0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00019cd0: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+00019ce0: 6d65 223a 224d 6174 6831 3238 7831 3238  me":"Math128x128
+00019cf0: 5f5f 4c6f 6755 6e64 6572 666c 6f77 222c  __LogUnderflow",
+00019d00: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00019d10: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00019d20: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00019d30: 3235 3622 2c22 6e61 6d65 223a 2278 222c  256","name":"x",
+00019d40: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00019d50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00019d60: 223a 2269 6e74 3235 3622 2c22 6e61 6d65  ":"int256","name
+00019d70: 223a 2279 222c 2274 7970 6522 3a22 696e  ":"y","type":"in
+00019d80: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00019d90: 4d61 7468 3132 3878 3132 385f 5f50 6f77  Math128x128__Pow
+00019da0: 6572 556e 6465 7266 6c6f 7722 2c22 7479  erUnderflow","ty
+00019db0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+00019dc0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00019dd0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00019de0: 222c 226e 616d 6522 3a22 7072 6f64 3122  ","name":"prod1"
+00019df0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00019e00: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00019e10: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00019e20: 6d65 223a 2264 656e 6f6d 696e 6174 6f72  me":"denominator
+00019e30: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00019e40: 3622 7d5d 2c22 6e61 6d65 223a 224d 6174  6"}],"name":"Mat
+00019e50: 6835 3132 4269 7473 5f5f 4d75 6c44 6976  h512Bits__MulDiv
+00019e60: 4f76 6572 666c 6f77 222c 2274 7970 6522  Overflow","type"
+00019e70: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00019e80: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00019e90: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00019ea0: 6e61 6d65 223a 2270 726f 6431 222c 2274  name":"prod1","t
+00019eb0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00019ec0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019ed0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00019ee0: 3a22 6f66 6673 6574 222c 2274 7970 6522  :"offset","type"
+00019ef0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+00019f00: 6d65 223a 224d 6174 6835 3132 4269 7473  me":"Math512Bits
+00019f10: 5f5f 4d75 6c53 6869 6674 4f76 6572 666c  __MulShiftOverfl
+00019f20: 6f77 222c 2274 7970 6522 3a22 6572 726f  ow","type":"erro
+00019f30: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+00019f40: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00019f50: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00019f60: 226f 6666 7365 7422 2c22 7479 7065 223a  "offset","type":
+00019f70: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00019f80: 6522 3a22 4d61 7468 3531 3242 6974 735f  e":"Math512Bits_
+00019f90: 5f4f 6666 7365 744f 7665 7266 6c6f 7773  _OffsetOverflows
+00019fa0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00019fb0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00019fc0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00019fd0: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
+00019fe0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00019ff0: 3622 7d5d 2c22 6e61 6d65 223a 2253 6166  6"}],"name":"Saf
+0001a000: 6543 6173 745f 5f45 7863 6565 6473 3132  eCast__Exceeds12
+0001a010: 3842 6974 7322 2c22 7479 7065 223a 2265  8Bits","type":"e
+0001a020: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001a030: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001a040: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001a050: 6522 3a22 7822 2c22 7479 7065 223a 2275  e":"x","type":"u
+0001a060: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+0001a070: 3a22 5361 6665 4361 7374 5f5f 4578 6365  :"SafeCast__Exce
+0001a080: 6564 7334 3042 6974 7322 2c22 7479 7065  eds40Bits","type
+0001a090: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+0001a0a0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+0001a0b0: 546f 6b65 6e48 656c 7065 725f 5f43 616c  TokenHelper__Cal
+0001a0c0: 6c46 6169 6c65 6422 2c22 7479 7065 223a  lFailed","type":
+0001a0d0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+0001a0e0: 7322 3a5b 5d2c 226e 616d 6522 3a22 546f  s":[],"name":"To
+0001a0f0: 6b65 6e48 656c 7065 725f 5f4e 6f6e 436f  kenHelper__NonCo
+0001a100: 6e74 7261 6374 222c 2274 7970 6522 3a22  ntract","type":"
+0001a110: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001a120: 223a 5b5d 2c22 6e61 6d65 223a 2254 6f6b  ":[],"name":"Tok
+0001a130: 656e 4865 6c70 6572 5f5f 5472 616e 7366  enHelper__Transf
+0001a140: 6572 4661 696c 6564 222c 2274 7970 6522  erFailed","type"
+0001a150: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001a160: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
+0001a170: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0001a180: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+0001a190: 5243 3230 222c 226e 616d 6522 3a22 746f  RC20","name":"to
+0001a1a0: 6b65 6e58 222c 2274 7970 6522 3a22 6164  kenX","type":"ad
+0001a1b0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001a1c0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001a1d0: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
+0001a1e0: 3a22 746f 6b65 6e59 222c 2274 7970 6522  :"tokenY","type"
+0001a1f0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001a200: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a210: 7432 3536 222c 226e 616d 6522 3a22 6269  t256","name":"bi
+0001a220: 6e53 7465 7022 2c22 7479 7065 223a 2275  nStep","type":"u
+0001a230: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
+0001a240: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001a250: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0001a260: 7458 222c 2274 7970 6522 3a22 7569 6e74  tX","type":"uint
+0001a270: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001a280: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001a290: 226e 616d 6522 3a22 616d 6f75 6e74 5922  "name":"amountY"
+0001a2a0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001a2b0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001a2c0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001a2d0: 6d65 223a 2261 6d6f 756e 7458 4d69 6e22  me":"amountXMin"
+0001a2e0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001a2f0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001a300: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001a310: 6d65 223a 2261 6d6f 756e 7459 4d69 6e22  me":"amountYMin"
+0001a320: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001a330: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001a340: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001a350: 6d65 223a 2261 6374 6976 6549 6444 6573  me":"activeIdDes
+0001a360: 6972 6564 222c 2274 7970 6522 3a22 7569  ired","type":"ui
+0001a370: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001a380: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001a390: 222c 226e 616d 6522 3a22 6964 536c 6970  ","name":"idSlip
+0001a3a0: 7061 6765 222c 2274 7970 6522 3a22 7569  page","type":"ui
+0001a3b0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001a3c0: 616c 5479 7065 223a 2269 6e74 3235 365b  alType":"int256[
+0001a3d0: 5d22 2c22 6e61 6d65 223a 2264 656c 7461  ]","name":"delta
+0001a3e0: 4964 7322 2c22 7479 7065 223a 2269 6e74  Ids","type":"int
+0001a3f0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+0001a400: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001a410: 5b5d 222c 226e 616d 6522 3a22 6469 7374  []","name":"dist
+0001a420: 7269 6275 7469 6f6e 5822 2c22 7479 7065  ributionX","type
+0001a430: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
+0001a440: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001a450: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+0001a460: 223a 2264 6973 7472 6962 7574 696f 6e59  ":"distributionY
+0001a470: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001a480: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+0001a490: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001a4a0: 226e 616d 6522 3a22 746f 222c 2274 7970  "name":"to","typ
+0001a4b0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001a4c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001a4d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001a4e0: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
+0001a4f0: 3a22 7569 6e74 3235 3622 7d5d 2c22 696e  :"uint256"}],"in
+0001a500: 7465 726e 616c 5479 7065 223a 2273 7472  ternalType":"str
+0001a510: 7563 7420 494c 4252 6f75 7465 722e 4c69  uct ILBRouter.Li
+0001a520: 7175 6964 6974 7950 6172 616d 6574 6572  quidityParameter
+0001a530: 7322 2c22 6e61 6d65 223a 225f 6c69 7175  s","name":"_liqu
+0001a540: 6964 6974 7950 6172 616d 6574 6572 7322  idityParameters"
+0001a550: 2c22 7479 7065 223a 2274 7570 6c65 227d  ,"type":"tuple"}
+0001a560: 5d2c 226e 616d 6522 3a22 6164 644c 6971  ],"name":"addLiq
+0001a570: 7569 6469 7479 222c 226f 7574 7075 7473  uidity","outputs
+0001a580: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001a590: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+0001a5a0: 6e61 6d65 223a 2264 6570 6f73 6974 4964  name":"depositId
+0001a5b0: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
+0001a5c0: 3536 5b5d 227d 2c7b 2269 6e74 6572 6e61  56[]"},{"interna
+0001a5d0: 6c54 7970 6522 3a22 7569 6e74 3235 365b  lType":"uint256[
+0001a5e0: 5d22 2c22 6e61 6d65 223a 226c 6971 7569  ]","name":"liqui
+0001a5f0: 6469 7479 4d69 6e74 6564 222c 2274 7970  dityMinted","typ
+0001a600: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
+0001a610: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001a620: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+0001a630: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0001a640: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0001a650: 636f 6d70 6f6e 656e 7473 223a 5b7b 2269  components":[{"i
+0001a660: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+0001a670: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
+0001a680: 6e61 6d65 223a 2274 6f6b 656e 5822 2c22  name":"tokenX","
+0001a690: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001a6a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a6b0: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+0001a6c0: 3022 2c22 6e61 6d65 223a 2274 6f6b 656e  0","name":"token
+0001a6d0: 5922 2c22 7479 7065 223a 2261 6464 7265  Y","type":"addre
+0001a6e0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+0001a6f0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001a700: 6e61 6d65 223a 2262 696e 5374 6570 222c  name":"binStep",
+0001a710: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001a720: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a730: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001a740: 6522 3a22 616d 6f75 6e74 5822 2c22 7479  e":"amountX","ty
+0001a750: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+0001a760: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001a770: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001a780: 2261 6d6f 756e 7459 222c 2274 7970 6522  "amountY","type"
+0001a790: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001a7a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a7b0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0001a7c0: 6f75 6e74 584d 696e 222c 2274 7970 6522  ountXMin","type"
+0001a7d0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001a7e0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a7f0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0001a800: 6f75 6e74 594d 696e 222c 2274 7970 6522  ountYMin","type"
+0001a810: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001a820: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a830: 7432 3536 222c 226e 616d 6522 3a22 6163  t256","name":"ac
+0001a840: 7469 7665 4964 4465 7369 7265 6422 2c22  tiveIdDesired","
+0001a850: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001a860: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a870: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001a880: 223a 2269 6453 6c69 7070 6167 6522 2c22  ":"idSlippage","
+0001a890: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001a8a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a8b0: 3a22 696e 7432 3536 5b5d 222c 226e 616d  :"int256[]","nam
+0001a8c0: 6522 3a22 6465 6c74 6149 6473 222c 2274  e":"deltaIds","t
+0001a8d0: 7970 6522 3a22 696e 7432 3536 5b5d 227d  ype":"int256[]"}
+0001a8e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a8f0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+0001a900: 6d65 223a 2264 6973 7472 6962 7574 696f  me":"distributio
+0001a910: 6e58 222c 2274 7970 6522 3a22 7569 6e74  nX","type":"uint
+0001a920: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+0001a930: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001a940: 5b5d 222c 226e 616d 6522 3a22 6469 7374  []","name":"dist
+0001a950: 7269 6275 7469 6f6e 5922 2c22 7479 7065  ributionY","type
+0001a960: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
+0001a970: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001a980: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0001a990: 2274 6f22 2c22 7479 7065 223a 2261 6464  "to","type":"add
+0001a9a0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+0001a9b0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001a9c0: 2c22 6e61 6d65 223a 2264 6561 646c 696e  ,"name":"deadlin
+0001a9d0: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0001a9e0: 3536 227d 5d2c 2269 6e74 6572 6e61 6c54  56"}],"internalT
+0001a9f0: 7970 6522 3a22 7374 7275 6374 2049 4c42  ype":"struct ILB
+0001aa00: 526f 7574 6572 2e4c 6971 7569 6469 7479  Router.Liquidity
+0001aa10: 5061 7261 6d65 7465 7273 222c 226e 616d  Parameters","nam
+0001aa20: 6522 3a22 5f6c 6971 7569 6469 7479 5061  e":"_liquidityPa
+0001aa30: 7261 6d65 7465 7273 222c 2274 7970 6522  rameters","type"
+0001aa40: 3a22 7475 706c 6522 7d5d 2c22 6e61 6d65  :"tuple"}],"name
+0001aa50: 223a 2261 6464 4c69 7175 6964 6974 7941  ":"addLiquidityA
+0001aa60: 5641 5822 2c22 6f75 7470 7574 7322 3a5b  VAX","outputs":[
+0001aa70: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001aa80: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+0001aa90: 6522 3a22 6465 706f 7369 7449 6473 222c  e":"depositIds",
+0001aaa0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
+0001aab0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+0001aac0: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+0001aad0: 226e 616d 6522 3a22 6c69 7175 6964 6974  "name":"liquidit
+0001aae0: 794d 696e 7465 6422 2c22 7479 7065 223a  yMinted","type":
+0001aaf0: 2275 696e 7432 3536 5b5d 227d 5d2c 2273  "uint256[]"}],"s
+0001ab00: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0001ab10: 2270 6179 6162 6c65 222c 2274 7970 6522  "payable","type"
+0001ab20: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001ab30: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0001ab40: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001ab50: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
+0001ab60: 3a22 5f74 6f6b 656e 5822 2c22 7479 7065  :"_tokenX","type
+0001ab70: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001ab80: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+0001ab90: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
+0001aba0: 6e61 6d65 223a 225f 746f 6b65 6e59 222c  name":"_tokenY",
+0001abb0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001abc0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001abd0: 223a 2275 696e 7432 3422 2c22 6e61 6d65  ":"uint24","name
+0001abe0: 223a 225f 6163 7469 7665 4964 222c 2274  ":"_activeId","t
+0001abf0: 7970 6522 3a22 7569 6e74 3234 227d 2c7b  ype":"uint24"},{
+0001ac00: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001ac10: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
+0001ac20: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+0001ac30: 3a22 7569 6e74 3136 227d 5d2c 226e 616d  :"uint16"}],"nam
+0001ac40: 6522 3a22 6372 6561 7465 4c42 5061 6972  e":"createLBPair
+0001ac50: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+0001ac60: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+0001ac70: 6e74 7261 6374 2049 4c42 5061 6972 222c  ntract ILBPair",
+0001ac80: 226e 616d 6522 3a22 7061 6972 222c 2274  "name":"pair","t
+0001ac90: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+0001aca0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001acb0: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+0001acc0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0001acd0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001ace0: 226e 616d 6522 3a22 6661 6374 6f72 7922  "name":"factory"
+0001acf0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+0001ad00: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+0001ad10: 7472 6163 7420 494c 4246 6163 746f 7279  tract ILBFactory
+0001ad20: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+0001ad30: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+0001ad40: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0001ad50: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+0001ad60: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+0001ad70: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0001ad80: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+0001ad90: 494c 4250 6169 7222 2c22 6e61 6d65 223a  ILBPair","name":
+0001ada0: 225f 4c42 5061 6972 222c 2274 7970 6522  "_LBPair","type"
+0001adb0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001adc0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001add0: 7432 3536 222c 226e 616d 6522 3a22 5f70  t256","name":"_p
+0001ade0: 7269 6365 222c 2274 7970 6522 3a22 7569  rice","type":"ui
+0001adf0: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+0001ae00: 2267 6574 4964 4672 6f6d 5072 6963 6522  "getIdFromPrice"
+0001ae10: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+0001ae20: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001ae30: 7432 3422 2c22 6e61 6d65 223a 2222 2c22  t24","name":"","
+0001ae40: 7479 7065 223a 2275 696e 7432 3422 7d5d  type":"uint24"}]
+0001ae50: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001ae60: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+0001ae70: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001ae80: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0001ae90: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001aea0: 7420 494c 4250 6169 7222 2c22 6e61 6d65  t ILBPair","name
+0001aeb0: 223a 225f 4c42 5061 6972 222c 2274 7970  ":"_LBPair","typ
+0001aec0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001aed0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001aee0: 696e 7432 3422 2c22 6e61 6d65 223a 225f  int24","name":"_
+0001aef0: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
+0001af00: 3234 227d 5d2c 226e 616d 6522 3a22 6765  24"}],"name":"ge
+0001af10: 7450 7269 6365 4672 6f6d 4964 222c 226f  tPriceFromId","o
+0001af20: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0001af30: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001af40: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
+0001af50: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001af60: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0001af70: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+0001af80: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+0001af90: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001afa0: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001afb0: 2049 4c42 5061 6972 222c 226e 616d 6522   ILBPair","name"
+0001afc0: 3a22 5f4c 4250 6169 7222 2c22 7479 7065  :"_LBPair","type
+0001afd0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001afe0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001aff0: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+0001b000: 616d 6f75 6e74 4f75 7422 2c22 7479 7065  amountOut","type
+0001b010: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001b020: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
+0001b030: 6f6c 222c 226e 616d 6522 3a22 5f73 7761  ol","name":"_swa
+0001b040: 7046 6f72 5922 2c22 7479 7065 223a 2262  pForY","type":"b
+0001b050: 6f6f 6c22 7d5d 2c22 6e61 6d65 223a 2267  ool"}],"name":"g
+0001b060: 6574 5377 6170 496e 222c 226f 7574 7075  etSwapIn","outpu
+0001b070: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001b080: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001b090: 6e61 6d65 223a 2261 6d6f 756e 7449 6e22  name":"amountIn"
+0001b0a0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001b0b0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001b0c0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001b0d0: 6d65 223a 2266 6565 7349 6e22 2c22 7479  me":"feesIn","ty
+0001b0e0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001b0f0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0001b100: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+0001b110: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+0001b120: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001b130: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001b140: 2049 4c42 5061 6972 222c 226e 616d 6522   ILBPair","name"
+0001b150: 3a22 5f4c 4250 6169 7222 2c22 7479 7065  :"_LBPair","type
+0001b160: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001b170: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001b180: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+0001b190: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
+0001b1a0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001b1b0: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
+0001b1c0: 6c22 2c22 6e61 6d65 223a 225f 7377 6170  l","name":"_swap
+0001b1d0: 466f 7259 222c 2274 7970 6522 3a22 626f  ForY","type":"bo
+0001b1e0: 6f6c 227d 5d2c 226e 616d 6522 3a22 6765  ol"}],"name":"ge
+0001b1f0: 7453 7761 704f 7574 222c 226f 7574 7075  tSwapOut","outpu
+0001b200: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001b210: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001b220: 6e61 6d65 223a 2261 6d6f 756e 744f 7574  name":"amountOut
+0001b230: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b240: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001b250: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001b260: 616d 6522 3a22 6665 6573 496e 222c 2274  ame":"feesIn","t
+0001b270: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001b280: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001b290: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+0001b2a0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001b2b0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001b2c0: 3a22 6f6c 6446 6163 746f 7279 222c 226f  :"oldFactory","o
+0001b2d0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0001b2e0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+0001b2f0: 6374 2049 4a6f 6546 6163 746f 7279 222c  ct IJoeFactory",
+0001b300: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+0001b310: 3a22 6164 6472 6573 7322 7d5d 2c22 7374  :"address"}],"st
+0001b320: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001b330: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+0001b340: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+0001b350: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0001b360: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+0001b370: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
+0001b380: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
+0001b390: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0001b3a0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+0001b3b0: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
+0001b3c0: 223a 225f 746f 6b65 6e59 222c 2274 7970  ":"_tokenY","typ
+0001b3d0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001b3e0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001b3f0: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
+0001b400: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
+0001b410: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
+0001b420: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001b430: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
+0001b440: 756e 7458 4d69 6e22 2c22 7479 7065 223a  untXMin","type":
+0001b450: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001b460: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001b470: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
+0001b480: 6f75 6e74 594d 696e 222c 2274 7970 6522  ountYMin","type"
+0001b490: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001b4a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001b4b0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+0001b4c0: 5f69 6473 222c 2274 7970 6522 3a22 7569  _ids","type":"ui
+0001b4d0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
+0001b4e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001b4f0: 3536 5b5d 222c 226e 616d 6522 3a22 5f61  56[]","name":"_a
+0001b500: 6d6f 756e 7473 222c 2274 7970 6522 3a22  mounts","type":"
+0001b510: 7569 6e74 3235 365b 5d22 7d2c 7b22 696e  uint256[]"},{"in
+0001b520: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001b530: 7265 7373 222c 226e 616d 6522 3a22 5f74  ress","name":"_t
+0001b540: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
+0001b550: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+0001b560: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001b570: 6e61 6d65 223a 225f 6465 6164 6c69 6e65  name":"_deadline
+0001b580: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b590: 3622 7d5d 2c22 6e61 6d65 223a 2272 656d  6"}],"name":"rem
+0001b5a0: 6f76 654c 6971 7569 6469 7479 222c 226f  oveLiquidity","o
+0001b5b0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0001b5c0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001b5d0: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0001b5e0: 7458 222c 2274 7970 6522 3a22 7569 6e74  tX","type":"uint
+0001b5f0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001b600: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001b610: 226e 616d 6522 3a22 616d 6f75 6e74 5922  "name":"amountY"
+0001b620: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001b630: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
+0001b640: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
+0001b650: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+0001b660: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+0001b670: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001b680: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+0001b690: 3022 2c22 6e61 6d65 223a 225f 746f 6b65  0","name":"_toke
+0001b6a0: 6e22 2c22 7479 7065 223a 2261 6464 7265  n","type":"addre
+0001b6b0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+0001b6c0: 7970 6522 3a22 7569 6e74 3136 222c 226e  ype":"uint16","n
+0001b6d0: 616d 6522 3a22 5f62 696e 5374 6570 222c  ame":"_binStep",
+0001b6e0: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+0001b6f0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001b700: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001b710: 223a 225f 616d 6f75 6e74 546f 6b65 6e4d  ":"_amountTokenM
+0001b720: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
+0001b730: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001b740: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001b750: 226e 616d 6522 3a22 5f61 6d6f 756e 7441  "name":"_amountA
+0001b760: 5641 584d 696e 222c 2274 7970 6522 3a22  VAXMin","type":"
+0001b770: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001b780: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001b790: 3536 5b5d 222c 226e 616d 6522 3a22 5f69  56[]","name":"_i
+0001b7a0: 6473 222c 2274 7970 6522 3a22 7569 6e74  ds","type":"uint
+0001b7b0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+0001b7c0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001b7d0: 5b5d 222c 226e 616d 6522 3a22 5f61 6d6f  []","name":"_amo
+0001b7e0: 756e 7473 222c 2274 7970 6522 3a22 7569  unts","type":"ui
+0001b7f0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
+0001b800: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001b810: 7373 2070 6179 6162 6c65 222c 226e 616d  ss payable","nam
+0001b820: 6522 3a22 5f74 6f22 2c22 7479 7065 223a  e":"_to","type":
+0001b830: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+0001b840: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001b850: 3235 3622 2c22 6e61 6d65 223a 225f 6465  256","name":"_de
+0001b860: 6164 6c69 6e65 222c 2274 7970 6522 3a22  adline","type":"
+0001b870: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+0001b880: 223a 2272 656d 6f76 654c 6971 7569 6469  ":"removeLiquidi
+0001b890: 7479 4156 4158 222c 226f 7574 7075 7473  tyAVAX","outputs
+0001b8a0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001b8b0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001b8c0: 6d65 223a 2261 6d6f 756e 7454 6f6b 656e  me":"amountToken
+0001b8d0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b8e0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001b8f0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001b900: 616d 6522 3a22 616d 6f75 6e74 4156 4158  ame":"amountAVAX
+0001b910: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b920: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
+0001b930: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
+0001b940: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0001b950: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0001b960: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001b970: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001b980: 6522 3a22 5f61 6d6f 756e 744f 7574 222c  e":"_amountOut",
+0001b990: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001b9a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001b9b0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001b9c0: 616d 6522 3a22 5f70 6169 7242 696e 5374  ame":"_pairBinSt
+0001b9d0: 6570 7322 2c22 7479 7065 223a 2275 696e  eps","type":"uin
+0001b9e0: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001b9f0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+0001ba00: 6374 2049 4552 4332 305b 5d22 2c22 6e61  ct IERC20[]","na
+0001ba10: 6d65 223a 225f 746f 6b65 6e50 6174 6822  me":"_tokenPath"
+0001ba20: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001ba30: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+0001ba40: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001ba50: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
+0001ba60: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001ba70: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001ba80: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001ba90: 5f64 6561 646c 696e 6522 2c22 7479 7065  _deadline","type
+0001baa0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+0001bab0: 616d 6522 3a22 7377 6170 4156 4158 466f  ame":"swapAVAXFo
+0001bac0: 7245 7861 6374 546f 6b65 6e73 222c 226f  rExactTokens","o
+0001bad0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0001bae0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001baf0: 365b 5d22 2c22 6e61 6d65 223a 2261 6d6f  6[]","name":"amo
+0001bb00: 756e 7473 496e 222c 2274 7970 6522 3a22  untsIn","type":"
+0001bb10: 7569 6e74 3235 365b 5d22 7d5d 2c22 7374  uint256[]"}],"st
+0001bb20: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001bb30: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+0001bb40: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+0001bb50: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001bb60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001bb70: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+0001bb80: 4f75 744d 696e 222c 2274 7970 6522 3a22  OutMin","type":"
+0001bb90: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001bba0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001bbb0: 3536 5b5d 222c 226e 616d 6522 3a22 5f70  56[]","name":"_p
+0001bbc0: 6169 7242 696e 5374 6570 7322 2c22 7479  airBinSteps","ty
+0001bbd0: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
+0001bbe0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001bbf0: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+0001bc00: 305b 5d22 2c22 6e61 6d65 223a 225f 746f  0[]","name":"_to
+0001bc10: 6b65 6e50 6174 6822 2c22 7479 7065 223a  kenPath","type":
+0001bc20: 2261 6464 7265 7373 5b5d 227d 2c7b 2269  "address[]"},{"i
+0001bc30: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+0001bc40: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
+0001bc50: 746f 222c 2274 7970 6522 3a22 6164 6472  to","type":"addr
+0001bc60: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0001bc70: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001bc80: 226e 616d 6522 3a22 5f64 6561 646c 696e  "name":"_deadlin
+0001bc90: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0001bca0: 3536 227d 5d2c 226e 616d 6522 3a22 7377  56"}],"name":"sw
+0001bcb0: 6170 4578 6163 7441 5641 5846 6f72 546f  apExactAVAXForTo
+0001bcc0: 6b65 6e73 222c 226f 7574 7075 7473 223a  kens","outputs":
+0001bcd0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001bce0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001bcf0: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
+0001bd00: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001bd10: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001bd20: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
+0001bd30: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+0001bd40: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001bd50: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001bd60: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
+0001bd70: 6f75 6e74 4f75 744d 696e 222c 2274 7970  ountOutMin","typ
+0001bd80: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001bd90: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001bda0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+0001bdb0: 3a22 5f70 6169 7242 696e 5374 6570 7322  :"_pairBinSteps"
+0001bdc0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001bdd0: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+0001bde0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+0001bdf0: 4552 4332 305b 5d22 2c22 6e61 6d65 223a  ERC20[]","name":
+0001be00: 225f 746f 6b65 6e50 6174 6822 2c22 7479  "_tokenPath","ty
+0001be10: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
+0001be20: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001be30: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0001be40: 223a 225f 746f 222c 2274 7970 6522 3a22  ":"_to","type":"
+0001be50: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+0001be60: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001be70: 3536 222c 226e 616d 6522 3a22 5f64 6561  56","name":"_dea
+0001be80: 646c 696e 6522 2c22 7479 7065 223a 2275  dline","type":"u
+0001be90: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+0001bea0: 3a22 7377 6170 4578 6163 7441 5641 5846  :"swapExactAVAXF
+0001beb0: 6f72 546f 6b65 6e73 5375 7070 6f72 7469  orTokensSupporti
+0001bec0: 6e67 4665 654f 6e54 7261 6e73 6665 7254  ngFeeOnTransferT
+0001bed0: 6f6b 656e 7322 2c22 6f75 7470 7574 7322  okens","outputs"
+0001bee0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001bef0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001bf00: 6522 3a22 616d 6f75 6e74 4f75 7422 2c22  e":"amountOut","
+0001bf10: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001bf20: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+0001bf30: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
+0001bf40: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0001bf50: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0001bf60: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001bf70: 7432 3536 222c 226e 616d 6522 3a22 5f61  t256","name":"_a
+0001bf80: 6d6f 756e 7449 6e22 2c22 7479 7065 223a  mountIn","type":
+0001bf90: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001bfa0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001bfb0: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
+0001bfc0: 6f75 6e74 4f75 744d 696e 4156 4158 222c  ountOutMinAVAX",
+0001bfd0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001bfe0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001bff0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001c000: 616d 6522 3a22 5f70 6169 7242 696e 5374  ame":"_pairBinSt
+0001c010: 6570 7322 2c22 7479 7065 223a 2275 696e  eps","type":"uin
+0001c020: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001c030: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+0001c040: 6374 2049 4552 4332 305b 5d22 2c22 6e61  ct IERC20[]","na
+0001c050: 6d65 223a 225f 746f 6b65 6e50 6174 6822  me":"_tokenPath"
+0001c060: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001c070: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+0001c080: 7970 6522 3a22 6164 6472 6573 7320 7061  ype":"address pa
+0001c090: 7961 626c 6522 2c22 6e61 6d65 223a 225f  yable","name":"_
+0001c0a0: 746f 222c 2274 7970 6522 3a22 6164 6472  to","type":"addr
+0001c0b0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0001c0c0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001c0d0: 226e 616d 6522 3a22 5f64 6561 646c 696e  "name":"_deadlin
+0001c0e0: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0001c0f0: 3536 227d 5d2c 226e 616d 6522 3a22 7377  56"}],"name":"sw
+0001c100: 6170 4578 6163 7454 6f6b 656e 7346 6f72  apExactTokensFor
+0001c110: 4156 4158 222c 226f 7574 7075 7473 223a  AVAX","outputs":
+0001c120: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001c130: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001c140: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
+0001c150: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001c160: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0001c170: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+0001c180: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0001c190: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0001c1a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001c1b0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001c1c0: 5f61 6d6f 756e 7449 6e22 2c22 7479 7065  _amountIn","type
+0001c1d0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001c1e0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001c1f0: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+0001c200: 616d 6f75 6e74 4f75 744d 696e 4156 4158  amountOutMinAVAX
+0001c210: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001c220: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001c230: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+0001c240: 226e 616d 6522 3a22 5f70 6169 7242 696e  "name":"_pairBin
+0001c250: 5374 6570 7322 2c22 7479 7065 223a 2275  Steps","type":"u
+0001c260: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
+0001c270: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+0001c280: 7261 6374 2049 4552 4332 305b 5d22 2c22  ract IERC20[]","
+0001c290: 6e61 6d65 223a 225f 746f 6b65 6e50 6174  name":"_tokenPat
+0001c2a0: 6822 2c22 7479 7065 223a 2261 6464 7265  h","type":"addre
+0001c2b0: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
+0001c2c0: 6c54 7970 6522 3a22 6164 6472 6573 7320  lType":"address 
+0001c2d0: 7061 7961 626c 6522 2c22 6e61 6d65 223a  payable","name":
+0001c2e0: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
+0001c2f0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001c300: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001c310: 222c 226e 616d 6522 3a22 5f64 6561 646c  ","name":"_deadl
+0001c320: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
+0001c330: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+0001c340: 7377 6170 4578 6163 7454 6f6b 656e 7346  swapExactTokensF
+0001c350: 6f72 4156 4158 5375 7070 6f72 7469 6e67  orAVAXSupporting
+0001c360: 4665 654f 6e54 7261 6e73 6665 7254 6f6b  FeeOnTransferTok
+0001c370: 656e 7322 2c22 6f75 7470 7574 7322 3a5b  ens","outputs":[
+0001c380: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001c390: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001c3a0: 3a22 616d 6f75 6e74 4f75 7422 2c22 7479  :"amountOut","ty
+0001c3b0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001c3c0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0001c3d0: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+0001c3e0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+0001c3f0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001c400: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001c410: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+0001c420: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
+0001c430: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001c440: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001c450: 7432 3536 222c 226e 616d 6522 3a22 5f61  t256","name":"_a
+0001c460: 6d6f 756e 744f 7574 4d69 6e22 2c22 7479  mountOutMin","ty
+0001c470: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+0001c480: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001c490: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+0001c4a0: 223a 225f 7061 6972 4269 6e53 7465 7073  ":"_pairBinSteps
+0001c4b0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001c4c0: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+0001c4d0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+0001c4e0: 4945 5243 3230 5b5d 222c 226e 616d 6522  IERC20[]","name"
+0001c4f0: 3a22 5f74 6f6b 656e 5061 7468 222c 2274  :"_tokenPath","t
+0001c500: 7970 6522 3a22 6164 6472 6573 735b 5d22  ype":"address[]"
+0001c510: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001c520: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001c530: 6522 3a22 5f74 6f22 2c22 7479 7065 223a  e":"_to","type":
+0001c540: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+0001c550: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001c560: 3235 3622 2c22 6e61 6d65 223a 225f 6465  256","name":"_de
+0001c570: 6164 6c69 6e65 222c 2274 7970 6522 3a22  adline","type":"
+0001c580: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+0001c590: 223a 2273 7761 7045 7861 6374 546f 6b65  ":"swapExactToke
+0001c5a0: 6e73 466f 7254 6f6b 656e 7322 2c22 6f75  nsForTokens","ou
+0001c5b0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+0001c5c0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001c5d0: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+0001c5e0: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
+0001c5f0: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
+0001c600: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
+0001c610: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+0001c620: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+0001c630: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001c640: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001c650: 6e61 6d65 223a 225f 616d 6f75 6e74 496e  name":"_amountIn
+0001c660: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001c670: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001c680: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001c690: 616d 6522 3a22 5f61 6d6f 756e 744f 7574  ame":"_amountOut
+0001c6a0: 4d69 6e22 2c22 7479 7065 223a 2275 696e  Min","type":"uin
+0001c6b0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+0001c6c0: 6c54 7970 6522 3a22 7569 6e74 3235 365b  lType":"uint256[
+0001c6d0: 5d22 2c22 6e61 6d65 223a 225f 7061 6972  ]","name":"_pair
+0001c6e0: 4269 6e53 7465 7073 222c 2274 7970 6522  BinSteps","type"
+0001c6f0: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
+0001c700: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+0001c710: 6f6e 7472 6163 7420 4945 5243 3230 5b5d  ontract IERC20[]
+0001c720: 222c 226e 616d 6522 3a22 5f74 6f6b 656e  ","name":"_token
+0001c730: 5061 7468 222c 2274 7970 6522 3a22 6164  Path","type":"ad
+0001c740: 6472 6573 735b 5d22 7d2c 7b22 696e 7465  dress[]"},{"inte
+0001c750: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001c760: 7373 222c 226e 616d 6522 3a22 5f74 6f22  ss","name":"_to"
+0001c770: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001c780: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001c790: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001c7a0: 6d65 223a 225f 6465 6164 6c69 6e65 222c  me":"_deadline",
+0001c7b0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001c7c0: 7d5d 2c22 6e61 6d65 223a 2273 7761 7045  }],"name":"swapE
+0001c7d0: 7861 6374 546f 6b65 6e73 466f 7254 6f6b  xactTokensForTok
+0001c7e0: 656e 7353 7570 706f 7274 696e 6746 6565  ensSupportingFee
+0001c7f0: 4f6e 5472 616e 7366 6572 546f 6b65 6e73  OnTransferTokens
+0001c800: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+0001c810: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001c820: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001c830: 6d6f 756e 744f 7574 222c 2274 7970 6522  mountOut","type"
+0001c840: 3a22 7569 6e74 3235 3622 7d5d 2c22 7374  :"uint256"}],"st
+0001c850: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001c860: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+0001c870: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+0001c880: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001c890: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001c8a0: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
+0001c8b0: 756e 7441 5641 584f 7574 222c 2274 7970  untAVAXOut","typ
+0001c8c0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001c8d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001c8e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001c8f0: 5f61 6d6f 756e 7449 6e4d 6178 222c 2274  _amountInMax","t
+0001c900: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001c910: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001c920: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+0001c930: 6522 3a22 5f70 6169 7242 696e 5374 6570  e":"_pairBinStep
+0001c940: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
+0001c950: 3536 5b5d 227d 2c7b 2269 6e74 6572 6e61  56[]"},{"interna
+0001c960: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001c970: 2049 4552 4332 305b 5d22 2c22 6e61 6d65   IERC20[]","name
+0001c980: 223a 225f 746f 6b65 6e50 6174 6822 2c22  ":"_tokenPath","
+0001c990: 7479 7065 223a 2261 6464 7265 7373 5b5d  type":"address[]
+0001c9a0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001c9b0: 6522 3a22 6164 6472 6573 7320 7061 7961  e":"address paya
+0001c9c0: 626c 6522 2c22 6e61 6d65 223a 225f 746f  ble","name":"_to
+0001c9d0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0001c9e0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0001c9f0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001ca00: 616d 6522 3a22 5f64 6561 646c 696e 6522  ame":"_deadline"
+0001ca10: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001ca20: 227d 5d2c 226e 616d 6522 3a22 7377 6170  "}],"name":"swap
+0001ca30: 546f 6b65 6e73 466f 7245 7861 6374 4156  TokensForExactAV
+0001ca40: 4158 222c 226f 7574 7075 7473 223a 5b7b  AX","outputs":[{
+0001ca50: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001ca60: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+0001ca70: 223a 2261 6d6f 756e 7473 496e 222c 2274  ":"amountsIn","t
+0001ca80: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+0001ca90: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+0001caa0: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+0001cab0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+0001cac0: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+0001cad0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001cae0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001caf0: 3a22 5f61 6d6f 756e 744f 7574 222c 2274  :"_amountOut","t
+0001cb00: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001cb10: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001cb20: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001cb30: 3a22 5f61 6d6f 756e 7449 6e4d 6178 222c  :"_amountInMax",
+0001cb40: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001cb50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001cb60: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001cb70: 616d 6522 3a22 5f70 6169 7242 696e 5374  ame":"_pairBinSt
+0001cb80: 6570 7322 2c22 7479 7065 223a 2275 696e  eps","type":"uin
+0001cb90: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001cba0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+0001cbb0: 6374 2049 4552 4332 305b 5d22 2c22 6e61  ct IERC20[]","na
+0001cbc0: 6d65 223a 225f 746f 6b65 6e50 6174 6822  me":"_tokenPath"
+0001cbd0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001cbe0: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+0001cbf0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001cc00: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
+0001cc10: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001cc20: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001cc30: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001cc40: 5f64 6561 646c 696e 6522 2c22 7479 7065  _deadline","type
+0001cc50: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+0001cc60: 616d 6522 3a22 7377 6170 546f 6b65 6e73  ame":"swapTokens
+0001cc70: 466f 7245 7861 6374 546f 6b65 6e73 222c  ForExactTokens",
+0001cc80: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+0001cc90: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001cca0: 3235 365b 5d22 2c22 6e61 6d65 223a 2261  256[]","name":"a
+0001ccb0: 6d6f 756e 7473 496e 222c 2274 7970 6522  mountsIn","type"
+0001ccc0: 3a22 7569 6e74 3235 365b 5d22 7d5d 2c22  :"uint256[]"}],"
+0001ccd0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0001cce0: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+0001ccf0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0001cd00: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0001cd10: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+0001cd20: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+0001cd30: 616d 6522 3a22 5f74 6f6b 656e 222c 2274  ame":"_token","t
+0001cd40: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0001cd50: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001cd60: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001cd70: 3a22 5f74 6f22 2c22 7479 7065 223a 2261  :"_to","type":"a
+0001cd80: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0001cd90: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001cda0: 3622 2c22 6e61 6d65 223a 225f 616d 6f75  6","name":"_amou
+0001cdb0: 6e74 222c 2274 7970 6522 3a22 7569 6e74  nt","type":"uint
+0001cdc0: 3235 3622 7d5d 2c22 6e61 6d65 223a 2273  256"}],"name":"s
+0001cdd0: 7765 6570 222c 226f 7574 7075 7473 223a  weep","outputs":
+0001cde0: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+0001cdf0: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+0001ce00: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+0001ce10: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+0001ce20: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001ce30: 2263 6f6e 7472 6163 7420 494c 4254 6f6b  "contract ILBTok
+0001ce40: 656e 222c 226e 616d 6522 3a22 5f6c 6254  en","name":"_lbT
+0001ce50: 6f6b 656e 222c 2274 7970 6522 3a22 6164  oken","type":"ad
+0001ce60: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001ce70: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0001ce80: 222c 226e 616d 6522 3a22 5f74 6f22 2c22  ","name":"_to","
+0001ce90: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001cea0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001ceb0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+0001cec0: 6d65 223a 225f 6964 7322 2c22 7479 7065  me":"_ids","type
+0001ced0: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
+0001cee0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001cef0: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+0001cf00: 223a 225f 616d 6f75 6e74 7322 2c22 7479  ":"_amounts","ty
+0001cf10: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
+0001cf20: 5d2c 226e 616d 6522 3a22 7377 6565 704c  ],"name":"sweepL
+0001cf30: 4254 6f6b 656e 222c 226f 7574 7075 7473  BToken","outputs
+0001cf40: 223a 5b5d 2c22 7374 6174 654d 7574 6162  ":[],"stateMutab
+0001cf50: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
+0001cf60: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0001cf70: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0001cf80: 3a5b 5d2c 226e 616d 6522 3a22 7761 7661  :[],"name":"wava
+0001cf90: 7822 2c22 6f75 7470 7574 7322 3a5b 7b22  x","outputs":[{"
+0001cfa0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+0001cfb0: 6f6e 7472 6163 7420 4957 4156 4158 222c  ontract IWAVAX",
+0001cfc0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+0001cfd0: 3a22 6164 6472 6573 7322 7d5d 2c22 7374  :"address"}],"st
+0001cfe0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001cff0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+0001d000: 6e63 7469 6f6e 227d 2c7b 2273 7461 7465  nction"},{"state
+0001d010: 4d75 7461 6269 6c69 7479 223a 2270 6179  Mutability":"pay
+0001d020: 6162 6c65 222c 2274 7970 6522 3a22 7265  able","type":"re
+0001d030: 6365 6976 6522 7d5d 2729 0a0a 2020 2020  ceive"}]')..    
+0001d040: 6465 6620 6765 745f 6964 5f66 726f 6d5f  def get_id_from_
+0001d050: 7072 6963 6528 5f77 6562 333a 5765 6233  price(_web3:Web3
+0001d060: 2c5f 726f 7574 655f 6164 6472 6573 733a  ,_route_address:
+0001d070: 7374 722c 5f72 6f75 7465 5f61 6269 2c5f  str,_route_abi,_
+0001d080: 6c62 5f70 6169 722c 5f70 7269 6365 293a  lb_pair,_price):
+0001d090: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001d0a0: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
+0001d0b0: 6374 2861 6464 7265 7373 3d5f 726f 7574  ct(address=_rout
+0001d0c0: 655f 6164 6472 6573 732c 2061 6269 3d5f  e_address, abi=_
+0001d0d0: 726f 7574 655f 6162 6929 2e66 756e 6374  route_abi).funct
+0001d0e0: 696f 6e73 2e67 6574 4964 4672 6f6d 5072  ions.getIdFromPr
+0001d0f0: 6963 6528 5f6c 625f 7061 6972 2c5f 7072  ice(_lb_pair,_pr
+0001d100: 6963 6529 2e63 616c 6c28 290a 0a20 2020  ice).call()..   
+0001d110: 2064 6566 2067 6574 5f70 7269 6365 5f66   def get_price_f
+0001d120: 726f 6d5f 6964 285f 7765 6233 3a57 6562  rom_id(_web3:Web
+0001d130: 332c 5f72 6f75 7465 5f61 6464 7265 7373  3,_route_address
+0001d140: 3a73 7472 2c5f 726f 7574 655f 6162 692c  :str,_route_abi,
+0001d150: 5f6c 625f 7061 6972 2c5f 6964 293a 0a20  _lb_pair,_id):. 
+0001d160: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
+0001d170: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
+0001d180: 2861 6464 7265 7373 3d5f 726f 7574 655f  (address=_route_
+0001d190: 6164 6472 6573 732c 2061 6269 3d5f 726f  address, abi=_ro
+0001d1a0: 7574 655f 6162 6929 2e66 756e 6374 696f  ute_abi).functio
+0001d1b0: 6e73 2e67 6574 5072 6963 6546 726f 6d49  ns.getPriceFromI
+0001d1c0: 6428 5f6c 625f 7061 6972 2c5f 6964 292e  d(_lb_pair,_id).
+0001d1d0: 6361 6c6c 2829 0a0a 2020 2020 2372 6574  call()..    #ret
+0001d1e0: 7572 6e20 5b61 6d6f 756e 745f 696e 2c66  urn [amount_in,f
+0001d1f0: 6565 5d0a 2020 2020 6465 6620 6765 745f  ee].    def get_
+0001d200: 7377 6170 5f69 6e28 5f77 6562 333a 5765  swap_in(_web3:We
+0001d210: 6233 2c5f 726f 7574 655f 6164 6472 6573  b3,_route_addres
+0001d220: 733a 7374 722c 5f72 6f75 7465 5f61 6269  s:str,_route_abi
+0001d230: 3a73 7472 2c5f 6c62 5f70 6169 722c 5f61  :str,_lb_pair,_a
+0001d240: 6d6f 756e 745f 6f75 742c 5f73 7761 705f  mount_out,_swap_
+0001d250: 666f 725f 793a 626f 6f6c 293a 0a20 2020  for_y:bool):.   
+0001d260: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
+0001d270: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
+0001d280: 6464 7265 7373 3d5f 726f 7574 655f 6164  ddress=_route_ad
+0001d290: 6472 6573 732c 2061 6269 3d5f 726f 7574  dress, abi=_rout
+0001d2a0: 655f 6162 6929 2e66 756e 6374 696f 6e73  e_abi).functions
+0001d2b0: 2e67 6574 5377 6170 496e 285f 6c62 5f70  .getSwapIn(_lb_p
+0001d2c0: 6169 722c 5f61 6d6f 756e 745f 6f75 742c  air,_amount_out,
+0001d2d0: 5f73 7761 705f 666f 725f 7929 2e63 616c  _swap_for_y).cal
+0001d2e0: 6c28 290a 2020 2020 0a20 2020 2023 7265  l().    .    #re
+0001d2f0: 7475 726e 205b 616d 6f75 6e74 5f6f 7574  turn [amount_out
+0001d300: 2c66 6565 5d0a 2020 2020 6465 6620 6765  ,fee].    def ge
+0001d310: 745f 7377 6170 5f6f 7574 285f 7765 6233  t_swap_out(_web3
+0001d320: 3a57 6562 332c 5f72 6f75 7465 5f61 6464  :Web3,_route_add
+0001d330: 7265 7373 3a73 7472 2c5f 726f 7574 655f  ress:str,_route_
+0001d340: 6162 693a 7374 722c 5f6c 625f 7061 6972  abi:str,_lb_pair
+0001d350: 2c5f 616d 6f75 6e74 5f69 6e2c 5f73 7761  ,_amount_in,_swa
+0001d360: 705f 666f 725f 793a 626f 6f6c 293a 0a20  p_for_y:bool):. 
+0001d370: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
+0001d380: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
+0001d390: 2861 6464 7265 7373 3d5f 726f 7574 655f  (address=_route_
+0001d3a0: 6164 6472 6573 732c 2061 6269 3d5f 726f  address, abi=_ro
+0001d3b0: 7574 655f 6162 6929 2e66 756e 6374 696f  ute_abi).functio
+0001d3c0: 6e73 2e67 6574 5377 6170 4f75 7428 5f6c  ns.getSwapOut(_l
+0001d3d0: 625f 7061 6972 2c5f 616d 6f75 6e74 5f69  b_pair,_amount_i
+0001d3e0: 6e2c 5f73 7761 705f 666f 725f 7929 2e63  n,_swap_for_y).c
+0001d3f0: 616c 6c28 290a 0a20 2020 2064 6566 2073  all()..    def s
+0001d400: 7761 705f 6578 6163 745f 746f 6b65 6e73  wap_exact_tokens
+0001d410: 5f66 6f72 5f74 6f6b 656e 7328 5f77 6562  _for_tokens(_web
+0001d420: 333a 5765 6233 2c5f 726f 7574 655f 6164  3:Web3,_route_ad
+0001d430: 6472 6573 733a 7374 722c 5f72 6f75 7465  dress:str,_route
+0001d440: 5f61 6269 2c0a 2020 2020 2020 2020 2020  _abi,.          
+0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d460: 2020 2020 2020 2020 2020 205f 616d 6f75             _amou
+0001d470: 6e74 5f69 6e2c 5f61 6d6f 756e 745f 6f75  nt_in,_amount_ou
+0001d480: 745f 6d69 6e2c 5f70 6169 725f 6269 6e5f  t_min,_pair_bin_
+0001d490: 7374 6570 732c 5f74 6f6b 656e 5f70 6174  steps,_token_pat
+0001d4a0: 682c 5f74 6f2c 5f64 6561 646c 696e 652c  h,_to,_deadline,
+0001d4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4d0: 2020 2020 2020 5f70 7562 6c69 635f 6b65        _public_ke
+0001d4e0: 792c 5f70 7269 7661 7465 5f6b 6579 293a  y,_private_key):
+0001d4f0: 0a20 2020 2020 2020 206e 6f6e 6365 3d5f  .        nonce=_
+0001d500: 7765 6233 2e65 7468 2e67 6574 5f74 7261  web3.eth.get_tra
+0001d510: 6e73 6163 7469 6f6e 5f63 6f75 6e74 285f  nsaction_count(_
+0001d520: 7075 626c 6963 5f6b 6579 290a 2020 2020  public_key).    
+0001d530: 2020 2020 726f 7574 655f 636f 6e74 7261      route_contra
+0001d540: 6374 3d5f 7765 6233 2e65 7468 2e63 6f6e  ct=_web3.eth.con
+0001d550: 7472 6163 7428 6164 6472 6573 733d 5f72  tract(address=_r
+0001d560: 6f75 7465 5f61 6464 7265 7373 2c20 6162  oute_address, ab
+0001d570: 693d 5f72 6f75 7465 5f61 6269 290a 2020  i=_route_abi).  
+0001d580: 2020 2020 2020 7377 6170 5f66 756e 6374        swap_funct
+0001d590: 696f 6e3d 726f 7574 655f 636f 6e74 7261  ion=route_contra
+0001d5a0: 6374 2e66 756e 6374 696f 6e73 2e73 7761  ct.functions.swa
+0001d5b0: 7045 7861 6374 546f 6b65 6e73 466f 7254  pExactTokensForT
+0001d5c0: 6f6b 656e 7328 5f61 6d6f 756e 745f 696e  okens(_amount_in
+0001d5d0: 2c5f 616d 6f75 6e74 5f6f 7574 5f6d 696e  ,_amount_out_min
+0001d5e0: 2c5f 7061 6972 5f62 696e 5f73 7465 7073  ,_pair_bin_steps
+0001d5f0: 2c5f 746f 6b65 6e5f 7061 7468 2c5f 746f  ,_token_path,_to
+0001d600: 2c5f 6465 6164 6c69 6e65 290a 2020 2020  ,_deadline).    
+0001d610: 2020 2020 7061 7261 6d73 3d7b 0a20 2020      params={.   
+0001d620: 2020 2020 2020 2020 2027 6672 6f6d 273a           'from':
+0001d630: 205f 7075 626c 6963 5f6b 6579 2c0a 2020   _public_key,.  
+0001d640: 2020 2020 2020 2020 2020 2776 616c 7565            'value
+0001d650: 273a 2030 2c0a 2020 2020 2020 2020 2020  ': 0,.          
+0001d660: 2020 276e 6f6e 6365 273a 206e 6f6e 6365    'nonce': nonce
+0001d670: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+0001d680: 7970 6527 3a20 2730 7832 270a 2020 2020  ype': '0x2'.    
+0001d690: 2020 2020 7d0a 2020 2020 2020 2020 7369      }.        si
+0001d6a0: 676e 6564 5f74 7261 6e73 6163 7469 6f6e  gned_transaction
+0001d6b0: 3d5f 7765 6233 2e65 7468 2e61 6363 6f75  =_web3.eth.accou
+0001d6c0: 6e74 2e73 6967 6e5f 7472 616e 7361 6374  nt.sign_transact
+0001d6d0: 696f 6e28 7377 6170 5f66 756e 6374 696f  ion(swap_functio
+0001d6e0: 6e2e 6275 696c 6454 7261 6e73 6163 7469  n.buildTransacti
+0001d6f0: 6f6e 2870 6172 616d 7329 2c70 7269 7661  on(params),priva
+0001d700: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
+0001d710: 6b65 7929 0a20 2020 2020 2020 2072 6573  key).        res
+0001d720: 706f 6e73 653d 5f77 6562 332e 6574 682e  ponse=_web3.eth.
+0001d730: 7365 6e64 5f72 6177 5f74 7261 6e73 6163  send_raw_transac
+0001d740: 7469 6f6e 2873 6967 6e65 645f 7472 616e  tion(signed_tran
+0001d750: 7361 6374 696f 6e2e 7261 7754 7261 6e73  saction.rawTrans
+0001d760: 6163 7469 6f6e 290a 2020 2020 2020 2020  action).        
+0001d770: 7265 7475 726e 2057 6562 332e 746f 4865  return Web3.toHe
+0001d780: 7828 7265 7370 6f6e 7365 290a 2020 2020  x(response).    
+0001d790: 0a20 2020 2064 6566 2073 7761 705f 746f  .    def swap_to
+0001d7a0: 6b65 6e73 5f66 6f72 5f65 7861 6374 5f74  kens_for_exact_t
+0001d7b0: 6f6b 656e 7328 5f77 6562 333a 5765 6233  okens(_web3:Web3
+0001d7c0: 2c5f 726f 7574 655f 6164 6472 6573 733a  ,_route_address:
+0001d7d0: 7374 722c 5f72 6f75 7465 5f61 6269 2c0a  str,_route_abi,.
+0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d800: 2020 2020 205f 616d 6f75 6e74 5f6f 7574       _amount_out
+0001d810: 2c5f 616d 6f75 6e74 5f69 6e5f 6d61 782c  ,_amount_in_max,
+0001d820: 5f70 6169 725f 6269 6e5f 7374 6570 732c  _pair_bin_steps,
+0001d830: 5f74 6f6b 656e 5f70 6174 682c 5f74 6f2c  _token_path,_to,
+0001d840: 5f64 6561 646c 696e 652c 0a20 2020 2020  _deadline,.     
+0001d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d870: 5f70 7562 6c69 635f 6b65 792c 5f70 7269  _public_key,_pri
+0001d880: 7661 7465 5f6b 6579 293a 0a20 2020 2020  vate_key):.     
+0001d890: 2020 206e 6f6e 6365 3d5f 7765 6233 2e65     nonce=_web3.e
+0001d8a0: 7468 2e67 6574 5f74 7261 6e73 6163 7469  th.get_transacti
+0001d8b0: 6f6e 5f63 6f75 6e74 285f 7075 626c 6963  on_count(_public
+0001d8c0: 5f6b 6579 290a 2020 2020 2020 2020 726f  _key).        ro
+0001d8d0: 7574 655f 636f 6e74 7261 6374 3d5f 7765  ute_contract=_we
+0001d8e0: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+0001d8f0: 6164 6472 6573 733d 5f72 6f75 7465 5f61  address=_route_a
+0001d900: 6464 7265 7373 2c20 6162 693d 5f72 6f75  ddress, abi=_rou
+0001d910: 7465 5f61 6269 290a 2020 2020 2020 2020  te_abi).        
+0001d920: 7377 6170 5f66 756e 6374 696f 6e3d 726f  swap_function=ro
+0001d930: 7574 655f 636f 6e74 7261 6374 2e66 756e  ute_contract.fun
+0001d940: 6374 696f 6e73 2e73 7761 7054 6f6b 656e  ctions.swapToken
+0001d950: 7346 6f72 4578 6163 7454 6f6b 656e 7328  sForExactTokens(
+0001d960: 5f61 6d6f 756e 745f 6f75 742c 5f61 6d6f  _amount_out,_amo
+0001d970: 756e 745f 696e 5f6d 6178 2c5f 7061 6972  unt_in_max,_pair
+0001d980: 5f62 696e 5f73 7465 7073 2c5f 746f 6b65  _bin_steps,_toke
+0001d990: 6e5f 7061 7468 2c5f 746f 2c5f 6465 6164  n_path,_to,_dead
+0001d9a0: 6c69 6e65 290a 2020 2020 2020 2020 7061  line).        pa
+0001d9b0: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
+0001d9c0: 2020 2027 6672 6f6d 273a 205f 7075 626c     'from': _publ
+0001d9d0: 6963 5f6b 6579 2c0a 2020 2020 2020 2020  ic_key,.        
+0001d9e0: 2020 2020 2776 616c 7565 273a 2030 2c0a      'value': 0,.
+0001d9f0: 2020 2020 2020 2020 2020 2020 276e 6f6e              'non
+0001da00: 6365 273a 206e 6f6e 6365 2c0a 2020 2020  ce': nonce,.    
+0001da10: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+0001da20: 2730 7832 270a 2020 2020 2020 2020 7d0a  '0x2'.        }.
+0001da30: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
+0001da40: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
+0001da50: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
+0001da60: 6e5f 7472 616e 7361 6374 696f 6e28 7377  n_transaction(sw
+0001da70: 6170 5f66 756e 6374 696f 6e2e 6275 696c  ap_function.buil
+0001da80: 6454 7261 6e73 6163 7469 6f6e 2870 6172  dTransaction(par
+0001da90: 616d 7329 2c70 7269 7661 7465 5f6b 6579  ams),private_key
+0001daa0: 3d5f 7072 6976 6174 655f 6b65 7929 0a20  =_private_key). 
+0001dab0: 2020 2020 2020 2072 6573 706f 6e73 653d         response=
+0001dac0: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
+0001dad0: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
+0001dae0: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+0001daf0: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
+0001db00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001db10: 2057 6562 332e 746f 4865 7828 7265 7370   Web3.toHex(resp
+0001db20: 6f6e 7365 290a 0a63 6c61 7373 204a 6f65  onse)..class Joe
+0001db30: 5632 5061 6972 3a0a 0a20 2020 206a 6f65  V2Pair:..    joe
+0001db40: 5f70 6169 725f 7632 5f61 6269 3d6a 736f  _pair_v2_abi=jso
+0001db50: 6e2e 6c6f 6164 7328 275b 7b22 696e 7075  n.loads('[{"inpu
+0001db60: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001db70: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+0001db80: 4c42 4661 6374 6f72 7922 2c22 6e61 6d65  LBFactory","name
+0001db90: 223a 225f 6661 6374 6f72 7922 2c22 7479  ":"_factory","ty
+0001dba0: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+0001dbb0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0001dbc0: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+0001dbd0: 7479 7065 223a 2263 6f6e 7374 7275 6374  type":"construct
+0001dbe0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001dbf0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001dc00: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001dc10: 3a22 6270 222c 2274 7970 6522 3a22 7569  :"bp","type":"ui
+0001dc20: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+0001dc30: 2242 696e 4865 6c70 6572 5f5f 4269 6e53  "BinHelper__BinS
+0001dc40: 7465 704f 7665 7266 6c6f 7773 222c 2274  tepOverflows","t
+0001dc50: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+0001dc60: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+0001dc70: 223a 2242 696e 4865 6c70 6572 5f5f 4964  ":"BinHelper__Id
+0001dc80: 4f76 6572 666c 6f77 7322 2c22 7479 7065  Overflows","type
+0001dc90: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+0001dca0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+0001dcb0: 4c42 5061 6972 5f5f 4164 6472 6573 735a  LBPair__AddressZ
+0001dcc0: 6572 6f22 2c22 7479 7065 223a 2265 7272  ero","type":"err
+0001dcd0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001dce0: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
+0001dcf0: 5f5f 4164 6472 6573 735a 6572 6f4f 7254  __AddressZeroOrT
+0001dd00: 6869 7322 2c22 7479 7065 223a 2265 7272  his","type":"err
+0001dd10: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001dd20: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
+0001dd30: 5f5f 416c 7265 6164 7949 6e69 7469 616c  __AlreadyInitial
+0001dd40: 697a 6564 222c 2274 7970 6522 3a22 6572  ized","type":"er
+0001dd50: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+0001dd60: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001dd70: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001dd80: 223a 2269 6422 2c22 7479 7065 223a 2275  ":"id","type":"u
+0001dd90: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+0001dda0: 3a22 4c42 5061 6972 5f5f 436f 6d70 6f73  :"LBPair__Compos
+0001ddb0: 6974 696f 6e46 6163 746f 7246 6c61 7765  itionFactorFlawe
+0001ddc0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+0001ddd0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001dde0: 226e 616d 6522 3a22 4c42 5061 6972 5f5f  "name":"LBPair__
+0001ddf0: 4469 7374 7269 6275 7469 6f6e 734f 7665  DistributionsOve
+0001de00: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
+0001de10: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001de20: 3a5b 5d2c 226e 616d 6522 3a22 4c42 5061  :[],"name":"LBPa
+0001de30: 6972 5f5f 466c 6173 684c 6f61 6e43 616c  ir__FlashLoanCal
+0001de40: 6c62 6163 6b46 6169 6c65 6422 2c22 7479  lbackFailed","ty
+0001de50: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001de60: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001de70: 3a22 4c42 5061 6972 5f5f 466c 6173 684c  :"LBPair__FlashL
+0001de80: 6f61 6e49 6e76 616c 6964 4261 6c61 6e63  oanInvalidBalanc
+0001de90: 6522 2c22 7479 7065 223a 2265 7272 6f72  e","type":"error
+0001dea0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001deb0: 226e 616d 6522 3a22 4c42 5061 6972 5f5f  "name":"LBPair__
+0001dec0: 466c 6173 684c 6f61 6e49 6e76 616c 6964  FlashLoanInvalid
+0001ded0: 546f 6b65 6e22 2c22 7479 7065 223a 2265  Token","type":"e
+0001dee0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001def0: 3a5b 5d2c 226e 616d 6522 3a22 4c42 5061  :[],"name":"LBPa
+0001df00: 6972 5f5f 496e 7375 6666 6963 6965 6e74  ir__Insufficient
+0001df10: 416d 6f75 6e74 7322 2c22 7479 7065 223a  Amounts","type":
+0001df20: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+0001df30: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0001df40: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001df50: 616d 6522 3a22 6964 222c 2274 7970 6522  ame":"id","type"
+0001df60: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001df70: 6d65 223a 224c 4250 6169 725f 5f49 6e73  me":"LBPair__Ins
+0001df80: 7566 6669 6369 656e 744c 6971 7569 6469  ufficientLiquidi
+0001df90: 7479 4275 726e 6564 222c 2274 7970 6522  tyBurned","type"
+0001dfa0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001dfb0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001dfc0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001dfd0: 6e61 6d65 223a 2269 6422 2c22 7479 7065  name":"id","type
+0001dfe0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+0001dff0: 616d 6522 3a22 4c42 5061 6972 5f5f 496e  ame":"LBPair__In
+0001e000: 7375 6666 6963 6965 6e74 4c69 7175 6964  sufficientLiquid
+0001e010: 6974 794d 696e 7465 6422 2c22 7479 7065  ityMinted","type
+0001e020: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+0001e030: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+0001e040: 4c42 5061 6972 5f5f 4f6e 6c79 4661 6374  LBPair__OnlyFact
+0001e050: 6f72 7922 2c22 7479 7065 223a 2265 7272  ory","type":"err
+0001e060: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001e070: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001e080: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001e090: 3a22 6665 6552 6563 6970 6965 6e74 222c  :"feeRecipient",
+0001e0a0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001e0b0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001e0c0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001e0d0: 6522 3a22 7365 6e64 6572 222c 2274 7970  e":"sender","typ
+0001e0e0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+0001e0f0: 6e61 6d65 223a 224c 4250 6169 725f 5f4f  name":"LBPair__O
+0001e100: 6e6c 7946 6565 5265 6369 7069 656e 7422  nlyFeeRecipient"
+0001e110: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+0001e120: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+0001e130: 616d 6522 3a22 4c42 5061 6972 5f5f 4f6e  ame":"LBPair__On
+0001e140: 6c79 5374 7269 6374 6c79 496e 6372 6561  lyStrictlyIncrea
+0001e150: 7369 6e67 4964 222c 2274 7970 6522 3a22  singId","type":"
+0001e160: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001e170: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001e180: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001e190: 6d65 223a 226e 6577 5369 7a65 222c 2274  me":"newSize","t
+0001e1a0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001e1b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001e1c0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001e1d0: 3a22 6f72 6163 6c65 5369 7a65 222c 2274  :"oracleSize","t
+0001e1e0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001e1f0: 2c22 6e61 6d65 223a 224c 4250 6169 725f  ,"name":"LBPair_
+0001e200: 5f4f 7261 636c 654e 6577 5369 7a65 546f  _OracleNewSizeTo
+0001e210: 6f53 6d61 6c6c 222c 2274 7970 6522 3a22  oSmall","type":"
+0001e220: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001e230: 223a 5b5d 2c22 6e61 6d65 223a 224c 4250  ":[],"name":"LBP
+0001e240: 6169 725f 5f57 726f 6e67 4c65 6e67 7468  air__WrongLength
+0001e250: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+0001e260: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0001e270: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+0001e280: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+0001e290: 6672 6f6d 222c 2274 7970 6522 3a22 6164  from","type":"ad
+0001e2a0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001e2b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001e2c0: 222c 226e 616d 6522 3a22 6964 222c 2274  ","name":"id","t
+0001e2d0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001e2e0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001e2f0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001e300: 3a22 616d 6f75 6e74 222c 2274 7970 6522  :"amount","type"
+0001e310: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001e320: 6d65 223a 224c 4254 6f6b 656e 5f5f 4275  me":"LBToken__Bu
+0001e330: 726e 4578 6365 6564 7342 616c 616e 6365  rnExceedsBalance
+0001e340: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e350: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001e360: 6e61 6d65 223a 224c 4254 6f6b 656e 5f5f  name":"LBToken__
+0001e370: 4275 726e 4672 6f6d 4164 6472 6573 7330  BurnFromAddress0
+0001e380: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e390: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001e3a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001e3b0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001e3c0: 6363 6f75 6e74 734c 656e 6774 6822 2c22  ccountsLength","
+0001e3d0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001e3e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001e3f0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001e400: 223a 2269 6473 4c65 6e67 7468 222c 2274  ":"idsLength","t
+0001e410: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001e420: 2c22 6e61 6d65 223a 224c 4254 6f6b 656e  ,"name":"LBToken
+0001e430: 5f5f 4c65 6e67 7468 4d69 736d 6174 6368  __LengthMismatch
+0001e440: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e450: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001e460: 6e61 6d65 223a 224c 4254 6f6b 656e 5f5f  name":"LBToken__
+0001e470: 4d69 6e74 546f 4164 6472 6573 7330 222c  MintToAddress0",
+0001e480: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+0001e490: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001e4a0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001e4b0: 6573 7322 2c22 6e61 6d65 223a 226f 776e  ess","name":"own
+0001e4c0: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+0001e4d0: 6573 7322 7d5d 2c22 6e61 6d65 223a 224c  ess"}],"name":"L
+0001e4e0: 4254 6f6b 656e 5f5f 5365 6c66 4170 7072  BToken__SelfAppr
+0001e4f0: 6f76 616c 222c 2274 7970 6522 3a22 6572  oval","type":"er
+0001e500: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+0001e510: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001e520: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0001e530: 223a 226f 776e 6572 222c 2274 7970 6522  ":"owner","type"
+0001e540: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001e550: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001e560: 7265 7373 222c 226e 616d 6522 3a22 7370  ress","name":"sp
+0001e570: 656e 6465 7222 2c22 7479 7065 223a 2261  ender","type":"a
+0001e580: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
+0001e590: 3a22 4c42 546f 6b65 6e5f 5f53 7065 6e64  :"LBToken__Spend
+0001e5a0: 6572 4e6f 7441 7070 726f 7665 6422 2c22  erNotApproved","
+0001e5b0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+0001e5c0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001e5d0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001e5e0: 7373 222c 226e 616d 6522 3a22 6672 6f6d  ss","name":"from
+0001e5f0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0001e600: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0001e610: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001e620: 616d 6522 3a22 6964 222c 2274 7970 6522  ame":"id","type"
+0001e630: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001e640: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001e650: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0001e660: 6f75 6e74 222c 2274 7970 6522 3a22 7569  ount","type":"ui
+0001e670: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+0001e680: 224c 4254 6f6b 656e 5f5f 5472 616e 7366  "LBToken__Transf
+0001e690: 6572 4578 6365 6564 7342 616c 616e 6365  erExceedsBalance
+0001e6a0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e6b0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001e6c0: 6e61 6d65 223a 224c 4254 6f6b 656e 5f5f  name":"LBToken__
+0001e6d0: 5472 616e 7366 6572 4672 6f6d 4f72 546f  TransferFromOrTo
+0001e6e0: 4164 6472 6573 7330 222c 2274 7970 6522  Address0","type"
+0001e6f0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001e700: 7473 223a 5b5d 2c22 6e61 6d65 223a 224c  ts":[],"name":"L
+0001e710: 4254 6f6b 656e 5f5f 5472 616e 7366 6572  BToken__Transfer
+0001e720: 546f 5365 6c66 222c 2274 7970 6522 3a22  ToSelf","type":"
+0001e730: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001e740: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001e750: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001e760: 6d65 223a 2278 222c 2274 7970 6522 3a22  me":"x","type":"
+0001e770: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001e780: 726e 616c 5479 7065 223a 2269 6e74 3235  rnalType":"int25
+0001e790: 3622 2c22 6e61 6d65 223a 2279 222c 2274  6","name":"y","t
+0001e7a0: 7970 6522 3a22 696e 7432 3536 227d 5d2c  ype":"int256"}],
+0001e7b0: 226e 616d 6522 3a22 4d61 7468 3132 3878  "name":"Math128x
+0001e7c0: 3132 385f 5f50 6f77 6572 556e 6465 7266  128__PowerUnderf
+0001e7d0: 6c6f 7722 2c22 7479 7065 223a 2265 7272  low","type":"err
+0001e7e0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001e7f0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001e800: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001e810: 3a22 7072 6f64 3122 2c22 7479 7065 223a  :"prod1","type":
+0001e820: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001e830: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001e840: 3235 3622 2c22 6e61 6d65 223a 2264 656e  256","name":"den
+0001e850: 6f6d 696e 6174 6f72 222c 2274 7970 6522  ominator","type"
+0001e860: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001e870: 6d65 223a 224d 6174 6835 3132 4269 7473  me":"Math512Bits
+0001e880: 5f5f 4d75 6c44 6976 4f76 6572 666c 6f77  __MulDivOverflow
+0001e890: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e8a0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001e8b0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001e8c0: 6e74 3235 3622 2c22 6e61 6d65 223a 2270  nt256","name":"p
+0001e8d0: 726f 6431 222c 2274 7970 6522 3a22 7569  rod1","type":"ui
+0001e8e0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001e8f0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001e900: 222c 226e 616d 6522 3a22 6f66 6673 6574  ","name":"offset
+0001e910: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001e920: 3622 7d5d 2c22 6e61 6d65 223a 224d 6174  6"}],"name":"Mat
+0001e930: 6835 3132 4269 7473 5f5f 4d75 6c53 6869  h512Bits__MulShi
+0001e940: 6674 4f76 6572 666c 6f77 222c 2274 7970  ftOverflow","typ
+0001e950: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e960: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001e970: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001e980: 2c22 6e61 6d65 223a 226f 6666 7365 7422  ,"name":"offset"
+0001e990: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001e9a0: 227d 5d2c 226e 616d 6522 3a22 4d61 7468  "}],"name":"Math
+0001e9b0: 3531 3242 6974 735f 5f4f 6666 7365 744f  512Bits__OffsetO
+0001e9c0: 7665 7266 6c6f 7773 222c 2274 7970 6522  verflows","type"
+0001e9d0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001e9e0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001e9f0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001ea00: 6e61 6d65 223a 225f 6d69 6e54 696d 6573  name":"_minTimes
+0001ea10: 7461 6d70 222c 2274 7970 6522 3a22 7569  tamp","type":"ui
+0001ea20: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001ea30: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001ea40: 222c 226e 616d 6522 3a22 5f6c 6f6f 6b55  ","name":"_lookU
+0001ea50: 7054 696d 6573 7461 6d70 222c 2274 7970  pTimestamp","typ
+0001ea60: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001ea70: 6e61 6d65 223a 224f 7261 636c 655f 5f4c  name":"Oracle__L
+0001ea80: 6f6f 6b55 7054 696d 6573 7461 6d70 546f  ookUpTimestampTo
+0001ea90: 6f4f 6c64 222c 2274 7970 6522 3a22 6572  oOld","type":"er
+0001eaa0: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+0001eab0: 5b5d 2c22 6e61 6d65 223a 224f 7261 636c  [],"name":"Oracl
+0001eac0: 655f 5f4e 6f74 496e 6974 6961 6c69 7a65  e__NotInitialize
+0001ead0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+0001eae0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001eaf0: 226e 616d 6522 3a22 5265 656e 7472 616e  "name":"Reentran
+0001eb00: 6379 4775 6172 6455 7067 7261 6465 6162  cyGuardUpgradeab
+0001eb10: 6c65 5f5f 416c 7265 6164 7949 6e69 7469  le__AlreadyIniti
+0001eb20: 616c 697a 6564 222c 2274 7970 6522 3a22  alized","type":"
+0001eb30: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001eb40: 223a 5b5d 2c22 6e61 6d65 223a 2252 6565  ":[],"name":"Ree
+0001eb50: 6e74 7261 6e63 7947 7561 7264 5570 6772  ntrancyGuardUpgr
+0001eb60: 6164 6561 626c 655f 5f52 6565 6e74 7261  adeable__Reentra
+0001eb70: 6e74 4361 6c6c 222c 2274 7970 6522 3a22  ntCall","type":"
+0001eb80: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001eb90: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001eba0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001ebb0: 6d65 223a 2278 222c 2274 7970 6522 3a22  me":"x","type":"
+0001ebc0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+0001ebd0: 223a 2253 6166 6543 6173 745f 5f45 7863  ":"SafeCast__Exc
+0001ebe0: 6565 6473 3131 3242 6974 7322 2c22 7479  eeds112Bits","ty
+0001ebf0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001ec00: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0001ec10: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001ec20: 222c 226e 616d 6522 3a22 7822 2c22 7479  ","name":"x","ty
+0001ec30: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001ec40: 226e 616d 6522 3a22 5361 6665 4361 7374  "name":"SafeCast
+0001ec50: 5f5f 4578 6365 6564 7331 3238 4269 7473  __Exceeds128Bits
+0001ec60: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001ec70: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001ec80: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001ec90: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
+0001eca0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001ecb0: 3622 7d5d 2c22 6e61 6d65 223a 2253 6166  6"}],"name":"Saf
+0001ecc0: 6543 6173 745f 5f45 7863 6565 6473 3234  eCast__Exceeds24
+0001ecd0: 4269 7473 222c 2274 7970 6522 3a22 6572  Bits","type":"er
+0001ece0: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+0001ecf0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001ed00: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001ed10: 223a 2278 222c 2274 7970 6522 3a22 7569  ":"x","type":"ui
+0001ed20: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+0001ed30: 2253 6166 6543 6173 745f 5f45 7863 6565  "SafeCast__Excee
+0001ed40: 6473 3430 4269 7473 222c 2274 7970 6522  ds40Bits","type"
+0001ed50: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001ed60: 7473 223a 5b5d 2c22 6e61 6d65 223a 2254  ts":[],"name":"T
+0001ed70: 6f6b 656e 4865 6c70 6572 5f5f 4361 6c6c  okenHelper__Call
+0001ed80: 4661 696c 6564 222c 2274 7970 6522 3a22  Failed","type":"
+0001ed90: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001eda0: 223a 5b5d 2c22 6e61 6d65 223a 2254 6f6b  ":[],"name":"Tok
+0001edb0: 656e 4865 6c70 6572 5f5f 4e6f 6e43 6f6e  enHelper__NonCon
+0001edc0: 7472 6163 7422 2c22 7479 7065 223a 2265  tract","type":"e
+0001edd0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001ede0: 3a5b 5d2c 226e 616d 6522 3a22 546f 6b65  :[],"name":"Toke
+0001edf0: 6e48 656c 7065 725f 5f54 7261 6e73 6665  nHelper__Transfe
+0001ee00: 7246 6169 6c65 6422 2c22 7479 7065 223a  rFailed","type":
+0001ee10: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+0001ee20: 7322 3a5b 5d2c 226e 616d 6522 3a22 5472  s":[],"name":"Tr
+0001ee30: 6565 4d61 7468 5f5f 4572 726f 7244 6570  eeMath__ErrorDep
+0001ee40: 7468 5365 6172 6368 222c 2274 7970 6522  thSearch","type"
+0001ee50: 3a22 6572 726f 7222 7d2c 7b22 616e 6f6e  :"error"},{"anon
+0001ee60: 796d 6f75 7322 3a66 616c 7365 2c22 696e  ymous":false,"in
+0001ee70: 7075 7473 223a 5b7b 2269 6e64 6578 6564  puts":[{"indexed
+0001ee80: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+0001ee90: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001eea0: 226e 616d 6522 3a22 6163 636f 756e 7422  "name":"account"
+0001eeb0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001eec0: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0001eed0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0001eee0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001eef0: 6522 3a22 7365 6e64 6572 222c 2274 7970  e":"sender","typ
+0001ef00: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001ef10: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+0001ef20: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
+0001ef30: 6f6f 6c22 2c22 6e61 6d65 223a 2261 7070  ool","name":"app
+0001ef40: 726f 7665 6422 2c22 7479 7065 223a 2262  roved","type":"b
+0001ef50: 6f6f 6c22 7d5d 2c22 6e61 6d65 223a 2241  ool"}],"name":"A
+0001ef60: 7070 726f 7661 6c46 6f72 416c 6c22 2c22  pprovalForAll","
+0001ef70: 7479 7065 223a 2265 7665 6e74 227d 2c7b  type":"event"},{
+0001ef80: 2261 6e6f 6e79 6d6f 7573 223a 6661 6c73  "anonymous":fals
+0001ef90: 652c 2269 6e70 7574 7322 3a5b 7b22 696e  e,"inputs":[{"in
+0001efa0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
+0001efb0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001efc0: 6573 7322 2c22 6e61 6d65 223a 2273 656e  ess","name":"sen
+0001efd0: 6465 7222 2c22 7479 7065 223a 2261 6464  der","type":"add
+0001efe0: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
+0001eff0: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+0001f000: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001f010: 226e 616d 6522 3a22 7265 6369 7069 656e  "name":"recipien
+0001f020: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
+0001f030: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
+0001f040: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+0001f050: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001f060: 616d 6522 3a22 6964 222c 2274 7970 6522  ame":"id","type"
+0001f070: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001f080: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
+0001f090: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001f0a0: 7432 3536 222c 226e 616d 6522 3a22 6665  t256","name":"fe
+0001f0b0: 6573 5822 2c22 7479 7065 223a 2275 696e  esX","type":"uin
+0001f0c0: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+0001f0d0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+0001f0e0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001f0f0: 2c22 6e61 6d65 223a 2266 6565 7359 222c  ,"name":"feesY",
+0001f100: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001f110: 7d5d 2c22 6e61 6d65 223a 2243 6f6d 706f  }],"name":"Compo
+0001f120: 7369 7469 6f6e 4665 6522 2c22 7479 7065  sitionFee","type
+0001f130: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
+0001f140: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
+0001f150: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
+0001f160: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
+0001f170: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+0001f180: 2c22 6e61 6d65 223a 2273 656e 6465 7222  ,"name":"sender"
+0001f190: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001f1a0: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0001f1b0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0001f1c0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001f1d0: 6522 3a22 7265 6369 7069 656e 7422 2c22  e":"recipient","
+0001f1e0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001f1f0: 2c7b 2269 6e64 6578 6564 223a 7472 7565  ,{"indexed":true
+0001f200: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001f210: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001f220: 3a22 6964 222c 2274 7970 6522 3a22 7569  :"id","type":"ui
+0001f230: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+0001f240: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+0001f250: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001f260: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+0001f270: 5822 2c22 7479 7065 223a 2275 696e 7432  X","type":"uint2
+0001f280: 3536 227d 2c7b 2269 6e64 6578 6564 223a  56"},{"indexed":
+0001f290: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
+0001f2a0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001f2b0: 6e61 6d65 223a 2261 6d6f 756e 7459 222c  name":"amountY",
+0001f2c0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001f2d0: 7d5d 2c22 6e61 6d65 223a 2244 6570 6f73  }],"name":"Depos
+0001f2e0: 6974 6564 546f 4269 6e22 2c22 7479 7065  itedToBin","type
+0001f2f0: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
+0001f300: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
+0001f310: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
+0001f320: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
+0001f330: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+0001f340: 2c22 6e61 6d65 223a 2273 656e 6465 7222  ,"name":"sender"
+0001f350: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001f360: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0001f370: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0001f380: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001f390: 6522 3a22 7265 6369 7069 656e 7422 2c22  e":"recipient","
+0001f3a0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001f3b0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001f3c0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f3d0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001f3e0: 223a 2261 6d6f 756e 7458 222c 2274 7970  ":"amountX","typ
+0001f3f0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001f400: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+0001f410: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001f420: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001f430: 616d 6f75 6e74 5922 2c22 7479 7065 223a  amountY","type":
+0001f440: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+0001f450: 6522 3a22 4665 6573 436f 6c6c 6563 7465  e":"FeesCollecte
+0001f460: 6422 2c22 7479 7065 223a 2265 7665 6e74  d","type":"event
+0001f470: 227d 2c7b 2261 6e6f 6e79 6d6f 7573 223a  "},{"anonymous":
+0001f480: 6661 6c73 652c 2269 6e70 7574 7322 3a5b  false,"inputs":[
+0001f490: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
+0001f4a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001f4b0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0001f4c0: 2273 656e 6465 7222 2c22 7479 7065 223a  "sender","type":
+0001f4d0: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+0001f4e0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+0001f4f0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+0001f500: 6163 7420 494c 4246 6c61 7368 4c6f 616e  act ILBFlashLoan
+0001f510: 4361 6c6c 6261 636b 222c 226e 616d 6522  Callback","name"
+0001f520: 3a22 7265 6365 6976 6572 222c 2274 7970  :"receiver","typ
+0001f530: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001f540: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+0001f550: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+0001f560: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+0001f570: 226e 616d 6522 3a22 746f 6b65 6e22 2c22  "name":"token","
+0001f580: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001f590: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001f5a0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f5b0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001f5c0: 223a 2261 6d6f 756e 7422 2c22 7479 7065  ":"amount","type
+0001f5d0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001f5e0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
+0001f5f0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001f600: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
+0001f610: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
+0001f620: 3235 3622 7d5d 2c22 6e61 6d65 223a 2246  256"}],"name":"F
+0001f630: 6c61 7368 4c6f 616e 222c 2274 7970 6522  lashLoan","type"
+0001f640: 3a22 6576 656e 7422 7d2c 7b22 616e 6f6e  :"event"},{"anon
+0001f650: 796d 6f75 7322 3a66 616c 7365 2c22 696e  ymous":false,"in
+0001f660: 7075 7473 223a 5b7b 2269 6e64 6578 6564  puts":[{"indexed
+0001f670: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+0001f680: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001f690: 2c22 6e61 6d65 223a 2270 7265 7669 6f75  ,"name":"previou
+0001f6a0: 7353 697a 6522 2c22 7479 7065 223a 2275  sSize","type":"u
+0001f6b0: 696e 7432 3536 227d 2c7b 2269 6e64 6578  int256"},{"index
+0001f6c0: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+0001f6d0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001f6e0: 3622 2c22 6e61 6d65 223a 226e 6577 5369  6","name":"newSi
+0001f6f0: 7a65 222c 2274 7970 6522 3a22 7569 6e74  ze","type":"uint
+0001f700: 3235 3622 7d5d 2c22 6e61 6d65 223a 224f  256"}],"name":"O
+0001f710: 7261 636c 6553 697a 6549 6e63 7265 6173  racleSizeIncreas
+0001f720: 6564 222c 2274 7970 6522 3a22 6576 656e  ed","type":"even
+0001f730: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+0001f740: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+0001f750: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+0001f760: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001f770: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001f780: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
+0001f790: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001f7a0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
+0001f7b0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001f7c0: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
+0001f7d0: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+0001f7e0: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+0001f7f0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
+0001f800: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001f810: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+0001f820: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
+0001f830: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+0001f840: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+0001f850: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001f860: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
+0001f870: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001f880: 3622 7d5d 2c22 6e61 6d65 223a 2250 726f  6"}],"name":"Pro
+0001f890: 746f 636f 6c46 6565 7343 6f6c 6c65 6374  tocolFeesCollect
+0001f8a0: 6564 222c 2274 7970 6522 3a22 6576 656e  ed","type":"even
+0001f8b0: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+0001f8c0: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+0001f8d0: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+0001f8e0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001f8f0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001f900: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
+0001f910: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001f920: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
+0001f930: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001f940: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
+0001f950: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+0001f960: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+0001f970: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0001f980: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001f990: 3622 2c22 6e61 6d65 223a 2269 6422 2c22  6","name":"id","
+0001f9a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001f9b0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001f9c0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f9d0: 3a22 626f 6f6c 222c 226e 616d 6522 3a22  :"bool","name":"
+0001f9e0: 7377 6170 466f 7259 222c 2274 7970 6522  swapForY","type"
+0001f9f0: 3a22 626f 6f6c 227d 2c7b 2269 6e64 6578  :"bool"},{"index
+0001fa00: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+0001fa10: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001fa20: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0001fa30: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
+0001fa40: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+0001fa50: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+0001fa60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001fa70: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
+0001fa80: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
+0001fa90: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
+0001faa0: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
+0001fab0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001fac0: 226e 616d 6522 3a22 766f 6c61 7469 6c69  "name":"volatili
+0001fad0: 7479 4163 6375 6d75 6c61 7465 6422 2c22  tyAccumulated","
+0001fae0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001faf0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001fb00: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001fb10: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001fb20: 223a 2266 6565 7322 2c22 7479 7065 223a  ":"fees","type":
+0001fb30: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+0001fb40: 6522 3a22 5377 6170 222c 2274 7970 6522  e":"Swap","type"
+0001fb50: 3a22 6576 656e 7422 7d2c 7b22 616e 6f6e  :"event"},{"anon
+0001fb60: 796d 6f75 7322 3a66 616c 7365 2c22 696e  ymous":false,"in
+0001fb70: 7075 7473 223a 5b7b 2269 6e64 6578 6564  puts":[{"indexed
+0001fb80: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+0001fb90: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001fba0: 226e 616d 6522 3a22 7365 6e64 6572 222c  "name":"sender",
+0001fbb0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001fbc0: 7d2c 7b22 696e 6465 7865 6422 3a74 7275  },{"indexed":tru
+0001fbd0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001fbe0: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0001fbf0: 223a 2266 726f 6d22 2c22 7479 7065 223a  ":"from","type":
+0001fc00: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+0001fc10: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+0001fc20: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001fc30: 7373 222c 226e 616d 6522 3a22 746f 222c  ss","name":"to",
+0001fc40: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001fc50: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+0001fc60: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+0001fc70: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001fc80: 616d 6522 3a22 6964 7322 2c22 7479 7065  ame":"ids","type
+0001fc90: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
+0001fca0: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+0001fcb0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001fcc0: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+0001fcd0: 223a 2261 6d6f 756e 7473 222c 2274 7970  ":"amounts","typ
+0001fce0: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
+0001fcf0: 2c22 6e61 6d65 223a 2254 7261 6e73 6665  ,"name":"Transfe
+0001fd00: 7242 6174 6368 222c 2274 7970 6522 3a22  rBatch","type":"
+0001fd10: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
+0001fd20: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
+0001fd30: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
+0001fd40: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+0001fd50: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0001fd60: 616d 6522 3a22 7365 6e64 6572 222c 2274  ame":"sender","t
+0001fd70: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0001fd80: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
+0001fd90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001fda0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0001fdb0: 2266 726f 6d22 2c22 7479 7065 223a 2261  "from","type":"a
+0001fdc0: 6464 7265 7373 227d 2c7b 2269 6e64 6578  ddress"},{"index
+0001fdd0: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
+0001fde0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0001fdf0: 222c 226e 616d 6522 3a22 746f 222c 2274  ","name":"to","t
+0001fe00: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0001fe10: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
+0001fe20: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001fe30: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001fe40: 3a22 6964 222c 2274 7970 6522 3a22 7569  :"id","type":"ui
+0001fe50: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+0001fe60: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+0001fe70: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001fe80: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+0001fe90: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001fea0: 3622 7d5d 2c22 6e61 6d65 223a 2254 7261  6"}],"name":"Tra
+0001feb0: 6e73 6665 7253 696e 676c 6522 2c22 7479  nsferSingle","ty
+0001fec0: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
+0001fed0: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
+0001fee0: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
+0001fef0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0001ff00: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0001ff10: 7322 2c22 6e61 6d65 223a 2273 656e 6465  s","name":"sende
+0001ff20: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
+0001ff30: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
+0001ff40: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+0001ff50: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0001ff60: 616d 6522 3a22 7265 6369 7069 656e 7422  ame":"recipient"
+0001ff70: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001ff80: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0001ff90: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0001ffa0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001ffb0: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
+0001ffc0: 7569 6e74 3235 3622 7d2c 7b22 696e 6465  uint256"},{"inde
+0001ffd0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
+0001ffe0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001fff0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+00020000: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
+00020010: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+00020020: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+00020030: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00020040: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
+00020050: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00020060: 3622 7d5d 2c22 6e61 6d65 223a 2257 6974  6"}],"name":"Wit
+00020070: 6864 7261 776e 4672 6f6d 4269 6e22 2c22  hdrawnFromBin","
+00020080: 7479 7065 223a 2265 7665 6e74 227d 2c7b  type":"event"},{
+00020090: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+000200a0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+000200b0: 7373 222c 226e 616d 6522 3a22 5f61 6363  ss","name":"_acc
+000200c0: 6f75 6e74 222c 2274 7970 6522 3a22 6164  ount","type":"ad
+000200d0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+000200e0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000200f0: 222c 226e 616d 6522 3a22 5f69 6422 2c22  ","name":"_id","
+00020100: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00020110: 5d2c 226e 616d 6522 3a22 6261 6c61 6e63  ],"name":"balanc
+00020120: 654f 6622 2c22 6f75 7470 7574 7322 3a5b  eOf","outputs":[
+00020130: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00020140: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00020150: 3a22 222c 2274 7970 6522 3a22 7569 6e74  :"","type":"uint
+00020160: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+00020170: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00020180: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00020190: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+000201a0: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+000201b0: 6464 7265 7373 5b5d 222c 226e 616d 6522  ddress[]","name"
+000201c0: 3a22 5f61 6363 6f75 6e74 7322 2c22 7479  :"_accounts","ty
+000201d0: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
+000201e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+000201f0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+00020200: 6d65 223a 225f 6964 7322 2c22 7479 7065  me":"_ids","type
+00020210: 223a 2275 696e 7432 3536 5b5d 227d 5d2c  ":"uint256[]"}],
+00020220: 226e 616d 6522 3a22 6261 6c61 6e63 654f  "name":"balanceO
+00020230: 6642 6174 6368 222c 226f 7574 7075 7473  fBatch","outputs
+00020240: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00020250: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+00020260: 6e61 6d65 223a 2262 6174 6368 4261 6c61  name":"batchBala
+00020270: 6e63 6573 222c 2274 7970 6522 3a22 7569  nces","type":"ui
+00020280: 6e74 3235 365b 5d22 7d5d 2c22 7374 6174  nt256[]"}],"stat
+00020290: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+000202a0: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+000202b0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+000202c0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+000202d0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+000202e0: 616d 6522 3a22 5f69 6473 222c 2274 7970  ame":"_ids","typ
+000202f0: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+00020300: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00020310: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+00020320: 6522 3a22 5f61 6d6f 756e 7473 222c 2274  e":"_amounts","t
+00020330: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+00020340: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020350: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00020360: 6522 3a22 5f74 6f22 2c22 7479 7065 223a  e":"_to","type":
+00020370: 2261 6464 7265 7373 227d 5d2c 226e 616d  "address"}],"nam
+00020380: 6522 3a22 6275 726e 222c 226f 7574 7075  e":"burn","outpu
+00020390: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+000203a0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+000203b0: 6e61 6d65 223a 2261 6d6f 756e 7458 222c  name":"amountX",
+000203c0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000203d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000203e0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+000203f0: 6522 3a22 616d 6f75 6e74 5922 2c22 7479  e":"amountY","ty
+00020400: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00020410: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00020420: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+00020430: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00020440: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00020450: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+00020460: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
+00020470: 6163 636f 756e 7422 2c22 7479 7065 223a  account","type":
+00020480: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00020490: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000204a0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
+000204b0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
+000204c0: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
+000204d0: 3a22 636f 6c6c 6563 7446 6565 7322 2c22  :"collectFees","
+000204e0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+000204f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00020500: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+00020510: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
+00020520: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00020530: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00020540: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
+00020550: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00020560: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
+00020570: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
+00020580: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+00020590: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+000205a0: 3a5b 5d2c 226e 616d 6522 3a22 636f 6c6c  :[],"name":"coll
+000205b0: 6563 7450 726f 746f 636f 6c46 6565 7322  ectProtocolFees"
+000205c0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+000205d0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+000205e0: 7431 3238 222c 226e 616d 6522 3a22 616d  t128","name":"am
+000205f0: 6f75 6e74 5822 2c22 7479 7065 223a 2275  ountX","type":"u
+00020600: 696e 7431 3238 227d 2c7b 2269 6e74 6572  int128"},{"inter
+00020610: 6e61 6c54 7970 6522 3a22 7569 6e74 3132  nalType":"uint12
+00020620: 3822 2c22 6e61 6d65 223a 2261 6d6f 756e  8","name":"amoun
+00020630: 7459 222c 2274 7970 6522 3a22 7569 6e74  tY","type":"uint
+00020640: 3132 3822 7d5d 2c22 7374 6174 654d 7574  128"}],"stateMut
+00020650: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+00020660: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
+00020670: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00020680: 7322 3a5b 5d2c 226e 616d 6522 3a22 6661  s":[],"name":"fa
+00020690: 6374 6f72 7922 2c22 6f75 7470 7574 7322  ctory","outputs"
+000206a0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+000206b0: 223a 2263 6f6e 7472 6163 7420 494c 4246  ":"contract ILBF
+000206c0: 6163 746f 7279 222c 226e 616d 6522 3a22  actory","name":"
+000206d0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000206e0: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
+000206f0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00020700: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00020710: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00020720: 616d 6522 3a22 6665 6550 6172 616d 6574  ame":"feeParamet
+00020730: 6572 7322 2c22 6f75 7470 7574 7322 3a5b  ers","outputs":[
+00020740: 7b22 636f 6d70 6f6e 656e 7473 223a 5b7b  {"components":[{
+00020750: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00020760: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
+00020770: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
+00020780: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
+00020790: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
+000207a0: 3622 2c22 6e61 6d65 223a 2262 6173 6546  6","name":"baseF
+000207b0: 6163 746f 7222 2c22 7479 7065 223a 2275  actor","type":"u
+000207c0: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
+000207d0: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+000207e0: 2c22 6e61 6d65 223a 2266 696c 7465 7250  ,"name":"filterP
+000207f0: 6572 696f 6422 2c22 7479 7065 223a 2275  eriod","type":"u
+00020800: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
+00020810: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+00020820: 2c22 6e61 6d65 223a 2264 6563 6179 5065  ,"name":"decayPe
+00020830: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
+00020840: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+00020850: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
+00020860: 226e 616d 6522 3a22 7265 6475 6374 696f  "name":"reductio
+00020870: 6e46 6163 746f 7222 2c22 7479 7065 223a  nFactor","type":
+00020880: 2275 696e 7431 3622 7d2c 7b22 696e 7465  "uint16"},{"inte
+00020890: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+000208a0: 3422 2c22 6e61 6d65 223a 2276 6172 6961  4","name":"varia
+000208b0: 626c 6546 6565 436f 6e74 726f 6c22 2c22  bleFeeControl","
+000208c0: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
+000208d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000208e0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
+000208f0: 2270 726f 746f 636f 6c53 6861 7265 222c  "protocolShare",
+00020900: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00020910: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00020920: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
+00020930: 3a22 6d61 7856 6f6c 6174 696c 6974 7941  :"maxVolatilityA
+00020940: 6363 756d 756c 6174 6564 222c 2274 7970  ccumulated","typ
+00020950: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
+00020960: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00020970: 6e74 3234 222c 226e 616d 6522 3a22 766f  nt24","name":"vo
+00020980: 6c61 7469 6c69 7479 4163 6375 6d75 6c61  latilityAccumula
+00020990: 7465 6422 2c22 7479 7065 223a 2275 696e  ted","type":"uin
+000209a0: 7432 3422 7d2c 7b22 696e 7465 726e 616c  t24"},{"internal
+000209b0: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
+000209c0: 6e61 6d65 223a 2276 6f6c 6174 696c 6974  name":"volatilit
+000209d0: 7952 6566 6572 656e 6365 222c 2274 7970  yReference","typ
+000209e0: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
+000209f0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00020a00: 6e74 3234 222c 226e 616d 6522 3a22 696e  nt24","name":"in
+00020a10: 6465 7852 6566 222c 2274 7970 6522 3a22  dexRef","type":"
+00020a20: 7569 6e74 3234 227d 2c7b 2269 6e74 6572  uint24"},{"inter
+00020a30: 6e61 6c54 7970 6522 3a22 7569 6e74 3430  nalType":"uint40
+00020a40: 222c 226e 616d 6522 3a22 7469 6d65 222c  ","name":"time",
+00020a50: 2274 7970 6522 3a22 7569 6e74 3430 227d  "type":"uint40"}
+00020a60: 5d2c 2269 6e74 6572 6e61 6c54 7970 6522  ],"internalType"
+00020a70: 3a22 7374 7275 6374 2046 6565 4865 6c70  :"struct FeeHelp
+00020a80: 6572 2e46 6565 5061 7261 6d65 7465 7273  er.FeeParameters
+00020a90: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+00020aa0: 6522 3a22 7475 706c 6522 7d5d 2c22 7374  e":"tuple"}],"st
+00020ab0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00020ac0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+00020ad0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00020ae0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00020af0: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
+00020b00: 6d65 223a 225f 6964 222c 2274 7970 6522  me":"_id","type"
+00020b10: 3a22 7569 6e74 3234 227d 2c7b 2269 6e74  :"uint24"},{"int
+00020b20: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
+00020b30: 222c 226e 616d 6522 3a22 5f73 7761 7046  ","name":"_swapF
+00020b40: 6f72 5922 2c22 7479 7065 223a 2262 6f6f  orY","type":"boo
+00020b50: 6c22 7d5d 2c22 6e61 6d65 223a 2266 696e  l"}],"name":"fin
+00020b60: 6446 6972 7374 4e6f 6e45 6d70 7479 4269  dFirstNonEmptyBi
+00020b70: 6e49 6422 2c22 6f75 7470 7574 7322 3a5b  nId","outputs":[
+00020b80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00020b90: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
+00020ba0: 2222 2c22 7479 7065 223a 2275 696e 7432  "","type":"uint2
+00020bb0: 3422 7d5d 2c22 7374 6174 654d 7574 6162  4"}],"stateMutab
+00020bc0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00020bd0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00020be0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00020bf0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00020c00: 7472 6163 7420 494c 4246 6c61 7368 4c6f  tract ILBFlashLo
+00020c10: 616e 4361 6c6c 6261 636b 222c 226e 616d  anCallback","nam
+00020c20: 6522 3a22 5f72 6563 6569 7665 7222 2c22  e":"_receiver","
+00020c30: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00020c40: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00020c50: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+00020c60: 3022 2c22 6e61 6d65 223a 225f 746f 6b65  0","name":"_toke
+00020c70: 6e22 2c22 7479 7065 223a 2261 6464 7265  n","type":"addre
+00020c80: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00020c90: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00020ca0: 6e61 6d65 223a 225f 616d 6f75 6e74 222c  name":"_amount",
+00020cb0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00020cc0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020cd0: 223a 2262 7974 6573 222c 226e 616d 6522  ":"bytes","name"
+00020ce0: 3a22 5f64 6174 6122 2c22 7479 7065 223a  :"_data","type":
+00020cf0: 2262 7974 6573 227d 5d2c 226e 616d 6522  "bytes"}],"name"
+00020d00: 3a22 666c 6173 684c 6f61 6e22 2c22 6f75  :"flashLoan","ou
+00020d10: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00020d20: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00020d30: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+00020d40: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00020d50: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+00020d60: 2266 6f72 6365 4465 6361 7922 2c22 6f75  "forceDecay","ou
+00020d70: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00020d80: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00020d90: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+00020da0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00020db0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00020dc0: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+00020dd0: 226e 616d 6522 3a22 5f69 6422 2c22 7479  "name":"_id","ty
+00020de0: 7065 223a 2275 696e 7432 3422 7d5d 2c22  pe":"uint24"}],"
+00020df0: 6e61 6d65 223a 2267 6574 4269 6e22 2c22  name":"getBin","
+00020e00: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00020e10: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00020e20: 3536 222c 226e 616d 6522 3a22 7265 7365  56","name":"rese
+00020e30: 7276 6558 222c 2274 7970 6522 3a22 7569  rveX","type":"ui
+00020e40: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+00020e50: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00020e60: 222c 226e 616d 6522 3a22 7265 7365 7276  ","name":"reserv
+00020e70: 6559 222c 2274 7970 6522 3a22 7569 6e74  eY","type":"uint
+00020e80: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+00020e90: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00020ea0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00020eb0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00020ec0: 226e 616d 6522 3a22 6765 7447 6c6f 6261  "name":"getGloba
+00020ed0: 6c46 6565 7322 2c22 6f75 7470 7574 7322  lFees","outputs"
+00020ee0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00020ef0: 223a 2275 696e 7431 3238 222c 226e 616d  ":"uint128","nam
+00020f00: 6522 3a22 6665 6573 5854 6f74 616c 222c  e":"feesXTotal",
+00020f10: 2274 7970 6522 3a22 7569 6e74 3132 3822  "type":"uint128"
+00020f20: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020f30: 223a 2275 696e 7431 3238 222c 226e 616d  ":"uint128","nam
+00020f40: 6522 3a22 6665 6573 5954 6f74 616c 222c  e":"feesYTotal",
+00020f50: 2274 7970 6522 3a22 7569 6e74 3132 3822  "type":"uint128"
+00020f60: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020f70: 223a 2275 696e 7431 3238 222c 226e 616d  ":"uint128","nam
+00020f80: 6522 3a22 6665 6573 5850 726f 746f 636f  e":"feesXProtoco
+00020f90: 6c22 2c22 7479 7065 223a 2275 696e 7431  l","type":"uint1
+00020fa0: 3238 227d 2c7b 2269 6e74 6572 6e61 6c54  28"},{"internalT
+00020fb0: 7970 6522 3a22 7569 6e74 3132 3822 2c22  ype":"uint128","
+00020fc0: 6e61 6d65 223a 2266 6565 7359 5072 6f74  name":"feesYProt
+00020fd0: 6f63 6f6c 222c 2274 7970 6522 3a22 7569  ocol","type":"ui
+00020fe0: 6e74 3132 3822 7d5d 2c22 7374 6174 654d  nt128"}],"stateM
+00020ff0: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+00021000: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00021010: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00021020: 5d2c 226e 616d 6522 3a22 6765 744f 7261  ],"name":"getOra
+00021030: 636c 6550 6172 616d 6574 6572 7322 2c22  cleParameters","
+00021040: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00021050: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00021060: 3536 222c 226e 616d 6522 3a22 6f72 6163  56","name":"orac
+00021070: 6c65 5361 6d70 6c65 4c69 6665 7469 6d65  leSampleLifetime
+00021080: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021090: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+000210a0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000210b0: 616d 6522 3a22 6f72 6163 6c65 5369 7a65  ame":"oracleSize
+000210c0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+000210d0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+000210e0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000210f0: 616d 6522 3a22 6f72 6163 6c65 4163 7469  ame":"oracleActi
+00021100: 7665 5369 7a65 222c 2274 7970 6522 3a22  veSize","type":"
+00021110: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00021120: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00021130: 3536 222c 226e 616d 6522 3a22 6f72 6163  56","name":"orac
+00021140: 6c65 4c61 7374 5469 6d65 7374 616d 7022  leLastTimestamp"
+00021150: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00021160: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00021170: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00021180: 6d65 223a 226f 7261 636c 6549 6422 2c22  me":"oracleId","
+00021190: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+000211a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+000211b0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+000211c0: 223a 226d 696e 222c 2274 7970 6522 3a22  ":"min","type":"
+000211d0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+000211e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+000211f0: 3536 222c 226e 616d 6522 3a22 6d61 7822  56","name":"max"
+00021200: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00021210: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
+00021220: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
+00021230: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+00021240: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00021250: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00021260: 3235 3622 2c22 6e61 6d65 223a 225f 7469  256","name":"_ti
+00021270: 6d65 4465 6c74 6122 2c22 7479 7065 223a  meDelta","type":
+00021280: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00021290: 6522 3a22 6765 744f 7261 636c 6553 616d  e":"getOracleSam
+000212a0: 706c 6546 726f 6d22 2c22 6f75 7470 7574  pleFrom","output
+000212b0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+000212c0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000212d0: 616d 6522 3a22 6375 6d75 6c61 7469 7665  ame":"cumulative
+000212e0: 4964 222c 2274 7970 6522 3a22 7569 6e74  Id","type":"uint
+000212f0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+00021300: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+00021310: 226e 616d 6522 3a22 6375 6d75 6c61 7469  "name":"cumulati
+00021320: 7665 566f 6c61 7469 6c69 7479 4163 6375  veVolatilityAccu
+00021330: 6d75 6c61 7465 6422 2c22 7479 7065 223a  mulated","type":
+00021340: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00021350: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00021360: 3235 3622 2c22 6e61 6d65 223a 2263 756d  256","name":"cum
+00021370: 756c 6174 6976 6542 696e 4372 6f73 7365  ulativeBinCrosse
+00021380: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
+00021390: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
+000213a0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+000213b0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+000213c0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+000213d0: 6e61 6d65 223a 2267 6574 5265 7365 7276  name":"getReserv
+000213e0: 6573 416e 6449 6422 2c22 6f75 7470 7574  esAndId","output
+000213f0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00021400: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00021410: 616d 6522 3a22 7265 7365 7276 6558 222c  ame":"reserveX",
+00021420: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00021430: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00021440: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00021450: 6522 3a22 7265 7365 7276 6559 222c 2274  e":"reserveY","t
+00021460: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00021470: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021480: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00021490: 3a22 6163 7469 7665 4964 222c 2274 7970  :"activeId","typ
+000214a0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+000214b0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+000214c0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+000214d0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+000214e0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+000214f0: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
+00021500: 6e61 6d65 223a 225f 6e65 774c 656e 6774  name":"_newLengt
+00021510: 6822 2c22 7479 7065 223a 2275 696e 7431  h","type":"uint1
+00021520: 3622 7d5d 2c22 6e61 6d65 223a 2269 6e63  6"}],"name":"inc
+00021530: 7265 6173 654f 7261 636c 654c 656e 6774  reaseOracleLengt
+00021540: 6822 2c22 6f75 7470 7574 7322 3a5b 5d2c  h","outputs":[],
+00021550: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00021560: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+00021570: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00021580: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00021590: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+000215a0: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
+000215b0: 6e61 6d65 223a 225f 746f 6b65 6e58 222c  name":"_tokenX",
+000215c0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+000215d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000215e0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
+000215f0: 3230 222c 226e 616d 6522 3a22 5f74 6f6b  20","name":"_tok
+00021600: 656e 5922 2c22 7479 7065 223a 2261 6464  enY","type":"add
+00021610: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+00021620: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+00021630: 226e 616d 6522 3a22 5f61 6374 6976 6549  "name":"_activeI
+00021640: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
+00021650: 3422 7d2c 7b22 696e 7465 726e 616c 5479  4"},{"internalTy
+00021660: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
+00021670: 6d65 223a 225f 7361 6d70 6c65 4c69 6665  me":"_sampleLife
+00021680: 7469 6d65 222c 2274 7970 6522 3a22 7569  time","type":"ui
+00021690: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+000216a0: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
+000216b0: 2c22 6e61 6d65 223a 225f 7061 636b 6564  ,"name":"_packed
+000216c0: 4665 6550 6172 616d 6574 6572 7322 2c22  FeeParameters","
+000216d0: 7479 7065 223a 2262 7974 6573 3332 227d  type":"bytes32"}
+000216e0: 5d2c 226e 616d 6522 3a22 696e 6974 6961  ],"name":"initia
+000216f0: 6c69 7a65 222c 226f 7574 7075 7473 223a  lize","outputs":
+00021700: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+00021710: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+00021720: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00021730: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00021740: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021750: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00021760: 3a22 5f6f 776e 6572 222c 2274 7970 6522  :"_owner","type"
+00021770: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+00021780: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00021790: 7265 7373 222c 226e 616d 6522 3a22 5f73  ress","name":"_s
+000217a0: 7065 6e64 6572 222c 2274 7970 6522 3a22  pender","type":"
+000217b0: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+000217c0: 223a 2269 7341 7070 726f 7665 6446 6f72  ":"isApprovedFor
+000217d0: 416c 6c22 2c22 6f75 7470 7574 7322 3a5b  All","outputs":[
+000217e0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000217f0: 2262 6f6f 6c22 2c22 6e61 6d65 223a 2222  "bool","name":""
+00021800: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
+00021810: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00021820: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+00021830: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00021840: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00021850: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00021860: 5b5d 222c 226e 616d 6522 3a22 5f69 6473  []","name":"_ids
+00021870: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021880: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+00021890: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
+000218a0: 222c 226e 616d 6522 3a22 5f64 6973 7472  ","name":"_distr
+000218b0: 6962 7574 696f 6e58 222c 2274 7970 6522  ibutionX","type"
+000218c0: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
+000218d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000218e0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+000218f0: 3a22 5f64 6973 7472 6962 7574 696f 6e59  :"_distributionY
+00021900: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021910: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+00021920: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00021930: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
+00021940: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+00021950: 226e 616d 6522 3a22 6d69 6e74 222c 226f  "name":"mint","o
+00021960: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+00021970: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00021980: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
+00021990: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+000219a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000219b0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+000219c0: 2222 2c22 7479 7065 223a 2275 696e 7432  "","type":"uint2
+000219d0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+000219e0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+000219f0: 2c22 6e61 6d65 223a 226c 6971 7569 6469  ,"name":"liquidi
+00021a00: 7479 4d69 6e74 6564 222c 2274 7970 6522  tyMinted","type"
+00021a10: 3a22 7569 6e74 3235 365b 5d22 7d5d 2c22  :"uint256[]"}],"
+00021a20: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00021a30: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00021a40: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00021a50: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00021a60: 616d 6522 3a22 6e61 6d65 222c 226f 7574  ame":"name","out
+00021a70: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00021a80: 6c54 7970 6522 3a22 7374 7269 6e67 222c  lType":"string",
+00021a90: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+00021aa0: 3a22 7374 7269 6e67 227d 5d2c 2273 7461  :"string"}],"sta
+00021ab0: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
+00021ac0: 7572 6522 2c22 7479 7065 223a 2266 756e  ure","type":"fun
+00021ad0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+00021ae0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00021af0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+00021b00: 6d65 223a 225f 6163 636f 756e 7422 2c22  me":"_account","
+00021b10: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00021b20: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00021b30: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+00021b40: 6d65 223a 225f 6964 7322 2c22 7479 7065  me":"_ids","type
+00021b50: 223a 2275 696e 7432 3536 5b5d 227d 5d2c  ":"uint256[]"}],
+00021b60: 226e 616d 6522 3a22 7065 6e64 696e 6746  "name":"pendingF
+00021b70: 6565 7322 2c22 6f75 7470 7574 7322 3a5b  ees","outputs":[
+00021b80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021b90: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00021ba0: 3a22 616d 6f75 6e74 5822 2c22 7479 7065  :"amountX","type
+00021bb0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00021bc0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00021bd0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+00021be0: 6d6f 756e 7459 222c 2274 7970 6522 3a22  mountY","type":"
+00021bf0: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
+00021c00: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+00021c10: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+00021c20: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+00021c30: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00021c40: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00021c50: 6522 3a22 5f66 726f 6d22 2c22 7479 7065  e":"_from","type
+00021c60: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00021c70: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+00021c80: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
+00021c90: 746f 222c 2274 7970 6522 3a22 6164 6472  to","type":"addr
+00021ca0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+00021cb0: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
+00021cc0: 222c 226e 616d 6522 3a22 5f69 6473 222c  ","name":"_ids",
+00021cd0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
+00021ce0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+00021cf0: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+00021d00: 226e 616d 6522 3a22 5f61 6d6f 756e 7473  "name":"_amounts
+00021d10: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021d20: 365b 5d22 7d5d 2c22 6e61 6d65 223a 2273  6[]"}],"name":"s
+00021d30: 6166 6542 6174 6368 5472 616e 7366 6572  afeBatchTransfer
+00021d40: 4672 6f6d 222c 226f 7574 7075 7473 223a  From","outputs":
+00021d50: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+00021d60: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+00021d70: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00021d80: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00021d90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021da0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00021db0: 3a22 5f66 726f 6d22 2c22 7479 7065 223a  :"_from","type":
+00021dc0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00021dd0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+00021de0: 6573 7322 2c22 6e61 6d65 223a 225f 746f  ess","name":"_to
+00021df0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00021e00: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+00021e10: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00021e20: 616d 6522 3a22 5f69 6422 2c22 7479 7065  ame":"_id","type
+00021e30: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00021e40: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00021e50: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+00021e60: 616d 6f75 6e74 222c 2274 7970 6522 3a22  amount","type":"
+00021e70: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+00021e80: 223a 2273 6166 6554 7261 6e73 6665 7246  ":"safeTransferF
+00021e90: 726f 6d22 2c22 6f75 7470 7574 7322 3a5b  rom","outputs":[
+00021ea0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00021eb0: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+00021ec0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00021ed0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00021ee0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00021ef0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+00021f00: 225f 7370 656e 6465 7222 2c22 7479 7065  "_spender","type
+00021f10: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00021f20: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
+00021f30: 6f6c 222c 226e 616d 6522 3a22 5f61 7070  ol","name":"_app
+00021f40: 726f 7665 6422 2c22 7479 7065 223a 2262  roved","type":"b
+00021f50: 6f6f 6c22 7d5d 2c22 6e61 6d65 223a 2273  ool"}],"name":"s
+00021f60: 6574 4170 7072 6f76 616c 466f 7241 6c6c  etApprovalForAll
+00021f70: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+00021f80: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00021f90: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00021fa0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00021fb0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00021fc0: 7465 726e 616c 5479 7065 223a 2262 7974  ternalType":"byt
+00021fd0: 6573 3332 222c 226e 616d 6522 3a22 5f70  es32","name":"_p
+00021fe0: 6163 6b65 6446 6565 5061 7261 6d65 7465  ackedFeeParamete
+00021ff0: 7273 222c 2274 7970 6522 3a22 6279 7465  rs","type":"byte
+00022000: 7333 3222 7d5d 2c22 6e61 6d65 223a 2273  s32"}],"name":"s
+00022010: 6574 4665 6573 5061 7261 6d65 7465 7273  etFeesParameters
+00022020: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+00022030: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00022040: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00022050: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00022060: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00022070: 7465 726e 616c 5479 7065 223a 2262 7974  ternalType":"byt
+00022080: 6573 3422 2c22 6e61 6d65 223a 225f 696e  es4","name":"_in
+00022090: 7465 7266 6163 6549 6422 2c22 7479 7065  terfaceId","type
+000220a0: 223a 2262 7974 6573 3422 7d5d 2c22 6e61  ":"bytes4"}],"na
+000220b0: 6d65 223a 2273 7570 706f 7274 7349 6e74  me":"supportsInt
+000220c0: 6572 6661 6365 222c 226f 7574 7075 7473  erface","outputs
+000220d0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+000220e0: 6522 3a22 626f 6f6c 222c 226e 616d 6522  e":"bool","name"
+000220f0: 3a22 222c 2274 7970 6522 3a22 626f 6f6c  :"","type":"bool
+00022100: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
+00022110: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
+00022120: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+00022130: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00022140: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
+00022150: 222c 226e 616d 6522 3a22 5f73 7761 7046  ","name":"_swapF
+00022160: 6f72 5922 2c22 7479 7065 223a 2262 6f6f  orY","type":"boo
+00022170: 6c22 7d2c 7b22 696e 7465 726e 616c 5479  l"},{"internalTy
+00022180: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+00022190: 616d 6522 3a22 5f74 6f22 2c22 7479 7065  ame":"_to","type
+000221a0: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
+000221b0: 616d 6522 3a22 7377 6170 222c 226f 7574  ame":"swap","out
+000221c0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+000221d0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+000221e0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7458  ,"name":"amountX
+000221f0: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
+00022200: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00022210: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00022220: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
+00022230: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
+00022240: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
+00022250: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
+00022260: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+00022270: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+00022280: 7473 223a 5b5d 2c22 6e61 6d65 223a 2273  ts":[],"name":"s
+00022290: 796d 626f 6c22 2c22 6f75 7470 7574 7322  ymbol","outputs"
+000222a0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+000222b0: 223a 2273 7472 696e 6722 2c22 6e61 6d65  ":"string","name
+000222c0: 223a 2222 2c22 7479 7065 223a 2273 7472  ":"","type":"str
+000222d0: 696e 6722 7d5d 2c22 7374 6174 654d 7574  ing"}],"stateMut
+000222e0: 6162 696c 6974 7922 3a22 7075 7265 222c  ability":"pure",
+000222f0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00022300: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00022310: 226e 616d 6522 3a22 746f 6b65 6e58 222c  "name":"tokenX",
+00022320: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+00022330: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+00022340: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
+00022350: 6d65 223a 2222 2c22 7479 7065 223a 2261  me":"","type":"a
+00022360: 6464 7265 7373 227d 5d2c 2273 7461 7465  ddress"}],"state
+00022370: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
+00022380: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
+00022390: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+000223a0: 5b5d 2c22 6e61 6d65 223a 2274 6f6b 656e  [],"name":"token
+000223b0: 5922 2c22 6f75 7470 7574 7322 3a5b 7b22  Y","outputs":[{"
+000223c0: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+000223d0: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+000223e0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+000223f0: 3a22 6164 6472 6573 7322 7d5d 2c22 7374  :"address"}],"st
+00022400: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00022410: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+00022420: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00022430: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00022440: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00022450: 616d 6522 3a22 5f69 6422 2c22 7479 7065  ame":"_id","type
+00022460: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00022470: 616d 6522 3a22 746f 7461 6c53 7570 706c  ame":"totalSuppl
+00022480: 7922 2c22 6f75 7470 7574 7322 3a5b 7b22  y","outputs":[{"
+00022490: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000224a0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000224b0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+000224c0: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
+000224d0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+000224e0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+000224f0: 5d27 290a 0a20 2020 2023 2072 6574 7572  ]')..    # retur
+00022500: 6e73 2028 7569 6e74 3235 3620 7265 7365  ns (uint256 rese
+00022510: 7276 6558 2c20 7569 6e74 3235 3620 7265  rveX, uint256 re
+00022520: 7365 7276 6559 2c20 7569 6e74 3235 3620  serveY, uint256 
+00022530: 6163 7469 7665 4964 290a 2020 2020 6465  activeId).    de
+00022540: 6620 6765 745f 7265 7365 7276 655f 616e  f get_reserve_an
+00022550: 645f 6964 285f 7765 6233 3a57 6562 332c  d_id(_web3:Web3,
+00022560: 5f70 6169 725f 6164 6472 6573 733a 7374  _pair_address:st
+00022570: 7229 3a0a 2020 2020 2020 2020 7061 6972  r):.        pair
+00022580: 5f63 6f6e 7472 6163 743d 5f77 6562 332e  _contract=_web3.
+00022590: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+000225a0: 7265 7373 3d5f 7061 6972 5f61 6464 7265  ress=_pair_addre
+000225b0: 7373 2c20 6162 693d 4a6f 6556 3250 6169  ss, abi=JoeV2Pai
+000225c0: 722e 6a6f 655f 7061 6972 5f76 325f 6162  r.joe_pair_v2_ab
+000225d0: 6929 0a20 2020 2020 2020 2072 6574 7572  i).        retur
+000225e0: 6e20 7061 6972 5f63 6f6e 7472 6163 742e  n pair_contract.
+000225f0: 6675 6e63 7469 6f6e 732e 6765 7452 6573  functions.getRes
+00022600: 6572 7665 7341 6e64 4964 2829 2e63 616c  ervesAndId().cal
+00022610: 6c28 290a 0a20 2020 2023 2066 756e 6374  l()..    # funct
+00022620: 696f 6e20 6765 7447 6c6f 6261 6c46 6565  ion getGlobalFee
+00022630: 7328 2920 6578 7465 726e 616c 2076 6965  s() external vie
+00022640: 7720 6f76 6572 7269 6465 2072 6574 7572  w override retur
+00022650: 6e73 2028 7569 6e74 3235 3620 6665 6573  ns (uint256 fees
+00022660: 5854 6f74 616c 2c20 7569 6e74 3235 3620  XTotal, uint256 
+00022670: 6665 6573 5954 6f74 616c 2c20 7569 6e74  feesYTotal, uint
+00022680: 3235 3620 6665 6573 5850 726f 746f 636f  256 feesXProtoco
+00022690: 6c2c 2075 696e 7432 3536 2066 6565 7359  l, uint256 feesY
+000226a0: 5072 6f74 6f63 6f6c 290a 2020 2020 6465  Protocol).    de
+000226b0: 6620 6765 745f 676c 6f62 616c 5f66 6565  f get_global_fee
+000226c0: 285f 7765 6233 3a57 6562 332c 5f70 6169  (_web3:Web3,_pai
+000226d0: 725f 6164 6472 6573 733a 7374 7229 3a0a  r_address:str):.
+000226e0: 2020 2020 2020 2020 7061 6972 5f63 6f6e          pair_con
+000226f0: 7472 6163 743d 5f77 6562 332e 6574 682e  tract=_web3.eth.
+00022700: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
+00022710: 3d5f 7061 6972 5f61 6464 7265 7373 2c20  =_pair_address, 
+00022720: 6162 693d 4a6f 6556 3250 6169 722e 6a6f  abi=JoeV2Pair.jo
+00022730: 655f 7061 6972 5f76 325f 6162 6929 0a20  e_pair_v2_abi). 
+00022740: 2020 2020 2020 2072 6574 7572 6e20 7061         return pa
+00022750: 6972 5f63 6f6e 7472 6163 742e 6675 6e63  ir_contract.func
+00022760: 7469 6f6e 732e 6765 7447 6c6f 6261 6c46  tions.getGlobalF
+00022770: 6565 7328 292e 6361 6c6c 2829 0a0a 2020  ees().call()..  
+00022780: 2020 2320 6675 6e63 7469 6f6e 2066 696e    # function fin
+00022790: 6446 6972 7374 4e6f 6e45 6d70 7479 4269  dFirstNonEmptyBi
+000227a0: 6e49 6428 7569 6e74 3234 205f 6964 2c20  nId(uint24 _id, 
+000227b0: 626f 6f6c 205f 7377 6170 466f 7259 2920  bool _swapForY) 
+000227c0: 6578 7465 726e 616c 2076 6965 7720 6f76  external view ov
+000227d0: 6572 7269 6465 2072 6574 7572 6e73 2028  erride returns (
+000227e0: 7569 6e74 3234 290a 2020 2020 6465 6620  uint24).    def 
+000227f0: 6669 6e64 5f66 6972 7374 5f6e 6f6e 5f65  find_first_non_e
+00022800: 6d70 7479 5f62 696e 5f69 6428 5f77 6562  mpty_bin_id(_web
+00022810: 333a 5765 6233 2c5f 7061 6972 5f61 6464  3:Web3,_pair_add
+00022820: 7265 7373 3a73 7472 2c5f 6964 2c5f 7377  ress:str,_id,_sw
+00022830: 6170 5f66 6f72 5f79 293a 0a20 2020 2020  ap_for_y):.     
+00022840: 2020 2070 6169 725f 636f 6e74 7261 6374     pair_contract
+00022850: 3d5f 7765 6233 2e65 7468 2e63 6f6e 7472  =_web3.eth.contr
+00022860: 6163 7428 6164 6472 6573 733d 5f70 6169  act(address=_pai
+00022870: 725f 6164 6472 6573 732c 2061 6269 3d4a  r_address, abi=J
+00022880: 6f65 5632 5061 6972 2e6a 6f65 5f70 6169  oeV2Pair.joe_pai
+00022890: 725f 7632 5f61 6269 290a 2020 2020 2020  r_v2_abi).      
+000228a0: 2020 7265 7475 726e 2070 6169 725f 636f    return pair_co
+000228b0: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+000228c0: 2e66 696e 6446 6972 7374 4e6f 6e45 6d70  .findFirstNonEmp
+000228d0: 7479 4269 6e49 6428 5f69 642c 5f73 7761  tyBinId(_id,_swa
+000228e0: 705f 666f 725f 7929 2e63 616c 6c28 290a  p_for_y).call().
+000228f0: 0a20 2020 2023 2066 756e 6374 696f 6e20  .    # function 
+00022900: 6765 7442 696e 2875 696e 7432 3420 5f69  getBin(uint24 _i
+00022910: 6429 2065 7874 6572 6e61 6c20 7669 6577  d) external view
+00022920: 206f 7665 7272 6964 6520 7265 7475 726e   override return
+00022930: 7320 2875 696e 7432 3536 2072 6573 6572  s (uint256 reser
+00022940: 7665 582c 2075 696e 7432 3536 2072 6573  veX, uint256 res
+00022950: 6572 7665 5929 0a20 2020 2064 6566 2067  erveY).    def g
+00022960: 6574 5f62 696e 285f 7765 6233 3a57 6562  et_bin(_web3:Web
+00022970: 332c 5f70 6169 725f 6164 6472 6573 733a  3,_pair_address:
+00022980: 7374 722c 5f69 6429 3a0a 2020 2020 2020  str,_id):.      
+00022990: 2020 7061 6972 5f63 6f6e 7472 6163 743d    pair_contract=
+000229a0: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
+000229b0: 6374 2861 6464 7265 7373 3d5f 7061 6972  ct(address=_pair
+000229c0: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
+000229d0: 6556 3250 6169 722e 6a6f 655f 7061 6972  eV2Pair.joe_pair
+000229e0: 5f76 325f 6162 6929 0a20 2020 2020 2020  _v2_abi).       
+000229f0: 2072 6574 7572 6e20 7061 6972 5f63 6f6e   return pair_con
+00022a00: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
+00022a10: 6765 7442 696e 285f 6964 292e 6361 6c6c  getBin(_id).call
+00022a20: 2829 0a0a 2020 2020 2320 6675 6e63 7469  ()..    # functi
+00022a30: 6f6e 2073 7761 7028 626f 6f6c 205f 7377  on swap(bool _sw
+00022a40: 6170 466f 7259 2c20 6164 6472 6573 7320  apForY, address 
+00022a50: 5f74 6f29 2065 7874 6572 6e61 6c20 6f76  _to) external ov
+00022a60: 6572 7269 6465 206e 6f6e 5265 656e 7472  erride nonReentr
+00022a70: 616e 7420 7265 7475 726e 7320 2875 696e  ant returns (uin
+00022a80: 7432 3536 2061 6d6f 756e 7458 4f75 742c  t256 amountXOut,
+00022a90: 2075 696e 7432 3536 2061 6d6f 756e 7459   uint256 amountY
+00022aa0: 4f75 7429 0a20 2020 2064 6566 2073 7761  Out).    def swa
+00022ab0: 7028 5f77 6562 333a 5765 6233 2c5f 7061  p(_web3:Web3,_pa
+00022ac0: 6972 5f61 6464 7265 7373 3a73 7472 2c5f  ir_address:str,_
+00022ad0: 7377 6170 5f66 6f72 5f79 2c5f 746f 293a  swap_for_y,_to):
+00022ae0: 0a20 2020 2020 2020 2070 6169 725f 636f  .        pair_co
+00022af0: 6e74 7261 6374 3d5f 7765 6233 2e65 7468  ntract=_web3.eth
+00022b00: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
+00022b10: 733d 5f70 6169 725f 6164 6472 6573 732c  s=_pair_address,
+00022b20: 2061 6269 3d4a 6f65 5632 5061 6972 2e6a   abi=JoeV2Pair.j
+00022b30: 6f65 5f70 6169 725f 7632 5f61 6269 290a  oe_pair_v2_abi).
+00022b40: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00022b50: 6169 725f 636f 6e74 7261 6374 2e66 756e  air_contract.fun
+00022b60: 6374 696f 6e73 2e73 7761 7028 5f73 7761  ctions.swap(_swa
+00022b70: 705f 666f 725f 792c 5f74 6f29 2e63 616c  p_for_y,_to).cal
+00022b80: 6c28 29                                  l()
```

### Comparing `dexhub-0.6.7/dexhub/interface/joe.py` & `dexhub-0.6.8/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub/util/helper.py` & `dexhub-0.6.8/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/dexhub.egg-info/PKG-INFO` & `dexhub-0.6.8/dexhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.7
+Version: 0.6.8
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.7/dexhub.egg-info/SOURCES.txt` & `dexhub-0.6.8/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.7/setup.py` & `dexhub-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.6.7",
+    version="0.6.8",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

