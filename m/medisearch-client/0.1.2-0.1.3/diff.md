# Comparing `tmp/medisearch_client-0.1.2.tar.gz` & `tmp/medisearch_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.2.tar", last modified: Sun Aug  6 00:59:22 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.3.tar", last modified: Sun Aug  6 02:58:45 2023, max compression
```

## Comparing `medisearch_client-0.1.2.tar` & `medisearch_client-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:59:22.354884 medisearch_client-0.1.2/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 00:59:22.354752 medisearch_client-0.1.2/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     3066 2023-08-06 00:48:32.000000 medisearch_client-0.1.2/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:59:22.353750 medisearch_client-0.1.2/medisearch_client/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.2/medisearch_client/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     5075 2023-08-06 00:12:22.000000 medisearch_client-0.1.2/medisearch_client/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:59:22.354567 medisearch_client-0.1.2/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 00:59:22.000000 medisearch_client-0.1.2/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 00:59:22.000000 medisearch_client-0.1.2/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 00:59:22.000000 medisearch_client-0.1.2/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 00:59:22.000000 medisearch_client-0.1.2/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 00:59:22.000000 medisearch_client-0.1.2/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 00:59:22.354925 medisearch_client-0.1.2/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 00:59:02.000000 medisearch_client-0.1.2/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.834055 medisearch_client-0.1.3/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 02:58:45.833785 medisearch_client-0.1.3/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3066 2023-08-06 00:48:32.000000 medisearch_client-0.1.3/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.832063 medisearch_client-0.1.3/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.3/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4779 2023-08-06 02:57:12.000000 medisearch_client-0.1.3/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.833443 medisearch_client-0.1.3/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 02:58:45.834132 medisearch_client-0.1.3/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 02:57:27.000000 medisearch_client-0.1.3/setup.py
```

### Comparing `medisearch_client-0.1.2/PKG-INFO` & `medisearch_client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch_client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
```

### Comparing `medisearch_client-0.1.2/README.md` & `medisearch_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `medisearch_client-0.1.2/medisearch_client/client.py` & `medisearch_client-0.1.3/medisearch_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,16 +129,7 @@
         break
       data = json.loads(self.socket.recv())
       yield data
       if "event" in data and (data["event"] == "articles" or
                               data["event"] == "error"):
         break
     self.interrupted = True
-
-
-client = MediSearchClient(api_key="your_api_key")
-resps = client.send_user_message(conversation=["Stomach pain"],
-                                 conversation_id="123410312311231212315",
-                                 should_stream_response = True)
-
-for response in resps:
-  print(response)
```

### Comparing `medisearch_client-0.1.2/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.3/medisearch_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
```

### Comparing `medisearch_client-0.1.2/setup.py` & `medisearch_client-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "websocket-client",
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
     description="A simple client for the MediSearch API",
```

