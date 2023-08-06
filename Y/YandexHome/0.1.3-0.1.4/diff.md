# Comparing `tmp/YandexHome-0.1.3.tar.gz` & `tmp/YandexHome-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.3.tar", last modified: Sun Aug  6 14:36:26 2023, max compression
+gzip compressed data, was "YandexHome-0.1.4.tar", last modified: Sun Aug  6 14:58:50 2023, max compression
```

## Comparing `YandexHome-0.1.3.tar` & `YandexHome-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.299953 YandexHome-0.1.3/
--rw-rw-rw-   0        0        0      132 2023-08-06 14:36:26.298951 YandexHome-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-06 14:35:59.000000 YandexHome-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 14:36:26.299953 YandexHome-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.280835 YandexHome-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.288875 YandexHome-0.1.3/src/YandexHome/
--rw-rw-rw-   0        0        0     5343 2023-08-06 14:34:39.000000 YandexHome-0.1.3/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     5894 2023-08-06 12:54:07.000000 YandexHome-0.1.3/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3097 2023-08-06 13:03:56.000000 YandexHome-0.1.3/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.3/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 14:36:26.296981 YandexHome-0.1.3/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 14:36:26.000000 YandexHome-0.1.3/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 14:58:50.266238 YandexHome-0.1.4/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:58:50.266238 YandexHome-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-06 14:58:38.000000 YandexHome-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 14:58:50.266238 YandexHome-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 14:58:50.245231 YandexHome-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 14:58:50.255251 YandexHome-0.1.4/src/YandexHome/
+-rw-rw-rw-   0        0        0     5331 2023-08-06 14:58:22.000000 YandexHome-0.1.4/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     5901 2023-08-06 14:41:39.000000 YandexHome-0.1.4/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3103 2023-08-06 14:41:53.000000 YandexHome-0.1.4/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.4/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:58:50.264229 YandexHome-0.1.4/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 14:58:50.000000 YandexHome-0.1.4/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 14:58:50.000000 YandexHome-0.1.4/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 14:58:50.000000 YandexHome-0.1.4/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-06 14:58:50.000000 YandexHome-0.1.4/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 14:58:50.000000 YandexHome-0.1.4/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.3/src/YandexHome/__init__.py` & `YandexHome-0.1.4/src/YandexHome/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
     async def get_scenarios(self):
         user_data = await self.get_user()
         scenarios = []
         for scenario in user_data['scenarios']:
             scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active']))
         return scenarios
             
-    async def get_device(self, deviceId: str):
+    async def get_device(self, id: str):
         async with ClientSession() as session:
-            async with session.get(f'https://api.iot.yandex.net/v1.0/devices/{deviceId}', headers={'Authorization': f'Bearer {self.token}'}) as req:
+            async with session.get(f'https://api.iot.yandex.net/v1.0/devices/{id}', headers={'Authorization': f'Bearer {self.token}'}) as req:
                 json = await req.json()
                 if json['status'] == 'ok':
                     device = Device(json['id'], json['name'], json['aliases'], json['room'], json['external_id'], json['skill_id'], json['type'], json['groups'], json['capabilities'], json['properties'], json.get('household_id', '0'), self.token)
                     return device
                 else:
                     raise YandexHomeError(json['message'])
```

### Comparing `YandexHome-0.1.3/src/YandexHome/device.py` & `YandexHome-0.1.4/src/YandexHome/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return f'<Capability retrievable={self.retrievable} type={self.type} parameters={self.parameters} {self.state["instance"]}={self.state["value"]} last_updated={self.last_updated} reportable={self.reportable}>'
     
     def __repr__(self) -> str:
         return self.__str__()
 
 class Device:
     def __init__(self, id: str, name: str, aliases: list[str], room: str, external_id: str, skill_id: str, device_type: str, groups: list[str], capabilities: list[dict], properties: list[dict], household_id: str, token: str):
-        self.__attr = ['id', 'name', 'aliases', 'room', 'external_id', 'skill_id', 'type', 'groups', '_Device__capabilities', '_Device__properties', 'household_id', '__token', 'avaible_properties']
+        self.__attr = ['id', 'name', 'aliases', 'room', 'external_id', 'skill_id', 'type', 'groups', 'household_id', '_Device__token', 'avaible_properties', '_Device__capabilities', '_Device__properties']
         self.id = id
         self.name = name
         self.aliases = aliases
         self.room = room
         self.external_id = external_id
         self.skill_id = skill_id
         self.type = device_type
```

### Comparing `YandexHome-0.1.3/src/YandexHome/group.py` & `YandexHome-0.1.4/src/YandexHome/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 device = Device(json['id'], json['name'], json['aliases'], json['room'], json['external_id'], json['skill_id'], json['type'], json['groups'], json['capabilities'], json['properties'], json.get('household_id', '0'), token)
                 return device
             else:
                 raise YandexHomeError(json['message'])
 
 class Group:
     def __init__(self, id: str, name: str, aliases: list[str], group_type: str, state: Literal['online', 'offline', 'split'], devices: list, token: str) -> None:
-        self.__attr = ['id', 'name', 'aliases', 'type', 'state', 'devices', '__token', 'capabilities', 'avaible_properties']
+        self.__attr = ['id', 'name', 'aliases', 'type', 'state', 'devices', '_Group__token', 'capabilities', 'avaible_properties']
         self.id = id
         self.name = name
         self.aliases = aliases
         self.type = group_type
         self.state = state
         self.devices: list[Device] = []
         self.__token = token
```

### Comparing `YandexHome-0.1.3/src/YandexHome/scenario.py` & `YandexHome-0.1.4/src/YandexHome/scenario.py`

 * *Files identical despite different names*

