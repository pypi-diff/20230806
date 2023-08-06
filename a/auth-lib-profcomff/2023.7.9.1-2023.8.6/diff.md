# Comparing `tmp/auth_lib_profcomff-2023.7.9.1.tar.gz` & `tmp/auth_lib_profcomff-2023.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.7.9.1.tar", last modified: Sun Jul  9 06:03:52 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.8.6.tar", last modified: Sun Aug  6 04:25:14 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.7.9.1.tar` & `auth_lib_profcomff-2023.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 06:03:52.000000 auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 06:03:52.776368 auth_lib_profcomff-2023.7.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-09 06:03:41.000000 auth_lib_profcomff-2023.7.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/setup.py
```

### Comparing `auth_lib_profcomff-2023.7.9.1/LICENSE` & `auth_lib_profcomff-2023.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9.1/PKG-INFO` & `auth_lib_profcomff-2023.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth_lib_profcomff
-Version: 2023.7.9.1
+Version: 2023.8.6
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.7.9.1/README.md` & `auth_lib_profcomff-2023.8.6/README.md`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9.1/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.8.6/auth_lib/aiomethods.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from typing import Any
 from urllib.parse import urljoin
 
 import aiohttp
 
-from .exceptions import AuthFailed, SessionExpired
+from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AsyncAuthLib:
-    url: str
+    auth_url: str
+    userdata_url: str
 
-    def __init__(self, url: str):
-        self.url = url
+    def __init__(self, *, auth_url: str | None = None, userdata_url: str | None = None):
+        self.auth_url = auth_url
+        self.userdata_url = userdata_url
 
     async def email_login(self, email: str, password: str) -> dict[str, Any]:
         json = {"email": email, "password": password}
         async with aiohttp.ClientSession() as session:
-            response = await session.post(url=f"{self.url}/email/login", json=json)
+            response = await session.post(
+                url=urljoin(self.auth_url, "email/login"), json=json
+            )
         match response.status:
             case 200:
                 return await response.json()
             case 401:
                 raise AuthFailed(response=await response.json())
 
     async def check_token(self, token: str) -> dict[str, Any] | None:
         headers = {"Authorization": token}
         async with aiohttp.request(
             "GET",
-            urljoin(self.url, "me"),
+            urljoin(self.auth_url, "me"),
             headers={"Authorization": token},
             params={
                 "info": [
                     "indirect_groups",
                     "session_scopes",
                 ]
             },
@@ -41,16 +45,28 @@
         if r.ok:
             return user_session
         return None
 
     async def logout(self, token: str) -> bool:
         headers = {"Authorization": token}
         async with aiohttp.ClientSession() as session:
-            response = await session.post(url=f"{self.url}/logout", headers=headers)
+            response = await session.post(
+                url=urljoin(self.auth_url, "logout"), headers=headers
+            )
 
         match response.status:
             case 200:
                 return True
             case 401:
                 raise AuthFailed(response=await response.json())
             case 403:
                 raise SessionExpired(response=await response.json())
+
+    async def get_user_data(self, token: str, user_id: int) -> dict[str | Any] | None:
+        headers = {"Authorization": token}
+        async with aiohttp.ClientSession() as session:
+            response = await session.get(
+                url=urljoin(self.userdata_url, f"user/{user_id}"), headers=headers
+            )
+        if response.ok:
+            return await response.json()
+        return None
```

### Comparing `auth_lib_profcomff-2023.7.9.1/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.8.6/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.7.9.1/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.8.6/auth_lib/fastapi.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,46 +10,63 @@
 from starlette.status import HTTP_403_FORBIDDEN
 
 from auth_lib.aiomethods import AsyncAuthLib
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
+    USERDATA_URL: str = "https://api.test.profcomff.com/userdata/"
     AUTH_AUTO_ERROR: bool = True
     AUTH_ALLOW_NONE: bool = False
+    ENABLE_USERDATA: bool = False
     model_config = ConfigDict(case_sensitive=True, env_file=".env", extra="ignore")
 
 
 class UnionAuth(SecurityBase):
-    model = APIKey.construct(in_=APIKeyIn.header, name="Authorization")
+    model = APIKey.model_construct(in_=APIKeyIn.header, name="Authorization")
     scheme_name = "token"
     settings = UnionAuthSettings()
 
     def __init__(
         self,
         scopes: list[str] = [],
         auto_error: bool | None = None,
         allow_none: bool | None = None,
+        enable_userdata: bool | None = None,
         auth_url=None,  # Для обратной совместимости
+        userdata_url=None,
     ) -> None:
         if auth_url is not None:
             warn(
                 "auth_url in args deprecated, use AUTH_URL env instead",
                 DeprecationWarning,
             )
+        if userdata_url is not None:
+            warn(
+                "userdata_url in args deprecated, use USERDATA_URL env instead",
+                DeprecationWarning,
+            )
         super().__init__()
         self.auth_url = auth_url or self.settings.AUTH_URL
         if not self.auth_url.endswith("/"):
             self.auth_url = self.auth_url + "/"
+        self.userdata_url = userdata_url or self.settings.USERDATA_URL
+        if not self.userdata_url.endswith("/"):
+            self.userdata_url = self.userdata_url + "/"
         self.auto_error = (
             auto_error if auto_error is not None else self.settings.AUTH_AUTO_ERROR
         )
         self.allow_none = (
             allow_none if allow_none is not None else self.settings.AUTH_ALLOW_NONE
         )
+        self.enable_userdata = (
+            enable_userdata
+            if enable_userdata is not None
+            else self.settings.ENABLE_USERDATA
+        )
         self.scopes = scopes
 
     def _except(self):
         if self.auto_error:
             raise HTTPException(
                 status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
             )
@@ -57,24 +74,42 @@
             return None
 
     async def _get_session(self, token: str | None) -> dict[str, Any] | None:
         if not token and self.allow_none:
             return None
         if not token:
             return self._except()
-        return await AsyncAuthLib(url=self.auth_url).check_token(token)
+        return await AsyncAuthLib(auth_url=self.auth_url).check_token(token)
+
+    async def _get_userdata(
+        self, token: str | None, user_id: int
+    ) -> dict[str, Any] | None:
+        if not token and self.allow_none:
+            return None
+        if not token:
+            return self._except()
+        if self.enable_userdata:
+            return await AsyncAuthLib(userdata_url=self.userdata_url).get_user_data(
+                token, user_id
+            )
+        return None
 
     async def __call__(
         self,
         request: Request,
     ) -> dict[str, Any] | None:
         token = request.headers.get("Authorization")
-        user_session = await self._get_session(token)
-        if user_session is None:
+        result = await self._get_session(token)
+        if result is None:
             return self._except()
+        if self.enable_userdata:
+            user_data_info = await self._get_userdata(token, result["id"])
+            result["userdata"] = []
+            if user_data_info is not None:
+                result["userdata"] = user_data_info["items"]
         session_scopes = set(
-            [scope["name"].lower() for scope in user_session["session_scopes"]]
+            [scope["name"].lower() for scope in result["session_scopes"]]
         )
         required_scopes = set([scope.lower() for scope in self.scopes])
         if required_scopes - session_scopes:
             self._except()
-        return user_session
+        return result
```

### Comparing `auth_lib_profcomff-2023.7.9.1/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2023.8.6/auth_lib/testing/testutils.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     if not marker:
         return (yield)
     scopes: tuple[str] = marker.args
     session_scopes = []
     for cnt, scope in enumerate(scopes):
         session_scopes.append({"id": cnt, "name": scope, "comment": ""})
     _return_val: dict[str, int | list[dict[str, str | int]]] = {
-        "user_id": marker.kwargs.get("user_id", 0),
-        "id": 0,
+        "id": marker.kwargs.get("user_id", 0),
         "session_scopes": session_scopes,
         "user_scopes": session_scopes,
     }
     patcher = patch(
         "auth_lib.fastapi.UnionAuth._get_session",
         new=AsyncMock(return_value=_return_val),
     )
```

### Comparing `auth_lib_profcomff-2023.7.9.1/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.7.9.1
+Version: 2023.8.6
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `auth_lib_profcomff-2023.7.9.1/setup.py` & `auth_lib_profcomff-2023.8.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
-with open("README.md", "r") as readme_file:
+with open("README.md", "r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.07.09.1",
+    version="2023.08.06",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
```

