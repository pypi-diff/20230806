# Comparing `tmp/pymstodo-0.1.4.tar.gz` & `tmp/pymstodo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymstodo-0.1.4.tar", last modified: Tue Jun 13 05:46:44 2023, max compression
+gzip compressed data, was "pymstodo-0.1.5.tar", last modified: Sun Aug  6 16:46:45 2023, max compression
```

## Comparing `pymstodo-0.1.4.tar` & `pymstodo-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 05:46:35.000000 pymstodo-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 05:46:44.078767 pymstodo-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-13 05:46:35.000000 pymstodo-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/pymstodo/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 05:46:35.000000 pymstodo-0.1.4/pymstodo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18722 2023-06-13 05:46:35.000000 pymstodo-0.1.4/pymstodo/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:46:44.078767 pymstodo-0.1.4/pymstodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 05:46:44.000000 pymstodo-0.1.4/pymstodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:46:44.078767 pymstodo-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 05:46:35.000000 pymstodo-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:46:45.301438 pymstodo-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-06 16:46:36.000000 pymstodo-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-06 16:46:45.301438 pymstodo-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-06 16:46:36.000000 pymstodo-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:46:45.297438 pymstodo-0.1.5/pymstodo/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-06 16:46:36.000000 pymstodo-0.1.5/pymstodo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-08-06 16:46:36.000000 pymstodo-0.1.5/pymstodo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 16:46:36.000000 pymstodo-0.1.5/pymstodo/windows_zones_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:46:45.301438 pymstodo-0.1.5/pymstodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-06 16:46:45.000000 pymstodo-0.1.5/pymstodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-06 16:46:45.000000 pymstodo-0.1.5/pymstodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:46:45.000000 pymstodo-0.1.5/pymstodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 16:46:45.000000 pymstodo-0.1.5/pymstodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 16:46:45.000000 pymstodo-0.1.5/pymstodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 16:46:45.301438 pymstodo-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-06 16:46:36.000000 pymstodo-0.1.5/setup.py
```

### Comparing `pymstodo-0.1.4/LICENSE` & `pymstodo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.4/PKG-INFO` & `pymstodo-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymstodo-0.1.4/README.md` & `pymstodo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pymstodo-0.1.4/pymstodo/client.py` & `pymstodo-0.1.5/pymstodo/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-import os
-import time
-import json
 import dataclasses
-from datetime import datetime
+import json
+import time
+from datetime import datetime, timezone
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 from requests_oauthlib import OAuth2Session
+from zoneinfo import ZoneInfo
+
+from .windows_zones_adapter import get_zoneinfo_name_by_windows_zone
 
 
 class PymstodoError(Exception):
     '''Basic Pymstodo exception'''
-    pass
+
+    def __init__(self, status_code: int, reason: str):
+        super().__init__(f'Error {status_code}: {reason}')
 
 
 class Token(TypedDict):
     token_type: str
     scope: List[str]
     expires_in: int
     ext_expires_in: int
     access_token: str
     refresh_token: str
     id_token: str
     expires_at: float
 
 
-class _DueDate(TypedDict):
+class _DateTimeTimeZone(TypedDict):
     dateTime: str
     timeZone: str
 
 
 class _Body(TypedDict):
     content: str
     contentType: Literal['text', 'html']
@@ -128,21 +132,22 @@
     '''Unique identifier for the task. By default, this value changes when the item is moved from one list to another'''
 
     body: _Body
 
     categories: list[str]
     '''The categories associated with the task'''
 
-    completedDateTime: str
-    '''The date and time in the specified time zone that the task was finished. It is in UTC and uses ISO 8601 format'''
+    completedDateTime: _DateTimeTimeZone
+    '''The date and time in the specified time zone that the task was finished. Uses ISO 8601 format'''
 
     createdDateTime: str
     '''The date and time when the task was created. It is in UTC and uses ISO 8601 format'''
 
-    dueDateTime: _DueDate
+    dueDateTime: _DateTimeTimeZone
+    '''The date and time in the specified time zone that the task is to be finished. Uses ISO 8601 format'''
 
     hasAttachments: bool
     '''Indicates whether the task has attachments'''
 
     title: str
     '''A brief description of the task'''
 
@@ -151,18 +156,18 @@
 
     isReminderOn: bool
     '''Set to true if an alert is set to remind the user of the task'''
 
     lastModifiedDateTime: str
     '''The date and time when the task was last modified. It is in UTC and uses ISO 8601 format'''
 
-    reminderDateTime: str
+    reminderDateTime: _DateTimeTimeZone
     '''The date and time in the specified time zone for a reminder alert of the task to occur. Uses ISO 8601 format'''
 
-    startDateTime: str
+    startDateTime: _DateTimeTimeZone
     '''The date and time in the specified time zone at which the task is scheduled to start. Uses ISO 8601 format'''
 
     status: str
 
     def __init__(self, **kwargs: Any) -> None:
         for f in dataclasses.fields(self):
             setattr(self, f.name, kwargs.get('id' if f.name == 'task_id' else f.name))
@@ -175,78 +180,71 @@
         return title
 
     @property
     def body_text(self) -> Optional[str]:
         '''The task body that typically contains information about the task'''
         if self.body:
             return self.body['content']
-        else:
-            return None
+        return None
 
     @property
     def completed_date(self) -> Optional[datetime]:
         '''The date and time in the specified time zone that the task was finished'''
         if self.completedDateTime:
-            return datetime.strptime(self.completedDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.completedDateTime['dateTime']).astimezone(ZoneInfo(get_zoneinfo_name_by_windows_zone(self.completedDateTime['timeZone'])))
+        return None
 
     @property
     def created_date(self) -> Optional[datetime]:
         '''The date and time when the task was created. It is in UTC'''
         if self.createdDateTime:
-            return datetime.strptime(self.createdDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.createdDateTime).astimezone(timezone.utc)
+        return None
 
     @property
     def due_date(self) -> Optional[datetime]:
         '''The date and time in the specified time zone that the task is to be finished'''
         if self.dueDateTime:
-            return datetime.strptime(self.dueDateTime['dateTime'].split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.dueDateTime['dateTime']).astimezone(ZoneInfo(get_zoneinfo_name_by_windows_zone(self.dueDateTime['timeZone'])))
+        return None
 
     @property
     def last_mod_date(self) -> Optional[datetime]:
         '''The date and time when the task was last modified. It is in UTC'''
         if self.lastModifiedDateTime:
-            return datetime.strptime(self.lastModifiedDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.lastModifiedDateTime).astimezone(timezone.utc)
+        return None
 
     @property
     def reminder_date(self) -> Optional[datetime]:
         '''The date and time in the specified time zone for a reminder alert of the task to occur'''
         if self.reminderDateTime:
-            return datetime.strptime(self.reminderDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.reminderDateTime['dateTime']).astimezone(ZoneInfo(get_zoneinfo_name_by_windows_zone(self.reminderDateTime['timeZone'])))
+        return None
 
     @property
     def start_date(self) -> Optional[datetime]:
         '''The date and time in the specified time zone at which the task is scheduled to start'''
         if self.startDateTime:
-            return datetime.strptime(self.startDateTime.split('.')[0], '%Y-%m-%dT%H:%M:%S')
-        else:
-            return None
+            return datetime.fromisoformat(self.startDateTime['dateTime']).astimezone(ZoneInfo(get_zoneinfo_name_by_windows_zone(self.startDateTime['timeZone'])))
+        return None
 
     @property
     def task_status(self) -> TaskStatus:
         '''Indicates the state or progress of the task'''
         return TaskStatus(self.status)
 
 
 class ToDoConnection:
     '''**To-Do connection** is your entry point to the To-Do API
 
     Args:
         client_id: API client ID
         client_secret: API client secret
-        token: Token obtained by method `get_token`        
+        token: Token obtained by method `get_token`
     '''
     _redirect: str = 'https://localhost/login/authorized'
     _scope: str = 'openid Tasks.ReadWrite'
     _authority: str = 'https://login.microsoftonline.com/common'
     _authorize_endpoint: str = '/oauth2/v2.0/authorize'
     _token_endpoint: str = '/oauth2/v2.0/token'
     _base_api_url: str = 'https://graph.microsoft.com/v1.0/me/todo/'
@@ -274,17 +272,16 @@
         return authorization_url
 
     @staticmethod
     def get_token(client_id: str, client_secret: str, redirect_resp: str) -> Any:
         '''Fetch the access token'''
         oa_sess = OAuth2Session(client_id, scope=ToDoConnection._scope, redirect_uri=ToDoConnection._redirect)
         token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
-        token = oa_sess.fetch_token(token_url, client_secret=client_secret, authorization_response=redirect_resp)
+        return oa_sess.fetch_token(token_url, client_secret=client_secret, authorization_response=redirect_resp)
 
-        return token
 
     def _refresh_token(self) -> None:
         now = time.time()
         expire_time = self.token['expires_at'] - 300
         if now >= expire_time:
             token_url = f'{ToDoConnection._authority}{ToDoConnection._token_endpoint}'
             oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope,
@@ -304,20 +301,19 @@
         Raises:
             PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists?$top={limit}')
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())['value']
-        lists = [TaskList(**list_data) for list_data in contents]
+        return [TaskList(**list_data) for list_data in contents]
 
-        return lists
 
     def create_list(self, name: str) -> TaskList:
         '''Create a new task list
 
         Args:
             name: Title of the new task list
 
@@ -327,15 +323,15 @@
         Raises:
             PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.post(f'{ToDoConnection._base_api_url}lists', json={'displayName': name})
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
     def get_list(self, list_id: str) -> TaskList:
         '''Read the properties of a task list
@@ -349,15 +345,15 @@
         Raises:
             PymstodoError: An error occurred accessing the API
         '''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists/{list_id}')
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
     def update_list(self, list_id: str, **list_data: Union[str, bool]) -> TaskList:
         '''Update the properties of a task list
@@ -371,15 +367,15 @@
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.patch(f'{ToDoConnection._base_api_url}lists/{list_id}', json=list_data)
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return TaskList(**contents)
 
     def delete_list(self, list_id: str) -> bool:
         '''Delete a task list
@@ -392,15 +388,15 @@
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.delete(f'{ToDoConnection._base_api_url}lists/{list_id}')
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         return True
 
     def get_tasks(self, list_id: str, limit: Optional[int] = 1000, status: Optional[TaskStatusFilter] = TaskStatusFilter.NOT_COMPLETED) -> List[Task]:
         '''Get tasks by a specified task list
 
         Args:
@@ -423,28 +419,27 @@
         }
         eff_limit = limit or 1000
         params = (
             filters.get(status or TaskStatusFilter.NOT_COMPLETED, filters[TaskStatusFilter.NOT_COMPLETED]),
             f'top={eff_limit}'
         )
         params_str = '&$'.join(filter(None, params))
-        url = f"{ToDoConnection._base_api_url}lists/{list_id}/tasks?${params_str}"
+        url = f'{ToDoConnection._base_api_url}lists/{list_id}/tasks?${params_str}'
         contents: List[Dict[str, Any]] = []
         while (len(contents) < eff_limit or eff_limit <= 0) and url:
             resp = oa_sess.get(url)
             if not resp.ok:
-                raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+                raise PymstodoError(resp.status_code, resp.reason)
             resp_content = json.loads(resp.content.decode())
             url = resp_content.get('@odata.nextLink')
             contents.extend(resp_content['value'])
         if limit:
             contents = contents[:limit]
-        tasks = [Task(**task_data) for task_data in contents]
+        return [Task(**task_data) for task_data in contents]
 
-        return tasks
 
     def create_task(self, title: str, list_id: str, due_date: Optional[datetime] = None, body_text: Optional[str] = None) -> Task:
         '''Create a new task in a specified task list
 
         Args:
             title: A brief description of the task
             list_id: Unique identifier for the task list
@@ -461,15 +456,15 @@
         task_data: Dict[str, Any] = {'title': title}
         if due_date:
             task_data['dueDateTime'] = {'dateTime': due_date.strftime('%Y-%m-%dT%H:%M:%S.0000000'), 'timeZone': 'UTC'}
         if body_text:
             task_data['body'] = {'content': body_text, 'contentType': 'text'}
         resp = oa_sess.post(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks', json=task_data)
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def get_task(self, task_id: str, list_id: str) -> Task:
         '''Read the properties of a task
@@ -483,15 +478,15 @@
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.get(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}')
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def update_task(self, task_id: str, list_id: str, **task_data: Union[str, int, bool]) -> Task:
         '''Update the properties of a task
@@ -506,15 +501,15 @@
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.patch(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}', json=task_data)
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         contents = json.loads(resp.content.decode())
 
         return Task(**contents)
 
     def delete_task(self, task_id: str, list_id: str) -> bool:
         '''Delete a task
@@ -528,15 +523,15 @@
 
         Raises:
             PymstodoError: An error occurred accessing the API'''
         self._refresh_token()
         oa_sess = OAuth2Session(self.client_id, scope=ToDoConnection._scope, token=self.token)
         resp = oa_sess.delete(f'{ToDoConnection._base_api_url}lists/{list_id}/tasks/{task_id}')
         if not resp.ok:
-            raise PymstodoError(f'Error {resp.status_code}: {resp.reason}')
+            raise PymstodoError(resp.status_code, resp.reason)
 
         return True
 
     def complete_task(self, task_id: str, list_id: str) -> Task:
         '''Complete a task
 
         Args:
```

### Comparing `pymstodo-0.1.4/pymstodo.egg-info/PKG-INFO` & `pymstodo-0.1.5/pymstodo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymstodo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Microsoft To Do API client
 Home-page: https://github.com/inbalboa/pymstodo
 Author: Sergey Shlyapugin
 Author-email: shlyapugin@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymstodo-0.1.4/setup.py` & `pymstodo-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
+from pathlib import Path
+
 import setuptools
 
 
 def long_description():
-    long_description = ''
-    with open('README.md', 'r') as ld:
-        long_description = ld.read()
-    return long_description
+    with Path('README.md').open() as ld:
+        return ld.read()
 
 def find_requires():
-    requirements = []
-    with open('requirements.txt', 'r') as reqs:
-        requirements = reqs.readlines()
-    return requirements
+    with Path('requirements.txt').open() as reqs:
+        return reqs.readlines()
 
 def find_version():
-    with open('VERSION', 'r') as ver:
-        version_ = ver.readline().strip()
-    return version_
+    with Path('VERSION').open() as ver:
+        return ver.readline().strip()
 
 
 setuptools.setup(
     name='pymstodo',
     version=find_version(),
     author='Sergey Shlyapugin',
     author_email='shlyapugin@gmail.com',
```

