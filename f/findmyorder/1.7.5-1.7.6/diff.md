# Comparing `tmp/findmyorder-1.7.5.tar.gz` & `tmp/findmyorder-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.7.5.tar", max compression
+gzip compressed data, was "findmyorder-1.7.6.tar", max compression
```

## Comparing `findmyorder-1.7.5.tar` & `findmyorder-1.7.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-08-05 16:15:37.301501 findmyorder-1.7.5/LICENSE
--rw-r--r--   0        0        0     2834 2023-08-05 16:15:37.301501 findmyorder-1.7.5/README.md
--rw-r--r--   0        0        0      113 2023-08-05 16:15:47.497521 findmyorder-1.7.5/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/config.py
--rw-r--r--   0        0        0     3221 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5931 2023-08-05 16:15:37.305501 findmyorder-1.7.5/findmyorder/main.py
--rw-r--r--   0        0        0     2878 2023-08-05 16:15:47.489521 findmyorder-1.7.5/pyproject.toml
--rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 findmyorder-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 10:50:34.880305 findmyorder-1.7.6/LICENSE
+-rw-r--r--   0        0        0     2923 2023-08-06 10:50:34.880305 findmyorder-1.7.6/README.md
+-rw-r--r--   0        0        0      113 2023-08-06 10:50:38.940566 findmyorder-1.7.6/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-06 10:50:34.880305 findmyorder-1.7.6/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-08-06 10:50:34.880305 findmyorder-1.7.6/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5931 2023-08-06 10:50:34.880305 findmyorder-1.7.6/findmyorder/main.py
+-rw-r--r--   0        0        0     2878 2023-08-06 10:50:38.932565 findmyorder-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 findmyorder-1.7.6/PKG-INFO
```

### Comparing `findmyorder-1.7.5/LICENSE` & `findmyorder-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.5/README.md` & `findmyorder-1.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,11 @@
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 </code>
 </pre>
 
-<h5>Example</h5>
 
-https://github.com/mraniki/findmyorder/blob/6211e686abf1321ab3d5a8ac33068f854b0e9336/examples/example.py#L1-L90
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/findmyorder/en/latest/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
+
```

#### html2text {}

```diff
@@ -36,10 +36,10 @@
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000',
 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type':
 None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28,
 731282, tzinfo=datetime.timezone.utc)}
-** Example **
-https://github.com/mraniki/findmyorder/blob/
-6211e686abf1321ab3d5a8ac33068f854b0e9336/examples/example.py#L1-L90
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

### Comparing `findmyorder-1.7.5/findmyorder/config.py` & `findmyorder-1.7.6/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.5/findmyorder/default_settings.toml` & `findmyorder-1.7.6/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.5/findmyorder/main.py` & `findmyorder-1.7.6/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.7.5/pyproject.toml` & `findmyorder-1.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.7.5"
+version = "1.7.6"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
```

### Comparing `findmyorder-1.7.5/PKG-INFO` & `findmyorder-1.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.7.5
+Version: 1.7.6
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,11 +54,12 @@
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000', 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type': None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28, 731282, tzinfo=datetime.timezone.utc)}
 </code>
 </pre>
 
-<h5>Example</h5>
 
-https://github.com/mraniki/findmyorder/blob/6211e686abf1321ab3d5a8ac33068f854b0e9336/examples/example.py#L1-L90
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/findmyorder/en/latest/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.7.5 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.7.6 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist: loguru
@@ -49,10 +49,10 @@
          fmo = FindMyOrder()
          msg_order = "buy EURUSD sl=1000 tp=1000 q=1 comment=FOMC"
          order = await fmo.get_order(msg_order)
          #{'action': 'BUY', 'instrument': 'EURUSD', 'stop_loss': '1000',
 'take_profit': '1000', 'quantity': '2', 'order_type': None, 'leverage_type':
 None, 'comment': None, 'timestamp': datetime.datetime(2023, 5, 3, 12, 10, 28,
 731282, tzinfo=datetime.timezone.utc)}
-** Example **
-https://github.com/mraniki/findmyorder/blob/
-6211e686abf1321ab3d5a8ac33068f854b0e9336/examples/example.py#L1-L90
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

