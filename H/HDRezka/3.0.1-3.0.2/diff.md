# Comparing `tmp/HDRezka-3.0.1.tar.gz` & `tmp/HDRezka-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HDRezka-3.0.1.tar", last modified: Tue May  9 07:12:05 2023, max compression
+gzip compressed data, was "HDRezka-3.0.2.tar", last modified: Sat Aug  5 11:15:30 2023, max compression
```

## Comparing `HDRezka-3.0.1.tar` & `HDRezka-3.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.726275 HDRezka-3.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.663775 HDRezka-3.0.1/HDRezka.egg-info/
--rw-rw-rw-   0        0        0     4943 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 07:12:05.000000 HDRezka-3.0.1/HDRezka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-01 05:24:49.000000 HDRezka-3.0.1/LICENSE
--rw-rw-rw-   0        0        0     4943 2023-05-09 07:12:05.726275 HDRezka-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      986 2023-05-09 07:05:54.000000 HDRezka-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.695084 HDRezka-3.0.1/hdrezka/
--rw-rw-rw-   0        0        0     1079 2023-05-09 07:06:59.000000 HDRezka-3.0.1/hdrezka/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/_antiobfuscation.py
--rw-rw-rw-   0        0        0      309 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/_bs4.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.695084 HDRezka-3.0.1/hdrezka/api/
--rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/api/__init__.py
--rw-rw-rw-   0        0        0     1472 2023-05-08 09:52:32.000000 HDRezka-3.0.1/hdrezka/api/ajax.py
--rw-rw-rw-   0        0        0      370 2023-05-08 06:08:44.000000 HDRezka-3.0.1/hdrezka/api/http.py
--rw-rw-rw-   0        0        0      832 2023-05-08 10:49:50.000000 HDRezka-3.0.1/hdrezka/api/search.py
--rw-rw-rw-   0        0        0      383 2023-05-08 10:49:13.000000 HDRezka-3.0.1/hdrezka/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/
--rw-rw-rw-   0        0        0       42 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/__init__.py
--rw-rw-rw-   0        0        0      113 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/_dataclass.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/info/
--rw-rw-rw-   0        0        0       44 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/__init__.py
--rw-rw-rw-   0        0        0      622 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/fields.py
--rw-rw-rw-   0        0        0     5459 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/info/info.py
--rw-rw-rw-   0        0        0     2905 2023-05-08 10:49:40.000000 HDRezka-3.0.1/hdrezka/post/page.py
--rw-rw-rw-   0        0        0     2612 2023-05-09 07:04:56.000000 HDRezka-3.0.1/hdrezka/post/post.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/urls/
--rw-rw-rw-   0        0        0       64 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/__init__.py
--rw-rw-rw-   0        0        0      416 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/_regexes.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.710666 HDRezka-3.0.1/hdrezka/post/urls/kind/
--rw-rw-rw-   0        0        0       71 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/__init__.py
--rw-rw-rw-   0        0        0      768 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/quality.py
--rw-rw-rw-   0        0        0     1490 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/subtitle.py
--rw-rw-rw-   0        0        0     2037 2023-05-08 10:43:14.000000 HDRezka-3.0.1/hdrezka/post/urls/kind/video.py
--rw-rw-rw-   0        0        0      553 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/short.py
--rw-rw-rw-   0        0        0      469 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/post/urls/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:12:05.726275 HDRezka-3.0.1/hdrezka/stream/
--rw-rw-rw-   0        0        0       23 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/stream/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-05-09 07:05:54.000000 HDRezka-3.0.1/hdrezka/stream/player.py
--rw-rw-rw-   0        0        0      398 2023-05-08 06:05:54.000000 HDRezka-3.0.1/hdrezka/translators.py
--rw-rw-rw-   0        0        0       42 2023-05-09 07:12:05.726275 HDRezka-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2007 2023-05-09 07:11:46.000000 HDRezka-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.548702 HDRezka-3.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.518974 HDRezka-3.0.2/HDRezka.egg-info/
+-rw-rw-rw-   0        0        0     5167 2023-08-05 11:15:30.000000 HDRezka-3.0.2/HDRezka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-08-05 11:15:30.000000 HDRezka-3.0.2/HDRezka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:15:30.000000 HDRezka-3.0.2/HDRezka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-05 11:15:30.000000 HDRezka-3.0.2/HDRezka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 11:15:30.000000 HDRezka-3.0.2/HDRezka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-08-05 09:19:06.000000 HDRezka-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5167 2023-08-05 11:15:30.547700 HDRezka-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1018 2023-08-05 09:19:06.000000 HDRezka-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.525051 HDRezka-3.0.2/hdrezka/
+-rw-rw-rw-   0        0        0     1079 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-08-05 10:20:56.000000 HDRezka-3.0.2/hdrezka/_antiobfuscation.py
+-rw-rw-rw-   0        0        0      309 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/_bs4.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.529878 HDRezka-3.0.2/hdrezka/api/
+-rw-rw-rw-   0        0        0       44 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/api/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-08-05 10:30:24.000000 HDRezka-3.0.2/hdrezka/api/ajax.py
+-rw-rw-rw-   0        0        0      370 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/api/http.py
+-rw-rw-rw-   0        0        0      832 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/api/search.py
+-rw-rw-rw-   0        0        0      383 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/errors.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.533871 HDRezka-3.0.2/hdrezka/post/
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/_dataclass.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.536988 HDRezka-3.0.2/hdrezka/post/info/
+-rw-rw-rw-   0        0        0       44 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/info/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/info/fields.py
+-rw-rw-rw-   0        0        0     5459 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/info/info.py
+-rw-rw-rw-   0        0        0     2905 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/page.py
+-rw-rw-rw-   0        0        0     2612 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/post.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.540986 HDRezka-3.0.2/hdrezka/post/urls/
+-rw-rw-rw-   0        0        0       64 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/_regexes.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.544534 HDRezka-3.0.2/hdrezka/post/urls/kind/
+-rw-rw-rw-   0        0        0       71 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/kind/__init__.py
+-rw-rw-rw-   0        0        0      768 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/kind/quality.py
+-rw-rw-rw-   0        0        0     1490 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/kind/subtitle.py
+-rw-rw-rw-   0        0        0     2214 2023-08-05 11:05:39.000000 HDRezka-3.0.2/hdrezka/post/urls/kind/video.py
+-rw-rw-rw-   0        0        0      553 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/short.py
+-rw-rw-rw-   0        0        0      469 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/post/urls/urls.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:15:30.546696 HDRezka-3.0.2/hdrezka/stream/
+-rw-rw-rw-   0        0        0       23 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/stream/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/stream/player.py
+-rw-rw-rw-   0        0        0      398 2023-08-05 09:19:06.000000 HDRezka-3.0.2/hdrezka/translators.py
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:15:30.548702 HDRezka-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2065 2023-08-05 11:06:28.000000 HDRezka-3.0.2/setup.py
```

### Comparing `HDRezka-3.0.1/HDRezka.egg-info/PKG-INFO` & `HDRezka-3.0.2/HDRezka.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 3.0.1
+Version: 3.0.2
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -66,14 +66,20 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.2
+
+- ### post.urls.kind.VideoURLs
+  - `__init__(self, data: str | dict)` now raises `TypeError`
+    if `data` isn't of type `str | dict` (see [this issue](https://github.com/NIKDISSV-Forever/HDRezka/issues/1))
+
 ## 3.0.1
 
 - Now `__await__` method (need `await ...` expression) instead `ainit` method
 
 ## 3.0.0
 
 - **Now a fully asynchronous package.**
```

### Comparing `HDRezka-3.0.1/HDRezka.egg-info/SOURCES.txt` & `HDRezka-3.0.2/HDRezka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/LICENSE` & `HDRezka-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/PKG-INFO` & `HDRezka-3.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HDRezka
-Version: 3.0.1
+Version: 3.0.2
 Summary: HDRezka (rezka.ag) Python API
 Home-page: https://github.com/NIKDISSV-Forever/HDRezka
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/HDRezka
 Project-URL: Documentation, https://nikdissv-forever.github.io/HDRezka/hdrezka
@@ -66,14 +66,20 @@
 
 # [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
 
 ---
 
 # CHANGELOG
 
+## 3.0.2
+
+- ### post.urls.kind.VideoURLs
+  - `__init__(self, data: str | dict)` now raises `TypeError`
+    if `data` isn't of type `str | dict` (see [this issue](https://github.com/NIKDISSV-Forever/HDRezka/issues/1))
+
 ## 3.0.1
 
 - Now `__await__` method (need `await ...` expression) instead `ainit` method
 
 ## 3.0.0
 
 - **Now a fully asynchronous package.**
```

### Comparing `HDRezka-3.0.1/README.md` & `HDRezka-3.0.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# [HDRezka](https://rezka.ag/) site API.
-
-# Install
-
-`pip install HDRezka`
-
-# Example
-
-```python
-import asyncio
-from hdrezka import Search
-
-async def main():
-    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use await Player(646)
-    print(player.post.info, end='\n\n')
-
-    translator_id = None  # default
-    for name, id_ in player.post.translators.name_id.items():
-        if 'субтитры' in name.casefold(): translator_id = id_; break
-
-    stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
-    video = stream.video
-    print(video.last_url)  # best quality (.m3u8)
-    print(video[video.min].last_url.mp4, end='\n\n')  # worst quality (.mp4)
-
-    subtitles = stream.subtitles
-    print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
-
-if __name__ == '__main__': asyncio.run(main())
-```
-
-# [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
+# [HDRezka](https://rezka.ag/) site API.
+
+# Install
+
+`pip install HDRezka`
+
+# Example
+
+```python
+import asyncio
+from hdrezka import Search
+
+async def main():
+    player = await (await Search('Breaking Bad').get_page(1))[0].player  # or just use await Player(646)
+    print(player.post.info, end='\n\n')
+
+    translator_id = None  # default
+    for name, id_ in player.post.translators.name_id.items():
+        if 'субтитры' in name.casefold(): translator_id = id_; break
+
+    stream = await player.get_stream(1, 1, translator_id)  # raise AJAXFail if invalid episode or translator
+    video = stream.video
+    print(video.last_url)  # best quality (.m3u8)
+    print(video[video.min].last_url.mp4, end='\n\n')  # worst quality (.mp4)
+
+    subtitles = stream.subtitles
+    print(subtitles.default.url)  # subtitles.ru.url or subtitles['Русский'].url
+
+if __name__ == '__main__': asyncio.run(main())
+```
+
+# [Documentation](https://nikdissv-forever.github.io/HDRezka/hdrezka)
```

### Comparing `HDRezka-3.0.1/hdrezka/__init__.py` & `HDRezka-3.0.2/hdrezka/__init__.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/_antiobfuscation.py` & `HDRezka-3.0.2/hdrezka/_antiobfuscation.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     '|JCFA|JCFe|JCM=|JCMh|JCMj|JCMk|JCNA|JCNe|JCQ=|JCQh|JCQj|JCQk|JCRA|JCRe|JEA=|JEAh|JEAj|JEAk|JEBA|JEBe|JF4=|JF4h'
     '|JF4j|JF4k|JF5A|JF5e|QCE=|QCEh|QCEj|QCEk|QCFA|QCFe|QCM=|QCMh|QCMj|QCMk|QCNA|QCNe|QCQ=|QCQh|QCQj|QCQk|QCRA|QCRe'
     '|QEA=|QEAh|QEAj|QEAk|QEBA|QEBe|QF4=|QF4h|QF4j|QF4k|QF5A|QF5e|XiE=|XiEh|XiEj|XiEk|XiFA|XiFe|XiM=|XiMh|XiMj|XiMk'
     '|XiNA|XiNe|XiQ=|XiQh|XiQj|XiQk|XiRA|XiRe|XkA=|XkAh|XkAj|XkAk|XkBA|XkBe|Xl4=|Xl4h|Xl4j|Xl4k|Xl5A|Xl5e').sub
 
 
 def clear_trash(trash_string: str) -> str:
-    return a2b_base64(b'%b==' % _sub_trash('', trash_string).encode('ASCII')).decode('ASCII')
+    return a2b_base64(_sub_trash('', trash_string).encode('ASCII') + b'==').decode('ASCII')
```

### Comparing `HDRezka-3.0.1/hdrezka/api/ajax.py` & `HDRezka-3.0.2/hdrezka/api/ajax.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     async def get_episodes(cls, id: AnyID, translator_id: AnyID):
         return await cls.get_cdn_series(
             {'action': 'get_episodes',
              'id': id,
              'translator_id': translator_id})
 
     @classmethod
-    async def get_stream(cls, id: AnyID, translator_id: AnyID, season: AnyID, episode: AnyID):
+    async def get_stream(cls, id: AnyID, translator_id: AnyID, season: AnyID, episode: AnyID) -> dict[str]:
         return await cls.get_cdn_series(
             {'action': 'get_stream',
              'id': id,
              'translator_id': translator_id,
              'season': season,
              'episode': episode}
         )
```

### Comparing `HDRezka-3.0.1/hdrezka/api/search.py` & `HDRezka-3.0.2/hdrezka/api/search.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/info/fields.py` & `HDRezka-3.0.2/hdrezka/post/info/fields.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/info/info.py` & `HDRezka-3.0.2/hdrezka/post/info/info.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/page.py` & `HDRezka-3.0.2/hdrezka/post/page.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/post.py` & `HDRezka-3.0.2/hdrezka/post/post.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/urls/kind/quality.py` & `HDRezka-3.0.2/hdrezka/post/urls/kind/quality.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/urls/kind/subtitle.py` & `HDRezka-3.0.2/hdrezka/post/urls/kind/subtitle.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/post/urls/kind/video.py` & `HDRezka-3.0.2/hdrezka/post/urls/kind/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,21 @@
         self.mp4 = str(self.removesuffix('8').removesuffix(':hls:manifest.m3u'))
 
 
 class VideoURLs:
     __slots__ = ('raw_data', 'qualities', 'min')
 
     def __init__(self, data: str | dict):
-        self.raw_data: dict[Quality, VideoURL] = (
-            {Quality(q): VideoURL(u) for q, u in findall_qualities(clear_trash(data))}
-            if isinstance(data, str) else data)
+        if isinstance(data, str):
+            self.raw_data: dict[Quality, VideoURL] = {
+                Quality(q): VideoURL(u) for q, u in findall_qualities(clear_trash(data))}
+        elif isinstance(data, dict):
+            self.raw_data = data
+        else:
+            raise TypeError(f'got {data!r} (type {type(data)}) but expected type {str | dict}')
         self.qualities: tuple[Quality] = *sorted(self.raw_data),
         self.min = int(self.qualities[0]) if self.qualities else 1
 
     @property
     def last_url(self) -> VideoURL:
         return self[-1].raw_data.popitem()[1]
```

### Comparing `HDRezka-3.0.1/hdrezka/post/urls/short.py` & `HDRezka-3.0.2/hdrezka/post/urls/short.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/hdrezka/stream/player.py` & `HDRezka-3.0.2/hdrezka/stream/player.py`

 * *Files identical despite different names*

### Comparing `HDRezka-3.0.1/setup.py` & `HDRezka-3.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from __future__ import annotations
-
-import setuptools
-
-with open('requirements.txt', encoding='UTF-8') as f:
-    install_requires = f.read().strip().splitlines()
-with open('README.md', encoding='UTF-8') as f:
-    long_description = f.read().strip()
-with open('CHANGELOG.md', encoding='UTF-8') as f:
-    long_description += f'\n\n---\n\n{f.read().strip()}\n'
-
-setuptools.setup(
-    name='HDRezka',
-    version='3.0.1',
-
-    author='Nikita (NIKDISSV)',
-    author_email='nikdissv@proton.me',
-
-    description='HDRezka (rezka.ag) Python API',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-
-    url='https://github.com/NIKDISSV-Forever/HDRezka',
-    project_urls={
-        'GitHub': 'https://github.com/NIKDISSV-Forever/HDRezka',
-        'Documentation': 'https://nikdissv-forever.github.io/HDRezka/hdrezka'
-    },
-    packages=setuptools.find_packages(),
-    install_requires=install_requires,
-
-    license='MIT',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Intended Audience :: End Users/Desktop',
-        'Intended Audience :: Information Technology',
-        'Intended Audience :: Other Audience',
-        'Intended Audience :: Telecommunications Industry',
-        'License :: OSI Approved',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Internet',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
-        'Topic :: Multimedia :: Video',
-
-    ],
-
-    python_requires='>=3.10',
-    keywords=['HDRezka', 'rezka.ag', 'watch online', 'api', 'stream']
-)
+from __future__ import annotations
+
+import setuptools
+
+with open('requirements.txt', encoding='UTF-8') as f:
+    install_requires = f.read().strip().splitlines()
+with open('README.md', encoding='UTF-8') as f:
+    long_description = f.read().strip()
+with open('CHANGELOG.md', encoding='UTF-8') as f:
+    long_description += f'\n\n---\n\n{f.read().strip()}\n'
+
+setuptools.setup(
+    name='HDRezka',
+    version='3.0.2',
+
+    author='Nikita (NIKDISSV)',
+    author_email='nikdissv@proton.me',
+
+    description='HDRezka (rezka.ag) Python API',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+
+    url='https://github.com/NIKDISSV-Forever/HDRezka',
+    project_urls={
+        'GitHub': 'https://github.com/NIKDISSV-Forever/HDRezka',
+        'Documentation': 'https://nikdissv-forever.github.io/HDRezka/hdrezka'
+    },
+    packages=setuptools.find_packages(),
+    install_requires=install_requires,
+
+    license='MIT',
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Environment :: Console',
+        'Intended Audience :: End Users/Desktop',
+        'Intended Audience :: Information Technology',
+        'Intended Audience :: Other Audience',
+        'Intended Audience :: Telecommunications Industry',
+        'License :: OSI Approved',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Internet',
+        'Topic :: Internet :: WWW/HTTP',
+        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+        'Topic :: Multimedia :: Video',
+
+    ],
+
+    python_requires='>=3.10',
+    keywords=['HDRezka', 'rezka.ag', 'watch online', 'api', 'stream']
+)
```

