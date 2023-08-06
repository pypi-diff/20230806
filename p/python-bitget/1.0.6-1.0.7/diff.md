# Comparing `tmp/python-bitget-1.0.6.tar.gz` & `tmp/python-bitget-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bitget-1.0.6.tar", last modified: Tue Mar  7 10:41:32 2023, max compression
+gzip compressed data, was "python-bitget-1.0.7.tar", last modified: Sun Aug  6 09:04:04 2023, max compression
```

## Comparing `python-bitget-1.0.6.tar` & `python-bitget-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 10:41:32.606781 python-bitget-1.0.6/
--rw-rw-rw-   0        0        0     5110 2023-03-07 10:41:32.606781 python-bitget-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4431 2023-01-31 03:15:35.000000 python-bitget-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 10:41:32.591161 python-bitget-1.0.6/pybitget/
--rw-rw-rw-   0        0        0      269 2023-03-07 10:36:54.000000 python-bitget-1.0.6/pybitget/__init__.py
--rw-rw-rw-   0        0        0    81697 2023-03-07 10:10:10.000000 python-bitget-1.0.6/pybitget/client.py
--rw-rw-rw-   0        0        0     3403 2023-03-02 03:06:25.000000 python-bitget-1.0.6/pybitget/enums.py
--rw-rw-rw-   0        0        0     1114 2023-01-12 12:57:52.000000 python-bitget-1.0.6/pybitget/exceptions.py
--rw-rw-rw-   0        0        0    11088 2023-02-02 13:25:25.000000 python-bitget-1.0.6/pybitget/stream.py
--rw-rw-rw-   0        0        0     1586 2023-01-28 03:15:50.000000 python-bitget-1.0.6/pybitget/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:41:32.606781 python-bitget-1.0.6/python_bitget.egg-info/
--rw-rw-rw-   0        0        0     5110 2023-03-07 10:41:32.000000 python-bitget-1.0.6/python_bitget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-03-07 10:41:32.000000 python-bitget-1.0.6/python_bitget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 10:41:32.000000 python-bitget-1.0.6/python_bitget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-03-07 10:41:32.000000 python-bitget-1.0.6/python_bitget.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-07 10:41:32.000000 python-bitget-1.0.6/python_bitget.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-27 06:13:12.000000 python-bitget-1.0.6/python_bitget.egg-info/zip-safe
--rw-rw-rw-   0        0        0      144 2023-03-07 10:41:32.606781 python-bitget-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1578 2023-01-27 06:10:48.000000 python-bitget-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:04:04.875451 python-bitget-1.0.7/
+-rw-rw-rw-   0        0        0     5333 2023-08-06 09:04:04.875451 python-bitget-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4654 2023-08-06 08:50:14.000000 python-bitget-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 09:04:04.859832 python-bitget-1.0.7/pybitget/
+-rw-rw-rw-   0        0        0      269 2023-08-06 08:41:08.000000 python-bitget-1.0.7/pybitget/__init__.py
+-rw-rw-rw-   0        0        0    82531 2023-08-06 08:38:05.000000 python-bitget-1.0.7/pybitget/client.py
+-rw-rw-rw-   0        0        0     3403 2023-03-02 03:06:25.000000 python-bitget-1.0.7/pybitget/enums.py
+-rw-rw-rw-   0        0        0     1114 2023-01-12 12:57:52.000000 python-bitget-1.0.7/pybitget/exceptions.py
+-rw-rw-rw-   0        0        0    11089 2023-08-06 08:16:52.000000 python-bitget-1.0.7/pybitget/stream.py
+-rw-rw-rw-   0        0        0     1586 2023-01-28 03:15:50.000000 python-bitget-1.0.7/pybitget/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:04:04.875451 python-bitget-1.0.7/python_bitget.egg-info/
+-rw-rw-rw-   0        0        0     5333 2023-08-06 09:04:04.000000 python-bitget-1.0.7/python_bitget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-08-06 09:04:04.000000 python-bitget-1.0.7/python_bitget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:04:04.000000 python-bitget-1.0.7/python_bitget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-08-06 09:04:04.000000 python-bitget-1.0.7/python_bitget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 09:04:04.000000 python-bitget-1.0.7/python_bitget.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-01-27 06:13:12.000000 python-bitget-1.0.7/python_bitget.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      144 2023-08-06 09:04:04.875451 python-bitget-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1578 2023-01-27 06:10:48.000000 python-bitget-1.0.7/setup.py
```

### Comparing `python-bitget-1.0.6/PKG-INFO` & `python-bitget-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bitget
-Version: 1.0.6
+Version: 1.0.7
 Summary: bitget python wrapper with rest API, websocket API.
 Home-page: https://github.com/cuongitl/python-bitget
 Author: Cuongitl
 Author-email: 
 License: MIT
 Keywords: Cuongitl bitget api restapi websocketapi example-python-bitget
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/cuongitl/python-bitget/-/blob/main/LICENSE)
 [![python-bitget Version](https://img.shields.io/pypi/v/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Python Versions](https://img.shields.io/pypi/pyversions/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Day](https://img.shields.io/pypi/dd/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Week](https://img.shields.io/pypi/dw/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Month](https://img.shields.io/pypi/dm/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
+[![Downloads](https://static.pepy.tech/badge/python-bitget)](https://pypi.org/project/python-bitget/)
 
 [bitget](https://www.bitget.com/en/referral/register?from=referral&clacCode=6EKP94LE) is a cryptocurrency derivatives exchange.
 
 This is a wrapper around the Bitget API as described on Bitget, including all features the API provides using clear and readable objects, both for the REST  as the websocket API.
 
  
 I am in no way affiliated with Bitget, use at your own risk.
@@ -99,24 +100,27 @@
 client.subscribe(channels, on_message)
 ```
 
 ## Donate / Sponsor
 I develop and maintain this package on my own for free in my spare time. 
 Donations are greatly appreciated. If you prefer to donate any other currency please contact me.
 
-* **BTC**:  `3LrqgdMbToh1mAD3sjhbv3oaEppXY7hkae`
+* **BTC**:  `19rvFC79eVoCMHxJ44hB3GLhiD2HHsMJoZ`
 
-* **BTC**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **BTC**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
 
-* **USDT**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **USDT**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
+
+* **USDT**:  `TCdyZs2mRhwYpCB5dZqiXEUoYRfiVJuq1H`  (TRC20)
 
 * **BGB**:  `0x3ee4ca7cc911ad4e423dec2ae8f2846e9a6a0a77`  (ERC-20)
 
-## Communities
-* Telegram: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+## Communities - Telegram
+* Bitget: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+* Author: [Cuongitl](https://t.me/Cuongitl)
 
 ## Release Notes
 The release notes can be found
 [here.](https://github.com/cuongitl/python-bitget/blob/master/release_notes.md)
 
 ## Contribution
 * Fork this repository.
```

### Comparing `python-bitget-1.0.6/README.md` & `python-bitget-1.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/cuongitl/python-bitget/-/blob/main/LICENSE)
 [![python-bitget Version](https://img.shields.io/pypi/v/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Python Versions](https://img.shields.io/pypi/pyversions/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Day](https://img.shields.io/pypi/dd/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Week](https://img.shields.io/pypi/dw/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Month](https://img.shields.io/pypi/dm/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
+[![Downloads](https://static.pepy.tech/badge/python-bitget)](https://pypi.org/project/python-bitget/)
 
 [bitget](https://www.bitget.com/en/referral/register?from=referral&clacCode=6EKP94LE) is a cryptocurrency derivatives exchange.
 
 This is a wrapper around the Bitget API as described on Bitget, including all features the API provides using clear and readable objects, both for the REST  as the websocket API.
 
  
 I am in no way affiliated with Bitget, use at your own risk.
@@ -81,24 +82,27 @@
 client.subscribe(channels, on_message)
 ```
 
 ## Donate / Sponsor
 I develop and maintain this package on my own for free in my spare time. 
 Donations are greatly appreciated. If you prefer to donate any other currency please contact me.
 
-* **BTC**:  `3LrqgdMbToh1mAD3sjhbv3oaEppXY7hkae`
+* **BTC**:  `19rvFC79eVoCMHxJ44hB3GLhiD2HHsMJoZ`
 
-* **BTC**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **BTC**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
 
-* **USDT**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **USDT**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
+
+* **USDT**:  `TCdyZs2mRhwYpCB5dZqiXEUoYRfiVJuq1H`  (TRC20)
 
 * **BGB**:  `0x3ee4ca7cc911ad4e423dec2ae8f2846e9a6a0a77`  (ERC-20)
 
-## Communities
-* Telegram: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+## Communities - Telegram
+* Bitget: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+* Author: [Cuongitl](https://t.me/Cuongitl)
 
 ## Release Notes
 The release notes can be found
 [here.](https://github.com/cuongitl/python-bitget/blob/master/release_notes.md)
 
 ## Contribution
 * Fork this repository.
```

### Comparing `python-bitget-1.0.6/pybitget/client.py` & `python-bitget-1.0.7/pybitget/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,27 +180,29 @@
             params["symbol"] = symbol
             params["limit"] = limit
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/fills', params)
         else:
             logger.error("pls check args")
             return False
 
-    def mix_get_candles(self, symbol, granularity, startTime, endTime):
+    def mix_get_candles(self, symbol, granularity, startTime, endTime, kLineType='market', limit=100):
         """
         Get Candle Data: https://bitgetlimited.github.io/apidoc/en/mix/#get-candle-data
         Limit rule: 20 times/1s (IP)
         Required: symbol, granularity, startTime, endTime
         :return:
         """
         params = {}
         if symbol and granularity and startTime and endTime:
             params["symbol"] = symbol
             params["granularity"] = granularity
             params["startTime"] = startTime
             params["endTime"] = endTime
+            params["kLineType"] = kLineType
+            params["limit"] = limit
             return self._request_with_params(GET, MIX_MARKET_V1_URL + '/candles', params)
         else:
             logger.error("pls check args")
             return False
 
     def mix_get_symbol_index_price(self, symbol):
         """
@@ -610,55 +612,66 @@
             params["marginCoin"] = marginCoin
             params["orderDataList"] = orderDataList
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/batch-orders', params)
         else:
             logger.error("pls check args")
             return False
 
-    def mix_cancel_order(self, symbol, marginCoin, orderId):
+    def mix_cancel_order(self, symbol, marginCoin, orderId='', clientOid=''):
         """
         Cancel Order: https://bitgetlimited.github.io/apidoc/en/mix/#cancel-order
         Limit rule: 10 times/1s (uid)
-        Required: symbol, marginCoin, orderId
+        Required: symbol, marginCoin, orderId or clientOid
+        - Order Id, int64 in string format, 'orderId' or 'clientOid' must have one
+        - Client Order Id, 'orderId' or 'clientOid' must have one
         """
         params = {}
-        if symbol and marginCoin and orderId:
+        if symbol and marginCoin and (orderId != '' or clientOid != ''):
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
-            params["orderId"] = orderId
+            if orderId != '':
+                params["orderId"] = orderId
+            elif clientOid != '':
+                params["clientOid"] = clientOid
+
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/cancel-order', params)
         else:
             logger.error("pls check args")
             return False
 
-    def mix_batch_cancel_orders(self, symbol, marginCoin, orderIds):
+    def mix_batch_cancel_orders(self, symbol, marginCoin, orderId: list = None, clientOid: list = None):
         """ Batch Cancel Order
-        https://bitgetlimited.github.io/apidoc/en/mix/#cancel-order
+        https://bitgetlimited.github.io/apidoc/en/mix/#batch-cancel-order
         Limit rule: 10 times/1s (uid)
-        Required: symbol, marginCoin, orderIds
+        Required: symbol, marginCoin, orderIds or clientOids
+        - Order Id list, int64 in string format, 'orderIds' or 'clientOids' must have one
+        - Client Order Id list, 'orderIds' or 'clientOids' must have one
         """
         params = {}
         if symbol and marginCoin and orderIds:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
-            params["orderIds"] = orderIds
+            if orderId is not None:
+                params["orderId"] = orderId
+            elif clientOid is not None:
+                params["clientOid"] = clientOid
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/cancel-batch-orders', params)
         else:
             logger.error("pls check args")
             return False
 
     def mix_cancel_all_orders(self, productType, marginCoin):
         """ Cancel All Order
         https://bitgetlimited.github.io/apidoc/en/mix/#cancel-all-order
         Limit rule: 10 times/1s (uid)
 
         Required: productType, marginCoin
         """
         params = {}
-        if productType and orderId:
+        if productType and marginCoin:
             params["productType"] = productType
             params["marginCoin"] = marginCoin
             return self._request_with_params(POST, MIX_ORDER_V1_URL + '/cancel-all-orders', params)
         else:
             logger.error("pls check args")
             return False
 
@@ -681,15 +694,15 @@
         Get All Open Order:::https://bitgetlimited.github.io/apidoc/en/mix/#get-all-open-order
         Required: productType
         :return:
         """
         params = {}
         if productType:
             params["productType"] = productType
-            if marginCoin:
+            if marginCoin is not None:
                 params["marginCoin"] = marginCoin
             return self._request_with_params(GET, MIX_ORDER_V1_URL + '/marginCoinCurrent', params)
         else:
             logger.error("pls check args")
             return False
 
     def mix_get_history_orders(self, symbol, startTime, endTime, pageSize, lastEndId='', isPre=False):
@@ -984,14 +997,15 @@
         Limit rule: 10 times/1s (uid)
         Required: symbol, marginCoin, orderId, triggerPrice, planType
         """
         params = {}
         if symbol and marginCoin and orderId and triggerPrice and planType:
             params["symbol"] = symbol
             params["marginCoin"] = marginCoin
+            params["orderId"] = orderId
             params["triggerPrice"] = triggerPrice
             params["planType"] = planType
             return self._request_with_params(POST, MIX_PLAN_V1_URL + '/modifyTPSLPlan', params)
         else:
             logger.error("pls check args")
             return False
```

### Comparing `python-bitget-1.0.6/pybitget/enums.py` & `python-bitget-1.0.7/pybitget/enums.py`

 * *Files identical despite different names*

### Comparing `python-bitget-1.0.6/pybitget/exceptions.py` & `python-bitget-1.0.7/pybitget/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-bitget-1.0.6/pybitget/stream.py` & `python-bitget-1.0.7/pybitget/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         self.send_message(WS_OP_SUBSCRIBE, channels)
 
     def unsubscribe(self, channels):
         try:
             for channel in channels:
                 if channel in self.__scribe_map:
-                    del self.__scribe_map[chanel]
+                    del self.__scribe_map[channel]
 
             for channel in channels:
                 if channel in self.__all_suribe:
                     self.__all_suribe.remove(channel)
 
             self.send_message(WS_OP_UNSUBSCRIBE, channels)
         except Exception as e:
```

### Comparing `python-bitget-1.0.6/pybitget/utils.py` & `python-bitget-1.0.7/pybitget/utils.py`

 * *Files identical despite different names*

### Comparing `python-bitget-1.0.6/python_bitget.egg-info/PKG-INFO` & `python-bitget-1.0.7/python_bitget.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bitget
-Version: 1.0.6
+Version: 1.0.7
 Summary: bitget python wrapper with rest API, websocket API.
 Home-page: https://github.com/cuongitl/python-bitget
 Author: Cuongitl
 Author-email: 
 License: MIT
 Keywords: Cuongitl bitget api restapi websocketapi example-python-bitget
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/cuongitl/python-bitget/-/blob/main/LICENSE)
 [![python-bitget Version](https://img.shields.io/pypi/v/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Python Versions](https://img.shields.io/pypi/pyversions/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Day](https://img.shields.io/pypi/dd/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Week](https://img.shields.io/pypi/dw/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
 [![python-bitget Downloads Per Month](https://img.shields.io/pypi/dm/python-bitget?logo=pypi)](https://pypi.org/project/python-bitget/)
+[![Downloads](https://static.pepy.tech/badge/python-bitget)](https://pypi.org/project/python-bitget/)
 
 [bitget](https://www.bitget.com/en/referral/register?from=referral&clacCode=6EKP94LE) is a cryptocurrency derivatives exchange.
 
 This is a wrapper around the Bitget API as described on Bitget, including all features the API provides using clear and readable objects, both for the REST  as the websocket API.
 
  
 I am in no way affiliated with Bitget, use at your own risk.
@@ -99,24 +100,27 @@
 client.subscribe(channels, on_message)
 ```
 
 ## Donate / Sponsor
 I develop and maintain this package on my own for free in my spare time. 
 Donations are greatly appreciated. If you prefer to donate any other currency please contact me.
 
-* **BTC**:  `3LrqgdMbToh1mAD3sjhbv3oaEppXY7hkae`
+* **BTC**:  `19rvFC79eVoCMHxJ44hB3GLhiD2HHsMJoZ`
 
-* **BTC**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **BTC**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
 
-* **USDT**:  `0x329a9F2b01aDA25F15eAE4C633d3bed8442c7BC6`  (BSC)
+* **USDT**:  `0xab4686635a02dff0babedddfee813d325f56cfb8`  (BEP20)
+
+* **USDT**:  `TCdyZs2mRhwYpCB5dZqiXEUoYRfiVJuq1H`  (TRC20)
 
 * **BGB**:  `0x3ee4ca7cc911ad4e423dec2ae8f2846e9a6a0a77`  (ERC-20)
 
-## Communities
-* Telegram: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+## Communities - Telegram
+* Bitget: [Bitget OPENAPI](https://t.me/bitgetOpenapi)
+* Author: [Cuongitl](https://t.me/Cuongitl)
 
 ## Release Notes
 The release notes can be found
 [here.](https://github.com/cuongitl/python-bitget/blob/master/release_notes.md)
 
 ## Contribution
 * Fork this repository.
```

### Comparing `python-bitget-1.0.6/setup.py` & `python-bitget-1.0.7/setup.py`

 * *Files identical despite different names*

