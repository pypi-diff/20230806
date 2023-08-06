# Comparing `tmp/YandexHome-0.1.2.tar.gz` & `tmp/YandexHome-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.2.tar", last modified: Sun Aug  6 14:30:05 2023, max compression
+gzip compressed data, was "YandexHome-0.1.3.tar", last modified: Sun Aug  6 14:36:26 2023, max compression
```

## Comparing `YandexHome-0.1.2.tar` & `YandexHome-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.261152 YandexHome-0.1.2/
--rw-rw-rw-   0        0        0      132 2023-08-06 14:30:05.261152 YandexHome-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-08-06 14:29:35.000000 YandexHome-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 14:30:05.261152 YandexHome-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.242187 YandexHome-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.249546 YandexHome-0.1.2/src/YandexHome/
--rw-rw-rw-   0        0        0     5200 2023-08-06 13:05:18.000000 YandexHome-0.1.2/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.2/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3097 2023-08-06 13:03:56.000000 YandexHome-0.1.2/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.2/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 14:30:05.259152 YandexHome-0.1.2/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 14:30:05.000000 YandexHome-0.1.2/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.299953 YandexHome-0.1.3/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:36:26.298951 YandexHome-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-06 14:35:59.000000 YandexHome-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 14:36:26.299953 YandexHome-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.280835 YandexHome-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.288875 YandexHome-0.1.3/src/YandexHome/
+-rw-rw-rw-   0        0        0     5343 2023-08-06 14:34:39.000000 YandexHome-0.1.3/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.3/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3097 2023-08-06 13:03:56.000000 YandexHome-0.1.3/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.3/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.296981 YandexHome-0.1.3/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.2/src/YandexHome/__init__.py` & `YandexHome-0.1.3/src/YandexHome/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from threading import Thread, Event
 from base64 import b64encode
 from aiohttp import ClientSession
 from .device import Device
 from .scenario import Scenario
 from .group import Group
 from typing import Any
+import webbrowser
 
 class StoppableThread(Thread):
     """Thread class with a stop() method. The thread itself has to check
     regularly for the stopped() condition."""
 
     def __init__(self,  *args, **kwargs):
         super(StoppableThread, self).__init__(*args, **kwargs)
@@ -38,14 +39,15 @@
             pclient_secret = client_secret
             self.get_token()
         elif (not token and not client_id and client_secret) or (not token and client_id and not client_secret) or (not token and not client_id and not client_secret):
             raise ClientDataInvalid("Отсутствуют client_id и client_secret для получения токена!")
         self.token = token
 
     def get_token(self):
+        webbrowser.open('https://oauth.yandex.ru/authorize?response_type=code&client_id=d347a18dfe8d40e6ba4ffa3eb1026415')
         server.start()
         server.join()
 
     async def get_user(self):
         async with ClientSession() as session:
             async with session.get('https://api.iot.yandex.net/v1.0/user/info', headers={'Authorization': f'Bearer {self.token}'}) as req:
                 json = await req.json()
```

### Comparing `YandexHome-0.1.2/src/YandexHome/device.py` & `YandexHome-0.1.3/src/YandexHome/device.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.2/src/YandexHome/group.py` & `YandexHome-0.1.3/src/YandexHome/group.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.2/src/YandexHome/scenario.py` & `YandexHome-0.1.3/src/YandexHome/scenario.py`

 * *Files identical despite different names*

