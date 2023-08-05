# Comparing `tmp/instagrapi-1.9.8.tar.gz` & `tmp/instagrapi-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/instagrapi-1.9.8.tar", last modified: Fri Aug  6 09:06:39 2021, max compression
+gzip compressed data, was "dist/instagrapi-1.9.9.tar", last modified: Fri Aug  6 11:53:08 2021, max compression
```

## Comparing `instagrapi-1.9.8.tar` & `instagrapi-1.9.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 09:06:39.000000 instagrapi-1.9.8/
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi/
--rw-r--r--   0 adw0rd     (501) staff       (20)     6065 2021-07-20 09:25:31.000000 instagrapi-1.9.8/instagrapi/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2140 2021-07-28 13:02:21.000000 instagrapi-1.9.8/instagrapi/config.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    11464 2021-08-02 21:24:52.000000 instagrapi-1.9.8/instagrapi/extractors.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi/mixins/
--rw-r--r--   0 adw0rd     (501) staff       (20)    22515 2021-08-06 09:06:38.000000 instagrapi-1.9.8/instagrapi/mixins/auth.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8289 2021-07-26 06:47:00.000000 instagrapi-1.9.8/instagrapi/mixins/story.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    22653 2021-07-28 14:36:04.000000 instagrapi-1.9.8/instagrapi/mixins/user.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     9211 2021-07-11 16:48:44.000000 instagrapi-1.9.8/instagrapi/mixins/public.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    18539 2021-06-24 08:52:25.000000 instagrapi-1.9.8/instagrapi/mixins/media.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     3086 2021-07-27 07:46:15.000000 instagrapi-1.9.8/instagrapi/mixins/timeline.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     5206 2021-05-15 21:43:44.000000 instagrapi-1.9.8/instagrapi/mixins/comment.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10240 2021-07-31 08:29:50.000000 instagrapi-1.9.8/instagrapi/mixins/igtv.py
--rw-rw-r--   0 adw0rd     (501) staff       (20)        0 2021-02-27 05:34:00.000000 instagrapi-1.9.8/instagrapi/mixins/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     8777 2021-07-31 08:29:50.000000 instagrapi-1.9.8/instagrapi/mixins/album.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    13237 2021-05-16 19:57:21.000000 instagrapi-1.9.8/instagrapi/mixins/hashtag.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     9319 2021-05-14 09:51:38.000000 instagrapi-1.9.8/instagrapi/mixins/location.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     5955 2021-06-13 19:27:20.000000 instagrapi-1.9.8/instagrapi/mixins/collection.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    17150 2021-07-31 08:29:50.000000 instagrapi-1.9.8/instagrapi/mixins/photo.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    17837 2021-07-28 13:02:21.000000 instagrapi-1.9.8/instagrapi/mixins/direct.py
--rw-rw-r--   0 adw0rd     (501) staff       (20)     1509 2021-03-06 15:40:00.000000 instagrapi-1.9.8/instagrapi/mixins/password.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    10191 2021-07-31 08:29:50.000000 instagrapi-1.9.8/instagrapi/mixins/clip.py
--rw-rw-r--   0 adw0rd     (501) staff       (20)     5987 2021-02-27 05:34:00.000000 instagrapi-1.9.8/instagrapi/mixins/insights.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    16412 2021-07-28 13:02:38.000000 instagrapi-1.9.8/instagrapi/mixins/challenge.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    28689 2021-07-31 08:29:50.000000 instagrapi-1.9.8/instagrapi/mixins/video.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    15152 2021-07-29 16:44:34.000000 instagrapi-1.9.8/instagrapi/mixins/private.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4829 2021-08-05 14:13:36.000000 instagrapi-1.9.8/instagrapi/mixins/account.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2790 2021-07-27 07:46:15.000000 instagrapi-1.9.8/instagrapi/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     7137 2021-08-03 09:21:53.000000 instagrapi-1.9.8/instagrapi/types.py
--rw-rw-r--   0 adw0rd     (501) staff       (20)      311 2021-02-27 05:34:00.000000 instagrapi-1.9.8/instagrapi/zones.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2709 2021-07-28 13:02:21.000000 instagrapi-1.9.8/instagrapi/utils.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     4748 2021-06-18 12:42:06.000000 instagrapi-1.9.8/instagrapi/exceptions.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     2079 2021-08-06 09:06:39.000000 instagrapi-1.9.8/PKG-INFO
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     2079 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      985 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       74 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       11 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2021-08-06 09:06:39.000000 instagrapi-1.9.8/instagrapi.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)     8335 2021-08-02 21:24:52.000000 instagrapi-1.9.8/README.md
--rw-r--r--   0 adw0rd     (501) staff       (20)     2530 2021-08-06 09:06:38.000000 instagrapi-1.9.8/setup.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2021-08-06 09:06:39.000000 instagrapi-1.9.8/setup.cfg
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 11:53:08.000000 instagrapi-1.9.9/
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     6065 2021-07-20 09:25:31.000000 instagrapi-1.9.9/instagrapi/story.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2140 2021-07-28 13:02:21.000000 instagrapi-1.9.9/instagrapi/config.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    11464 2021-08-02 21:24:52.000000 instagrapi-1.9.9/instagrapi/extractors.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi/mixins/
+-rw-r--r--   0 adw0rd     (501) staff       (20)    22515 2021-08-06 09:06:38.000000 instagrapi-1.9.9/instagrapi/mixins/auth.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8289 2021-07-26 06:47:00.000000 instagrapi-1.9.9/instagrapi/mixins/story.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    22653 2021-07-28 14:36:04.000000 instagrapi-1.9.9/instagrapi/mixins/user.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     9540 2021-08-06 11:51:06.000000 instagrapi-1.9.9/instagrapi/mixins/public.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    18539 2021-06-24 08:52:25.000000 instagrapi-1.9.9/instagrapi/mixins/media.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     3086 2021-07-27 07:46:15.000000 instagrapi-1.9.9/instagrapi/mixins/timeline.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     5206 2021-05-15 21:43:44.000000 instagrapi-1.9.9/instagrapi/mixins/comment.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10240 2021-07-31 08:29:50.000000 instagrapi-1.9.9/instagrapi/mixins/igtv.py
+-rw-rw-r--   0 adw0rd     (501) staff       (20)        0 2021-02-27 05:34:00.000000 instagrapi-1.9.9/instagrapi/mixins/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8777 2021-07-31 08:29:50.000000 instagrapi-1.9.9/instagrapi/mixins/album.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    13237 2021-05-16 19:57:21.000000 instagrapi-1.9.9/instagrapi/mixins/hashtag.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     9319 2021-05-14 09:51:38.000000 instagrapi-1.9.9/instagrapi/mixins/location.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     5955 2021-06-13 19:27:20.000000 instagrapi-1.9.9/instagrapi/mixins/collection.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    17150 2021-07-31 08:29:50.000000 instagrapi-1.9.9/instagrapi/mixins/photo.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    17837 2021-07-28 13:02:21.000000 instagrapi-1.9.9/instagrapi/mixins/direct.py
+-rw-rw-r--   0 adw0rd     (501) staff       (20)     1509 2021-03-06 15:40:00.000000 instagrapi-1.9.9/instagrapi/mixins/password.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    10191 2021-07-31 08:29:50.000000 instagrapi-1.9.9/instagrapi/mixins/clip.py
+-rw-rw-r--   0 adw0rd     (501) staff       (20)     5987 2021-02-27 05:34:00.000000 instagrapi-1.9.9/instagrapi/mixins/insights.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    16412 2021-07-28 13:02:38.000000 instagrapi-1.9.9/instagrapi/mixins/challenge.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    28689 2021-07-31 08:29:50.000000 instagrapi-1.9.9/instagrapi/mixins/video.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    15152 2021-07-29 16:44:34.000000 instagrapi-1.9.9/instagrapi/mixins/private.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4829 2021-08-05 14:13:36.000000 instagrapi-1.9.9/instagrapi/mixins/account.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2790 2021-07-27 07:46:15.000000 instagrapi-1.9.9/instagrapi/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     7137 2021-08-03 09:21:53.000000 instagrapi-1.9.9/instagrapi/types.py
+-rw-rw-r--   0 adw0rd     (501) staff       (20)      311 2021-02-27 05:34:00.000000 instagrapi-1.9.9/instagrapi/zones.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2709 2021-07-28 13:02:21.000000 instagrapi-1.9.9/instagrapi/utils.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     4748 2021-06-18 12:42:06.000000 instagrapi-1.9.9/instagrapi/exceptions.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2079 2021-08-06 11:53:08.000000 instagrapi-1.9.9/PKG-INFO
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2079 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      985 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       74 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       11 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2021-08-06 11:53:08.000000 instagrapi-1.9.9/instagrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)     8335 2021-08-02 21:24:52.000000 instagrapi-1.9.9/README.md
+-rw-r--r--   0 adw0rd     (501) staff       (20)     2530 2021-08-06 11:53:05.000000 instagrapi-1.9.9/setup.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2021-08-06 11:53:08.000000 instagrapi-1.9.9/setup.cfg
```

### Comparing `instagrapi-1.9.8/instagrapi/story.py` & `instagrapi-1.9.9/instagrapi/story.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/config.py` & `instagrapi-1.9.9/instagrapi/config.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/extractors.py` & `instagrapi-1.9.9/instagrapi/extractors.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/auth.py` & `instagrapi-1.9.9/instagrapi/mixins/auth.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/story.py` & `instagrapi-1.9.9/instagrapi/mixins/story.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/user.py` & `instagrapi-1.9.9/instagrapi/mixins/user.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/public.py` & `instagrapi-1.9.9/instagrapi/mixins/public.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import json
 import logging
 import time
-from json.decoder import JSONDecodeError
+
+try:
+    from simplejson.errors import JSONDecodeError
+except ImportError:
+    from json.decoder import JSONDecodeError
 
 import requests
 
 from instagrapi.exceptions import (
     ClientBadRequestError,
     ClientConnectionError,
     ClientError,
@@ -21,14 +25,16 @@
 from instagrapi.utils import json_value
 
 
 class PublicRequestMixin:
     public_requests_count = 0
     PUBLIC_API_URL = "https://www.instagram.com/"
     GRAPHQL_PUBLIC_API_URL = "https://www.instagram.com/graphql/query/"
+    last_public_response = None
+    last_public_json = {}
     request_logger = logging.getLogger("public_request")
     request_timeout = 1
 
     def __init__(self, *args, **kwargs):
         self.public = requests.Session()
         self.public.headers.update(
             {
@@ -59,21 +65,18 @@
             return_json=return_json,
         )
         assert retries_count <= 10, "Retries count is too high"
         assert retries_timeout <= 600, "Retries timeout is too high"
         for iteration in range(retries_count):
             try:
                 return self._send_public_request(url, **kwargs)
-            except (
-                ClientLoginRequired,
-                ClientNotFoundError,
-                ClientBadRequestError,
-            ) as e:
-                # Stop retries
-                raise e
+            except (ClientLoginRequired, ClientNotFoundError, ClientBadRequestError) as e:
+                raise e  # Stop retries
+            # except JSONDecodeError as e:
+            #     raise ClientJSONDecodeError(e, respones=self.last_public_response)
             except ClientError as e:
                 msg = str(e)
                 if all((
                     isinstance(e, ClientConnectionError),
                     "SOCKSHTTPSConnectionPool" in msg,
                     "Max retries exceeded with url" in msg,
                     "Failed to establish a new connection" in msg
@@ -116,17 +119,20 @@
             self.request_logger.info(
                 "[%s] [%s] %s %s",
                 self.public.proxies.get("https"),
                 response.status_code,
                 "POST" if data else "GET",
                 response.url,
             )
-
+            self.last_public_response = response
             response.raise_for_status()
-            return response.json() if return_json else response.text
+            if return_json:
+                self.last_public_json = response.json()
+                return self.last_public_json
+            return response.text
 
         except JSONDecodeError as e:
             if "/login/" in response.url:
                 raise ClientLoginRequired(e, response=response)
 
             self.request_logger.error(
                 "Status %s: JSONDecodeError in public_request (url=%s) >>> %s",
```

### Comparing `instagrapi-1.9.8/instagrapi/mixins/media.py` & `instagrapi-1.9.9/instagrapi/mixins/media.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/timeline.py` & `instagrapi-1.9.9/instagrapi/mixins/timeline.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/comment.py` & `instagrapi-1.9.9/instagrapi/mixins/comment.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/igtv.py` & `instagrapi-1.9.9/instagrapi/mixins/igtv.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/album.py` & `instagrapi-1.9.9/instagrapi/mixins/album.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/hashtag.py` & `instagrapi-1.9.9/instagrapi/mixins/hashtag.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/location.py` & `instagrapi-1.9.9/instagrapi/mixins/location.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/collection.py` & `instagrapi-1.9.9/instagrapi/mixins/collection.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/photo.py` & `instagrapi-1.9.9/instagrapi/mixins/photo.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/direct.py` & `instagrapi-1.9.9/instagrapi/mixins/direct.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/password.py` & `instagrapi-1.9.9/instagrapi/mixins/password.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/clip.py` & `instagrapi-1.9.9/instagrapi/mixins/clip.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/insights.py` & `instagrapi-1.9.9/instagrapi/mixins/insights.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/challenge.py` & `instagrapi-1.9.9/instagrapi/mixins/challenge.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/video.py` & `instagrapi-1.9.9/instagrapi/mixins/video.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/private.py` & `instagrapi-1.9.9/instagrapi/mixins/private.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/mixins/account.py` & `instagrapi-1.9.9/instagrapi/mixins/account.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/__init__.py` & `instagrapi-1.9.9/instagrapi/__init__.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/types.py` & `instagrapi-1.9.9/instagrapi/types.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/utils.py` & `instagrapi-1.9.9/instagrapi/utils.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/instagrapi/exceptions.py` & `instagrapi-1.9.9/instagrapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/PKG-INFO` & `instagrapi-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagrapi
-Version: 1.9.8
+Version: 1.9.9
 Summary: Fast and effective Instagram Private API wrapper
 Home-page: https://github.com/adw0rd/instagrapi
 Author: Mikhail Andreev
 Author-email: x11org@gmail.com
 License: MIT
 Description: 
         Fast and effective Instagram Private API wrapper (public+private requests and challenge resolver).
```

### Comparing `instagrapi-1.9.8/instagrapi.egg-info/PKG-INFO` & `instagrapi-1.9.9/instagrapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagrapi
-Version: 1.9.8
+Version: 1.9.9
 Summary: Fast and effective Instagram Private API wrapper
 Home-page: https://github.com/adw0rd/instagrapi
 Author: Mikhail Andreev
 Author-email: x11org@gmail.com
 License: MIT
 Description: 
         Fast and effective Instagram Private API wrapper (public+private requests and challenge resolver).
```

### Comparing `instagrapi-1.9.8/instagrapi.egg-info/SOURCES.txt` & `instagrapi-1.9.9/instagrapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/README.md` & `instagrapi-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `instagrapi-1.9.8/setup.py` & `instagrapi-1.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # requirements = [
 #     line.strip()
 #     for line in open('requirements.txt').readlines()
 # ]
 
 setup(
     name='instagrapi',
-    version='1.9.8',
+    version='1.9.9',
     author='Mikhail Andreev',
     author_email='x11org@gmail.com',
     license='MIT',
     url='https://github.com/adw0rd/instagrapi',
     install_requires=requirements,
     keywords=[
         'instagram private api', 'instagram-private-api', 'instagram api', 'instagram-api', 'instagram',
```

