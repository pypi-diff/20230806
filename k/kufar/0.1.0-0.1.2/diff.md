# Comparing `tmp/kufar-0.1.0.tar.gz` & `tmp/kufar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kufar-0.1.0.tar", max compression
+gzip compressed data, was "kufar-0.1.2.tar", max compression
```

## Comparing `kufar-0.1.0.tar` & `kufar-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0     1092 2023-08-05 12:04:25.455957 kufar-0.1.0/README.md
--rw-r--r--   0        0        0       68 2023-08-05 11:35:45.019473 kufar-0.1.0/kufar/__init__.py
--rw-r--r--   0        0        0     2043 2023-07-29 20:00:58.266740 kufar-0.1.0/kufar/_instance.py
--rw-r--r--   0        0        0       33 2023-07-28 21:49:58.034019 kufar-0.1.0/kufar/base/__init__.py
--rw-r--r--   0        0        0      311 2023-07-29 16:13:26.223161 kufar-0.1.0/kufar/base/consts.py
--rw-r--r--   0        0        0     1085 2023-07-28 14:47:50.320124 kufar-0.1.0/kufar/base/service.py
--rw-r--r--   0        0        0      865 2023-08-05 11:58:20.878034 kufar-0.1.0/kufar/main.py
--rw-r--r--   0        0        0      228 2023-08-05 11:23:31.890773 kufar-0.1.0/kufar/packages/__init__.py
--rw-r--r--   0        0        0       59 2023-07-25 16:04:03.360800 kufar-0.1.0/kufar/packages/account/__init__.py
--rw-r--r--   0        0        0       49 2023-07-25 15:51:30.614338 kufar-0.1.0/kufar/packages/account/consts.py
--rw-r--r--   0        0        0      342 2023-07-29 20:03:15.926993 kufar-0.1.0/kufar/packages/account/instance.py
--rw-r--r--   0        0        0     1065 2023-07-25 16:02:37.233087 kufar-0.1.0/kufar/packages/account/schemas.py
--rw-r--r--   0        0        0       56 2023-07-23 15:34:32.222711 kufar-0.1.0/kufar/packages/ads/__init__.py
--rw-r--r--   0        0        0      481 2023-07-23 13:42:00.380534 kufar-0.1.0/kufar/packages/ads/consts.py
--rw-r--r--   0        0        0     1349 2023-08-03 19:00:57.514794 kufar-0.1.0/kufar/packages/ads/instance.py
--rw-r--r--   0        0        0     1766 2023-07-23 18:28:34.875680 kufar-0.1.0/kufar/packages/ads/schemas.py
--rw-r--r--   0        0        0       57 2023-08-05 11:27:21.432470 kufar-0.1.0/kufar/packages/auth/__init__.py
--rw-r--r--   0        0        0      626 2023-07-22 22:32:30.637123 kufar-0.1.0/kufar/packages/auth/consts.py
--rw-r--r--   0        0        0     3095 2023-08-05 11:27:40.199275 kufar-0.1.0/kufar/packages/auth/instance.py
--rw-r--r--   0        0        0     1522 2023-07-24 22:45:05.670279 kufar-0.1.0/kufar/packages/auth/schemas.py
--rw-r--r--   0        0        0       61 2023-07-23 15:36:00.162686 kufar-0.1.0/kufar/packages/categories/__init__.py
--rw-r--r--   0        0        0       51 2023-07-23 11:08:06.422709 kufar-0.1.0/kufar/packages/categories/consts.py
--rw-r--r--   0        0        0      261 2023-07-23 18:49:44.404106 kufar-0.1.0/kufar/packages/categories/instance.py
--rw-r--r--   0        0        0      450 2023-07-23 15:35:48.536466 kufar-0.1.0/kufar/packages/categories/schemas.py
--rw-r--r--   0        0        0       38 2023-07-17 12:52:41.600378 kufar-0.1.0/kufar/packages/cities/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-23 18:28:34.885680 kufar-0.1.0/kufar/packages/cities/schemas.py
--rw-r--r--   0        0        0        0 2023-07-17 14:45:07.248718 kufar-0.1.0/kufar/packages/favorites/__init__.py
--rw-r--r--   0        0        0      454 2023-07-23 14:22:42.043337 kufar-0.1.0/kufar/packages/favorites/consts.py
--rw-r--r--   0        0        0        0 2023-07-17 15:03:09.351459 kufar-0.1.0/kufar/packages/filters/__init__.py
--rw-r--r--   0        0        0      355 2023-07-17 15:05:01.389073 kufar-0.1.0/kufar/packages/filters/consts.py
--rw-r--r--   0        0        0       61 2023-07-29 19:59:29.946584 kufar-0.1.0/kufar/packages/messaging/__init__.py
--rw-r--r--   0        0        0       46 2023-07-29 19:58:00.789767 kufar-0.1.0/kufar/packages/messaging/consts.py
--rw-r--r--   0        0        0      329 2023-07-29 20:01:30.646799 kufar-0.1.0/kufar/packages/messaging/instance.py
--rw-r--r--   0        0        0      136 2023-07-29 19:59:09.043215 kufar-0.1.0/kufar/packages/messaging/schemas.py
--rw-r--r--   0        0        0       58 2023-07-23 15:36:32.596276 kufar-0.1.0/kufar/packages/saved/__init__.py
--rw-r--r--   0        0        0      303 2023-07-23 13:31:33.266733 kufar-0.1.0/kufar/packages/saved/consts.py
--rw-r--r--   0        0        0     1088 2023-07-23 18:50:16.193853 kufar-0.1.0/kufar/packages/saved/instance.py
--rw-r--r--   0        0        0      522 2023-07-23 18:28:34.882347 kufar-0.1.0/kufar/packages/saved/schemas.py
--rw-r--r--   0        0        0       60 2023-07-28 21:47:24.009387 kufar-0.1.0/kufar/packages/user_ads/__init__.py
--rw-r--r--   0        0        0      269 2023-07-29 15:55:53.257477 kufar-0.1.0/kufar/packages/user_ads/consts.py
--rw-r--r--   0        0        0     1361 2023-07-29 19:38:21.469427 kufar-0.1.0/kufar/packages/user_ads/instance.py
--rw-r--r--   0        0        0     2429 2023-07-23 18:28:34.869013 kufar-0.1.0/kufar/packages/user_ads/schemas.py
--rw-r--r--   0        0        0      316 2023-08-05 11:34:56.949125 kufar-0.1.0/kufar/schemas.py
--rw-r--r--   0        0        0       58 2023-08-05 11:33:01.798289 kufar-0.1.0/kufar/utils/__init__.py
--rw-r--r--   0        0        0      652 2023-07-28 14:50:46.635125 kufar-0.1.0/kufar/utils/auth.py
--rw-r--r--   0        0        0     4523 2023-08-05 11:30:07.097017 kufar-0.1.0/kufar/utils/requester.py
--rw-r--r--   0        0        0      327 2023-07-29 19:50:11.049129 kufar-0.1.0/kufar/utils/signature_decoder.py
--rw-r--r--   0        0        0      954 2023-07-28 21:40:23.089150 kufar-0.1.0/kufar/utils/state.py
--rw-r--r--   0        0        0      968 2023-08-05 12:05:30.309173 kufar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 kufar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-08-06 19:07:08.660012 kufar-0.1.2/README.md
+-rw-r--r--   0        0        0       68 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/__init__.py
+-rw-r--r--   0        0        0     2250 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/_instance.py
+-rw-r--r--   0        0        0       33 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/__init__.py
+-rw-r--r--   0        0        0      311 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/consts.py
+-rw-r--r--   0        0        0     1167 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/base/service.py
+-rw-r--r--   0        0        0      206 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/__init__.py
+-rw-r--r--   0        0        0       59 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/__init__.py
+-rw-r--r--   0        0        0       49 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/consts.py
+-rw-r--r--   0        0        0      347 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/instance.py
+-rw-r--r--   0        0        0     1065 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/account/schemas.py
+-rw-r--r--   0        0        0       56 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/__init__.py
+-rw-r--r--   0        0        0      911 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/consts.py
+-rw-r--r--   0        0        0     1680 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/instance.py
+-rw-r--r--   0        0        0     1766 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/ads/schemas.py
+-rw-r--r--   0        0        0       57 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/__init__.py
+-rw-r--r--   0        0        0      626 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/consts.py
+-rw-r--r--   0        0        0     3017 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/instance.py
+-rw-r--r--   0        0        0     1522 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/auth/schemas.py
+-rw-r--r--   0        0        0       61 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/__init__.py
+-rw-r--r--   0        0        0       51 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/consts.py
+-rw-r--r--   0        0        0      259 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/instance.py
+-rw-r--r--   0        0        0      450 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/categories/schemas.py
+-rw-r--r--   0        0        0        0 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/favorites/__init__.py
+-rw-r--r--   0        0        0      454 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/favorites/consts.py
+-rw-r--r--   0        0        0       36 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/__init__.py
+-rw-r--r--   0        0        0      315 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/consts.py
+-rw-r--r--   0        0        0      783 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/instance.py
+-rw-r--r--   0        0        0     1407 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/filters/schemas.py
+-rw-r--r--   0        0        0       61 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/__init__.py
+-rw-r--r--   0        0        0       46 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/consts.py
+-rw-r--r--   0        0        0      342 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/instance.py
+-rw-r--r--   0        0        0      136 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/messaging/schemas.py
+-rw-r--r--   0        0        0       58 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/__init__.py
+-rw-r--r--   0        0        0      303 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/consts.py
+-rw-r--r--   0        0        0     1041 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/instance.py
+-rw-r--r--   0        0        0      522 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/saved/schemas.py
+-rw-r--r--   0        0        0       60 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/consts.py
+-rw-r--r--   0        0        0     1301 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/instance.py
+-rw-r--r--   0        0        0     2429 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/packages/user_ads/schemas.py
+-rw-r--r--   0        0        0      317 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/schemas.py
+-rw-r--r--   0        0        0       58 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/__init__.py
+-rw-r--r--   0        0        0      652 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/auth.py
+-rw-r--r--   0        0        0     4665 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/requester.py
+-rw-r--r--   0        0        0      327 2023-08-06 19:07:08.660012 kufar-0.1.2/kufar/utils/signature_decoder.py
+-rw-r--r--   0        0        0      942 2023-08-06 19:07:08.664013 kufar-0.1.2/kufar/utils/state.py
+-rw-r--r--   0        0        0     1123 2023-08-06 19:07:08.664013 kufar-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 kufar-0.1.2/PKG-INFO
```

### Comparing `kufar-0.1.0/kufar/_instance.py` & `kufar-0.1.2/kufar/_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from base import consts
-from packages import (
+from .base import consts
+from .packages import (
     AccountService,
     AdsService,
     AuthService,
     CategoryService,
     LogInPayload,
     MessagingService,
     SavedService,
     UserAdsService,
+    FilterService,
 )
-from utils.requester import Requester
-from utils.state import State
+from .utils.requester import Requester
+from .utils.state import State
 
 
 class KufarApi:
     __inited: bool = False
 
     _client: Requester
 
     account: AccountService
     ads: AdsService
     auth: AuthService
     categories: CategoryService
     saved: SavedService
     user_ads: UserAdsService
     messaging: MessagingService
+    filters: FilterService
 
     state: State
 
     def __init__(self, client: Requester, state: State):
         self._client = client
 
         self.state = state
@@ -36,27 +38,33 @@
         self.ads = AdsService(self._client, consts.API_URL)
         self.auth = AuthService(self._client, consts.CRE_API_URL)
         self.categories = CategoryService(self._client, consts.API_URL)
         self.saved = SavedService(self._client, consts.API_URL)
         self.user_ads = UserAdsService(self._client, consts.BAPI_URL)
         self.account = AccountService(self._client, consts.API_URL)
         self.messaging = MessagingService(self._client, consts.API_URL)
+        self.filters = FilterService(self._client, consts.API_URL)
 
     def _load_tokens_from_state(self):
         if self.state.access_token is not None:
-            self._client.patch_headers({
-                "authorization": f"Bearer {self.state.access_token}",
-                "session-id": str(self.state.session_id),
-            })
+            self._client.patch_headers(
+                {
+                    "authorization": f"Bearer {self.state.access_token}",
+                    "session-id": str(self.state.session_id),
+                }
+            )
 
     async def init(self):
         if self.__inited:
             return
         await self.state.load()
         self._load_tokens_from_state()
+
+        await self.filters.get_base_filters()
+
         self.__inited = True
 
     async def authenticate(self, email: str, password: str):
         if (await self.auth.is_login_captcha_required()).is_required:
             raise Exception("Captcha required")
         tokens = await self.auth.login(LogInPayload(login=email, password=password))
         if tokens:
```

### Comparing `kufar-0.1.0/kufar/base/service.py` & `kufar-0.1.2/kufar/base/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from dataclasses import dataclass
 from functools import wraps
 
 from pydantic import BaseModel, ValidationError
-from utils.requester import Requester
+from kufar.utils.requester import Requester
 
 
 @dataclass
 class BaseService:
     client: Requester
     base_url: str
 
@@ -15,21 +15,24 @@
         attr = super().__getattribute__(item)
 
         if callable(attr):
             return_type = inspect.signature(attr).return_annotation
 
             if not return_type:
                 return attr
-            
-            if issubclass(return_type, BaseModel):
+
+            if inspect.isclass(return_type) and issubclass(return_type, BaseModel):
+
                 @wraps(attr)
                 async def wrapper_func(*args, **kwargs):
                     self.client.url = self.base_url
                     response = await attr(*args, **kwargs)
                     try:
                         return return_type.model_validate(response)
                     except ValidationError as e:
-                        print(f'Error while validating response. Response is: {response}\nError is: {e}')
+                        print(
+                            f"Error while validating response. Response is: {response}\nError is: {e}"
+                        )
                         return None
 
                 return wrapper_func
         return attr
```

### Comparing `kufar-0.1.0/kufar/packages/account/schemas.py` & `kufar-0.1.2/kufar/packages/account/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/packages/ads/instance.py` & `kufar-0.1.2/kufar/packages/ads/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-from base import BaseService
+from kufar.base import BaseService
+from kufar.utils.auth import auth_required
 
 from . import consts
 from .schemas import (
     GetAdvertByListIdResponse,
     GetAdvertResponse,
     GetPhoneResponse,
     GetUserSearchAdvertsResponse,
 )
 
 
 class AdsService(BaseService):
-    async def get_advert(self, ad_id: int, lang: str = 'ru') -> GetAdvertResponse:
+    async def get_advert(self, ad_id: int, lang: str = "ru") -> GetAdvertResponse:
         return await self.client.get(
             consts.GET_ADVERT.format(ad_id=ad_id),
             headers=consts.SEGMENTATION_HEADER,
-            params={'lang': lang}
+            params={"lang": lang},
         )
 
-    async def get_advert_by_list_id(self, msgi: str, size: str, lang: str = 'ru') -> GetAdvertByListIdResponse:
+    async def get_advert_by_list_id(
+        self, msgi: str, size: str, lang: str = "ru"
+    ) -> GetAdvertByListIdResponse:
         return await self.client.get(
             consts.SEARCH_ADVERTS,
             headers=consts.SEGMENTATION_HEADER_WITH_HACK,
-            params={
-                'msgi': msgi,
-                'size': size,
-                'lang': lang
-            }
+            params={"msgi": msgi, "size": size, "lang": lang},
         )
 
     async def get_ad_phone(self, ad_id: int) -> GetPhoneResponse:
         return await self.client.get(consts.GET_PHONE.format(ad_id=ad_id))
 
-    async def user_search_adverts(self, size: int, cursor: str | None = None) -> GetUserSearchAdvertsResponse:
+    @auth_required
+    async def user_search_adverts(
+        self, size: int, cursor: str | None = None
+    ) -> GetUserSearchAdvertsResponse:
         return await self.client.get(
             consts.SEARCH_ADVERTS,
             headers=consts.USER_SEGMENTATION_HEADER,
-            params={
-                'size': size,
-                'cursor': cursor
-            }
+            params={"size": size, "cursor": cursor},
+        )
+
+    async def search_adverts(
+        self, size: int, query: str, cursor: str | None = None
+    ) -> GetAdvertByListIdResponse:
+        return await self.client.get(
+            consts.SEARCH_ADVERTS,
+            headers=consts.SEGMENTATION_HEADER_WITH_HACK,
+            params={"query": query, "size": size, "cursor": cursor},
         )
```

### Comparing `kufar-0.1.0/kufar/packages/ads/schemas.py` & `kufar-0.1.2/kufar/packages/ads/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/packages/auth/consts.py` & `kufar-0.1.2/kufar/packages/auth/consts.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/packages/auth/instance.py` & `kufar-0.1.2/kufar/packages/auth/instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from base import BaseService
-from utils.auth import auth_required
+from kufar.base import BaseService
+from kufar.utils.auth import auth_required
 
 from . import consts
 from .schemas import (
     ChangePasswordPayload,
     HistoryResponse,
     IsCaptchaRequiredResponse,
     LogInPayload,
@@ -20,42 +20,32 @@
     async def login(self, payload: LogInPayload) -> LogInResponse:
         return await self.client.post(
             consts.LOG_IN,
             {
                 **payload.model_dump(exclude_none=True),
                 "captcha_platform": "android",
                 "captcha_type": "recaptcha",
-                "captcha_secret_version": "v1"
+                "captcha_secret_version": "v1",
             },
-            params={'token_type': 'user'}
+            params={"token_type": "user"},
         )
 
     async def login_apple(self, token: str, full_name: str) -> LogInResponse:
         return await self.client.post(
-            consts.LOG_IN_APPLE,
-            {'token': token, 'full_name': full_name}
+            consts.LOG_IN_APPLE, {"token": token, "full_name": full_name}
         )
 
     async def login_google(self, token: str) -> LogInResponse:
-        return await self.client.post(
-            consts.LOG_IN_GOOGLE,
-            {'token': token}
-        )
+        return await self.client.post(consts.LOG_IN_GOOGLE, {"token": token})
 
     async def login_mail_ru(self, token: str) -> LogInResponse:
-        return await self.client.post(
-            consts.LOG_IN_MAIL_RU,
-            {'token': token}
-        )
+        return await self.client.post(consts.LOG_IN_MAIL_RU, {"token": token})
 
     async def login_yandex(self, token: str) -> LogInResponse:
-        return await self.client.post(
-            consts.LOG_IN_YANDEX,
-            {'token': token}
-        )
+        return await self.client.post(consts.LOG_IN_YANDEX, {"token": token})
 
     @auth_required
     async def logout(self) -> None:
         return await self.client.get(consts.LOG_OUT)
 
     @auth_required
     async def logout_all(self) -> None:
@@ -68,20 +58,22 @@
         return await self.client.post(consts.CREATE_ACCOUNT, payload.model_dump())
 
     async def is_login_captcha_required(self) -> IsCaptchaRequiredResponse:
         return await self.client.get(consts.IS_LOGIN_CAPTCHA_REQUIRED)
 
     @auth_required
     async def login_history(self, cursor: str | None = None) -> HistoryResponse:
-        return await self.client.get(consts.LOGIN_HISTORY, params={'cursor': cursor})
+        return await self.client.get(consts.LOGIN_HISTORY, params={"cursor": cursor})
 
     async def reset_password(self, payload: ResetPasswordPayload) -> any:
         return await self.client.post(consts.RESET_PASSWORD, payload.model_dump())
 
     async def reset_password_request(self, payload: ResetPasswordRequestPayload) -> any:
-        return await self.client.post(consts.RESET_PASSWORD_REQUEST, payload.model_dump())
+        return await self.client.post(
+            consts.RESET_PASSWORD_REQUEST, payload.model_dump()
+        )
 
     async def request_sms_code(self, phone: str) -> RequestSmsCodeResponse:
-        return await self.client.get(consts.REQUEST_SMS_CODE, params={'phone': phone})
+        return await self.client.get(consts.REQUEST_SMS_CODE, params={"phone": phone})
 
     async def verify_sms_code(self, payload: VerifySmsCodePayload) -> LogInResponse:
         return await self.client.post(consts.VERIFY_SMS_CODE, payload.model_dump())
```

### Comparing `kufar-0.1.0/kufar/packages/auth/schemas.py` & `kufar-0.1.2/kufar/packages/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/packages/saved/instance.py` & `kufar-0.1.2/kufar/packages/saved/instance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-from base import BaseService
+from kufar.base import BaseService
 from . import consts
-from .schemas import (
-    SavedSearch,
-    SavedSearches
-)
+from .schemas import SavedSearch, SavedSearches
 
 
 class SavedService(BaseService):
     async def mark_search_seen(self, account_id: int, search_id: int) -> None:
-        return await self.client.post(consts.MARK_SEARCH_SEEN.format(
-            account_id=account_id,
-            search_id=search_id
-        ))
+        return await self.client.post(
+            consts.MARK_SEARCH_SEEN.format(account_id=account_id, search_id=search_id)
+        )
 
     async def delete_search(self, account_id: int, search_id: int) -> None:
-        return await self.client.delete(consts.DELETE_SEARCH.format(
-            account_id=account_id,
-            search_id=search_id
-        ))
+        return await self.client.delete(
+            consts.DELETE_SEARCH.format(account_id=account_id, search_id=search_id)
+        )
 
-    async def get_searches(self, account_id: int, cursor: str | None = None) -> SavedSearches:
-        return await self.client.get(consts.GET_FAVORITE_SEARCHES.format(
-            account_id=account_id
-        ), params={
-            'cursor': cursor
-        })
+    async def get_searches(
+        self, account_id: int, cursor: str | None = None
+    ) -> SavedSearches:
+        return await self.client.get(
+            consts.GET_FAVORITE_SEARCHES.format(account_id=account_id),
+            params={"cursor": cursor},
+        )
 
     async def save_search(self, account_id: int, query: str) -> SavedSearch:
-        return await self.client.post(consts.SAVE_SEARCH.format(
-            account_id=account_id
-        ), {
-            'query': query
-        })
+        return await self.client.post(
+            consts.SAVE_SEARCH.format(account_id=account_id), {"query": query}
+        )
```

### Comparing `kufar-0.1.0/kufar/packages/saved/schemas.py` & `kufar-0.1.2/kufar/packages/saved/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/packages/user_ads/schemas.py` & `kufar-0.1.2/kufar/packages/user_ads/schemas.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/utils/auth.py` & `kufar-0.1.2/kufar/utils/auth.py`

 * *Files identical despite different names*

### Comparing `kufar-0.1.0/kufar/utils/requester.py` & `kufar-0.1.2/kufar/utils/requester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,137 +1,139 @@
 from json import JSONDecodeError
 from typing import Literal, Self
 
 from aiohttp import ClientSession, ContentTypeError
 
 from .signature_decoder import decode_signature
-from base import consts
+from ..base import consts
 
 
 class Requester:
     __base_url: str
     __client: ClientSession | None = None
     __headers: dict[str, str]
-    __hash: str = ''
+    __hash: str = ""
 
     def __init__(self):
-        self.__base_url = ''
+        self.__base_url = ""
         self.__headers = consts.BASE_HEADERS
 
     async def __aenter__(self) -> Self:
-            self.__client = ClientSession(
-                base_url=self.__base_url if len(self.__base_url) else None,
-                headers=self.__headers
-            )
-            return self
+        self.__client = ClientSession(
+            base_url=self.__base_url if len(self.__base_url) else None,
+            headers=self.__headers,
+        )
+        return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if self.__client:
             await self.__client.close()
         self.__client = None
 
     @property
     def url(self):
         return self.__base_url
 
     @url.setter
     def url(self, value: str):
         self.__base_url = value
-    
+
     async def post(self, path: str, payload: dict | None = None, **kwargs):
-        prev_headers = kwargs.get('headers') or {}
-        kwargs.update({
-            'headers': {
-                **prev_headers,
-                'content-type': 'application/json; charset=UTF-8'
+        prev_headers = kwargs.get("headers") or {}
+        kwargs.update(
+            {
+                "headers": {
+                    **prev_headers,
+                    "content-type": "application/json; charset=UTF-8",
+                }
             }
-        })
-        return await self._request('POST', path, json=payload, **kwargs)
+        )
+        return await self._request("POST", path, json=payload, **kwargs)
 
     async def get(self, path: str, **kwargs):
-        return await self._request('GET', path, **kwargs)
+        return await self._request("GET", path, **kwargs)
 
     async def delete(self, path: str, **kwargs):
-        return await self._request('DELETE', path, **kwargs)
-    
+        return await self._request("DELETE", path, **kwargs)
+
     async def post_legacy(self, path: str, **kwargs):
-        return await self._legacy_request('POST', path, **kwargs)
-    
+        return await self._legacy_request("POST", path, **kwargs)
+
     async def get_legacy(self, path: str, **kwargs):
-        return await self._legacy_request('GET', path, **kwargs)
-    
+        return await self._legacy_request("GET", path, **kwargs)
+
     @property
     def headers(self):
         return self.__headers
 
     def patch_headers(self, new_headers: dict[str, str]):
-        self.__headers = {
-            **self.__headers,
-            **new_headers
-        }
+        self.__headers = {**self.__headers, **new_headers}
         if self.__client:
             self.__client.headers.update(self.__headers)
 
     def select_headers(self, *args: str):
         if len(args) == 1:
             return self.__headers.get(args[0])
         return {k: v for k, v in self.__headers.items() if k in args}
 
     async def _request(
-            self, 
-            method: Literal['GET', 'POST', 'PUT', 'DELETE'], 
-            path: str, 
-            **kwargs
+        self, method: Literal["GET", "POST", "PUT", "DELETE"], path: str, **kwargs
     ):
         if not self.__client:
-            raise Exception('Not initialized client. You should use async context manager')
+            raise Exception(
+                "Not initialized client. You should use async context manager"
+            )
         if not self.__base_url:
-            raise Exception('base_url not specified')
-        if kwargs.get('headers'):
-            kwargs['headers'] = {
+            raise Exception("base_url not specified")
+        if kwargs.get("headers"):
+            kwargs["headers"] = {
                 **self.__headers,
-                **kwargs.get('headers') # type: ignore
+                **kwargs.get("headers"),  # type: ignore
             }
         else:
-            kwargs['headers'] = self.__headers
-        url = f'{self.__base_url}{path}'
-        async with self.__client.request(method, url, **kwargs) as res:
+            kwargs["headers"] = self.__headers
+        url = f"{self.__base_url}{path}"
+        params = exclude_none(kwargs.get("params") or {})
+        kwargs.pop("params")
+        async with self.__client.request(method, url, **kwargs, params=params) as res:
             try:
                 return await res.json()
             except (ContentTypeError, JSONDecodeError) as e:
-                print(f'Error while decoding. Content: {await res.text()}')
+                print(f"Error while decoding. Content: {await res.text()}")
                 raise e
-    
-    async def _legacy_request(self, method: str, path: str, **kwargs) -> any: # type: ignore
-        url = f'{self.__base_url}{path}'
+
+    async def _legacy_request(self, method: str, path: str, **kwargs) -> any:  # type: ignore
+        url = f"{self.__base_url}{path}"
         if not self.__client:
             return None
-        headers: dict = self.select_headers(
-            'user-agent', 'x-app-name', 'x-app-version', 'x-device-id') or {} # type: ignore
+        headers: dict = (
+            self.select_headers(
+                "user-agent", "x-app-name", "x-app-version", "x-device-id"
+            )
+            or {}
+        )  # type: ignore
         async with self.__client.request(
-            method, 
+            method,
             url,
             **kwargs,
             allow_redirects=False,
             params={
-                'app_id': 'android',
-                'account_token': self.select_headers('session-id'),
-                'hash': decode_signature(self.__hash),
-                **(kwargs.get('params') or {})
-            },
-            headers={
-                **headers,
-                **(kwargs.get('headers') or {})
+                "app_id": "android",
+                "account_token": self.select_headers("session-id"),
+                "hash": decode_signature(self.__hash),
+                **(exclude_none(kwargs.get("params") or {})),
             },
+            headers={**headers, **(kwargs.get("headers") or {})},
         ) as res:
             try:
                 data = await res.json()
             except (ContentTypeError, JSONDecodeError) as e:
-                print(f'Error while decoding. Content: {(await res.text())[:1000]}')
+                print(f"Error while decoding. Content: {(await res.text())[:1000]}")
                 raise e
-        if 'authorize' in data:
-            self.__hash = str(data.get('authorize').get('challenge', ''))
-            return await self._legacy_request(
-                method,
-                path
-            )
+        if "authorize" in data:
+            self.__hash = str(data.get("authorize").get("challenge", ""))
+            return await self._legacy_request(method, path)
         return data
+
+
+def exclude_none(input: dict) -> dict:
+    return {k: v for k, v in input.items() if v is not None}
```

### Comparing `kufar-0.1.0/kufar/utils/state.py` & `kufar-0.1.2/kufar/utils/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
     def __init__(self, file_path: str):
         self.__file_path = file_path
         self.__state = {}
 
     async def load(self) -> None:
         if os.path.isfile(self.__file_path):
-            async with aiofiles.open(self.__file_path, 'r') as f:
+            async with aiofiles.open(self.__file_path, "r") as f:
                 self.__state = json.loads(await f.read())
-        
+
     async def save(self) -> None:
-        async with aiofiles.open(self.__file_path, 'w') as f:
+        async with aiofiles.open(self.__file_path, "w") as f:
             await f.write(json.dumps(self.__state))
 
     def __getattr__(self, name: str) -> str | int | None:
-        return object.__getattribute__(self, '_State__state').get(name, None)
-    
+        return object.__getattribute__(self, "_State__state").get(name, None)
+
     def __setattr__(self, name: str, value: str | int) -> None:
         if name in self.__annotations__.keys():
             return object.__setattr__(self, name, value)
-        object.__getattribute__(self, '_State__state')[name] = value
+        object.__getattribute__(self, "_State__state")[name] = value
```

