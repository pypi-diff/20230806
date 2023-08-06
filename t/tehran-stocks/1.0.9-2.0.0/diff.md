# Comparing `tmp/tehran-stocks-1.0.9.tar.gz` & `tmp/tehran_stocks-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tehran-stocks-1.0.9.tar", max compression
+gzip compressed data, was "tehran_stocks-2.0.0.tar", max compression
```

## Comparing `tehran-stocks-1.0.9.tar` & `tehran_stocks-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,16 @@
--rw-r--r--   0        0        0     1068 2021-12-12 15:56:59.756477 tehran-stocks-1.0.9/LICENSE
--rw-r--r--   0        0        0     6807 2022-04-18 11:47:46.542098 tehran-stocks-1.0.9/README.md
--rw-r--r--   0        0        0      839 2022-06-19 13:56:12.866963 tehran-stocks-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      539 2022-04-04 10:58:59.417610 tehran-stocks-1.0.9/src/tehran_stocks/__init__.py
--rw-r--r--   0        0        0       22 2021-12-12 15:56:59.757598 tehran-stocks-1.0.9/src/tehran_stocks/config/__init__.py
--rw-r--r--   0        0        0      200 2022-06-19 13:40:50.571642 tehran-stocks-1.0.9/src/tehran_stocks/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      198 2021-12-12 16:50:12.747245 tehran-stocks-1.0.9/src/tehran_stocks/config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2902 2022-06-19 13:41:15.725186 tehran-stocks-1.0.9/src/tehran_stocks/config/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     2587 2022-04-18 12:07:07.814047 tehran-stocks-1.0.9/src/tehran_stocks/config/__pycache__/engine.cpython-39.pyc
--rw-r--r--   0        0        0      100 2022-04-04 10:58:59.418002 tehran-stocks-1.0.9/src/tehran_stocks/config/config.default.yml
--rw-r--r--   0        0        0     2313 2022-06-19 13:51:31.211898 tehran-stocks-1.0.9/src/tehran_stocks/config/engine.py
--rw-r--r--   0        0        0      154 2021-12-12 15:56:59.757825 tehran-stocks-1.0.9/src/tehran_stocks/download/__init__.py
--rw-r--r--   0        0        0      396 2022-03-15 11:37:19.831563 tehran-stocks-1.0.9/src/tehran_stocks/download/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4424 2022-04-18 12:07:10.408464 tehran-stocks-1.0.9/src/tehran_stocks/download/__pycache__/names.cpython-39.pyc
--rw-r--r--   0        0        0     5113 2022-04-18 12:07:41.752704 tehran-stocks-1.0.9/src/tehran_stocks/download/__pycache__/price.cpython-39.pyc
--rw-r--r--   0        0        0     4606 2022-06-19 11:43:42.915594 tehran-stocks-1.0.9/src/tehran_stocks/download/names.py
--rw-r--r--   0        0        0     4760 2022-04-04 10:58:59.419290 tehran-stocks-1.0.9/src/tehran_stocks/download/price.py
--rw-r--r--   0        0        0     1384 2022-06-19 11:46:50.562212 tehran-stocks-1.0.9/src/tehran_stocks/initializer.py
--rw-r--r--   0        0        0       77 2021-12-12 15:56:59.758248 tehran-stocks-1.0.9/src/tehran_stocks/models/__init__.py
--rw-r--r--   0        0        0      282 2022-03-15 11:37:19.902313 tehran-stocks-1.0.9/src/tehran_stocks/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      451 2022-04-18 12:07:10.555772 tehran-stocks-1.0.9/src/tehran_stocks/models/__pycache__/create.cpython-39.pyc
--rw-r--r--   0        0        0     6527 2022-04-18 12:07:10.557817 tehran-stocks-1.0.9/src/tehran_stocks/models/__pycache__/stocks.cpython-39.pyc
--rw-r--r--   0        0        0      171 2022-04-04 10:58:59.419898 tehran-stocks-1.0.9/src/tehran_stocks/models/create.py
--rw-r--r--   0        0        0     6610 2022-04-18 11:47:46.544682 tehran-stocks-1.0.9/src/tehran_stocks/models/stocks.py
--rw-r--r--   0        0        0     8096 2022-06-19 13:56:27.256505 tehran-stocks-1.0.9/setup.py
--rw-r--r--   0        0        0     7811 2022-06-19 13:56:27.256975 tehran-stocks-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-06 12:20:17.496880 tehran_stocks-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6807 2023-08-06 12:20:17.497161 tehran_stocks-2.0.0/README.md
+-rw-r--r--   0        0        0      853 2023-08-06 13:41:30.753248 tehran_stocks-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-08-06 12:20:17.498265 tehran_stocks-2.0.0/src/tehran_stocks/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-06 12:20:17.498345 tehran_stocks-2.0.0/src/tehran_stocks/config/__init__.py
+-rw-r--r--   0        0        0      100 2023-08-06 12:20:17.498397 tehran_stocks-2.0.0/src/tehran_stocks/config/config.default.yml
+-rw-r--r--   0        0        0     2313 2023-08-06 12:20:17.498457 tehran_stocks-2.0.0/src/tehran_stocks/config/engine.py
+-rw-r--r--   0        0        0      154 2023-08-06 12:20:17.498536 tehran_stocks-2.0.0/src/tehran_stocks/download/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-06 13:41:30.753363 tehran_stocks-2.0.0/src/tehran_stocks/download/base.py
+-rw-r--r--   0        0        0     4722 2023-08-06 13:41:30.753681 tehran_stocks-2.0.0/src/tehran_stocks/download/names.py
+-rw-r--r--   0        0        0     4853 2023-08-06 13:41:30.754078 tehran_stocks-2.0.0/src/tehran_stocks/download/price.py
+-rw-r--r--   0        0        0     1384 2023-08-06 12:20:17.498736 tehran_stocks-2.0.0/src/tehran_stocks/initializer.py
+-rw-r--r--   0        0        0       77 2023-08-06 12:20:17.498838 tehran_stocks-2.0.0/src/tehran_stocks/models/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-06 12:20:17.498892 tehran_stocks-2.0.0/src/tehran_stocks/models/create.py
+-rw-r--r--   0        0        0     6626 2023-08-06 13:41:30.754423 tehran_stocks-2.0.0/src/tehran_stocks/models/stocks.py
+-rw-r--r--   0        0        0     7771 1970-01-01 00:00:00.000000 tehran_stocks-2.0.0/PKG-INFO
```

### Comparing `tehran-stocks-1.0.9/LICENSE` & `tehran_stocks-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tehran-stocks-1.0.9/README.md` & `tehran_stocks-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tehran-stocks-1.0.9/pyproject.toml` & `tehran_stocks-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "tehran-stocks"
-version = "1.0.9"
+version = "2.0.0"
 description = "Data Downloader for Tehran stock market"
 authors = ["Mehdi Ghodsizadeh <mehdi.ghodsizadeh@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ghodsizadeh.github.io/tehran-stocks/"
 repository = "https://github.com/ghodsizadeh/tehran-stocks.git"
 packages = [
     { include = "tehran_stocks", from = 'src' }
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = "^3.8.1"
 requests = "^2.26.0"
 SQLAlchemy = "^1.4.28"
 jalali-pandas = "^0.2.0"
-pandas = "^1.3.5"
 lxml = "^4.8.0"
-aiohttp = "^3.8.1"
-cchardet = "^2.1.7"
+aiohttp = "^3.8.5"
 aiodns = "^3.0.0"
 PyYAML = "^6.0"
+pandas = "^2.0.3"
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.group.dev.dependencies]
 pre-commit = "^2.16.0"
 pylint = "^2.12.2"
-pytest = "^6.2.5"
+pytest = "^7.4.0"
 ipython = "^7.31.0"
 ipdb = "^0.13.9"
+pytest-asyncio = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/__init__.py` & `tehran_stocks-2.0.0/src/tehran_stocks/__init__.py`

 * *Files identical despite different names*

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/config/engine.py` & `tehran_stocks-2.0.0/src/tehran_stocks/config/engine.py`

 * *Files identical despite different names*

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/download/names.py` & `tehran_stocks-2.0.0/src/tehran_stocks/download/names.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from asyncio import tasks
 import requests
 import re
 import time
 import tehran_stocks.config as db
 from tehran_stocks.models import Stocks
-
+from .base import BASE_URL
 
 def get_stock_ids():
-    url = "http://tsetmc.com/tsev2/data/MarketWatchPlus.aspx"
+    url = f"{BASE_URL}/tsev2/data/MarketWatchPlus.aspx"
     r = requests.get(url)
     ids = set(re.findall(r"\d{15,20}", r.text))
     return list(ids)
 
 
 def get_stock_groups():
     """
     group numbers from tccim, to avoid searching useless group numbers.
     its a helper for other parts of package to collect stock lists.
     """
-    r = requests.get("http://www.tsetmc.com/Loader.aspx?ParTree=111C1213")
-    return re.findall(r"\d{2}", r.text)
+    r = requests.get(f"{BASE_URL}/Loader.aspx?ParTree=111C1213")
+    return list(set(re.findall(r"\d{2}", r.text)))
 
 
 def create_or_update_stock_from_dict(stock_id, stock):
     if exist := Stocks.query.filter_by(code=stock_id).first():
         print(f"stock with code {stock_id} exist")
         exist.shareCount = stock["shareCount"]
         exist.baseVol = stock["baseVol"]
@@ -47,20 +47,23 @@
         an str of an interger or an integer if not started by 0 whicj represent  the Id
         in tsetmc website i.e. arg i={stock_id} inside  the url
     group_id:
         int: number that represent group of stock
 
     """
 
-    url = f"http://www.tsetmc.com/Loader.aspx?ParTree=151311&i={stock_id}"
+    url = f"{BASE_URL}/Loader.aspx?ParTree=151311&i={stock_id}"
     r = requests.get(url)
-    stock = {
-        "code": stock_id,
-        "instId": re.findall(r"InstrumentID='([\w\d]*)|$',", r.text)[0],
-    }
+    try:
+        stock = {
+            "code": stock_id,
+            "instId": re.findall(r"InstrumentID='([\w\d]*)|$',", r.text)[0],
+        }
+    except IndexError:
+        return 
 
     stock["insCode"] = (
         stock_id if re.findall(r"InsCode='(\d*)',", r.text)[0] == stock_id else 0
     )
     stock["baseVol"] = float(re.findall(r"BaseVol=([\.\d]*),", r.text)[0])
     try:
         stock["name"] = re.findall(r"LVal18AFC='([\D]*)',", r.text)[0]
@@ -108,36 +111,36 @@
     Download Stock Table,
     1- gets groups
     2- gets stock in groups
     3- download stock detail
     4- save them to database
     5- guides you to use the package
     """
-    URL = "https://ts-api.ir/api/stocks"
-    try:
-        print("try Downloading stock table from the package api... ")
-        print("visit: https://ts-api.ir/")
-        r = requests.get(URL)
-        if r.status_code != 200:
-            raise ConnectionError("connection error")
-        data = r.json()
-        stocks = data["stocks"]
-        db.session.rollback()
-        for stock in stocks:
-            del stock["id"]
-            create_or_update_stock_from_dict(stock["code"], stock)
-        db.session.commit()
-        return
-
-    except ConnectionError:
-        print("fall back to manual mode")
-        pass
-    except Exception as e:
-        print(e)
-        pass
+    # URL = "https://ts-api.ir/api/stocks"
+    # try:
+    #     print("try Downloading stock table from the package api... ")
+    #     print("visit: https://ts-api.ir/")
+    #     r = requests.get(URL)
+    #     if r.status_code != 200:
+    #         raise ConnectionError("connection error")
+    #     data = r.json()
+    #     stocks = data["stocks"]
+    #     db.session.rollback()
+    #     for stock in stocks:
+    #         del stock["id"]
+    #         create_or_update_stock_from_dict(stock["code"], stock)
+    #     db.session.commit()
+    #     return
+
+    # except ConnectionError:
+    #     print("fall back to manual mode")
+    #     pass
+    # except Exception as e:
+    #     print(e)
+    #     pass
     print("Downloading group ids...")
     stocks = get_stock_ids()
     for i, stock in enumerate(stocks):
         get_stock_detail(stock)
         print(
             f"downloading stocks details, changes: {(i+1)/len(stocks)*100:.1f}% completed",
             end="\r",
```

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/download/price.py` & `tehran_stocks-2.0.0/src/tehran_stocks/download/price.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import aiohttp
 import pandas as pd
 import requests
 import io
 
 import tehran_stocks.config as db
 from tehran_stocks.models import StockPrice, Stocks
+from .base import BASE_URL
 
 
 def convert_to_shamsi(date):
     date = str(date)
     return jdate.fromgregorian(
         day=int(date[-2:]), month=int(date[4:6]), year=int(date[:4])
     ).strftime("%Y/%m/%d")
@@ -21,15 +22,15 @@
 
 def get_stock_price_history(stock_id: int) -> pd.DataFrame:
     """Get stock price history from the web.
 
     params:
     ----------------
     stock_id: int
-        http://www.tsetmc.com/Loader.aspx?ParTree=151311&i=**35700344742885862#**
+        http://www.old.tsetmc.com/Loader.aspx?ParTree=151311&i=**35700344742885862#**
         number after i=
 
     return:
     ----------------
     pd.DataFrame
         date: str
         open: float
@@ -39,18 +40,21 @@
         volume: int
 
     example
     ----------------
     df = get_stock_price_history(35700344742885862)
     """
     now = datetime.now().strftime("%Y%m%d")
-    url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={stock_id}&DateFrom=20000101&DateTo={now}&b=0"
+    url = f"{BASE_URL}/tse/data/Export-txt.aspx?a=InsTrade&InsCode={stock_id}&DateFrom=20000101&DateTo={now}&b=0"
+
     s = requests.get(url).content
     df = pd.read_csv(io.StringIO(s.decode("utf-8")))
     df.columns = [i[1:-1].lower() for i in df.columns]
+    if 'ticker' not in df.columns or 'close' not in df.columns:
+        return pd.DataFrame()
     return df
 
 
 async def update_stock_price(code: str):
     """
     Update (or download for the first time) Stock prices
 
@@ -76,17 +80,17 @@
             )
             max_date = pd.read_sql(max_date_query, db.engine)
             last_date = max_date.date.iat[0]
         except Exception as e:
             last_date = None
         try:
             if last_date is None:  # no any record added in database
-                url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom=20000101&DateTo={now}&b=0"
+                url = f"{BASE_URL}/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom=20000101&DateTo={now}&b=0"
             elif str(last_date) < now:  # need to updata new price data
-                url = f"http://www.tsetmc.com/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom={str(last_date)}&DateTo={now}&b=0"
+                url = f"{BASE_URL}/tse/data/Export-txt.aspx?a=InsTrade&InsCode={code}&DateFrom={str(last_date)}&DateTo={now}&b=0"
             else:  # The price data for this code is updateed
                 return
         except Exception as e:
             print(f"Error on formating price:{str(e)}")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as resp:
```

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/initializer.py` & `tehran_stocks-2.0.0/src/tehran_stocks/initializer.py`

 * *Files identical despite different names*

### Comparing `tehran-stocks-1.0.9/src/tehran_stocks/models/stocks.py` & `tehran_stocks-2.0.0/src/tehran_stocks/models/stocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from tehran_stocks.config import *
 from sqlalchemy.orm import relationship
 import pandas as pd
 import requests
 import jalali_pandas
+from tehran_stocks.download.base import BASE_URL
 
 
 class Stocks(Base):
     __tablename__ = "stocks"
 
     id = Column(Integer, primary_key=True)
     name = Column(String)
@@ -53,30 +54,30 @@
         """get changes in price for dividend and changes in share
         postive value is dividend and negative value is changes in share
 
         Returns:
             pd.DataFrame: _description_
         """
 
-        url = f"http://www.tsetmc.com/Loader.aspx?Partree=15131G&i={self.code}"
+        url = f"{BASE_URL}/Loader.aspx?Partree=15131G&i={self.code}"
         r = requests.get(url)
         changes = pd.read_html(r.text)[0]
         changes.columns = ["date", "after", "before"]
         changes["dividend"] = changes.before - changes.after
         changes["date"] = changes.date.jalali.parse_jalali("%Y/%m/%d")
         changes["gdate"] = changes.date.jalali.to_gregorian()
         return changes
 
     def get_shares_history(self) -> pd.DataFrame:
         """_summary_get changes in shares
 
         Returns:
             pd.DataFrame: return day of shares changes and shares count [date, new_shares, old_shares, gdate]
         """
-        url = f"http://www.tsetmc.com/Loader.aspx?Partree=15131H&i={self.code}"
+        url = f"{BASE_URL}/Loader.aspx?Partree=15131H&i={self.code}"
         r = requests.get(url)
         df = pd.read_html(r.text)[0]
         df.columns = ["date", "new_shares", "old_shares"]
         df["date"] = df.date.jalali.parse_jalali("%Y/%m/%d")
         df["gdate"] = df.date.jalali.to_gregorian()
         return df
 
@@ -116,15 +117,15 @@
         last_price, last_close, last_open, last_high, last_low, last_vol, trade_count, trade_value,market_cap
         instantly from the website
 
         Returns:
             dict: { last_price, last_close, last_open, last_high, last_low, last_vol, trade_count, trade_value,market_cap}
         """
         url = (
-            f"http://www.tsetmc.com/tsev2/data/instinfodata.aspx?i={self.code}&c=27%20"
+            f"{BASE_URL}/tsev2/data/instinfodata.aspx?i={self.code}&c=27%20"
         )
         headers = {
             "Connection": "keep-alive",
             "Accept": "text/plain, */*; q=0.01",
             "DNT": "1",
             "X-Requested-With": "XMLHttpRequest",
             "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.74 Safari/537.36",
```

### Comparing `tehran-stocks-1.0.9/PKG-INFO` & `tehran_stocks-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: tehran-stocks
-Version: 1.0.9
+Version: 2.0.0
 Summary: Data Downloader for Tehran stock market
 Home-page: https://ghodsizadeh.github.io/tehran-stocks/
 License: MIT
 Author: Mehdi Ghodsizadeh
 Author-email: mehdi.ghodsizadeh@gmail.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: SQLAlchemy (>=1.4.28,<2.0.0)
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: cchardet (>=2.1.7,<3.0.0)
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: jalali-pandas (>=0.2.0,<0.3.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/ghodsizadeh/tehran-stocks.git
 Description-Content-Type: text/markdown
 
 # Tehran Stock Market بورس تهران در پایتون
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
```

