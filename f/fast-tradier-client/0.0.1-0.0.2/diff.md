# Comparing `tmp/fast_tradier_client-0.0.1.tar.gz` & `tmp/fast_tradier_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-0.0.1.tar", last modified: Sun Aug  6 21:25:52 2023, max compression
+gzip compressed data, was "fast_tradier_client-0.0.2.tar", last modified: Sun Aug  6 21:46:22 2023, max compression
```

## Comparing `fast_tradier_client-0.0.1.tar` & `fast_tradier_client-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.290759 fast_tradier_client-0.0.1/
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1073 2023-08-06 21:19:35.000000 fast_tradier_client-0.0.1/LICENSE
--rw-r--r--   0 guoliangwang   (501) staff       (20)     7973 2023-08-06 21:25:52.290591 fast_tradier_client-0.0.1/PKG-INFO
--rw-r--r--   0 guoliangwang   (501) staff       (20)     7346 2023-08-06 21:25:47.000000 fast_tradier_client-0.0.1/README.md
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.285024 fast_tradier_client-0.0.1/fast_tradier/
--rw-r--r--   0 guoliangwang   (501) staff       (20)    14048 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/FastTradierAsyncClient.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)    13764 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/FastTradierClient.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.285989 fast_tradier_client-0.0.1/fast_tradier/interfaces/
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1971 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1835 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/interfaces/IBrokerClient.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)      180 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/interfaces/IModel.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)      281 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.287133 fast_tradier_client-0.0.1/fast_tradier/models/
--rw-r--r--   0 guoliangwang   (501) staff       (20)      392 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/DataClassModelBase.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1248 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/models/ModelBase.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)     5173 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/models/OptionOrder.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1872 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/models/TOSTradierConverter.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/models/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.287658 fast_tradier_client-0.0.1/fast_tradier/models/account/
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1974 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/account/AccountBalance.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)      359 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/account/Position.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.288162 fast_tradier_client-0.0.1/fast_tradier/models/market_data/
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1841 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/market_data/Quote.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1790 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/market_data/TradierQuote.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.288292 fast_tradier_client-0.0.1/fast_tradier/models/trading/
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.288759 fast_tradier_client-0.0.1/fast_tradier/utils/
--rw-r--r--   0 guoliangwang   (501) staff       (20)      216 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/fast_tradier/utils/OptionUtils.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)      758 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/utils/TimeUtils.py
--rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.1/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:25:52.290275 fast_tradier_client-0.0.1/fast_tradier_client.egg-info/
--rw-r--r--   0 guoliangwang   (501) staff       (20)     7973 2023-08-06 21:25:52.000000 fast_tradier_client-0.0.1/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 guoliangwang   (501) staff       (20)     1090 2023-08-06 21:25:52.000000 fast_tradier_client-0.0.1/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 guoliangwang   (501) staff       (20)        1 2023-08-06 21:25:52.000000 fast_tradier_client-0.0.1/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 guoliangwang   (501) staff       (20)       13 2023-08-06 21:25:52.000000 fast_tradier_client-0.0.1/fast_tradier_client.egg-info/top_level.txt
--rw-r--r--   0 guoliangwang   (501) staff       (20)      700 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.1/pyproject.toml
--rw-r--r--   0 guoliangwang   (501) staff       (20)       38 2023-08-06 21:25:52.290848 fast_tradier_client-0.0.1/setup.cfg
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.121331 fast_tradier_client-0.0.2/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1073 2023-08-06 21:19:35.000000 fast_tradier_client-0.0.2/LICENSE
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     7997 2023-08-06 21:46:22.121154 fast_tradier_client-0.0.2/PKG-INFO
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     7370 2023-08-06 21:46:16.000000 fast_tradier_client-0.0.2/README.md
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.117540 fast_tradier_client-0.0.2/fast_tradier/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)    14048 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/FastTradierAsyncClient.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)    13764 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/FastTradierClient.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.118266 fast_tradier_client-0.0.2/fast_tradier/interfaces/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1971 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1835 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/interfaces/IBrokerClient.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      180 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/interfaces/IModel.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      281 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.118772 fast_tradier_client-0.0.2/fast_tradier/models/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      392 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/DataClassModelBase.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1248 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/models/ModelBase.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/models/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.119199 fast_tradier_client-0.0.2/fast_tradier/models/account/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1974 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/account/AccountBalance.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      359 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/account/Position.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.119585 fast_tradier_client-0.0.2/fast_tradier/models/market_data/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1841 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/market_data/Quote.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1790 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/market_data/TradierQuote.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.119930 fast_tradier_client-0.0.2/fast_tradier/models/trading/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     5173 2023-08-06 21:46:16.000000 fast_tradier_client-0.0.2/fast_tradier/models/trading/OptionOrder.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1872 2023-08-06 21:46:16.000000 fast_tradier_client-0.0.2/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.120467 fast_tradier_client-0.0.2/fast_tradier/utils/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      216 2023-08-06 21:15:09.000000 fast_tradier_client-0.0.2/fast_tradier/utils/OptionUtils.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      758 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/utils/TimeUtils.py
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        0 2023-08-06 16:50:02.000000 fast_tradier_client-0.0.2/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 guoliangwang   (501) staff       (20)        0 2023-08-06 21:46:22.120968 fast_tradier_client-0.0.2/fast_tradier_client.egg-info/
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     7997 2023-08-06 21:46:22.000000 fast_tradier_client-0.0.2/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 guoliangwang   (501) staff       (20)     1106 2023-08-06 21:46:22.000000 fast_tradier_client-0.0.2/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 guoliangwang   (501) staff       (20)        1 2023-08-06 21:46:22.000000 fast_tradier_client-0.0.2/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 guoliangwang   (501) staff       (20)       13 2023-08-06 21:46:22.000000 fast_tradier_client-0.0.2/fast_tradier_client.egg-info/top_level.txt
+-rw-r--r--   0 guoliangwang   (501) staff       (20)      700 2023-08-06 21:46:16.000000 fast_tradier_client-0.0.2/pyproject.toml
+-rw-r--r--   0 guoliangwang   (501) staff       (20)       38 2023-08-06 21:46:22.121393 fast_tradier_client-0.0.2/setup.cfg
```

### Comparing `fast_tradier_client-0.0.1/LICENSE` & `fast_tradier_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/PKG-INFO` & `fast_tradier_client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Tradier client for trading stocks and options through Tradier API
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,16 +87,16 @@
 
 2. Test Client:
 ```python
 
 from fast_tradier.FastTradierAsyncClient import FastTradierAsyncClient
 from fast_tradier.FastTradierClient import FastTradierClient
 from fast_tradier.models.market_data.Quote import Quote
-from fast_tradier.models.OptionOrder import OptionLeg
-from fast_tradier.models.OptionOrder import OptionOrder
+from fast_tradier.models.trading.OptionOrder import OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder
 
 import asyncio
 
 #TODO: replace the client_id and sandbox access token with yours
 sandbox_client_id = 'VA123456789'
 sandbox_at = 'abcdefghijklmnopqrstuvwxyzzzz'
 
@@ -193,15 +193,15 @@
 ```
 
 3. Test model like `TradierQuote`:
 
 ```python
 import json
 from fast_tradier.models.market_data.TradierQuote import TradierQuote
-from fast_tradier.models.OptionOrder import OptionOrder, OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder, OptionLeg
 
 quote1 = TradierQuote(symbol='spx', type='stock', open=1000.0, high=2012.1, low=1999.0, close=4910.1, volume=30000, bid=1.2, ask=2.3, last_price=4.3)
 json_obj = quote1.serialize()
 print('serialize: ', json_obj)
 
 quote2 = TradierQuote.deserialize_from_json(json_obj)
 print('quote2.ask: ', quote2.ask)
```

### Comparing `fast_tradier_client-0.0.1/README.md` & `fast_tradier_client-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 2. Test Client:
 ```python
 
 from fast_tradier.FastTradierAsyncClient import FastTradierAsyncClient
 from fast_tradier.FastTradierClient import FastTradierClient
 from fast_tradier.models.market_data.Quote import Quote
-from fast_tradier.models.OptionOrder import OptionLeg
-from fast_tradier.models.OptionOrder import OptionOrder
+from fast_tradier.models.trading.OptionOrder import OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder
 
 import asyncio
 
 #TODO: replace the client_id and sandbox access token with yours
 sandbox_client_id = 'VA123456789'
 sandbox_at = 'abcdefghijklmnopqrstuvwxyzzzz'
 
@@ -179,15 +179,15 @@
 ```
 
 3. Test model like `TradierQuote`:
 
 ```python
 import json
 from fast_tradier.models.market_data.TradierQuote import TradierQuote
-from fast_tradier.models.OptionOrder import OptionOrder, OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder, OptionLeg
 
 quote1 = TradierQuote(symbol='spx', type='stock', open=1000.0, high=2012.1, low=1999.0, close=4910.1, volume=30000, bid=1.2, ask=2.3, last_price=4.3)
 json_obj = quote1.serialize()
 print('serialize: ', json_obj)
 
 quote2 = TradierQuote.deserialize_from_json(json_obj)
 print('quote2.ask: ', quote2.ask)
```

### Comparing `fast_tradier_client-0.0.1/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-0.0.2/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/FastTradierClient.py` & `fast_tradier_client-0.0.2/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-0.0.2/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-0.0.2/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/ModelBase.py` & `fast_tradier_client-0.0.2/fast_tradier/models/ModelBase.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/OptionOrder.py` & `fast_tradier_client-0.0.2/fast_tradier/models/trading/OptionOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/TOSTradierConverter.py` & `fast_tradier_client-0.0.2/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-0.0.2/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-0.0.2/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-0.0.2/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-0.0.2/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.0.1/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-0.0.2/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Tradier client for trading stocks and options through Tradier API
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,16 +87,16 @@
 
 2. Test Client:
 ```python
 
 from fast_tradier.FastTradierAsyncClient import FastTradierAsyncClient
 from fast_tradier.FastTradierClient import FastTradierClient
 from fast_tradier.models.market_data.Quote import Quote
-from fast_tradier.models.OptionOrder import OptionLeg
-from fast_tradier.models.OptionOrder import OptionOrder
+from fast_tradier.models.trading.OptionOrder import OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder
 
 import asyncio
 
 #TODO: replace the client_id and sandbox access token with yours
 sandbox_client_id = 'VA123456789'
 sandbox_at = 'abcdefghijklmnopqrstuvwxyzzzz'
 
@@ -193,15 +193,15 @@
 ```
 
 3. Test model like `TradierQuote`:
 
 ```python
 import json
 from fast_tradier.models.market_data.TradierQuote import TradierQuote
-from fast_tradier.models.OptionOrder import OptionOrder, OptionLeg
+from fast_tradier.models.trading.OptionOrder import OptionOrder, OptionLeg
 
 quote1 = TradierQuote(symbol='spx', type='stock', open=1000.0, high=2012.1, low=1999.0, close=4910.1, volume=30000, bid=1.2, ask=2.3, last_price=4.3)
 json_obj = quote1.serialize()
 print('serialize: ', json_obj)
 
 quote2 = TradierQuote.deserialize_from_json(json_obj)
 print('quote2.ask: ', quote2.ask)
```

### Comparing `fast_tradier_client-0.0.1/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-0.0.2/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 fast_tradier/interfaces/IBrokerAsyncClient.py
 fast_tradier/interfaces/IBrokerClient.py
 fast_tradier/interfaces/IModel.py
 fast_tradier/interfaces/IRealTimeQuoteProvider.py
 fast_tradier/interfaces/__init__.py
 fast_tradier/models/DataClassModelBase.py
 fast_tradier/models/ModelBase.py
-fast_tradier/models/OptionOrder.py
-fast_tradier/models/TOSTradierConverter.py
 fast_tradier/models/__init__.py
 fast_tradier/models/account/AccountBalance.py
 fast_tradier/models/account/Position.py
 fast_tradier/models/account/__init__.py
 fast_tradier/models/market_data/Quote.py
 fast_tradier/models/market_data/TradierQuote.py
 fast_tradier/models/market_data/__init__.py
+fast_tradier/models/trading/OptionOrder.py
+fast_tradier/models/trading/TOSTradierConverter.py
 fast_tradier/models/trading/__init__.py
 fast_tradier/utils/OptionUtils.py
 fast_tradier/utils/TimeUtils.py
 fast_tradier/utils/__init__.py
 fast_tradier_client.egg-info/PKG-INFO
 fast_tradier_client.egg-info/SOURCES.txt
 fast_tradier_client.egg-info/dependency_links.txt
```

### Comparing `fast_tradier_client-0.0.1/pyproject.toml` & `fast_tradier_client-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

