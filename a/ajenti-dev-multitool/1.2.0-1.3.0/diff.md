# Comparing `tmp/ajenti-dev-multitool-1.2.0.tar.gz` & `tmp/ajenti-dev-multitool-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ajenti-dev-multitool-1.2.0.tar", last modified: Mon Mar 22 09:32:26 2021, max compression
+gzip compressed data, was "ajenti-dev-multitool-1.3.0.tar", last modified: Sun Aug  6 16:10:41 2023, max compression
```

## Comparing `ajenti-dev-multitool-1.2.0.tar` & `ajenti-dev-multitool-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2021-03-22 09:32:26.236852 ajenti-dev-multitool-1.2.0/
--rw-r--r--   0 eugene     (503) staff       (20)      231 2021-03-22 09:32:26.237028 ajenti-dev-multitool-1.2.0/PKG-INFO
--rwxr-xr-x   0 eugene     (503) staff       (20)    24519 2021-03-22 09:30:47.000000 ajenti-dev-multitool-1.2.0/ajenti-dev-multitool
-drwxr-xr-x   0 eugene     (503) staff       (20)        0 2021-03-22 09:32:26.236533 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/
--rw-r--r--   0 eugene     (503) staff       (20)      231 2021-03-22 09:32:26.000000 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (503) staff       (20)      258 2021-03-22 09:32:26.000000 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (503) staff       (20)        1 2021-03-22 09:32:26.000000 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (503) staff       (20)       26 2021-03-22 09:32:26.000000 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/requires.txt
--rw-r--r--   0 eugene     (503) staff       (20)        1 2021-03-22 09:32:26.000000 ajenti-dev-multitool-1.2.0/ajenti_dev_multitool.egg-info/top_level.txt
--rw-r--r--   0 eugene     (503) staff       (20)       67 2021-03-22 09:32:26.237897 ajenti-dev-multitool-1.2.0/setup.cfg
--rwxr-xr-x   0 eugene     (503) staff       (20)      383 2021-03-22 09:31:20.000000 ajenti-dev-multitool-1.2.0/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-08-06 16:10:41.497173 ajenti-dev-multitool-1.3.0/
+-rw-r--r--   0 eugene     (501) staff       (20)      175 2023-08-06 16:10:41.497231 ajenti-dev-multitool-1.3.0/PKG-INFO
+-rwxr-xr-x   0 eugene     (501) staff       (20)    27305 2023-08-06 16:10:30.000000 ajenti-dev-multitool-1.3.0/ajenti-dev-multitool
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-08-06 16:10:41.497011 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      175 2023-08-06 16:10:41.000000 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      258 2023-08-06 16:10:41.000000 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-08-06 16:10:41.000000 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       26 2023-08-06 16:10:41.000000 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-08-06 16:10:41.000000 ajenti-dev-multitool-1.3.0/ajenti_dev_multitool.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       67 2023-08-06 16:10:41.497434 ajenti-dev-multitool-1.3.0/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)      383 2023-08-06 16:10:39.000000 ajenti-dev-multitool-1.3.0/setup.py
```

### Comparing `ajenti-dev-multitool-1.2.0/ajenti-dev-multitool` & `ajenti-dev-multitool-1.3.0/ajenti-dev-multitool`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import os
 import re
 import shutil
 import sys
 import tempfile
 import time
 import yaml
-from gevent import subprocess
+import requests
+from gevent import subprocess, sleep
+
+CROWDIN_API_BASEURL = "https://api.crowdin.com/api/v2"
 
 # Ignore ajenti specific python objects
 yaml.add_multi_constructor('tag:yaml.org,2002:python/object:', lambda a, b, c: None)
 
 for dep in ['Plugin', 'Binary', 'OptionalPlugin', 'File', 'Module']:
     yaml.add_constructor(f'!{dep}Dependency', lambda a, b: None, Loader=yaml.SafeLoader)
 
@@ -391,79 +394,142 @@
                     '-U',
                     po_path, pot_path,
                 ])
             else:
                 with open(po_path, 'w') as f:
                     f.write(open(pot_path).read())
 
+def _get_crowdin_projectid(project_identifier, headers):
+    resp = json.loads(requests.get(f"{CROWDIN_API_BASEURL}/projects", headers=headers).content)
+
+    for project in resp['data']:
+        if project['data']['identifier'] == project_identifier:
+            return project['data']['id']
+    return None
+
+def _get_crowdin_fileId(project_id, headers):
+    filesId = {}
+    resp = requests.get(f"{CROWDIN_API_BASEURL}/projects/{project_id}/files?limit=100", headers=headers)
+    for f in json.loads(resp.content)['data']:
+        # Only managing files under the directory 2.0
+        if f['data']['path'].startswith('/2.0/'):
+            filesId[f['data']['name']] = f['data']['id']
+    return filesId
+
+def _get_crowdin_token():
+    try:
+        crowdin_token = open('.crowdin.token').read().strip().split('\n')
+        if len(crowdin_token) == 2:
+            project_identifier = crowdin_token[1]
+        else:
+            project_identifier = 'ajenti'
+        return crowdin_token[0], project_identifier
+    except Exception as e:
+        logging.error(f'Could not read ".crowdin.token": {e}')
+        sys.exit(1)
 
 def run_push_crowdin(plugins, add=False):
     dir = tempfile.mkdtemp()
-    logging.info('Working in %s' % dir)
+    logging.info(f'Working in {dir}')
+
+    # Generating .po files
     for plugin in plugins:
         locale_path = os.path.join(plugin, 'locale')
         pot_path = os.path.join(locale_path, 'app.pot')
         if os.path.exists(pot_path):
             logging.info('Copying %s', pot_path)
             with open(os.path.join(dir, os.path.split(plugin)[1] + '.po'), 'w') as f:
                 f.write(open(pot_path).read())
 
-    try:
-        crowdin_key = open('.crowdin.key').read().strip().split('\n')
-        if len(crowdin_key) == 2:
-            project_name = crowdin_key[1]
-        else:
-            project_name = 'ajenti'
-        key = crowdin_key[0]
-    except Exception as e:
-        logging.error('Could not read ".crowdin.key": %s', e)
-        sys.exit(1)
+    token, project_identifier = _get_crowdin_token()
+    headers = {
+        'Authorization': f'Bearer {token}',
+        'Content-Type': 'application/json'
+    }
 
+    projectId = _get_crowdin_projectid(project_identifier, headers)
+    if projectId is None:
+        logging.error("Project id not found")
+        return
+
+    # Dict like {'filename': id}
+    filesId = _get_crowdin_fileId(projectId, headers)
+
+    # Uploading
     for file in os.listdir(dir):
-        logging.info(' :: uploading %s' % file)
-        subprocess.check_call([
-            'curl', '-F', 'files[/2.0/%s]=@%s' % (
-                file,
-                os.path.join(dir, file),
-            ),
-            'https://api.crowdin.com/api/project/%s/%s?key=%s' % (
-                project_name,
-                'add-file' if add else 'update-file',
-                key
-            )
-        ])
+        logging.info(f' :: uploading {file}')
+
+        # First need to create a storage through the API
+        headers['Content-Type'] = 'application/text-plain'
+        headers['Crowdin-API-FileName'] = f'storage-{file}'
+
+        with open(os.path.join(dir, file), 'r') as f:
+            content = f.read()
+
+        resp = requests.post(f"{CROWDIN_API_BASEURL}/storages", data=content, headers=headers)
+        # We need the storage ID for later
+        storageId = json.loads(resp.content)['data']['id']
+
+        # Finally update file with the content of the storage
+        headers['Content-Type'] = 'application/json'
+        fileId = filesId.get(file, None)
+        if fileId:
+            data = json.dumps({'storageId': storageId, 'updateOption':"keep_translations_and_approvals"})
+            logging.debug(f"Updating file {file} on Crowdin")
+            requests.put(f"{CROWDIN_API_BASEURL}/projects/{projectId}/files/{fileId}", data= data, headers=headers)
+        else:
+            logging.warning(f"Could not find file {file} on Crowdin")
+            if add:
+                logging.debug(f"Uploading new file {file} to Crowdin")
+                data = json.dumps({'name': file, 'storageId': storageId, 'directoryId': 92})
+                requests.post(f"{CROWDIN_API_BASEURL}/projects/{projectId}/files", data= data, headers=headers)
 
     shutil.rmtree(dir)
 
 
 def run_pull_crowdin(plugins):
-    try:
-        crowdin_key = open('.crowdin.key').read().strip().split('\n')
-        if len(crowdin_key) == 2:
-            project_name = crowdin_key[1]
-        else:
-            project_name = 'ajenti'
-        key = crowdin_key[0]
-    except Exception as e:
-        logging.error('Could not read ".crowdin.key": %s', e)
-        sys.exit(1)
+
+    token, project_identifier = _get_crowdin_token()
 
     map = dict((os.path.split(p)[1], p) for p in plugins)
     dir = tempfile.mkdtemp()
     logging.info('Working in %s' % dir)
 
     logging.info('Requesting build')
-    subprocess.check_call([
-        'curl', 'https://api.crowdin.com/api/project/%s/export?key=%s' % (project_name, key)
-    ])
+
+    headers = {'Authorization': f'Bearer {token}', 'Content-Type': 'application/json'}
+
+    projectId = _get_crowdin_projectid(project_identifier, headers)
+    if projectId is None:
+        logging.error("Project id not found")
+        return
+
+    resp = requests.post(f"{CROWDIN_API_BASEURL}/projects/{projectId}/translations/builds", data='{}', headers=headers)
+    content = json.loads(resp.content)
+
+    if 200 <= resp.status_code < 300:
+        buildId = content['data']['id']
+    else:
+        logging.error(content['error']['message'])
+
+    progress = 0
+    while progress < 100:
+        sleep(2)
+        resp = json.loads(requests.get(f"{CROWDIN_API_BASEURL}/projects/{projectId}/translations/builds/{buildId}", headers=headers).content)
+        progress = resp['data']['progress']
+        logging.info(f"Build processing {progress}%")
 
     logging.info('Downloading')
+
+    resp = requests.get(f"{CROWDIN_API_BASEURL}/projects/{projectId}/translations/builds/{buildId}/download", headers=headers)
+    download_url = json.loads(resp.content)['data']['url']
+
     zip_path = os.path.join(dir, 'all.zip')
     subprocess.check_call([
-        'wget', 'https://api.crowdin.com/api/project/%s/download/all.zip?key=%s' % (project_name, key),
+        'wget', download_url,
         '-O', zip_path
     ])
 
     subprocess.check_call([
         'unzip', 'all.zip'
     ], cwd=dir)
```

