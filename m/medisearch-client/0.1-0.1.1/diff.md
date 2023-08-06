# Comparing `tmp/medisearch_client-0.1.tar.gz` & `tmp/medisearch_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.tar", last modified: Sun Aug  6 00:33:21 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.1.tar", last modified: Sun Aug  6 00:49:48 2023, max compression
```

## Comparing `medisearch_client-0.1.tar` & `medisearch_client-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:33:21.415630 medisearch_client-0.1/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3352 2023-08-06 00:33:21.415505 medisearch_client-0.1/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     3070 2023-08-06 00:32:06.000000 medisearch_client-0.1/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:33:21.414670 medisearch_client-0.1/medisearch/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1/medisearch/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     5075 2023-08-06 00:12:22.000000 medisearch_client-0.1/medisearch/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:33:21.415335 medisearch_client-0.1/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3352 2023-08-06 00:33:21.000000 medisearch_client-0.1/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      266 2023-08-06 00:33:21.000000 medisearch_client-0.1/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 00:33:21.000000 medisearch_client-0.1/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 00:33:21.000000 medisearch_client-0.1/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       11 2023-08-06 00:33:21.000000 medisearch_client-0.1/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 00:33:21.415669 medisearch_client-0.1/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      563 2023-08-05 22:20:32.000000 medisearch_client-0.1/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:49:48.638249 medisearch_client-0.1.1/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 00:49:48.638115 medisearch_client-0.1.1/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3066 2023-08-06 00:48:32.000000 medisearch_client-0.1.1/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:49:48.637282 medisearch_client-0.1.1/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.1/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     5075 2023-08-06 00:12:22.000000 medisearch_client-0.1.1/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 00:49:48.637956 medisearch_client-0.1.1/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 00:49:48.000000 medisearch_client-0.1.1/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 00:49:48.000000 medisearch_client-0.1.1/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 00:49:48.000000 medisearch_client-0.1.1/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 00:49:48.000000 medisearch_client-0.1.1/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 00:49:48.000000 medisearch_client-0.1.1/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 00:49:48.638284 medisearch_client-0.1.1/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 00:49:19.000000 medisearch_client-0.1.1/setup.py
```

### Comparing `medisearch_client-0.1/PKG-INFO` & `medisearch_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: medisearch_client
-Version: 0.1
-Summary: A simple WebSocket client for the MediSearch API
+Version: 0.1.1
+Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
 ```bash
-pip install medisearch-api-client
+pip install medisearch_client
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
```

### Comparing `medisearch_client-0.1/README.md` & `medisearch_client-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
 ```bash
-pip install medisearch-api-client
+pip install medisearch_client
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
```

### Comparing `medisearch_client-0.1/medisearch/client.py` & `medisearch_client-0.1.1/medisearch_client/client.py`

 * *Files identical despite different names*

### Comparing `medisearch_client-0.1/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.1/medisearch_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: medisearch-client
-Version: 0.1
-Summary: A simple WebSocket client for the MediSearch API
+Version: 0.1.1
+Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
 ```bash
-pip install medisearch-api-client
+pip install medisearch_client
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
```

### Comparing `medisearch_client-0.1/setup.py` & `medisearch_client-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
-        'websocket-client',
+        "websocket-client",
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
-    description="A simple WebSocket client for the MediSearch API",
+    description="A simple client for the MediSearch API",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MediSearch/medisearch_client_python",
-)
+)
```

