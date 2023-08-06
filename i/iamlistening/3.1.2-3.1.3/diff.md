# Comparing `tmp/iamlistening-3.1.2.tar.gz` & `tmp/iamlistening-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.1.2.tar", max compression
+gzip compressed data, was "iamlistening-3.1.3.tar", max compression
```

## Comparing `iamlistening-3.1.2.tar` & `iamlistening-3.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-08-06 10:02:03.454791 iamlistening-3.1.2/LICENSE
--rw-r--r--   0        0        0     2533 2023-08-06 10:02:03.454791 iamlistening-3.1.2/README.md
--rw-r--r--   0        0        0       81 2023-08-06 10:02:05.390811 iamlistening-3.1.2/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3275 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0        0 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      672 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0     3221 2023-08-06 10:02:05.382811 iamlistening-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 iamlistening-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 10:08:04.114823 iamlistening-3.1.3/LICENSE
+-rw-r--r--   0        0        0     2755 2023-08-06 10:08:04.114823 iamlistening-3.1.3/README.md
+-rw-r--r--   0        0        0       81 2023-08-06 10:08:05.514822 iamlistening-3.1.3/iamlistening/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3275 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      672 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-06 10:08:04.114823 iamlistening-3.1.3/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3221 2023-08-06 10:08:05.510822 iamlistening-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4005 1970-01-01 00:00:00.000000 iamlistening-3.1.3/PKG-INFO
```

### Comparing `iamlistening-3.1.2/LICENSE` & `iamlistening-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/README.md` & `iamlistening-3.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,7 +36,13 @@
         msg = await listener.handler.get_latest_message()
         if msg:
             logger.info(f"Frasier👂: {msg}")
 
 </code>
 </pre>
 
+
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/iamlistening/en/latest/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
+
+
+
```

#### html2text {}

```diff
@@ -25,7 +25,10 @@
     listener = Listener()
     await listener.start()
     while listener.handler.connected:
         msg = await listener.handler.get_latest_message()
         if msg:
             logger.info(f"Frasierð: {msg}")
 
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

### Comparing `iamlistening-3.1.2/iamlistening/config.py` & `iamlistening-3.1.3/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/default_settings.toml` & `iamlistening-3.1.3/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/main.py` & `iamlistening-3.1.3/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/chat_manager.py` & `iamlistening-3.1.3/iamlistening/platform/chat_manager.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/discord.py` & `iamlistening-3.1.3/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/guilded.py` & `iamlistening-3.1.3/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/lemmy.py` & `iamlistening-3.1.3/iamlistening/platform/clients/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.1.3/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/matrix.py` & `iamlistening-3.1.3/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/revolt.py` & `iamlistening-3.1.3/iamlistening/platform/clients/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.1.3/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/telegram.py` & `iamlistening-3.1.3/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/iamlistening/platform/clients/tinode.py` & `iamlistening-3.1.3/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.2/pyproject.toml` & `iamlistening-3.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.1.2"
+version = "3.1.3"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
```

### Comparing `iamlistening-3.1.2/PKG-INFO` & `iamlistening-3.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.1.2
+Version: 3.1.3
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -66,7 +66,13 @@
         if msg:
             logger.info(f"Frasier👂: {msg}")
 
 </code>
 </pre>
 
 
+<h5>Documentation</h5>
+<a href="https://talky.readthedocs.io/projects/iamlistening/en/latest/"><img src="https://img.shields.io/badge/Documentation-000000?style=for-the-badge&logo=readthedocs&logoColor=white"></a><br>
+
+
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.1.2 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.1.3 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
@@ -42,7 +42,10 @@
     listener = Listener()
     await listener.start()
     while listener.handler.connected:
         msg = await listener.handler.get_latest_message()
         if msg:
             logger.info(f"Frasierð: {msg}")
 
+** Documentation **
+[https://img.shields.io/badge/Documentation-000000?style=for-the-
+badge&logo=readthedocs&logoColor=white]
```

