# Comparing `tmp/hydra_chain_py-2.7.6.tar.gz` & `tmp/hydra_chain_py-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_chain_py-2.7.6.tar", max compression
+gzip compressed data, was "hydra_chain_py-2.8.0.tar", max compression
```

## Comparing `hydra_chain_py-2.7.6.tar` & `hydra_chain_py-2.8.0.tar`

### file list

```diff
@@ -1,37 +1,65 @@
--rw-r--r--   0        0        0    48485 2022-10-29 18:58:47.604374 hydra_chain_py-2.7.6/LICENSE
--rw-r--r--   0        0        0     9319 2022-11-06 23:27:20.220997 hydra_chain_py-2.7.6/README.md
--rw-r--r--   0        0        0      188 2022-11-07 03:47:20.812038 hydra_chain_py-2.7.6/hydra/__init__.py
--rw-r--r--   0        0        0     7262 2022-10-29 18:58:47.604374 hydra_chain_py-2.7.6/hydra/app/__init__.py
--rw-r--r--   0        0        0     4057 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/ascan.py
--rw-r--r--   0        0        0     3592 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/atrace.py
--rw-r--r--   0        0        0     1024 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/call.py
--rw-r--r--   0        0        0     1645 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/cli.py
--rw-r--r--   0        0        0     3223 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/lstx.py
--rw-r--r--   0        0        0     2244 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/peerscan.py
--rw-r--r--   0        0        0     1359 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/test.py
--rw-r--r--   0        0        0     6444 2022-11-06 21:38:38.835516 hydra_chain_py-2.7.6/hydra/app/top.py
--rw-r--r--   0        0        0     3563 2022-10-29 18:58:47.608374 hydra_chain_py-2.7.6/hydra/app/txvio.py
--rw-r--r--   0        0        0     5531 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/hy.py
--rw-r--r--   0        0        0       51 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/kc/__init__.py
--rw-r--r--   0        0        0     2507 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/kc/prices.py
--rw-r--r--   0        0        0     2207 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/log.py
--rw-r--r--   0        0        0        0 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/res/.keep
--rw-r--r--   0        0        0       88 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/rpc/__init__.py
--rw-r--r--   0        0        0     4771 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/rpc/base.py
--rw-r--r--   0        0        0     1675 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/rpc/explorer.py
--rw-r--r--   0        0        0    20540 2022-10-29 18:58:47.612374 hydra_chain_py-2.7.6/hydra/rpc/hydra.py
--rw-r--r--   0        0        0     2069 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/__init__.py
--rw-r--r--   0        0        0      105 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/__main__.py
--rw-r--r--   0        0        0       18 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/app/__init__.py
--rw-r--r--   0        0        0      108 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/app/__main__.py
--rw-r--r--   0        0        0      255 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/app/cli.py
--rw-r--r--   0        0        0      191 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/rpc.py
--rw-r--r--   0        0        0      127 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/test/tests.py
--rw-r--r--   0        0        0      299 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/util/__init__.py
--rw-r--r--   0        0        0     1063 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/util/asyncc.py
--rw-r--r--   0        0        0      357 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/util/sha.py
--rw-r--r--   0        0        0      674 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/util/struct.py
--rw-r--r--   0        0        0     1237 2022-10-29 18:58:47.616374 hydra_chain_py-2.7.6/hydra/util/tlru.py
--rw-r--r--   0        0        0      906 2022-11-07 04:06:17.558906 hydra_chain_py-2.7.6/pyproject.toml
--rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 hydra_chain_py-2.7.6/setup.py
--rw-r--r--   0        0        0    10230 1970-01-01 00:00:00.000000 hydra_chain_py-2.7.6/PKG-INFO
+-rw-r--r--   0        0        0    48485 2022-10-29 18:58:47.604374 hydra_chain_py-2.8.0/LICENSE
+-rw-r--r--   0        0        0     9319 2022-11-06 23:27:20.220997 hydra_chain_py-2.8.0/README.md
+-rw-r--r--   0        0        0      188 2022-11-07 03:47:20.812038 hydra_chain_py-2.8.0/hydra/__init__.py
+-rw-r--r--   0        0        0     7262 2022-10-29 18:58:47.604374 hydra_chain_py-2.8.0/hydra/app/__init__.py
+-rw-r--r--   0        0        0     7367 2022-11-06 21:20:20.976303 hydra_chain_py-2.8.0/hydra/app/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13183 2023-08-06 18:53:39.085690 hydra_chain_py-2.8.0/hydra/app/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3833 2022-11-07 02:06:25.507379 hydra_chain_py-2.8.0/hydra/app/__pycache__/ascan.cpython-310.pyc
+-rw-r--r--   0        0        0     3242 2022-11-07 02:06:25.507379 hydra_chain_py-2.8.0/hydra/app/__pycache__/atrace.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2022-11-07 02:06:25.507379 hydra_chain_py-2.8.0/hydra/app/__pycache__/call.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2022-11-06 23:31:55.386859 hydra_chain_py-2.8.0/hydra/app/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0        0        0     3537 2022-11-07 02:06:25.511379 hydra_chain_py-2.8.0/hydra/app/__pycache__/lstx.cpython-310.pyc
+-rw-r--r--   0        0        0     2782 2022-11-07 02:06:25.511379 hydra_chain_py-2.8.0/hydra/app/__pycache__/peerscan.cpython-310.pyc
+-rw-r--r--   0        0        0     1501 2022-11-07 02:06:25.451380 hydra_chain_py-2.8.0/hydra/app/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5464 2022-11-07 02:06:25.511379 hydra_chain_py-2.8.0/hydra/app/__pycache__/top.cpython-310.pyc
+-rw-r--r--   0        0        0     3441 2022-11-07 02:06:25.507379 hydra_chain_py-2.8.0/hydra/app/__pycache__/txvio.cpython-310.pyc
+-rw-r--r--   0        0        0     4057 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/ascan.py
+-rw-r--r--   0        0        0     3592 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/atrace.py
+-rw-r--r--   0        0        0     1024 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/call.py
+-rw-r--r--   0        0        0     1645 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/cli.py
+-rw-r--r--   0        0        0     3223 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/lstx.py
+-rw-r--r--   0        0        0     2244 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/peerscan.py
+-rw-r--r--   0        0        0     1359 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/test.py
+-rw-r--r--   0        0        0     6444 2022-11-06 21:38:38.835516 hydra_chain_py-2.8.0/hydra/app/top.py
+-rw-r--r--   0        0        0     3563 2022-10-29 18:58:47.608374 hydra_chain_py-2.8.0/hydra/app/txvio.py
+-rw-r--r--   0        0        0     5531 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/hy.py
+-rw-r--r--   0        0        0       51 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/kc/__init__.py
+-rw-r--r--   0        0        0     2507 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/kc/prices.py
+-rw-r--r--   0        0        0     2207 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/log.py
+-rw-r--r--   0        0        0        0 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/res/.keep
+-rw-r--r--   0        0        0       88 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/rpc/__init__.py
+-rw-r--r--   0        0        0      252 2022-11-06 22:14:32.218820 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      314 2023-08-06 18:53:39.105690 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4995 2022-11-06 22:14:32.222820 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     7947 2023-08-06 18:53:39.109690 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2389 2022-11-06 22:14:32.278819 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/explorer.cpython-310.pyc
+-rw-r--r--   0        0        0     3640 2023-08-06 18:53:39.169691 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/explorer.cpython-311.pyc
+-rw-r--r--   0        0        0    25217 2022-11-06 22:14:32.278819 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/hydra.cpython-310.pyc
+-rw-r--r--   0        0        0    40006 2023-08-06 18:53:39.169691 hydra_chain_py-2.8.0/hydra/rpc/__pycache__/hydra.cpython-311.pyc
+-rw-r--r--   0        0        0     4771 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/rpc/base.py
+-rw-r--r--   0        0        0     1675 2022-10-29 18:58:47.612374 hydra_chain_py-2.8.0/hydra/rpc/explorer.py
+-rw-r--r--   0        0        0    20586 2022-11-07 09:35:01.258538 hydra_chain_py-2.8.0/hydra/rpc/hydra.py
+-rw-r--r--   0        0        0     2069 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/__init__.py
+-rw-r--r--   0        0        0      105 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/__main__.py
+-rw-r--r--   0        0        0     2647 2022-11-06 23:31:55.246862 hydra_chain_py-2.8.0/hydra/test/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      564 2022-11-06 23:31:55.386859 hydra_chain_py-2.8.0/hydra/test/__pycache__/rpc.cpython-310.pyc
+-rw-r--r--   0        0        0      196 2022-11-06 23:31:55.326861 hydra_chain_py-2.8.0/hydra/test/__pycache__/tests.cpython-310.pyc
+-rw-r--r--   0        0        0       18 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/app/__init__.py
+-rw-r--r--   0        0        0      108 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/app/__main__.py
+-rw-r--r--   0        0        0      156 2022-11-06 23:31:55.326861 hydra_chain_py-2.8.0/hydra/test/app/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      650 2022-11-06 23:31:55.326861 hydra_chain_py-2.8.0/hydra/test/app/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0        0        0      255 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/app/cli.py
+-rw-r--r--   0        0        0      191 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/rpc.py
+-rw-r--r--   0        0        0      127 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/test/tests.py
+-rw-r--r--   0        0        0      299 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/util/__init__.py
+-rw-r--r--   0        0        0      553 2022-11-06 22:14:32.262819 hydra_chain_py-2.8.0/hydra/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      780 2023-08-06 18:53:39.161691 hydra_chain_py-2.8.0/hydra/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1822 2022-11-06 22:14:32.262819 hydra_chain_py-2.8.0/hydra/util/__pycache__/asyncc.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-08-06 18:53:39.161691 hydra_chain_py-2.8.0/hydra/util/__pycache__/asyncc.cpython-311.pyc
+-rw-r--r--   0        0        0      577 2022-11-07 02:06:25.511379 hydra_chain_py-2.8.0/hydra/util/__pycache__/sha.cpython-310.pyc
+-rw-r--r--   0        0        0     1063 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/util/asyncc.py
+-rw-r--r--   0        0        0      357 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/util/sha.py
+-rw-r--r--   0        0        0      674 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/util/struct.py
+-rw-r--r--   0        0        0     1237 2022-10-29 18:58:47.616374 hydra_chain_py-2.8.0/hydra/util/tlru.py
+-rw-r--r--   0        0        0      974 2023-08-06 18:55:08.842836 hydra_chain_py-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10179 1970-01-01 00:00:00.000000 hydra_chain_py-2.8.0/PKG-INFO
```

### Comparing `hydra_chain_py-2.7.6/LICENSE` & `hydra_chain_py-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/README.md` & `hydra_chain_py-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/__init__.py` & `hydra_chain_py-2.8.0/hydra/app/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/ascan.py` & `hydra_chain_py-2.8.0/hydra/app/ascan.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/atrace.py` & `hydra_chain_py-2.8.0/hydra/app/atrace.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/call.py` & `hydra_chain_py-2.8.0/hydra/app/call.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/cli.py` & `hydra_chain_py-2.8.0/hydra/app/cli.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/lstx.py` & `hydra_chain_py-2.8.0/hydra/app/lstx.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/peerscan.py` & `hydra_chain_py-2.8.0/hydra/app/peerscan.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/test.py` & `hydra_chain_py-2.8.0/hydra/app/test.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/top.py` & `hydra_chain_py-2.8.0/hydra/app/top.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/app/txvio.py` & `hydra_chain_py-2.8.0/hydra/app/txvio.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/hy.py` & `hydra_chain_py-2.8.0/hydra/hy.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/kc/prices.py` & `hydra_chain_py-2.8.0/hydra/kc/prices.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/log.py` & `hydra_chain_py-2.8.0/hydra/log.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/rpc/base.py` & `hydra_chain_py-2.8.0/hydra/rpc/base.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/rpc/explorer.py` & `hydra_chain_py-2.8.0/hydra/rpc/explorer.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/rpc/hydra.py` & `hydra_chain_py-2.8.0/hydra/rpc/hydra.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         )
 
     def __repr__(self):
         return f"{self.__class__.__name__}(url=\"{self.url}\", wallet=\"{self.wallet}\")"
 
     @staticmethod
     def __parse_url__(url: str, testnet=False):
+        # TODO: Also parse wallet from path.
+
         url_split = urlsplit(url)
 
         schemes_hydra = ("mainnet", "main", "testnet", "test")
         schemes_main = ("http", "mainnet", "main")
         schemes = schemes_main + ("testnet", "test")
 
         scheme = url_split.scheme if not testnet else schemes[-1]
```

### Comparing `hydra_chain_py-2.7.6/hydra/test/__init__.py` & `hydra_chain_py-2.8.0/hydra/test/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/util/asyncc.py` & `hydra_chain_py-2.8.0/hydra/util/asyncc.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/util/struct.py` & `hydra_chain_py-2.8.0/hydra/util/struct.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/hydra/util/tlru.py` & `hydra_chain_py-2.8.0/hydra/util/tlru.py`

 * *Files identical despite different names*

### Comparing `hydra_chain_py-2.7.6/pyproject.toml` & `hydra_chain_py-2.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydra-chain-py"
-version = "2.7.6"
+version = "2.8.0"
 description = "Hydra Chain Tools & Application Library."
 authors = [
     "Phillip Sitbon <phillip.sitbon@gmail.com>",
     "Halospace Foundation <contact@halospace.org>",
 ]
 readme = "README.md"
 license = "AGPLv3"
@@ -22,20 +22,20 @@
 hy = "hydra.hy:Hydra.main"
 hycli = "hydra.app.cli:HydraCLIApp.main"
 peerscan = "hydra.app.peerscan:PeerScan.main"
 hytop = "hydra.app.top:TopApp.main"
 hytest = "hydra.test:Test.main"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-argcomplete = "^2.0.0"
+python = "^3.11"
+argcomplete = "^3.1.1"
 requests = "^2.28.1"
-pytz = "^2022.6"
+pytz = "^2023.3"
 attrdict3 = "^2.0.2"
 python-kucoin = "^2.1.3"
 pycryptodome = "^3.15.0"
 currencies = "^2020.12.12"
-pytest = "^7.2.0"
+pytest = "^7.4.0"  # TODO: Make optional once testing is decoupled from main package.
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hydra_chain_py-2.7.6/setup.py` & `hydra_chain_py-2.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,341 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hydra-chain-py
+Version: 2.8.0
+Summary: Hydra Chain Tools & Application Library.
+Home-page: https://github.com/hydraverse/hypy
+License: AGPLv3
+Author: Phillip Sitbon
+Author-email: phillip.sitbon@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: argcomplete (>=3.1.1,<4.0.0)
+Requires-Dist: attrdict3 (>=2.0.2,<3.0.0)
+Requires-Dist: currencies (>=2020.12.12,<2021.0.0)
+Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: python-kucoin (>=2.1.3,<3.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/hydraverse/hypy
+Description-Content-Type: text/markdown
 
-packages = \
-['hydra',
- 'hydra.app',
- 'hydra.kc',
- 'hydra.rpc',
- 'hydra.test',
- 'hydra.test.app',
- 'hydra.util']
-
-package_data = \
-{'': ['*'], 'hydra': ['res/*']}
-
-install_requires = \
-['argcomplete>=2.0.0,<3.0.0',
- 'attrdict3>=2.0.2,<3.0.0',
- 'currencies>=2020.12.12,<2021.0.0',
- 'pycryptodome>=3.15.0,<4.0.0',
- 'pytest>=7.2.0,<8.0.0',
- 'python-kucoin>=2.1.3,<3.0.0',
- 'pytz>=2022.6,<2023.0',
- 'requests>=2.28.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['hy = hydra.hy:Hydra.main',
-                     'hycli = hydra.app.cli:HydraCLIApp.main',
-                     'hytest = hydra.test:Test.main',
-                     'hytop = hydra.app.top:TopApp.main',
-                     'peerscan = hydra.app.peerscan:PeerScan.main']}
-
-setup_kwargs = {
-    'name': 'hydra-chain-py',
-    'version': '2.7.6',
-    'description': 'Hydra Chain Tools & Application Library.',
-    'long_description': '# [Hydra Chain Integration & Tools Library](https://pypi.org/project/hydra-chain-py/)\n\nThis is a Python support library for the Hydra Chain project (https://hydrachain.org) aimed at simplifying the process of using and developing apps for the blockchain.\n\nPrimarily, `hypy` (pronounced "hippie") currently provides:\n- RPC tools to access the Hydra JSON-RPC service.\n- A flexible command line tool with simple integration.\n- Application infrastructure to extend apps & tools.\n- Integrated apps for common tasks such as monitoring or connecting to new nodes.\n\n# Quick Start\n\nIf you know what this is and just want to get going, install:\n\n```commandline\npip install hydra-chain-py\n```\n\nOr with poetry:\n\n```commandline\npoetry add hydra-chain-py\n```\n\nThis adds the `hydra` package to your Python installation. \n\nThen, to get started, run:\n\n```commandline\nhy --help\n```\n\nFull download/install and usage instructions follow.\n\n# Usage\n\nThis library connects to a Hydra node on a local system or over a network.\n\nThe primary tool to interface with the node is called `hycli`, and for the most part behaves exactly the same as `hydra-cli`,\nwith some nicer output options:\n\n```commandline\nhycli getinfo\n```\n```shell\ngetinfo                \n  .version             180506\n  .protocolversion     70017\n  .walletversion       169900\n  .balance             28047.31917165\n  .stake               1452.99760027\n  .locked              \n    .used              128\n    .free              65408\n    .total             65536\n    .locked            65536\n    .chunks_used       2\n    .chunks_free       2\n  .blocks              155763\n  .timeoffset          0\n  .connections         8\n  .proxy               \n  .difficulty          \n    .proof-of-work     1.52587890625e-05\n    .proof-of-stake    797825.1819042678\n  .testnet             True\n  .moneysupply         20931869.76468454\n  .burnedcoins         73748.17511400\n  .keypoololdest       1635530802\n  .keypoolsize         2000\n  .unlocked_until      1741407462\n  .relayfee            0.004\n  .errors \n```\n\nThere\'s also `hytop`, which periodically displays useful node status info in a human-readable format:\n\n```commandline\nhytop -C\n```\n```shell\nnow                           2022-01-05 16:21:36.930567-08:00\nutcnow                        2022-01-06 00:21:36.930584\nconnectioncount               8\napr                           107.2079665372164\n\nstakinginfo\n  .enabled                    True\n  .staking                    True\n  .difficulty                 797825.1819042678\n  .search-interval            1:51:28\n  .weight                     28047.31917165\n  .netstakeweight             3918664.173517\n  .expectedtime               4:58:03\n\nwalletinfo\n  .walletname                 \'\'\n  .balance                    28047.31917165\n  .stake                      1452.99760027\n  .txcount                    2769\n  .unlocked_until             2025-03-07 20:17:42\n```\n\nAnd `peerscan`, which attempts to connect to new nodes:\n\n```commandline\npeerscan -vv\n```\n```shell\nINFO:hypy:server reports 327 connections\nINFO:hypy:loaded 327 peers\nINFO:hypy:loaded 1201 nodes\nINFO:hypy:trying 883 potential new peers\nINFO:hypy:server now reports 329 connections\n```\n\n# Clone & Install\n\nThis is both a library that you can import into your Python code and a command line tool that you can use and extend.\n\nWhen installing `hypy`, the command line tools become available as well.\n\nTo install the latest from git without cloning the repository,  jump down to the [Remote Installation](#Remote-Installation) section.\n\n### Clone/Download Sources:\n\n```commandline\ngit clone https://github.com/hydraverse/hypy\n```\n```shell\nCloning into \'hypy\'...\n...\n```\n\n### Environment\n\nThe simplest way to use `hypy` is to install it at the system level, but sometimes it can be hard to manage varying Python\nversion needs and dependencies.\n\nIf installing at the system level, jump down to the [Installation](#Installing) section.\n\n#### Poetry\n\nThis is now the only recommended/supported way to install or develop with this package.\n\nCreate a new poetry project:\n\n```commandline\npoetry new myproject && cd myproject && poetry add hydra-chain-py\n```\n\n# Installing\n\n### From Source\n\nInstalling from the cloned `hypy` library folder:\n\n```commandline\npoetry install .\n```\n\n### Remote Installation <a name="Remote-Installation"></a>\n\nInstalling directly from GitHub:\n\n```commandline\npoetry add git+https://github.com/hydraverse/hypy\n```\n\nOr to get a specific branch, tag, or revision:\n\n```commandline\npoetry add git+https://github.com/hydraverse/hypy@v2.7.2\n```\n\nThis example installs the `v2.7.2` tagged version.\n\n### Uninstall\n\n```commandline\npip uninstall hypy\n```\nOr\n```commandline\npoetry remove hydra-chain-py\n```\n\n### Packaging\n\nYou can create a redistributable wheel package for later installation with the following command:\n\n```commandline\npoetry build\n```\n\n# Use: `hy`\n\n`hy` is the *Hydra Chain Tool*, a command-line toolkit meant to run standalone modules, aka `apps`, with convenient access to instantiated library objects.\n\nSome apps are provided by the library, and the `hy` module provides you with a means to\nintegrate your own apps and run them as if they were part of the tool. More on that in the example app below.\n\nRunning an app on the command line looks something like this **(note: \'֍\' is the command shell prompt)**:\n\n```commandline\nhy [-h] <some-app> [-h] [options] [app params]\n```\n\nUse the `-h` option *before* the app name to see a list of apps, and after to get usage for a particular app.\n\nThe primary apps currently available are `cli` and `test`. These are provided as system-level\ncommands alongside `hy` when you install `hypy`.\n\nThis means that instead of calling `hy cli ...`, for example, you can use `hycli ...` instead.\n\nNote that all program options (except `-h` or `-v`) must appear *after* the app name.\n\n# Run Unit Tests\n\n`hy test - [-k "<test_name_pattern> or <test_name_pattern> ..."]`\n\nThis command is also available globally (with slight variation, no need for `-` param) after installation as `hytest`.\n\nYou can also specify different parameters for the tests with environment variables, such as `HYPY_LOG`.\nThese variables also work with `hy`.\n\n```commandline\nHY_RPC_WALLET=watch HY_LOG=ERROR hy test -\n```\n```shell\n=========================== test session starts ============================\nplatform linux -- Python 3.8.10, pytest-6.2.5, py-1.11.0, pluggy-1.0.0\nrootdir: /home/halo/pr/hy/hypy\ncollected 13 items                                                         \n\nhydra/test/app/cli.py::HydraCLIAppTest::test_app_cli_runnable PASSED [  7%]\nhydra/test/rpc.py::HydraRPCTest::test_rpc_stub PASSED                [ 15%]\nhydra/app/txvio.py::TxVIOAppTest::test_0_txvio_runnable PASSED       [ 23%]\nhydra/app/txvio.py::TxVIOAppTest::test_1_txvio_run PASSED            [ 30%]\nhydra/app/ascan.py::AScanAppTest::test_0_ascan_runnable PASSED       [ 38%]\nhydra/app/ascan.py::AScanAppTest::test_1_ascan_run PASSED            [ 46%]\nhydra/app/atrace.py::ATraceAppTest::test_0_atrace_runnable PASSED    [ 53%]\nhydra/app/atrace.py::ATraceAppTest::test_1_atrace_run PASSED         [ 61%]\nhydra/app/lstx.py::TxListAppTest::test_0_lstx_runnable PASSED        [ 69%]\nhydra/app/lstx.py::TxListAppTest::test_1_lstx_run PASSED             [ 76%]\nhydra/app/peerscan.py::PeerScanTest::test_0_peerscan_runnable PASSED [ 84%]\nhydra/app/peerscan.py::PeerScanTest::test_1_peerscan_run PASSED      [ 92%]\nhydra/app/top.py::TopAppTest::test_0_top_runnable PASSED             [100%]\n\n=========================== 13 passed in 37.17s ============================\n```\n\n### Standalone Testing\n\nWhen developing ouside the library, tests can be run for standalone Application implementations.\n\n```commandline\nhy-test examples/my_hydra_app.py\n```\n\n# Full Usage: `hy`\n\n**NOTE:** Tab-completion is available via `argcomplete` but per-app parameters\nwon\'t be shown, only the primary `hy` parameters.\n\n### `hy`\n\n```commandline\nhy -h\n```\n```shell\nusage: hy [-h] [-v] [-l LOG] [--rpc RPC] [--rpc-wallet RPC_WALLET]\n          [--rpc-testnet] [-J] [-j] [-f]\n          {cli,test,ascan,atrace,lstx,txvio,peerscan,top} ...\n\nHyPy Library Application Tool.\n\npositional arguments:\n  {cli,test,ascan,atrace,lstx,txvio,peerscan,top}\n                        application to run.\n  ARGS                  application args.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -v, --verbose         verbose level (up to 3x) (env: HYPY_V).\n  -l LOG, --log LOG     log level (name: error,warning,info,debug,notset)\n                        (env: HYPY_LOG).\n  --rpc RPC             rpc url (env: HY_RPC)\n  --rpc-wallet RPC_WALLET\n                        rpc wallet name override (env: HY_RPC_WALLET)\n  --rpc-testnet         rpc testnet override (env: HY_RPC_WALLET)\n  -J, --json-pretty     output parseable json\n  -j, --json            output parseable json\n  -f, --full            output full names (non-json only)\n```\n\n### `cli`\n\n```commandline\nhycli -h\n```\n```shell\nusage: hy cli ... [-f] ...\n\noptional arguments:\n  ...\n\ncli:\n  rpc cli interface\n\n  -f, --full            output full names (non-json only)\n  CALL                  rpc function to call\n  PARAM                 rpc function parameters\n```\n\nOnly the last section in an app\'s help message (`cli` in the above case) will differ\nbetween apps.\n',
-    'author': 'Phillip Sitbon',
-    'author_email': 'phillip.sitbon@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/hydraverse/hypy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+# [Hydra Chain Integration & Tools Library](https://pypi.org/project/hydra-chain-py/)
 
+This is a Python support library for the Hydra Chain project (https://hydrachain.org) aimed at simplifying the process of using and developing apps for the blockchain.
+
+Primarily, `hypy` (pronounced "hippie") currently provides:
+- RPC tools to access the Hydra JSON-RPC service.
+- A flexible command line tool with simple integration.
+- Application infrastructure to extend apps & tools.
+- Integrated apps for common tasks such as monitoring or connecting to new nodes.
+
+# Quick Start
+
+If you know what this is and just want to get going, install:
+
+```commandline
+pip install hydra-chain-py
+```
+
+Or with poetry:
+
+```commandline
+poetry add hydra-chain-py
+```
+
+This adds the `hydra` package to your Python installation. 
+
+Then, to get started, run:
+
+```commandline
+hy --help
+```
+
+Full download/install and usage instructions follow.
+
+# Usage
+
+This library connects to a Hydra node on a local system or over a network.
+
+The primary tool to interface with the node is called `hycli`, and for the most part behaves exactly the same as `hydra-cli`,
+with some nicer output options:
+
+```commandline
+hycli getinfo
+```
+```shell
+getinfo                
+  .version             180506
+  .protocolversion     70017
+  .walletversion       169900
+  .balance             28047.31917165
+  .stake               1452.99760027
+  .locked              
+    .used              128
+    .free              65408
+    .total             65536
+    .locked            65536
+    .chunks_used       2
+    .chunks_free       2
+  .blocks              155763
+  .timeoffset          0
+  .connections         8
+  .proxy               
+  .difficulty          
+    .proof-of-work     1.52587890625e-05
+    .proof-of-stake    797825.1819042678
+  .testnet             True
+  .moneysupply         20931869.76468454
+  .burnedcoins         73748.17511400
+  .keypoololdest       1635530802
+  .keypoolsize         2000
+  .unlocked_until      1741407462
+  .relayfee            0.004
+  .errors 
+```
+
+There's also `hytop`, which periodically displays useful node status info in a human-readable format:
+
+```commandline
+hytop -C
+```
+```shell
+now                           2022-01-05 16:21:36.930567-08:00
+utcnow                        2022-01-06 00:21:36.930584
+connectioncount               8
+apr                           107.2079665372164
+
+stakinginfo
+  .enabled                    True
+  .staking                    True
+  .difficulty                 797825.1819042678
+  .search-interval            1:51:28
+  .weight                     28047.31917165
+  .netstakeweight             3918664.173517
+  .expectedtime               4:58:03
+
+walletinfo
+  .walletname                 ''
+  .balance                    28047.31917165
+  .stake                      1452.99760027
+  .txcount                    2769
+  .unlocked_until             2025-03-07 20:17:42
+```
+
+And `peerscan`, which attempts to connect to new nodes:
+
+```commandline
+peerscan -vv
+```
+```shell
+INFO:hypy:server reports 327 connections
+INFO:hypy:loaded 327 peers
+INFO:hypy:loaded 1201 nodes
+INFO:hypy:trying 883 potential new peers
+INFO:hypy:server now reports 329 connections
+```
+
+# Clone & Install
+
+This is both a library that you can import into your Python code and a command line tool that you can use and extend.
+
+When installing `hypy`, the command line tools become available as well.
+
+To install the latest from git without cloning the repository,  jump down to the [Remote Installation](#Remote-Installation) section.
+
+### Clone/Download Sources:
+
+```commandline
+git clone https://github.com/hydraverse/hypy
+```
+```shell
+Cloning into 'hypy'...
+...
+```
+
+### Environment
+
+The simplest way to use `hypy` is to install it at the system level, but sometimes it can be hard to manage varying Python
+version needs and dependencies.
+
+If installing at the system level, jump down to the [Installation](#Installing) section.
+
+#### Poetry
+
+This is now the only recommended/supported way to install or develop with this package.
+
+Create a new poetry project:
+
+```commandline
+poetry new myproject && cd myproject && poetry add hydra-chain-py
+```
+
+# Installing
+
+### From Source
+
+Installing from the cloned `hypy` library folder:
+
+```commandline
+poetry install .
+```
+
+### Remote Installation <a name="Remote-Installation"></a>
+
+Installing directly from GitHub:
+
+```commandline
+poetry add git+https://github.com/hydraverse/hypy
+```
+
+Or to get a specific branch, tag, or revision:
+
+```commandline
+poetry add git+https://github.com/hydraverse/hypy@v2.7.2
+```
+
+This example installs the `v2.7.2` tagged version.
+
+### Uninstall
+
+```commandline
+pip uninstall hypy
+```
+Or
+```commandline
+poetry remove hydra-chain-py
+```
+
+### Packaging
+
+You can create a redistributable wheel package for later installation with the following command:
+
+```commandline
+poetry build
+```
+
+# Use: `hy`
+
+`hy` is the *Hydra Chain Tool*, a command-line toolkit meant to run standalone modules, aka `apps`, with convenient access to instantiated library objects.
+
+Some apps are provided by the library, and the `hy` module provides you with a means to
+integrate your own apps and run them as if they were part of the tool. More on that in the example app below.
+
+Running an app on the command line looks something like this **(note: '֍' is the command shell prompt)**:
+
+```commandline
+hy [-h] <some-app> [-h] [options] [app params]
+```
+
+Use the `-h` option *before* the app name to see a list of apps, and after to get usage for a particular app.
+
+The primary apps currently available are `cli` and `test`. These are provided as system-level
+commands alongside `hy` when you install `hypy`.
+
+This means that instead of calling `hy cli ...`, for example, you can use `hycli ...` instead.
+
+Note that all program options (except `-h` or `-v`) must appear *after* the app name.
+
+# Run Unit Tests
+
+`hy test - [-k "<test_name_pattern> or <test_name_pattern> ..."]`
+
+This command is also available globally (with slight variation, no need for `-` param) after installation as `hytest`.
+
+You can also specify different parameters for the tests with environment variables, such as `HYPY_LOG`.
+These variables also work with `hy`.
+
+```commandline
+HY_RPC_WALLET=watch HY_LOG=ERROR hy test -
+```
+```shell
+=========================== test session starts ============================
+platform linux -- Python 3.8.10, pytest-6.2.5, py-1.11.0, pluggy-1.0.0
+rootdir: /home/halo/pr/hy/hypy
+collected 13 items                                                         
+
+hydra/test/app/cli.py::HydraCLIAppTest::test_app_cli_runnable PASSED [  7%]
+hydra/test/rpc.py::HydraRPCTest::test_rpc_stub PASSED                [ 15%]
+hydra/app/txvio.py::TxVIOAppTest::test_0_txvio_runnable PASSED       [ 23%]
+hydra/app/txvio.py::TxVIOAppTest::test_1_txvio_run PASSED            [ 30%]
+hydra/app/ascan.py::AScanAppTest::test_0_ascan_runnable PASSED       [ 38%]
+hydra/app/ascan.py::AScanAppTest::test_1_ascan_run PASSED            [ 46%]
+hydra/app/atrace.py::ATraceAppTest::test_0_atrace_runnable PASSED    [ 53%]
+hydra/app/atrace.py::ATraceAppTest::test_1_atrace_run PASSED         [ 61%]
+hydra/app/lstx.py::TxListAppTest::test_0_lstx_runnable PASSED        [ 69%]
+hydra/app/lstx.py::TxListAppTest::test_1_lstx_run PASSED             [ 76%]
+hydra/app/peerscan.py::PeerScanTest::test_0_peerscan_runnable PASSED [ 84%]
+hydra/app/peerscan.py::PeerScanTest::test_1_peerscan_run PASSED      [ 92%]
+hydra/app/top.py::TopAppTest::test_0_top_runnable PASSED             [100%]
+
+=========================== 13 passed in 37.17s ============================
+```
+
+### Standalone Testing
+
+When developing ouside the library, tests can be run for standalone Application implementations.
+
+```commandline
+hy-test examples/my_hydra_app.py
+```
+
+# Full Usage: `hy`
+
+**NOTE:** Tab-completion is available via `argcomplete` but per-app parameters
+won't be shown, only the primary `hy` parameters.
+
+### `hy`
+
+```commandline
+hy -h
+```
+```shell
+usage: hy [-h] [-v] [-l LOG] [--rpc RPC] [--rpc-wallet RPC_WALLET]
+          [--rpc-testnet] [-J] [-j] [-f]
+          {cli,test,ascan,atrace,lstx,txvio,peerscan,top} ...
+
+HyPy Library Application Tool.
+
+positional arguments:
+  {cli,test,ascan,atrace,lstx,txvio,peerscan,top}
+                        application to run.
+  ARGS                  application args.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --verbose         verbose level (up to 3x) (env: HYPY_V).
+  -l LOG, --log LOG     log level (name: error,warning,info,debug,notset)
+                        (env: HYPY_LOG).
+  --rpc RPC             rpc url (env: HY_RPC)
+  --rpc-wallet RPC_WALLET
+                        rpc wallet name override (env: HY_RPC_WALLET)
+  --rpc-testnet         rpc testnet override (env: HY_RPC_WALLET)
+  -J, --json-pretty     output parseable json
+  -j, --json            output parseable json
+  -f, --full            output full names (non-json only)
+```
+
+### `cli`
+
+```commandline
+hycli -h
+```
+```shell
+usage: hy cli ... [-f] ...
+
+optional arguments:
+  ...
+
+cli:
+  rpc cli interface
+
+  -f, --full            output full names (non-json only)
+  CALL                  rpc function to call
+  PARAM                 rpc function parameters
+```
+
+Only the last section in an app's help message (`cli` in the above case) will differ
+between apps.
 
-setup(**setup_kwargs)
```

