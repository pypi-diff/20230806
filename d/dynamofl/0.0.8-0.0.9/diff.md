# Comparing `tmp/dynamofl-0.0.8.tar.gz` & `tmp/dynamofl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamofl-0.0.8.tar", last modified: Mon Feb 14 05:49:10 2022, max compression
+gzip compressed data, was "dynamofl-0.0.9.tar", last modified: Tue Apr 12 20:51:49 2022, max compression
```

## Comparing `dynamofl-0.0.8.tar` & `dynamofl-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-02-14 05:49:10.086339 dynamofl-0.0.8/
--rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-02-14 05:49:10.091027 dynamofl-0.0.8/PKG-INFO
-drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-02-14 05:49:10.084224 dynamofl-0.0.8/dynamofl/
--rw-r--r--   0 emileindik   (501) staff       (20)       74 2022-02-09 01:14:10.000000 dynamofl-0.0.8/dynamofl/__init__.py
--rw-r--r--   0 emileindik   (501) staff       (20)     8148 2022-02-14 05:46:20.000000 dynamofl-0.0.8/dynamofl/src.py
-drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-02-14 05:49:10.086151 dynamofl-0.0.8/dynamofl.egg-info/
--rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-02-14 05:49:09.000000 dynamofl-0.0.8/dynamofl.egg-info/PKG-INFO
--rw-r--r--   0 emileindik   (501) staff       (20)      220 2022-02-14 05:49:10.000000 dynamofl-0.0.8/dynamofl.egg-info/SOURCES.txt
--rw-r--r--   0 emileindik   (501) staff       (20)        1 2022-02-14 05:49:09.000000 dynamofl-0.0.8/dynamofl.egg-info/dependency_links.txt
--rw-r--r--   0 emileindik   (501) staff       (20)       17 2022-02-14 05:49:10.000000 dynamofl-0.0.8/dynamofl.egg-info/requires.txt
--rw-r--r--   0 emileindik   (501) staff       (20)        9 2022-02-14 05:49:10.000000 dynamofl-0.0.8/dynamofl.egg-info/top_level.txt
--rw-r--r--   0 emileindik   (501) staff       (20)      104 2021-10-23 03:06:00.000000 dynamofl-0.0.8/pyproject.toml
--rw-r--r--   0 emileindik   (501) staff       (20)      221 2022-02-14 05:49:10.091530 dynamofl-0.0.8/setup.cfg
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.534735 dynamofl-0.0.9/
+-rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-04-12 20:51:49.534924 dynamofl-0.0.9/PKG-INFO
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.526846 dynamofl-0.0.9/dynamofl/
+-rw-r--r--   0 emileindik   (501) staff       (20)       25 2022-04-12 20:48:47.000000 dynamofl-0.0.9/dynamofl/__init__.py
+-rw-r--r--   0 emileindik   (501) staff       (20)     8988 2022-04-12 20:48:38.000000 dynamofl-0.0.9/dynamofl/src.py
+drwxr-xr-x   0 emileindik   (501) staff       (20)        0 2022-04-12 20:51:49.534355 dynamofl-0.0.9/dynamofl.egg-info/
+-rw-r--r--   0 emileindik   (501) staff       (20)      157 2022-04-12 20:51:48.000000 dynamofl-0.0.9/dynamofl.egg-info/PKG-INFO
+-rw-r--r--   0 emileindik   (501) staff       (20)      220 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/SOURCES.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)        1 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/dependency_links.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)       41 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/requires.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)        9 2022-04-12 20:51:49.000000 dynamofl-0.0.9/dynamofl.egg-info/top_level.txt
+-rw-r--r--   0 emileindik   (501) staff       (20)      104 2021-10-23 03:06:00.000000 dynamofl-0.0.9/pyproject.toml
+-rw-r--r--   0 emileindik   (501) staff       (20)      247 2022-04-12 20:51:49.535678 dynamofl-0.0.9/setup.cfg
```

### Comparing `dynamofl-0.0.8/dynamofl/src.py` & `dynamofl-0.0.9/dynamofl/src.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,37 @@
+from gevent import monkey; monkey.patch_all()
 import os
 import pathlib
 import json
-from time import sleep
+import threading
 
 import requests
+from websocket import create_connection
+import gevent
 
-
-WAIT_SECONDS = 3
 API_VERSION = 'v1'
 
 def _check_for_error(r):
     if not r.ok:
         print(json.dumps(json.loads(r.text), indent=4))
     r.raise_for_status()
 
 
-class Base:
-    def __init__(self):
-        self.token = ''
-        self.host = ''
-
-    def init(self, token, host='https://api.dynamofl.com'):
-        self.host = host
+class _Base:
+    def __init__(self, token, host):
         self.token = token
+        self.host = host
 
     def _get_route(self):
         return f'{self.host}/{API_VERSION}'
 
     def _get_headers(self):
         return {'Authorization': f'Bearer {self.token}'}
 
-    def make_request(self, method, url, params=None, files=None, list=False):
+    def _make_request(self, method, url, params=None, files=None, list=False):
         if method == 'POST':
             r = requests.post(
                 f'{self._get_route()}{url}',
                 headers=self._get_headers(),
                 json=params,
                 files=files
             )
@@ -56,143 +53,123 @@
             if list:
                 return r.json()['data']
             else:
                 return r.json()
 
 
 
-class _Project(Base):
-    def __init__(self, host, token, key):
-        super().__init__()
-        self.init(token, host)
+class _Project(_Base):
+    def __init__(self, token, host, key, ws):
+        super().__init__(token, host)
         self.key = key
-    
+        self.ws = ws
+
     def get_info(self):
-        return self.make_request('GET', f'/projects/{self.key}')
+        return self._make_request('GET', f'/projects/{self.key}')
 
     def update_rounds(self, rounds):
-        return self.make_request('POST', f'/projects/{self.key}', params={'rounds': rounds})
+        return self._make_request('POST', f'/projects/{self.key}', params={'rounds': rounds})
 
     def update_schedule(self, schedule):
-        return self.make_request('POST', f'/projects/{self.key}', params={'schedule': schedule})
+        return self._make_request('POST', f'/projects/{self.key}', params={'schedule': schedule})
 
     def update_paused(self, paused):
-        return self.make_request('POST', f'/projects/{self.key}', params={'paused': paused})
+        return self._make_request('POST', f'/projects/{self.key}', params={'paused': paused})
 
     def update_auto_increment(self, auto_increment):
-        return self.make_request('POST', f'/projects/{self.key}', params={'autoIncrement': auto_increment})
+        return self._make_request('POST', f'/projects/{self.key}', params={'autoIncrement': auto_increment})
 
     def update_optimizer_params(self, optimizer_params):
-        return self.make_request('POST', f'/projects/{self.key}', params={'optimizerParams': optimizer_params})
+        return self._make_request('POST', f'/projects/{self.key}', params={'optimizerParams': optimizer_params})
 
     def delete_project(self):
-        return self.make_request('DELETE', f'/projects/{self.key}')
+        return self._make_request('DELETE', f'/projects/{self.key}')
 
     def add_contributor(self, email, role='member'):
-        return self.make_request('POST', f'/projects/{self.key}/contributors', params={'email': email, 'role': role})
+        return self._make_request('POST', f'/projects/{self.key}/contributors', params={'email': email, 'role': role})
 
     def delete_contributor(self, email):
-        return self.make_request('DELETE', f'/projects/{self.key}/contributors', params={'email': email})
+        return self._make_request('DELETE', f'/projects/{self.key}/contributors', params={'email': email})
 
     def get_next_schedule(self):
-        return self.make_request('GET', f'/projects/{self.key}/schedule')
+        return self._make_request('GET', f'/projects/{self.key}/schedule')
 
     def increment_round(self):
-        return self.make_request('POST', f'/projects/{self.key}/increment')
+        return self._make_request('POST', f'/projects/{self.key}/increment')
 
     def create_datalink(self, datalink_key, description=None):
         params = {'key': datalink_key}
         if description:
             params['description'] = description
-        return self.make_request('POST', f'/projects/{self.key}/datalinks', params=params)
+        return self._make_request('POST', f'/projects/{self.key}/datalinks', params=params)
 
     def get_datalinks(self):
-        return self.make_request('GET', f'/projects/{self.key}/datalinks', list=True)
+        return self._make_request('GET', f'/projects/{self.key}/datalinks', list=True)
 
     def get_datalink(self, datalink_key):
-        return self.make_request('GET', f'/projects/{self.key}/datalinks/{datalink_key}')
+        return self._make_request('GET', f'/projects/{self.key}/datalinks/{datalink_key}')
 
     def delete_datalink(self, datalink_key):
-        return self.make_request('DELETE', f'/projects/{self.key}/datalinks/{datalink_key}')
+        return self._make_request('DELETE', f'/projects/{self.key}/datalinks/{datalink_key}')
 
     def get_rounds(self):
-        return self.make_request('GET', f'/projects/{self.key}/rounds', list=True)
+        return self._make_request('GET', f'/projects/{self.key}/rounds', list=True)
 
     def get_round(self, round):
-        return self.make_request('GET', f'/projects/{self.key}/rounds/{round}')
+        return self._make_request('GET', f'/projects/{self.key}/rounds/{round}')
 
     def get_stats(self, round=None, datalink_key=None):
         params = {}
         if round is not None:
             params['round'] = round
         if datalink_key is not None:
             params['datalink'] = datalink_key
-        return self.make_request('GET', f'/projects/{self.key}/stats', params, list=True)
+        return self._make_request('GET', f'/projects/{self.key}/stats', params, list=True)
 
     def get_stats_avg(self):
-        return self.make_request('GET', f'/projects/{self.key}/stats/avg')
+        return self._make_request('GET', f'/projects/{self.key}/stats/avg')
 
-    def get_submissions(self, datalink_key=None, round=None):
+    def get_submissions(self, datalink_key=None, round=None, owned=None):
         params = {}
         if round is not None:
             params['round'] = round
         if datalink_key is not None:
             params['datalink'] = datalink_key
-        return self.make_request('GET', f'/projects/{self.key}/submissions', params, list=True)
-
-    def wait_for_round_to_end(self, round, throw_on_federation_error=False):
-        federation_error = None
-        while True:
-            j = self.make_request('GET', f'/projects/{self.key}/rounds/{round}')
-
-            if j and j['federationError']:
-                if throw_on_federation_error:
-                    raise Exception(j)
-                if federation_error != j['federationError']:
-                    federation_error = j['federationError']
-                    print('Federation error occured:\n  ' + federation_error)
-            if j and j['endTime']:
-                return
-            sleep(WAIT_SECONDS)
+        if owned is not None:
+            params['owned'] = owned
+        return self._make_request('GET', f'/projects/{self.key}/submissions', params, list=True)
 
     def upload_optimizer(self, path):
         with open(path, 'rb') as f:
-            self.make_request('POST', f'/projects/{self.key}/optimizers', files={'optimizer': f})
-
-
-
+            self._make_request('POST', f'/projects/{self.key}/optimizers', files={'optimizer': f})
 
     def report_stats(self, scores, num_samples, round, datalink_key):
-        return self.make_request('POST', f'/projects/{self.key}/stats', params={
+        return self._make_request('POST', f'/projects/{self.key}/stats', params={
             'round': round,
             'scores': scores,
             'numPoints': num_samples,
             'datalink': datalink_key
         })
 
     def push_model(self, path, datalink_key, params=None):
         if params is not None:
-            self.make_request('POST', f'/projects/{self.key}/models/{datalink_key}/params', params=params)
+            self._make_request('POST', f'/projects/{self.key}/models/{datalink_key}/params', params=params)
 
         if datalink_key is None:
             url = f'/projects/{self.key}/models'
         else:
             url = f'/projects/{self.key}/models/{datalink_key}'
         with open(path, 'rb') as f:
-            self.make_request('POST', url, files={'modelfile': f})
+            self._make_request('POST', url, files={'modelfile': f})
 
     def pull_model(self, filepath, datalink_key=None, round=None, throw_error=False):
         params = {}
         if round is not None:
             params['round'] = round
 
-        if round is not None and datalink_key is None:
-            self.wait_for_round_to_end(round, throw_on_federation_error=throw_error)
-
-
         if datalink_key is None:
             url = f'{self._get_route()}/projects/{self.key}/models'
         else:
             url = f'{self._get_route()}/projects/{self.key}/models/{datalink_key}'
         r = requests.get(url, headers=self._get_headers(), params=params)
         _check_for_error(r)
 
@@ -200,45 +177,72 @@
         pathlib.Path(directory).mkdir(parents=True, exist_ok=True) 
 
         with open(filepath, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192): 
                 f.write(chunk)
 
 
-class _Client(Base):
-    def __init__(self):
-        super().__init__()
-
-    def _check_init(self):
-        if not self.host or not self.token:
-            raise ValueError('Must call init() first, passing in API key.')
+class DynamoFL(_Base):
+    def __init__(self, token, host='https://api.dynamofl.com'):
+        super().__init__(token, host)
+
+        self.wshost = self.host.replace('http', 'ws', 1)
+        self.project_callbacks = {}
+        self.on_round_threads = {}
+
+        self.ws = create_connection(self.wshost)
+        self.ws.send('{ "action": "auth", "token": "' + self.token + '" }')
+
+        t = threading.Thread(target=self._gevent_ws_loop)
+        t.setDaemon(False)
+        t.start()
+
+    def _gevent_ws_loop(self):
+        while True:
+            res = self.ws.recv()
+            j = json.loads(res)
+            if 'data' in j and 'project' in j['data'] and 'key' in j['data']['project']:
+                project_key = j['data']['project']['key']
+            if j['event'] == 'project-complete':
+                if project_key in self.on_round_threads:
+                    self.on_round_threads[project_key].kill()
+                    del self.project_callbacks[project_key]
+                    if not len(self.project_callbacks.keys()):
+                        return
+            if j['event'] == 'round-complete':
+                if project_key in self.on_round_threads:
+                    self.on_round_threads[project_key].kill()
+                if project_key in self.project_callbacks:
+                    callback = self.project_callbacks[project_key]
+                    self.on_round_threads[project_key] = gevent.spawn(callback, j['data']['project'])
+            if j['event'] == 'round-error':
+                if project_key in self.on_round_threads:
+                    print('Federation error occured:\n  ' + j['data']['errorMessage'])
+
+    def on_new_round(self, project_key, callback):
+        info = self._make_request('GET', f'/projects/{project_key}')
+        # if info['isComplete']:
+        #     g.join()
+        #     return
+        self.project_callbacks[project_key] = callback
+        self.on_round_threads[project_key] = gevent.spawn(callback, info)
 
     def get_user(self):
-        return self.make_request('GET', f'/user')
+        return self._make_request('GET', f'/user')
 
     def create_project(self, base_model_path, params):
-        self._check_init()
-
-        j = self.make_request('POST', '/projects', params=params)
+        j = self._make_request('POST', '/projects', params=params)
 
-        project = _Project(self.host, self.token, j['key'])
+        project = _Project(self.token, self.host, j['key'], self.ws)
         project.push_model(base_model_path, None)
 
         return project
 
     def get_project(self, project_key):
-        self._check_init()
-        j = self.make_request('GET', f'/projects/{project_key}')
-        return _Project(self.host, self.token, j['key'])
+        j = self._make_request('GET', f'/projects/{project_key}')
+        return _Project(self.token, self.host, j['key'], self.ws)
 
     def get_projects(self):
-        self._check_init()
-        return self.make_request('GET', f'/projects', list=True)
+        return self._make_request('GET', f'/projects', list=True)
 
 
-client = _Client()
 
-init = client.init
-get_user = client.get_user
-create_project = client.create_project
-get_project = client.get_project
-get_projects = client.get_projects
```

