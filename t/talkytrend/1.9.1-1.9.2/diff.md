# Comparing `tmp/talkytrend-1.9.1.tar.gz` & `tmp/talkytrend-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.9.1.tar", max compression
+gzip compressed data, was "talkytrend-1.9.2.tar", max compression
```

## Comparing `talkytrend-1.9.1.tar` & `talkytrend-1.9.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-19 15:22:48.076501 talkytrend-1.9.1/LICENSE
--rw-r--r--   0        0        0     3419 2023-07-19 15:22:48.076501 talkytrend-1.9.1/README.md
--rw-r--r--   0        0        0     3107 2023-07-19 15:22:51.404527 talkytrend-1.9.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-19 15:22:51.412527 talkytrend-1.9.1/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/config.py
--rw-r--r--   0        0        0     2542 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6432 2023-07-19 15:22:48.076501 talkytrend-1.9.1/talkytrend/main.py
--rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 talkytrend-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-19 17:21:08.201546 talkytrend-1.9.2/LICENSE
+-rw-r--r--   0        0        0     3419 2023-07-19 17:21:08.201546 talkytrend-1.9.2/README.md
+-rw-r--r--   0        0        0     3107 2023-07-19 17:21:10.825568 talkytrend-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-19 17:21:10.833568 talkytrend-1.9.2/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-19 17:21:08.201546 talkytrend-1.9.2/talkytrend/config.py
+-rw-r--r--   0        0        0     2543 2023-07-19 17:21:08.201546 talkytrend-1.9.2/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6490 2023-07-19 17:21:08.201546 talkytrend-1.9.2/talkytrend/main.py
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 talkytrend-1.9.2/PKG-INFO
```

### Comparing `talkytrend-1.9.1/LICENSE` & `talkytrend-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.9.1/README.md` & `talkytrend-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.9.1/pyproject.toml` & `talkytrend-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.9.1"
+version = "1.9.2"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.9.1/talkytrend/config.py` & `talkytrend-1.9.2/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.9.1/talkytrend/default_settings.toml` & `talkytrend-1.9.2/talkytrend/default_settings.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 enable_feed = true
 news_feed = "http://feeds.feedburner.com/zerohedge/feed/"
 # news_feed="https://www.financialjuice.com/feed.ashx?xy=rss"
 # news_feed = "https://www.dailyfx.com/feeds/market-news"
 #news_feed="https://www.reutersagency.com/feed/?taxonomy=best-sectors&post_type=best"
 finnhub_api_key= ""
 alphavantage_api_key = "demo"
-twelvedata_api_key = ""
+twelvedata_api_key = ""
```

### Comparing `talkytrend-1.9.1/talkytrend/main.py` & `talkytrend-1.9.2/talkytrend/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,17 @@
                     "signal": current_signal
                 }
                 table.add_row([asset["id"], current_signal])
                 signals.append(signal_item)
 
         return table.get_string()
 
+    async def fetch_sentiment(self):
+        return None
+
     async def fetch_key_events(self):
         def filter_events(data, today):
             return [event for event in data if event.get('date', '') > today]
 
         def is_usd_high_impact(event):
             return (
                 event.get('impact') == 'High' and
```

### Comparing `talkytrend-1.9.1/PKG-INFO` & `talkytrend-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.9.1
+Version: 1.9.2
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.9.1 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.9.2 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

