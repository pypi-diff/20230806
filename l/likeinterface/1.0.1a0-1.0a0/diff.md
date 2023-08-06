# Comparing `tmp/likeinterface-1.0.1a0.tar.gz` & `tmp/likeinterface-1.0a0.tar.gz`

## Comparing `likeinterface-1.0.1a0.tar` & `likeinterface-1.0a0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/Makefile
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/.github/dependabot.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/licenses/LICENSE.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/__meta__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/constants.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/exceptions.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/interface.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/network.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/session.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/__init__.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/base.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/auth/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/auth/get_authorization_information.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/auth/get_user_information.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/auth/root_auth.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/auth/sign_in.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/like/__init__.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/like/evaluator.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/methods/like/root_like.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/base.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/auth/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/auth/authorization.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/auth/user.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/like/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/types/like/hand.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/utils/__init__.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/utils/pydantic.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/likeinterface/utils/response_validator.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/.gitignore
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/README.md
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/pyproject.toml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 likeinterface-1.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 likeinterface-1.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 likeinterface-1.0a0/Makefile
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 likeinterface-1.0a0/.github/dependabot.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 likeinterface-1.0a0/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 likeinterface-1.0a0/licenses/LICENSE.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/__meta__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/constants.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/exceptions.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/interface.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/network.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/session.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/__init__.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/base.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/auth/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/auth/get_authorization_information.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/auth/root_auth.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/auth/sign_in.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/like/__init__.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/like/evaluator.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/methods/like/root_like.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/base.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/auth/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/auth/authorization.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/auth/user.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/like/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/types/like/hand.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/utils/__init__.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/utils/pydantic.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 likeinterface-1.0a0/likeinterface/utils/response_validator.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 likeinterface-1.0a0/.gitignore
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 likeinterface-1.0a0/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 likeinterface-1.0a0/pyproject.toml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 likeinterface-1.0a0/PKG-INFO
```

### Comparing `likeinterface-1.0.1a0/Makefile` & `likeinterface-1.0a0/Makefile`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/.github/workflows/pre-commit-updater.yml` & `likeinterface-1.0a0/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/licenses/LICENSE.txt` & `likeinterface-1.0a0/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/interface.py` & `likeinterface-1.0a0/likeinterface/interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import Any, Dict, Optional
 
 import httpx
+from fastapi.requests import Request
 
 from likeinterface.methods import LikeType, Method
 from likeinterface.network import Network
 from likeinterface.session import Session
 
 
 class Interface:
@@ -17,9 +18,19 @@
         *,
         session: Optional[httpx.AsyncClient] = None,
         connect_kwargs: Dict[str, Any] = defaultdict(),  # noqa
     ) -> None:
         self.network = network
         self.session = Session(session=session, connect_kwargs=connect_kwargs)
 
-    async def request(self, method: Method[LikeType], timeout: Optional[int] = None) -> LikeType:
-        return await self.session.request(interface=self, method=method, timeout=timeout)
+    async def request(
+        self,
+        method: Method[LikeType],
+        timeout: Optional[int] = None,
+        fastapi_request: Optional[Request] = None,
+    ) -> LikeType:
+        return await self.session.request(
+            interface=self,
+            method=method,
+            timeout=timeout,
+            fastapi_request=fastapi_request,
+        )
```

### Comparing `likeinterface-1.0.1a0/likeinterface/session.py` & `likeinterface-1.0a0/likeinterface/session.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, Optional, cast
 
 import httpx
+from fastapi.requests import Request
 
 from likeinterface.constants import REQUEST_TIMEOUT
 from likeinterface.exceptions import LikeNetworkError
 from likeinterface.methods import LikeType, Method
 from likeinterface.utils.response_validator import response_validator
 
 if TYPE_CHECKING:
@@ -47,24 +48,37 @@
     ) -> None:
         super(Session, self).__init__(
             session=session,
             connect_kwargs=connect_kwargs,
         )
 
     async def request(
-        self, interface: Interface, method: Method[LikeType], timeout: Optional[int] = None
+        self,
+        interface: Interface,
+        method: Method[LikeType],
+        timeout: Optional[int] = None,
+        fastapi_request: Optional[Request] = None,
     ) -> LikeType:
         await self.create()
 
         request = method.request(interface=interface)
 
+        if fastapi_request:
+            json = await fastapi_request.json()
+
+            if isinstance(json, Dict):
+                request.data |= json
+
         try:
             response = await self.session.post(  # type: ignore[union-attr]
                 url=interface.network.url(method=method.__name__),
                 json=request.data,
+                params=fastapi_request.query_params if fastapi_request else None,
+                headers=fastapi_request.headers if fastapi_request else None,
+                cookies=fastapi_request.cookies if fastapi_request else None,
                 timeout=REQUEST_TIMEOUT if not timeout else timeout,
             )
         except asyncio.TimeoutError:
             raise LikeNetworkError("Exception %s: %s." % (method, "request timeout error"))
         except httpx.NetworkError as e:
             raise LikeNetworkError(
                 "Exception for method %s: %s." % (method.__name__, f"{type(e).__name__}: {e}")
```

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/base.py` & `likeinterface-1.0a0/likeinterface/methods/base.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/auth/get_authorization_information.py` & `likeinterface-1.0a0/likeinterface/methods/auth/get_authorization_information.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if TYPE_CHECKING:
     from likeinterface.interface import Interface
 
 
 class GetAuthorizationInformationMethod(Method[User]):
     """
-    Use this method to get information about current user.
+    Use this method to get information about user.
 
     Parameters
       Name            | Type   | Required | Description
 
       1. access_token | String | Yes      | Auth access token
 
     Result
```

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/auth/get_user_information.py` & `likeinterface-1.0a0/likeinterface/methods/like/evaluator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from likeinterface.methods.base import Method, Request
-from likeinterface.types import User
+from likeinterface.types import Hand
 
 if TYPE_CHECKING:
     from likeinterface.interface import Interface
 
 
-class GetUserInformationMethod(Method[User]):
+class EvaluatorMethod(Method[List[Hand]]):
     """
-    Use this method to get information about any user.
+    Use this method to evaluate hands.
 
     Parameters
-      Name       | Type    | Required | Description
+      Name     | Type            | Required | Description
 
-      1. user_id | Integer | Yes      | User ID in the system
+      1. board | Array of String | Yes      | Card table, for example, ["Ac", "As", "Ah", "Ad", "Td"]
+
+      2. hands | Array Of String | Yes      | Player hand, for example, ["2c2h", "2d2s"]
 
     Result
-      :class:`likeinterface.types.auth.user.User`
+      Array of :class:`likeinterface.types.like.hand.Hand`
     """
 
-    __name__ = "auth.getUserInformation"
-    __returning__ = User
+    __name__ = "like.evaluator"
+    __returning__ = List[Hand]
 
-    user_id: int
+    board: List[str]
+    hands: List[str]
 
     def request(self, interface: Interface) -> Request:
         return Request(method=self.__name__, data=self.model_dump())
```

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/auth/root_auth.py` & `likeinterface-1.0a0/likeinterface/methods/auth/root_auth.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/auth/sign_in.py` & `likeinterface-1.0a0/likeinterface/methods/auth/sign_in.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       6. auth_date   | Integer | Yes      | User authorization date
       7. hash        | String  | Yes      | Hash of all fields
 
     Result
       :class:`likeinterface.types.auth.authorization.Authorization`
     """
 
-    __name__ = "auth.signIn"
+    __name__ = "/auth.signIn"
     __returning__ = Authorization
 
     telegram_id: int
     first_name: str
     last_name: Optional[str] = None
     username: Optional[str] = None
     photo_url: Optional[str] = None
```

### Comparing `likeinterface-1.0.1a0/likeinterface/methods/like/root_like.py` & `likeinterface-1.0a0/likeinterface/methods/like/root_like.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/types/auth/user.py` & `likeinterface-1.0a0/likeinterface/types/auth/user.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/utils/pydantic.py` & `likeinterface-1.0a0/likeinterface/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/likeinterface/utils/response_validator.py` & `likeinterface-1.0a0/likeinterface/utils/response_validator.py`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/.gitignore` & `likeinterface-1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `likeinterface-1.0.1a0/pyproject.toml` & `likeinterface-1.0a0/pyproject.toml`

 * *Files identical despite different names*

