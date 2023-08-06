# Comparing `tmp/playht-0.0.2-py3-none-any.whl.zip` & `tmp/playht-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1898 bytes, number of entries: 7
+Zip file size: 2433 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       28 b- defN 23-Aug-06 17:48 playht/__init__.py
--rw-r--r--  2.0 unx      277 b- defN 23-Aug-06 18:13 playht/__version__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Aug-06 17:48 playht/playht.py
--rw-r--r--  2.0 unx      595 b- defN 23-Aug-06 18:17 playht-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 18:17 playht-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-06 18:17 playht-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      514 b- defN 23-Aug-06 18:17 playht-0.0.2.dist-info/RECORD
-7 files, 1620 bytes uncompressed, 986 bytes compressed:  39.1%
+-rw-r--r--  2.0 unx      277 b- defN 23-Aug-06 18:48 playht/__version__.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Aug-06 18:46 playht/playht.py
+-rw-r--r--  2.0 unx      595 b- defN 23-Aug-06 18:48 playht-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 18:48 playht-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-06 18:48 playht-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      515 b- defN 23-Aug-06 18:48 playht-0.0.3.dist-info/RECORD
+7 files, 3068 bytes uncompressed, 1521 bytes compressed:  50.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: playht/__version__.py
 Comment: 
 
 Filename: playht/playht.py
 Comment: 
 
-Filename: playht-0.0.2.dist-info/METADATA
+Filename: playht-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: playht-0.0.2.dist-info/WHEEL
+Filename: playht-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: playht-0.0.2.dist-info/top_level.txt
+Filename: playht-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: playht-0.0.2.dist-info/RECORD
+Filename: playht-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## playht/__version__.py

```diff
@@ -6,13 +6,13 @@
 # rhcproc@gmail.com
 #
 # License: MIT
 #
 
 __title__ = 'playht'
 __license__ = 'MIT'
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 __author__ = 'Hans Park'
 __contact__ = 'rhcproc@gmail.com'
 __url__ = 'https://github.com/rhcproc/playht'
 __description__ = (
     '')
```

## playht/playht.py

```diff
@@ -1,7 +1,48 @@
 
+import requests
+import re
+
+
 class PlayHT:
-    def __init__(self):
-        self._ht = {}
+    def __init__(self, user_id, secret_key):
+        self.user_id = user_id
+        self.secret_key = secret_key
+        self.headers = {
+            'AUTHORIZATION': f'Bearer {self.secret_key}',
+            'X-USER-ID': self.user_id,
+            'accept': 'text/event-stream',
+            'content-type': 'application/json'
+        }
+
+    def get_mp3_url(self, text, voice):
+        response = requests.post("https://play.ht/api/v2/tts",
+                                 headers=self.headers,
+                                 json={
+                                        "text": text,
+                                        "voice": voice
+                                 },
+                                 stream=True)
+        chunk_list = []
+        if response.status_code == 200:
+            for chunk in response.iter_content(chunk_size=3):
+                if chunk:
+                    chunk_list.append(chunk.decode('utf-8'))
+
+        chunk_data = ''.join(chunk_list)
+        url = re.findall(r'"url":"(.*?)"', chunk_data)
+        if len(url) > 0:
+            return url[0]
+        else:
+            return None
+
+    def download_mp3(self, url, filename):
+        doc = requests.get(url)
+        with open(filename, 'wb') as f:
+            f.write(doc.content)
 
-    def print(self):
-        print('PlayHT')
+    def tts(self, text, voice, filename):
+        url = self.get_mp3_url(text=text, voice=voice)
+        if url is not None:
+            self.download_mp3(url=url, filename=filename)
+        else:
+            print("Error: url is None")
```

## Comparing `playht-0.0.2.dist-info/METADATA` & `playht-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playht
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/rhcproc/playht
 Author: Hans Park
 Author-email: rhcproc@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

