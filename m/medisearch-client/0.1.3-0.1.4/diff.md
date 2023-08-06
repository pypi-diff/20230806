# Comparing `tmp/medisearch_client-0.1.3.tar.gz` & `tmp/medisearch_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.3.tar", last modified: Sun Aug  6 02:58:45 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.4.tar", last modified: Sun Aug  6 03:08:14 2023, max compression
```

## Comparing `medisearch_client-0.1.3.tar` & `medisearch_client-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.834055 medisearch_client-0.1.3/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 02:58:45.833785 medisearch_client-0.1.3/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     3066 2023-08-06 00:48:32.000000 medisearch_client-0.1.3/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.832063 medisearch_client-0.1.3/medisearch_client/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.3/medisearch_client/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     4779 2023-08-06 02:57:12.000000 medisearch_client-0.1.3/medisearch_client/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 02:58:45.833443 medisearch_client-0.1.3/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3340 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 02:58:45.000000 medisearch_client-0.1.3/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 02:58:45.834132 medisearch_client-0.1.3/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 02:57:27.000000 medisearch_client-0.1.3/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.367505 medisearch_client-0.1.4/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:08:14.367358 medisearch_client-0.1.4/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3233 2023-08-06 03:06:58.000000 medisearch_client-0.1.4/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.366499 medisearch_client-0.1.4/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.4/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4779 2023-08-06 02:57:12.000000 medisearch_client-0.1.4/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.367176 medisearch_client-0.1.4/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 03:08:14.367543 medisearch_client-0.1.4/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 03:07:54.000000 medisearch_client-0.1.4/setup.py
```

### Comparing `medisearch_client-0.1.3/PKG-INFO` & `medisearch_client-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 
@@ -92,16 +92,16 @@
 ## Error Handling
 
 MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
 
 - `error_auth`: Incorrect API key.
 
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support.
+- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_llm`: Issues with the Language Learning Model (LLM). If persistent, consider contacting MediSearch support.
+- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries.
+- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
   
 - `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
 
 For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
```

### Comparing `medisearch_client-0.1.3/README.md` & `medisearch_client-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 ## Error Handling
 
 MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
 
 - `error_auth`: Incorrect API key.
 
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support.
+- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_llm`: Issues with the Language Learning Model (LLM). If persistent, consider contacting MediSearch support.
+- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries.
+- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
   
 - `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
 
 For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
```

### Comparing `medisearch_client-0.1.3/medisearch_client/client.py` & `medisearch_client-0.1.4/medisearch_client/client.py`

 * *Files identical despite different names*

### Comparing `medisearch_client-0.1.3/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.4/medisearch_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
 
@@ -92,16 +92,16 @@
 ## Error Handling
 
 MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
 
 - `error_auth`: Incorrect API key.
 
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support.
+- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_llm`: Issues with the Language Learning Model (LLM). If persistent, consider contacting MediSearch support.
+- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
   
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries.
+- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
   
 - `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
 
 For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
```

### Comparing `medisearch_client-0.1.3/setup.py` & `medisearch_client-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         "websocket-client",
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
     description="A simple client for the MediSearch API",
```

