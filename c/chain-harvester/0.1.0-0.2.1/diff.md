# Comparing `tmp/chain_harvester-0.1.0.tar.gz` & `tmp/chain_harvester-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chain_harvester-0.1.0.tar", max compression
+gzip compressed data, was "chain_harvester-0.2.1.tar", max compression
```

## Comparing `chain_harvester-0.1.0.tar` & `chain_harvester-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-08-04 20:40:41.767908 chain_harvester-0.1.0/LICENSE
--rw-r--r--   0        0        0      277 2023-08-04 20:40:41.767908 chain_harvester-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-04 20:40:41.767908 chain_harvester-0.1.0/chain_harvester/__init__.py
--rw-r--r--   0        0        0     9199 2023-08-04 20:40:41.767908 chain_harvester-0.1.0/chain_harvester/chain.py
--rw-r--r--   0        0        0     1588 2023-08-04 20:41:03.016191 chain_harvester-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 chain_harvester-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/LICENSE
+-rw-r--r--   0        0        0      205 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/__init__.py
+-rw-r--r--   0        0        0     8697 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/chain.py
+-rw-r--r--   0        0        0     5591 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/constants.py
+-rw-r--r--   0        0        0     6719 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/multicall.py
+-rw-r--r--   0        0        0        0 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/networks/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/networks/ethereum/__init__.py
+-rw-r--r--   0        0        0     1245 2023-08-06 09:48:50.930056 chain_harvester-0.2.1/chain_harvester/networks/ethereum/mainnet.py
+-rw-r--r--   0        0        0     1543 2023-08-06 09:49:14.454223 chain_harvester-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 chain_harvester-0.2.1/PKG-INFO
```

### Comparing `chain_harvester-0.1.0/LICENSE` & `chain_harvester-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chain_harvester-0.1.0/chain_harvester/chain.py` & `chain_harvester-0.2.1/chain_harvester/chain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,118 +1,102 @@
-import inspect
 import json
 import logging
 import os
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
 
+from chain_harvester.multicall import Call, Multicall
+
 log = logging.getLogger(__name__)
 
 
 class Chain:
     def __init__(
         self,
         rpc=None,
-        chain=None,
+        w3=None,
         step=None,
-        etherscan_api_key=None,
-        abis_path=None,
         chain_id=None,
+        rpc_nodes=None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.rpc = rpc
-        self._chain = chain
+        self._w3 = w3
         self.step = step or 10_000
         self.provider = rpc
-        self.etherscan_api_key = etherscan_api_key
-        self.abis_path = abis_path
+
         self.chain_id = chain_id
+        self.rpc_nodes = rpc_nodes
 
         self._abis = {}
         self.current_block = 0
-        self.retry = 0
+
+        self.chain = None
+        self.network = None
 
     @property
-    def chain(self):
-        if not self._chain:
+    def w3(self):
+        if not self._w3:
             session = requests.Session()
             retries = 3
             retry = Retry(
                 total=retries,
                 read=retries,
                 connect=retries,
                 backoff_factor=0.5,
                 status_forcelist=(429,),
                 respect_retry_after_header=True,
             )
             adapter = HTTPAdapter(max_retries=retry)
             session.mount("http://", adapter)
             session.mount("https://", adapter)
 
-            self._chain = Web3(Web3.HTTPProvider(self.rpc, request_kwargs={"timeout": 60}, session=session))
-            self._chain.middleware_onion.inject(geth_poa_middleware, layer=0)
-        return self._chain
+            self._w3 = Web3(Web3.HTTPProvider(self.rpc, request_kwargs={"timeout": 60}, session=session))
+            self._w3.middleware_onion.inject(geth_poa_middleware, layer=0)
+        return self._w3
 
     @property
     def eth(self):
-        return self.chain.eth
+        return self.w3.eth
 
     def get_block_info(self, block_number):
         return self.eth.get_block(block_number)
 
     def get_latest_block(self):
         return self.eth.get_block_number()
 
-    def get_abi_from_etherscan(self, contract_address):
-        try:
-            req = requests.get(
-                "https://api.etherscan.io/api?module=contract&action=getabi&address="
-                + contract_address
-                + "&apikey="
-                + self.etherscan_api_key,
-                timeout=5,
-            )
-        except requests.exceptions.Timeout:
-            log.exception("Timeout when get abi from etherscan", extra={"contract_address": contract_address})
-            raise
-        resp = json.loads(req.text)
-        abi = json.loads(resp["result"])
-        return abi
+    def get_abi_from_source(self, contract_address):
+        raise NotImplementedError
 
     def load_abi(self, contract_address):
         contract_address = contract_address.lower()
         if contract_address not in self._abis:
-            if not os.path.exists(self.abis_path):
-                os.makedirs(self.abis_path)
-            current_file_path = inspect.getfile(inspect.currentframe())
-            current_directory = os.path.dirname(os.path.abspath(current_file_path))
-            file_path = os.path.join(current_directory, "abis", f"{contract_address}.json")
+            file_path = os.path.join(self.abis_path, f"{contract_address}.json")
             if os.path.exists(file_path):
                 with open(file_path) as f:
                     self._abis[contract_address] = json.loads(f.read())
             else:
-                abi = self.get_abi_from_etherscan(contract_address)
-
+                abi = self.get_abi_from_source(contract_address)
                 with open(file_path, "w") as f:
                     json.dump(abi, f)
                 with open(file_path) as f:
                     self._abis[contract_address] = json.loads(f.read())
         return self._abis[contract_address]
 
     def get_contract(self, contract_address):
         if Web3.is_address(contract_address):
             contract_address = Web3.to_checksum_address(contract_address)
         abi = self.load_abi(contract_address)
-        return self.chain.eth.contract(address=contract_address, abi=abi)
+        return self.eth.contract(address=contract_address, abi=abi)
 
     def call_contract_function(self, contract_address, function_name, *args, **kwargs):
         contract_address = Web3.to_checksum_address(contract_address)
         contract = self.get_contract(contract_address)
         contract_function = contract.get_function_by_name(function_name)
         result = contract_function(*args).call(block_identifier=kwargs.get("block_identifier", "latest"))
         return result
@@ -241,7 +225,16 @@
                 extra_log={
                     "event_attr": event_attr,
                     "contract_address": contract.address,
                 },
             )
 
         return self._yield_events(fetch_events_func, from_block, to_block)
+
+    def multicall(self, calls, block_identifier=None):
+        multicalls = []
+        for address, function, response in calls:
+            multicalls.append(Call(address, function, [response]))
+
+        multi = Multicall(multicalls, self.chain_id, _w3=self.w3, block_identifier=block_identifier)
+
+        return multi()
```

### Comparing `chain_harvester-0.1.0/pyproject.toml` & `chain_harvester-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 [tool.poetry]
 name = "chain_harvester"
-version = "v0.1.0"
+version = "v0.2.1"
 description = "A Python library designed to interface with various blockchain networks, enabling the retrieval of data."
 authors = ["0xCommanderKeen <f91289621+0xCommanderKeen@users.noreply.github.com>"]
 repository = "https://github.com/blockanalitica/chain-harvester"
 documentation = "https://blockanalitica.github.io/chain-harvester/"
 readme = "README.md"
 packages = [
   {include = "chain_harvester"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 web3 = "^6.8.0"
 requests = "^2.31.0"
+eth-abi = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 tox = "^4.6.4"
+python-dotenv = "^1.0.0"
 
 
-[tool.poetry.group.docs.dependencies]
-mkdocs = "^1.5.2"
-mkdocs-material = "^9.1.0"
-mkdocstrings-python = "1.2.1"
-mkdocstrings = "0.22"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
@@ -73,14 +69,16 @@
     "TRY",
 ]
 ignore = [
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
+    "TRY300"
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
+"intregration_tests/*" = ["S101"]
```

### Comparing `chain_harvester-0.1.0/PKG-INFO` & `chain_harvester-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: chain-harvester
-Version: 0.1.0
+Version: 0.2.1
 Summary: A Python library designed to interface with various blockchain networks, enabling the retrieval of data.
 Home-page: https://github.com/blockanalitica/chain-harvester
 Author: 0xCommanderKeen
 Author-email: f91289621+0xCommanderKeen@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: eth-abi (>=4.1.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: web3 (>=6.8.0,<7.0.0)
 Project-URL: Documentation, https://blockanalitica.github.io/chain-harvester/
 Project-URL: Repository, https://github.com/blockanalitica/chain-harvester
 Description-Content-Type: text/markdown
 
 # chain-harvester
 
 A Python library designed to interface with various blockchain networks, enabling the retrieval of data.
 
 - **Github repository**: <https://github.com/blockanalitica/chain-harvester/>
-- **Documentation** <https://blockanalitica .github.io/chain-harvester/>
+
```

