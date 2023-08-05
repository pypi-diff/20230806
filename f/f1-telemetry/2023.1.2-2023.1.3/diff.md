# Comparing `tmp/f1_telemetry-2023.1.2.tar.gz` & `tmp/f1_telemetry-2023.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1_telemetry-2023.1.2.tar", max compression
+gzip compressed data, was "f1_telemetry-2023.1.3.tar", max compression
```

## Comparing `f1_telemetry-2023.1.2.tar` & `f1_telemetry-2023.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1791 2023-07-14 17:44:45.006978 f1_telemetry-2023.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/__init__.py
--rw-r--r--   0        0        0     2307 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/__main__.py
--rw-r--r--   0        0        0    16287 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/collector.py
--rw-r--r--   0        0        0     1155 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/live.py
--rw-r--r--   0        0        0     6097 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/model.py
--rw-r--r--   0        0        0     2883 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/report.py
--rw-r--r--   0        0        0      467 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/server.py
--rw-r--r--   0        0        0     1393 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/storage.py
--rw-r--r--   0        0        0     2742 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/view.py
--rw-r--r--   0        0        0    73384 2023-07-14 17:44:45.026978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/Formula1-Regular.ttf
--rw-r--r--   0        0        0   203029 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/bg.jpg
--rw-r--r--   0        0        0    33104 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/art/car.svg
--rw-r--r--   0        0        0     5266 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/index.html
--rw-r--r--   0        0        0    35177 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/live.html
--rw-r--r--   0        0        0     6497 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/live.js
--rw-r--r--   0        0        0     9991 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/plots.js
--rw-r--r--   0        0        0     4647 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/queries.js
--rw-r--r--   0        0        0     1321 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/style.css
--rw-r--r--   0        0        0     3189 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/trace.js
--rw-r--r--   0        0        0      787 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/utils.js
--rw-r--r--   0        0        0     6089 2023-07-14 17:44:45.030978 f1_telemetry-2023.1.2/f1_telemetry/webapp/view.js
--rw-r--r--   0        0        0     1078 2023-07-14 17:44:56.462948 f1_telemetry-2023.1.2/pyproject.toml
--rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 f1_telemetry-2023.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1791 2023-08-05 22:28:42.967756 f1_telemetry-2023.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/__init__.py
+-rw-r--r--   0        0        0     2634 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/__main__.py
+-rw-r--r--   0        0        0    16287 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/collector.py
+-rw-r--r--   0        0        0     1155 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/live.py
+-rw-r--r--   0        0        0     6097 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/model.py
+-rw-r--r--   0        0        0     2883 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/report.py
+-rw-r--r--   0        0        0      467 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/server.py
+-rw-r--r--   0        0        0     1393 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/storage.py
+-rw-r--r--   0        0        0     2742 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/view.py
+-rw-r--r--   0        0        0    73384 2023-08-05 22:28:42.987756 f1_telemetry-2023.1.3/f1_telemetry/webapp/art/Formula1-Regular.ttf
+-rw-r--r--   0        0        0   203029 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/art/bg.jpg
+-rw-r--r--   0        0        0    33104 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/art/car.svg
+-rw-r--r--   0        0        0     5266 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/index.html
+-rw-r--r--   0        0        0    35177 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/live.html
+-rw-r--r--   0        0        0     6497 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/live.js
+-rw-r--r--   0        0        0     9991 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/plots.js
+-rw-r--r--   0        0        0     4647 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/queries.js
+-rw-r--r--   0        0        0     1321 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/style.css
+-rw-r--r--   0        0        0     3189 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/trace.js
+-rw-r--r--   0        0        0      787 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/utils.js
+-rw-r--r--   0        0        0     6089 2023-08-05 22:28:42.991757 f1_telemetry-2023.1.3/f1_telemetry/webapp/view.js
+-rw-r--r--   0        0        0     1078 2023-08-05 22:28:58.939757 f1_telemetry-2023.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 f1_telemetry-2023.1.3/PKG-INFO
```

### Comparing `f1_telemetry-2023.1.2/README.md` & `f1_telemetry-2023.1.3/README.md`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/__main__.py` & `f1_telemetry-2023.1.3/f1_telemetry/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,28 @@
         "-b",
         "--bucket",
         help="InfluxDB Bucket",
         type=str,
         default=DEFAULT_BUCKET,
     )
     argp.add_argument(
+        "-a",
+        "--address",
+        help="F1 game telemetry address",
+        type=str,
+        default="localhost",
+    )
+    argp.add_argument(
+        "-p",
+        "--port",
+        help="F1 game telemetry port",
+        type=int,
+        default=20777,
+    )
+    argp.add_argument(
         "-H",
         "--host",
         help="Server host address",
         type=str,
         default="localhost",
     )
     argp.add_argument(
@@ -56,15 +70,15 @@
             if not sink.connected:
                 print(
                     "WARNING: InfluxDB not available. Telemetry data will not be stored."
                 )
             else:
                 print("Connected to InfluxDB")
 
-            listener = PacketListener()
+            listener = PacketListener(host=args.address, port=args.port)
             collector = TelemetryCollector(listener, sink, args.report)
 
             server_thread = Thread(target=serve, args=(args.org, args.token, args.host))
             server_thread.daemon = True
             server_thread.start()
 
             print("Listening for telemetry data ...")
```

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/collector.py` & `f1_telemetry-2023.1.3/f1_telemetry/collector.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/live.py` & `f1_telemetry-2023.1.3/f1_telemetry/live.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/model.py` & `f1_telemetry-2023.1.3/f1_telemetry/model.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/report.py` & `f1_telemetry-2023.1.3/f1_telemetry/report.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/storage.py` & `f1_telemetry-2023.1.3/f1_telemetry/storage.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/view.py` & `f1_telemetry-2023.1.3/f1_telemetry/view.py`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/Formula1-Regular.ttf` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/art/Formula1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/bg.jpg` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/art/bg.jpg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/art/car.svg` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/art/car.svg`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/index.html` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/index.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/live.html` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/live.html`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/live.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/live.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/plots.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/plots.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/queries.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/queries.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/style.css` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/style.css`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/trace.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/trace.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/utils.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/utils.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/f1_telemetry/webapp/view.js` & `f1_telemetry-2023.1.3/f1_telemetry/webapp/view.js`

 * *Files identical despite different names*

### Comparing `f1_telemetry-2023.1.2/pyproject.toml` & `f1_telemetry-2023.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = ["Gabriele N. Tornetta <phoenix1987@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "f1_telemetry"},
 ]
 readme = "README.md"
 repository = "https://github.com/P403n1x87/f1-telemetry"
-version = "2023.1.2"
+version = "2023.1.3"
 
 [tool.isort]
 force_single_line = true
 lines_after_imports = 2
 profile = "black"
 
 [tool.poetry.dependencies]
```

### Comparing `f1_telemetry-2023.1.2/PKG-INFO` & `f1_telemetry-2023.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f1-telemetry
-Version: 2023.1.2
+Version: 2023.1.3
 Summary: F1 telemetry data collection and visualisation
 Home-page: https://github.com/P403n1x87/f1-telemetry
 License: MIT
 Author: Gabriele N. Tornetta
 Author-email: phoenix1987@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

