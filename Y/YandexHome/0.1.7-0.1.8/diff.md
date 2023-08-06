# Comparing `tmp/YandexHome-0.1.7.tar.gz` & `tmp/YandexHome-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.7.tar", last modified: Sun Aug  6 15:40:21 2023, max compression
+gzip compressed data, was "YandexHome-0.1.8.tar", last modified: Sun Aug  6 15:52:16 2023, max compression
```

## Comparing `YandexHome-0.1.7.tar` & `YandexHome-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:40:21.267205 YandexHome-0.1.7/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:40:21.266198 YandexHome-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-06 15:40:06.000000 YandexHome-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 15:40:21.267205 YandexHome-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 15:40:21.248571 YandexHome-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 15:40:21.256585 YandexHome-0.1.7/src/YandexHome/
--rw-rw-rw-   0        0        0     8386 2023-08-06 15:39:56.000000 YandexHome-0.1.7/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.7/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3103 2023-08-06 14:41:53.000000 YandexHome-0.1.7/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.7/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:40:21.264590 YandexHome-0.1.7/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:40:21.000000 YandexHome-0.1.7/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 15:40:21.000000 YandexHome-0.1.7/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:40:21.000000 YandexHome-0.1.7/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-06 15:40:21.000000 YandexHome-0.1.7/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 15:40:21.000000 YandexHome-0.1.7/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.185297 YandexHome-0.1.8/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:52:16.185297 YandexHome-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-06 15:47:45.000000 YandexHome-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:52:16.186344 YandexHome-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.168673 YandexHome-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.175689 YandexHome-0.1.8/src/YandexHome/
+-rw-rw-rw-   0        0        0     8436 2023-08-06 15:50:22.000000 YandexHome-0.1.8/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.8/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3459 2023-08-06 15:51:56.000000 YandexHome-0.1.8/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.8/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.183298 YandexHome-0.1.8/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.7/src/YandexHome/__init__.py` & `YandexHome-0.1.8/src/YandexHome/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,59 +64,59 @@
             devices.append(device)
         return devices
                 
     async def get_groups(self):
         user_data = await self.get_user()
         groups = []
         for group in user_data['groups']:
-            group = Group(group['id'], group['name'], group['aliases'], group['group_type'], group['state'], group['devices'], self.token)
+            group = Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token)
             groups.append(group)
         return groups
     
     async def get_group(self, id: str = None, *, name: str = None):
         user_data = await self.get_user()
         if name or id:
             groups = []
             for group in user_data['groups']:
                 if id != None:
                     if group['id'] == id:
-                        group = Group(group['id'], group['name'], group['aliases'], group['group_type'], group['state'], group['devices'], self.token)
+                        group = Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token)
                         return group
                 if name != None:
                     if group['name'].lower() == name.lower() or name.lower() in [alias.lower() for alias in group['aliases']]:
-                        groups.append(Group(group['id'], group['name'], group['aliases'], group['group_type'], group['state'], group['devices'], self.token))
+                        groups.append(Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token))
             if len(groups) > 0:
                 if len(groups) == 1:
                     return groups[0]
                 else:
                     return groups
             else:
                 raise YandexHomeError("Группы с таким именем не найдены!")
         else:
             raise YandexHomeError('Не указан ни id, ни name.')
 
     async def get_scenarios(self):
         user_data = await self.get_user()
         scenarios = []
         for scenario in user_data['scenarios']:
-            scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active']))
+            scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active'], self.token))
         return scenarios
     
     async def get_scenario(self, id: str = None, *, name: str = None):
         user_data = await self.get_user()
         if name or id:
             scenarios = []
             for scenario in user_data['scenarios']:
                 if id != None:
                     if scenario['id'] == id:
-                        scenario = Scenario(scenario['id'], scenario['name'], scenario['is_active'])
+                        scenario = Scenario(scenario['id'], scenario['name'], scenario['is_active'], self.token)
                         return scenario
                 if name != None:
                     if scenario['name'].lower() == scenario['name'].lower():
-                        scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active']))
+                        scenarios.append(Scenario(scenario['id'], scenario['name'], scenario['is_active'], self.token))
             if len(scenarios) > 0:
                 if len(scenarios) == 1:
                     return scenarios[0]
                 else:
                     return scenarios
             else:
                 raise YandexHomeError("Сценарии с таким именем не найдены!")
@@ -134,23 +134,23 @@
                     else:
                         raise YandexHomeError(json['message'])
         if name:
             devices = await self.get_devices()
             founded_devices = []
             for device in devices:
                 device: Device
-                if name.lower == device.name.lower() or name.lower() in [x.lower() for x in device.aliases]:
-                    founded_devices.append(device)
+                if name.lower() == device.name.lower() or name.lower() in [x.lower() for x in device.aliases]:
+                    founded_devices.append(await self.get_device(device.id))
             if len(founded_devices) > 0:
                 if len(founded_devices) == 1:
                     return founded_devices[0]
                 else:
                     return founded_devices
             else:
-                raise YandexHomeError("Сценарии с таким именем не найдены!")
+                raise YandexHomeError("Устройства с таким именем не найдены!")
         raise YandexHomeError('Не указан ни id, ни name.')
 
 
             
     async def action(self, device: Device, actionType: str, instance: str, value: Any):
         async with ClientSession() as session:
             async with session.post(f'https://api.iot.yandex.net/v1.0/devices/actions', headers={'Authorization': f'Bearer {self.token}'}, json={'devices': [{'id': device.id, 'actions': [{'type': actionType, 'state': {'instance': instance, 'value': value}}]}]}) as req:
```

### Comparing `YandexHome-0.1.7/src/YandexHome/device.py` & `YandexHome-0.1.8/src/YandexHome/device.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.7/src/YandexHome/group.py` & `YandexHome-0.1.8/src/YandexHome/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,29 @@
         for device in self.devices:
             for capability in device.capabilities:
                 self.capabilities.append(capability)
         self.avaible_properties = []
         for capability in self.capabilities:
             self.avaible_properties.append(capability.instance)
             self.__setattr__(capability.instance, capability.__getattribute__(capability.instance))
-
+            
     def __setattr__(self, __name: str, __value: Any) -> None:
+        first = False
+        try: self.__getattribute__(__name)
+        except: first = True
         object.__setattr__(self, __name, __value)
-        if __name not in self.__attr and __name != '__attr':
+        if __name not in self.__attr and __name != '_Device__attr' and not first:
             action_type = ''
             for capability in self.capabilities:
                 if capability.instance == __name:
                     action_type = capability.type
             req = run(post(f'https://api.iot.yandex.net/v1.0/groups/{self.id}/actions', headers={'Authorization': f'Bearer {self.__token}'}, json={'actions': [{'type': action_type, 'state': {'instance': __name, 'value': __value}}]}))
             if req['status'] == 'error':
                 raise YandexHomeError(req['message'])
+            if req['devices'][0]['capabilities'][0]['state']['action_result']['status'].lower() == 'error':
+                raise YandexHomeError(req['devices'][0]['capabilities'][0]['state']['action_result']['error_code'])
             
     def __str__(self):
         return f'<Group avaible_properties={self.avaible_properties} id={self.id} name={self.name} aliases={self.aliases} type={self.type} state={self.state} devices={self.devices} capabilities={self.capabilities}>'
     
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `YandexHome-0.1.7/src/YandexHome/scenario.py` & `YandexHome-0.1.8/src/YandexHome/scenario.py`

 * *Files identical despite different names*

