# Comparing `tmp/volstreet-1.0.9.tar.gz` & `tmp/volstreet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.0.9.tar", last modified: Wed Jul 26 20:59:19 2023, max compression
+gzip compressed data, was "volstreet-1.1.0.tar", last modified: Sun Aug  6 15:10:22 2023, max compression
```

## Comparing `volstreet-1.0.9.tar` & `volstreet-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.381528 volstreet-1.0.9/
--rw-rw-rw-   0        0        0      497 2023-07-26 20:59:19.382520 volstreet-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.0.9/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-07-26 20:59:19.382520 volstreet-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.376541 volstreet-1.0.9/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.0.9/volstreet/__init__.py
--rw-rw-rw-   0        0        0     9094 2023-07-16 12:56:47.000000 volstreet-1.0.9/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2685 2023-06-26 20:11:40.000000 volstreet-1.0.9/volstreet/constants.py
--rw-rw-rw-   0        0        0    43796 2023-07-25 18:04:18.000000 volstreet-1.0.9/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   192627 2023-07-26 20:57:45.000000 volstreet-1.0.9/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      211 2023-07-16 12:56:47.000000 volstreet-1.0.9/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.0.9/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    13488 2023-07-25 17:19:23.000000 volstreet-1.0.9/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:59:19.381528 volstreet-1.0.9/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 20:59:19.000000 volstreet-1.0.9/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.571510 volstreet-1.1.0/
+-rw-rw-rw-   0        0        0      497 2023-08-06 15:10:22.571510 volstreet-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.1.0/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-08-06 15:10:22.572323 volstreet-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.561394 volstreet-1.1.0/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.1.0/volstreet/__init__.py
+-rw-rw-rw-   0        0        0    10080 2023-08-06 14:57:40.000000 volstreet-1.1.0/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2716 2023-08-03 18:56:13.000000 volstreet-1.1.0/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43826 2023-07-28 13:59:59.000000 volstreet-1.1.0/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   202207 2023-08-04 16:01:04.000000 volstreet-1.1.0/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      729 2023-08-02 13:31:19.000000 volstreet-1.1.0/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.1.0/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14350 2023-08-04 10:10:12.000000 volstreet-1.1.0/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:10:22.570006 volstreet-1.1.0/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 15:10:22.000000 volstreet-1.1.0/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.0.9/setup.cfg` & `volstreet-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 390d 0a61  rsion = 1.0.9..a
+00000020: 7273 696f 6e20 3d20 312e 312e 300d 0a61  rsion = 1.1.0..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-1.0.9/volstreet/SmartWebSocketV2.py` & `volstreet-1.1.0/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.9/volstreet/blackscholes.py` & `volstreet-1.1.0/volstreet/blackscholes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 from scipy.stats import norm
 from scipy.optimize import brentq
 import numpy as np
+import logging
+from datetime import datetime
+from volstreet.exceptions import OptionModelInputError
+
+bs_logger = logging.getLogger("blackscholes")
+today = datetime.now().strftime("%Y-%m-%d")
+file_handler = logging.FileHandler(f"bs-{today}.log")
+formatter = logging.Formatter("%(asctime)s : %(levelname)s : %(name)s : %(message)s")
+file_handler.setFormatter(formatter)
+file_handler.setLevel(logging.INFO)
+bs_logger.setLevel(logging.INFO)
+bs_logger.addHandler(file_handler)
 
 N = norm.cdf
 binary_flag = {"c": 1, "p": -1}
 
 
 def pdf(x):
     """the probability density function"""
@@ -93,20 +105,26 @@
 
 def implied_volatility(price, S, K, t, r, flag):
     if flag.upper().startswith("P"):
         f = lambda sigma: price - put(S, K, t, r, sigma)
     else:
         f = lambda sigma: price - call(S, K, t, r, sigma)
 
-    return brentq(
-        f, a=1e-12, b=100, xtol=1e-15, rtol=1e-15, maxiter=1000, full_output=False
-    )
+    try:
+        return brentq(
+            f, a=1e-12, b=100, xtol=1e-15, rtol=1e-15, maxiter=1000, full_output=False
+        )
+    except Exception as e:
+        bs_logger.error(
+            f"Error in implied_volatility: {e}, price={price}, S={S}, K={K}, t={t}, r={r}, flag={flag}"
+        )
+        raise e
 
 
-def main():
+def test_func():
     # Comparing time to calculate implied volatility using two different methods
     import timeit
 
     # Generate random data
     np.random.seed(42)
     Ss = np.random.uniform(40000, 45000, 100)
     Ks = np.random.uniform(40000, 45000, 100)
@@ -264,14 +282,19 @@
     :param strike: strike price
     :param timeleft: time left to expiry in years
     :param time_delta: in minutes
     :param _print_details: print details of the adjustment
     :return:
     """
     flag = flag.lower()[0]
+    strike_diff = current_spot - strike if flag == "c" else strike - current_spot
+    if strike_diff > current_price:
+        raise OptionModelInputError(
+            f"Current price {current_price} of {'call' if flag == 'c' else 'put'} is less than the strike difference"
+        )
     price_func = call if flag == "c" else put
     vol = implied_volatility(current_price, current_spot, strike, timeleft, 0.06, flag)
     delta_ = delta(current_spot, strike, timeleft, 0.06, vol, flag)
     estimated_movement_points = (target_price - current_price) / delta_
     estimated_movement = estimated_movement_points / current_spot
     timeleft = timeleft - (time_delta / 525600) if time_delta else timeleft
```

### Comparing `volstreet-1.0.9/volstreet/constants.py` & `volstreet-1.1.0/volstreet/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
 def create_logger(name):
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     today = datetime.now().strftime("%Y-%m-%d")
     info_log_filename = f"error-{today}.log"
     info_handler = logging.FileHandler(info_log_filename)
-    formatter = logging.Formatter("%(asctime)s:%(levelname)s:%(message)s")
+    formatter = logging.Formatter(
+        "%(asctime)s : %(levelname)s : %(name)s : %(message)s"
+    )
     info_handler.setFormatter(formatter)
     info_handler.setLevel(logging.INFO)
     logger.addHandler(info_handler)
 
     error_log_filename = f"info-{today}.log"
     error_handler = logging.FileHandler(error_log_filename)
     error_handler.setFormatter(formatter)
```

### Comparing `volstreet-1.0.9/volstreet/datamodule.py` & `volstreet-1.1.0/volstreet/datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,21 +858,22 @@
     for ticker in tickers:
         print(f"Fetching data for {ticker}")
         get_1m_data(kite_object, ticker, path=path)
 
 
 def backtest_intraday_trend(
     one_min_df,
+    vix_df,
     open_nth=0,
     beta=1,
     trend_threshold=1,
     stop_loss=0.3,
     max_entries=3,
-    eod_client=None,
     rolling_days=60,
+    randomize=False,
 ):
     one_min_df = one_min_df.copy()
     if one_min_df.index.name == "date":
         one_min_df = one_min_df.reset_index()
     one_min_df = one_min_df[
         (one_min_df["date"].dt.time > time(9, 15))
         & (one_min_df["date"].dt.time < time(15, 30))
@@ -882,35 +883,32 @@
         datetime(2015, 2, 28).date(),
         datetime(2016, 10, 30).date(),
         datetime(2019, 10, 27).date(),
         datetime(2020, 2, 1).date(),
         datetime(2020, 11, 14).date(),
     ]
 
-    # Fetching vix data and calculating beta
-    if eod_client is None:
-        client = DataClient(api_key=__import__("os").environ.get("EOD_API_KEY"))
-    else:
-        client = eod_client
-
-    vix = client.get_data("VIX", return_columns=["open", "close"])
-    vix = vix.resample("B").ffill()
+    vix = vix_df.copy()
     vix["open"] = vix["open"] * beta
     vix["close"] = vix["close"] * beta
 
     one_min_df.drop(
         one_min_df[one_min_df["date"].dt.date.isin(unavailable_dates)].index,
         inplace=True,
     )
     open_prices = (
         one_min_df.groupby(one_min_df["date"].dt.date).apply(lambda x: x.iloc[open_nth]).open.to_frame()
     )
     open_data = open_prices.merge(
         vix["open"].to_frame(), left_index=True, right_index=True, suffixes=("", "_vix")
     )
+
+    if randomize:
+        trend_threshold = 0.0001
+
     open_data["threshold_movement"] = (open_data["open_vix"] / 48) * trend_threshold
     open_data["upper_bound"] = open_data["open"] * (
         1 + open_data["threshold_movement"] / 100
     )
     open_data["lower_bound"] = open_data["open"] * (
         1 - open_data["threshold_movement"] / 100
     )
@@ -920,15 +918,15 @@
         one_min_df.groupby(one_min_df["date"].dt.date)
         .apply(lambda x: x["close"].pct_change().abs().mean() * 100)
     )
 
     daily_minute_vols_rolling = daily_minute_vols.rolling(rolling_days, min_periods=1).mean()
 
     daily_open_to_close_trends = (
-        one_min_df.close.groupby(one_min_df["date"].dt.date)
+        one_min_df.open.groupby(one_min_df["date"].dt.date)
         .apply(lambda x: (x.iloc[-1] / x.iloc[0] - 1) * 100)
     )
 
     daily_open_to_close_trends_rolling = daily_open_to_close_trends.abs().rolling(rolling_days, min_periods=1).mean()
 
     rolling_ratio = daily_open_to_close_trends_rolling / daily_minute_vols_rolling
 
@@ -958,14 +956,16 @@
 
         """ The group is a dataframe """
 
         all_entries_in_a_day = {}
         # Find the first index where the absolute price change crosses the threshold
         entry = 1
         while entry <= max_entries:
+            # Filtering the dataframe to only include the rows after open nth
+            group = group.iloc[open_nth:]
             idx = group[
                 abs(group["change_from_open"]) >= group["threshold_movement"]
             ].first_valid_index()
             if idx is not None:  # if there is a crossing
                 result_dict = {
                     "returns": 0,
                     "trigger_time": np.nan,
@@ -975,15 +975,18 @@
                     "stop_loss_time": np.nan,
                 }
                 # Record the price and time of crossing the threshold
                 cross_price = group.loc[idx, "close"]
                 cross_time = group.loc[idx, "date"]
 
                 # Determine the direction of the movement
-                direction = np.sign(group.loc[idx, "change_from_open"])
+                if randomize:
+                    direction = np.random.choice([-1, 1])
+                else:
+                    direction = np.sign(group.loc[idx, "change_from_open"])
 
                 # Calculate the stoploss price
                 if stop_loss == 'dynamic':
                     # Selecting previous days rolling ratio
                     current_rolling_ratio = rolling_ratio.loc[:cross_time.date()].iloc[-1]
                     # Calculating the stop_loss pct
                     if current_rolling_ratio > 30:
```

### Comparing `volstreet-1.0.9/volstreet/dealingroom.py` & `volstreet-1.1.0/volstreet/dealingroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from smartapi import SmartConnect
 from smartapi.smartExceptions import DataException
 import pyotp
 from threading import Thread
 from volstreet.SmartWebSocketV2 import SmartWebSocketV2
 from volstreet.constants import scrips, holidays, symbol_df, logger
 from volstreet import blackscholes as bs, datamodule as dm
+from volstreet.exceptions import OptionModelInputError
 from collections import defaultdict, deque
 import yfinance as yf
 from fuzzywuzzy import process
 import re
 import logging
 import functools
 import itertools
@@ -904,14 +905,15 @@
         self.lot_size = fetch_lot_size(self.name)
         self.fetch_expirys(self.symbol)
         self.freeze_qty = self.fetch_freeze_limit()
         self.available_strikes = None
         self.available_straddle_strikes = None
         self.intraday_straddle_forced_exit = False
         self.base = get_base(self.name)
+        self.strategy_log = defaultdict(list)
 
         if self.name == "BANKNIFTY":
             self.exchange_type = 1
         elif self.name == "NIFTY":
             self.exchange_type = 1
         elif self.name in [
             "FINNIFTY",
@@ -1275,22 +1277,26 @@
             raise Exception("Orders rejected")
         elif any(call_order_statuses == "open") or any(put_order_statuses == "open"):
             notifier(
                 f"{order_prefix}Some orders pending for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s). You can modify the orders.",
                 self.webhook_url,
             )
+            if return_avg_price:
+                return call_price, put_price
         elif any(call_order_statuses == "rejected") or any(
             put_order_statuses == "rejected"
         ):
             notifier(
                 f"{order_prefix}Some orders rejected for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s). You can place the rejected orders again.",
                 self.webhook_url,
             )
+            if return_avg_price:
+                return call_price, put_price
         else:
             notifier(
                 f"{order_prefix}ERROR. Order statuses uncertain for {buy_or_sell} {self.name} "
                 + f"{strike_info} {expiry} {quantity_in_lots} lot(s).",
                 self.webhook_url,
             )
             raise Exception("Order statuses uncertain")
@@ -2887,29 +2893,41 @@
             current_spot = info_dict.get("underlying_ltp")
 
             # If the spot has moved in the direction of stop loss
             time_left_day_start = info_dict.get("time_left_day_start")
             time_left_now = timetoexpiry(expiry)
             time_delta = (time_left_day_start - time_left_now) * 525600
             time_delta = int(time_delta)
-            estimated_movement = bs.target_movement(
-                side,
-                info_dict.get(f"{side}_avg_price"),
-                info_dict.get(f"{side}_stop_loss_price"),
-                entry_spot,
-                info_dict.get("traded_strangle").call_strike
-                if side == "call"
-                else info_dict.get("traded_strangle").put_strike,
-                time_left_day_start,
-                time_delta,
-            )
+            try:
+                estimated_movement = bs.target_movement(
+                    side,
+                    info_dict.get(f"{side}_avg_price"),
+                    info_dict.get(f"{side}_stop_loss_price"),
+                    entry_spot,
+                    info_dict.get("traded_strangle").call_strike
+                    if side == "call"
+                    else info_dict.get("traded_strangle").put_strike,
+                    time_left_day_start,
+                    time_delta,
+                )
+            except OptionModelInputError:
+                estimated_movement = (
+                    0.0015 if side == "call" else -0.0015
+                )  # Remove hard coded number
+                input_error_message = (
+                    f"OptionModelInputError in justify_stop_loss for {self.name} {side} strangle. "
+                    f"Setting estimated_movement to {estimated_movement}"
+                )
+                logger.error(input_error_message)
+                notifier(input_error_message, self.webhook_url)
+
             actual_movement = (current_spot - entry_spot) / entry_spot
             difference_in_sign = np.sign(estimated_movement) != np.sign(actual_movement)
             lack_of_movement = abs(actual_movement) < 0.8 * abs(estimated_movement)
-            # 0.8 above is a magic number TODO: Remove magic number and find a better way to check for lack of movement
+            # Remove hard coded number.
             if difference_in_sign or lack_of_movement:
                 if not info_dict.get(f"{side}_sl_check_notification_sent"):
                     message = (
                         f"{self.name} strangle {side} stop loss appears to be unjustified. "
                         f"Estimated movement: {estimated_movement}, Actual movement: {actual_movement}"
                     )
                     notifier(message, self.webhook_url)
@@ -3075,15 +3093,15 @@
                     break
                 refresh_orderbook = False
                 sleep(1)
 
         # Entering the main function
 
         # Setting strikes and expiry
-        order_tag = "Intraday Strangle"
+        order_tag = "Intraday strangle"
         underlying_ltp = self.fetch_ltp()
         temp_call_strike = underlying_ltp * (1 + call_strike_offset)
         temp_put_strike = underlying_ltp * (1 - put_strike_offset)
         temp_call_strike = findstrike(temp_call_strike, self.base)
         temp_put_strike = findstrike(temp_put_strike, self.base)
         expiry = self.current_expiry
 
@@ -3113,14 +3131,16 @@
             "SELL",
             quantity_in_lots,
             "LIMIT",
             order_tag,
             self.webhook_url,
             return_avg_price=True,
         )
+        call_avg_price = call_ltp if np.isnan(call_avg_price) else call_avg_price
+        put_avg_price = put_ltp if np.isnan(put_avg_price) else put_avg_price
         total_avg_price = call_avg_price + put_avg_price
 
         # Setting stop loss
         stop_loss_dict = {
             "fixed": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
             "dynamic": {"BANKNIFTY": 1.7, "NIFTY": 1.5},
         }
@@ -3141,27 +3161,28 @@
         put_stop_loss_price = (
             put_avg_price * put_stop_loss
             if put_stop_loss
             else put_avg_price * stop_loss
         )
 
         # Logging information and sending notification
-        self.log_combined_order(
-            call_strike=strangle.call_strike,
-            put_strike=strangle.put_strike,
-            expiry=expiry,
-            buy_or_sell="SELL",
-            call_price=call_avg_price,
-            put_price=put_avg_price,
-            order_tag=order_tag,
-        )
+        trade_log = {
+            "Time": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
+            "Index": self.name,
+            "Call strike": strangle.call_strike,
+            "Put strike": strangle.put_strike,
+            "Expiry": expiry,
+            "Action": "SELL",
+            "Call price": call_avg_price,
+            "Put price": put_avg_price,
+            "Total price": total_avg_price,
+            "Order tag": order_tag,
+        }
 
-        summary_message = "\n".join(
-            f"{k}: {v}" for k, v in self.order_log[order_tag][-1].items()
-        )
+        summary_message = "\n".join(f"{k}: {v}" for k, v in trade_log.items())
 
         traded_call_iv, traded_put_iv, traded_avg_iv = strangle_iv(
             callprice=call_avg_price,
             putprice=put_avg_price,
             callstrike=strangle.call_strike,
             putstrike=strangle.put_strike,
             spot=underlying_ltp,
@@ -3296,15 +3317,18 @@
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
                     self.webhook_url,
                     return_avg_price=True,
                 )
             # noinspection PyTypeChecker
-            if place_sl_orders and not shared_info_dict["exit_triggers"]["convert_to_butterfly"]:
+            if (
+                place_sl_orders
+                and not shared_info_dict["exit_triggers"]["convert_to_butterfly"]
+            ):
                 cancel_pending_orders(
                     shared_info_dict["call_stop_loss_order_ids"]
                     + shared_info_dict["put_stop_loss_order_ids"]
                 )
             shared_info_dict["call_exit_price"] = call_exit_avg_price
             shared_info_dict["put_exit_price"] = put_exit_avg_price
 
@@ -3319,15 +3343,17 @@
                     "BUY",
                     quantity_in_lots,
                     "LIMIT",
                     order_tag,
                     self.webhook_url,
                 )
             if place_sl_orders:
-                cancel_pending_orders(shared_info_dict[f"{exit_option_type}_stop_loss_order_ids"])
+                cancel_pending_orders(
+                    shared_info_dict[f"{exit_option_type}_stop_loss_order_ids"]
+                )
             shared_info_dict[f"{exit_option_type}_exit_price"] = non_sl_exit_price
 
         else:  # Both stop losses hit
             pass
 
         # Calculate profit
         total_exit_price = (
@@ -3348,43 +3374,42 @@
             f"Profit Pts: {total_avg_price - total_exit_price}\n"
         )
         exit_dict = {
             "Call exit price": shared_info_dict["call_exit_price"],
             "Put exit price": shared_info_dict["put_exit_price"],
             "Total exit price": total_exit_price,
             "Points captured": total_avg_price - total_exit_price,
-            "Call SL": shared_info_dict["call_sl"],
-            "Put SL": shared_info_dict["put_sl"],
+            "Call stop loss": shared_info_dict["call_sl"],
+            "Put stop loss": shared_info_dict["put_sl"],
         }
-        try:
-            self.order_log[order_tag][0].update(exit_dict)
-        except Exception as e:
-            notifier(
-                f"{self.name}: Error updating order list with exit details. {e}",
-                self.webhook_url,
-            )
+
         notifier(exit_message, self.webhook_url)
         shared_info_dict["trade_complete"] = True
         position_monitor_thread.join()
+
+        trade_log.update(exit_dict)
+        self.strategy_log[order_tag].append(trade_log)
+
         return shared_info_dict
 
     @log_errors
     def intraday_trend(
         self,
         quantity_in_lots,
         start_time=(9, 15, 58),
         exit_time=(15, 27),
         sleep_time=5,
         threshold_movement=None,
         seconds_to_avg=45,
         beta=0.8,
         max_entries=3,
     ):
+        strategy_tag = "Intraday trend"
+
         while currenttime().time() < time(*start_time):
-            print(f"{self.name} trender sleeping till {start_time}")
             sleep(1)
 
         open_price = self.fetch_ltp()
         threshold_movement = (
             threshold_movement or (get_current_vix() * (beta or 1)) / 48
         )
 
@@ -3406,14 +3431,15 @@
             f"Lower limit: {price_boundaries[1]:0.2f}.",
             self.webhook_url,
         )
 
         entries = 0
         last_print_time = currenttime()
         movement = 0
+        entries_log = []
         while entries < max_entries and currenttime().time() < exit_time:
             # Scan for entry condition
             notifier(
                 f"{self.name} trender {entries+1} scanning for entry condition.",
                 self.webhook_url,
             )
             while (abs(movement) < threshold_movement) and (
@@ -3448,23 +3474,47 @@
             stop_loss_price = price * (0.997 if position == "BUY" else 1.003)
             stop_loss_hit = False
             notifier(
                 f"{self.name} {position} trender triggered with {movement:0.2f} movement. {self.name} at {price}. "
                 f"Stop loss at {stop_loss_price}.",
                 self.webhook_url,
             )
-            place_option_order_and_notify(
+            call_entry_price, put_entry_price = place_option_order_and_notify(
                 atm_synthetic_fut,
                 position,
                 quantity_in_lots,
                 "LIMIT",
-                f"{self.name} trender",
+                strategy_tag,
+                self.webhook_url,
+                return_avg_price=True,
+            )
+
+            if call_entry_price == 0 or put_entry_price == 0:
+                call_entry_price, put_entry_price = atm_synthetic_fut.fetch_ltp()
+
+            entry_price = atm_strike + call_entry_price - put_entry_price
+            spot_future_basis = entry_price - price
+
+            notifier(
+                f"{self.name} trender {entries+1} entry price: {entry_price}, "
+                f"spot-future basis: {spot_future_basis}",
                 self.webhook_url,
             )
 
+            trade_info = {
+                "Entry time": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
+                "Position": position,
+                "Spot price": price,
+                "Entry price": entry_price,
+                "Spot-future basis": spot_future_basis,
+                "Stop loss": stop_loss_price,
+                "Threshold movement": threshold_movement,
+                "Movement": movement,
+            }
+
             # Tracking position
             while currenttime().time() < exit_time and not stop_loss_hit:
                 ltp = self.fetch_ltp()
                 price_deque.append(ltp)
                 avg_price = sum(price_deque) / len(price_deque) if price_deque else ltp
                 movement = (avg_price - open_price) / open_price * 100
 
@@ -3472,29 +3522,61 @@
                     (avg_price < stop_loss_price)
                     if position == "BUY"
                     else (avg_price > stop_loss_price)
                 )
                 sleep(sleep_time)
 
             # Exit condition met exiting position (stop loss or time)
+            price = self.fetch_ltp()
             stop_loss_message = f"Trender stop loss hit. " if stop_loss_hit else ""
             notifier(
-                f"{stop_loss_message}{self.name} trender {entries+1} exiting. {self.name} at {self.fetch_ltp()}.",
+                f"{stop_loss_message}{self.name} trender {entries+1} exiting. {self.name} at {price}.",
                 self.webhook_url,
             )
-            place_option_order_and_notify(
+            call_exit_price, put_exit_price = place_option_order_and_notify(
                 atm_synthetic_fut,
                 "BUY" if position == "SELL" else "SELL",
                 quantity_in_lots,
                 "LIMIT",
-                f"{self.name} trender",
+                strategy_tag,
                 self.webhook_url,
             )
+
+            if call_exit_price == 0 or put_exit_price == 0:
+                call_exit_price, put_exit_price = atm_synthetic_fut.fetch_ltp()
+
+            exit_price = atm_strike + call_exit_price - put_exit_price
+            pnl = (
+                (exit_price - entry_price)
+                if position == "BUY"
+                else (entry_price - exit_price)
+            )
+            spot_future_basis = exit_price - price
+
+            notifier(
+                f"{self.name} trender {entries+1} exit price: {exit_price}, "
+                f"spot-future basis: {spot_future_basis}, pnl: {pnl}",
+                self.webhook_url,
+            )
+
+            trade_info.update(
+                {
+                    "Exit time": currenttime().strftime("%d-%m-%Y %H:%M:%S"),
+                    "Stop loss hit": stop_loss_hit,
+                    "Spot exit price": price,
+                    "Exit price": exit_price,
+                    "Spot-future basis": spot_future_basis,
+                    "PnL": pnl,
+                }
+            )
+            entries_log.append(trade_info)
             entries += 1
 
+        self.strategy_log[strategy_tag].extend(entries_log)
+
     def intraday_straddle_delta_hedged(
         self,
         quantity_in_lots,
         exit_time=(15, 30),
         websocket=None,
         wait_for_equality=False,
         delta_threshold=1,
@@ -3678,32 +3760,41 @@
         return data.tolist()
     elif hasattr(data, "item"):  # Check for numpy scalar types, e.g., numpy.int32
         return data.item()
     else:
         return data
 
 
-def append_data_to_json(data_dict: defaultdict, file_name: str):
+def append_data_to_json(new_data: defaultdict | dict | list, file_name: str) -> None:
     # Attempt to read the existing data from the JSON file
     try:
         with open(file_name, "r") as file:
-            data = json.load(file)
+            existing_data = json.load(file)
     except (FileNotFoundError, json.JSONDecodeError):
         # If the file doesn't exist or has invalid JSON content, create an empty list and write it to the file
-        data = []
+        existing_data = []
         with open(file_name, "w") as file:
-            json.dump(data, file)
+            json.dump(existing_data, file)
 
     # Convert the defaultdict to a regular dict, make it JSON serializable, and append it to the list
-    serializable_data = convert_to_serializable(dict(data_dict))
-    data.append(serializable_data)
+
+    if isinstance(new_data, (defaultdict, dict)):
+        if isinstance(new_data, defaultdict):
+            new_data = dict(new_data)
+        serialized_data = convert_to_serializable(new_data)
+        existing_data.append(serialized_data)
+    elif isinstance(new_data, list):
+        serialized_data = convert_to_serializable(new_data)
+        existing_data.extend(serialized_data)
+    else:
+        raise TypeError("New data must be a defaultdict, dict, or list.")
 
     # Write the updated data back to the JSON file with indentation
     with open(file_name, "w") as file:
-        json.dump(data, file, indent=4, default=str)
+        json.dump(existing_data, file, indent=4, default=str)
 
 
 def word_to_num(s):
     word = {
         "one": 1,
         "two": 2,
         "three": 3,
@@ -3833,41 +3924,88 @@
         return fetch_data(obj.orderBook, "orderbook")
     elif book in {"positions", "position"}:
         return fetch_data(obj.position, "positions")
     else:
         raise ValueError(f"Invalid book type '{book}'.")
 
 
-def lookup_and_return(book, field_to_lookup, value_to_lookup, field_to_return):
+def lookup_and_return(
+    book, field_to_lookup, value_to_lookup, field_to_return
+) -> np.array:
     def filter_and_return(data: list):
-        if not isinstance(field_to_lookup, list):
+        if not isinstance(field_to_lookup, (list, tuple, np.ndarray)):
             field_to_lookup_ = [field_to_lookup]
             value_to_lookup_ = [value_to_lookup]
         else:
             field_to_lookup_ = field_to_lookup
             value_to_lookup_ = value_to_lookup
 
-        bucket = [
-            entry[field_to_return]
-            for entry in data
-            if all(
-                (
-                    entry[field] == value
-                    if not isinstance(value, list)
-                    else entry[field] in value
+        if isinstance(
+            field_to_return, (list, tuple, np.ndarray)
+        ):  # Return a dict as multiple fields are requested
+            bucket = {field: [] for field in field_to_return}
+            for entry in data:
+                if all(
+                    (
+                        entry[field] == value
+                        if not isinstance(value, (list, tuple, np.ndarray))
+                        else entry[field] in value
+                    )
+                    for field, value in zip(field_to_lookup_, value_to_lookup_)
+                ) and all(entry[field] != "" for field in field_to_lookup_):
+                    for field in field_to_return:
+                        bucket[field].append(entry[field])
+
+            if all(len(v) == 0 for v in bucket.values()):
+                return {}
+            else:
+                # Flatten the dictionary if all fields contain only one value
+                if all(len(v) == 1 for v in bucket.values()):
+                    bucket = {k: v[0] for k, v in bucket.items()}
+                return bucket
+        else:  # Return a numpy array as only one field is requested
+            # Check if 'orderid' is in field_to_lookup_
+            if "orderid" in field_to_lookup_:
+                sort_by_orderid = True
+                orderid_index = field_to_lookup_.index("orderid")
+            else:
+                sort_by_orderid = False
+                orderid_index = None
+
+            bucket = [
+                (entry["orderid"], entry[field_to_return])
+                if sort_by_orderid
+                else entry[field_to_return]
+                for entry in data
+                if all(
+                    (
+                        entry[field] == value
+                        if not isinstance(value, (list, tuple, np.ndarray))
+                        else entry[field] in value
+                    )
+                    for field, value in zip(field_to_lookup_, value_to_lookup_)
                 )
-                for field, value in zip(field_to_lookup_, value_to_lookup_)
-            )
-            and all(entry[field] != "" for field in field_to_lookup_)
-        ]
+                and all(entry[field] != "" for field in field_to_lookup_)
+            ]
 
-        if len(bucket) == 0:
-            return 0
-        else:
-            return np.array(bucket)
+            if len(bucket) == 0:
+                return np.array([])
+            else:
+                if sort_by_orderid:
+                    # Create a dict mapping order ids to their index in value_to_lookup
+                    orderid_to_index = {
+                        value: index
+                        for index, value in enumerate(value_to_lookup_[orderid_index])
+                    }
+                    # Sort the bucket based on the order of 'orderid' in value_to_lookup
+                    bucket.sort(key=lambda x: orderid_to_index[x[0]])
+                    # Return only the field_to_return values
+                    return np.array([x[1] for x in bucket])
+                else:
+                    return np.array(bucket)
 
     if not (
         isinstance(field_to_lookup, (str, list, tuple, np.ndarray))
         and isinstance(value_to_lookup, (str, list, tuple, np.ndarray))
     ):
         raise ValueError(
             "Both 'field_to_lookup' and 'value_to_lookup' must be strings or lists."
@@ -4034,15 +4172,15 @@
     notify_url=None,
 ):
     pending_text = "trigger pending"
     context = f"{context} " if context else ""
 
     statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
 
-    if isinstance(statuses, (int, np.int32, np.int64)):
+    if not isinstance(statuses, np.ndarray) or statuses.size == 0:
         logger.error(f"Statuses is {statuses} for orderid(s) {order_ids}")
 
     if all(statuses == pending_text):
         return False, False
 
     elif all(statuses == "rejected") or all(statuses == "cancelled"):
         rejection_reasons = lookup_and_return(order_book, "orderid", order_ids, "text")
@@ -4252,15 +4390,17 @@
     ].sort_values("expiry_dt")
     closest_expiry = strike_array.expiry_dt.iloc[0]
     strike_array = (
         strike_array.loc[strike_array.expiry_dt == closest_expiry]["strike"] / 100
     )
     upper_bound = np.percentile(strike_array, 90)
     lower_bound = np.percentile(strike_array, 30)
-    strike_array = strike_array[strike_array.between(lower_bound, upper_bound, inclusive='both')]
+    strike_array = strike_array[
+        strike_array.between(lower_bound, upper_bound, inclusive="both")
+    ]
     strike_differences = np.diff(strike_array.sort_values().unique())
     values, counts = np.unique(strike_differences, return_counts=True)
     mode = values[np.argmax(counts)]
     return mode
 
 
 def fetch_symbol_token(
@@ -4958,13 +5098,109 @@
     syn_fut = SyntheticFuture(strike, name, expiry)
     call_order_ids, put_order_ids = syn_fut.place_order(
         buy_or_sell, quantity_in_lots, prices, stop_loss_order, order_tag
     )
     return call_order_ids, put_order_ids
 
 
+def handle_open_orders(*order_ids, action, modify_percentage=0.01, stage=0):
+    """Modifies orders if they are pending by the provided modification percentage"""
+    print(
+        f"\nEntering handle_open_orders with order_ids: {order_ids}, "
+        f"modify_percentage: {modify_percentage}, stage: {stage}"
+    )
+
+    if stage >= 10:
+        print("Stage >= 10, exiting function without modifying any orders")
+        return None
+
+    stage_increment = int(modify_percentage * 100)
+    stage_increment = max(stage_increment, 1)
+    print(f"Calculated stage_increment as: {stage_increment}")
+
+    order_book = fetch_book("orderbook")
+    sleep(1)
+
+    statuses = lookup_and_return(order_book, "orderid", order_ids, "status")
+    print(f"Looked up order statuses: {statuses}")
+
+    if all(statuses == "complete"):
+        print("All orders are complete, exiting function without modifying any orders")
+        return None
+    elif any(np.isin(statuses, ["rejected", "cancelled"])):
+        print(
+            "Some orders are rejected or cancelled, exiting function without modifying any orders"
+        )
+        return None
+    elif any(statuses == "open"):
+        print("Some orders are open, proceeding with modifications")
+
+        open_order_ids = [
+            order_id
+            for order_id, status in zip(order_ids, statuses)
+            if status == "open"
+        ]
+        print(f"Open order ids: {open_order_ids}")
+
+        for order_id in open_order_ids:
+            relevant_fields = [
+                "orderid",
+                "variety",
+                "symboltoken",
+                "price",
+                "ordertype",
+                "producttype",
+                "exchange",
+                "tradingsymbol",
+                "quantity",
+                "duration",
+                "status",
+            ]
+
+            current_params = lookup_and_return(
+                order_book, "orderid", order_id, relevant_fields
+            )
+            print(f"Current params for order {order_id}: {current_params}")
+
+            old_price = current_params["price"]
+            print(f"Old price for order {order_id}: {old_price}")
+
+            new_price = (
+                old_price * (1 + modify_percentage)
+                if action == "BUY"
+                else old_price * (1 - modify_percentage)
+            )
+            new_price = custom_round(new_price)
+            print(f"New price for order {order_id}: {new_price}")
+
+            modified_params = current_params.copy()
+            modified_params["price"] = new_price
+            modified_params.pop("status")
+            # print(f"Modified params for order {order_id}: {modified_params}")
+
+            obj.modifyOrder(modified_params)
+            print(f"Modified order {order_id} with new price: {new_price}")
+
+        order_book = fetch_book("orderbook")
+        sleep(1)
+
+        statuses = lookup_and_return(order_book, "orderid", open_order_ids, "status")
+        print(f"Looked up order statuses after modifications: {statuses}")
+
+        if any(statuses == "open"):
+            print("Some orders are still open, recalling function with increased stage")
+            return handle_open_orders(
+                *open_order_ids,
+                action=action,
+                modify_percentage=modify_percentage,
+                stage=stage + stage_increment,
+            )
+
+        print("All orders are now complete or closed, exiting function")
+
+
 def cancel_pending_orders(order_ids, variety="STOPLOSS"):
     if isinstance(order_ids, (list, np.ndarray)):
         for order_id in order_ids:
             obj.cancelOrder(order_id, variety)
     else:
         obj.cancelOrder(order_ids, variety)
```

### Comparing `volstreet-1.0.9/volstreet/discord_bot.py` & `volstreet-1.1.0/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.9/volstreet/nsefunctions.py` & `volstreet-1.1.0/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.0.9/volstreet/strategies.py` & `volstreet-1.1.0/volstreet/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,17 @@
         webhook_url=discord_webhook_url,
     )
     nifty = vs.Index("NIFTY", webhook_url=discord_webhook_url)
     bnf = vs.Index("BANKNIFTY", webhook_url=discord_webhook_url)
     fin = vs.Index("FINNIFTY", webhook_url=discord_webhook_url)
     midcap = vs.Index("MIDCPNIFTY", webhook_url=discord_webhook_url)
 
-    indices = vs.get_strangle_indices_to_trade(nifty, bnf, fin, midcap, safe_indices=safe_indices)
+    indices = vs.get_strangle_indices_to_trade(
+        nifty, bnf, fin, midcap, safe_indices=safe_indices
+    )
 
     parameters["quantity_in_lots"] = parameters["quantity_in_lots"] // len(indices)
 
     # Setting the shared data
     if shared_data:
         shared_data = vs.SharedData()
         update_data_thread = threading.Thread(target=shared_data.update_data)
@@ -129,16 +131,18 @@
     if shared_data and update_data_thread is not None:
         shared_data.force_stop = True
         update_data_thread.join()
 
     # Call the data appender function on the traded indices
     for index in indices:
         vs.append_data_to_json(
-            index.order_log, f"{user}_{index.name}_{strategy}_log.json"
+            index.strategy_log["Intraday strangle"],
+            f"{user}_{index.name}_intraday_strangle.json",
         )
+        vs.notifier(f"Appended data for {index.name} {strategy}.", discord_webhook_url)
 
 
 def overnight_straddle_nifty(
     quantity_in_lots,
     client=None,
     user=None,
     pin=None,
@@ -217,40 +221,60 @@
 
     """
 
     user, pin, apikey, authkey, discord_webhook_url = get_user_data(
         client, user, pin, apikey, authkey, webhook_url
     )
 
+    if special_parameters is None:
+        special_parameters = {}
+
     if vs.currenttime().date() in vs.holidays:
         vs.notifier("Today is a holiday hence exiting.", discord_webhook_url)
         exit()
 
     vs.login(
         user=user,
         pin=pin,
         apikey=apikey,
         authkey=authkey,
         webhook_url=discord_webhook_url,
     )
 
+    indices = [vs.Index(index, webhook_url=discord_webhook_url) for index in indices]
+
     threads = []
-    for index_symbol in indices:
+    for index in indices:
         index_parameters = parameters.copy()
-        index_parameters.update(special_parameters.get(index_symbol, {}))
-        index = vs.Index(index_symbol, webhook_url=discord_webhook_url)
+        index_parameters.update(special_parameters.get(index.name, {}))
         thread = threading.Thread(target=index.intraday_trend, kwargs=index_parameters)
         threads.append(thread)
 
     for thread in threads:
         thread.start()
 
     for thread in threads:
         thread.join()
 
+    # Call the data appender function on the traded indices
+    for index in indices:
+        try:  # Remove this try except block after testing
+            vs.append_data_to_json(
+                index.strategy_log["Intraday trend"],
+                f"{user}_{index.name}_intraday_trend.json",
+            )
+            vs.notifier(
+                f"Appended data for {index.name} intraday trend.", discord_webhook_url
+            )
+        except Exception as e:
+            vs.notifier(
+                f"Appending intraday trend data failed for {index.name}: {e}",
+                discord_webhook_url,
+            )
+
 
 def index_vs_constituents(
     index_symbol,
     strike_offset=0,
     index_strike_offset=None,
     cutoff_pct=90,
     exposure_per_stock=10000000,
```

### Comparing `volstreet-1.0.9/volstreet.egg-info/requires.txt` & `volstreet-1.1.0/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

