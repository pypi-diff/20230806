# Comparing `tmp/apit212-1.0.2.tar.gz` & `tmp/apit212-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-1.0.2.tar", last modified: Fri Jul 28 13:33:38 2023, max compression
+gzip compressed data, was "apit212-1.0.3.tar", last modified: Sat Aug  5 11:41:07 2023, max compression
```

## Comparing `apit212-1.0.2.tar` & `apit212-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:33:38.983512 apit212-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     7653 2023-07-28 13:33:38.975052 apit212-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6886 2023-07-28 13:32:41.000000 apit212-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 13:33:38.911339 apit212-1.0.2/apit212/
--rw-rw-rw-   0        0        0    18838 2023-07-28 13:32:50.000000 apit212-1.0.2/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.2/apit212/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-1.0.2/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.2/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:33:38.972635 apit212-1.0.2/apit212.egg-info/
--rw-rw-rw-   0        0        0     7653 2023-07-28 13:33:38.000000 apit212-1.0.2/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-28 13:33:38.000000 apit212-1.0.2/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:33:38.000000 apit212-1.0.2/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-28 13:33:38.000000 apit212-1.0.2/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 13:33:38.000000 apit212-1.0.2/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-07-28 13:30:36.000000 apit212-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 13:33:38.983512 apit212-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-07-28 13:28:40.000000 apit212-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.258344 apit212-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9396 2023-08-05 11:41:07.255802 apit212-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8629 2023-08-05 08:54:08.000000 apit212-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.204880 apit212-1.0.3/apit212/
+-rw-rw-rw-   0        0        0    41429 2023-08-05 11:34:45.000000 apit212-1.0.3/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.3/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-08-05 10:09:12.000000 apit212-1.0.3/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.3/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:41:07.254791 apit212-1.0.3/apit212.egg-info/
+-rw-rw-rw-   0        0        0     9396 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 11:41:07.000000 apit212-1.0.3/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-08-05 11:38:51.000000 apit212-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:41:07.258344 apit212-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-08-05 10:40:41.000000 apit212-1.0.3/setup.py
```

### Comparing `apit212-1.0.2/LICENSE` & `apit212-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-1.0.2/PKG-INFO` & `apit212-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: apit212
-Version: 1.0.2
-Summary: Unofficial trading212 API
-Home-page: https://github.com/Flock92/aPit212
-Author: Flock92
-Author-email: Flock92 <stuwe_3000@outlook.com>
-Maintainer-email: Flock92 <stuwe_3000@outlook.com>
-License: MIT
-Project-URL: Homepage, https://github.com/Flock92/apit212
-Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
-Keywords: trading,trading212,api,trade,flock92
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires: requests
-Requires: selenium
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -151,22 +129,62 @@
 
 {'20434246': {'accountId': ********, 'tradingType': 'CFD', 'currency': 'GBP',
 'freeForWithdraw': 486.83, 'freeForCfdTransfer': 0, 'total': 486.83,
 'lockedCash': {'totalLockedCash': 0, 'lockedCash': []}}}
 
 ```
 
+### Add trailing stop loss
+
+the *trailing_stop* function allows you to add a trailing stop to a open position.
+
+```py
+
+trailing_stop = client.trailing_stop(position_id="***-****-***", distance=0.5)
+
+```
+
+### Add/Change stoploss and takeprofit
+
+The *add_limits* function allows you to add a stoploss and takeprofit to an existing position.
+
+```py
+
+update_limits = client.add_limits(position_id="***-****-***", TP=1 , SL=1)
+
+```
+To set a new stoploss or takeprofit just pass the distance to the TP (take profit) or SL (stop loss) params. The function will get the current price and apply the distance.
+
+### Get all position history
+
+The *all_position_hist* function will return the position history.
+
+```py
+
+position_history = client.all_position_hist()
+
+```
+
+### Get order history
+
+The *all_order_hist* returns orders data
+
+```py
+
+order_history = client.all_order_hist()
+
+```
 
 ### Get Insturments info
 
 The *get_instrument* function will retunr information about the instrument. 
 
 ```py
 
-tsla_info = get_instruments_info('TSLA')
+tsla_info = client.get_instruments_info(instrument='TSLA')
 
 print(tsla_info)
 
 ```
 
 #### Console:
 
@@ -174,14 +192,37 @@
 
 {'code': 'TSLA', 'type': 'STOCK', 'margin': 0.2, 'shortPositionSwap': -0.07030593058663,
 'longPositionSwap': -0.27928156941337, 'tsSwapCharges': '1970-01-01T23:00:00.000+02:00',
 'marginPercent': '20', 'leverage': '1:5'}
 
 ```
 
+### Get position information
+
+The *get_position* function will returns information for the qouted positionID.
+
+```py
+
+position = client.get_position(position_id="***-****-***")
+
+print(position)
+
+```
+
+#### console
+
+```bash
+
+[{'eventType': {'action': 'opened', 'source': 'MARKET_ORDER'}, 
+'eventNumber': {'name': 'MO3053019640', 'id': '274187113', 'frontend': 'WC4'}, 'time': '2023-08-02T22:42:54.000+03:00', 
+'direction': 'sell', 'quantity': 1.0, 'price': '105.29', 'avgQuantity': 1.0, 'avgPrice': '105.2900', 'modifiedDirection': 
+'sell'}]
+
+```
+
 ### Get Summary
 
 The *get_summary* function will return the account summary. this function can also be used to get order ID's and there current PPL
 
 ```py
 
 summary = client.get_summary()
@@ -263,14 +304,15 @@
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
 You can also use the *cancel_all_orders* to cancel all pending limits orders.
 
+
 ```py
 
 cancel_all = client.cancel_all_orders()
 
 ```
 
 ### Close Position
@@ -309,10 +351,23 @@
            'Cookie': 'TRADING212_SESSION_DEMO=***********;'}
 
 client = Apit212(username="flock92@account.api", password="pass******", headers=headers)
 
 
 ```
 
+## CODE EXAMPLES
+
+Code below will add a stoploss and takeprofit to an existing position
+
+```py
+
+summary = client.get_summary()
+
+for items in enumerate(summary["open"]["items"])
+    positionID = items[i[0]]["positionId"]
+
+```
+
 ## Disclaimer
 
 This is an unofficial API & either myself of trading212 are responsible for the use of this API. It is strongly advised that you use a practice account before moving onto real money. *apit212 is **not** a trading bot*
```

### Comparing `apit212-1.0.2/README.md` & `apit212-1.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: apit212
+Version: 1.0.3
+Summary: Unofficial trading212 API
+Home-page: https://github.com/Flock92/aPit212
+Author: Flock92
+Author-email: Flock92 <stuwe_3000@outlook.com>
+Maintainer-email: Flock92 <stuwe_3000@outlook.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Flock92/apit212
+Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
+Keywords: trading,trading212,api,trade,flock92
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires: requests
+Requires: selenium
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -129,22 +151,62 @@
 
 {'20434246': {'accountId': ********, 'tradingType': 'CFD', 'currency': 'GBP',
 'freeForWithdraw': 486.83, 'freeForCfdTransfer': 0, 'total': 486.83,
 'lockedCash': {'totalLockedCash': 0, 'lockedCash': []}}}
 
 ```
 
+### Add trailing stop loss
+
+the *trailing_stop* function allows you to add a trailing stop to a open position.
+
+```py
+
+trailing_stop = client.trailing_stop(position_id="***-****-***", distance=0.5)
+
+```
+
+### Add/Change stoploss and takeprofit
+
+The *add_limits* function allows you to add a stoploss and takeprofit to an existing position.
+
+```py
+
+update_limits = client.add_limits(position_id="***-****-***", TP=1 , SL=1)
+
+```
+To set a new stoploss or takeprofit just pass the distance to the TP (take profit) or SL (stop loss) params. The function will get the current price and apply the distance.
+
+### Get all position history
+
+The *all_position_hist* function will return the position history.
+
+```py
+
+position_history = client.all_position_hist()
+
+```
+
+### Get order history
+
+The *all_order_hist* returns orders data
+
+```py
+
+order_history = client.all_order_hist()
+
+```
 
 ### Get Insturments info
 
 The *get_instrument* function will retunr information about the instrument. 
 
 ```py
 
-tsla_info = get_instruments_info('TSLA')
+tsla_info = client.get_instruments_info(instrument='TSLA')
 
 print(tsla_info)
 
 ```
 
 #### Console:
 
@@ -152,14 +214,37 @@
 
 {'code': 'TSLA', 'type': 'STOCK', 'margin': 0.2, 'shortPositionSwap': -0.07030593058663,
 'longPositionSwap': -0.27928156941337, 'tsSwapCharges': '1970-01-01T23:00:00.000+02:00',
 'marginPercent': '20', 'leverage': '1:5'}
 
 ```
 
+### Get position information
+
+The *get_position* function will returns information for the qouted positionID.
+
+```py
+
+position = client.get_position(position_id="***-****-***")
+
+print(position)
+
+```
+
+#### console
+
+```bash
+
+[{'eventType': {'action': 'opened', 'source': 'MARKET_ORDER'}, 
+'eventNumber': {'name': 'MO3053019640', 'id': '274187113', 'frontend': 'WC4'}, 'time': '2023-08-02T22:42:54.000+03:00', 
+'direction': 'sell', 'quantity': 1.0, 'price': '105.29', 'avgQuantity': 1.0, 'avgPrice': '105.2900', 'modifiedDirection': 
+'sell'}]
+
+```
+
 ### Get Summary
 
 The *get_summary* function will return the account summary. this function can also be used to get order ID's and there current PPL
 
 ```py
 
 summary = client.get_summary()
@@ -241,14 +326,15 @@
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
 You can also use the *cancel_all_orders* to cancel all pending limits orders.
 
+
 ```py
 
 cancel_all = client.cancel_all_orders()
 
 ```
 
 ### Close Position
@@ -287,10 +373,23 @@
            'Cookie': 'TRADING212_SESSION_DEMO=***********;'}
 
 client = Apit212(username="flock92@account.api", password="pass******", headers=headers)
 
 
 ```
 
+## CODE EXAMPLES
+
+Code below will add a stoploss and takeprofit to an existing position
+
+```py
+
+summary = client.get_summary()
+
+for items in enumerate(summary["open"]["items"])
+    positionID = items[i[0]]["positionId"]
+
+```
+
 ## Disclaimer
 
 This is an unofficial API & either myself of trading212 are responsible for the use of this API. It is strongly advised that you use a practice account before moving onto real money. *apit212 is **not** a trading bot*
```

### Comparing `apit212-1.0.2/apit212/apitconstant.py` & `apit212-1.0.3/apit212/apitconstant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 #CONSTANT ELEMENTS FROM apit212
 URL = 'https://www.trading212.com/'
 LOGIN_BUTTON = '//*[@id="__next"]/header/div/div/div[2]/div[1]/div[2]/p'
 COOKIE_POPUP = '//*[@id="__next"]/main/div[2]/div/div[2]/div[2]/div[2]/div[1]'
 SUBMIT_BUTTON = '//*[@id="__next"]/main/div[2]/div/div[2]/div/div[2]/div/form/div[5]/input'
 POPUP_CLOSE = '//*[@id="app"]/div[6]/div/div[2]/div/div/div/div[2]/div/div[1]/div[3]/div/span/div'
 REMEBER_ME_TOGGLE = '//*[@id="__next"]/main/div[2]/div/div[2]/div/div[2]/div/form/div[4]/div[2]/input'
@@ -16,7 +17,8 @@
 LIVE_RESULTS = '//*[@id="app"]/div[3]/div[2]/div[2]/div/div[2]/div[2]/div[4]/div[1]/div[2]'
 BLOCKED_FUNDS = '//*[@id="app"]/div[3]/div[2]/div[2]/div/div[2]/div[2]/div[4]/div[3]/div[2]'
 MARGIN_INDICATORS = '//*[@id="app"]/div[5]/div[2]/div[2]/div/div[2]/div[2]/div[4]/div[4]/div/div/div/div'
 
 APP = '//*[@id="app"]'
 
 SETUP_ERR = 'FAILED TO SETUP PROFILE'
+
```

### Comparing `apit212-1.0.2/apit212/cfdScrape.py` & `apit212-1.0.3/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.2/apit212.egg-info/PKG-INFO` & `apit212-1.0.3/apit212.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
@@ -151,22 +151,62 @@
 
 {'20434246': {'accountId': ********, 'tradingType': 'CFD', 'currency': 'GBP',
 'freeForWithdraw': 486.83, 'freeForCfdTransfer': 0, 'total': 486.83,
 'lockedCash': {'totalLockedCash': 0, 'lockedCash': []}}}
 
 ```
 
+### Add trailing stop loss
+
+the *trailing_stop* function allows you to add a trailing stop to a open position.
+
+```py
+
+trailing_stop = client.trailing_stop(position_id="***-****-***", distance=0.5)
+
+```
+
+### Add/Change stoploss and takeprofit
+
+The *add_limits* function allows you to add a stoploss and takeprofit to an existing position.
+
+```py
+
+update_limits = client.add_limits(position_id="***-****-***", TP=1 , SL=1)
+
+```
+To set a new stoploss or takeprofit just pass the distance to the TP (take profit) or SL (stop loss) params. The function will get the current price and apply the distance.
+
+### Get all position history
+
+The *all_position_hist* function will return the position history.
+
+```py
+
+position_history = client.all_position_hist()
+
+```
+
+### Get order history
+
+The *all_order_hist* returns orders data
+
+```py
+
+order_history = client.all_order_hist()
+
+```
 
 ### Get Insturments info
 
 The *get_instrument* function will retunr information about the instrument. 
 
 ```py
 
-tsla_info = get_instruments_info('TSLA')
+tsla_info = client.get_instruments_info(instrument='TSLA')
 
 print(tsla_info)
 
 ```
 
 #### Console:
 
@@ -174,14 +214,37 @@
 
 {'code': 'TSLA', 'type': 'STOCK', 'margin': 0.2, 'shortPositionSwap': -0.07030593058663,
 'longPositionSwap': -0.27928156941337, 'tsSwapCharges': '1970-01-01T23:00:00.000+02:00',
 'marginPercent': '20', 'leverage': '1:5'}
 
 ```
 
+### Get position information
+
+The *get_position* function will returns information for the qouted positionID.
+
+```py
+
+position = client.get_position(position_id="***-****-***")
+
+print(position)
+
+```
+
+#### console
+
+```bash
+
+[{'eventType': {'action': 'opened', 'source': 'MARKET_ORDER'}, 
+'eventNumber': {'name': 'MO3053019640', 'id': '274187113', 'frontend': 'WC4'}, 'time': '2023-08-02T22:42:54.000+03:00', 
+'direction': 'sell', 'quantity': 1.0, 'price': '105.29', 'avgQuantity': 1.0, 'avgPrice': '105.2900', 'modifiedDirection': 
+'sell'}]
+
+```
+
 ### Get Summary
 
 The *get_summary* function will return the account summary. this function can also be used to get order ID's and there current PPL
 
 ```py
 
 summary = client.get_summary()
@@ -263,14 +326,15 @@
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
 You can also use the *cancel_all_orders* to cancel all pending limits orders.
 
+
 ```py
 
 cancel_all = client.cancel_all_orders()
 
 ```
 
 ### Close Position
@@ -309,10 +373,23 @@
            'Cookie': 'TRADING212_SESSION_DEMO=***********;'}
 
 client = Apit212(username="flock92@account.api", password="pass******", headers=headers)
 
 
 ```
 
+## CODE EXAMPLES
+
+Code below will add a stoploss and takeprofit to an existing position
+
+```py
+
+summary = client.get_summary()
+
+for items in enumerate(summary["open"]["items"])
+    positionID = items[i[0]]["positionId"]
+
+```
+
 ## Disclaimer
 
 This is an unofficial API & either myself of trading212 are responsible for the use of this API. It is strongly advised that you use a practice account before moving onto real money. *apit212 is **not** a trading bot*
```

### Comparing `apit212-1.0.2/pyproject.toml` & `apit212-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-1.0.2/setup.py` & `apit212-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

