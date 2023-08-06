# Comparing `tmp/dxsp-4.2.4.tar.gz` & `tmp/dxsp-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.2.4.tar", max compression
+gzip compressed data, was "dxsp-4.2.5.tar", max compression
```

## Comparing `dxsp-4.2.4.tar` & `dxsp-4.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-08-04 18:55:20.366511 dxsp-4.2.4/LICENSE
--rw-r--r--   0        0        0     2857 2023-08-04 18:55:20.366511 dxsp-4.2.4/README.md
--rw-r--r--   0        0        0      158 2023-08-04 18:55:20.366511 dxsp-4.2.4/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-08-04 18:55:20.366511 dxsp-4.2.4/dxsp/config.py
--rw-r--r--   0        0        0    12124 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5743 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-08-04 18:55:20.370511 dxsp-4.2.4/dxsp/utils/utils.py
--rw-r--r--   0        0        0     3929 2023-08-04 18:55:26.494509 dxsp-4.2.4/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 10:16:06.333841 dxsp-4.2.5/LICENSE
+-rw-r--r--   0        0        0     2740 2023-08-06 10:16:06.333841 dxsp-4.2.5/README.md
+-rw-r--r--   0        0        0      158 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/config.py
+-rw-r--r--   0        0        0    12124 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-08-06 10:16:06.333841 dxsp-4.2.5/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     3931 2023-08-06 10:16:10.561876 dxsp-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 dxsp-4.2.5/PKG-INFO
```

### Comparing `dxsp-4.2.4/LICENSE` & `dxsp-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/README.md` & `dxsp-4.2.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a>
-<a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
   </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/dxsp/"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
   <a href="https://codeclimate.com/github/mraniki/dxsp/maintainability"><img src="https://api.codeclimate.com/v1/badges/ec80e827d5878e60ba12/maintainability" /></a>
     </td>
     <td align="left"> 
 Swap made easy<br>
-Trade on any blockchains with uniswap based router or 0x protocol.
+Trade on any blockchains <br>with uniswap based router or 0x protocol.
     </td> 
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
@@ -35,11 +34,10 @@
     dex = DexSwap()
     #BUY 10 USDT to SWAP with BITCOIN
     demo_tx = await dex.get_swap('USDT','wBTC',10)
     print("demo_tx ", demo_tx)
 </code>
 </pre>
 
-<h5>Example</h5>
-
-https://github.com/mraniki/dxsp/blob/822cc96df0878782ca059b6dbf44bd451ccd32fa/examples/example.py#L1-L68
 
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/dxsp/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
```

#### html2text {}

```diff
@@ -1,37 +1,34 @@
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
-[https://img.shields.io/badge/github-
-%23000000.svg?style=for-the-
+the-badge&logo=wikipedia&logoColor=white] [https://
+img.shields.io/badge/github-%23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [https://img.shields.io/
-docker/pulls/mraniki/tt?style=for-the-badge]                       [Logo]
-[https://img.shields.io/badge/tips-000000?style=for-the-
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
+badge/tips-000000?style=for-the-                                     [Logo]
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/mraniki/tt?style=for-
+the-badge] [https://img.shields.io/badge/talky-
+blue?style=for-the-badge&logo=telegram&logoColor=white]
 [https://img.shields.io/pypi/v/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey]
 [https://img.shields.io/github/actions/workflow/status/     Swap made easy
 mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-            Trade on any
-badge&logo=GitHub&logoColor=white]                          blockchains with
-[https://readthedocs.org/projects/dxsp/badge/               uniswap based
+badge&logo=GitHub&logoColor=white]                          blockchains
+[https://readthedocs.org/projects/dxsp/badge/               with uniswap based
 ?version=latest&style=for-the-badge]                        router or 0x
 [https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-        protocol.
 2fb099f1fc2a]
 [https://codecov.io/gh/mraniki/dxsp/branch/main/graph/
 badge.svg?token=39ED0ZA6IH]
 [https://api.codeclimate.com/v1/badges/
 ec80e827d5878e60ba12/maintainability]
 ** How to use it **
 
    from dxsp import DexSwap
     dex = DexSwap()
     #BUY 10 USDT to SWAP with BITCOIN
     demo_tx = await dex.get_swap('USDT','wBTC',10)
     print("demo_tx ", demo_tx)
-** Example **
-https://github.com/mraniki/dxsp/blob/822cc96df0878782ca059b6dbf44bd451ccd32fa/
-examples/example.py#L1-L68
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

### Comparing `dxsp-4.2.4/dxsp/default_settings.toml` & `dxsp-4.2.5/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/main.py` & `dxsp-4.2.5/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/protocols/oneinch.py` & `dxsp-4.2.5/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/protocols/uniswap.py` & `dxsp-4.2.5/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/protocols/zerox.py` & `dxsp-4.2.5/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/utils/account_utils.py` & `dxsp-4.2.5/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/utils/contract_utils.py` & `dxsp-4.2.5/dxsp/utils/contract_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/dxsp/utils/explorer_utils.py` & `dxsp-4.2.5/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.2.4/pyproject.toml` & `dxsp-4.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.2.4"
+version = "4.2.5"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -49,14 +49,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.2.0"
 eth_tester = "^0.9.0b2"
@@ -78,14 +79,15 @@
 
 
 
 
 
 
 
+
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5,<6"
 sphinx_bootstrap_theme = "^0.8.1"
```

### Comparing `dxsp-4.2.4/PKG-INFO` & `dxsp-4.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.2.4
+Version: 4.2.5
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,36 +20,35 @@
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a>
-<a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
   </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/v/dxsp?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/dxsp/"><img src="https://img.shields.io/pypi/dm/dxsp?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
       <a href="https://github.com/mraniki/dxsp/"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
-   <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
+   <a href="https://talky.readthedocs.io/projects/dxsp/"><img src="https://readthedocs.org/projects/dxsp/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-dxsp-main"><img src="https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-2fb099f1fc2a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/dxsp"><img src="https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH"/> </a><br>
   <a href="https://codeclimate.com/github/mraniki/dxsp/maintainability"><img src="https://api.codeclimate.com/v1/badges/ec80e827d5878e60ba12/maintainability" /></a>
     </td>
     <td align="left"> 
 Swap made easy<br>
-Trade on any blockchains with uniswap based router or 0x protocol.
+Trade on any blockchains <br>with uniswap based router or 0x protocol.
     </td> 
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
@@ -57,12 +56,11 @@
     dex = DexSwap()
     #BUY 10 USDT to SWAP with BITCOIN
     demo_tx = await dex.get_swap('USDT','wBTC',10)
     print("demo_tx ", demo_tx)
 </code>
 </pre>
 
-<h5>Example</h5>
-
-https://github.com/mraniki/dxsp/blob/822cc96df0878782ca059b6dbf44bd451ccd32fa/examples/example.py#L1-L68
 
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/dxsp/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
```

#### html2text {}

```diff
@@ -1,49 +1,46 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.2.4 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.5 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
 pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-URL: Changelog, https://
 github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst Project-URL: Issues, https://
 github.com/mraniki/dxsp/issues Project-URL: Support, https://github.com/
 mraniki/dxsp/discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
-[https://img.shields.io/badge/github-
-%23000000.svg?style=for-the-
+the-badge&logo=wikipedia&logoColor=white] [https://
+img.shields.io/badge/github-%23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [https://img.shields.io/
-docker/pulls/mraniki/tt?style=for-the-badge]                       [Logo]
-[https://img.shields.io/badge/tips-000000?style=for-the-
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
+badge/tips-000000?style=for-the-                                     [Logo]
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/mraniki/tt?style=for-
+the-badge] [https://img.shields.io/badge/talky-
+blue?style=for-the-badge&logo=telegram&logoColor=white]
 [https://img.shields.io/pypi/v/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/dxsp?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey]
 [https://img.shields.io/github/actions/workflow/status/     Swap made easy
 mraniki/dxsp/%F0%9F%91%B7Flow.yml?style=for-the-            Trade on any
-badge&logo=GitHub&logoColor=white]                          blockchains with
-[https://readthedocs.org/projects/dxsp/badge/               uniswap based
+badge&logo=GitHub&logoColor=white]                          blockchains
+[https://readthedocs.org/projects/dxsp/badge/               with uniswap based
 ?version=latest&style=for-the-badge]                        router or 0x
 [https://codebeat.co/badges/b1376839-73bc-4b41-bfc1-        protocol.
 2fb099f1fc2a]
 [https://codecov.io/gh/mraniki/dxsp/branch/main/graph/
 badge.svg?token=39ED0ZA6IH]
 [https://api.codeclimate.com/v1/badges/
 ec80e827d5878e60ba12/maintainability]
 ** How to use it **
 
    from dxsp import DexSwap
     dex = DexSwap()
     #BUY 10 USDT to SWAP with BITCOIN
     demo_tx = await dex.get_swap('USDT','wBTC',10)
     print("demo_tx ", demo_tx)
-** Example **
-https://github.com/mraniki/dxsp/blob/822cc96df0878782ca059b6dbf44bd451ccd32fa/
-examples/example.py#L1-L68
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

