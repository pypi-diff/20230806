# Comparing `tmp/avilla-elizabeth-1.0.0a5.tar.gz` & `tmp/avilla-elizabeth-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla-elizabeth-1.0.0a5.tar", last modified: Sun Dec 25 09:53:47 2022, max compression
+gzip compressed data, was "avilla-elizabeth-1.0.0rc4.tar", last modified: Wed Aug 31 04:41:00 2022, max compression
```

## Comparing `avilla-elizabeth-1.0.0a5.tar` & `avilla-elizabeth-1.0.0rc4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-25 09:53:28.177185 avilla-elizabeth-1.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2022-12-25 09:53:28.177185 avilla-elizabeth-1.0.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/event/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/impl/friend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/message_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/avilla/elizabeth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2022-12-25 09:53:28.181186 avilla-elizabeth-1.0.0a5/pyproject.toml
--rw-------   0 runner    (1001) docker     (123)     7339 2022-12-25 09:53:47.561184 avilla-elizabeth-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-08-31 04:32:04.327287 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/__init__.py
+-rw-rw-rw-   0        0        0     1474 2022-08-31 04:32:04.328263 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/_query.py
+-rw-rw-rw-   0        0        0     2164 2022-08-31 04:32:04.330401 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/account.py
+-rw-rw-rw-   0        0        0     4206 2022-08-31 04:32:04.331330 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/__init__.py
+-rw-rw-rw-   0        0        0     2481 2022-08-31 04:32:04.333136 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/config.py
+-rw-rw-rw-   0        0        0     6231 2022-08-31 04:32:04.336566 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/http.py
+-rw-rw-rw-   0        0        0     2934 2022-08-31 04:32:04.337964 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/util.py
+-rw-rw-rw-   0        0        0     6998 2022-08-31 04:32:04.339974 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/ws.py
+-rw-rw-rw-   0        0        0      175 2022-08-31 04:32:04.341001 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/element.py
+-rw-rw-rw-   0        0        0     5247 2022-08-31 04:32:04.342904 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/event_parser.py
+-rw-rw-rw-   0        0        0      898 2022-08-31 04:32:04.343937 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/exception.py
+-rw-rw-rw-   0        0        0     1208 2022-08-31 04:32:04.345888 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/__init__.py
+-rw-rw-rw-   0        0        0     1781 2022-08-31 04:34:09.980332 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/friend.py
+-rw-rw-rw-   0        0        0     9574 2022-08-31 04:34:09.989126 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/group.py
+-rw-rw-rw-   0        0        0     1867 2022-08-31 04:32:04.360005 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/message_deserializer.py
+-rw-rw-rw-   0        0        0     1808 2022-08-31 04:32:04.361963 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/message_serializer.py
+-rw-rw-rw-   0        0        0     2333 2022-08-31 04:34:09.996931 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/protocol.py
+-rw-rw-rw-   0        0        0     1524 2022-08-31 04:32:04.363912 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/resource.py
+-rw-rw-rw-   0        0        0     1988 2022-08-31 04:32:04.364894 avilla-elizabeth-1.0.0rc4/avilla/elizabeth/service.py
+-rw-rw-rw-   0        0        0     1091 2022-02-26 15:50:19.520302 avilla-elizabeth-1.0.0rc4/LICENSE
+-rw-rw-rw-   0        0        0     2051 2022-08-31 04:36:38.408969 avilla-elizabeth-1.0.0rc4/pyproject.toml
+-rw-rw-rw-   0        0        0     7166 2022-08-31 04:32:04.240367 avilla-elizabeth-1.0.0rc4/README.md
+-rw-rw-rw-   0        0        0     7371 2022-08-31 04:41:00.756210 avilla-elizabeth-1.0.0rc4/PKG-INFO
```

### Comparing `avilla-elizabeth-1.0.0a5/LICENSE` & `avilla-elizabeth-1.0.0rc4/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Graia Project
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Graia Project
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `avilla-elizabeth-1.0.0a5/README.md` & `avilla-elizabeth-1.0.0rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: avilla-elizabeth
+Version: 1.0.0rc4
+License: MIT
+Author-email: GreyElaina <GreyElaina@outlook.com>
+Requires-Python: >=3.9
+Project-URL: homepage, https://github.com/GraiaProject/Avilla
+Project-URL: repository, https://github.com/GraiaProject/Avilla
+Description-Content-Type: text/markdown
+
 <div align="center">
 
 # Avilla
 
 _The next-gen framework for IM development._
 
 > 即刻动身, 踏上寻找第二个故乡的旅程.
@@ -35,35 +45,34 @@
  - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
  - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
 
 ## Quick Start
 
 ```py
 from creart import create
-from graia.amnesia.builtins.aiohttp import AiohttpClientService
+from graia.amnesia.builtins.aiohttp import AiohttpService
 from graia.broadcast import Broadcast
 
-from avilla.core import Avilla, Context, MessageReceived
+from avilla.core import Avilla, MessageReceived, Relationship, Selector
 from avilla.elizabeth.connection.config import WebsocketClientConfig
 from avilla.elizabeth.protocol import ElizabethProtocol
 
 broadcast = create(Broadcast)
-avilla = Avilla(
-    broadcast, [ElizabethProtocol(WebsocketClientConfig("bot-account", "mah-verify-code"))], [AiohttpClientService()]
-)
-
+avilla = Avilla(broadcast, [
+    ElizabethProtocol(
+        WebsocketClientConfig("bot-account", "mah-verify-code")
+    )
+], [AiohttpService()])
 
 @broadcast.receiver(MessageReceived)
-async def on_message_received(ctx: Context, event: MessageReceived):
-    if ctx.client.follows("group.member(<master-account>)"):
-        await ctx.scene.send_message("Hello, Avilla!")
-
+async def on_message_received(event: MessageReceived, rs: Relationship):
+    if Selector.fragment().as_dyn().group("*").member("master-account").match(rs.ctx):
+        await rs.send_message("Hello, Avilla!")
 
 avilla.launch_manager.launch_blocking(loop=broadcast.loop)
-
 ```
 
 ## 部件发布情况
 
 |代号|协议|开发进度|PyPI|维护者|开源协议|
 | :-: | :-: | :-: | :-: | :-: | :-: |
 |      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |MIT|
@@ -107,7 +116,8 @@
 
 </div>
 
 
 ## 开源协议
 
 若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
+
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/_query.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/_query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Callable
-
-from avilla.core.querier import ProtocolAbstractQueryHandler, query
-from avilla.core.selector import Selector
-from avilla.elizabeth.account import ElizabethAccount
-
-if TYPE_CHECKING:
-    from avilla.core.context import Context
-
-
-class ElizabethRootQuery(ProtocolAbstractQueryHandler):
-    @query("group")
-    async def query_group(self, rs: Context, prefix: Selector, checker: Callable[[Selector], bool]):
-        account = rs.account
-        assert isinstance(account, ElizabethAccount)
-        result: list[dict] = await account.call("groupList", {"__method__": "get"})
-        for i in result:
-            group = Selector().land(rs.land).group(str(i["id"]))
-            if checker(group):
-                yield group
-
-
-class ElizabethGroupQuery(ProtocolAbstractQueryHandler, prefix="group"):
-    @query("member")
-    async def query_member(self, rs: Context, prefix: Selector, checker: Callable[[Selector], bool]):
-        account = rs.account
-        assert isinstance(account, ElizabethAccount)
-        result: list[dict] = await account.call(
-            "memberList", {"__method__": "get", "target": int(prefix.pattern["group"])}
-        )
-        for i in result:
-            member = Selector().land(rs.land).group(str(i["group"]["id"])).member(str(i["id"]))
-            if checker(member):
-                yield member
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Callable
+
+from avilla.core.querier import ProtocolAbstractQueryHandler, query
+from avilla.core.utilles.selector import Selector
+from avilla.elizabeth.account import ElizabethAccount
+
+if TYPE_CHECKING:
+    from avilla.core.relationship import Relationship
+
+
+class ElizabethRootQuery(ProtocolAbstractQueryHandler):
+    @query("group")
+    async def query_group(self, rs: Relationship, prefix: Selector, checker: Callable[[Selector], bool]):
+        account = rs.account
+        assert isinstance(account, ElizabethAccount)
+        result: list[dict] = await account.call("groupList", {"__method__": "get"})
+        for i in result:
+            group = Selector().land(rs.land).group(str(i["id"]))
+            if checker(group):
+                yield group
+
+
+class ElizabethGroupQuery(ProtocolAbstractQueryHandler, prefix="group"):
+    @query("member")
+    async def query_member(self, rs: Relationship, prefix: Selector, checker: Callable[[Selector], bool]):
+        account = rs.account
+        assert isinstance(account, ElizabethAccount)
+        result: list[dict] = await account.call(
+            "memberList", {"__method__": "get", "target": int(prefix.pattern["group"])}
+        )
+        for i in result:
+            member = Selector().land(rs.land).group(str(i["group"]["id"])).member(str(i["id"]))
+            if checker(member):
+                yield member
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/__init__.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Generic, Optional
+from typing import TYPE_CHECKING, Any, Generic, Optional, Set, Type
 
 from graia.amnesia.transport.common.status import (
     ConnectionStatus as BaseConnectionStatus,
 )
-from launart import ExportInterface, Launchable, LaunchableStatus
+from launart import Launchable, LaunchableStatus
 from loguru import logger
 from statv import Stats
 
-from avilla.spec.core.application import AccountAvailable, AccountUnavailable
+from avilla.core.utilles.selector import Selector
 
 from .config import HttpClientConfig, HttpServerConfig, T_Config
 from .config import U_Config as U_Config
 from .config import WebsocketClientConfig, WebsocketServerConfig
 from .util import CallMethod, camel_to_snake
 
 if TYPE_CHECKING:
@@ -55,20 +55,20 @@
         )
 
 
 class ElizabethConnection(Launchable, Generic[T_Config]):
     status: ConnectionStatus
     protocol: ElizabethProtocol
     config: T_Config
-    dependencies: frozenset[str | type[ExportInterface]]
+    dependencies: frozenset[str]
 
     http_conn: Optional["HttpClientConnection"]
 
     @property
-    def required(self):
+    def required(self) -> Set[str]:
         return set(self.dependencies)
 
     @property
     def stages(self):
         return set()
 
     def register_account(self):
@@ -78,22 +78,14 @@
         if self.account not in self.protocol.avilla.accounts:
             self.protocol.avilla.add_account(self.account)
             logger.success(
                 f"Registered account: {self.config.account}",
                 alt=f"[green]Registered account: [magenta]{self.config.account}[/]",
             )
 
-    def on_connected_update(self, statv: ConnectionStatus, stats: Stats[bool], past: bool, current: bool) -> None:
-        if past != current:
-            logger.warning(f"Account({self.account.id}): {'Connected' if current else 'Disconnected'}")
-            proto = self.account.protocol
-            proto.avilla.broadcast.postEvent(
-                (AccountAvailable if current else AccountUnavailable)(proto.avilla, self.account)
-            )
-
     def __init__(self, protocol: ElizabethProtocol, config: T_Config) -> None:
         from avilla.elizabeth.account import ElizabethAccount
 
         from .http import HttpClientConnection
 
         self.id = ".".join(
             [
@@ -102,15 +94,14 @@
                 str(config.account),
                 camel_to_snake(self.__class__.__qualname__),
             ]
         )
         self.protocol = protocol
         self.config = config
         self.status = ConnectionStatus()
-        self.status.on_update(ConnectionStatus.connected)(self.on_connected_update)
         if config.use_http:
             self.http_conn = HttpClientConnection(protocol, HttpClientConfig.cast(config))
             self.http_conn.is_hook = True
             self.http_conn.status = self.status
             self.dependencies |= self.http_conn.dependencies
         else:
             self.http_conn = None
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/config.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/config.py`

 * *Files identical despite different names*

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/http.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from aiohttp import FormData
 from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
 from graia.amnesia.json import Json
 from graia.amnesia.transport import Transport
 from graia.amnesia.transport.common.http import AbstractServerRequestIO, HttpEndpoint
 from graia.amnesia.transport.common.http.extra import HttpRequest
-from graia.amnesia.transport.common.server import AbstractRouter
 from launart import Launart
 from launart.utilles import wait_fut
 from loguru import logger
 
 from ..exception import InvalidSession
 from . import ElizabethConnection
 from .config import HttpClientConfig, HttpServerConfig
@@ -22,15 +21,15 @@
 if TYPE_CHECKING:
     from avilla.elizabeth.protocol import ElizabethProtocol
 
 
 class HttpServerConnection(ElizabethConnection[HttpServerConfig], Transport):
     """HTTP 服务器连接"""
 
-    dependencies = frozenset([AbstractRouter])
+    dependencies = frozenset(["http.universal_server"])
 
     def __init__(self, protocol: ElizabethProtocol, config: HttpServerConfig) -> None:
         super().__init__(protocol, config)
         self.handlers[HttpEndpoint(self.config.path, ["POST"])] = self.__class__.handle_request
 
     async def handle_request(self, io: AbstractServerRequestIO):
         req: HttpRequest = await io.extra(HttpRequest)
@@ -40,30 +39,28 @@
             if req.headers.get(k) != v:
                 return "Authorization failed", {"status": 401}
         data = Json.deserialize((await io.read()).decode("utf-8"))
         assert isinstance(data, dict)
         self.status.connected = True
         self.status.alive = True
         self.register_account()  # LINK: hot registration
-        try:
-            event, context = await self.protocol.parse_event(self.account, data)
-            self.protocol.post_event(event, context)
-        except Exception:
-            logger.exception("error on parsing event: ", data)
+        event = await self.protocol.event_parser.parse_event(self.protocol, self.account, data)
+        if event is not None:
+            self.protocol.post_event(event)
         return {"command": "", "data": {}}
 
     async def launch(self, mgr: Launart) -> None:
         router = get_router(mgr)
         router.use(self)
 
 
 class HttpClientConnection(ElizabethConnection[HttpClientConfig]):
     """HTTP 客户端连接"""
 
-    dependencies = frozenset([AiohttpClientInterface])
+    dependencies = frozenset(["http.universal_client"])
     http_interface: AiohttpClientInterface
 
     def __init__(self, protocol: ElizabethProtocol, config: HttpClientConfig) -> None:
         super().__init__(protocol, config)
         self.is_hook: bool = False
 
     async def request(
@@ -140,16 +137,14 @@
                 except Exception as e:
                     self.status.session_key = None
                     self.status.alive = False
                     logger.exception(e)
                     continue
                 assert isinstance(data, list)
                 for event_data in data:
-                    try:
-                        event, context = await self.protocol.parse_event(self.account, event_data)
-                        self.protocol.post_event(event, context)
-                    except Exception:
-                        logger.exception("error on parsing event: ", event_data)
+                    event = await self.protocol.event_parser.parse_event(self.protocol, self.account, event_data)
+                    if event is not None:
+                        self.protocol.post_event(event)
                 await wait_fut(
                     [asyncio.sleep(0.5), mgr.status.wait_for_sigexit()],
                     return_when=asyncio.FIRST_COMPLETED,
                 )
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/util.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/util.py`

 * *Files identical despite different names*

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/connection/ws.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/connection/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import asyncio
 import secrets
 from typing import TYPE_CHECKING, Any, Dict, MutableMapping, Optional, TypeVar
 from weakref import WeakValueDictionary
 
 from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
 from graia.amnesia.transport import Transport
-from graia.amnesia.transport.common.client import AbstractClientInterface
 from graia.amnesia.transport.common.http.extra import HttpRequest
 from graia.amnesia.transport.common.websocket import (
     AbstractWebsocketIO,
     WebsocketCloseEvent,
     WebsocketConnectEvent,
     WebsocketEndpoint,
     WebsocketReceivedEvent,
@@ -67,19 +66,17 @@
             logger.success("Successfully got session key", style="green bold")
             self.register_account()  # LINK: hot registration
             return
         if sync_id in self.futures:
             self.futures[sync_id].set_result(data)
         elif "type" in data:
             self.status.alive = True
-            try:
-                event, context = await self.protocol.parse_event(self.account, data)
-                self.protocol.post_event(event, context)
-            except Exception:
-                logger.exception("error on parsing event: ", data)
+            event = await self.protocol.event_parser.parse_event(self.protocol, self.account, data)
+            if event:
+                self.protocol.post_event(event)
         else:
             logger.warning(f"Got unknown data: {raw}")
 
     @t.handle(WebsocketReconnect)
     async def _(self, _) -> bool:
         logger.warning("Websocket reconnecting in 5s...", style="dark_orange")
         await asyncio.sleep(5)
@@ -117,15 +114,15 @@
 t = TransportRegistrar()
 
 
 @t.apply
 class WebsocketServerConnection(BaseWebsocketConnection[WebsocketServerConfig]):
     """Websocket 服务器连接"""
 
-    dependencies = frozenset([AbstractClientInterface])
+    dependencies = frozenset(["http.universal_server"])
 
     config: WebsocketServerConfig
 
     def __init__(self, protocol: ElizabethProtocol, config: WebsocketServerConfig) -> None:
         super().__init__(protocol, config)
         self.declares.append(WebsocketEndpoint(self.config.path))
 
@@ -161,15 +158,15 @@
 t = TransportRegistrar()
 
 
 @t.apply
 class WebsocketClientConnection(BaseWebsocketConnection[WebsocketClientConfig]):
     """Websocket 客户端连接"""
 
-    dependencies = frozenset([AbstractClientInterface])
+    dependencies = frozenset(["http.universal_client"])
     http_interface: AiohttpClientInterface
     config: WebsocketClientConfig
 
     @property
     def stages(self):
         return {"blocking"}
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/exception.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/exception.py`

 * *Files identical despite different names*

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/impl/__init__.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
-
-from avilla.core.trait.context import bounds, fetch, get_artifacts
-from avilla.core.trait.signature import CompleteRule
-from avilla.elizabeth.resource import (
-    ElizabethAudioResource,
-    ElizabethImageResource,
-    ElizabethResource,
-)
-
-# from graia.amnesia.transport.common.http import AbstractClientInterface
-
-
-if TYPE_CHECKING:
-    from avilla.core.context import Context
-
-# raise_for_no_namespace()
-
-# Relationship Complete
-
-# with scope("group"), prefix("group"):
-#     completes("member", "group.member")
-with bounds("group"):
-    get_artifacts().setdefault(CompleteRule("member"), "group.member")
-
-
-@fetch(ElizabethImageResource)  # type: ignore
-@fetch(ElizabethAudioResource)
-async def fetch_from_url(ctx: Context, res: ElizabethResource) -> bytes:
-    if not res.url:
-        raise NotImplementedError
-    # print(ctx.avilla.launch_manager._service_bind)
-    client = ctx.avilla.launch_manager.get_interface(AiohttpClientInterface)
-    # NOTE: wait for amnesia's fix on this.
-    return await (await client.request("GET", res.url)).io().read()
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from graia.amnesia.builtins.aiohttp import AiohttpClientInterface
+
+from avilla.core.trait.context import prefix, raise_for_no_namespace, scope
+from avilla.core.trait.recorder import completes, default_target, fetch, impl, pull
+from avilla.core.utilles.selector import Selector
+from avilla.elizabeth.resource import ElizabethAudioResource, ElizabethImageResource
+
+# from graia.amnesia.transport.common.http import AbstractClientInterface
+
+
+if TYPE_CHECKING:
+    from avilla.core.relationship import Relationship
+
+raise_for_no_namespace()
+
+# Relationship Complete
+
+with scope("group"), prefix("group"):
+    completes("member", "group.member")
+
+
+@fetch(ElizabethImageResource)
+@fetch(ElizabethAudioResource)
+async def fetch_from_url(rs: Relationship, res: ElizabethAudioResource | ElizabethImageResource) -> bytes:
+    if not res.url:
+        raise NotImplementedError
+    print(rs.avilla.launch_manager._service_bind)
+    client = rs.avilla.launch_manager.get_interface(AiohttpClientInterface)
+    # NOTE: wait for amnesia's fix on this.
+    return await (await client.request("GET", res.url)).io().read()
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/impl/friend.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/impl/friend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,50 @@
-from __future__ import annotations
-
-from datetime import datetime
-from typing import TYPE_CHECKING
-
-from avilla.core.selector import Selector
-from avilla.core.trait.context import bounds, implement
-from avilla.spec.core.message import MessageRevoke, MessageSend
-
-from ...core.message import Message
-
-if TYPE_CHECKING:
-    from graia.amnesia.message import __message_chain_class__
-
-    from avilla.core.context import Context
-
-    from ..protocol import ElizabethProtocol
-
-
-with bounds("friend"):
-
-    # casts(MessageSend)
-    # casts(MessageRevoke)
-
-    @implement(MessageSend.send)
-    async def send_friend_message(
-        ctx: Context, target: Selector, message: __message_chain_class__, *, reply: Selector | None = None
-    ) -> Selector:
-        if TYPE_CHECKING:
-            assert isinstance(ctx.protocol, ElizabethProtocol)
-        serialized_msg = await ctx.protocol.serialize_message(message)
-        result = await ctx.account.call(
-            "sendFriendMessage",
-            {
-                "__method__": "post",
-                "target": int(target.pattern["friend"]),
-                "messageChain": serialized_msg,
-                **({"quote": reply.pattern["message"]} if reply is not None else {}),
-            },
-        )
-        message_metadata = Message(
-            describe=Message,
-            id=str(result["messageId"]),
-            scene=Selector().land(ctx.land).friend(str(target.pattern["friend"])),
-            content=message,
-            time=datetime.now(),
-            sender=ctx.account.to_selector(),
-        )
-        message_selector = message_metadata.to_selector()
-        ctx._collect_metadatas(message_selector, message_metadata)
-        return message_selector
-
-    @implement(MessageRevoke.revoke)
-    async def revoke_friend_message(ctx: Context, message: Selector):
-        await ctx.account.call(
-            "recall",
-            {
-                "__method__": "post",
-                "messageId": int(message.pattern["message"]),
-                "target": int(message.pattern["friend"]),
-            },
-        )
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from avilla.core.message import Message
+from avilla.core.skeleton.message import MessageTrait
+from avilla.core.trait.context import prefix, raise_for_no_namespace, scope
+from avilla.core.trait.recorder import default_target, impl, pull
+from avilla.core.utilles.selector import Selector
+
+if TYPE_CHECKING:
+    from graia.amnesia.message import MessageChain
+
+    from avilla.core.relationship import Relationship
+
+
+raise_for_no_namespace()
+
+with scope("qq", "friend"), prefix("friend"):
+
+    @default_target(MessageTrait.send)
+    def send_friend_message_default_target(rs: Relationship):
+        return rs.ctx
+
+    @impl(MessageTrait.send)
+    async def send_friend_message(
+        rs: Relationship, target: Selector, message: MessageChain, *, reply: Selector | None = None
+    ) -> Selector:
+        serialized_msg = await rs.protocol.serialize_message(message)
+        result = await rs.account.call(
+            "sendFriendMessage",
+            {
+                "__method__": "post",
+                "target": int(target.pattern["friend"]),
+                "messageChain": serialized_msg,
+                **({"quote": reply.pattern["message"]} if reply is not None else {}),
+            },
+        )
+        return Selector().land(rs.land).group(target.pattern["friend"]).message(result["messageId"])
+
+    @impl(MessageTrait.revoke)
+    async def revoke_friend_message(rs: Relationship, message: Selector):
+        await rs.account.call(
+            "recall",
+            {
+                "__method__": "post",
+                "messageId": int(message.pattern["message"]),
+                "target": int(message.pattern["friend"]),
+            },
+        )
```

### Comparing `avilla-elizabeth-1.0.0a5/avilla/elizabeth/resource.py` & `avilla-elizabeth-1.0.0rc4/avilla/elizabeth/resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from __future__ import annotations
-
-from avilla.core.resource import Resource
-from avilla.core.selector import Selector
-
-
-class ElizabethResource(Resource[bytes]):
-    url: str | None = None
-    path: str | None = None
-    base64: str | None = None
-    scene: Selector | None = None
-
-    def __init__(
-        self,
-        id: str,
-        url: str | None = None,
-        path: str | None = None,
-        base64: str | None = None,
-        scene: Selector | None = None,
-    ) -> None:
-        self.id = id
-        self.url = url
-        self.path = path
-        self.base64 = base64
-        self.scene = scene
-
-    @property
-    def type(self) -> str:
-        return "elizabeth_resource"
-
-    @property
-    def selector(self) -> Selector:
-        return (self.scene or Selector()).appendix(self.type, self.id)
-
-
-class ElizabethImageResource(ElizabethResource):
-    @property
-    def type(self) -> str:
-        return "picture"
-
-
-class ElizabethAudioResource(ElizabethResource):
-    length: int | None = None
-
-    def __init__(
-        self,
-        id: str,
-        url: str | None = None,
-        path: str | None = None,
-        base64: str | None = None,
-        length: int | None = None,
-        scene: Selector | None = None,
-    ) -> None:
-        super().__init__(id, url, path, base64, scene)
-        self.length = length
-
-    @property
-    def type(self) -> str:
-        return "audio"
+from __future__ import annotations
+
+from avilla.core.resource import Resource
+from avilla.core.utilles.selector import Selector
+
+
+class ElizabethResource(Resource[bytes]):
+    url: str | None = None
+    path: str | None = None
+    base64: str | None = None
+    mainline: Selector | None = None
+
+    def __init__(
+        self,
+        id: str,
+        url: str | None = None,
+        path: str | None = None,
+        base64: str | None = None,
+        mainline: Selector | None = None,
+    ) -> None:
+        self.id = id
+        self.url = url
+        self.path = path
+        self.base64 = base64
+        self.mainline = mainline
+
+    @property
+    def type(self) -> str:
+        return "elizabeth_resource"
+
+    @property
+    def selector(self) -> Selector:
+        return (self.mainline.copy() if self.mainline is not None else Selector()).appendix(self.type, self.id)
+
+
+class ElizabethImageResource(ElizabethResource):
+    @property
+    def type(self) -> str:
+        return "picture"
+
+
+class ElizabethAudioResource(ElizabethResource):
+    length: int | None = None
+
+    def __init__(
+        self,
+        id: str,
+        url: str | None = None,
+        path: str | None = None,
+        base64: str | None = None,
+        mainline: Selector | None = None,
+        length: int | None = None,
+    ) -> None:
+        super().__init__(id, url, path, base64, mainline)
+        self.length = length
+
+    @property
+    def type(self) -> str:
+        return "audio"
```

### Comparing `avilla-elizabeth-1.0.0a5/pyproject.toml` & `avilla-elizabeth-1.0.0rc4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avilla-elizabeth"
-version = "1.0.0-alpha.5"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = []
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
@@ -32,25 +32,21 @@
 [tool.mina]
 enabled = false
 
 [tool.mina.packages.core]
 includes = [
     "avilla/core",
     "avilla/core/py.typed",
-    "avilla/spec/core",
 ]
 
 [tool.mina.packages.core.project]
 name = "avilla-core"
-version = "1.0.0-alpha.5"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
-    { name = "BlueGlassBlock", email = "blueglassblock@outlook.com" },
-    { name = "ProgramRipper", email = "programripper@foxmail.com" },
-    { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-broadcast",
     "graia-amnesia",
     "loguru",
     "yarl",
     "launart",
@@ -67,21 +63,20 @@
 repository = "https://github.com/GraiaProject/Avilla"
 
 [tool.mina.packages.elizabeth]
 includes = [
     "avilla/elizabeth",
 ]
 raw-dependencies = [
-    "avilla-core >= 1.0.0-alpha.5",
-    "avilla-spec-qq >= 1.0.0-alpha.5",
+    "avilla-core>=1.0.0rc4",
 ]
 
 [tool.mina.packages.elizabeth.project]
 name = "avilla-elizabeth"
-version = "1.0.0-alpha.5"
+version = "1.0.0rc4"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = []
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
@@ -89,43 +84,14 @@
 [tool.mina.packages.elizabeth.project.license]
 text = "MIT"
 
 [tool.mina.packages.elizabeth.project.urls]
 homepage = "https://github.com/GraiaProject/Avilla"
 repository = "https://github.com/GraiaProject/Avilla"
 
-[tool.mina.packages."spec/qq"]
-includes = [
-    "avilla/spec/qq",
-]
-raw_dependencies = [
-    "avilla-core >= 1.0.0-alpha.5",
-]
-
-[tool.mina.packages."spec/qq".project]
-name = "avilla-spec-qq"
-version = "1.0.0-alpha.5"
-authors = [
-    { name = "GreyElaina", email = "GreyElaina@outlook.com" },
-    { name = "BlueGlassBlock", email = "blueglassblock@outlook.com" },
-    { name = "ProgramRipper", email = "programripper@foxmail.com" },
-    { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
-]
-dependencies = []
-description = ""
-readme = "README.md"
-requires-python = ">=3.9"
-
-[tool.mina.packages."spec/qq".project.license]
-text = "MIT"
-
-[tool.mina.packages."spec/qq".project.urls]
-homepage = "https://github.com/GraiaProject/Avilla"
-repository = "https://github.com/GraiaProject/Avilla"
-
 [tool.black]
 include = "\\.pyi?$"
 line-length = 120
 target-version = [
     "py39",
 ]
```

### Comparing `avilla-elizabeth-1.0.0a5/PKG-INFO` & `avilla-elizabeth-1.0.0rc4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,124 +1,112 @@
-Metadata-Version: 2.1
-Name: avilla-elizabeth
-Version: 1.0.0-alpha.5
-License: MIT
-Author-email: GreyElaina <GreyElaina@outlook.com>
-Requires-Python: >=3.9
-Project-URL: homepage, https://github.com/GraiaProject/Avilla
-Project-URL: repository, https://github.com/GraiaProject/Avilla
-Description-Content-Type: text/markdown
-
-<div align="center">
-
-# Avilla
-
-_The next-gen framework for IM development._
-
-> 即刻动身, 踏上寻找第二个故乡的旅程.
-
-</div>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="code_style" />
-  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" />
-
-</p>
-
-Avilla 是 `Graia Project` 的 "下一代" 框架实现,
-通过对 [ `OneBot` ](https://github.com/botuniverse/onebot), [ `Telegram Bot API` ](https://core.telegram.org/bots) 及其他的基于不同即时通讯软件实现的各式对接接口,
-以及其他具有相应概念的 "异步消息流" 实例进行总结, 抽象其中最为基本的各式模型, 构造了一个理论上可以实现零成本切换对接平台的框架.
-
-**该框架目前处于快速迭代状态, API 可能会发生 _剧烈_ 变化, 可能还不适合进行生产性的开发与运维**
-
-> 项目名称取自日本轻小说 《魔女之旅》 的角色 "艾维莉亚(Avilla)".
-
-|Docs|[![docs](https://img.shields.io/badge/docs%20on-readthedocs-black)](https://graia.readthedocs.io/)|[![docs](https://img.shields.io/badge/docs%20on-netlify-informational)](https://graia.netlify.app/)|[![docs](https://img.shields.io/badge/docs%20on-cloudflare-orange)](https://graia.pages.dev/)|
-|:-:|:-:|:-:|:-:|
-
-## Notable Features
-
- - **原生跨平台**: 开创性的 Relationship 操作模型, 配合最小功能单元, 行为扩展等诸多独特设计, 无论是简单的消息收发还是平台设计的独特交互, Avilla 都能处理地得心应手.
- - **原生多账号**: Avilla 在设计之初, 就考虑了同时管理多个账号, 甚至是多个平台上的多个账号这些问题, 并加以研究与解决. 而现在, 账号管理本应如此简单便捷而收放自如.
- - **一次编写, 多平台可用**: 得益于 Avilla 的强大抽象, 开发者只需面向 Avilla 就能完成核心业务的开发, 显著的减少了维护成本.
- - **平台特性友好**: Avilla 以 Activity, Reaction, Extension 等诸项设计, 使得开发者在运用平台特性的方式更加规范而不失表达性. 担心平台间特性的不通用? 你可以同时为多个平台编写不同的特性用例, Avilla 会自动应用可用的适配, 不改动核心逻辑的同时保证基本特性的可用!
-  > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
- - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
- - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
-
-## Quick Start
-
-```py
-from creart import create
-from graia.amnesia.builtins.aiohttp import AiohttpClientService
-from graia.broadcast import Broadcast
-
-from avilla.core import Avilla, Context, MessageReceived
-from avilla.elizabeth.connection.config import WebsocketClientConfig
-from avilla.elizabeth.protocol import ElizabethProtocol
-
-broadcast = create(Broadcast)
-avilla = Avilla(
-    broadcast, [ElizabethProtocol(WebsocketClientConfig("bot-account", "mah-verify-code"))], [AiohttpClientService()]
-)
-
-
-@broadcast.receiver(MessageReceived)
-async def on_message_received(ctx: Context, event: MessageReceived):
-    if ctx.client.follows("group.member(<master-account>)"):
-        await ctx.scene.send_message("Hello, Avilla!")
-
-
-avilla.launch_manager.launch_blocking(loop=broadcast.loop)
-
-```
-
-## 部件发布情况
-
-|代号|协议|开发进度|PyPI|维护者|开源协议|
-| :-: | :-: | :-: | :-: | :-: | :-: |
-|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |MIT|
-| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |AGPLv3|
-|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official | - |
-|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official | - |
-|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     | - |
-| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official | - |
-
-## 我们的愿景
-
-创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
-助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
-
-## 相关项目
-
-<div align="center">
-
-星座的光芒是由一个个星点共同组成的, 任何优秀的作品都绝不会是一个人的功绩.  
-而若是没有这些项目, Avilla 的实现就无从谈起.  
-排名不分顺序, 可能有许遗漏, 这里仅列出部分较为重要的项目.
-
-</div>
-
-  + [ `Nonebot Team` ](https://github.com/nonebot):
-    - [ `Nonebot v2` ](https://github.com/nonebot/nonebot2): 同样是社区中赫赫有名的优秀框架.
-  + [ `Arclet Project` ](https://github.com/ArcletProject): 在借鉴的基础上, 还进行了难能可贵的优秀创新, 仍在不断成长的框架实现.
-  + [ `Mamoe Technologies` ](https://github.com/mamoe):
-    - [ `mirai` ](https://github.com/mamoe/mirai)
-    - [ `mirai-api-http` ](https://github.com/project-mirai/mirai-api-http)
-  + [ `OneBot Spec` ](https://github.com/botuniverse/onebot): Avilla for OneBot 所依据的实现规范, 同时也是 Avilla Protocol 设计时的参考之一.
-  + [ `go-cqhttp` ](https://github.com/Mrs4s/go-cqhttp): 可能是现在运用最为广泛的 OneBot v11 & v12 实现.
-
-无论如何, Avilla 都是 Graia Project 下的一个子项目, 以下项目均在不同层面上支持了 Avilla 的开发:
-  + [ `Broadcast Control` ](https://github.com/GraiaProject/BroadcastControl): 事件系统实现, 最为锋利的魔剑(Magic Sword).
-  + [ `Ariadne` ](https://github.com/GraiaProject/Ariadne): 继承了前作的衣钵, 在 Avilla 尚未成熟之际撑起大梁的后续作品, 同样进行了可贵的创新.
-
-<div align="center">
-
-衷心感谢这些以及其他未被提及的项目.
-
-</div>
-
-
-## 开源协议
-
-若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
-
+<div align="center">
+
+# Avilla
+
+_The next-gen framework for IM development._
+
+> 即刻动身, 踏上寻找第二个故乡的旅程.
+
+</div>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="code_style" />
+  <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" />
+
+</p>
+
+Avilla 是 `Graia Project` 的 "下一代" 框架实现,
+通过对 [ `OneBot` ](https://github.com/botuniverse/onebot), [ `Telegram Bot API` ](https://core.telegram.org/bots) 及其他的基于不同即时通讯软件实现的各式对接接口,
+以及其他具有相应概念的 "异步消息流" 实例进行总结, 抽象其中最为基本的各式模型, 构造了一个理论上可以实现零成本切换对接平台的框架.
+
+**该框架目前处于快速迭代状态, API 可能会发生 _剧烈_ 变化, 可能还不适合进行生产性的开发与运维**
+
+> 项目名称取自日本轻小说 《魔女之旅》 的角色 "艾维莉亚(Avilla)".
+
+|Docs|[![docs](https://img.shields.io/badge/docs%20on-readthedocs-black)](https://graia.readthedocs.io/)|[![docs](https://img.shields.io/badge/docs%20on-netlify-informational)](https://graia.netlify.app/)|[![docs](https://img.shields.io/badge/docs%20on-cloudflare-orange)](https://graia.pages.dev/)|
+|:-:|:-:|:-:|:-:|
+
+## Notable Features
+
+ - **原生跨平台**: 开创性的 Relationship 操作模型, 配合最小功能单元, 行为扩展等诸多独特设计, 无论是简单的消息收发还是平台设计的独特交互, Avilla 都能处理地得心应手.
+ - **原生多账号**: Avilla 在设计之初, 就考虑了同时管理多个账号, 甚至是多个平台上的多个账号这些问题, 并加以研究与解决. 而现在, 账号管理本应如此简单便捷而收放自如.
+ - **一次编写, 多平台可用**: 得益于 Avilla 的强大抽象, 开发者只需面向 Avilla 就能完成核心业务的开发, 显著的减少了维护成本.
+ - **平台特性友好**: Avilla 以 Activity, Reaction, Extension 等诸项设计, 使得开发者在运用平台特性的方式更加规范而不失表达性. 担心平台间特性的不通用? 你可以同时为多个平台编写不同的特性用例, Avilla 会自动应用可用的适配, 不改动核心逻辑的同时保证基本特性的可用!
+  > 担心可用性? 我们同样提供了一些核心的非平台依赖实现, 例如 `TextCommand`, 这些组件仅要求平台实现最基本的交互实现, 剩下的一切交给 Avilla 处理!
+ - **现有基建兼容**: 得益于 `Amnesia`, `Commander`, `Twilight`, `Alconna` 或是基于 `Launart` 编写的各式扩展, 可以直接与 Avilla 协同而无需任何迁移成本.
+ - **高可伸缩性**: Avilla 既支持单文件使用, 亦支持基于 Graia Saya 驱动的模块系统编写应用.
+
+## Quick Start
+
+```py
+from creart import create
+from graia.amnesia.builtins.aiohttp import AiohttpService
+from graia.broadcast import Broadcast
+
+from avilla.core import Avilla, MessageReceived, Relationship, Selector
+from avilla.elizabeth.connection.config import WebsocketClientConfig
+from avilla.elizabeth.protocol import ElizabethProtocol
+
+broadcast = create(Broadcast)
+avilla = Avilla(broadcast, [
+    ElizabethProtocol(
+        WebsocketClientConfig("bot-account", "mah-verify-code")
+    )
+], [AiohttpService()])
+
+@broadcast.receiver(MessageReceived)
+async def on_message_received(event: MessageReceived, rs: Relationship):
+    if Selector.fragment().as_dyn().group("*").member("master-account").match(rs.ctx):
+        await rs.send_message("Hello, Avilla!")
+
+avilla.launch_manager.launch_blocking(loop=broadcast.loop)
+```
+
+## 部件发布情况
+
+|代号|协议|开发进度|PyPI|维护者|开源协议|
+| :-: | :-: | :-: | :-: | :-: | :-: |
+|      [Core](avilla/core)      |        -         | **Alpha** |       [![image](https://img.shields.io/pypi/v/avilla-core)](https://pypi.org/project/avilla-core)       | Official |MIT|
+| [Elizabeth](avilla/elizabeth) | `mirai-api-http` |  **WIP**  |  [![image](https://img.shields.io/pypi/v/avilla-elizabeth)](https://pypi.org/project/avilla-elizabeth)  | Official |AGPLv3|
+|    [-](avilla/onebot/v11)     |   `OneBot v11`   |  **WIP**  | [![image](https://img.shields.io/pypi/v/avilla-onebot-v11)](https://pypi.org/project/avilla-onebot-v11) | Official | - |
+|    [-](avilla/onebot/v12)     |   `OneBot v12`   | **Draft** | [![image](https://img.shields.io/pypi/v/avilla-onebot-v12)](https://pypi.org/project/avilla-onebot-v12) | Official | - |
+|     [-](avilla/telegram)      |    `Telegram`    | **Draft** |   [![image](https://img.shields.io/pypi/v/avilla-telegram)](https://pypi.org/project/avilla-telegram)   |    -     | - |
+| [Nightcord](avilla/nightcord) |  `Discord Bots`  | **Draft** |  [![image](https://img.shields.io/pypi/v/avilla-nightcord)](https://pypi.org/project/avilla-nightcord)  | Official | - |
+
+## 我们的愿景
+
+创造出比这之前还要更加具有潜力和创造性的作品, 借此有力促进社区的发展,
+助力社区的艺术家们 (Developers & Artists) 以更高的效率, 基于更完善的底层, 创作出更加精彩的作品.
+
+## 相关项目
+
+<div align="center">
+
+星座的光芒是由一个个星点共同组成的, 任何优秀的作品都绝不会是一个人的功绩.  
+而若是没有这些项目, Avilla 的实现就无从谈起.  
+排名不分顺序, 可能有许遗漏, 这里仅列出部分较为重要的项目.
+
+</div>
+
+  + [ `Nonebot Team` ](https://github.com/nonebot):
+    - [ `Nonebot v2` ](https://github.com/nonebot/nonebot2): 同样是社区中赫赫有名的优秀框架.
+  + [ `Arclet Project` ](https://github.com/ArcletProject): 在借鉴的基础上, 还进行了难能可贵的优秀创新, 仍在不断成长的框架实现.
+  + [ `Mamoe Technologies` ](https://github.com/mamoe):
+    - [ `mirai` ](https://github.com/mamoe/mirai)
+    - [ `mirai-api-http` ](https://github.com/project-mirai/mirai-api-http)
+  + [ `OneBot Spec` ](https://github.com/botuniverse/onebot): Avilla for OneBot 所依据的实现规范, 同时也是 Avilla Protocol 设计时的参考之一.
+  + [ `go-cqhttp` ](https://github.com/Mrs4s/go-cqhttp): 可能是现在运用最为广泛的 OneBot v11 & v12 实现.
+
+无论如何, Avilla 都是 Graia Project 下的一个子项目, 以下项目均在不同层面上支持了 Avilla 的开发:
+  + [ `Broadcast Control` ](https://github.com/GraiaProject/BroadcastControl): 事件系统实现, 最为锋利的魔剑(Magic Sword).
+  + [ `Ariadne` ](https://github.com/GraiaProject/Ariadne): 继承了前作的衣钵, 在 Avilla 尚未成熟之际撑起大梁的后续作品, 同样进行了可贵的创新.
+
+<div align="center">
+
+衷心感谢这些以及其他未被提及的项目.
+
+</div>
+
+
+## 开源协议
+
+若非特殊说明, Avilla 及其子包默认使用 MIT 作为开源协议, 但如果你若引用到了使用 GPL/AGPL/LGPL 等具有传染性开源协议的项目, 无论是对 Avilla 实现或是使用了相应 Avilla 实现的项目仍需要遵循相关规则.
```

