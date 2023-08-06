# Comparing `tmp/janus_client-0.3.0.tar.gz` & `tmp/janus_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_client-0.3.0.tar", max compression
+gzip compressed data, was "janus_client-0.4.0.tar", max compression
```

## Comparing `janus_client-0.3.0.tar` & `janus_client-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      274 2023-07-29 17:16:45.751175 janus_client-0.3.0/janus_client/__init__.py
--rw-r--r--   0        0        0    11597 2023-07-29 13:05:52.613860 janus_client-0.3.0/janus_client/core.py
--rw-r--r--   0        0        0     7592 2023-07-29 16:26:44.628495 janus_client-0.3.0/janus_client/media.py
--rw-r--r--   0        0        0     2570 2023-07-29 09:16:50.135149 janus_client-0.3.0/janus_client/plugin_base.py
--rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.3.0/janus_client/plugin_video_room.py
--rw-r--r--   0        0        0     8225 2023-07-29 12:49:05.375883 janus_client-0.3.0/janus_client/plugin_video_room_ffmpeg.py
--rw-r--r--   0        0        0     3552 2023-07-29 09:33:38.945245 janus_client-0.3.0/janus_client/session.py
--rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.3.0/LICENSE
--rw-r--r--   0        0        0      886 2023-07-29 17:27:15.029727 janus_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4449 2023-07-29 17:22:33.485710 janus_client-0.3.0/README.md
--rw-r--r--   0        0        0     5445 1970-01-01 00:00:00.000000 janus_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-08-06 06:54:43.649064 janus_client-0.4.0/janus_client/__init__.py
+-rw-r--r--   0        0        0    11283 2023-08-05 06:20:05.227375 janus_client-0.4.0/janus_client/core.py
+-rw-r--r--   0        0        0     7592 2023-07-29 16:26:44.628495 janus_client-0.4.0/janus_client/media.py
+-rw-r--r--   0        0        0     2816 2023-08-05 13:01:11.384945 janus_client-0.4.0/janus_client/plugin_base.py
+-rw-r--r--   0        0        0     1238 2023-08-05 12:51:20.448331 janus_client-0.4.0/janus_client/plugin_video_call.py
+-rw-r--r--   0        0        0    14360 2023-07-22 06:24:20.872509 janus_client-0.4.0/janus_client/plugin_video_room.py
+-rw-r--r--   0        0        0     7975 2023-08-05 13:30:07.030590 janus_client-0.4.0/janus_client/plugin_video_room_ffmpeg.py
+-rw-r--r--   0        0        0     4022 2023-08-06 06:16:17.063277 janus_client-0.4.0/janus_client/session.py
+-rw-r--r--   0        0        0     8072 2023-08-06 08:59:28.189276 janus_client-0.4.0/janus_client/transport.py
+-rw-r--r--   0        0        0     4330 2023-08-06 08:57:53.281310 janus_client-0.4.0/janus_client/transport_http.py
+-rw-r--r--   0        0        0     2660 2023-08-06 06:12:27.825554 janus_client-0.4.0/janus_client/transport_websocket.py
+-rw-r--r--   0        0        0     1069 2023-07-22 06:24:20.872509 janus_client-0.4.0/LICENSE
+-rw-r--r--   0        0        0      949 2023-08-06 09:09:28.545057 janus_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4662 2023-08-06 09:05:43.870792 janus_client-0.4.0/README.md
+-rw-r--r--   0        0        0     5716 1970-01-01 00:00:00.000000 janus_client-0.4.0/PKG-INFO
```

### Comparing `janus_client-0.3.0/janus_client/core.py` & `janus_client-0.4.0/janus_client/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,25 +83,14 @@
         """Disconnect from server"""
 
         logger.info("Disconnecting")
         self.receive_message_task.cancel()
         await self.ws.close()
         self.connected = False
 
-    def is_async_response(self, response: dict) -> bool:
-        janus_type = response["janus"]
-        return (
-            (janus_type == "event")
-            or (janus_type == "detached")
-            or (janus_type == "webrtcup")
-            or (janus_type == "media")
-            or (janus_type == "slowlink")
-            or (janus_type == "hangup")
-        )
-
     def receive_message_done_cb(self, task: asyncio.Task, context=None) -> None:
         try:
             # Check if any exceptions are raised
             task.exception()
             # traceback.print_tb(exception.__traceback__)
             # logger.info(f"{type(exception)} : {exception}")
         except asyncio.CancelledError:
@@ -113,21 +102,21 @@
 
     async def receive_message(self) -> None:
         if not self.ws:
             raise Exception("Not connected to server.")
 
         async for message_raw in self.ws:
             response = json.loads(message_raw)
-            logger.info(f"Receive: {response}")
+            logger.info(f"Received: {response}")
 
-            if self.is_async_response(response):
-                self.handle_async_response(response)
-            else:
+            if "transaction" in response:
                 transaction_id = response["transaction"]
                 await self.transactions[transaction_id].put(response)
+            else:
+                self.handle_async_response(response)
 
     async def send(self, message: JanusMessage) -> dict:
         """Send message to server
 
         :param message: JSON serializable dictionary to send
 
         :returns: Synchronous response from Janus server
@@ -151,14 +140,15 @@
         logger.info(f"Send: {message_json}")
         await self.ws.send(message_json)
 
         # Wait for response
         # Assumption: there will be one and only one synchronous reply for a transaction.
         #   Other replies with the same transaction ID are asynchronous.
         response = await self.transactions[message.transaction].get()
+        logger.info(f"Transaction response: {response}")
 
         # Transaction complete, delete it
         del self.transactions[message.transaction]
         return response
 
     def handle_async_response(self, response: dict) -> None:
         if "session_id" in response:
```

### Comparing `janus_client-0.3.0/janus_client/media.py` & `janus_client-0.4.0/janus_client/media.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.3.0/janus_client/plugin_base.py` & `janus_client-0.4.0/janus_client/plugin_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .session import JanusSession, SessionMessage
+import logging
 
+from .transport import ResponseHandlerType
+from .session import JanusSession
 
-class PluginMessage(SessionMessage):
-    handle_id: int = None
+
+logger = logging.getLogger(__name__)
 
 
 class JanusPlugin:
     """Base class to inherit when implementing a plugin"""
 
     name: str = "janus.plugin.base.dummy"
     """Plugin name
@@ -18,39 +20,50 @@
 
     @property
     def id(self) -> int:
         return self.__id
 
     async def attach(self, session: JanusSession):
         if self.__id:
-            raise Exception(f"Plugin already attached to session ({self.session.id})")
+            raise Exception(f"Plugin already attached to session ({self.session})")
 
         self.session = session
         self.__id = await session.attach_plugin(self)
 
     async def destroy(self):
         """Destroy plugin handle"""
 
-        await self.send(PluginMessage(janus="detach"))
+        await self.send({"janus": "detach"})
         self.session.detach_plugin(self)
 
-    async def send(self, message: PluginMessage) -> dict:
+    def __sanitize_message(self, message: dict) -> None:
+        if "handle_id" in message:
+            logger.warn(
+                f"Should not set handle_id ({message['handle_id']}). Overriding."
+            )
+            del message["handle_id"]
+
+    async def send(
+        self,
+        message: dict,
+        response_handler: ResponseHandlerType = lambda response: response,
+    ) -> dict:
         """Send raw message to plugin
 
         Will auto attach plugin ID to the message.
 
         :param message: JSON serializable dictionary to send
         :return: Synchronous reply from server
         """
 
-        if message.handle_id:
-            raise Exception("Plugin handle ID must not be manually added")
+        self.__sanitize_message(message=message)
 
-        message.handle_id = self.__id
-        return await self.session.send(message)
+        return await self.session.send(
+            message, handle_id=self.__id, response_handler=response_handler
+        )
 
     def handle_async_response(self, response: dict):
         """Handle asynchronous events from Janus
 
         Must be overridden
 
         :raises NotImplementedError: If not overridden and received event from server
@@ -61,25 +74,22 @@
     async def trickle(self, sdpMLineIndex, candidate):
         """Send WebRTC candidates to Janus
 
         :param sdpMLineIndex: (I don't know what is this)
         :param candidate: Candidate payload. (I got it from WebRTC instance callback)
         """
 
-        class TrickleMessage(PluginMessage):
-            candidate: dict
-
         candidate_payload = dict()
         if candidate:
             candidate_payload = {
                 "sdpMLineIndex": sdpMLineIndex,
                 "candidate": candidate,
             }
         else:
             # Reference: https://janus.conf.meetecho.com/docs/rest.html
             # - a null candidate or a completed JSON object to notify the end of the candidates.
             # TODO: test it
             candidate_payload = None
 
         # await self.send({"janus": "trickle", "candidate": candidate_payload})
-        await self.send(TrickleMessage(janus="trickle", candidate=candidate_payload))
+        await self.send({"janus": "trickle", "candidate": candidate_payload})
         # TODO: Implement sending an array of candidates
```

### Comparing `janus_client-0.3.0/janus_client/plugin_video_room.py` & `janus_client-0.4.0/janus_client/plugin_video_room.py`

 * *Files identical despite different names*

### Comparing `janus_client-0.3.0/janus_client/plugin_video_room_ffmpeg.py` & `janus_client-0.4.0/janus_client/plugin_video_room_ffmpeg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import logging
 
-from .plugin_base import JanusPlugin, PluginMessage
+from .plugin_base import JanusPlugin
 from aiortc import RTCPeerConnection, RTCSessionDescription, VideoStreamTrack
 from .media import MediaPlayer
 
 logger = logging.getLogger(__name__)
 
 
 class JanusVideoRoomPlugin(JanusPlugin):
@@ -18,15 +18,15 @@
 
     name = "janus.plugin.videoroom"  #: Plugin name
     pc = RTCPeerConnection()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.joined_event = asyncio.Event()
-        self.loop = asyncio.get_running_loop()
+        # self.loop = asyncio.get_running_loop()
 
     def handle_async_response(self, response: dict):
         if response["janus"] == "event":
             logger.info(f"Event response: {response}")
             if "plugindata" in response:
                 if response["plugindata"]["data"]["videoroom"] == "attached":
                     # Subscriber attached
@@ -49,43 +49,38 @@
         | There is an API to configure and publish at the same time, but it's not implemented yet.
 
         :param room_id: Room ID to join. This must be available at the server.
         :param publisher_id: Your publisher ID to set.
         :param display_name: Your display name when you join the room.
         """
 
-        class JoinMessage(PluginMessage):
-            body: dict
-
         response = await self.send(
-            JoinMessage(
-                janus="message",
-                body={
+            {
+                "janus": "message",
+                "body": {
                     "request": "join",
                     "ptype": "publisher",
                     "room": room_id,
                     "id": publisher_id,
                     "display": display_name,
                 },
-            )
+            },
+            response_handler=lambda response: response if response["janus"] == "ack" else None,
         )
         logger.info(f"Room join response: {response}")
         await self.joined_event.wait()
 
     async def leave(self):
-        class LeaveMessage(PluginMessage):
-            body: dict
-
         response = await self.send(
-            LeaveMessage(
-                janus="message",
-                body={
+            {
+                "janus": "message",
+                "body": {
                     "request": "leave",
                 },
-            )
+            }
         )
         logger.info(f"Room leave response: {response}")
 
     async def publish(self, ffmpeg_input, width: int, height: int) -> None:
         """Publish video stream to the room
 
         Should already have joined a room before this. Then this will publish the
@@ -114,45 +109,38 @@
 
         # send offer
         await self.pc.setLocalDescription(await self.pc.createOffer())
 
         request = {"request": "configure"}
         request.update(media)
 
-        class PublishMessage(PluginMessage):
-            body: dict
-            jsep: dict
-
         await self.send(
-            PublishMessage(
-                janus="message",
-                body=request,
-                jsep={
+            {
+                "janus": "message",
+                "body": request,
+                "jsep": {
                     "sdp": self.pc.localDescription.sdp,
                     "trickle": False,
                     "type": self.pc.localDescription.type,
                 },
-            )
+            }
         )
 
         await self.joined_event.wait()
 
     async def unpublish(self) -> None:
         """Stop publishing"""
 
-        class UnpublishMessage(PluginMessage):
-            body: dict
-
         await self.send(
-            UnpublishMessage(
-                janus="message",
-                body={
+            {
+                "janus": "message",
+                "body": {
                     "request": "unpublish",
                 },
-            )
+            }
         )
         await self.pc.close()
 
     async def subscribe(self, room_id: int, feed_id: int) -> None:
         """Subscribe to a feed
 
         :param room_id: Room ID containing the feed. The same ID that
```

### Comparing `janus_client-0.3.0/LICENSE` & `janus_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_client-0.3.0/pyproject.toml` & `janus_client-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "janus-client"
-version = "0.3.0"
-description = "Janus webrtc client in async Python."
+version = "0.4.0"
+description = "Janus gatewau webrtc async client in Python."
 authors = ["Joseph Lim <josephlim_94@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "janus_client"}]
 repository = "https://github.com/josephlim94/janus_gst_client_py"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -20,12 +20,13 @@
 python = "^3.10"
 websockets = "^11.0.3"
 aiortc = "^1.5.0"
 ffmpeg-python = "^0.2.0"
 numpy = "^1.25.1"
 av = "^10.0.0"
 pydantic = "^2.1.1"
+aiohttp = {extras = ["speedups"], version = "^3.8.5"}
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `janus_client-0.3.0/README.md` & `janus_client-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -33,23 +33,31 @@
 
 References:
 - [Aiortc Janus](https://github.com/aiortc/aiortc/tree/main/examples/janus).
 - [FFmpeg webrtc](https://github.com/ossrs/ffmpeg-webrtc/pull/1).
 
 ### Features
 
-:heavy_check_mark: Connect to Janus server through websocket (using [websockets](https://github.com/aaugustin/websockets))  
+:heavy_check_mark: Connect to Janus server through:
+  - Websocket API ([websockets](https://github.com/aaugustin/websockets))
+  - HTTP ([aiohttp](https://docs.aiohttp.org/en/stable/index.html))
+
 :heavy_check_mark: Automatically manage Janus client connection
 :heavy_check_mark: Manage message transactions with Janus  
 :heavy_check_mark: Manage sessions  
 ```python
 from janus_client import JanusSession
 
+# Protocol will be derived from base_url
+session = JanusSession(
+    base_url="wss://janusmy.josephgetmyip.com/janusbasews/janus",
+)
+# OR
 session = JanusSession(
-    uri="wss://janusmy.josephgetmyip.com/janusbasews/janus",
+    base_url="https://janusmy.josephgetmyip.com/janusbase/janus",
 )
 ```
 :heavy_check_mark: Manage plugins  
 :heavy_check_mark: Manage multiple sessions and or multiple plugins at the same time  
 ```python
 from janus_client import JanusVideoRoomPlugin
```

### Comparing `janus_client-0.3.0/PKG-INFO` & `janus_client-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: janus-client
-Version: 0.3.0
-Summary: Janus webrtc client in async Python.
+Version: 0.4.0
+Summary: Janus gatewau webrtc async client in Python.
 Home-page: https://github.com/josephlim94/janus_gst_client_py
 License: MIT
 Author: Joseph Lim
 Author-email: josephlim_94@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0)
 Requires-Dist: aiortc (>=1.5.0,<2.0.0)
 Requires-Dist: av (>=10.0.0,<11.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Project-URL: Repository, https://github.com/josephlim94/janus_gst_client_py
@@ -58,23 +59,31 @@
 
 References:
 - [Aiortc Janus](https://github.com/aiortc/aiortc/tree/main/examples/janus).
 - [FFmpeg webrtc](https://github.com/ossrs/ffmpeg-webrtc/pull/1).
 
 ### Features
 
-:heavy_check_mark: Connect to Janus server through websocket (using [websockets](https://github.com/aaugustin/websockets))  
+:heavy_check_mark: Connect to Janus server through:
+  - Websocket API ([websockets](https://github.com/aaugustin/websockets))
+  - HTTP ([aiohttp](https://docs.aiohttp.org/en/stable/index.html))
+
 :heavy_check_mark: Automatically manage Janus client connection
 :heavy_check_mark: Manage message transactions with Janus  
 :heavy_check_mark: Manage sessions  
 ```python
 from janus_client import JanusSession
 
+# Protocol will be derived from base_url
+session = JanusSession(
+    base_url="wss://janusmy.josephgetmyip.com/janusbasews/janus",
+)
+# OR
 session = JanusSession(
-    uri="wss://janusmy.josephgetmyip.com/janusbasews/janus",
+    base_url="https://janusmy.josephgetmyip.com/janusbase/janus",
 )
 ```
 :heavy_check_mark: Manage plugins  
 :heavy_check_mark: Manage multiple sessions and or multiple plugins at the same time  
 ```python
 from janus_client import JanusVideoRoomPlugin
```

