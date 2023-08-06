# Comparing `tmp/graia-amnesia-0.7.1.tar.gz` & `tmp/graia_amnesia-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia-amnesia-0.7.1.tar", last modified: Mon Dec 12 15:04:14 2022, max compression
+gzip compressed data, was "graia_amnesia-0.8.0.tar", last modified: Sun Aug  6 13:52:36 2023, max compression
```

## Comparing `graia-amnesia-0.7.1.tar` & `graia_amnesia-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,15 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-12 15:03:50.441705 graia-amnesia-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-12 15:03:50.441705 graia-amnesia-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19876 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/builtins/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/builtins/memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/builtins/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/builtins/uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/backend/orjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/backend/std.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/backend/ujson.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/json/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/message/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/message/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/http/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/http/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/http/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/websocket/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/websocket/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/websocket/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/common/websocket/shortcut.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/rider.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/transport/utilles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-12 15:03:50.445704 graia-amnesia-0.7.1/src/graia/amnesia/utilles.py
--rw-------   0 runner    (1001) docker     (123)     2191 2022-12-12 15:04:14.693645 graia-amnesia-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 13:52:25.327967 graia_amnesia-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1804 2023-08-06 13:52:25.327967 graia_amnesia-0.8.0/README.md
+-rw-r--r--   0        0        0      631 2023-08-06 13:52:36.500010 graia_amnesia-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/__init__.py
+-rw-r--r--   0        0        0     3337 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/__init__.py
+-rw-r--r--   0        0        0     6238 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/asgitypes.py
+-rw-r--r--   0        0        0     2800 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/asgi/middleware.py
+-rw-r--r--   0        0        0     2539 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/builtins/memcache.py
+-rw-r--r--   0        0        0      276 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/__init__.py
+-rw-r--r--   0        0        0    19775 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/chain.py
+-rw-r--r--   0        0        0     2078 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/element.py
+-rw-r--r--   0        0        0     2222 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/message/formatter.py
+-rw-r--r--   0        0        0     2539 2023-08-06 13:52:25.331967 graia_amnesia-0.8.0/src/graia/amnesia/utilles.py
+-rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 graia_amnesia-0.8.0/PKG-INFO
```

### Comparing `graia-amnesia-0.7.1/LICENSE` & `graia_amnesia-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graia-amnesia-0.7.1/README.md` & `graia_amnesia-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `graia-amnesia-0.7.1/src/graia/amnesia/builtins/memcache.py` & `graia_amnesia-0.8.0/src/graia/amnesia/builtins/memcache.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 from datetime import timedelta
 from heapq import heappop, heappush
 from time import time
 from typing import Any
 
 from launart import Launart, Service
 
-from graia.amnesia.transport.common.storage import CacheStorage
 
-
-class Memcache(CacheStorage[Any]):
+class Memcache:
     cache: dict[str, tuple[float | None, Any]]
     expire: list[tuple[float, str]]
 
     def __init__(
         self,
         cache: dict[str, tuple[float | None, Any]],
         expire: list[tuple[float, str]],
@@ -52,42 +50,42 @@
 
     async def keys(self) -> list[str]:
         return list(self.cache.keys())
 
 
 class MemcacheService(Service):
     id = "cache.client/memcache"
-    supported_interface_types = {Memcache}, {CacheStorage: 10}
 
     interval: float
-    cache: dict[str, tuple[float | None, Any]]
+    _cache: dict[str, tuple[float | None, Any]]
     expire: list[tuple[float, str]]
 
     def __init__(
         self,
         interval: float = 0.1,
         cache: dict[str, tuple[float | None, Any]] | None = None,
         expire: list[tuple[float, str]] | None = None,
     ):
         self.interval = interval
-        self.cache = cache or {}
+        self._cache = cache or {}
         self.expire = expire or []
         super().__init__()
 
-    def get_interface(self, _) -> Memcache:
-        return Memcache(self.cache, self.expire)
-
     @property
     def required(self):
         return set()
 
     @property
     def stages(self):
         return {"blocking"}
 
+    @property
+    def cache(self):
+        return Memcache(self._cache, self.expire)
+
     async def launch(self, manager: Launart) -> None:
         async with self.stage("blocking"):
             while not manager.status.exiting:
                 while self.expire and self.expire[0][0] <= time():
                     _, key = heappop(self.expire)
-                    self.cache.pop(key, None)
+                    self._cache.pop(key, None)
                 await asyncio.sleep(self.interval)
```

### Comparing `graia-amnesia-0.7.1/src/graia/amnesia/message/__init__.py` & `graia_amnesia-0.8.0/src/graia/amnesia/message/chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Iterable, Iterator
 from copy import deepcopy
-from typing import TYPE_CHECKING, Any, ClassVar, Sequence, TypeVar, overload
+from typing import TYPE_CHECKING, Any, Sequence, TypeVar, overload
 
 from typing_extensions import Self
 
 from .element import Element, Text
 
 if TYPE_CHECKING:
     E = TypeVar("E", bound=Element)
@@ -59,14 +59,16 @@
 
     - `removesuffix`: 尝试移除后缀
 
     - `replace`: 替换消息链的一部分
 
     """
 
+    _text_class: type[Text]
+
     content: list[Element]
 
     def __init__(self, elements: list[Element]):
         """从传入的序列(可以是元组 tuple, 也可以是列表 list) 创建消息链.
         Args:
             elements (list[T]): 包含且仅包含消息元素的序列
         Returns:
@@ -75,15 +77,15 @@
         self.content = elements
 
     def has(self, item: Element | type[Element] | Self | Sequence[str | Element]) -> bool:
         """
         判断消息链中是否含有特定的内容.
 
         Args:
-            item (Element | type[Element] | Self | Sequence[str | Element]): 需要判断的元素/元素类型/消息链/字符串/元素列表.
+            item (Element | type[Element] | Self | Sequence[str | Element]): 需判断内容.
 
         Returns:
             bool: 判断结果
         """
         if isinstance(item, type):
             return item in [type(i) for i in self.content]
         if isinstance(item, Element):
@@ -204,21 +206,21 @@
 
         result = []
 
         texts = []
         for i in self.content:
             if not isinstance(i, Text):
                 if texts:
-                    result.append(__text_element_class__("".join(texts)))
+                    result.append(self._text_class("".join(texts)))
                     texts.clear()  # 清空缓存
                 result.append(i)
             else:
                 texts.append(i.text)
         if texts:
-            result.append(__text_element_class__("".join(texts)))
+            result.append(self._text_class("".join(texts)))
             texts.clear()  # 清空缓存
         return self.__class__(result)
 
     def exclude(self, *types: type[Element]) -> Self:
         """将除了在给出的消息元素类型中符合的消息元素重新包装为一个新的消息链
         Args:
             *types (type[Element]): 将排除在外的消息元素类型
@@ -253,15 +255,15 @@
             if isinstance(element, Text):
                 split_result = element.text.split(pattern)
                 for index, split_str in enumerate(split_result):
                     if tmp and index > 0:
                         result.append(self.__class__(tmp))
                         tmp = []
                     if split_str or raw_string:
-                        tmp.append(__text_element_class__(split_str))
+                        tmp.append(self._text_class(split_str))
             else:
                 tmp.append(element)
         if tmp:
             result.append(self.__class__(tmp))
             tmp = []
         return result
 
@@ -322,15 +324,15 @@
             copy (bool): 是否要在副本上修改.
 
         Returns:
             MessageChain: copy = True 时返回副本, 否则返回自己的引用.
         """
         chain_ref = self.copy() if copy else self
         if isinstance(element, str):
-            element = __text_element_class__(element)
+            element = self._text_class(element)
         chain_ref.content.append(element)
         return chain_ref
 
     def extend(
         self,
         *content: Self | Element | list[Element | str],
         copy: bool = False,
@@ -346,21 +348,21 @@
             MessageChain: copy = True 时返回副本, 否则返回自己的引用.
         """
         result = []
         for i in content:
             if isinstance(i, Element):
                 result.append(i)
             elif isinstance(i, str):
-                result.append(__text_element_class__(i))
+                result.append(self._text_class(i))
             elif isinstance(i, MessageChain):
                 result.extend(i.content)
             else:
                 for e in i:
                     if isinstance(e, str):
-                        result.append(__text_element_class__(e))
+                        result.append(self._text_class(e))
                     else:
                         result.append(e)
         if copy:
             return self.__class__(deepcopy(self.content) + result)
         self.content.extend(result)
         return self
 
@@ -535,45 +537,41 @@
         # Merge result
         result_list: list[Element] = []
         char_stk: list[str] = []
         for v in unzipped_result:
             if isinstance(v, str):
                 char_stk.append(v)
             else:
-                result_list.append(__text_element_class__("".join(char_stk)))
+                result_list.append(self._text_class("".join(char_stk)))
                 char_stk = []
                 result_list.append(v)
         if char_stk:
-            result_list.append(__text_element_class__("".join(char_stk)))
+            result_list.append(self._text_class("".join(char_stk)))
         return self.__class__(result_list)
 
     def __add__(self, content: MessageChain | list[Element] | Element | str) -> Self:
         if isinstance(content, str):
-            content = __text_element_class__(content)
+            content = self._text_class(content)
         if isinstance(content, Element):
             content = [content]
         if isinstance(content, MessageChain):
             content = content.content
-        return __message_chain_class__(self.content + content)
+        return type(self)(self.content + content)
 
     def __radd__(self, content: MessageChain | list[Element] | Element | str) -> Self:
         if isinstance(content, str):
-            content = __text_element_class__(content)
+            content = self._text_class(content)
         if isinstance(content, Element):
             content = [content]
         if isinstance(content, MessageChain):
             content = content.content
-        return __message_chain_class__(content + self.content)
+        return type(self)(content + self.content)
 
     def __iadd__(self, content: MessageChain | list[Element] | Element | str) -> Self:
         if isinstance(content, str):
-            content = __text_element_class__(content)
+            content = self._text_class(content)
         if isinstance(content, Element):
             content = [content]
         if isinstance(content, MessageChain):
             content = content.content
         self.content.extend(content)
         return self
-
-
-__message_chain_class__: type[MessageChain] = MessageChain
-__text_element_class__: type[Text] = Text
```

### Comparing `graia-amnesia-0.7.1/src/graia/amnesia/message/element.py` & `graia_amnesia-0.8.0/src/graia/amnesia/message/element.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
-    from . import MessageChain, __message_chain_class__, __text_element_class__
+    from . import MessageChain
 
 
 class Element:
+    _chain_class: type[MessageChain]
+
     def __str__(self) -> str:
         return ""
 
     def __add__(self: Element, content: MessageChain | list[Element] | Element | str) -> MessageChain:
-        from . import __message_chain_class__, __text_element_class__
+        from . import MessageChain
 
         if isinstance(content, str):
-            content = [__text_element_class__(content)]
+            content = [self._chain_class._text_class(content)]
         if isinstance(content, Element):
             content = [content]
         if isinstance(content, MessageChain):
             content = content.content
-        return MessageChain(content + [self])
+        return self._chain_class(content + [self])
 
     def __radd__(self: Element, content: MessageChain | list[Element] | Element | str) -> MessageChain:
-        from . import __message_chain_class__, __text_element_class__
-
+        from . import MessageChain
+        
         if isinstance(content, str):
-            content = [__text_element_class__(content)]
+            content = [self._chain_class._text_class(content)]
         if isinstance(content, Element):
             content = [content]
         if isinstance(content, MessageChain):
             content = content.content
-        return __message_chain_class__([self] + content)
+        return self._chain_class([self] + content)
 
 
 class Text(Element):
     text: str
     style: str | None
 
     def __init__(self, text: str, style: str | None = None) -> None:
```

### Comparing `graia-amnesia-0.7.1/src/graia/amnesia/message/formatter.py` & `graia_amnesia-0.8.0/src/graia/amnesia/message/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 from typing import ClassVar
 
 from graia.amnesia.message import MessageChain
 from graia.amnesia.message.element import Element
 
 
 class Formatter:
-
     format_string: str
     __message_chain_class__: ClassVar[type[MessageChain]] = MessageChain
 
     def __init__(self, format_string: str) -> None:
         self.format_string = format_string
 
     @classmethod
     def ensure_element(cls, obj: str | Element) -> Element:
-        return cls.__message_chain_class__.__text_element_class__(obj) if isinstance(obj, str) else obj
+        return cls.__message_chain_class__._text_class(obj) if isinstance(obj, str) else obj
 
     @classmethod
     def extract_chain(cls, obj: Element | MessageChain | str | Sequence[Element]) -> list[Element]:
         if isinstance(obj, MessageChain):
             return obj.content
         if isinstance(obj, str):
             obj = cls.ensure_element(obj)
```

### Comparing `graia-amnesia-0.7.1/src/graia/amnesia/utilles.py` & `graia_amnesia-0.8.0/src/graia/amnesia/utilles.py`

 * *Files identical despite different names*

### Comparing `graia-amnesia-0.7.1/PKG-INFO` & `graia_amnesia-0.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: graia-amnesia
-Version: 0.7.1
+Version: 0.8.0
 Summary: a collection of shared components for graia
+Author-Email: GreyElaina <GreyElaina@outlook.com>
 License: MIT
-Author-email: GreyElaina <GreyElaina@outlook.com>
-Requires-Python: >=3.8,<4.0
-Provides-Extra: aiohttp
-Provides-Extra: colorful
-Provides-Extra: orjson
-Provides-Extra: starlette
-Provides-Extra: ujson
-Provides-Extra: uvicorn
+Requires-Python: <4.0,>=3.8
+Requires-Dist: launart<1.0.0,>=0.7.0
+Requires-Dist: typing-extensions>=4.0.0
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Amnesia
 
 _A collection of common components for Graia Project._
@@ -55,8 +51,7 @@
  - `Launch API` 可以优化应用的启动流程, 适用于 `Saya` 或是单纯的 `Broadcast Control` 应用;
  - `Service` 使维护和访问资源的流程更加合理;
  - ...或许还会有更多?
 
 ## 协议
 
 本项目以 MIT 协议开源.
-
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: graia-amnesia Version: 0.7.1 Summary: a collection
-of shared components for graia License: MIT Author-email: GreyElaina
-outlook.com> Requires-Python: >=3.8,<4.0 Provides-Extra: aiohttp Provides-
-Extra: colorful Provides-Extra: orjson Provides-Extra: starlette Provides-
-Extra: ujson Provides-Extra: uvicorn Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: graia-amnesia Version: 0.8.0 Summary: a collection
+of shared components for graia Author-Email: GreyElaina
+outlook.com> License: MIT Requires-Python: <4.0,>=3.8 Requires-Dist:
+launart<1.0.0,>=0.7.0 Requires-Dist: typing-extensions>=4.0.0 Description-
+Content-Type: text/markdown
       # Amnesia _A collection of common components for Graia Project._ >
         äºæ¯æå¤©ä»å°å°æ¥. > æ¯ä¸å¤©é½ä¼å¸¦æ¥æ°çéé,
                 çºµä½¿æç»å¿å´ä¹ä¸ä¼å®³ææå¤©å°æ¥.
       [PyPI] [code_style] [https://img.shields.io/badge/%20imports-isort-
  %231674b1?style=flat&labelColor=ef8336] [https://results.pre-commit.ci/badge/
                     github/GraiaProject/Amnesia/master.svg]
 ## ç®è¿° Amnesia æ¯ä¸ç³»åå±ç¨ç»ä»¶çéå, åå«äºä»¥ä¸åå®¹: -
```

