# Comparing `tmp/async_wrapper-0.4.6.tar.gz` & `tmp/async_wrapper-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.6.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.7.tar", max compression
```

## Comparing `async_wrapper-0.4.6.tar` & `async_wrapper-0.4.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-08-05 12:04:15.257181 async_wrapper-0.4.6/LICENSE
--rw-r--r--   0        0        0     1681 2023-08-05 12:04:15.257181 async_wrapper-0.4.6/README.md
--rw-r--r--   0        0        0     3467 2023-08-05 12:04:31.509246 async_wrapper-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      479 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-05 12:04:31.549247 async_wrapper-0.4.6/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      595 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     2462 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1407 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      551 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/py.typed
--rw-r--r--   0        0        0     8007 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      207 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     6984 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      837 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0    10697 2023-08-05 12:04:15.261180 async_wrapper-0.4.6/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 async_wrapper-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 08:27:34.711743 async_wrapper-0.4.7/LICENSE
+-rw-r--r--   0        0        0     1836 2023-08-06 08:27:34.711743 async_wrapper-0.4.7/README.md
+-rw-r--r--   0        0        0     3779 2023-08-06 08:27:51.808116 async_wrapper-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-06 08:27:51.860117 async_wrapper-0.4.7/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     2462 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1141 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      551 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0    10648 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      207 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     7137 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      866 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0    10823 2023-08-06 08:27:34.715743 async_wrapper-0.4.7/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 async_wrapper-0.4.7/PKG-INFO
```

### Comparing `async_wrapper-0.4.6/LICENSE` & `async_wrapper-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.6/README.md` & `async_wrapper-0.4.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
+[![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=main)](#)
+[![codecov](https://codecov.io/gh/phi-friday/async-wrapper/branch/main/graph/badge.svg?token=R1RAQ5F0YD)](https://codecov.io/gh/phi-friday/async-wrapper)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
 $ pip install async_wrapper
 ```
```

### Comparing `async_wrapper-0.4.6/pyproject.toml` & `async_wrapper-0.4.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.6"
+version = "0.4.7"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
@@ -18,20 +18,21 @@
 exceptiongroup = { version = "^1.1.2", markers = "python_version < '3.11'" }
 
 [tool.poetry.extras]
 uvloop = ['uvloop']
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.282"
-black = "23.3.0"
+black = "23.7.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 trio = "^0.22.2"
 pyyaml = ">=6.0.1"    # cython error
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
@@ -113,7 +114,21 @@
 known-local-folder = ["async_wrapper"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.pyright]
 pythonVersion = '3.8'
 pythonPlatform = 'Linux'
 diagnostic = 'basic'
+
+[tool.pytest.ini_options]
+addopts = "--cov=src/async_wrapper --cov-report html --cov-report=xml"
+testpaths = ["tests"]
+
+[tool.coverage.run]
+omit = ["./tests/**/*"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: no cover",
+    "if TYPE_CHECKING:",
+    "raise NotImplementedError",
+]
```

### Comparing `async_wrapper-0.4.6/src/async_wrapper/convert/_async.py` & `async_wrapper-0.4.7/src/async_wrapper/convert/_async.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.6/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.7/src/async_wrapper/convert/_sync.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.6/src/async_wrapper/convert/main.py` & `async_wrapper-0.4.7/src/async_wrapper/convert/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 __all__ = ["toggle_func", "async_to_sync", "sync_to_async"]
 
 
 @overload
 def toggle_func(
     func: Callable[ParamT, Coroutine[Any, Any, ValueT]],
 ) -> Callable[ParamT, ValueT]:
-    ...
+    ...  # pragma: no cover
 
 
 @overload
 def toggle_func(
     func: Callable[ParamT, ValueT],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
-    ...
+    ...  # pragma: no cover
 
 
 def toggle_func(
     func: Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]],
 ) -> Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     """sync to async, async to sync
```

### Comparing `async_wrapper-0.4.6/src/async_wrapper/exception.py` & `async_wrapper-0.4.7/src/async_wrapper/exception.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.6/src/async_wrapper/queue.py` & `async_wrapper-0.4.7/src/async_wrapper/queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from __future__ import annotations
 
 import math
 import sys
-from typing import TYPE_CHECKING, Generic, TypeVar
+from contextlib import asynccontextmanager, contextmanager
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncContextManager,
+    AsyncGenerator,
+    ContextManager,
+    Generator,
+    Generic,
+    TypeVar,
+)
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group, fail_after
 from anyio.streams.memory import BrokenResourceError, ClosedResourceError, EndOfStream
 
 from async_wrapper.exception import QueueBrokenError, QueueEmptyError, QueueFullError
 
-if sys.version_info < (3, 11):
+if sys.version_info < (3, 11):  # pragma: no cover
     from exceptiongroup import ExceptionGroup  # type: ignore
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from anyio.streams.memory import (
         MemoryObjectReceiveStream,
         MemoryObjectSendStream,
         MemoryObjectStreamStatistics,
     )
     from typing_extensions import Self
 
-__all__ = ["Queue"]
+__all__ = ["Queue", "create_queue"]
 
 ValueT = TypeVar("ValueT")
 
 
 class Queue(Generic[ValueT]):
     """obtained from asyncio.Queue"""
 
+    __slots__ = ("_putter", "_getter", "_close_putter", "_close_getter")
+
     _putter: MemoryObjectSendStream[ValueT]
     _getter: MemoryObjectReceiveStream[ValueT]
 
     def __init__(
         self,
         max_size: float | None = None,
         stream: tuple[MemoryObjectSendStream[ValueT], MemoryObjectReceiveStream[ValueT]]
@@ -47,17 +59,70 @@
             putter, getter = stream
             if putter._closed or getter._closed:  # noqa: SLF001
                 raise QueueBrokenError("putter or getter is closed")
             if putter._state.buffer is not getter._state.buffer:  # noqa: SLF001
                 raise QueueBrokenError("putter and getter has diff buffer.")
             self._putter, self._getter = stream
 
+        self._close_putter: bool = True
+        self._close_getter: bool = True
+
+    @property
+    def aputter(self) -> AsyncContextManager[Self]:
+        """aclose putter only"""
+        return self._as_aputter()
+
+    @property
+    def agetter(self) -> AsyncContextManager[Self]:
+        """aclose getter only"""
+        return self._as_agetter()
+
+    @property
+    def putter(self) -> ContextManager[Self]:
+        """close putter only"""
+        return self._as_putter()
+
+    @property
+    def getter(self) -> ContextManager[Self]:
+        """close getter only"""
+        return self._as_getter()
+
+    @asynccontextmanager
+    async def _as_aputter(self) -> AsyncGenerator[Self, None]:
+        try:
+            yield self
+        finally:
+            await self._putter.aclose()
+
+    @asynccontextmanager
+    async def _as_agetter(self) -> AsyncGenerator[Self, None]:
+        try:
+            yield self
+        finally:
+            await self._getter.aclose()
+
+    @contextmanager
+    def _as_putter(self) -> Generator[Self, None, None]:
+        try:
+            yield self
+        finally:
+            self._putter.close()
+
+    @contextmanager
+    def _as_getter(self) -> Generator[Self, None, None]:
+        try:
+            yield self
+        finally:
+            self._getter.close()
+
     @property
     def _closed(self) -> bool:
-        return self._putter._closed or self._getter._closed  # noqa: SLF001
+        return (not self._close_putter or self._putter._closed) and (  # noqa: SLF001
+            not self._close_getter or self._getter._closed  # noqa: SLF001
+        )
 
     def qsize(self) -> int:
         """number of items in the queue."""
         return len(self._getter._state.buffer)  # noqa: SLF001
 
     @property
     def maxsize(self) -> float:
@@ -160,21 +225,25 @@
             self._close()
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     async def _aclose(self) -> None:
         """close the stream as async"""
         async with create_task_group() as task_group:
-            task_group.start_soon(self._getter.aclose)
-            task_group.start_soon(self._putter.aclose)
+            if self._close_getter:
+                task_group.start_soon(self._getter.aclose)
+            if self._close_putter:
+                task_group.start_soon(self._putter.aclose)
 
     def _close(self) -> None:
         """close the stream as sync"""
-        self._getter.close()
-        self._putter.close()
+        if self._close_getter:
+            self._getter.close()
+        if self._close_putter:
+            self._putter.close()
 
     def clone(self, *, putter: bool = False, getter: bool = False) -> Queue[ValueT]:
         """create clone of this queue.
 
         Args:
             putter: if true, clone putter. Defaults to False.
             getter: if true, clone getter. Defaults to False.
@@ -191,41 +260,52 @@
         """create clone of this queue"""
         if self._closed:
             raise QueueBrokenError("the queue is already closed")
         if not putter and not getter:
             raise ValueError("putter and getter are None.")
         _putter = self._putter.clone() if putter else self._putter
         _getter = self._getter.clone() if getter else self._getter
-        return Queue(stream=(_putter, _getter))
+        new = Queue(stream=(_putter, _getter))
+        new._close_putter = putter  # noqa: SLF001
+        new._close_getter = getter  # noqa: SLF001
+        return new
 
     def statistics(self) -> MemoryObjectStreamStatistics:
         """return statstics from stream"""
         return self._getter._state.statistics()  # noqa: SLF001
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        self.close()
+        try:
+            self.close()
+        finally:
+            self._close_getter = True
+            self._close_putter = True
 
     async def __aenter__(self) -> Self:
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
-        await self.aclose()
+        try:
+            await self.aclose()
+        finally:
+            self._close_getter = True
+            self._close_putter = True
 
     def __aiter__(self) -> Self:
         return self
 
     async def __anext__(self) -> ValueT:
         try:
             return await self.aget()
@@ -236,7 +316,27 @@
         return self
 
     def __next__(self) -> ValueT:
         try:
             return self.get()
         except (EndOfStream, QueueEmptyError, QueueBrokenError) as exc:
             raise StopIteration from exc
+
+    def __len__(self) -> int:
+        return self.qsize()
+
+    def __repr__(self) -> str:
+        max_size = "inf" if self.maxsize == math.inf else self.maxsize
+        size = self.qsize()
+        return f"<Queue: max={max_size}, size={size}>"
+
+
+def create_queue(max_size: float | None = None) -> Queue[Any]:
+    """create queue like asyncio.Queue
+
+    Args:
+        max_size: queue size. Defaults to None.
+
+    Returns:
+        queue using anyio stream
+    """
+    return Queue(max_size)
```

### Comparing `async_wrapper-0.4.6/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.7/src/async_wrapper/task_group/task_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     >>>     assert soon_2.value == 2
     >>>
     >>>
     >>> if __name__ == "__main__":
     >>>     anyio.run(main)
     """
 
+    __slots__ = ("_task_group", "_active_self")
+
     def __init__(self, task_group: _TaskGroup) -> None:
         self._task_group = task_group
         self._active_self = False
 
     @property
     @override
     def cancel_scope(self) -> CancelScope:
@@ -134,14 +136,16 @@
         """
         return SoonWrapper(func, self, semaphore=semaphore, limiter=limiter, lock=lock)
 
 
 class SoonWrapper(Generic[ParamT, ValueT_co]):
     """wrapped func using in TaskGroupWrapper"""
 
+    __slots__ = ("func", "task_group", "semaphore", "limiter", "lock", "_wrapped")
+
     def __init__(  # noqa: PLR0913
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: _TaskGroup,
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
@@ -188,15 +192,15 @@
                     await stack.enter_async_context(self.limiter)
                 if self.lock is not None:
                     await stack.enter_async_context(self.lock)
 
                 result = await self.func(*args, **kwargs)
                 value._value = result  # noqa: SLF001
                 return result
-            raise RuntimeError("never")
+            raise RuntimeError("never")  # pragma: no cover
 
         self._wrapped = wrapped
         return wrapped
 
     def copy(
         self,
         semaphore: Semaphore | None = None,
```

### Comparing `async_wrapper-0.4.6/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.7/src/async_wrapper/task_group/value.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 __all__ = ["SoonValue"]
 
 
 class SoonValue(Generic[ValueT_co]):
     """will get value soon"""
 
+    __slots__ = ("_value",)
+
     def __init__(self) -> None:
         self._value: ValueT_co | local = Pending
 
     def __repr__(self) -> str:
         status = "pending" if self._value is Pending else "done"
         return f"<SoonValue: status={status}>"
```

### Comparing `async_wrapper-0.4.6/src/async_wrapper/wait.py` & `async_wrapper-0.4.7/src/async_wrapper/wait.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     >>> $ poetry run python main.py
     >>> test: start
     >>> test2: start
     >>> test: end
     >>> test2: end
     """
 
+    __slots__ = ("_event", "_func", "_args", "_kwargs")
+
     _event: Event
 
     def __init__(
         self,
         func: Callable[ParamT, Awaitable[Any]],
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
@@ -173,14 +175,16 @@
     >>>     assert result == [3, 2, 4, 1]
     >>>
     >>>
     >>> if __name__ == "__main__":
     >>>     anyio.run(main)
     """
 
+    __slots__ = ("_events", "__setter", "__getter", "__task_group")
+
     def __init__(self, task_group: TaskGroup | None = None) -> None:
         self._events: dict[Waiter, MemoryObjectReceiveStream[Any]] = {}
         self.__setter: MemoryObjectSendStream[Waiter] | None = None
         self.__getter: MemoryObjectReceiveStream[Waiter] | None = None
         self.__task_group: TaskGroup | None = task_group
 
     @property
```

### Comparing `async_wrapper-0.4.6/PKG-INFO` & `async_wrapper-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.6
+Version: 0.4.7
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,16 @@
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
+[![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=main)](#)
+[![codecov](https://codecov.io/gh/phi-friday/async-wrapper/branch/main/graph/badge.svg?token=R1RAQ5F0YD)](https://codecov.io/gh/phi-friday/async-wrapper)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
 $ pip install async_wrapper
 ```
```

