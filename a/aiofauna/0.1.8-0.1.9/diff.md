# Comparing `tmp/aiofauna-0.1.8.tar.gz` & `tmp/aiofauna-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.8.tar", max compression
+gzip compressed data, was "aiofauna-0.1.9.tar", max compression
```

## Comparing `aiofauna-0.1.8.tar` & `aiofauna-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.8/LICENSE
--rwxr-xr-x   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.8/README.md
--rwxr-xr-x   0        0        0     3698 2023-05-11 08:26:07.398242 aiofauna-0.1.8/aiofauna/__init__.py
--rwxr-xr-x   0        0        0    16796 2023-05-11 08:26:00.406228 aiofauna-0.1.8/aiofauna/api.py
--rwxr-xr-x   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.8/aiofauna/asgi.py
--rwxr-xr-x   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.8/aiofauna/client.py
--rwxr-xr-x   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.8/aiofauna/datastructures.py
--rwxr-xr-x   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.8/aiofauna/deprecated.py
--rwxr-xr-x   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.8/aiofauna/errors.py
--rwxr-xr-x   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.8/aiofauna/helpers.py
--rwxr-xr-x   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.8/aiofauna/json.py
--rwxr-xr-x   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.8/aiofauna/objects.py
--rwxr-xr-x   0        0        0    21874 2023-05-11 21:04:02.733525 aiofauna-0.1.8/aiofauna/odm.py
--rwxr-xr-x   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.8/aiofauna/page.py
--rwxr-xr-x   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.8/aiofauna/query.py
--rwxr-xr-x   0        0        0      661 2023-05-11 08:23:40.249922 aiofauna-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3597 2023-05-11 21:05:02.670231 aiofauna-0.1.8/setup.py
--rw-r--r--   0        0        0     3697 2023-05-11 21:05:02.671110 aiofauna-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0     2680 2023-05-13 04:15:02.851110 aiofauna-0.1.9/README.md
+-rwxr-xr-x   0        0        0     3698 2023-05-11 08:26:07.398242 aiofauna-0.1.9/aiofauna/__init__.py
+-rwxr-xr-x   0        0        0    17979 2023-05-13 07:43:45.897504 aiofauna-0.1.9/aiofauna/api.py
+-rwxr-xr-x   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.9/aiofauna/asgi.py
+-rwxr-xr-x   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.9/aiofauna/client.py
+-rwxr-xr-x   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.9/aiofauna/datastructures.py
+-rwxr-xr-x   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.9/aiofauna/deprecated.py
+-rwxr-xr-x   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.9/aiofauna/errors.py
+-rwxr-xr-x   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.9/aiofauna/helpers.py
+-rwxr-xr-x   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.9/aiofauna/json.py
+-rwxr-xr-x   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.9/aiofauna/objects.py
+-rwxr-xr-x   0        0        0    21874 2023-05-11 21:04:02.733525 aiofauna-0.1.9/aiofauna/odm.py
+-rwxr-xr-x   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.9/aiofauna/page.py
+-rwxr-xr-x   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.9/aiofauna/query.py
+-rwxr-xr-x   0        0        0      661 2023-05-13 08:01:20.376072 aiofauna-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3601 2023-05-13 08:01:58.200949 aiofauna-0.1.9/setup.py
+-rw-r--r--   0        0        0     3699 2023-05-13 08:01:58.201685 aiofauna-0.1.9/PKG-INFO
```

### Comparing `aiofauna-0.1.8/LICENSE` & `aiofauna-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/README.md` & `aiofauna-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,7 +40,9 @@
 📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)
 
 📦 [PyPi](https://pypi.org/project/aiofauna/)
 
 📦 [GitHub](https://github.com/obahamonde/aiofauna)
 
 📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)
+
+
```

### Comparing `aiofauna-0.1.8/aiofauna/__init__.py` & `aiofauna-0.1.9/aiofauna/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/api.py` & `aiofauna-0.1.9/aiofauna/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 """REST API Module with automatic OpenAPI generation."""
+from __future__ import annotations
 import json
 import base64
 import asyncio
 from json import JSONDecoder
 from typing import Any, Dict, List, Union
 from inspect import signature
 from uuid import UUID
 from datetime import datetime, date, time
 from functools import singledispatch
 from enum import Enum
+from dataclasses import dataclass
+import uuid
 from aiohttp.web import Application, Request, Response, json_response
 from aiohttp.web_request import FileField
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
+from multidict import CIMultiDict   
 from .json import FaunaJSONEncoder, parse_json_or_none
 from .odm import AsyncFaunaModel
 
+
+
+class UploadFile(BaseModel):
+    """
+    File Upload Model
+    """
+
+    filename: str
+    content_type: str
+    data: bytes
+    size: int
+    headers: Dict[str, str]
+
+        
+            
 def jsonable_encoder(
     obj: Any,
     *,
     include: List[str] = [],
     exclude: List[str] = [],
     by_alias: bool = False,
     skip_defaults: bool = False,
@@ -140,109 +159,129 @@
             open_api_params[name] = {
                 "in": param_location,
                 "name": name,
                 "required": True,
                 "schema": {"type": type_, "default": param.default, "required": True},
             }
 
-        elif issubclass(type_, (BaseModel, AsyncFaunaModel)):
+        elif type_ in [UploadFile, FileField]:
             open_api_params[name] = {
-                "in": "body",
-                "name": name,
-                "required": True,
-                "schema": type_.schema(),
+        "in": "formData",
+        "name": name,
+        "required": True,
+        "schema": {"type": "file", "format": "binary"},
+        "consumes": ["multipart/form-data"],
+        "headers": {
+            "Content-Type": {
+                "type": "string",
+                "default": "multipart/form-data"
             }
-
-        elif issubclass(type_, FileField):
+        }
+    }
+        
+        
+        elif issubclass(type_, (BaseModel, AsyncFaunaModel)) and type_ != UploadFile:
             open_api_params[name] = {
-                "in": "formData",
+                "in": "body",
                 "name": name,
                 "required": True,
-                "schema": {"type": "file"},
+                "schema": type_.schema(),
             }
 
+        
         else:
             continue
 
     return open_api_params
 
 
 def update_open_api(
     open_api: Dict[str, Any],
     path: str,
     method: str,
     func: Any,
     open_api_params: Dict[str, Any],
 ) -> None:
-    """
-    Helper function to update the open_api dictionary with the parameters of a function.
-    """
     if path in ["/openapi.json", "/docs"]:
         return
 
-    if method in ("GET", "HEAD", "DELETE"):
+    _scalars = []
+    _body = None
+    _is_file_upload = False
+
+    for param in open_api_params.values():
+        if isinstance(param["schema"], dict):
+            if "type" in param["schema"] and param["schema"]["type"] != "object":
+                _scalars.append(param)
+            else:
+                _body = {
+                    "content": {"application/json": {"schema": param["schema"]}}
+                }
+        elif param["in"] == "formData" and param["schema"]["type"] == "file":
+            _is_file_upload = True
+            _scalars.append(param)
+        else:
+            continue
+
+    if _body:
+        open_api["paths"].setdefault(path, {})[method.lower()] = {
+        "summary": func.__name__,
+        "description": func.__doc__,
+        "parameters": _scalars,
+        "requestBody": _body if not _is_file_upload else {
+            "content": {
+                "multipart/form-data": {
+                    "schema": {
+                        "properties": {
+                            "file": {
+                                "type": "array",
+                                "items": {
+                                    "type": "string",
+                                    "format": "binary"
+                                }
+                            }
+                        }
+                    }
+                }
+            }
+        },
+        "responses": {"200": {"description": "OK"}},
+    }
+        open_api["components"]["schemas"].update(param["schema"])  # type: ignore
+    else:
         open_api["paths"].setdefault(path, {})[method.lower()] = {
             "summary": func.__name__,
             "description": func.__doc__,
-            "parameters": list(open_api_params.values()),
+            "parameters": _scalars,
             "responses": {"200": {"description": "OK"}},
         }
-    elif method in ("POST", "PUT", "PATCH"):
-        _scalars = []
-        _body = None
-        for param in open_api_params.values():
-            if isinstance(param["schema"], dict):
-                if "type" in param["schema"] and param["schema"]["type"] != "object":
-                    _scalars.append(param)
-                else:
-                    _body = {
-                        "content": {"application/json": {"schema": param["schema"]}}
-                    }
-            else:
-                continue
-
-        if _body:
-            open_api["paths"].setdefault(path, {})[method.lower()] = {
-                "summary": func.__name__,
-                "description": func.__doc__,
-                "parameters": _scalars,
-                "requestBody": _body,
-                "responses": {"200": {"description": "OK"}},
-            }
-            open_api["components"]["schemas"].update(param["schema"])  # type: ignore
-
-        else:
-            open_api["paths"].setdefault(path, {})[method.lower()] = {
-                "summary": func.__name__,
-                "description": func.__doc__,
-                "parameters": _scalars,
-                "responses": {"200": {"description": "OK"}},
-            }
-
-
-
+        
 async def inject_signature(request: Request, params: dict):
     """
     FastAPIesque function to shape the signature of a function to the request.
     """
     args_to_apply = {}
 
     for name, param in params.items():
-        type_ = param.annotation
-        if type_ in (str, int, float, bool) and name in request.match_info:
+        annotation = param.annotation
+        if annotation in (str, int, float, bool) and name in request.match_info:
             args_to_apply[name] = request.match_info[name]
-        elif type_ in (str, int, float, bool) and name in request.query:
-            args_to_apply[name] = type_(request.query[name])
-        elif issubclass(type_, BaseModel):
+        elif annotation in (str, int, float, bool) and name in request.query:
+            args_to_apply[name] = annotation(request.query[name])
+        elif annotation in [FileField, UploadFile]:
+                headers = dict(request.headers)
+                new_headers = CIMultiDict(**headers, **{"content-type": "multipart/form-data"})
+                new_request = request.clone(headers=new_headers)
+                print(new_request.has_body)
+                args_to_apply[name] = new_request
+        elif issubclass(annotation, BaseModel):
             data = await request.json(loads=JSONDecoder().decode)
             if isinstance(data, Union[str,bytes]):
                 data = json.loads(data, object_hook=parse_json_or_none)
-            args_to_apply[name] = type_(**data)
-        elif issubclass(type_, FileField):
-            args_to_apply[name] = await request.post()
+            args_to_apply[name] = annotation(**data)
         else:
             continue
     return args_to_apply
 
 
 @singledispatch
 def do_response(response: Any) -> Response:
@@ -340,16 +379,14 @@
     return Response(
         status=200,
         body=json.dumps(processed_response),
         content_type="application/json",
     )
 
 
-
-
 class Api(Application):
     """
 
     Api class to create a fastapi-like api.
 
     """
 
@@ -383,15 +420,21 @@
                 <style>
                 html
                 {{
                     box-sizing: border-box;
                     overflow: -moz-scrollbars-vertical;
                     overflow-y: scroll;
                 }}
-
+                
+                .swagger-ui .topbar
+                {{
+                    display: none;
+                }}
+                    
+                    
                 *,
                 *:before,
                 *:after
                 {{
                     box-sizing: inherit;
                 }}
```

### Comparing `aiofauna-0.1.8/aiofauna/asgi.py` & `aiofauna-0.1.9/aiofauna/asgi.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/client.py` & `aiofauna-0.1.9/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/datastructures.py` & `aiofauna-0.1.9/aiofauna/datastructures.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/errors.py` & `aiofauna-0.1.9/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/helpers.py` & `aiofauna-0.1.9/aiofauna/helpers.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/json.py` & `aiofauna-0.1.9/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/objects.py` & `aiofauna-0.1.9/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/odm.py` & `aiofauna-0.1.9/aiofauna/odm.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/page.py` & `aiofauna-0.1.9/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/aiofauna/query.py` & `aiofauna-0.1.9/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.8/pyproject.toml` & `aiofauna-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 repository = "https://github.com/obahamonde/aiofauna"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `aiofauna-0.1.8/setup.py` & `aiofauna-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'aiohttp>=3.8.4,<4.0.0',
  'aiohttp_cors>=0.7.0,<0.8.0',
  'iso8601>=1.1.0,<2.0.0',
  'pydantic[dotenv]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
-    'long_description': '---\ntitle: AioFauna\n---\n# AioFauna\n\n🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.\n\n🔥 Inspired by FastAPI focuses on Developer Experience, Productivity and Versatility.\n\n🌟 Features:\n\n✅ Supports Python 3.7+, comes with an opinionated ODM (Object Document Mapper) out of the box for FaunaDB that abstracts out complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.\n\n✅ Performant and scalable: Built on top of Aiohttp a powerful http server and client and FaunaDB an scalable serverless database for modern applications.\n\n✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness, being ASGI compliant is compatible with most async python frameworks.\n\n✅ Automatic Swagger UI generation: Automatic generation of interactive Swagger UI documentation for instant testing of your API.\n\n✅ SSE (Server Sent Events): Built-in support for SSE (Server Sent Events) for real-time streaming of data from FaunaDB to your application.\n\n✅ Robust data validation: Built-in support for Pydantic models for robust data validation and serialization.\n\n✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections with FaunaModel ODM.\n\n✅ Full JSON communication: Custom encoder to ensure seamless data exchange between your application and FaunaDB backend.\n\n✅ Markdown and Jinja support with live reload: experiment an smooth frontend devserver experience without leaving your backend code.\n\n✅ Inspired by fastapi, you will work with almost the same syntax and features like path operations, path parameters, query parameters, request body, status codes and more.\n\n💡 With aiofauna, you can build fast, scalable, and reliable modern applications, while building seamless integrations thanks to the fastest http client aiohttp and the most versatile database FaunaDB, you will enjoy integrating with third party services such as APIs, Data Sources and Cloud Services.\n\n📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀\n\n#Python #FaunaDB #Async #Pydantic #aiofauna\n\n⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.\n\n📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)\n\n📦 [PyPi](https://pypi.org/project/aiofauna/)\n\n📦 [GitHub](https://github.com/obahamonde/aiofauna)\n\n📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)\n',
+    'long_description': '---\ntitle: AioFauna\n---\n# AioFauna\n\n🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.\n\n🔥 Inspired by FastAPI focuses on Developer Experience, Productivity and Versatility.\n\n🌟 Features:\n\n✅ Supports Python 3.7+, comes with an opinionated ODM (Object Document Mapper) out of the box for FaunaDB that abstracts out complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.\n\n✅ Performant and scalable: Built on top of Aiohttp a powerful http server and client and FaunaDB an scalable serverless database for modern applications.\n\n✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness, being ASGI compliant is compatible with most async python frameworks.\n\n✅ Automatic Swagger UI generation: Automatic generation of interactive Swagger UI documentation for instant testing of your API.\n\n✅ SSE (Server Sent Events): Built-in support for SSE (Server Sent Events) for real-time streaming of data from FaunaDB to your application.\n\n✅ Robust data validation: Built-in support for Pydantic models for robust data validation and serialization.\n\n✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections with FaunaModel ODM.\n\n✅ Full JSON communication: Custom encoder to ensure seamless data exchange between your application and FaunaDB backend.\n\n✅ Markdown and Jinja support with live reload: experiment an smooth frontend devserver experience without leaving your backend code.\n\n✅ Inspired by fastapi, you will work with almost the same syntax and features like path operations, path parameters, query parameters, request body, status codes and more.\n\n💡 With aiofauna, you can build fast, scalable, and reliable modern applications, while building seamless integrations thanks to the fastest http client aiohttp and the most versatile database FaunaDB, you will enjoy integrating with third party services such as APIs, Data Sources and Cloud Services.\n\n📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀\n\n#Python #FaunaDB #Async #Pydantic #aiofauna\n\n⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.\n\n📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)\n\n📦 [PyPi](https://pypi.org/project/aiofauna/)\n\n📦 [GitHub](https://github.com/obahamonde/aiofauna)\n\n📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)\n\n\n',
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/obahamonde/aiofauna',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aiofauna-0.1.8/PKG-INFO` & `aiofauna-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/obahamonde/aiofauna
 License: MIT
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -68,7 +68,9 @@
 
 📦 [PyPi](https://pypi.org/project/aiofauna/)
 
 📦 [GitHub](https://github.com/obahamonde/aiofauna)
 
 📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)
 
+
+
```

