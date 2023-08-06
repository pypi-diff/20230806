# Comparing `tmp/medisearch_client-0.1.7.tar.gz` & `tmp/medisearch_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.7.tar", last modified: Sun Aug  6 04:13:00 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.8.tar", last modified: Sun Aug  6 04:28:03 2023, max compression
```

## Comparing `medisearch_client-0.1.7.tar` & `medisearch_client-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.892015 medisearch_client-0.1.7/
--rw-r--r--   0 mpmisko    (501) staff       (20)     4391 2023-08-06 04:13:00.891873 medisearch_client-0.1.7/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     4117 2023-08-06 04:11:39.000000 medisearch_client-0.1.7/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.890994 medisearch_client-0.1.7/medisearch_client/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.7/medisearch_client/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     4896 2023-08-06 04:08:57.000000 medisearch_client-0.1.7/medisearch_client/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.891681 medisearch_client-0.1.7/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     4391 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       50 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 04:13:00.892058 medisearch_client-0.1.7/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      597 2023-08-06 04:12:17.000000 medisearch_client-0.1.7/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:28:03.542280 medisearch_client-0.1.8/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4087 2023-08-06 04:28:03.542153 medisearch_client-0.1.8/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3813 2023-08-06 04:24:35.000000 medisearch_client-0.1.8/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:28:03.541306 medisearch_client-0.1.8/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.8/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4678 2023-08-06 04:27:28.000000 medisearch_client-0.1.8/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:28:03.541983 medisearch_client-0.1.8/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4087 2023-08-06 04:28:03.000000 medisearch_client-0.1.8/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 04:28:03.000000 medisearch_client-0.1.8/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 04:28:03.000000 medisearch_client-0.1.8/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       50 2023-08-06 04:28:03.000000 medisearch_client-0.1.8/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 04:28:03.000000 medisearch_client-0.1.8/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 04:28:03.542317 medisearch_client-0.1.8/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      597 2023-08-06 04:27:54.000000 medisearch_client-0.1.8/setup.py
```

### Comparing `medisearch_client-0.1.7/PKG-INFO` & `medisearch_client-0.1.8/medisearch_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: medisearch_client
-Version: 0.1.7
+Name: medisearch-client
+Version: 0.1.8
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 # MediSearch API Client
@@ -80,34 +80,14 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-
-### Interrupting generation
-
-You may interrupt the generation of the response by running:
-
-```python
-client.interrupt()
-```
-
-This is useful for implementing a 'stop-generate'-like button on your frontend.
-
-
-### Closing the connection
-
-To close the connection, simply run:
-
-```python
-client.close()
-```
-
 ## Output structure
 
 In the following call to our API
 
 ```
 responses = client.send_user_message(
     conversation=["By how much does sport increase life expectancy?"],
```

### Comparing `medisearch_client-0.1.7/README.md` & `medisearch_client-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -71,34 +71,14 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-
-### Interrupting generation
-
-You may interrupt the generation of the response by running:
-
-```python
-client.interrupt()
-```
-
-This is useful for implementing a 'stop-generate'-like button on your frontend.
-
-
-### Closing the connection
-
-To close the connection, simply run:
-
-```python
-client.close()
-```
-
 ## Output structure
 
 In the following call to our API
 
 ```
 responses = client.send_user_message(
     conversation=["By how much does sport increase life expectancy?"],
```

### Comparing `medisearch_client-0.1.7/medisearch_client/client.py` & `medisearch_client-0.1.8/medisearch_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import json
 import websocket
 
 
 class MediSearchClient:
   """Sample client for the MediSearch API."""
 
-  def __init__(self, api_key):
+  def __init__(self, api_key: str):
     self.api_key = api_key
     self.url = "wss://public.backend.medisearch.io:443/ws/medichat/api"
-    self.socket = websocket.create_connection(self.url)
     self.interrupted = False
 
   def send_user_message(
       self,
       conversation: list[str],
       conversation_id: str,
       should_stream_response: bool = False,
@@ -57,44 +56,37 @@
         "conversation": conversation,
         "key": self.api_key,
         "id": conversation_id,
         "settings": {
             "language": language
         }
     }
-    self._send_payload(payload)
-    response_iter = self._response_iterator()
+    socket = websocket.create_connection(self.url)
+    self._send_payload(payload, socket)
+    response_iter = self._response_iterator(socket)
     if should_stream_response:
       return response_iter
 
     responses = list(response_iter)
     # Filter all llm_response events except for the last one.
     return self._filter_llm_responses(responses)
 
-  def interrupt(self) -> None:
-    """Interrupt the conversation with the MediSearch API."""
-    payload = {"event": "interrupt", "key": self.api_key}
-    self._send_payload(payload)
-    self.interrupted = True
-
-  def close(self) -> None:
-    """Close the connection to the MediSearch API."""
-    payload = {"event": "close", "key": self.api_key}
-    self._send_payload(payload)
-
-  def reconnect(self, attempts: int = 4) -> None:
+  def _reconnect(self,
+                 socket: websocket.WebSocket,
+                 attempts: int = 4) -> websocket.WebSocket:
     """Reconnect to the MediSearch API.
 
     Args:
+        socket: The websocket connection to the MediSearch API.
         attempts: Number of attempts to reconnect. Defaults to 4.
     """
     for _ in range(attempts):
       try:
-        self.socket = websocket.create_connection(self.url)
-        return
+        socket = websocket.create_connection(self.url)
+        return socket
       except Exception as _:  # pylint: disable=broad-except
         pass
     raise RuntimeError(
         "Failed to reconnect to the WebSocket server after multiple attempts.")
 
   def _filter_llm_responses(
       self, responses: list[dict[str, str]]) -> list[dict[str, str]]:
@@ -107,33 +99,30 @@
         seen_llm_response = True
         filtered_responses.append(resp)
       elif resp["event"] != "llm_response":
         filtered_responses.append(resp)
 
     return list(reversed(filtered_responses))
 
-  def _send_payload(self, payload):
-    if not self.socket.connected:
-      self.reconnect()
+  def _send_payload(self, payload: dict[str, str],
+                    socket: websocket.WebSocket) -> None:
+    if not socket.connected:
+      socket = self._reconnect(socket=socket)
     try:
-      self.socket.send(json.dumps(payload))
+      socket.send(json.dumps(payload))
     except websocket.WebSocketConnectionClosedException as _:
       raise websocket.WebSocketConnectionClosedException(
           ("WebSocket connection lost. Please reinitialize the client or check"
            " the server status."))
 
-  def _response_iterator(self):
+  def _response_iterator(self, socket: websocket.WebSocket):
     while True:
-      if not self.socket.connected:
-        self.reconnect()
+      if not socket.connected:
+        self._reconnect(socket=socket)
       if self.interrupted:
         break
-      try:
-        data = json.loads(self.socket.recv())
-      except Exception as _:  # pylint: disable=broad-except
-        self.reconnect()
-        continue
+      data = json.loads(socket.recv())
       yield data
       if "event" in data and (data["event"] == "articles" or
                               data["event"] == "error"):
         break
     self.interrupted = False
```

### Comparing `medisearch_client-0.1.7/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: medisearch-client
-Version: 0.1.7
+Name: medisearch_client
+Version: 0.1.8
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 # MediSearch API Client
@@ -80,34 +80,14 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-
-### Interrupting generation
-
-You may interrupt the generation of the response by running:
-
-```python
-client.interrupt()
-```
-
-This is useful for implementing a 'stop-generate'-like button on your frontend.
-
-
-### Closing the connection
-
-To close the connection, simply run:
-
-```python
-client.close()
-```
-
 ## Output structure
 
 In the following call to our API
 
 ```
 responses = client.send_user_message(
     conversation=["By how much does sport increase life expectancy?"],
```

### Comparing `medisearch_client-0.1.7/setup.py` & `medisearch_client-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
         "websocket-client", "pyasn1", "pyopenssl", "ndg-httpsclient"
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
     description="A simple client for the MediSearch API",
```

