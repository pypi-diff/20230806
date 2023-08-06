# Comparing `tmp/mikan_card_downloader-1.1.2.tar.gz` & `tmp/mikan_card_downloader-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.1.2.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.2.0.tar", max compression
```

## Comparing `mikan_card_downloader-1.1.2.tar` & `mikan_card_downloader-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.2/LICENSE
--rw-r--r--   0        0        0     1041 2023-05-31 16:51:08.786603 mikan_card_downloader-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.2/src/mikan/__init__.py
--rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/classes.py
--rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/config.py
--rw-r--r--   0        0        0     3294 2023-05-31 10:39:28.598760 mikan_card_downloader-1.1.2/src/mikan/downloader.py
--rw-r--r--   0        0        0     5673 2023-05-31 10:47:12.451838 mikan_card_downloader-1.1.2/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.2/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.2/src/mikan/py.typed
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1041 2023-08-06 21:29:30.042111 mikan_card_downloader-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.0/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.2.0/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-07-26 18:37:20.320555 mikan_card_downloader-1.2.0/src/mikan/config.py
+-rw-r--r--   0        0        0     3360 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.0/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5673 2023-05-31 10:47:12.451838 mikan_card_downloader-1.2.0/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.2.0/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2402 2023-08-06 21:27:00.227335 mikan_card_downloader-1.2.0/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.2.0/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.2.0/PKG-INFO
```

### Comparing `mikan_card_downloader-1.1.2/LICENSE` & `mikan_card_downloader-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.2/pyproject.toml` & `mikan_card_downloader-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.1.2"
+version = "1.2.0"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.1.2/src/mikan/classes.py` & `mikan_card_downloader-1.2.0/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.2/src/mikan/config.py` & `mikan_card_downloader-1.2.0/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.2/src/mikan/downloader.py` & `mikan_card_downloader-1.2.0/src/mikan/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,20 @@
     async def __aexit__(self, ext_type: None, value: None, trace: None) -> None:
         await self.session.close()
 
     async def download_file(self, item: str) -> None:
         try:
             res = await self.session.get(f"https:{item}")
             if res.status == 200:
-                res_data = await res.read()
+                # res_data = await res.read()
                 self.path.mkdir(exist_ok=True, parents=True)
 
                 with open(self.path / self.get_card_image_name(item), "wb") as file:
-                    file.write(res_data)
+                    async for chunk in res.content.iter_any():
+                        file.write(chunk)
 
                 message = f"Downloaded item {self.get_card_image_name(item)}."
 
         except aiohttp.ClientError as e:
             message = f"Couldn't download item {item}: {e}"
 
         tqdm.write(message)
```

### Comparing `mikan_card_downloader-1.1.2/src/mikan/html_parser.py` & `mikan_card_downloader-1.2.0/src/mikan/html_parser.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.2/src/mikan/json_utils.py` & `mikan_card_downloader-1.2.0/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.2/src/mikan/main.py` & `mikan_card_downloader-1.2.0/src/mikan/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 import platformdirs
 
 from mikan import config
 from mikan.classes import Card, Item, SIF2Card, SIFCard, Still
 from mikan.downloader import Downloader
 
+MIKAN_PATH = Path(platformdirs.user_config_dir("mikan", ensure_exists=True))
+
 
 class UnrecognizedArgumentException(Exception):
     pass
 
 
 class InvalidPathException(Exception):
     pass
 
 
-async def run(
-    path: Path = Path(platformdirs.user_config_dir("mikan", ensure_exists=True))
-) -> None:
+async def run(path: Path = MIKAN_PATH) -> None:
     img_type: Type[Card | Still | SIFCard | SIF2Card] = Card
     if len(sys.argv) > 1:
         if sys.argv[1] == "--stills":
             img_type = Still
         elif sys.argv[1] == "--sif":
             img_type = SIFCard
         elif sys.argv[1] == "--sif2":
```

### Comparing `mikan_card_downloader-1.1.2/PKG-INFO` & `mikan_card_downloader-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.1.2
+Version: 1.2.0
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

