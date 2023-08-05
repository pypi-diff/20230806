# Comparing `tmp/openrpc-7.0.2.tar.gz` & `tmp/openrpc-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrpc-7.0.2.tar", max compression
+gzip compressed data, was "openrpc-7.2.0.tar", max compression
```

## Comparing `openrpc-7.0.2.tar` & `openrpc-7.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-07-28 19:04:29.147665 openrpc-7.0.2/LICENSE
--rw-r--r--   0        0        0     3255 2023-07-28 19:04:29.147665 openrpc-7.0.2/README.md
--rw-r--r--   0        0        0     1045 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/__init__.py
--rw-r--r--   0        0        0      183 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_depends.py
--rw-r--r--   0        0        0        0 2023-07-28 19:04:29.171665 openrpc-7.0.2/openrpc/_discover/__init__.py
--rw-r--r--   0        0        0     4266 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_discover/_methods.py
--rw-r--r--   0        0        0     6112 2023-07-28 19:04:29.147665 openrpc-7.0.2/openrpc/_discover/_schemas.py
--rw-r--r--   0        0        0     1289 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_discover/discover.py
--rw-r--r--   0        0        0     7862 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_method_processor.py
--rw-r--r--   0        0        0     6235 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_method_registrar.py
--rw-r--r--   0        0        0     9417 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_objects.py
--rw-r--r--   0        0        0     7616 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_request_processor.py
--rw-r--r--   0        0        0      280 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_router.py
--rw-r--r--   0        0        0     1168 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_rpcmethod.py
--rw-r--r--   0        0        0     9267 2023-07-28 19:04:29.148665 openrpc-7.0.2/openrpc/_server.py
--rw-r--r--   0        0        0        0 2023-07-28 19:04:29.172665 openrpc-7.0.2/openrpc/py.typed
--rw-r--r--   0        0        0     1477 2023-07-28 19:04:29.148665 openrpc-7.0.2/pyproject.toml
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 openrpc-7.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-05 21:04:36.552772 openrpc-7.2.0/LICENSE
+-rw-r--r--   0        0        0     2018 2023-08-05 21:04:36.552772 openrpc-7.2.0/README.md
+-rw-r--r--   0        0        0     1045 2023-08-05 21:04:36.555772 openrpc-7.2.0/openrpc/__init__.py
+-rw-r--r--   0        0        0      183 2023-08-05 21:04:36.555772 openrpc-7.2.0/openrpc/_depends.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:04:36.582772 openrpc-7.2.0/openrpc/_discover/__init__.py
+-rw-r--r--   0        0        0     4631 2023-08-05 21:04:36.555772 openrpc-7.2.0/openrpc/_discover/_methods.py
+-rw-r--r--   0        0        0     6110 2023-08-05 21:04:36.555772 openrpc-7.2.0/openrpc/_discover/_schemas.py
+-rw-r--r--   0        0        0     1287 2023-08-05 21:04:36.555772 openrpc-7.2.0/openrpc/_discover/discover.py
+-rw-r--r--   0        0        0     8541 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_method_processor.py
+-rw-r--r--   0        0        0     5917 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_method_registrar.py
+-rw-r--r--   0        0        0     9417 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_objects.py
+-rw-r--r--   0        0        0     7616 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_request_processor.py
+-rw-r--r--   0        0        0      280 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_router.py
+-rw-r--r--   0        0        0     1168 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_rpcmethod.py
+-rw-r--r--   0        0        0     9361 2023-08-05 21:04:36.556772 openrpc-7.2.0/openrpc/_server.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:04:36.582772 openrpc-7.2.0/openrpc/py.typed
+-rw-r--r--   0        0        0     1477 2023-08-05 21:04:36.556772 openrpc-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 openrpc-7.2.0/PKG-INFO
```

### Comparing `openrpc-7.0.2/LICENSE` & `openrpc-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.2/README.md` & `openrpc-7.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,68 @@
-<div align=center>
-  <h1>OpenRPC</h1>
-  <h3>Transport agnostic framework for developing
-  <a href="https://open-rpc.org">OpenRPC</a> servers.</h3>
-  <img src="https://img.shields.io/badge/License-MIT-blue.svg"
-   height="20"
-   alt="License: MIT">
-  <img src="https://img.shields.io/badge/code%20style-black-000000.svg"
-   height="20"
-   alt="Code style: black">
-  <img src="https://img.shields.io/pypi/v/openrpc.svg"
-   height="20"
-   alt="PyPI version">
-  <img src="https://img.shields.io/badge/coverage-100%25-success"
-   height="20"
-   alt="Code Coverage">
-  <a href="https://gitlab.com/mburkard/openrpc/-/blob/main/CONTRIBUTING.md">
-    <img src="https://img.shields.io/static/v1.svg?label=Contributions&message=Welcome&color=2267a0"
-     height="20"
-     alt="Contributions Welcome">
-  </a>
-</div>
+Metadata-Version: 2.1
+Name: openrpc
+Version: 7.2.0
+Summary: Transport agnostic framework for developing OpenRPC servers.
+Home-page: https://gitlab.com/mburkard/openrpc
+License: MIT
+Author: Matthew Burkard
+Author-email: matthewjburkard@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: jsonrpc2-objects (>=3.0.0,<4.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Project-URL: Repository, https://gitlab.com/mburkard/openrpc
+Description-Content-Type: text/markdown
+
+# Python OpenRPC
+
+![](https://img.shields.io/badge/License-MIT-blue.svg)
+![](https://img.shields.io/badge/code%20style-black-000000.svg)
+![](https://img.shields.io/pypi/v/openrpc.svg)
+![](https://img.shields.io/badge/coverage-100%25-success)
+
+**Documentation**: https://python-openrpc.burkard.cloud
+
+**Source Code**: https://gitlab.com/mburkard/openrpc
+
+Python OpenRPC is a transport agnostic framework for quickly and easily
+developing [OpenRPC](https://open-rpc.org/) servers in Python.
+
+## Requirements
+
+- Python 3.9+
+- [Pydantic](https://docs.pydantic.dev/latest/) for data models.
 
 ## Installation
 
 OpenRPC is on PyPI and can be installed with:
 
 ```shell
 pip install openrpc
 ```
 
+Or with [Poetry](https://python-poetry.org/)
+
 ```shell
 poetry add openrpc
 ```
 
-## Usage
-
-This library provides an `RPCServer` class that can be used to quickly create an OpenRPC
-Server.
-
-```python
-from openrpc import RPCServer
-
-rpc = RPCServer(title="Demo Server", version="1.0.0")
-```
-
-### Register a function as an RPC Method
-
-To register a method with the RPCServer add the `@rpc.method()` decorator to a function.
-
-```python
-@rpc.method()
-def add(a: int, b: int) -> int:
-    return a + b
-```
-
-### Process JSON RPC Request
+## Example
 
-OpenRPC is transport agnostic. To use it, pass JSON RPC requests as strings or byte
-strings to the `process_request` or `process_request_async` method.
-
-The `process_request` will return a JSON RPC response as a string.
-
-```python
-req = """
-{
-  "id": 1,
-  "method": "add",
-  "params": {"a": 2, "b": 2},
-  "jsonrpc": "2.0"
-}
-"""
-await rpc.process_request_async(req)
-# returns -> '{"id": 1, "result": 4, "jsonrpc": "2.0"}'
-```
-
-### Pydantic Support
-
-For data classes to work properly use Pydantic. RPCServer will use Pydantic for JSON
-serialization/deserialization when calling methods and when generating schemas
-with `rpc.discover`.
-
-### RPC Discover
-
-The `rpc.discover` method is automatically generated. It relies heavily on type hints.
-
-## Example Using Sanic
-
-A quick example using `OpenRPC` exposing the methods
-using a [Sanic](https://sanic.dev/en/) websocket server.
+This is a minimal OpenRPC server using a [Sanic](https://sanic.dev/en/) websocket server
+as the transport method.
 
 ```python
 from openrpc import RPCServer
 from sanic import Request, Sanic, Websocket
 
 app = Sanic("DemoServer")
 rpc = RPCServer(title="DemoServer", version="1.0.0")
@@ -134,15 +105,20 @@
 {
   "id": 1,
   "result": 4,
   "jsonrpc": "2.0"
 }
 ```
 
-## Support The Developer
+## Template App
+
+You can bootstrap your OpenRPC server by cloning the
+[template app](https://gitlab.com/mburkard/openrpc-app-template).
+
+## Support the Developer
 
 <a href="https://www.buymeacoffee.com/mburkard" target="_blank">
-  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png"
+  <img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me a Coffee"
        width="217"
-       height="60"
-       alt="Buy Me A Coffee">
+       height="60"/>
 </a>
+
```

### Comparing `openrpc-7.0.2/openrpc/__init__.py` & `openrpc-7.2.0/openrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.2/openrpc/_discover/_methods.py` & `openrpc-7.2.0/openrpc/_discover/_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-"""Module for generating Open-RPC document methods."""
+"""Module for generating OpenRPC document methods."""
 
 import inspect
 from typing import (
     Any,
     Callable,
     get_args,
     get_origin,
     get_type_hints,
     Iterable,
+    Optional,
     Type,
     Union,
 )
 
-from openrpc._rpcmethod import RPCMethod
 from openrpc import ContentDescriptorObject, Depends, MethodObject, SchemaObject
+from openrpc._rpcmethod import RPCMethod
 
 NoneType = type(None)
 
 
 def get_methods(
     rpc_methods: Iterable[RPCMethod], type_schema_map: dict[Type, SchemaObject]
 ) -> list[MethodObject]:
-    """Get Open-RPC method objects.
+    """Get OpenRPC method objects.
 
     :param rpc_methods: Decorated functions data.
     :param type_schema_map: Type to Schema map.
-    :return: Open-RPC method objects.
+    :return: OpenRPC method objects.
     """
     return [
         MethodObject(
             name=rpc.metadata.name or rpc.function.__name__,
             params=rpc.metadata.params or _get_params(rpc.function, type_schema_map),
             result=rpc.metadata.result or _get_result(rpc.function, type_schema_map),
             tags=rpc.metadata.tags,
             summary=rpc.metadata.summary,
-            description=rpc.metadata.description,
+            description=_get_description(rpc),
             externalDocs=rpc.metadata.external_docs,
             deprecated=rpc.metadata.deprecated,
             servers=rpc.metadata.servers,
             errors=rpc.metadata.errors,
             links=rpc.metadata.links,
             paramStructure=rpc.metadata.param_structure,
             examples=rpc.metadata.examples,
@@ -136,7 +137,17 @@
     if origin in flat_collections or annotation in flat_collections:
         return "array"
     if dict in [origin, annotation]:
         return "object"
     if NoneType is annotation:
         return "null"
     return py_to_schema.get(annotation) or "object"
+
+
+def _get_description(rpc_method: RPCMethod) -> Optional[str]:
+    description = rpc_method.metadata.description
+    if not description:
+        description = rpc_method.function.__doc__
+        # If using function doc as description only take intro line.
+        if description:
+            description = description.split("\n")[0]
+    return description
```

### Comparing `openrpc-7.0.2/openrpc/_discover/_schemas.py` & `openrpc-7.2.0/openrpc/_discover/_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module for generating Open-RPC document model and enum schemas."""
+"""Module for generating OpenRPC document model and enum schemas."""
 
 import inspect
 from enum import Enum
 from typing import (
     Any,
     Callable,
     get_args,
@@ -131,15 +131,15 @@
     # noinspection PydanticTypeChecker
     return isinstance(type_, Type) and issubclass(type_, BaseModel)  # type: ignore
 
 
 def _get_flattened_schemas(
     type_to_schema_map: dict[Type, SchemaObject]
 ) -> dict[Type, SchemaObject]:
-    # Pydantic uses $defs which do not work in Open-RPC playground,
+    # Pydantic uses $defs which do not work in OpenRPC playground,
     # a number of alterations to Pydantic generated schemas need to be
     # made.
     schemas = {}
     for type_, schema in type_to_schema_map.items():
         flat_schema = schema
 
         # Move allOf item to top-level.
```

### Comparing `openrpc-7.0.2/openrpc/_discover/discover.py` & `openrpc-7.2.0/openrpc/_discover/discover.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 def get_openrpc_doc(
     info: InfoObject, rpc_methods: Iterable[RPCMethod]
 ) -> OpenRPCObject:
     """Get an Open RPC document describing the RPC server.
 
     :param info: RPC server info.
     :param rpc_methods: RPC server methods.
-    :return: The Open-RPC doc for the given server.
+    :return: The OpenRPC doc for the given server.
     """
     type_schema_map = get_type_to_schema_map([rpc.function for rpc in rpc_methods])
     components = ComponentsObject(
         schemas={v.title or "": v for v in type_schema_map.values()}
     )
 
     return OpenRPCObject(
         **json.loads(
             OpenRPCObject(
                 openrpc="1.2.6",
                 info=info,
                 methods=get_methods(rpc_methods, type_schema_map),
                 components=components,
             ).model_dump_json(by_alias=True, exclude_unset=True)
-            # Workaround to Open-RPC playground bug resolving definitions.
+            # Workaround to OpenRPC playground bug resolving definitions.
             .replace("#/$defs/", "#/components/schemas/")
         )
     )
```

### Comparing `openrpc-7.0.2/openrpc/_method_processor.py` & `openrpc-7.2.0/openrpc/_method_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Module responsible for processing a method call."""
 
 __all__ = ("MethodProcessor",)
 
 import inspect
 import logging
+import traceback
 from enum import Enum
+from pathlib import Path
 from typing import (
     Any,
     get_args,
     get_origin,
     get_type_hints,
     Optional,
     Type,
@@ -126,15 +128,15 @@
         params: Optional[Union[dict, list]]
         params_msg = ""
         missing_dependencies = [
             k for k in self.method.depends_params if k not in self.depends
         ]
         if missing_dependencies:
             raise AttributeError(
-                "Missing dependent values %s  for method [%s]"
+                "Missing dependent values %s for method [%s]"
                 % (missing_dependencies, self.method.metadata.name)
             )
         dependencies = {k: self.depends.get(k) for k in self.method.depends_params}
         # Call method.
         if isinstance(self.request, (Request, Notification)):
             result = self.method.function(**dependencies)
         elif isinstance(self.request.params, list):
@@ -168,18 +170,19 @@
 
         if isinstance(error, JSONRPCError):
             return ErrorResponse(
                 id=self.request.id, error=error.rpc_error
             ).model_dump_json()
 
         if self.debug:
+            traceback_str = _get_trimmed_traceback(error)
             error_object: ErrorType = DataError(
                 code=self.uncaught_error_code,
                 message="Server error",
-                data=f"{type(error).__name__}: {error}",
+                data=f"{type(error).__name__}: {error}\n{traceback_str}",
             )
         else:
             error_object = Error(code=self.uncaught_error_code, message="Server error")
 
         return ErrorResponse(id=self.request.id, error=error_object).model_dump_json()
 
     def _get_list_params(self, params: list, annotations: dict) -> list:
@@ -218,7 +221,19 @@
                 return [self._deserialize_param(it, types[0]) for it in param]
             try:
                 return p_type(**param)
             except (TypeError, AttributeError, KeyError):
                 return p_type(param)
         except (TypeError, AttributeError, KeyError, ValueError):
             return NotDeserialized
+
+
+def _get_trimmed_traceback(error: Exception) -> str:
+    tb = traceback.extract_tb(error.__traceback__)
+    # Remove framework inner workings from traceback.
+    file_path = Path(__file__).resolve()
+    external_tb = [frame for frame in tb if Path(frame.filename).resolve() != file_path]
+
+    # Format the external traceback into a string
+    external_traceback_string = "".join(traceback.format_list(external_tb))
+    exception_message = "".join(traceback.format_exception_only(type(error), error))
+    return f"{external_traceback_string}{exception_message}"
```

### Comparing `openrpc-7.0.2/openrpc/_method_registrar.py` & `openrpc-7.2.0/openrpc/_method_registrar.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,14 @@
         errors: Optional[list[ErrorObject]] = None,
         links: Optional[list[LinkObject]] = None,
         param_structure: Optional[ParamStructure] = None,
         examples: Optional[list[ExamplePairingObject]] = None,
     ) -> Union[CallableType, Callable[[DecoratedCallableType], DecoratedCallableType]]:
         """Register a method with this OpenRPC server.
 
-        Can be used as a plain decorator, eg:
-
-        .. code-block:: python
-
-            @method
-            def my_func()
-
-        Or additional method info can be provided with a MethodObject:
-
-        .. code-block:: python
-
-            @method(name="dot.case.method", deprecated=True)
-            def my_func()
-
         :param args: The method if this is used as a plain decorator.
         :param name: The canonical name for the method.
         :param params: A list of parameters that are applicable for this
             method.
         :param result: The description of the result returned by the
             method.
         :param tags: A list of tags for API documentation control.
```

### Comparing `openrpc-7.0.2/openrpc/_objects.py` & `openrpc-7.2.0/openrpc/_objects.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.2/openrpc/_request_processor.py` & `openrpc-7.2.0/openrpc/_request_processor.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.2/openrpc/_rpcmethod.py` & `openrpc-7.2.0/openrpc/_rpcmethod.py`

 * *Files identical despite different names*

### Comparing `openrpc-7.0.2/openrpc/_server.py` & `openrpc-7.2.0/openrpc/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         version: Optional[str] = None,
         description: Optional[str] = None,
         terms_of_service: Optional[str] = None,
         contact: Optional[ContactObject] = None,
         license_: Optional[LicenseObject] = None,
         debug: bool = False,  # noqa: FBT001,FBT002
     ) -> None:
-        """Init an Open-RPC server.
+        """Init an OpenRPC server.
 
-        :param title: Open-RPC title.
+        :param title: OpenRPC title.
         :param version: API version.
         :param description: Description of the app.
         :param terms_of_service: App terms of service.
         :param contact: Contact information.
         :param license_: App license.
         :param debug: Include internal error details in responses.
         """
@@ -207,15 +207,16 @@
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
 
         :param data: A JSON-RPC2 request.
         :param depends: Values passed to functions with dependencies.
             Values will be passed if the keyname matches the arg name
             that is a dependency.
-        :return: A valid JSON-RPC2 response.
+        :return: A JSON-RPC2 response or None if the request was a
+            notification.
         """
         try:
             log.debug("Processing request: %s", data)
             resp = self._request_processor.process(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
             return resp  # noqa: TRY300
@@ -229,15 +230,16 @@
 
         If the method called by the request is async it will be awaited.
 
         :param data: A JSON-RPC2 request.
         :param depends: Values passed to functions with dependencies.
             Values will be passed if the keyname matches the arg name
             that is a dependency.
-        :return: A valid JSON-RPC2 response.
+        :return: A JSON-RPC2 response or None if the request was a
+            notification.
         """
         try:
             log.debug("Processing request: %s", data)
             resp = await self._request_processor.process_async(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
             return resp  # noqa: TRY300
```

### Comparing `openrpc-7.0.2/pyproject.toml` & `openrpc-7.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrpc"
-version = "7.0.2"
+version = "7.2.0"
 description = "Transport agnostic framework for developing OpenRPC servers."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/openrpc"
 homepage = "https://gitlab.com/mburkard/openrpc"
 license = "MIT"
 authors = ["Matthew Burkard <matthewjburkard@gmail.com>"]
 classifiers = [
@@ -26,15 +26,15 @@
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.1.0"
 mypy = "^1.0.0"
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.21.0"
-ruff = "^0.0.280"
+ruff = "^0.0.282"
 
 [build-system]
 
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

