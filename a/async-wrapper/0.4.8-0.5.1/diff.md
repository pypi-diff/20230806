# Comparing `tmp/async_wrapper-0.4.8.tar.gz` & `tmp/async_wrapper-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.8.tar", max compression
+gzip compressed data, was "async_wrapper-0.5.1.tar", max compression
```

## Comparing `async_wrapper-0.4.8.tar` & `async_wrapper-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-08-06 09:02:54.717703 async_wrapper-0.4.8/LICENSE
--rw-r--r--   0        0        0     1836 2023-08-06 09:02:54.717703 async_wrapper-0.4.8/README.md
--rw-r--r--   0        0        0     3806 2023-08-06 09:03:12.293771 async_wrapper-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      513 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-06 09:03:12.345772 async_wrapper-0.4.8/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0     1424 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     4315 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1141 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      551 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/exception.py
--rw-r--r--   0        0        0        0 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/py.typed
--rw-r--r--   0        0        0    11533 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/queue.py
--rw-r--r--   0        0        0      207 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     7137 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0      866 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0    10796 2023-08-06 09:02:54.721704 async_wrapper-0.4.8/src/async_wrapper/wait.py
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 async_wrapper-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1836 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/README.md
+-rw-r--r--   0        0        0     3983 2023-08-06 19:26:55.955239 async_wrapper-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-06 19:26:55.999239 async_wrapper-0.5.1/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0     1668 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     4568 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1226 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0     1560 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/exception.py
+-rw-r--r--   0        0        0        0 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0    12169 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/queue.py
+-rw-r--r--   0        0        0      207 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     7500 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      866 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0    11566 2023-08-06 19:26:39.799144 async_wrapper-0.5.1/src/async_wrapper/wait.py
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 async_wrapper-0.5.1/PKG-INFO
```

### Comparing `async_wrapper-0.4.8/LICENSE` & `async_wrapper-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.8/README.md` & `async_wrapper-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.8/pyproject.toml` & `async_wrapper-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.8"
+version = "0.5.1"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
-homepage = "https://github.com/phi-friday/async-wrapper"
+homepage = "https://async-wrapper.readthedocs.io/"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = "^3.7.0"
@@ -26,14 +26,21 @@
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 trio = "^0.22.2"
 pyyaml = ">=6.0.1"    # cython error
 pytest-cov = "^4.1.0"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.1.2"
+readthedocs-sphinx-search = "^0.3.1"
+sphinx-rtd-theme = "^1.2.2"
+sphinx-mdinclude = "^0.5.3"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
 select = ["ALL"]
@@ -105,14 +112,15 @@
     "ANN201",
     "PLR0133",
     "W605",
     "D103",
     "D102",
     "PLR2004",
 ]
+"./src/docs/conf.py" = ['E402']
 
 [tool.ruff.isort]
 known-local-folder = ["async_wrapper"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.pyright]
 include = ["src", "tests"]
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/__init__.py` & `async_wrapper-0.5.1/src/async_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.8/src/async_wrapper/convert/_async.py` & `async_wrapper-0.5.1/src/async_wrapper/convert/_async.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,49 +11,50 @@
 
 __all__ = ["sync_to_async"]
 
 
 def sync_to_async(
     func: Callable[ParamT, ValueT_co],
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT_co]]:
-    """convert sync func to async func
+    """Convert a synchronous function to an asynchronous function.
 
     Args:
-        func: sync func
+        func: The synchronous function to be converted.
 
     Returns:
-        async func
+        An asynchronous function
+        that behaves equivalently to the input synchronous function.
 
-    how to use:
-    >>> import time
-    >>>
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import sync_to_async
-    >>>
-    >>>
-    >>> @sync_to_async
-    >>> def test(x: int) -> int:
-    >>>     print(f"[{x}] test: start")
-    >>>     time.sleep(1)
-    >>>     print(f"[{x}] test: end")
-    >>>     return x
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     start = time.perf_counter()
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         for i in range(4):
-    >>>             task_group.start_soon(test, i)
-    >>>     end = time.perf_counter()
-    >>>     assert end - start < 1.1
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
+    Example:
+        >>> import time
+        >>>
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import sync_to_async
+        >>>
+        >>>
+        >>> @sync_to_async
+        >>> def test(x: int) -> int:
+        >>>     print(f"[{x}] test: start")
+        >>>     time.sleep(1)
+        >>>     print(f"[{x}] test: end")
+        >>>     return x
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     start = time.perf_counter()
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         for i in range(4):
+        >>>             task_group.start_soon(test, i)
+        >>>     end = time.perf_counter()
+        >>>     assert end - start < 1.1
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
     """
 
     @wraps(func)
     async def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
         return await anyio.to_thread.run_sync(partial(func, *args, **kwargs))
 
     return inner
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.5.1/src/async_wrapper/convert/_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,83 +17,81 @@
 current_async_lib_var = ContextVar("current_async_lib", default="asyncio")
 use_uvloop_var = ContextVar("use_uvloop", default=False)
 
 
 def async_to_sync(
     func: Callable[ParamT, Awaitable[ValueT_co]],
 ) -> Callable[ParamT, ValueT_co]:
-    """convert awaitable func to sync func.
+    """Convert an awaitable function to a synchronous function.
 
-    if in asnyc context, try to use same backend.
-    default to asyncio.
+    If used within an asynchronous context, attempts to use the same backend.
+    Defaults to asyncio.
 
     Args:
-        func: awaitable func.
+        func: An awaitable function.
 
     Returns:
-        sync func.
+        A synchronous function.
 
-    how to use:
-    >>> import asyncio
-    >>> import time
-    >>>
-    >>> import anyio
-    >>> import sniffio
-    >>>
-    >>> from async_wrapper import async_to_sync
-    >>>
-    >>>
-    >>> @async_to_sync
-    >>> async def test(x: int) -> int:
-    >>>     backend = sniffio.current_async_library()
-    >>>     if backend == "asyncio":
-    >>>         loop = asyncio.get_running_loop()
-    >>>         print(backend, loop)
-    >>>     else:
-    >>>         print(backend)
-    >>>     await anyio.sleep(1)
-    >>>     return x
-    >>>
-    >>>
-    >>> def main() -> None:
-    >>>     start = time.perf_counter()
-    >>>     result = test(1)
-    >>>     end = time.perf_counter()
-    >>>     assert result == 1
-    >>>     assert end - start < 1.1
-    >>>
-    >>>
-    >>> async def async_main() -> None:
-    >>>     start = time.perf_counter()
-    >>>     result = test(1)
-    >>>     end = time.perf_counter()
-    >>>     assert result == 1
-    >>>     assert end - start < 1.1
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     main()
-    >>>     anyio.run(
-    >>>         async_main,
-    >>>         backend="asyncio",
-    >>>         backend_options={"use_uvloop": True},
-    >>>     )
-    >>>     anyio.run(
-    >>>         async_main,
-    >>>         backend="asyncio",
-    >>>         backend_options={"use_uvloop": True},
-    >>>     )
-    >>>     anyio.run(async_main, backend="trio")
-
-    stdout:
-    >>> $ poetry run python main.py
-    >>> asyncio <_UnixSelectorEventLoop running=True closed=False debug=False>
-    >>> asyncio <_UnixSelectorEventLoop running=True closed=False debug=False>
-    >>> asyncio <uvloop.Loop running=True closed=False debug=False>
-    >>> trio
+    Example:
+        >>> import asyncio
+        >>> import time
+        >>>
+        >>> import anyio
+        >>> import sniffio
+        >>>
+        >>> from async_wrapper import async_to_sync
+        >>>
+        >>>
+        >>> @async_to_sync
+        >>> async def test(x: int) -> int:
+        >>>     backend = sniffio.current_async_library()
+        >>>     if backend == "asyncio":
+        >>>         loop = asyncio.get_running_loop()
+        >>>         print(backend, loop)
+        >>>     else:
+        >>>         print(backend)
+        >>>     await anyio.sleep(1)
+        >>>     return x
+        >>>
+        >>>
+        >>> def main() -> None:
+        >>>     start = time.perf_counter()
+        >>>     result = test(1)
+        >>>     end = time.perf_counter()
+        >>>     assert result == 1
+        >>>     assert end - start < 1.1
+        >>>
+        >>>
+        >>> async def async_main() -> None:
+        >>>     start = time.perf_counter()
+        >>>     result = test(1)
+        >>>     end = time.perf_counter()
+        >>>     assert result == 1
+        >>>     assert end - start < 1.1
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     main()
+        >>>     anyio.run(
+        >>>         async_main,
+        >>>         backend="asyncio",
+        >>>         backend_options={"use_uvloop": True},
+        >>>     )
+        >>>     anyio.run(
+        >>>         async_main,
+        >>>         backend="asyncio",
+        >>>         backend_options={"use_uvloop": True},
+        >>>     )
+        >>>     anyio.run(async_main, backend="trio")
+        $ poetry run python main.py
+        asyncio <_UnixSelectorEventLoop running=True closed=False debug=False>
+        asyncio <_UnixSelectorEventLoop running=True closed=False debug=False>
+        asyncio <uvloop.Loop running=True closed=False debug=False>
+        trio
     """
     sync_func = _as_sync(func)
 
     @wraps(func)
     def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
         backend = _get_current_backend()
         use_uvloop = _check_uvloop()
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/convert/main.py` & `async_wrapper-0.5.1/src/async_wrapper/convert/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 ) -> Callable[ParamT, Coroutine[Any, Any, ValueT]]:
     ...  # pragma: no cover
 
 
 def toggle_func(
     func: Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]],
 ) -> Callable[ParamT, ValueT] | Callable[ParamT, Coroutine[Any, Any, ValueT]]:
-    """sync to async, async to sync
+    """Convert between synchronous and asynchronous functions.
 
     Args:
-        func: sync or async func
-        backend: sync or async backend. Defaults to None.
+        func: A function that can be either synchronous or asynchronous.
 
     Returns:
-        async or sync func
+        A function that matches the desired synchronicity,
+        either synchronous or asynchronous.
     """
     if iscoroutinefunction(func):
         return async_to_sync(func)
     return sync_to_async(func)  # type: ignore
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/queue.py` & `async_wrapper-0.5.1/src/async_wrapper/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
     Generic,
     TypeVar,
 )
 
 from anyio import WouldBlock, create_memory_object_stream, create_task_group, fail_after
 from anyio.streams.memory import BrokenResourceError, ClosedResourceError, EndOfStream
 
-from async_wrapper.exception import QueueBrokenError, QueueEmptyError, QueueFullError
+from async_wrapper.exception import (
+    QueueBrokenError,
+    QueueClosedError,
+    QueueEmptyError,
+    QueueFullError,
+)
 
 if sys.version_info < (3, 11):  # pragma: no cover
     from exceptiongroup import ExceptionGroup  # type: ignore
 
 if TYPE_CHECKING:
     from types import TracebackType
 
@@ -34,74 +39,85 @@
 
 __all__ = ["Queue", "create_queue"]
 
 ValueT = TypeVar("ValueT")
 
 
 class Queue(Generic[ValueT]):
-    """obtained from asyncio.Queue
+    """obtained from :class:`asyncio.Queue`
 
-    how tow use:
-    >>> from __future__ import annotations
-    >>>
-    >>> from typing import Any
-    >>>
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import Queue
-    >>>
-    >>>
-    >>> async def aput(queue: Queue[Any], value: Any) -> None:
-    >>>     async with queue:
-    >>>         await queue.aput(value)
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     queue: Queue[Any] = Queue(10)
-    >>>
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         async with queue.aputter:
-    >>>             for i in range(10):
-    >>>                 task_group.start_soon(aput, queue.clone(putter=True), i)
-    >>>
-    >>>     async with queue.agetter:
-    >>>         result = {x async for x in queue}
-    >>>
-    >>>     assert result == set(range(10))
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
+    Example:
+        >>> from __future__ import annotations
+        >>>
+        >>> from typing import Any
+        >>>
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import Queue
+        >>>
+        >>>
+        >>> async def aput(queue: Queue[Any], value: Any) -> None:
+        >>>     async with queue:
+        >>>         await queue.aput(value)
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     queue: Queue[Any] = Queue(10)
+        >>>
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         async with queue.aputter:
+        >>>             for i in range(10):
+        >>>                 task_group.start_soon(aput, queue.clone(putter=True), i)
+        >>>
+        >>>     async with queue.agetter:
+        >>>         result = {x async for x in queue}
+        >>>
+        >>>     assert result == set(range(10))
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
     """
 
     __slots__ = ("_putter", "_getter", "_close_putter", "_close_getter")
 
     _putter: MemoryObjectSendStream[ValueT]
     _getter: MemoryObjectReceiveStream[ValueT]
 
-    def __init__(
-        self,
-        max_size: float | None = None,
-        stream: tuple[MemoryObjectSendStream[ValueT], MemoryObjectReceiveStream[ValueT]]
-        | None = None,
-    ) -> None:
-        if stream is None:
-            self._putter, self._getter = create_memory_object_stream(
-                max_buffer_size=max_size or math.inf,
-            )
-        else:
-            putter, getter = stream
-            if putter._closed or getter._closed:  # noqa: SLF001
-                raise QueueBrokenError("putter or getter is closed")
-            if putter._state.buffer is not getter._state.buffer:  # noqa: SLF001
-                raise QueueBrokenError("putter and getter has diff buffer.")
-            self._putter, self._getter = stream
+    if TYPE_CHECKING:
+
+        def __init__(self, max_size: float | None = None) -> None:
+            ...
+
+    else:
+
+        def __init__(
+            self,
+            max_size: float | None = None,
+            *,
+            _stream: tuple[
+                MemoryObjectSendStream[ValueT],
+                MemoryObjectReceiveStream[ValueT],
+            ]
+            | None = None,
+        ) -> None:
+            if _stream is None:
+                self._putter, self._getter = create_memory_object_stream(
+                    max_buffer_size=max_size or math.inf,
+                )
+            else:
+                putter, getter = _stream
+                if putter._closed or getter._closed:  # noqa: SLF001
+                    raise QueueBrokenError("putter or getter is closed")
+                if putter._state.buffer is not getter._state.buffer:  # noqa: SLF001
+                    raise QueueBrokenError("putter and getter has diff buffer.")
+                self._putter, self._getter = _stream
 
-        self._close_putter: bool = True
-        self._close_getter: bool = True
+            self._close_putter: bool = True
+            self._close_getter: bool = True
 
     @property
     def aputter(self) -> AsyncContextManager[Self]:
         """aclose putter only"""
         return self._as_aputter()
 
     @property
@@ -288,20 +304,20 @@
             return self._clone(putter=putter, getter=getter)
         except (ClosedResourceError, BrokenResourceError) as exc:
             raise QueueBrokenError from exc
 
     def _clone(self, *, putter: bool, getter: bool) -> Queue[ValueT]:
         """create clone of this queue"""
         if self._closed:
-            raise QueueBrokenError("the queue is already closed")
+            raise QueueClosedError("the queue is already closed")
         if not putter and not getter:
-            raise ValueError("putter and getter are None.")
+            raise RuntimeError("putter and getter are None.")
         _putter = self._putter.clone() if putter else self._putter
         _getter = self._getter.clone() if getter else self._getter
-        new = Queue(stream=(_putter, _getter))
+        new = Queue(_stream=(_putter, _getter))  # type: ignore
         new._close_putter = putter  # noqa: SLF001
         new._close_getter = getter  # noqa: SLF001
         return new
 
     def statistics(self) -> MemoryObjectStreamStatistics:
         """return statstics from stream"""
         return self._getter._state.statistics()  # noqa: SLF001
@@ -338,38 +354,48 @@
 
     def __aiter__(self) -> Self:
         return self
 
     async def __anext__(self) -> ValueT:
         try:
             return await self.aget()
-        except (EndOfStream, QueueEmptyError, QueueBrokenError) as exc:
+        except (
+            EndOfStream,
+            QueueEmptyError,
+            QueueBrokenError,
+            QueueClosedError,
+        ) as exc:
             raise StopAsyncIteration from exc
 
     def __iter__(self) -> Self:
         return self
 
     def __next__(self) -> ValueT:
         try:
             return self.get()
-        except (EndOfStream, QueueEmptyError, QueueBrokenError) as exc:
+        except (
+            EndOfStream,
+            QueueEmptyError,
+            QueueBrokenError,
+            QueueClosedError,
+        ) as exc:
             raise StopIteration from exc
 
     def __len__(self) -> int:
         return self.qsize()
 
     def __repr__(self) -> str:
         max_size = "inf" if self.maxsize == math.inf else self.maxsize
         size = self.qsize()
         return f"<Queue: max={max_size}, size={size}>"
 
 
 def create_queue(max_size: float | None = None) -> Queue[Any]:
-    """create queue like asyncio.Queue
+    """create queue like :class:`asyncio.Queue`
 
     Args:
         max_size: queue size. Defaults to None.
 
     Returns:
-        queue using anyio stream
+        new :obj:`Queue` using :class:`anyio.abc.ObjectStream`
     """
     return Queue(max_size)
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.5.1/src/async_wrapper/task_group/task_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,42 +20,42 @@
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 __all__ = ["TaskGroupWrapper", "create_task_group_wrapper"]
 
 
 class TaskGroupWrapper(_TaskGroup):
-    """wrap anyio.TaskGroup
+    """wrap :class:`anyio.abc.TaskGroup`
 
-    how to use:
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import TaskGroupWrapper
-    >>>
-    >>>
-    >>> async def test(x: int) -> int:
-    >>>     await anyio.sleep(0.1)
-    >>>     return x
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         async with TaskGroupWrapper(task_group) as tg:
-    >>>             func = tg.wrap(test)
-    >>>             soon_1 = func(1)
-    >>>             soon_2 = func(2)
-    >>>
-    >>>     assert soon_1.is_ready
-    >>>     assert soon_2.is_ready
-    >>>     assert soon_1.value == 1
-    >>>     assert soon_2.value == 2
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
+    Example:
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import TaskGroupWrapper
+        >>>
+        >>>
+        >>> async def test(x: int) -> int:
+        >>>     await anyio.sleep(0.1)
+        >>>     return x
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         async with TaskGroupWrapper(task_group) as tg:
+        >>>             func = tg.wrap(test)
+        >>>             soon_1 = func(1)
+        >>>             soon_2 = func(2)
+        >>>
+        >>>     assert soon_1.is_ready
+        >>>     assert soon_2.is_ready
+        >>>     assert soon_1.value == 1
+        >>>     assert soon_2.value == 2
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
     """
 
     __slots__ = ("_task_group", "_active_self")
 
     def __init__(self, task_group: _TaskGroup) -> None:
         self._task_group = task_group
         self._active_self = False
@@ -117,32 +117,32 @@
     def wrap(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
     ) -> SoonWrapper[ParamT, ValueT_co]:
-        """wrap function to use in wrapper.
+        """Wrap a function to be used within a wrapper.
 
-        func will return soon value.
+        The wrapped function will return a value shortly.
 
         Args:
-            func: target func
-            semaphore: anyio semaphore. Defaults to None.
-            limiter: anyio capacity limiter. defaults to None.
-            lock: anyio lock. defaults to None.
+            func: The target function to be wrapped.
+            semaphore: An :obj:`anyio.Semaphore`. Defaults to None.
+            limiter: An :obj:`anyio.CapacityLimiter`. Defaults to None.
+            lock: An :obj:`anyio.Lock`. Defaults to None.
 
         Returns:
-            wrapped func
+            The wrapped function.
         """
         return SoonWrapper(func, self, semaphore=semaphore, limiter=limiter, lock=lock)
 
 
 class SoonWrapper(Generic[ParamT, ValueT_co]):
-    """wrapped func using in TaskGroupWrapper"""
+    """wrapped func using in :class:`TaskGroupWrapper`"""
 
     __slots__ = ("func", "task_group", "semaphore", "limiter", "lock", "_wrapped")
 
     def __init__(  # noqa: PLR0913
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: _TaskGroup,
@@ -203,29 +203,26 @@
 
     def copy(
         self,
         semaphore: Semaphore | None = None,
         limiter: CapacityLimiter | None = None,
         lock: Lock | None = None,
     ) -> Self:
-        """copy self.
+        """Create a copy of this object.
 
         Args:
-            semaphore: anyio semaphore.
-                Defaults to None.
-                if not None, overwrite.
-            limiter: anyio capacity limiter.
-                Defaults to None.
-                if not None, overwrite.
-            lock: anyio lock.
-                Defaults to None.
-                if not None, overwrite.
+            semaphore: An :obj:`anyio.Semaphore`.
+                If provided, it will overwrite the existing semaphore. Defaults to None.
+            limiter: An :obj:`anyio.CapacityLimiter`.
+                If provided, it will overwrite the existing limiter. Defaults to None.
+            lock: An :obj:`anyio.Lock`.
+                If provided, it will overwrite the existing lock. Defaults to None.
 
         Returns:
-            self
+            A copy of this object with optional overwritten components.
         """
         if semaphore is None:
             semaphore = self.semaphore
         if limiter is None:
             limiter = self.limiter
         if lock is None:
             lock = self.lock
@@ -238,15 +235,15 @@
         )
 
 
 def create_task_group_wrapper() -> TaskGroupWrapper:
     """create new task group wrapper
 
     Returns:
-        task group wrapper
+        new :obj:`TaskGroupWrapper`
     """
     return TaskGroupWrapper(_create_task_group())
 
 
 def _is_active(task_group: _TaskGroup) -> bool:
     # trio, asyncio
     return task_group._active  # type: ignore # noqa: SLF001
```

### Comparing `async_wrapper-0.4.8/src/async_wrapper/task_group/value.py` & `async_wrapper-0.5.1/src/async_wrapper/task_group/value.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.8/src/async_wrapper/wait.py` & `async_wrapper-0.5.1/src/async_wrapper/wait.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,47 +23,45 @@
 ParamT = ParamSpec("ParamT")
 Pending = local()
 
 
 class Waiter(Event):
     """wait wrapper
 
-    how to use:
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import Waiter
-    >>>
-    >>>
-    >>> async def test() -> None:
-    >>>     print("test: start")
-    >>>     await anyio.sleep(1)
-    >>>     print("test: end")
-    >>>
-    >>>
-    >>> async def test2(event: anyio.Event) -> None:
-    >>>     print("test2: start")
-    >>>     await event.wait()
-    >>>     print("test2: end")
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         event = Waiter(test)(task_group)
-    >>>         task_group.start_soon(test2, event)
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
-
-    output:
-    >>> $ poetry run python main.py
-    >>> test: start
-    >>> test2: start
-    >>> test: end
-    >>> test2: end
+    Example:
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import Waiter
+        >>>
+        >>>
+        >>> async def test() -> None:
+        >>>     print("test: start")
+        >>>     await anyio.sleep(1)
+        >>>     print("test: end")
+        >>>
+        >>>
+        >>> async def test2(event: anyio.Event) -> None:
+        >>>     print("test2: start")
+        >>>     await event.wait()
+        >>>     print("test2: end")
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         event = Waiter(test)(task_group)
+        >>>         task_group.start_soon(test2, event)
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
+        $ poetry run python main.py
+        test: start
+        test2: start
+        test: end
+        test2: end
     """
 
     __slots__ = ("_event", "_func", "_args", "_kwargs")
 
     _event: Event
 
     def __init__(
@@ -89,15 +87,15 @@
     def __copy__(self) -> Self:
         return self.copy()
 
     def copy(self, *args: Any, **kwargs: Any) -> Self:
         """create new event
 
         Returns:
-            new
+            new :obj:`Waiter`
         """
         if not args:
             args = tuple(self._args)
         if not kwargs:
             kwargs = self._kwargs.copy()
         return Waiter(self._func, *args, **kwargs)  # type: ignore
 
@@ -126,61 +124,65 @@
 
     @override
     def statistics(self) -> EventStatistics:
         return self._event.statistics()
 
 
 class Completed:
-    """like asyncio.as_completed
+    """like :func:`asyncio.as_completed`
 
-    how to use:
-    >>> from __future__ import annotations
-    >>>
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import Completed
-    >>>
-    >>>
-    >>> async def test(x: int, sleep: float, result: list[int] | None = None) -> int:
-    >>>     print(f"[{x}] test: start")
-    >>>     await anyio.sleep(sleep)
-    >>>     print(f"[{x}] test: end")
-    >>>     if result is not None:
-    >>>         result.append(x)
-    >>>     return x
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     result: list[int] = []
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         task_group.start_soon(test, 1, 1, result)
-    >>>         async with Completed(task_group) as completed:
-    >>>             completed.start_soon(None, test, 2, 0.2)
-    >>>             completed.start_soon(None, test, 3, 0.1)
-    >>>             completed.start_soon(None, test, 4, 0.3)
-    >>>
-    >>>             result.extend([value async for value in completed])
-    >>>
-    >>>     assert result == [3, 2, 4, 1]
-    >>>
-    >>>     result = []
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         task_group.start_soon(test, 1, 1, result)
-    >>>         async with Completed() as completed:
-    >>>             completed.start_soon(task_group, test, 2, 0.2)
-    >>>             completed.start_soon(task_group, test, 3, 0.1)
-    >>>             completed.start_soon(task_group, test, 4, 0.3)
-    >>>
-    >>>             result.extend([value async for value in completed])
-    >>>
-    >>>     assert result == [3, 2, 4, 1]
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
+    Example:
+        >>> from __future__ import annotations
+        >>>
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import Completed
+        >>>
+        >>>
+        >>> async def test(
+        >>>     x: int,
+        >>>     sleep: float,
+        >>>     result: list[int] | None = None,
+        >>> ) -> int:
+        >>>     print(f"[{x}] test: start")
+        >>>     await anyio.sleep(sleep)
+        >>>     print(f"[{x}] test: end")
+        >>>     if result is not None:
+        >>>         result.append(x)
+        >>>     return x
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     result: list[int] = []
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         task_group.start_soon(test, 1, 1, result)
+        >>>         async with Completed(task_group) as completed:
+        >>>             completed.start_soon(None, test, 2, 0.2)
+        >>>             completed.start_soon(None, test, 3, 0.1)
+        >>>             completed.start_soon(None, test, 4, 0.3)
+        >>>
+        >>>             result.extend([value async for value in completed])
+        >>>
+        >>>     assert result == [3, 2, 4, 1]
+        >>>
+        >>>     result = []
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         task_group.start_soon(test, 1, 1, result)
+        >>>         async with Completed() as completed:
+        >>>             completed.start_soon(task_group, test, 2, 0.2)
+        >>>             completed.start_soon(task_group, test, 3, 0.1)
+        >>>             completed.start_soon(task_group, test, 4, 0.3)
+        >>>
+        >>>             result.extend([value async for value in completed])
+        >>>
+        >>>     assert result == [3, 2, 4, 1]
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
     """
 
     __slots__ = ("_events", "__setter", "__getter", "__task_group")
 
     def __init__(self, task_group: TaskGroup | None = None) -> None:
         self._events: dict[Waiter, MemoryObjectReceiveStream[Any]] = {}
         self.__setter: MemoryObjectSendStream[Waiter] | None = None
@@ -220,23 +222,26 @@
     def start_soon(
         self,
         task_group: TaskGroup | None,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
     ) -> None:
-        """like TaskGroup.start_soon
+        """Start a coroutine in a task group,
+        similar to :meth:`anyio.abc.TaskGroup.start_soon`.
 
-        if it has already TaskGroup, task_group should be same object.
+        If a task group is already provided,
+        the task_group parameter should be the same object.
 
         Args:
-            task_group: anyio Task Group. defaults to None.
-            func: target func
-            name: using in anyio.TaskGroup.start_soon. Defaults to None.
-        """
+            task_group: An :class:`anyio.abc.TaskGroup`. Defaults to None.
+            func: The target coroutine function.
+            name: The name used in :meth:`anyio.abc.TaskGroup.start_soon`.
+                Defaults to None.
+        """  # noqa: D205
         if not self._is_active:
             raise PendingError("enter first")
         task_group = self._task_group(task_group)
         waiter, getter = _create_waiter(func, *args)
         waiter(task_group, name=name)
         self._events[waiter] = getter
 
@@ -296,57 +301,57 @@
 
 async def wait_for(
     event: Event | Iterable[Event],
     func: Callable[ParamT, Awaitable[ValueT_co]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
 ) -> ValueT_co:
-    """wait func using event.
+    """Wait for an event before executing an awaitable function.
+
+    like :func:`asyncio.wait_for`
 
     Args:
-        event: anyio event
-        func: awaitable func
+        event: An :obj:`anyio.Event` or an iterable of events.
+        func: An awaitable function to be executed.
 
     Returns:
-        func result
+        The result of the executed function.
 
-    how to use:
-    >>> import anyio
-    >>>
-    >>> from async_wrapper import wait_for
-    >>>
-    >>>
-    >>> async def test() -> None:
-    >>>     print("test: start")
-    >>>     await anyio.sleep(1)
-    >>>     print("test: end")
-    >>>
-    >>>
-    >>> async def test2(event: anyio.Event) -> None:
-    >>>     print("test2: start")
-    >>>     await event.wait()
-    >>>     print("test2: end")
-    >>>
-    >>>
-    >>> async def main() -> None:
-    >>>     event = anyio.Event()
-    >>>     async with anyio.create_task_group() as task_group:
-    >>>         task_group.start_soon(wait_for, event, test)
-    >>>         task_group.start_soon(test2, event)
-    >>>
-    >>>
-    >>> if __name__ == "__main__":
-    >>>     anyio.run(main)
-
-    output:
-    >>> $ poetry run python main.py
-    >>> test: start
-    >>> test2: start
-    >>> test: end
-    >>> test2: end
+    Example:
+        >>> import anyio
+        >>>
+        >>> from async_wrapper import wait_for
+        >>>
+        >>>
+        >>> async def test() -> None:
+        >>>     print("test: start")
+        >>>     await anyio.sleep(1)
+        >>>     print("test: end")
+        >>>
+        >>>
+        >>> async def test2(event: anyio.Event) -> None:
+        >>>     print("test2: start")
+        >>>     await event.wait()
+        >>>     print("test2: end")
+        >>>
+        >>>
+        >>> async def main() -> None:
+        >>>     event = anyio.Event()
+        >>>     async with anyio.create_task_group() as task_group:
+        >>>         task_group.start_soon(wait_for, event, test)
+        >>>         task_group.start_soon(test2, event)
+        >>>
+        >>>
+        >>> if __name__ == "__main__":
+        >>>     anyio.run(main)
+        $ poetry run python main.py
+        test: start
+        test2: start
+        test: end
+        test2: end
     """
     event = set(event) if not isinstance(event, Event) else (event,)
     try:
         return await func(*args, **kwargs)
     finally:
         for sub in event:
             sub.set()
```

### Comparing `async_wrapper-0.4.8/PKG-INFO` & `async_wrapper-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.8
+Version: 0.5.1
 Summary: async wrapper
-Home-page: https://github.com/phi-friday/async-wrapper
+Home-page: https://async-wrapper.readthedocs.io/
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

