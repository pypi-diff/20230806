# Comparing `tmp/nonebot_adapter_onebot-2.2.3.tar.gz` & `tmp/nonebot_adapter_onebot-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_onebot-2.2.3.tar", max compression
+gzip compressed data, was "nonebot_adapter_onebot-2.2.4.tar", max compression
```

## Comparing `nonebot_adapter_onebot-2.2.3.tar` & `nonebot_adapter_onebot-2.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1064 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/LICENSE
--rw-r--r--   0        0        0     3931 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/README.md
--rw-r--r--   0        0        0      657 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/__init__.py
--rw-r--r--   0        0        0     3676 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/collator.py
--rw-r--r--   0        0        0     1040 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/store.py
--rw-r--r--   0        0        0     3087 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/utils.py
--rw-r--r--   0        0        0      721 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/__init__.py
--rw-r--r--   0        0        0    16027 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/adapter.py
--rw-r--r--   0        0        0     7347 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.py
--rw-r--r--   0        0        0    12564 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.pyi
--rw-r--r--   0        0        0      822 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/config.py
--rw-r--r--   0        0        0    13247 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/event.py
--rw-r--r--   0        0        0     1541 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/exception.py
--rw-r--r--   0        0        0     8664 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/helpers.py
--rw-r--r--   0        0        0    10577 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/message.py
--rw-r--r--   0        0        0     2036 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/permission.py
--rw-r--r--   0        0        0     1302 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/utils.py
--rw-r--r--   0        0        0      428 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/__init__.py
--rw-r--r--   0        0        0    24430 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/adapter.py
--rw-r--r--   0        0        0     7506 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.py
--rw-r--r--   0        0        0    15093 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.pyi
--rw-r--r--   0        0        0     1007 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/config.py
--rw-r--r--   0        0        0     8217 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/event.py
--rw-r--r--   0        0        0     6704 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/exception.py
--rw-r--r--   0        0        0     4136 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/message.py
--rw-r--r--   0        0        0      569 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/permission.py
--rw-r--r--   0        0        0     1674 2023-04-27 10:11:01.261117 nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/utils.py
--rw-r--r--   0        0        0     1649 2023-04-27 10:11:01.265124 nonebot_adapter_onebot-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 nonebot_adapter_onebot-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/LICENSE
+-rw-r--r--   0        0        0     3931 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/README.md
+-rw-r--r--   0        0        0      657 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/__init__.py
+-rw-r--r--   0        0        0     3666 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/collator.py
+-rw-r--r--   0        0        0     1040 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/store.py
+-rw-r--r--   0        0        0     3087 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/utils.py
+-rw-r--r--   0        0        0      721 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/__init__.py
+-rw-r--r--   0        0        0    16198 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/adapter.py
+-rw-r--r--   0        0        0     7344 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/bot.py
+-rw-r--r--   0        0        0    12670 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/bot.pyi
+-rw-r--r--   0        0        0      822 2023-08-06 04:27:04.827120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/config.py
+-rw-r--r--   0        0        0    12620 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/event.py
+-rw-r--r--   0        0        0     1541 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/exception.py
+-rw-r--r--   0        0        0     8624 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/helpers.py
+-rw-r--r--   0        0        0     9988 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/message.py
+-rw-r--r--   0        0        0     2036 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/permission.py
+-rw-r--r--   0        0        0     1302 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/utils.py
+-rw-r--r--   0        0        0      428 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/__init__.py
+-rw-r--r--   0        0        0    24894 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/adapter.py
+-rw-r--r--   0        0        0     7503 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/bot.py
+-rw-r--r--   0        0        0    15044 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/bot.pyi
+-rw-r--r--   0        0        0     1007 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/config.py
+-rw-r--r--   0        0        0     8041 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/event.py
+-rw-r--r--   0        0        0     6709 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/exception.py
+-rw-r--r--   0        0        0     4032 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/message.py
+-rw-r--r--   0        0        0      569 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/permission.py
+-rw-r--r--   0        0        0     1649 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/utils.py
+-rw-r--r--   0        0        0     2141 2023-08-06 04:27:04.831120 nonebot_adapter_onebot-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5029 1970-01-01 00:00:00.000000 nonebot_adapter_onebot-2.2.4/PKG-INFO
```

### Comparing `nonebot_adapter_onebot-2.2.3/LICENSE` & `nonebot_adapter_onebot-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/README.md` & `nonebot_adapter_onebot-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/__init__.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/collator.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/collator.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,29 +52,29 @@
                 )
             self.tree[key] = model
 
     def _key_from_dict(self, data: Dict[str, Any]) -> str:
         keys: List[Optional[str]] = []
         for key in self.keys:
             if isinstance(key, tuple):
-                fields = list(filter(None, map(lambda k: data.get(k, None), key)))
+                fields = list(filter(None, (data.get(k, None) for k in key)))
                 if len(fields) > 1:
                     raise ValueError(f"Invalid data with incorrect fields: {fields}")
                 field = fields[0] if fields else None
             else:
                 field = data.get(key)
             keys.append(field)
         return self._generate_key(keys)
 
     def _key_from_model(self, model: Type[E]) -> str:
         keys: List[Optional[str]] = []
         for key in self.keys:
             if isinstance(key, tuple):
                 fields = list(
-                    filter(None, map(lambda k: self._get_model_field(model, k), key))
+                    filter(None, (self._get_model_field(model, k) for k in key))
                 )
                 if len(fields) > 1:
                     raise ValueError(f"Invalid model with incorrect fields: {fields}")
                 field = fields[0] if fields else None
             else:
                 field = self._get_model_field(model, key)
             keys.append(field and self._get_literal_field_default(field))
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/store.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/utils.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/__init__.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/adapter.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     description: onebot.v11.adapter 模块
 """
 import hmac
 import json
 import asyncio
 import inspect
 import contextlib
+from typing_extensions import override
 from typing import Any, Dict, List, Type, Union, Callable, Optional, Generator, cast
 
-from nonebot.typing import overrides
 from nonebot.exception import WebSocketClosed
 from nonebot.utils import DataclassEncoder, escape_tag
 from nonebot.drivers import (
     URL,
     Driver,
     Request,
     Response,
@@ -57,25 +57,25 @@
             ("message_type", "notice_type", "request_type", "meta_event_type"),
             "sub_type",
         ),
     )
 
     _result_store = ResultStore()
 
-    @overrides(BaseAdapter)
+    @override
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.onebot_config: Config = Config(**self.config.dict())
         """OneBot V11 配置"""
         self.connections: Dict[str, WebSocket] = {}
         self.tasks: List["asyncio.Task"] = []
         self._setup()
 
     @classmethod
-    @overrides(BaseAdapter)
+    @override
     def get_name(cls) -> str:
         """适配器名称: `OneBot V11`"""
         return "OneBot V11"
 
     def _setup(self) -> None:
         if isinstance(self.driver, ReverseDriver):
             http_setup = HTTPServerSetup(
@@ -113,21 +113,24 @@
             )
             self.setup_websocket_server(ws_setup)
 
         if self.onebot_config.onebot_ws_urls:
             if not isinstance(self.driver, ForwardDriver):
                 log(
                     "WARNING",
-                    f"Current driver {self.config.driver} don't support forward connections! Ignored",
+                    (
+                        f"Current driver {self.config.driver} does not support "
+                        "forward connections! Ignored"
+                    ),
                 )
             else:
                 self.driver.on_startup(self._start_forward)
                 self.driver.on_shutdown(self._stop_forward)
 
-    @overrides(BaseAdapter)
+    @override
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         websocket = self.connections.get(bot.self_id, None)
         timeout: float = data.get("_timeout", self.config.api_timeout)
         log("DEBUG", f"Calling API <y>{api}</y>")
 
         if websocket:
             seq = self._result_store.get_seq()
@@ -236,15 +239,15 @@
 
         try:
             while True:
                 data = await websocket.receive()
                 json_data = json.loads(data)
                 if event := self.json_to_event(json_data):
                     asyncio.create_task(bot.handle_event(event))
-        except WebSocketClosed as e:
+        except WebSocketClosed:
             log("WARNING", f"WebSocket for Bot {escape_tag(self_id)} closed by peer")
         except Exception as e:
             log(
                 "ERROR",
                 "<r><bg #f8bbd0>Error while process data from websocket "
                 f"for bot {escape_tag(self_id)}.</bg #f8bbd0></r>",
                 e,
@@ -353,16 +356,20 @@
                             "ERROR",
                             "<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
                             e,
                         )
                     except Exception as e:
                         log(
                             "ERROR",
-                            "<r><bg #f8bbd0>Error while process data from websocket"
-                            f"{escape_tag(str(url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                            (
+                                "<r><bg #f8bbd0>"
+                                "Error while process data from websocket"
+                                f"{escape_tag(str(url))}. Trying to reconnect..."
+                                "</bg #f8bbd0></r>"
+                            ),
                             e,
                         )
                     finally:
                         if bot:
                             self.connections.pop(bot.self_id, None)
                             self.bot_disconnect(bot)
                             bot = None
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 FrontMatter:
     sidebar_position: 3
     description: onebot.v11.bot 模块
 """
 
 import re
+from typing_extensions import override
 from typing import Any, Union, Callable
 
-from nonebot.typing import overrides
 from nonebot.message import handle_event
 
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
 from .message import Message, MessageSegment
 from .event import Event, Reply, MessageEvent
@@ -22,15 +22,15 @@
     """检查消息中存在的回复，去除并赋值 `event.reply`, `event.to_me`。
 
     参数:
         bot: Bot 对象
         event: MessageEvent 对象
     """
     try:
-        index = list(map(lambda x: x.type == "reply", event.message)).index(True)
+        index = [x.type == "reply" for x in event.message].index(True)
     except ValueError:
         return
     msg_seg = event.message[index]
     try:
         event.reply = Reply.parse_obj(await bot.get_msg(message_id=msg_seg.data["id"]))
     except Exception as e:
         log("WARNING", f"Error when getting message reply info: {repr(e)}", e)
@@ -189,29 +189,30 @@
             event.message.reduce()
             await _check_reply(self, event)
             _check_at_me(self, event)
             _check_nickname(self, event)
 
         await handle_event(self, event)
 
-    @overrides(BaseBot)
+    @override
     async def send(
         self,
         event: Event,
         message: Union[str, Message, MessageSegment],
         **kwargs: Any,
     ) -> Any:
         """根据 `event` 向触发事件的主体回复消息。
 
         参数:
             event: Event 对象
             message: 要发送的消息
             at_sender (bool): 是否 @ 事件主体
             reply_message (bool): 是否回复事件消息
-            kwargs: 其他参数，可以与 {ref}`nonebot.adapters.onebot.v11.adapter.Adapter.custom_send` 配合使用
+            kwargs: 其他参数，可以与
+                {ref}`nonebot.adapters.onebot.v11.adapter.Adapter.custom_send` 配合使用
 
         返回:
             API 调用返回数据
 
         异常:
             ValueError: 缺少 `user_id`, `group_id`
             NetworkError: 网络错误
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/bot.pyi` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/bot.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any, Dict, List, Union, Optional
+from typing import Any
 
 from nonebot.adapters import Bot as BaseBot
 
 from .event import Event, MessageEvent
 from .message import Message, MessageSegment
 
-async def _check_reply(bot: "Bot", event: MessageEvent): ...
-def _check_at_me(bot: "Bot", event: MessageEvent): ...
-def _check_nickname(bot: "Bot", event: MessageEvent): ...
+async def _check_reply(bot: Bot, event: MessageEvent): ...
+def _check_at_me(bot: Bot, event: MessageEvent): ...
+def _check_nickname(bot: Bot, event: MessageEvent): ...
 async def send(
-    bot: "Bot",
+    bot: Bot,
     event: Event,
-    message: Union[str, Message, MessageSegment],
+    message: str | Message | MessageSegment,
     at_sender: bool = ...,
     reply_message: bool = ...,
     **kwargs: Any,
 ) -> Any: ...
 
 class Bot(BaseBot):
     async def call_api(self, api: str, **data) -> Any:
@@ -39,55 +39,59 @@
     ) -> Any: ...
     async def send_private_msg(
         self,
         *,
         user_id: int,
         message: str | Message,
         auto_escape: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """发送私聊消息。
 
         参数:
             user_id: 对方 QQ 号
             message: 要发送的内容
-            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），只在 `message` 字段是字符串时有效
+            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），
+                只在 `message` 字段是字符串时有效
         """
         ...
     async def send_group_msg(
         self,
         *,
         group_id: int,
         message: str | Message,
         auto_escape: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """发送群消息。
 
         参数:
             group_id: 群号
             message: 要发送的内容
-            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），只在 `message` 字段是字符串时有效
+            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），
+                只在 `message` 字段是字符串时有效
         """
         ...
     async def send_msg(
         self,
         *,
-        message_type: Optional[str] = ...,
-        user_id: Optional[int] = ...,
-        group_id: Optional[int] = ...,
-        message: Union[str, Message],
+        message_type: str | None = ...,
+        user_id: int | None = ...,
+        group_id: int | None = ...,
+        message: str | Message,
         auto_escape: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """发送消息。
 
         参数:
-            message_type: 消息类型，支持 `private`、`group`，分别对应私聊、群组、讨论组，如不传入，则根据传入的 `*_id` 参数判断
+            message_type: 消息类型，支持 `private`、`group`，
+                分别对应私聊、群组、讨论组，如不传入，则根据传入的 `*_id` 参数判断
             user_id: 对方 QQ 号（消息类型为 `private` 时需要）
             group_id: 群号（消息类型为 `group` 时需要）
             message: 要发送的内容
-            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），只在 `message` 字段是字符串时有效
+            auto_escape: 消息内容是否作为纯文本发送（即不解析 CQ 码），
+                只在 `message` 字段是字符串时有效
         """
         ...
     async def delete_msg(
         self,
         *,
         message_id: int,
     ) -> None:
@@ -97,15 +101,15 @@
             message_id: 消息 ID
         """
         ...
     async def get_msg(
         self,
         *,
         message_id: int,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取消息。
 
         参数:
             message_id: 消息 ID
         """
         ...
     async def get_forward_msg(
@@ -162,16 +166,16 @@
             duration: 禁言时长，单位秒，`0` 表示取消禁言
         """
         ...
     async def set_group_anonymous_ban(
         self,
         *,
         group_id: int,
-        anonymous: Optional[Dict[str, Any]] = ...,
-        anonymous_flag: Optional[str] = ...,
+        anonymous: dict[str, Any] | None = ...,
+        anonymous_flag: str | None = ...,
         duration: int = ...,
     ) -> None:
         """群组匿名用户禁言。
 
         参数:
             group_id: 群号
             anonymous: 可选，要禁言的匿名用户对象（群消息上报的 `anonymous` 字段）
@@ -301,152 +305,158 @@
         approve: bool = ...,
         reason: str = ...,
     ) -> None:
         """处理加群请求／邀请。
 
         参数:
             flag: 加群请求的 flag（需从上报的数据中获得）
-            sub_type: `add` 或 `invite`，请求类型（需要和上报消息中的 `sub_type` 字段相符）
+            sub_type: `add` 或 `invite`，
+                请求类型（需要和上报消息中的 `sub_type` 字段相符）
             approve: 是否同意请求／邀请
             reason: 拒绝理由（仅在拒绝时有效）
         """
         ...
-    async def get_login_info(self) -> Dict[str, Any]:
+    async def get_login_info(self) -> dict[str, Any]:
         """获取登录号信息。"""
         ...
     async def get_stranger_info(
         self,
         *,
         user_id: int,
         no_cache: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取陌生人信息。
 
         参数:
             user_id: QQ 号
             no_cache: 是否不使用缓存（使用缓存可能更新不及时，但响应更快）
         """
         ...
-    async def get_friend_list(self) -> List[Dict[str, Any]]:
+    async def get_friend_list(self) -> list[dict[str, Any]]:
         """获取好友列表。"""
         ...
     async def get_group_info(
         self,
         *,
         group_id: int,
         no_cache: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取群信息。
 
         参数:
             group_id: 群号
             no_cache: 是否不使用缓存（使用缓存可能更新不及时，但响应更快）
         """
         ...
-    async def get_group_list(self) -> List[Dict[str, Any]]:
+    async def get_group_list(self) -> list[dict[str, Any]]:
         """获取群列表。"""
         ...
     async def get_group_member_info(
         self,
         *,
         group_id: int,
         user_id: int,
         no_cache: bool = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取群成员信息。
 
         参数:
             group_id: 群号
             user_id: QQ 号
             no_cache: 是否不使用缓存（使用缓存可能更新不及时，但响应更快）
         """
         ...
     async def get_group_member_list(
         self,
         *,
         group_id: int,
-    ) -> List[Dict[str, Any]]:
+    ) -> list[dict[str, Any]]:
         """获取群成员列表。
 
         参数:
             group_id: 群号
         """
         ...
     async def get_group_honor_info(
         self,
         *,
         group_id: int,
         type: str = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取群荣誉信息。
 
         参数:
             group_id: 群号
-            type: 要获取的群荣誉类型，可传入 `talkative` `performer` `legend` `strong_newbie` `emotion` 以分别获取单个类型的群荣誉数据，或传入 `all` 获取所有数据
+            type: 要获取的群荣誉类型，
+                可传入 `talkative` `performer` `legend` `strong_newbie` `emotion`
+                以分别获取单个类型的群荣誉数据，或传入 `all` 获取所有数据
         """
         ...
     async def get_cookies(
         self,
         *,
         domain: str = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取 Cookies。
 
         参数:
             domain: 需要获取 cookies 的域名
         """
         ...
-    async def get_csrf_token(self) -> Dict[str, Any]:
+    async def get_csrf_token(self) -> dict[str, Any]:
         """获取 CSRF Token。"""
         ...
     async def get_credentials(
         self,
         *,
         domain: str = ...,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取 QQ 相关接口凭证。
 
         参数:
             domain: 需要获取 cookies 的域名
         """
         ...
     async def get_record(
         self,
         *,
         file: str,
         out_format: str,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取语音。
 
         参数:
-            file: 收到的语音文件名（CQ 码的 `file` 参数），如 `0B38145AA44505000B38145AA4450500.silk`
-            out_format: 要转换到的格式，目前支持 `mp3`、`amr`、`wma`、`m4a`、`spx`、`ogg`、`wav`、`flac`
+            file: 收到的语音文件名（CQ 码的 `file` 参数），
+                如 `0B38145AA44505000B38145AA4450500.silk`
+            out_format: 要转换到的格式，
+                目前支持 `mp3`、`amr`、`wma`、`m4a`、`spx`、`ogg`、`wav`、`flac`
         """
         ...
     async def get_image(
         self,
         *,
         file: str,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """获取图片。
 
         参数:
-            file: 收到的图片文件名（CQ 码的 `file` 参数），如 `6B4DE3DFD1BD271E3297859D41C530F5.jpg`
+            file: 收到的图片文件名（CQ 码的 `file` 参数），
+                如 `6B4DE3DFD1BD271E3297859D41C530F5.jpg`
         """
         ...
-    async def can_send_image(self) -> Dict[str, Any]:
+    async def can_send_image(self) -> dict[str, Any]:
         """检查是否可以发送图片。"""
         ...
-    async def can_send_record(self) -> Dict[str, Any]:
+    async def can_send_record(self) -> dict[str, Any]:
         """检查是否可以发送语音。"""
         ...
-    async def get_status(self) -> Dict[str, Any]:
+    async def get_status(self) -> dict[str, Any]:
         """获取插件运行状态。"""
         ...
-    async def get_version_info(self) -> Dict[str, Any]:
+    async def get_version_info(self) -> dict[str, Any]:
         """获取版本信息。"""
         ...
     async def set_restart(
         self,
         *,
         delay: int = ...,
     ) -> None:
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/config.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/event.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/event.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 FrontMatter:
     sidebar_position: 4
     description: onebot.v11.event 模块
 """
 
 from copy import deepcopy
+from typing_extensions import override
 from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
 
-from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from pydantic import BaseModel, root_validator
 
 from nonebot.adapters import Event as BaseEvent
 from nonebot.adapters.onebot.utils import highlight_rich_message
 
 from .message import Message
@@ -28,39 +28,39 @@
     [OneBot 文档]: https://github.com/botuniverse/onebot-11/blob/master/README.md
     """
 
     time: int
     self_id: int
     post_type: str
 
-    @overrides(BaseEvent)
+    @override
     def get_type(self) -> str:
         return self.post_type
 
-    @overrides(BaseEvent)
+    @override
     def get_event_name(self) -> str:
         return self.post_type
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(str(self.dict()))
 
-    @overrides(BaseEvent)
+    @override
     def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
-    @overrides(BaseEvent)
+    @override
     def get_user_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    @overrides(BaseEvent)
+    @override
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
 
-    @overrides(BaseEvent)
+    @override
     def is_tome(self) -> bool:
         return False
 
 
 # Models
 class Sender(BaseModel):
     user_id: Optional[int] = None
@@ -145,78 +145,78 @@
 
     @root_validator(pre=True, allow_reuse=True)
     def check_message(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "message" in values:
             values["original_message"] = deepcopy(values["message"])
         return values
 
-    @overrides(Event)
+    @override
     def get_event_name(self) -> str:
         sub_type = getattr(self, "sub_type", None)
         return f"{self.post_type}.{self.message_type}" + (
             f".{sub_type}" if sub_type else ""
         )
 
-    @overrides(Event)
+    @override
     def get_message(self) -> Message:
         return self.message
 
-    @overrides(Event)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(Event)
+    @override
     def get_session_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.to_me
 
 
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     message_type: Literal["private"]
 
-    @overrides(Event)
+    @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.message_id} from {self.user_id} "
             f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
         )
 
 
 class GroupMessageEvent(MessageEvent):
     """群消息"""
 
     message_type: Literal["group"]
     group_id: int
     anonymous: Optional[Anonymous] = None
 
-    @overrides(Event)
+    @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] "
             f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
         )
 
-    @overrides(MessageEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 # Notice Events
 class NoticeEvent(Event):
     """通知事件"""
 
     post_type: Literal["notice"]
     notice_type: str
 
-    @overrides(Event)
+    @override
     def get_event_name(self) -> str:
         sub_type = getattr(self, "sub_type", None)
         return f"{self.post_type}.{self.notice_type}" + (
             f".{sub_type}" if sub_type else ""
         )
 
 
@@ -224,237 +224,237 @@
     """群文件上传事件"""
 
     notice_type: Literal["group_upload"]
     user_id: int
     group_id: int
     file: File
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class GroupAdminNoticeEvent(NoticeEvent):
     """群管理员变动"""
 
     notice_type: Literal["group_admin"]
     sub_type: str
     user_id: int
     group_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class GroupDecreaseNoticeEvent(NoticeEvent):
     """群成员减少事件"""
 
     notice_type: Literal["group_decrease"]
     sub_type: str
     user_id: int
     group_id: int
     operator_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class GroupIncreaseNoticeEvent(NoticeEvent):
     """群成员增加事件"""
 
     notice_type: Literal["group_increase"]
     sub_type: str
     user_id: int
     group_id: int
     operator_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class GroupBanNoticeEvent(NoticeEvent):
     """群禁言事件"""
 
     notice_type: Literal["group_ban"]
     sub_type: str
     user_id: int
     group_id: int
     operator_id: int
     duration: int
 
-    @overrides(NoticeEvent)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class FriendAddNoticeEvent(NoticeEvent):
     """好友添加事件"""
 
     notice_type: Literal["friend_add"]
     user_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return str(self.user_id)
 
 
 class GroupRecallNoticeEvent(NoticeEvent):
     """群消息撤回事件"""
 
     notice_type: Literal["group_recall"]
     user_id: int
     group_id: int
     operator_id: int
     message_id: int
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class FriendRecallNoticeEvent(NoticeEvent):
     """好友消息撤回事件"""
 
     notice_type: Literal["friend_recall"]
     user_id: int
     message_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return str(self.user_id)
 
 
 class NotifyEvent(NoticeEvent):
     """提醒事件"""
 
     notice_type: Literal["notify"]
     sub_type: str
     user_id: int
     group_id: int
 
-    @overrides(NoticeEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(NoticeEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class PokeNotifyEvent(NotifyEvent):
     """戳一戳提醒事件"""
 
     sub_type: Literal["poke"]
     target_id: int
     group_id: Optional[int] = None
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.target_id == self.self_id
 
-    @overrides(NotifyEvent)
+    @override
     def get_session_id(self) -> str:
         if not self.group_id:
             return str(self.user_id)
         return super().get_session_id()
 
 
 class LuckyKingNotifyEvent(NotifyEvent):
     """群红包运气王提醒事件"""
 
     sub_type: Literal["lucky_king"]
     target_id: int
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.target_id == self.self_id
 
-    @overrides(NotifyEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.target_id)
 
-    @overrides(NotifyEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.target_id}"
 
 
 class HonorNotifyEvent(NotifyEvent):
     """群荣誉变更提醒事件"""
 
     sub_type: Literal["honor"]
     honor_type: str
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.user_id == self.self_id
 
 
 # Request Events
 class RequestEvent(Event):
     """请求事件"""
 
     post_type: Literal["request"]
     request_type: str
 
-    @overrides(Event)
+    @override
     def get_event_name(self) -> str:
         sub_type = getattr(self, "sub_type", None)
         return f"{self.post_type}.{self.request_type}" + (
             f".{sub_type}" if sub_type else ""
         )
 
 
@@ -462,19 +462,19 @@
     """加好友请求事件"""
 
     request_type: Literal["friend"]
     user_id: int
     comment: str
     flag: str
 
-    @overrides(RequestEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(RequestEvent)
+    @override
     def get_session_id(self) -> str:
         return str(self.user_id)
 
     async def approve(self, bot: "Bot", remark: str = ""):
         return await bot.set_friend_add_request(
             flag=self.flag, approve=True, remark=remark
         )
@@ -489,19 +489,19 @@
     request_type: Literal["group"]
     sub_type: str
     group_id: int
     user_id: int
     comment: str
     flag: str
 
-    @overrides(RequestEvent)
+    @override
     def get_user_id(self) -> str:
         return str(self.user_id)
 
-    @overrides(RequestEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
     async def approve(self, bot: "Bot"):
         return await bot.set_group_add_request(
             flag=self.flag, sub_type=self.sub_type, approve=True
         )
@@ -515,22 +515,22 @@
 # Meta Events
 class MetaEvent(Event):
     """元事件"""
 
     post_type: Literal["meta_event"]
     meta_event_type: str
 
-    @overrides(Event)
+    @override
     def get_event_name(self) -> str:
         sub_type = getattr(self, "sub_type", None)
         return f"{self.post_type}.{self.meta_event_type}" + (
             f".{sub_type}" if sub_type else ""
         )
 
-    @overrides(Event)
+    @override
     def get_log_string(self) -> str:
         raise NoLogException
 
 
 class LifecycleMetaEvent(MetaEvent):
     """生命周期元事件"""
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/exception.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/helpers.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from asyncio import get_running_loop
 from typing import Any, Dict, List, Union, Optional, DefaultDict
 
 from nonebot.matcher import Matcher
 from nonebot.params import Depends, EventMessage
 
 from .bot import Bot
+from .event import Event
 from .message import Message, MessageSegment
-from .event import Event, MessageEvent, GroupMessageEvent
 
 
 def extract_image_urls(message: Message) -> List[str]:
     """提取消息中的图片链接
 
     参数:
         message: 消息对象
@@ -303,16 +303,16 @@
         bot: 实例化的Bot类
         event: 事件对象
         message: 消息对象或消息文本
         at_sender: 是否在消息中添加 @ 用户
         revoke_interval: 撤回消息的间隔时间, 单位为秒
 
     返回:
-        asyncio.TimerHandle: [`TimerHandle`](https://docs.python.org/zh-cn/3/library/asyncio-eventloop.html#asyncio.TimerHandle) 对象, 可以用来取消定时撤回任务
-    """
+        [`TimerHandle`](https://docs.python.org/zh-cn/3/library/asyncio-eventloop.html#asyncio.TimerHandle) 对象, 可以用来取消定时撤回任务
+    """  # noqa: E501
     message_data: Dict[str, Any] = await bot.send(
         event, message, at_sender=at_sender, **kwargs
     )
     message_id: int = message_data["message_id"]
 
     loop = get_running_loop()
     return loop.call_later(
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/permission.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v11/utils.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v11/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/adapter.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     sidebar_position: 1
     description: onebot.v12.adapter 模块
 """
 import json
 import asyncio
 import inspect
 import contextlib
+from typing_extensions import override
 from typing import (
     Any,
     Dict,
     List,
     Type,
     Union,
     Callable,
@@ -19,15 +20,14 @@
     Optional,
     Generator,
     cast,
 )
 
 import msgpack
 from pygtrie import CharTrie
-from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from nonebot.exception import WebSocketClosed
 from nonebot.drivers import (
     URL,
     Driver,
     Request,
     Response,
@@ -89,19 +89,19 @@
     exc_classes: ClassVar[CharTrie] = CharTrie(
         (retcode, Exc) for Exc in DEFAULT_EXCEPTIONS for retcode in Exc.__retcode__
     )
 
     _result_store: ClassVar[ResultStore] = ResultStore()
 
     @classmethod
-    @overrides(BaseAdapter)
+    @override
     def get_name(cls) -> str:
         return "OneBot V12"
 
-    @overrides(BaseAdapter)
+    @override
     def __init__(self, driver: Driver, **kwargs: Any) -> None:
         super().__init__(driver, **kwargs)
         self.onebot_config: Config = Config(**self.config.dict())
         self.connections: Dict[str, WebSocket] = {}
         self.tasks: List["asyncio.Task"] = []
         self._setup()
 
@@ -148,21 +148,24 @@
                     self._handle_ws,
                 )
             )
         if self.onebot_config.onebot_ws_urls:
             if not isinstance(self.driver, ForwardDriver):
                 log(
                     "WARNING",
-                    f"Current driver {self.config.driver} don't support forward connections! Ignored",
+                    (
+                        f"Current driver {self.config.driver} does not support "
+                        "forward connections! Ignored"
+                    ),
                 )
             else:
                 self.driver.on_startup(self._start_forward)
                 self.driver.on_shutdown(self._stop_forward)
 
-    @overrides(BaseAdapter)
+    @override
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         websocket = self.connections.get(bot.self_id)
         timeout: float = data.get("_timeout", self.config.api_timeout)
         log("DEBUG", f"Calling API <y>{api}</y>")
 
         action_data = {
             "action": api,
@@ -360,19 +363,22 @@
                         if not bot:
                             bot = Bot(self, self_id, impl, event.self.platform)
                             self.bot_connect(bot)
                             bots[self_id] = bot
                             self.connections[self_id] = websocket
                             log(
                                 "INFO",
-                                f"<y>Bot {escape_tag(event.self.user_id)}</y> connected",
+                                (
+                                    f"<y>Bot {escape_tag(event.self.user_id)}</y> "
+                                    "connected"
+                                ),
                             )
                         asyncio.create_task(bot.handle_event(event))
 
-        except WebSocketClosed as e:
+        except WebSocketClosed:
             self_id = ", ".join(bots)
             log("WARNING", f"WebSocket for Bot {escape_tag(self_id)} closed by peer")
         except Exception as e:
             self_id = ", ".join(bots)
             log(
                 "ERROR",
                 "<r><bg #f8bbd0>Error while process data from websocket "
@@ -479,28 +485,36 @@
                                 if not bot:
                                     bot = Bot(self, self_id, impl, event.self.platform)
                                     self.bot_connect(bot)
                                     bots[self_id] = bot
                                     self.connections[self_id] = ws
                                     log(
                                         "INFO",
-                                        f"<y>Bot {escape_tag(event.self.user_id)}</y> connected",
+                                        (
+                                            "<y>"
+                                            f"Bot {escape_tag(event.self.user_id)}"
+                                            "</y> connected"
+                                        ),
                                     )
                                 asyncio.create_task(bot.handle_event(event))
                     except WebSocketClosed as e:
                         log(
                             "ERROR",
                             "<r><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></r>",
                             e,
                         )
                     except Exception as e:
                         log(
                             "ERROR",
-                            "<r><bg #f8bbd0>Error while process data from websocket"
-                            f"{escape_tag(str(url))}. Trying to reconnect...</bg #f8bbd0></r>",
+                            (
+                                "<r><bg #f8bbd0>"
+                                "Error while process data from websocket"
+                                f"{escape_tag(str(url))}. Trying to reconnect..."
+                                "</bg #f8bbd0></r>"
+                            ),
                             e,
                         )
                     finally:
                         for self_id, bot in bots.items():
                             self.connections.pop(self_id, None)
                             self.bot_disconnect(bot)
                         bots.clear()
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 FrontMatter:
     sidebar_position: 3
     description: onebot.v12.bot 模块
 """
 
 import re
+from typing_extensions import override
 from typing import TYPE_CHECKING, Any, Union
 
-from nonebot.typing import overrides
 from nonebot.message import handle_event
 
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
 from .message import Message, MessageSegment
 from .event import Event, Reply, MessageEvent
@@ -25,15 +25,15 @@
     """检查消息中存在的回复，去除并赋值 `event.reply`, `event.to_me`。
 
     参数:
         bot: Bot 对象
         event: MessageEvent 对象
     """
     try:
-        index = list(map(lambda x: x.type == "reply", event.message)).index(True)
+        index = [x.type == "reply" for x in event.message].index(True)
     except ValueError:
         return
 
     msg_seg = event.message[index]
 
     try:
         event.reply = Reply.parse_obj(msg_seg.data)
@@ -197,26 +197,27 @@
         if isinstance(event, MessageEvent):
             event.message.reduce()
             _check_reply(self, event)
             _check_to_me(self, event)
             _check_nickname(self, event)
         await handle_event(self, event)
 
-    @overrides(BaseBot)
+    @override
     async def send(
         self, event: Event, message: Union[str, Message, MessageSegment], **kwargs: Any
     ) -> Any:
         """根据 `event` 向触发事件的主体回复消息。
 
         参数:
             event: Event 对象
             message: 要发送的消息
             at_sender (bool): 是否 @ 事件主体
             reply_message (bool): 是否回复事件消息
-            kwargs: 其他参数，可以与 {ref}`nonebot.adapters.onebot.v12.adapter.Adapter.custom_send` 配合使用
+            kwargs: 其他参数，可以与
+                {ref}`nonebot.adapters.onebot.v12.adapter.Adapter.custom_send` 配合使用
 
         返回:
             API 调用返回数据
 
         异常:
             ValueError: 缺少 `user_id`, `group_id`
             NetworkError: 网络错误
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/bot.pyi` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/bot.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Union, Literal, Optional, TypedDict, overload
+from typing import Any, Literal, TypedDict, overload
 
 from nonebot.adapters import Bot as BaseBot
 
 from .adapter import Adapter
 from .event import Event as EventModel
 from .message import Message, MessageSegment
 from .event import MessageEvent as MessageEventModel
@@ -20,15 +20,15 @@
 
 class BotStatus(TypedDict):
     self: BotSelf
     online: bool
 
 class GetStatusResp(TypedDict):
     good: str
-    bots: List[BotStatus]
+    bots: list[BotStatus]
 
 class GetVersionResp(TypedDict):
     impl: str
     version: str
     onebot_version: str
 
 class SendMessageResp(TypedDict):
@@ -78,42 +78,42 @@
 
 class UploadFileFragmentedResp(TypedDict):
     file_id: str
 
 class GetFileUrlResp(TypedDict):
     name: str
     url: str
-    headers: Optional[Dict[str, str]]
-    sha256: Optional[str]
+    headers: dict[str, str] | None
+    sha256: str | None
 
 class GetFilePathResp(TypedDict):
     name: str
     path: str
-    sha256: Optional[str]
+    sha256: str | None
 
 class GetFileDataResp(TypedDict):
     name: str
-    data: Union[str, bytes]
-    sha256: Optional[str]
+    data: str | bytes
+    sha256: str | None
 
 class GetFileFragmentedPrepareResp(TypedDict):
     name: str
     total_size: int
     sha256: str
 
 class GetFileFragmentedTransferResp(TypedDict):
-    data: Union[str, bytes]
+    data: str | bytes
 
-def _check_reply(bot: "Bot", event: MessageEventModel): ...
-def _check_to_me(bot: "Bot", event: MessageEventModel): ...
-def _check_nickname(bot: "Bot", event: MessageEventModel): ...
+def _check_reply(bot: Bot, event: MessageEventModel): ...
+def _check_to_me(bot: Bot, event: MessageEventModel): ...
+def _check_nickname(bot: Bot, event: MessageEventModel): ...
 async def send(
-    bot: "Bot",
+    bot: Bot,
     event: EventModel,
-    message: Union[str, Message, MessageSegment],
+    message: str | Message | MessageSegment,
     at_sender: bool = ...,
     reply_message: bool = ...,
     **kwargs: Any,
 ) -> Any: ...
 
 class Bot(BaseBot):
     impl: str
@@ -138,24 +138,24 @@
         ...
     async def handle_event(self, event: EventModel) -> None: ...
     async def send(
         self, event: EventModel, message: str | Message | MessageSegment, **kwargs: Any
     ) -> Any: ...
     async def get_latest_events(
         self, *, limit: int = ..., timeout: int = ..., **kwargs: Any
-    ) -> List[Event]:
+    ) -> list[Event]:
         """获取最新事件列表
 
         参数:
             limit: 获取的事件数量上限，0 表示不限制
             timeout: 没有事件时要等待的秒数，0 表示使用短轮询，不等待
             kwargs: 扩展字段
         """
         ...
-    async def get_supported_actions(self, **kwargs: Any) -> List[str]:
+    async def get_supported_actions(self, **kwargs: Any) -> list[str]:
         """获取支持的动作列表
 
         参数:
             kwargs: 扩展字段
         """
         ...
     async def get_status(self, **kwargs: Any) -> GetStatusResp:
@@ -182,15 +182,16 @@
         channel_id: str = ...,
         message: Message,
         **kwargs: Any,
     ) -> SendMessageResp:
         """发送消息
 
         参数:
-            detail_type: 发送的类型，可以为 private、group 或扩展的类型，和消息事件的 detail_type 字段对应
+            detail_type: 发送的类型，
+                可以为 private、group 或扩展的类型，和消息事件的 detail_type 字段对应
             user_id: 用户 ID，当 detail_type 为 private 时必须传入
             group_id: 群 ID，当 detail_type 为 group 时必须传入
             guild_id: Guild 群组 ID，当 detail_type 为 channel 时必须传入
             channel_id: 频道 ID，当 detail_type 为 channel 时必须传入
             message: 消息内容
             kwargs: 扩展字段
         """
@@ -209,30 +210,30 @@
         """获取用户信息
 
         参数:
             user_id: 用户 ID，可以是好友，也可以是陌生人
             kwargs: 扩展字段
         """
         ...
-    async def get_friend_list(self, **kwargs: Any) -> List[GetUserInfoResp]:
+    async def get_friend_list(self, **kwargs: Any) -> list[GetUserInfoResp]:
         """获取好友列表
 
         参数:
             kwargs: 扩展字段
         """
         ...
     async def get_group_info(self, *, group_id: str, **kwargs: Any) -> GetGroupInfoResp:
         """获取群信息
 
         参数:
             group_id: 群 ID
             kwargs: 扩展字段
         """
         ...
-    async def get_group_list(self, **kwargs: Any) -> List[GetGroupInfoResp]:
+    async def get_group_list(self, **kwargs: Any) -> list[GetGroupInfoResp]:
         """获取群列表
 
         参数:
             kwargs: 扩展字段
         """
         ...
     async def get_group_member_info(
@@ -244,15 +245,15 @@
             group_id: 群 ID
             user_id: 用户 ID
             kwargs: 扩展字段
         """
         ...
     async def get_group_member_list(
         self, *, group_id: str, **kwargs: Any
-    ) -> List[GetGroupMemberInfoResp]:
+    ) -> list[GetGroupMemberInfoResp]:
         """获取群成员列表
 
         参数:
             group_id: 群 ID
             kwargs: 扩展字段
         """
         ...
@@ -279,15 +280,15 @@
         """获取 Guild 信息
 
         参数:
             guild_id: 群组 ID
             kwargs: 扩展字段
         """
         ...
-    async def get_guild_list(self, **kwargs: Any) -> List[GetGuildInfoResp]:
+    async def get_guild_list(self, **kwargs: Any) -> list[GetGuildInfoResp]:
         """获取群组列表
 
         参数:
             kwargs: 扩展字段
         """
         ...
     async def set_guild_name(
@@ -310,15 +311,15 @@
             guild_id: 群组 ID
             user_id: 用户 ID
             kwargs: 扩展字段
         """
         ...
     async def get_guild_member_list(
         self, *, guild_id: str, **kwargs: Any
-    ) -> List[GetGuildMemberInfoResp]:
+    ) -> list[GetGuildMemberInfoResp]:
         """获取群组成员列表
 
         参数:
             guild_id: 群组 ID
             kwargs: 扩展字段
         """
         ...
@@ -339,15 +340,15 @@
             guild_id: 群组 ID
             channel_id: 频道 ID
             kwargs: 扩展字段
         """
         ...
     async def get_channel_list(
         self, *, guild_id: str, joined_only: bool = False, **kwargs: Any
-    ) -> List[GetChannelInfoResp]:
+    ) -> list[GetChannelInfoResp]:
         """获取频道列表
 
         参数:
             guild_id: 群组 ID
             joined_only: 只获取机器人账号已加入的频道列表
             kwargs: 扩展字段
         """
@@ -374,15 +375,15 @@
             channel_id: 频道 ID
             user_id: 用户 ID
             kwargs: 扩展字段
         """
         ...
     async def get_channel_member_list(
         self, *, guild_id: str, channel_id: str, **kwargs: Any
-    ) -> List[GetChannelMemberInfoResp]:
+    ) -> list[GetChannelMemberInfoResp]:
         """获取频道成员列表
 
         参数:
             guild_id: 群组 ID
             channel_id: 频道 ID
             kwargs: 扩展字段
         """
@@ -400,15 +401,15 @@
         ...
     async def upload_file(
         self,
         *,
         type: Literal["url", "path", "data"] | str,
         name: str,
         url: str = ...,
-        headers: Dict[str, str] = ...,
+        headers: dict[str, str] = ...,
         path: str = ...,
         data: bytes = ...,
         sha256: str = ...,
         **kwargs: Any,
     ) -> UploadFileResp:
         """上传文件
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/config.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/event.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 FrontMatter:
     sidebar_position: 4
     description: onebot.v12.event 模块
 """
 
 from copy import deepcopy
 from datetime import datetime
+from typing_extensions import override
 from typing import Any, Dict, List, Literal, Optional
 
-from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 from pydantic import Extra, BaseModel, root_validator
 
 from nonebot.adapters import Event as BaseEvent
 from nonebot.adapters.onebot.utils import highlight_rich_message
 
 from .message import Message
@@ -28,39 +28,39 @@
 
     id: str
     time: datetime
     type: Literal["message", "notice", "request", "meta"]
     detail_type: str
     sub_type: str
 
-    @overrides(BaseEvent)
+    @override
     def get_type(self) -> str:
         return self.type
 
-    @overrides(BaseEvent)
+    @override
     def get_event_name(self) -> str:
         return ".".join(filter(None, (self.type, self.detail_type, self.sub_type)))
 
-    @overrides(BaseEvent)
+    @override
     def get_event_description(self) -> str:
         return escape_tag(str(self.dict()))
 
-    @overrides(BaseEvent)
+    @override
     def get_message(self) -> Message:
         raise ValueError("Event has no message!")
 
-    @overrides(BaseEvent)
+    @override
     def get_user_id(self) -> str:
         raise ValueError("Event has no user_id!")
 
-    @overrides(BaseEvent)
+    @override
     def get_session_id(self) -> str:
         raise ValueError("Event has no session_id!")
 
-    @overrides(BaseEvent)
+    @override
     def is_tome(self) -> bool:
         return False
 
 
 class BotSelf(BaseModel, extra=Extra.allow):
     """机器人自身标识"""
 
@@ -119,70 +119,70 @@
 
     @root_validator(pre=True, allow_reuse=True)
     def check_message(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "message" in values:
             values["original_message"] = deepcopy(values["message"])
         return values
 
-    @overrides(Event)
+    @override
     def get_message(self) -> Message:
         return self.message
 
-    @overrides(Event)
+    @override
     def get_user_id(self) -> str:
         return self.user_id
 
-    @overrides(Event)
+    @override
     def get_session_id(self) -> str:
         return self.user_id
 
-    @overrides(Event)
+    @override
     def is_tome(self) -> bool:
         return self.to_me
 
 
 class PrivateMessageEvent(MessageEvent):
     """私聊消息"""
 
     detail_type: Literal["private"]
 
-    @overrides(Event)
+    @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.message_id} from {self.user_id} "
             f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
         )
 
 
 class GroupMessageEvent(MessageEvent):
     """群消息"""
 
     detail_type: Literal["group"]
     group_id: str
 
-    @overrides(Event)
+    @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.message_id} from {self.user_id}@[群:{self.group_id}] "
             f"{''.join(highlight_rich_message(repr(self.original_message.to_rich_text())))}"
         )
 
-    @overrides(MessageEvent)
+    @override
     def get_session_id(self) -> str:
         return f"group_{self.group_id}_{self.user_id}"
 
 
 class ChannelMessageEvent(MessageEvent):
     """频道消息"""
 
     detail_type: Literal["channel"]
     guild_id: str
     channel_id: str
 
-    @overrides(Event)
+    @override
     def get_event_description(self) -> str:
         texts: List[str] = []
         msg_string: List[str] = []
         for seg in self.original_message:
             if seg.is_text():
                 texts.append(str(seg))
             else:
@@ -192,15 +192,15 @@
                 texts.clear()
         msg_string.append(escape_tag("".join(texts)))
         return (
             f"Message {self.message_id} from {self.user_id}@"
             f"[群组:{self.guild_id}, 频道:{self.channel_id}] {''.join(msg_string)!r}"
         )
 
-    @overrides(MessageEvent)
+    @override
     def get_session_id(self) -> str:
         return f"guild_{self.guild_id}_channel_{self.channel_id}_{self.user_id}"
 
 
 class NoticeEvent(BotEvent):
     """通知事件"""
 
@@ -333,15 +333,15 @@
 
 # Meta Events
 class MetaEvent(Event):
     """元事件"""
 
     type: Literal["meta"]
 
-    @overrides(Event)
+    @override
     def get_log_string(self) -> str:
         raise NoLogException
 
 
 class ImplVersion(BaseModel, extra=Extra.allow):
     impl: str
     version: str
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/exception.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,16 @@
 
 
 class WhoAmI(RequestError):
     """未指定机器人账号。
 
     OneBot V12 协议错误码: 10101。
 
-    OneBot 实现在单个 OneBot Connect 连接上支持多个机器人账号，但动作请求未指定要使用的账号。
+    OneBot 实现在单个 OneBot Connect 连接上支持多个机器人账号，
+    但动作请求未指定要使用的账号。
     """
 
     __retcode__ = ("10101",)
 
 
 class UnknownSelf(RequestError):
     """未知的机器人账号。
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/message.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,32 @@
 
 FrontMatter:
     sidebar_position: 5
     description: onebot.v12.message 模块
 """
 
 from functools import partial
+from typing_extensions import override
 from typing import Any, Type, Iterable, Optional
 
-from nonebot.typing import overrides
-
 from nonebot.adapters import Message as BaseMessage
 from nonebot.adapters.onebot.utils import rich_escape
 from nonebot.adapters.onebot.utils import truncate as trunc
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
 
 class MessageSegment(BaseMessageSegment["Message"]):
     """OneBot v12 协议 MessageSegment 适配。具体方法参考协议消息段类型或源码。"""
 
     @classmethod
-    @overrides(BaseMessageSegment)
+    @override
     def get_message_class(cls) -> Type["Message"]:
         return Message
 
-    @overrides(BaseMessageSegment)
+    @override
     def __str__(self) -> str:
         return self.to_rich_text(truncate=None)
 
     def to_rich_text(self, truncate: Optional[int] = 70) -> str:
         if self.is_text():
             return rich_escape(self.data.get("text", ""), escape_comma=False)
 
@@ -37,15 +36,15 @@
         params = ", ".join(
             f"{k}={rich_escape(truncate_func(str(v)))}"
             for k, v in self.data.items()
             if v is not None
         )
         return f"[{self.type}{':' if params else ''}{params}]"
 
-    @overrides(BaseMessageSegment)
+    @override
     def is_text(self) -> bool:
         return self.type == "text"
 
     @staticmethod
     def text(text: str, **kwargs) -> "MessageSegment":
         return MessageSegment("text", {**kwargs, "text": text})
 
@@ -99,27 +98,27 @@
     @staticmethod
     def reply(message_id: str, **kwargs: Any) -> "MessageSegment":
         return MessageSegment("reply", {**kwargs, "message_id": message_id})
 
 
 class Message(BaseMessage[MessageSegment]):
     @classmethod
-    @overrides(BaseMessage)
+    @override
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
     def to_rich_text(self, truncate: Optional[int] = 70) -> str:
         return "".join(seg.to_rich_text(truncate=truncate) for seg in self)
 
     @staticmethod
-    @overrides(BaseMessage)
+    @override
     def _construct(msg: str) -> Iterable[MessageSegment]:
         yield MessageSegment.text(msg)
 
-    @overrides(BaseMessage)
+    @override
     def extract_plain_text(self) -> str:
         return "".join(seg.data["text"] for seg in self if seg.is_text())
 
     def reduce(self) -> None:
         index = 1
         while index < len(self):
             if self[index - 1].type == "text" and self[index].type == "text":
```

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/permission.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_onebot-2.2.3/nonebot/adapters/onebot/v12/utils.py` & `nonebot_adapter_onebot-2.2.4/nonebot/adapters/onebot/v12/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     description: onebot.v12.utils 模块
 """
 
 import datetime
 from typing import TypeVar
 from base64 import b64encode
 from functools import partial
+from typing_extensions import override
 
-from nonebot.typing import overrides
 from pydantic.json import custom_pydantic_encoder
 from nonebot.utils import DataclassEncoder, logger_wrapper
 
 T = TypeVar("T")
 
 
 log = logger_wrapper("OneBot V12")
@@ -41,24 +41,27 @@
         return [flattened_to_nested(item) for item in data]  # type: ignore
     return data
 
 
 class CustomEncoder(DataclassEncoder):
     """OneBot V12 使用的 `JSONEncoder`"""
 
-    @overrides(DataclassEncoder)
+    @override
     def default(self, o):
         if isinstance(o, bytes):
             return b64encode(o).decode()
-        return super(CustomEncoder, self).default(o)
+        return super().default(o)
 
 
 def timestamp(obj: datetime.datetime):
     return obj.timestamp()
 
 
 # https://12.onebot.dev/connect/data-protocol/basic-types/
 msgpack_type_encoders = {
     datetime.datetime: timestamp,
 }
 
-msgpack_encoder = partial(custom_pydantic_encoder, msgpack_type_encoders)  # type: ignore
+msgpack_encoder = partial(
+    custom_pydantic_encoder,
+    msgpack_type_encoders,  # type: ignore
+)
```

### Comparing `nonebot_adapter_onebot-2.2.3/pyproject.toml` & `nonebot_adapter_onebot-2.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [tool.poetry]
 name = "nonebot-adapter-onebot"
-version = "2.2.3"
+version = "2.2.4"
 description = "OneBot(CQHTTP) adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://adapter-onebot.netlify.app/"
 repository = "https://github.com/nonebot/adapter-onebot"
 documentation = "https://adapter-onebot.netlify.app/"
 keywords = ["bot", "qq", "qqbot", "coolq", "onebot", "cqhttp"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Library",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3"
-]
-packages = [
-  { include = "nonebot" }
+  "Programming Language :: Python :: 3",
 ]
+packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 msgpack = "^1.0.3"
 nonebot2 = "^2.0.0-beta.3"
+typing-extensions = ">=4.0.0,<5.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pycln = "^2.1.3"
 isort = "^5.10.1"
 black = "^23.1.0"
+ruff = "^0.0.282"
 nonebug = "^0.3.0"
 nonemoji = "^0.1.2"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.2.0"
 pytest-asyncio = "^0.21.0"
 nb-autodoc = "^1.0.0a5"
-nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = ["fastapi"] }
+nonebot2 = { git = "https://github.com/nonebot/nonebot2.git", branch = "master", extras = [
+  "fastapi",
+] }
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 addopts = "--cov nonebot.adapters.onebot --cov-report term-missing"
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310", "py311"]
 include = '\.pyi?$'
 extend-exclude = '''
@@ -52,14 +52,27 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
-[tool.pycln]
-path = "."
-all = false
+[tool.ruff]
+select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q"]
+ignore = ["E402", "C901", "UP037", "PYI021"]
+
+line-length = 88
+target-version = "py38"
+
+[tool.ruff.per-file-ignores]
+"nonebot/adapters/onebot/__init__.py" = ["F401"]
+"nonebot/adapters/onebot/v11/__init__.py" = ["F403"]
+"nonebot/adapters/onebot/v12/__init__.py" = ["F403"]
+"packages/nonebot-adapter-cqhttp/nonebot/adapters/cqhttp/__init__.py" = ["F403"]
+
+[tool.ruff.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_adapter_onebot-2.2.3/PKG-INFO` & `nonebot_adapter_onebot-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-onebot
-Version: 2.2.3
+Version: 2.2.4
 Summary: OneBot(CQHTTP) adapter for nonebot2
 Home-page: https://adapter-onebot.netlify.app/
 License: MIT
 Keywords: bot,qq,qqbot,coolq,onebot,cqhttp
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -14,17 +14,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.3,<3.0.0)
+Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://adapter-onebot.netlify.app/
 Project-URL: Repository, https://github.com/nonebot/adapter-onebot
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://onebot.adapters.nonebot.dev/">
     <picture>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-onebot Version: 2.2.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-onebot Version: 2.2.4 Summary:
 OneBot(CQHTTP) adapter for nonebot2 Home-page: https://adapter-
 onebot.netlify.app/ License: MIT Keywords: bot,qq,qqbot,coolq,onebot,cqhttp
 Author: yanyongyu Author-email: yyy@nonebot.dev Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Robot Framework Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Requires-Dist: msgpack (>=1.0.3,<2.0.0) Requires-Dist: nonebot2
-(>=2.0.0-beta.3,<3.0.0) Project-URL: Documentation, https://adapter-
+Programming Language :: Python :: 3.11 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
+Requires-Dist: nonebot2 (>=2.0.0-beta.3,<3.0.0) Requires-Dist: typing-
+extensions (>=4.0.0,<5.0.0) Project-URL: Documentation, https://adapter-
 onebot.netlify.app/ Project-URL: Repository, https://github.com/nonebot/
 adapter-onebot Description-Content-Type: text/markdown
                           __[nonebot-adapter-onebot]_
            # NoneBot-Adapter-OneBot   _â¨ OneBot åè®®éé â¨_
 [license] [pypi] [python] [https://codecov.io/gh/nonebot/adapter-onebot/branch/
 master/graph/badge.svg?token=45OH1IVM9C] [site] [https://results.pre-commit.ci/
                badge/github/nonebot/adapter-onebot/master.svg]
```

