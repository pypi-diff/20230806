# Comparing `tmp/YandexHome-0.0.3.tar.gz` & `tmp/YandexHome-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.0.3.tar", last modified: Sun Aug  6 09:59:45 2023, max compression
+gzip compressed data, was "YandexHome-0.1.0.tar", last modified: Sun Aug  6 12:55:40 2023, max compression
```

## Comparing `YandexHome-0.0.3.tar` & `YandexHome-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:59:45.293783 YandexHome-0.0.3/
--rw-rw-rw-   0        0        0      118 2023-08-06 09:59:45.292781 YandexHome-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-08-06 09:59:29.000000 YandexHome-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 09:59:45.293783 YandexHome-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 09:59:45.275784 YandexHome-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 09:59:45.280293 YandexHome-0.0.3/src/YandexHome/
-drwxrwxrwx   0        0        0        0 2023-08-06 09:59:45.291748 YandexHome-0.0.3/src/YandexHome/Device/
--rw-rw-rw-   0        0        0     4888 2023-08-06 09:16:21.000000 YandexHome-0.0.3/src/YandexHome/Device/__init__.py
--rw-rw-rw-   0        0        0     4244 2023-08-06 09:59:25.000000 YandexHome-0.0.3/src/YandexHome/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:59:45.289811 YandexHome-0.0.3/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      118 2023-08-06 09:59:45.000000 YandexHome-0.0.3/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-08-06 09:59:45.000000 YandexHome-0.0.3/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:59:45.000000 YandexHome-0.0.3/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-08-06 09:59:45.000000 YandexHome-0.0.3/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 09:59:45.000000 YandexHome-0.0.3/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 12:55:40.709807 YandexHome-0.1.0/
+-rw-rw-rw-   0        0        0      132 2023-08-06 12:55:40.708969 YandexHome-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-08-06 12:55:15.000000 YandexHome-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 12:55:40.709807 YandexHome-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 12:55:40.673099 YandexHome-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 12:55:40.683120 YandexHome-0.1.0/src/YandexHome/
+-rw-rw-rw-   0        0        0     5200 2023-08-06 12:54:37.000000 YandexHome-0.1.0/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.0/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     2785 2023-08-06 12:34:13.000000 YandexHome-0.1.0/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.0/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:55:40.692137 YandexHome-0.1.0/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 12:55:40.000000 YandexHome-0.1.0/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 12:55:40.000000 YandexHome-0.1.0/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 12:55:40.000000 YandexHome-0.1.0/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-06 12:55:40.000000 YandexHome-0.1.0/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 12:55:40.000000 YandexHome-0.1.0/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.0.3/src/YandexHome/__init__.py` & `YandexHome-0.1.0/src/YandexHome/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from flask import Flask, request
 from threading import Thread, Event
-import base64
-import aiohttp
-from .Device import Device
+from base64 import b64encode
+from aiohttp import ClientSession
+from .device import Device
+from .scenario import Scenario
+from .group import Group
 from typing import Any
 
 class StoppableThread(Thread):
     """Thread class with a stop() method. The thread itself has to check
     regularly for the stopped() condition."""
 
     def __init__(self,  *args, **kwargs):
@@ -16,14 +18,15 @@
     def stop(self):
         self._stop_event.set()
 
     def stopped(self):
         return self._stop_event.is_set()
 
 class ClientDataInvalid(BaseException): pass
+class YandexHomeError(BaseException): pass
 
 app = Flask(__name__)
 server = StoppableThread(target=app.run, args=('localhost', 5030))
 pclient_id = None
 pclient_secret = None
 
 class YandexHome:
@@ -38,49 +41,71 @@
             raise ClientDataInvalid("Отсутствуют client_id и client_secret для получения токена!")
         self.token = token
 
     def get_token(self):
         server.start()
         server.join()
 
-    async def get_devices(self):
-        async with aiohttp.ClientSession() as session:
+    async def get_user(self):
+        async with ClientSession() as session:
             async with session.get('https://api.iot.yandex.net/v1.0/user/info', headers={'Authorization': f'Bearer {self.token}'}) as req:
                 json = await req.json()
                 if json['status'] == 'ok':
-                    devices = []
-                    for device in json['devices']:
-                        device = Device(device['id'], device['name'], device['aliases'], device['room'], device['external_id'], device['skill_id'], device['type'], device['groups'], device['capabilities'], device['properties'], device['household_id'], self.token)
-                        devices.append(device)
-                    return devices
+                    return json
                 else:
-                    return 'error!'
+                    raise YandexHomeError(json['message'])
+
+    async def get_devices(self):
+        user_data = await self.get_user()
+        devices = []
+        for device in user_data['devices']:
+            device = Device(device['id'], device['name'], device['aliases'], device['room'], device['external_id'], device['skill_id'], device['type'], device['groups'], device['capabilities'], device['properties'], device['household_id'], self.token)
+            devices.append(device)
+        return devices
+                
+    async def get_groups(self):
+        user_data = await self.get_user()
+        groups = []
+        for group in user_data['groups']:
+            group = Group(group['id'], group['name'], group['aliases'], group['group_type'], group['state'], group['devices'], self.token)
+            groups.append(group)
+        return groups
+    
+    async def get_scenarios(self):
+        user_data = await self.get_user()
+        scenarios = []
+        for scenario in user_data['scenarios']:
+            scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active']))
+        return scenarios
             
-    async def get_device_state(self, deviceId: str):
-        async with aiohttp.ClientSession() as session:
+    async def get_device(self, deviceId: str):
+        async with ClientSession() as session:
             async with session.get(f'https://api.iot.yandex.net/v1.0/devices/{deviceId}', headers={'Authorization': f'Bearer {self.token}'}) as req:
                 json = await req.json()
                 if json['status'] == 'ok':
                     device = Device(json['id'], json['name'], json['aliases'], json['room'], json['external_id'], json['skill_id'], json['type'], json['groups'], json['capabilities'], json['properties'], json.get('household_id', '0'), self.token)
                     return device
                 else:
-                    return 'error!'
+                    raise YandexHomeError(json['message'])
             
     async def action(self, device: Device, actionType: str, instance: str, value: Any):
-        async with aiohttp.ClientSession() as session:
+        async with ClientSession() as session:
             async with session.post(f'https://api.iot.yandex.net/v1.0/devices/actions', headers={'Authorization': f'Bearer {self.token}'}, json={'devices': [{'id': device.id, 'actions': [{'type': actionType, 'state': {'instance': instance, 'value': value}}]}]}) as req:
                 json = await req.json()
-                return json
+                if json['status'] == 'ok':
+                    return json
+                else:
+                    raise YandexHomeError(json['message'])
 
 @app.route('/')
 async def yandex_callback():
     if pclient_id and pclient_secret:
         code = request.args.get('code')
         auth = f"{pclient_id}:{pclient_secret}"
         auth_bytes = auth.encode('ascii')
-        base64_bytes = base64.b64encode(auth_bytes)
+        base64_bytes = b64encode(auth_bytes)
         base64_auth = base64_bytes.decode('ascii')
-        async with aiohttp.ClientSession() as session:
+        async with ClientSession() as session:
             async with session.post('https://oauth.yandex.ru/token', headers={'Authorization': f'Basic {base64_auth}'}, data={'grant_type': 'authorization_code', 'code': code}) as req:
                 json = await req.json()
                 token = json['access_token']
-                return f'Твой токен: {token}'
+                return f'Твой токен: {token}'
```

