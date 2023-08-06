# Comparing `tmp/superagent_py-0.0.42.tar.gz` & `tmp/superagent_py-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.42.tar", max compression
+gzip compressed data, was "superagent_py-0.0.43.tar", max compression
```

## Comparing `superagent_py-0.0.42.tar` & `superagent_py-0.0.43.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-08-05 11:22:14.235989 superagent_py-0.0.42/LICENSE
--rw-r--r--   0        0        0     3251 2023-08-05 11:22:14.235989 superagent_py-0.0.42/README.md
--rw-r--r--   0        0        0      380 2023-08-05 11:22:14.235989 superagent_py-0.0.42/pyproject.toml
--rw-r--r--   0        0        0      656 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/__init__.py
--rw-r--r--   0        0        0     3186 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-05 11:22:14.235989 superagent_py-0.0.42/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/py.typed
--rw-r--r--   0        0        0      361 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14615 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    12664 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/tags/__init__.py
--rw-r--r--   0        0        0    10575 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0    11638 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-08-05 11:22:14.239989 superagent_py-0.0.42/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-06 18:21:38.090294 superagent_py-0.0.43/LICENSE
+-rw-r--r--   0        0        0     3251 2023-08-06 18:21:38.090294 superagent_py-0.0.43/README.md
+-rw-r--r--   0        0        0      380 2023-08-06 18:21:38.090294 superagent_py-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14615 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-08-06 18:21:38.090294 superagent_py-0.0.43/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8684 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    12904 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-06 18:21:38.094294 superagent_py-0.0.43/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.43/PKG-INFO
```

### Comparing `superagent_py-0.0.42/LICENSE` & `superagent_py-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/README.md` & `superagent_py-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/__init__.py` & `superagent_py-0.0.43/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/client.py` & `superagent_py-0.0.43/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.43/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.43/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/agent/client.py` & `superagent_py-0.0.43/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.43/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.43/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.43/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/auth/client.py` & `superagent_py-0.0.43/src/superagent/resources/auth/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -70,14 +70,41 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def oauth_handler(
+        self, *, email: str, name: str, access_token: typing.Optional[str] = OMIT, provider: typing.Optional[str] = OMIT
+    ) -> typing.Any:
+        _request: typing.Dict[str, typing.Any] = {"email": email, "name": name}
+        if access_token is not OMIT:
+            _request["access_token"] = access_token
+        if provider is not OMIT:
+            _request["provider"] = provider
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/oauth/callback"),
+            json=jsonable_encoder(_request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncAuthClient:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
     async def sign_in(self, *, email: str, password: str) -> typing.Any:
@@ -121,14 +148,42 @@
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def oauth_handler(
+        self, *, email: str, name: str, access_token: typing.Optional[str] = OMIT, provider: typing.Optional[str] = OMIT
+    ) -> typing.Any:
+        _request: typing.Dict[str, typing.Any] = {"email": email, "name": name}
+        if access_token is not OMIT:
+            _request["access_token"] = access_token
+        if provider is not OMIT:
+            _request["provider"] = provider
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment}/", "api/v1/auth/oauth/callback"),
+                json=jsonable_encoder(_request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `superagent_py-0.0.42/src/superagent/resources/documents/client.py` & `superagent_py-0.0.43/src/superagent/resources/documents/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,24 +40,27 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_document(
         self,
         *,
         type: str,
         url: typing.Optional[str] = OMIT,
+        content: typing.Optional[str] = OMIT,
         name: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         from_page: typing.Optional[int] = OMIT,
         to_page: typing.Optional[int] = OMIT,
         splitter: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"type": type, "name": name}
         if url is not OMIT:
             _request["url"] = url
+        if content is not OMIT:
+            _request["content"] = content
         if authorization is not OMIT:
             _request["authorization"] = authorization
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if from_page is not OMIT:
             _request["from_page"] = from_page
         if to_page is not OMIT:
@@ -166,24 +169,27 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_document(
         self,
         *,
         type: str,
         url: typing.Optional[str] = OMIT,
+        content: typing.Optional[str] = OMIT,
         name: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         from_page: typing.Optional[int] = OMIT,
         to_page: typing.Optional[int] = OMIT,
         splitter: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"type": type, "name": name}
         if url is not OMIT:
             _request["url"] = url
+        if content is not OMIT:
+            _request["content"] = content
         if authorization is not OMIT:
             _request["authorization"] = authorization
         if metadata is not OMIT:
             _request["metadata"] = metadata
         if from_page is not OMIT:
             _request["from_page"] = from_page
         if to_page is not OMIT:
```

### Comparing `superagent_py-0.0.42/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.43/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/tags/client.py` & `superagent_py-0.0.43/src/superagent/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/tools/client.py` & `superagent_py-0.0.43/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/traces/client.py` & `superagent_py-0.0.43/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/resources/user/client.py` & `superagent_py-0.0.43/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.43/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/src/superagent/types/validation_error.py` & `superagent_py-0.0.43/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.42/PKG-INFO` & `superagent_py-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.42
+Version: 0.0.43
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

