# Comparing `tmp/hades-core-0.0.2.tar.gz` & `tmp/hades-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-core-0.0.2.tar", last modified: Wed Jul 26 14:07:14 2023, max compression
+gzip compressed data, was "hades-core-0.0.3.tar", last modified: Sun Aug  6 09:08:57 2023, max compression
```

## Comparing `hades-core-0.0.2.tar` & `hades-core-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 14:07:03.000000 hades-core-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-26 14:07:14.928542 hades-core-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-26 14:07:03.000000 hades-core-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/exchange/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/messager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-26 14:07:03.000000 hades-core-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:07:14.928542 hades-core-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 09:08:47.000000 hades-core-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-08-06 09:08:57.941694 hades-core-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-06 09:08:47.000000 hades-core-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades/core/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/backtesting/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/backtesting/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades/core/exchange/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/exchange/binance_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/exchange/okx_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades/core/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/messager/dingding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/messager/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-06 09:08:47.000000 hades-core-0.0.3/hades/core/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 09:08:57.941694 hades-core-0.0.3/hades_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-08-06 09:08:57.000000 hades-core-0.0.3/hades_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-06 09:08:57.000000 hades-core-0.0.3/hades_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 09:08:57.000000 hades-core-0.0.3/hades_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-06 09:08:57.000000 hades-core-0.0.3/hades_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 09:08:57.000000 hades-core-0.0.3/hades_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-08-06 09:08:47.000000 hades-core-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 09:08:57.941694 hades-core-0.0.3/setup.cfg
```

### Comparing `hades-core-0.0.2/LICENSE` & `hades-core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hades-core-0.0.2/PKG-INFO` & `hades-core-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hades-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: cryptocurrency trading bot
 Author-email: Gary Guo <gary.guo.china@gmail.com>
 Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -229,15 +229,15 @@
 ### 1. Setup Environment
 
 ```shell
 python -m venv runtime
 runtime\Scripts\activate
 pip install -r requirements.txt
 # if requirements.txt not work
-pip3 install python-okx websockets requests binance-futures-connector
+pip3 install python-okx websockets requests binance-futures-connector python-telegram-bot pydantic
 ```
 
 ### 2. Change Configuration
 
 copy `example.conf` and rename to `app.conf` , change parameter
 
 ```ini
@@ -251,12 +251,18 @@
 passphrase       = passphrase
 ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
 ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
 ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
 domain           = https://aws.okx.com
 useServerTime    = False
 
-[notification]
+# optional
+[dingding]
 token            = token
 prefix           = prefix
 period           = 8-23
+
+# optional
+[telegram]
+token            = token
+period           = 8-23
 ```
```

### Comparing `hades-core-0.0.2/README.md` & `hades-core-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ### 1. Setup Environment
 
 ```shell
 python -m venv runtime
 runtime\Scripts\activate
 pip install -r requirements.txt
 # if requirements.txt not work
-pip3 install python-okx websockets requests binance-futures-connector
+pip3 install python-okx websockets requests binance-futures-connector python-telegram-bot pydantic
 ```
 
 ### 2. Change Configuration
 
 copy `example.conf` and rename to `app.conf` , change parameter
 
 ```ini
@@ -29,12 +29,18 @@
 passphrase       = passphrase
 ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
 ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
 ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
 domain           = https://aws.okx.com
 useServerTime    = False
 
-[notification]
+# optional
+[dingding]
 token            = token
 prefix           = prefix
 period           = 8-23
+
+# optional
+[telegram]
+token            = token
+period           = 8-23
 ```
```

### Comparing `hades-core-0.0.2/hades/core/__init__.py` & `hades-core-0.0.3/hades/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import logging
 
-from hades.core.config import TradeBotConf
-from hades.core.messager import Messager
 from hades.core.model import Order, Position, Tick, Bar, Balance, Trade
 from hades.core.strategy import Strategy, Exchange, Subscriber, ExchangeEnum
-from hades.core.exchange.binance import BinanceUMSubscriber
-from hades.core.exchange.okx import OkxSubscriber
+from hades.core.config import TradeBotConf
+from hades.core.exchange import BinanceUMSubscriber, OkxSubscriber
 from hades.core.executor import TradeExecutor
-
+from hades.core.messager import Messenger, MessageFactory, MessageEnum
 
 logging.basicConfig(filename='log.txt',
                     format='%(asctime)s - %(levelname)s - %(name)s - %(funcName)s - %(message)s',
                     level=logging.INFO)
 
 logging.getLogger('okx.websocket.WsClientProtocol').setLevel(logging.ERROR)
 
 __all__ = ['TradeBotConf',
-           'Messager',
            'Strategy',
            'Exchange',
            'Subscriber',
            'ExchangeEnum',
            'BinanceUMSubscriber',
            'OkxSubscriber',
            'TradeExecutor',
            'Order',
            'Position',
            'Tick',
            'Bar',
            'Trade',
-           'Balance']
-
+           'Balance',
+           'Messenger',
+           'MessageEnum',
+           'MessageFactory']
```

### Comparing `hades-core-0.0.2/hades/core/config.py` & `hades-core-0.0.3/hades/core/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,50 @@
+import os
 from configparser import ConfigParser
 from os import path
-import os
 
-BINANCE_API_KEY      = 'BINANCE_API_KEY'
-BINANCE_SECRET_KEY   = 'BINANCE_SECRET_KEY'
+BINANCE_API_KEY = 'BINANCE_API_KEY'
+BINANCE_SECRET_KEY = 'BINANCE_SECRET_KEY'
 
-NOTIFICATION_TOKEN  = 'NOTIFICATION_TOKEN'
+NOTIFICATION_TOKEN = 'NOTIFICATION_TOKEN'
 NOTIFICATION_PREFIX = 'NOTIFICATION_PREFIX'
 NOTIFICATION_PERIOD = 'NOTIFICATION_PERIOD'
 
+
 class TradeBotConf:
     def __init__(self, conf: ConfigParser = None) -> None:
         if not conf:
-            self.binance               = {}
-            self.binance['apiKey']     = os.environ.get(BINANCE_API_KEY)
-            self.binance['secretKey']  = os.environ.get(BINANCE_SECRET_KEY)
-            self.token                 = os.environ.get(NOTIFICATION_TOKEN)
-            self.prefix                = os.environ.get(NOTIFICATION_PREFIX)
-            self.period                = os.environ.get(NOTIFICATION_PERIOD)
+            self.binance = {'apiKey': os.environ.get(BINANCE_API_KEY), 'secretKey': os.environ.get(BINANCE_SECRET_KEY)}
+            self.token = os.environ.get(NOTIFICATION_TOKEN)
+            self.prefix = os.environ.get(NOTIFICATION_PREFIX)
+            self.period = os.environ.get(NOTIFICATION_PERIOD)
         else:
             if conf.has_section('okx'):
-                self.okx                   = {}
-                self.okx['apiKey']         = conf['okx']['apiKey']
-                self.okx['secretKey']      = conf['okx']['secretKey']
-                self.okx['passphrase']     = conf['okx']['passphrase']
-                self.okx['ws_private']     = conf['okx']['ws_private']
-                self.okx['ws_public']      = conf['okx']['ws_public']
-                self.okx['ws_business']    = conf['okx']['ws_business']
-                self.okx['domain']         = conf['okx']['domain']
-                self.okx['useServerTime']  = conf.getboolean('okx', 'useServerTime')
+                self.okx = {
+                    'apiKey': conf['okx']['apiKey'],
+                    'secretKey': conf['okx']['secretKey'],
+                    'passphrase': conf['okx']['passphrase'],
+                    'ws_private': conf['okx']['ws_private'],
+                    'ws_public': conf['okx']['ws_public'],
+                    'ws_business': conf['okx']['ws_business'],
+                    'domain': conf['okx']['domain'],
+                    'useServerTime': conf.getboolean('okx', 'useServerTime')}
             if conf.has_section('binance'):
-                self.binance               = {}
-                self.binance['apiKey']     = conf['binance']['apiKey']
-                self.binance['secretKey']  = conf['binance']['secretKey']
-            if conf.has_section('notification'):
-                self.token                 = conf['notification']['token']
-                self.prefix                = conf['notification']['prefix']
-                self.period                = conf['notification']['period']
-        
-    
+                self.binance = {'apiKey': conf['binance']['apiKey'], 'secretKey': conf['binance']['secretKey']}
+            if conf.has_section('dingding'):
+                self.token = conf['dingding']['token']
+                self.prefix = conf['dingding']['prefix']
+                self.period = conf['dingding']['period']
+            if conf.has_section('telegram'):
+                self.token = conf['telegram']['token']
+                self.period = conf['telegram']['period']
+
     @staticmethod
     def load():
         parser = ConfigParser()
-        ROOT_DIR = os.path.abspath(os.curdir)
-        conf_file = path.join(ROOT_DIR, 'app.conf')
+        root_dir = os.path.abspath(os.curdir)
+        conf_file = path.join(root_dir, 'app.conf')
         if path.exists(conf_file):
             parser.read(conf_file, encoding='UTF-8')
             return TradeBotConf(parser)
         else:
             return TradeBotConf()
```

### Comparing `hades-core-0.0.2/hades/core/exchange/binance.py` & `hades-core-0.0.3/hades/core/exchange/binance_ex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,257 +1,276 @@
-from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
-from binance.um_futures import UMFutures
-
 import asyncio
-from datetime import datetime
-from typing import List
 import logging
+from datetime import datetime
+from typing import List, Optional
+
+from binance.um_futures import UMFutures
+from binance.websocket.um_futures.websocket_client import UMFuturesWebsocketClient
+
+from hades.core import TradeBotConf, Strategy, Exchange, Subscriber, Order, Position, Balance, Tick, Bar, Trade
 
-from hades.core import TradeBotConf, Strategy, Subscriber, Exchange,  Order, Position, Balance, Tick, Bar, Trade
 
 class BinanceUMExchangeClient(Exchange):
-    def __init__(self,  conf: TradeBotConf) -> None:
+    def __init__(self, conf: TradeBotConf) -> None:
         self.conf = {
             'key': conf.binance['apiKey'],
             'secret': conf.binance['secretKey']
         }
         self.client = UMFutures(**self.conf)
-       
+
     # Account Info
     def get_positions(self) -> List[Position]:
         response: List[Position] = []
         for pos in self.client.account()['positions']:
             if float(pos['positionAmt']) != 0:
                 response.append(Position(
                     symbol=pos['symbol'],
-                    instrumentType='SWAP',
+                    instrument_type='SWAP',
                     side=pos['positionSide'],
                     quantity=float(pos['positionAmt']),
                     unrealized_profit=round(float(pos['unrealizedProfit']), 3),
-                    unrealized_profit_ratio = round(float(pos['unrealizedProfit']) / float(pos['initialMargin']) * 100, 2),
+                    unrealized_profit_ratio=round(float(pos['unrealizedProfit']) / float(pos['initialMargin']) * 100,
+                                                  2),
                     mode='isolated' if pos['isolated'] else 'cross',
                     price=float(pos['entryPrice']),
                     timestamp=datetime.fromtimestamp(int(pos['updateTime'] / 1000))
                 ))
         return response
 
     def get_balance(self):
         response: List[Balance] = []
         for record in self.client.balance(recvWindow=6000):
             if float(record['availableBalance']) != 0:
-                response.append(Balance(asset=record['asset'], availableBalance=float(record['availableBalance'])))
+                response.append(Balance(asset=record['asset'], available_balance=float(record['availableBalance'])))
         return response
 
-    
     def place_buy_order(self, symbol: str, size: float, price: float):
         params = {
             'symbol': symbol,
             'side': 'BUY',
             'type': 'LIMIT',
             'timeInForce': 'GTC',
             'quantity': size,
             'price': price
         }
         return self.client.new_order(**params)
-    
+
     def get_orders(self) -> List[Order]:
         orders = []
         for record in self.client.get_orders():
             orders.append(Order(
-                orderId=record['orderId'],
-                orderType=record['type'],
+                order_id=record['orderId'],
+                order_type=record['type'],
                 symbol=record['symbol'],
-                instrumentType='SWAP',
+                instrument_type='SWAP',
                 price=float(record['price']),
                 status=record['status'],
                 side=record['side'],
                 quantity=float(record['origQty']),
                 timestamp=datetime.fromtimestamp(record['updateTime'] / 1000)
             ))
         return orders
-    
+
     def place_sell_order(self, symbol: str, size: float, price: float):
         params = {
             'symbol': symbol,
             'side': 'SELL',
             'type': 'LIMIT',
             'timeInForce': 'GTC',
             'quantity': size,
             'price': price
         }
         return self.client.new_order(**params)
-    
-    def cancel_order(self, orderId: str, symbol: str):
-        return self.client.cancel_order(symbol=symbol, orderId=int(orderId))
-    
+
+    def cancel_order(self, order_id: str, symbol: str):
+        return self.client.cancel_order(symbol=symbol, orderId=int(order_id))
+
     def close_position(self, symbol: str):
         pass
 
     # get latest 100 bar
     def get_candlesticks(self, symbol: str, bar: str = '1m', limit: int = 100) -> List[Bar]:
-        bars =[]
+        bars = []
         for bar in self.client.klines(symbol=symbol, interval=bar, limit=limit):
             _stamp, _open, _high, _low, _close, _vol, *_ = bar
             bars.append(Bar(
                 timestamp=datetime.fromtimestamp(_stamp / 1000),
                 open=float(_open),
                 high=float(_high),
                 low=float(_low),
                 close=float(_close),
                 vol=float(_vol)
             ))
         return bars
 
-                            
     def get_trades(self, symbol: str) -> List[Trade]:
         trades: List[Trade] = []
         cache = {}
         for record in self.client.get_account_trades(symbol=symbol):
             if record['commissionAsset'] == 'USDT':
-                priceToUSDT = 1
+                price_to_usdt = 1
             else:
                 if record['commissionAsset'] not in cache:
-                    priceToUSDT = float(self.client.mark_price(symbol=f"{record['commissionAsset']}USDT")['markPrice'])
-                    cache[record['commissionAsset']] = priceToUSDT
+                    price_to_usdt = float(
+                        self.client.mark_price(symbol=f"{record['commissionAsset']}USDT")['markPrice'])
+                    cache[record['commissionAsset']] = price_to_usdt
                 else:
-                    priceToUSDT = cache[record['commissionAsset']]
-                
+                    price_to_usdt = cache[record['commissionAsset']]
+
             trades.append(Trade(
-                 id=record['id'],
-                 orderId=record['orderId'],
-                 symbol=record['symbol'],
-                 side=record['side'],
-                 price=float(record['price']),
-                 quantity=float(record['qty']),
-                 realizedPnl=float(record['realizedPnl']),
-                 marginAsset=record['marginAsset'],
-                 quoteQty=float(record['quoteQty']),
-                 commissionToUSDT=priceToUSDT * float(record['commission']),
-                 commission=float(record['commission']),
-                 commissionAsset=record['commissionAsset'],
-                 timestamp=datetime.fromtimestamp(record['time'] / 1000),
-                 maker=bool(record['maker'])
+                id=str(record['id']),
+                order_id=str(record['orderId']),
+                symbol=record['symbol'],
+                side=record['side'],
+                price=float(record['price']),
+                quantity=float(record['qty']),
+                realized_pnl=float(record['realizedPnl']),
+                margin_asset=record['marginAsset'],
+                quote_quantity=float(record['quoteQty']),
+                commission_to_usdt=price_to_usdt * float(record['commission']),
+                commission=float(record['commission']),
+                commission_asset=record['commissionAsset'],
+                timestamp=datetime.fromtimestamp(record['time'] / 1000),
+                maker=bool(record['maker'])
             ))
         return trades
 
+
+def _process_positions(msg_stamp: int, record: dict) -> List[Position]:
+    # handle positions
+    positions: List[Position] = []
+    for _position in record.get('P'):
+        if float(_position['iw']) != 0:
+            positions.append(Position(
+                symbol=_position.get('s'),
+                instrument_type='SWAP',
+                side=_position.get('ps'),
+                quantity=float(_position['pa']),
+                unrealized_profit=round(float(_position['up']), 3),
+                unrealized_profit_ratio=round(float(_position['up']) / float(_position['iw']) * 100, 2),
+                mode=_position.get('mt'),
+                price=float(_position['ep']),  # entry price
+                timestamp=datetime.fromtimestamp(int(msg_stamp / 1000))
+            ))
+    return positions
+
+
+def _process_order(data: dict) -> Order:
+    record = data.get('o', {})
+    logging.info(record)
+    order = Order(
+        order_id=str(record.get('i')),
+        # MARKET
+        # LIMIT
+        # STOP
+        # TAKE_PROFIT
+        # LIQUIDATION
+        order_type=record.get('o'),
+        symbol=record.get('s'),
+        instrument_type='SWAP',
+        price=float(record.get('ap')),
+        # NEW
+        # CANCELED
+        # CALCULATED
+        # EXPIRED
+        # TRADE
+        # AMENDMENT
+        status=record.get('x'),
+        # BUY || SELL
+        side=record.get('S'),
+        quantity=float(record.get('q')),
+        timestamp=datetime.fromtimestamp(int(record.get('T')) / 1000)
+    )
+    return order
+
+
+def _process_bar(data: dict, msg_stamp: int) -> Bar:
+    record = data.get('k', {})
+    bar = Bar(
+        timestamp=datetime.fromtimestamp(int(msg_stamp) / 1000),
+        open=float(record['o']),
+        high=float(record['h']),
+        low=float(record['l']),
+        close=float(record['c']),
+        vol=float(record['q']),
+    )
+    return bar
+
+
+def _process_balance(record: dict) -> List[Balance]:
+    balance: List[Balance] = []
+    for record in record.get('B'):
+        balance.append(Balance(
+            asset=record['a'],  # asset
+            available_balance=round(float(record['bc']), 2),  # balance
+        ))
+    return balance
+
+
 class BinanceUMSubscriber(Subscriber):
     def __init__(self, strategy: Strategy) -> None:
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        self.strategy.on_init_exchange(BinanceUMExchangeClient(conf))
-        self.conf = {
-            'key': conf.binance['apiKey'],
-            'secret': conf.binance['secretKey']
+        self.conf: TradeBotConf = TradeBotConf.load()
+        super().__init__(strategy)
+        self.config = {
+            'key': self.conf.binance['apiKey'],
+            'secret': self.conf.binance['secretKey']
         }
-        self.listenKey: str = None
+        self.listenKey: Optional[str] = None
         self.last_auth: datetime = datetime.utcnow()
-        self.last_tick: int = None
-        self.last_bar : int = None
-        
-    
+        self.last_tick: Optional[int] = None
+        self.last_bar: Optional[int] = None
+
+    def get_exchange(self) -> Exchange:
+        return self.strategy.on_init_exchange(BinanceUMExchangeClient(self.conf))
+
     def renew(self):
         logging.info('renew key')
         if self.listenKey:
-            self.client.renew_listen_key(self.listenKey)
-    
+            self.client.renew_listen_key(listenKey=self.listenKey)
+
     def _run(self):
-        self.client = UMFutures(**self.conf)
+        self.client = UMFutures(**self.config)
         self.listenKey = self.client.new_listen_key()['listenKey']
         self.ws = UMFuturesWebsocketClient()
         idx = 1
         for symbol in self.strategy.symbols:
             self.ws.mini_ticker(id=idx, callback=self.handle_message, symbol=symbol)
             idx += 1
         for symbol in self.strategy.symbols:
             for bar_type in self.strategy.klines:
                 self.ws.kline(id=idx, callback=self.handle_message, symbol=symbol, interval=bar_type)
                 idx += 1
-        self.ws.user_data(listen_key=self.listenKey, id=idx+1, callback=self.handle_message)
+        self.ws.user_data(listen_key=self.listenKey, id=idx + 1, callback=self.handle_message)
         self.ws.run()
 
     def run(self) -> asyncio.Task:
         return asyncio.create_task(self._run())
-    
+
     def stop(self):
         self.ws.stop()
 
     def handle_message(self, data: dict):
         if (datetime.utcnow() - self.last_auth).seconds > 60 * 45:
             self.renew()
             self.last_auth = datetime.utcnow()
-        event = data.get('e')
-        msg_stamp = data.get('E')
-        
+        event: str = data.get('e')
+        msg_stamp: int = data.get('E')
+
         if not event:
             return
         elif '24hrMiniTicker' == event:
             if not self.last_tick or msg_stamp - self.last_tick >= 1000:
-                tick = Tick(symbol=data.get('s'), price=round(float(data.get('c')), 4), timestmap=datetime.fromtimestamp(int(msg_stamp / 1000)))
-                self.strategy.on_tick([tick])
+                self.on_tick([Tick(symbol=data.get('s'),
+                                   price=round(float(data.get('c')), 4),
+                                   timestamp=datetime.fromtimestamp(int(msg_stamp / 1000)))])
             self.last_tick = msg_stamp
         elif 'ORDER_TRADE_UPDATE' == event:
-            record = data.get('o', {})
-            logging.info(record)
-            order = Order(
-                orderId=record.get('i'),
-                # MARKET
-                # LIMIT
-                # STOP
-                # TAKE_PROFIT
-                # LIQUIDATION
-                orderType=record.get('o'),
-                symbol=record.get('s'),
-                instrumentType='SWAP',
-                price=float(record.get('ap')),
-                # NEW
-                # CANCELED
-                # CALCULATED
-                # EXPIRED
-                # TRADE
-                # AMENDMENT
-                status=record.get('x'),
-                # BUY || SELL
-                side=record.get('S'),
-                quantity=float(record.get('q')),
-                timestamp=datetime.fromtimestamp(int(record.get('T')) / 1000)
-            )
-            self.strategy.on_order_status([order])
+            self.on_order_status([_process_order(data)])
         elif 'ACCOUNT_UPDATE' == event:
             record = data.get('a', {})
-            # handle positions
-            positions: List[Position] = []
-            for _position in record.get('P'):
-                if float(_position['iw']) != 0:
-                    positions.append(Position(
-                        symbol=_position.get('s'),
-                        instrumentType='SWAP',
-                        side=_position.get('ps'),
-                        quantity=float(_position['pa']),
-                        unrealized_profit=round(float(_position['up']), 3),
-                        unrealized_profit_ratio = round(float(_position['up']) / float(_position['iw']) * 100, 2),
-                        mode=_position.get('mt'),                    
-                        price=float(_position['ep']),            # entry price
-                        timestamp=datetime.fromtimestamp(int(msg_stamp / 1000))
-                    ))
-            self.strategy.on_position_status(positions)
+            self.on_position_status(_process_positions(msg_stamp, record))
             # handle balance
-            balance: List[Balance] = []
-            for record in record.get('B'):
-                balance.append(Balance(
-                    asset=record['a'],                                # asset
-                    availableBalance=round(float(record['bc']), 2),   # balance
-                ))
-            if len(balance) > 0:
-                self.strategy.on_balance_status(balance)
+            self.on_balance_status(_process_balance(record))
         elif 'kline' == event:
-            if not self.last_bar or msg_stamp - self.last_bar >= 1000: 
-                record = data.get('k', {})
-                bar = Bar(
-                    timestamp=datetime.fromtimestamp(int(msg_stamp) / 1000),
-                    open=float(record['o']),
-                    high=float(record['h']),
-                    low=float(record['l']),
-                    close=float(record['c']),
-                    vol=float(record['q']),
-                )
-                self.strategy.on_bar([bar])
-            self.last_bar = msg_stamp
+            if not self.last_bar or msg_stamp - self.last_bar >= 1000:
+                self.on_bar([_process_bar(data, msg_stamp)])
+            self.last_bar = msg_stamp
```

### Comparing `hades-core-0.0.2/hades/core/exchange/okx.py` & `hades-core-0.0.3/hades/core/exchange/okx_ex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,151 +1,158 @@
-
 import asyncio
-import websockets
-from okx.websocket import WsUtils
-import okx.Trade as Trade
-import okx.Account as Account
-import okx.MarketData as Market
-
-from typing import List
-from datetime import datetime
 import json
 import logging
+from asyncio import Future
+from datetime import datetime
+from typing import List, Tuple
+
+import okx.Account as AccountApi
+import okx.MarketData as MarketApi
+import okx.Trade as TradeApi
+import websockets
+from okx.websocket import WsUtils
 
-from hades.core import TradeBotConf, Strategy, Exchange, Subscriber, Order, Position, Balance, Tick, Bar
+from hades.core import TradeBotConf, Strategy, Exchange, Subscriber, Order, Position, Balance, Tick, Bar, Trade
 
 
 class OkxExchangeClient(Exchange):
-    def __init__(self,  conf: TradeBotConf) -> None:
+    def __init__(self, conf: TradeBotConf) -> None:
         self.conf = {
             'api_key': conf.okx['apiKey'],
             'api_secret_key': conf.okx['secretKey'],
             'domain': conf.okx['domain'],
             'passphrase': conf.okx['passphrase'],
             'flag': '0'
         }
-        self.tradeApi = Trade.TradeAPI(**self.conf)
-        self.accountApi = Account.AccountAPI(**self.conf)
-        self.marketApi = Market.MarketAPI(**self.conf)
-    # Account Info
+        self.tradeApi = TradeApi.TradeAPI(**self.conf)
+        self.accountApi = AccountApi.AccountAPI(**self.conf)
+        self.marketApi = MarketApi.MarketAPI(**self.conf)
+
     def get_positions(self) -> List[Position]:
         response = self.accountApi.get_positions()
         if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_position(response['data']) 
+            return to_okx_position(response['data'])
         return []
 
-    def get_balance(self):
+    def get_balance(self) -> List[Balance]:
         return self.accountApi.get_account_balance()
-    # Trade Info
+
     def get_orders(self) -> List[Order]:
         response = self.tradeApi.get_order_list()
         if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_order(response['data']) 
+            return to_okx_order(response['data'])
         return []
-    
-    def place_buy_order(self, symbol: str, size: float, price: float):
-        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='buy', sz=str(size), px=str(price), ordType='post_only')
-    
-    def place_sell_order(self, symbol: str, size: float, price: float):
-        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='sell', sz=str(size), px=str(price), ordType='post_only')
-    
-    def cancel_order(self, orderId: str, symbol: str):
-        return self.tradeApi.cancel_order(instId=symbol, ordId=orderId)
-    
+
+    def place_buy_order(self, symbol: str, size: float, price: float) -> Order:
+        return self.tradeApi.place_order(instId=symbol,
+                                         tdMode='isolated',
+                                         side='buy',
+                                         sz=str(size),
+                                         px=str(price),
+                                         ordType='post_only')
+
+    def place_sell_order(self, symbol: str, size: float, price: float) -> Order:
+        return self.tradeApi.place_order(instId=symbol,
+                                         tdMode='isolated',
+                                         side='sell',
+                                         sz=str(size),
+                                         px=str(price),
+                                         ordType='post_only')
+
+    def cancel_order(self, order_id: str, symbol: str) -> Order:
+        return self.tradeApi.cancel_order(instId=symbol, ordId=order_id)
+
     def close_position(self, symbol: str):
         return self.tradeApi.close_positions(instId=symbol, mgnMode='isolated')
 
-    # get latest 100 bar
     def get_candlesticks(self, symbol: str, bar: str = '1m', limit: int = 100) -> List[Bar]:
         response = self.marketApi.get_candlesticks(instId=symbol, bar=bar, limit=str(limit))
         if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_bar(response['data']) 
+            return to_okx_bar(response['data'])
+        return []
+
+    def get_trades(self, symbol: str) -> List[Trade]:
         return []
-    
+
 
 def to_okx_tick(data: dict) -> List[Tick]:
-    ticks = []
-    ticks.append(Tick(
+    return [Tick(
         symbol=data['instId'],
         price=float(data['last']),
-        timestmap = datetime.fromtimestamp(int(data['ts']) / 1000)
-    ))
-    return ticks
+        timestamp=datetime.fromtimestamp(int(data['ts']) / 1000)
+    )]
 
 
 def to_okx_position(data: List[dict]) -> List[Position]:
     positions = []
     for record in data:
         positions.append(Position(
             symbol=record.get('instId'),
-            instrumentType=record.get('instType'),
+            instrument_type=record.get('instType'),
             side=record.get('posSide'),
             quantity=float(record.get('pos')),
             unrealized_profit=round(float(record.get('upl')), 2),
-            unrealized_profit_ratio = round(float(record.get('uplRatio')) * 100, 2) ,
+            unrealized_profit_ratio=round(float(record.get('uplRatio')) * 100, 2),
             mode=record.get('mgnMode'),
             price=float(record.get('avgPx')),
             timestamp=datetime.fromtimestamp(int(record['cTime']) / 1000)
         ))
     return positions
-   
+
 
 def to_okx_bar(records: List[str]) -> List[Bar]:
     bars: List[Bar] = []
     for record in records:
-        timestamp, open, high, low, close, vol, _, _, _ = record
+        timestamp, _open, high, low, close, vol, _, _, _ = record
         bars.append(Bar(
             timestamp=datetime.fromtimestamp(int(timestamp) / 1000),
-            open=float(open),
+            open=float(_open),
             high=float(high),
             low=float(low),
             close=float(close),
             vol=float(vol),
-        )) 
+        ))
     return bars
 
 
 def to_okx_order(records: List[dict]) -> List[Order]:
     orders = []
     for data in records:
         orders.append(Order(
-            orderId=data.get('ordId'),
-            orderType=data.get('ordType'),
+            order_id=data.get('ordId'),
+            order_type=data.get('ordType'),
             symbol=data.get('instId'),
-            instrumentType=data.get('instType'),
+            instrument_type=data.get('instType'),
             price=float(data.get('px')),
             status=data.get('state'),
             side=data.get('side'),
             quantity=0,
             timestamp=datetime.fromtimestamp(int(data.get('cTime')) / 1000)
         ))
     return orders
 
 
 def to_okx_balance(records: dict) -> List[Balance]:
     balance = []
     if 'details' in records:
         for record in records['details']:
             if float(record.get('availBal')) != 0:
-                balance.append(Balance(asset=record['ccy'], availableBalance=float(record.get('availBal'))))
+                balance.append(Balance(asset=record['ccy'], available_balance=float(record.get('availBal'))))
     return balance
 
 
 class Subscription:
     def __init__(self, channel: str, arg: dict, interval: int = 0) -> None:
         self.channel = channel
         self.arg = {
             'channel': channel,
             "extraParams": "{\"updateInterval\": INTERVAL}".replace('INTERVAL', str(interval)),
             **arg
         }
 
-    def __repr__(self) -> str:
-        return self.arg
-
 
 class OkxConnectionManager:
     def __init__(self,
                  uri: str,
                  subscriptions: List[Subscription],
                  conf: TradeBotConf = None,
                  private: bool = False) -> None:
@@ -175,15 +182,15 @@
                         'args': [sub.arg]
                     }))
                 async for message in conn:
                     await self.handle_message(json.loads(message))
             except websockets.ConnectionClosed:
                 logging.error(f"{','.join([sub.channel for sub in self.subscriptions])} reconnecting")
                 continue
-  
+
     async def handle_message(self, message: dict):
         if message.get('event'):
             logging.info(f"{','.join([sub.channel for sub in self.subscriptions])} {json.dumps(message)}")
 
 
 class BalanceSubscribe(OkxConnectionManager):
     def __init__(self, strategy: Strategy) -> None:
@@ -203,15 +210,16 @@
 
 class OrderSubscriber(OkxConnectionManager):
     def __init__(self, strategy: Strategy) -> None:
         self.channel = 'orders'
         self.strategy = strategy
         conf = TradeBotConf.load()
         logging.info('init OrderSubscriber')
-        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType})], conf, True)
+        super().__init__(conf.okx['ws_private'],
+                         [Subscription(self.channel, {'instType': self.strategy.instrument_type})], conf, True)
 
     async def handle_message(self, message: dict):
         await super().handle_message(message)
         if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
             orders = to_okx_order(message['data'])
             self.strategy.on_order_status(orders)
         logging.info(f'[order] {json.dumps(message)}')
@@ -219,16 +227,17 @@
 
 class PositionSubscriber(OkxConnectionManager):
     def __init__(self, strategy: Strategy) -> None:
         self.channel = 'positions'
         self.strategy = strategy
         conf = TradeBotConf.load()
         logging.info('init PositionSubscriber')
-        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType}, interval=3)], conf, True)
-
+        super().__init__(conf.okx['ws_private'],
+                         [Subscription(self.channel, {'instType': self.strategy.instrument_type}, interval=3)], conf,
+                         True)
 
     async def handle_message(self, message: dict):
         await super().handle_message(message)
         if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
             positions = to_okx_position(message['data'])
             self.strategy.on_position_status(positions)
         logging.debug(f'[position] {json.dumps(message)}')
@@ -236,19 +245,21 @@
 
 class TickSubscriber(OkxConnectionManager):
     def __init__(self, strategy: Strategy) -> None:
         self.channel = 'tickers'
         self.strategy = strategy
         conf = TradeBotConf.load()
         logging.info('init TickSubscriber')
-        super().__init__(conf.okx['ws_public'], [Subscription(self.channel, {'instId': sub}, interval=1) for sub in self.strategy.symbols])
+        super().__init__(conf.okx['ws_public'],
+                         [Subscription(self.channel, {'instId': sub}, interval=1) for sub in self.strategy.symbols])
 
     async def handle_message(self, message: dict):
         await super().handle_message(message)
-        if message.get('arg', {}).get('channel') == self.channel and message.get('data') and len(message.get('data')) > 0:
+        if message.get('arg', {}).get('channel') == self.channel and message.get('data') and len(
+                message.get('data')) > 0:
             ticks = to_okx_tick(message['data'][0])
             self.strategy.on_tick(ticks)
         logging.debug(f'[tick] {json.dumps(message)}')
 
 
 class BarSubscriber(OkxConnectionManager):
     def __init__(self, strategy: Strategy) -> None:
@@ -257,30 +268,53 @@
         conf = TradeBotConf.load()
         logging.info('init BarSubscriber')
         subscriptions = []
         for symbol in self.strategy.symbols:
             for bar_type in self.bar_types:
                 logging.info(f'subscribe {bar_type}-{symbol}')
                 subscriptions.append(Subscription(f'{bar_type}', {'instId': symbol}, interval=1))
-        
+
         super().__init__(conf.okx['ws_public'], subscriptions)
 
     async def handle_message(self, message: dict):
         await super().handle_message(message)
-        if message.get('arg', {}).get('channel', None) in self.bar_types and message.get('data') and len(message.get('data')) > 0:
+        if message.get('arg', {}).get('channel', None) in self.bar_types and message.get('data') and len(
+                message.get('data')) > 0:
             bars = to_okx_bar(message['data'])
             self.strategy.on_bar(bars)
         logging.debug(f'[bar] {json.dumps(message)}')
 
 
 class OkxSubscriber(Subscriber):
+
     def __init__(self, strategy: Strategy) -> None:
+        super().__init__(strategy)
         self.strategy = strategy
         self.strategy.on_init_exchange(OkxExchangeClient(TradeBotConf.load()))
-    
-    
-    def run(self) -> List[asyncio.Future]:
+
+    def on_tick(self, ticks: List[Tick]):
+        super().on_tick(ticks)
+
+    def on_bar(self, bars: List[Bar]):
+        super().on_bar(bars)
+
+    def on_order_status(self, orders: List[Order]):
+        super().on_order_status(orders)
+
+    def on_balance_status(self, balance: List[Balance]):
+        super().on_balance_status(balance)
+
+    def on_position_status(self, positions: List[Position]):
+        super().on_position_status(positions)
+
+    def run(self) -> Future[tuple[None, None, None, None, None]]:
         return asyncio.gather(BalanceSubscribe(self.strategy).run(),
-                            OrderSubscriber(self.strategy).run(),
-                            BarSubscriber(self.strategy).run(),
-                            TickSubscriber(self.strategy).run(),
-                            PositionSubscriber(self.strategy).run())
+                              OrderSubscriber(self.strategy).run(),
+                              BarSubscriber(self.strategy).run(),
+                              TickSubscriber(self.strategy).run(),
+                              PositionSubscriber(self.strategy).run())
+
+    def stop(self) -> None:
+        super().stop()
+
+    def get_exchange(self) -> Exchange:
+        return super().get_exchange()
```

### Comparing `hades-core-0.0.2/hades/core/executor.py` & `hades-core-0.0.3/hades/core/executor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from hades.core import Strategy, BinanceUMSubscriber, OkxSubscriber, Subscriber, ExchangeEnum
+from hades.core.backtesting import BackTestingSubscriber
 
 
-class TradeExecutor():
-    def __init__(self, strategy: Strategy, backtesting: bool, exchange:ExchangeEnum=ExchangeEnum.Binance) -> None:
-        self.backtesting = backtesting
+class TradeExecutor:
+    def __init__(self, strategy: Strategy, exchange: ExchangeEnum = ExchangeEnum.Binance) -> None:
         self.strategy = strategy
         self.exchange = exchange
         self.subscriber = self.__get_subscriber(self.exchange)
 
     async def execute(self):
         await self.subscriber.run()
 
-    def __get_subscriber(self, exchange:ExchangeEnum) -> Subscriber:
+    def __get_subscriber(self, exchange: ExchangeEnum) -> Subscriber:
         if exchange == ExchangeEnum.Binance:
             return BinanceUMSubscriber(self.strategy)
         elif exchange == ExchangeEnum.OKX:
             return OkxSubscriber(self.strategy)
-        raise  ValueError('current exchange does not support')
-    
+        elif exchange == ExchangeEnum.BackTesting:
+            return BackTestingSubscriber(self.strategy)
+        raise ValueError('current exchange does not support')
+
     def stop(self):
         self.subscriber.stop()
-
```

### Comparing `hades-core-0.0.2/hades/core/messager.py` & `hades-core-0.0.3/hades/core/messager/dingding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-from datetime import datetime
-import logging
 import requests
+
 from hades.core import TradeBotConf
+from hades.core.messager.base import Messenger
 
 
-class Messager:
+class DingDingMessenger(Messenger):
     def __init__(self, conf: TradeBotConf) -> None:
+        super().__init__(conf)
+
         self.prefix = conf.prefix
-        self.start, self.end = conf.period.split('-')
         self.url = f'https://oapi.dingtalk.com/robot/send?access_token={conf.token}'
         self.session = requests.session()
         self.session.headers.update({
             'Content-Type': 'application/json',
         })
-        self.last_notify = None
 
-    def notify(self, text) -> bool:
+    def _send_message(self, text) -> bool:
         data = {
             'msgtype': 'text',
             'text': {
                 'content': f'{self.prefix} {text}'
             }
         }
-        now = datetime.utcnow()
-        if now.hour >= int(self.start) and now.hour < int(self.end):
-            response = self.session.post(self.url, json=data)
-            return 'errmsg' in response.json() and response.json()['errmsg'] == 'ok'
-        else:
-            logging.info(f'message = {text} not sent')
-
-    def notify_with_interval(self, text, minute: int = 5) -> bool:
-        now = datetime.utcnow()
-        if not self.last_notify or (now - self.last_notify).seconds >= minute * 60:
-            self.last_notify = now
-            self.notify(text)
+        response = self.session.post(self.url, json=data)
+        return 'errmsg' in response.json() and response.json()['errmsg'] == 'ok'
```

### Comparing `hades-core-0.0.2/hades_core.egg-info/PKG-INFO` & `hades-core-0.0.3/hades_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hades-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: cryptocurrency trading bot
 Author-email: Gary Guo <gary.guo.china@gmail.com>
 Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -229,15 +229,15 @@
 ### 1. Setup Environment
 
 ```shell
 python -m venv runtime
 runtime\Scripts\activate
 pip install -r requirements.txt
 # if requirements.txt not work
-pip3 install python-okx websockets requests binance-futures-connector
+pip3 install python-okx websockets requests binance-futures-connector python-telegram-bot pydantic
 ```
 
 ### 2. Change Configuration
 
 copy `example.conf` and rename to `app.conf` , change parameter
 
 ```ini
@@ -251,12 +251,18 @@
 passphrase       = passphrase
 ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
 ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
 ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
 domain           = https://aws.okx.com
 useServerTime    = False
 
-[notification]
+# optional
+[dingding]
 token            = token
 prefix           = prefix
 period           = 8-23
+
+# optional
+[telegram]
+token            = token
+period           = 8-23
 ```
```

### Comparing `hades-core-0.0.2/pyproject.toml` & `hades-core-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 [project]
 # This is the name of your project. The first time you publish this
 # package, this name will be registered for you. It will determine how
 # users can install this project, e.g.:
 #
 # $ pip install sampleproject
 #
@@ -33,75 +32,74 @@
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
 requires-python = ">=3.7"
 
 # This is either text indicating the license for the distribution, or a file
 # that contains the license
 # https://packaging.python.org/en/latest/specifications/core-metadata/#license
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 
 # This field adds keywords for your project which will appear on the
 # project page. What does your project relate to?
 #
 # Note that this is a list of additional keywords, separated
 # by commas, to be used to assist searching for the distribution in a
 # larger catalog.
-keywords = ["okx", "binance", "cryptocurrency"] 
+keywords = ["okx", "binance", "cryptocurrency"]
 
 # This should be your name or the name of the organization who originally
 # authored the project, and a valid email address corresponding to the name
 # listed.
 authors = [
-     {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
+    { name = "Gary Guo", email = "gary.guo.china@gmail.com" },
 ]
 
 # This should be your name or the names of the organization who currently
 # maintains the project, and a valid email address corresponding to the name
 # listed.
 maintainers = [
-    {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
+    { name = "Gary Guo", email = "gary.guo.china@gmail.com" },
 ]
 
 # Classifiers help users find your project by categorizing it.
 #
 # For a list of valid classifiers, see https://pypi.org/classifiers/
-classifiers = [  # Optional
-  # How mature is this project? Common values are
-  #   3 - Alpha
-  #   4 - Beta
-  #   5 - Production/Stable
-  "Development Status :: 3 - Alpha",
-
-  # Indicate who your project is intended for
-  "Intended Audience :: Developers",
-  "Topic :: Software Development :: Build Tools",
-
-  # Pick your license as you wish
-  "License :: OSI Approved :: MIT License",
-
-  # Specify the Python versions you support here. In particular, ensure
-  # that you indicate you support Python 3. These classifiers are *not*
-  # checked by "pip install". See instead "python_requires" below.
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3 :: Only",
+classifiers = [# Optional
+    # How mature is this project? Common values are
+    #   3 - Alpha
+    #   4 - Beta
+    #   5 - Production/Stable
+    "Development Status :: 3 - Alpha",
+    # Indicate who your project is intended for
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Build Tools",
+    # Pick your license as you wish
+    "License :: OSI Approved :: MIT License",
+    # Specify the Python versions you support here. In particular, ensure
+    # that you indicate you support Python 3. These classifiers are *not*
+    # checked by "pip install". See instead "python_requires" below.
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
 ]
 
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
-dependencies = [ # Optional
-   "python-okx", 
-   "websockets", 
-   "requests", 
-   "binance-futures-connector"
+dependencies = [# Optional
+    "python-okx",
+    "websockets",
+    "requests",
+    "binance-futures-connector",
+    "python-telegram-bot",
+    "pydantic"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
@@ -130,11 +128,11 @@
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bandit]
-exclude_dirs = ["build","dist","tests","runtime"]
+exclude_dirs = ["build", "dist", "tests", "runtime"]
 
 [tool.setuptools.dynamic]
-version = {attr = "hades.__version__"}
+version = { attr = "hades.__version__" }
```

