# Comparing `tmp/iamlistening-3.1.1.tar.gz` & `tmp/iamlistening-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.1.1.tar", max compression
+gzip compressed data, was "iamlistening-3.1.2.tar", max compression
```

## Comparing `iamlistening-3.1.1.tar` & `iamlistening-3.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-08-04 18:57:41.265846 iamlistening-3.1.1/LICENSE
--rw-r--r--   0        0        0     2769 2023-08-04 18:57:41.265846 iamlistening-3.1.1/README.md
--rw-r--r--   0        0        0       81 2023-08-04 18:57:45.505896 iamlistening-3.1.1/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3275 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0        0 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      672 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-04 18:57:41.265846 iamlistening-3.1.1/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0     3221 2023-08-04 18:57:45.497896 iamlistening-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 iamlistening-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 10:02:03.454791 iamlistening-3.1.2/LICENSE
+-rw-r--r--   0        0        0     2533 2023-08-06 10:02:03.454791 iamlistening-3.1.2/README.md
+-rw-r--r--   0        0        0       81 2023-08-06 10:02:05.390811 iamlistening-3.1.2/iamlistening/__init__.py
+-rw-r--r--   0        0        0      688 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/config.py
+-rw-r--r--   0        0        0     1376 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3275 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      672 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      912 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-06 10:02:03.454791 iamlistening-3.1.2/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0     3221 2023-08-06 10:02:05.382811 iamlistening-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 iamlistening-3.1.2/PKG-INFO
```

### Comparing `iamlistening-3.1.1/LICENSE` & `iamlistening-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/README.md` & `iamlistening-3.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a> <a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
@@ -26,18 +26,17 @@
      
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
-      from iamlistening import Listener
-      listener = Listener()
-      await listener.start()
-      while True:
-          msg = await listener.handler.get_latest_message()
-          if msg:
+    listener = Listener()
+    await listener.start()
+    while listener.handler.connected:
+        msg = await listener.handler.get_latest_message()
+        if msg:
             logger.info(f"Frasier👂: {msg}")
 
 </code>
 </pre>
```

#### html2text {}

```diff
@@ -1,18 +1,16 @@
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
-[https://img.shields.io/badge/github-
-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [Docker_Pulls]
-[https://img.shields.io/badge/tips-000000?style=for-the-             [Logo]
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
+the-badge&logo=wikipedia&logoColor=white] [https://
+img.shields.io/badge/github-%23000000.svg?style=for-the-
+badge&logo=github&logoColor=white] [https://img.shields.io/
+badge/tips-000000?style=for-the-                                     [Logo]
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/mraniki/tt?style=for-
+the-badge] [https://img.shields.io/badge/talky-
+blue?style=for-the-badge&logo=telegram&logoColor=white]
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
@@ -20,15 +18,14 @@
 ?version=latest&style=for-the-badge]                        guilded, mastodon,
 [https://codebeat.co/badges/4085334e-4590-41f6-a70c-        lemmy.
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
-      from iamlistening import Listener
-      listener = Listener()
-      await listener.start()
-      while True:
-          msg = await listener.handler.get_latest_message()
-          if msg:
+    listener = Listener()
+    await listener.start()
+    while listener.handler.connected:
+        msg = await listener.handler.get_latest_message()
+        if msg:
             logger.info(f"Frasierð: {msg}")
```

### Comparing `iamlistening-3.1.1/iamlistening/config.py` & `iamlistening-3.1.2/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/default_settings.toml` & `iamlistening-3.1.2/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/main.py` & `iamlistening-3.1.2/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/chat_manager.py` & `iamlistening-3.1.2/iamlistening/platform/chat_manager.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/discord.py` & `iamlistening-3.1.2/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/guilded.py` & `iamlistening-3.1.2/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/lemmy.py` & `iamlistening-3.1.2/iamlistening/platform/clients/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.1.2/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/matrix.py` & `iamlistening-3.1.2/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/revolt.py` & `iamlistening-3.1.2/iamlistening/platform/clients/revolt.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.1.2/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/telegram.py` & `iamlistening-3.1.2/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/iamlistening/platform/clients/tinode.py` & `iamlistening-3.1.2/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.1.1/pyproject.toml` & `iamlistening-3.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.1.1"
+version = "3.1.2"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
```

### Comparing `iamlistening-3.1.1/PKG-INFO` & `iamlistening-3.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.1.1
+Version: 3.1.2
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,19 +27,19 @@
 Project-URL: Support, https://github.com/mraniki/iamlistening/discussions
 Description-Content-Type: text/markdown
 
 
 <table style="border: 1px solid transparent">
   <tr>
     <td>
-<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a><br>
-<a href="https://github.com/mraniki/iamlistening/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
-<a href="https://hub.docker.com/r/mraniki/tt"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a><br>
-<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a>
-<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a> <a href="https://discord.gg/gMNERs5M9"><img src="https://img.shields.io/discord/1049307055867035648?style=for-the-badge&logo=discord&logoColor=white&label=%20%20&color=blue"></a>
+<a href="https://talkytrader.github.io/wiki/"><img src="https://img.shields.io/badge/Wiki-%23000000.svg?style=for-the-badge&logo=wikipedia&logoColor=white"></a>
+<a href="https://github.com/mraniki/tt/"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"></a>
+<a href="https://coindrop.to/mraniki"><img src="https://img.shields.io/badge/tips-000000?style=for-the-badge&logo=buymeacoffee&logoColor=white"></a><br>
+<a href="https://hub.docker.com/r/mraniki/tt"><img src="https://img.shields.io/docker/pulls/mraniki/tt?style=for-the-badge"></a>
+<a href="https://t.me/TTTalkyTraderChat/1"><img src="https://img.shields.io/badge/talky-blue?style=for-the-badge&logo=telegram&logoColor=white"></a><br>
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/242846519-f76331f6-8821-49eb-8f1c-06aedd8557be.jpeg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/v/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/iamlistening/"><img src="https://img.shields.io/pypi/dm/iamlistening?style=for-the-badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey"></a><br>
@@ -55,19 +55,18 @@
      
   </tr>
 </table>
 
 <h5>How to use it</h5>
 <pre>
 <code>
-      from iamlistening import Listener
-      listener = Listener()
-      await listener.start()
-      while True:
-          msg = await listener.handler.get_latest_message()
-          if msg:
+    listener = Listener()
+    await listener.start()
+    while listener.handler.connected:
+        msg = await listener.handler.get_latest_message()
+        if msg:
             logger.info(f"Frasier👂: {msg}")
 
 </code>
 </pre>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.1.1 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.1.2 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
@@ -12,24 +12,22 @@
 (>=1.30.0,<2.0.0) Requires-Dist: simplematrixbotlib (>=2.9.0,<3.0.0) Requires-
 Dist: telethon (>=1.28.5,<2.0.0) Requires-Dist: tinode_grpc (>=0.22.3,<0.23.0)
 Project-URL: Changelog, https://github.com/mraniki/iamlistening/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/iamlistening/
 issues Project-URL: Support, https://github.com/mraniki/iamlistening/
 discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
-the-badge&logo=wikipedia&logoColor=white]
-[https://img.shields.io/badge/github-
-%23000000.svg?style=for-the-
-badge&logo=github&logoColor=white] [Docker_Pulls]
-[https://img.shields.io/badge/tips-000000?style=for-the-             [Logo]
-badge&logo=buymeacoffee&logoColor=white] [https://
-img.shields.io/badge/talky-blue?style=for-the-
-badge&logo=telegram&logoColor=white] [https://
-img.shields.io/discord/1049307055867035648?style=for-the-
-badge&logo=discord&logoColor=white&label=%20%20&color=blue]
+the-badge&logo=wikipedia&logoColor=white] [https://
+img.shields.io/badge/github-%23000000.svg?style=for-the-
+badge&logo=github&logoColor=white] [https://img.shields.io/
+badge/tips-000000?style=for-the-                                     [Logo]
+badge&logo=buymeacoffee&logoColor=white]
+[https://img.shields.io/docker/pulls/mraniki/tt?style=for-
+the-badge] [https://img.shields.io/badge/talky-
+blue?style=for-the-badge&logo=telegram&logoColor=white]
 [https://img.shields.io/pypi/v/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/iamlistening?style=for-the-
 badge&logo=PyPI&logoColor=white&label=pypi&labelColor=grey] A python package to
 [https://img.shields.io/github/actions/workflow/status/     listen to messaging
 mraniki/iamlistening/%F0%9F%91%B7Flow.yml?style=for-the-    platforms,
 badge&logo=GitHub&logoColor=white]                          such as discord,
@@ -37,15 +35,14 @@
 ?version=latest&style=for-the-badge]                        guilded, mastodon,
 [https://codebeat.co/badges/4085334e-4590-41f6-a70c-        lemmy.
 69e9a2641c79]
 [https://codecov.io/gh/mraniki/iamlistening/branch/main/
 graph/badge.svg?token=QZ55U6KQFN]
 ** How to use it **
 
-      from iamlistening import Listener
-      listener = Listener()
-      await listener.start()
-      while True:
-          msg = await listener.handler.get_latest_message()
-          if msg:
+    listener = Listener()
+    await listener.start()
+    while listener.handler.connected:
+        msg = await listener.handler.get_latest_message()
+        if msg:
             logger.info(f"Frasierð: {msg}")
```

