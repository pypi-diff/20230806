# Comparing `tmp/medisearch_client-0.1.5.tar.gz` & `tmp/medisearch_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.5.tar", last modified: Sun Aug  6 03:19:51 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.7.tar", last modified: Sun Aug  6 04:13:00 2023, max compression
```

## Comparing `medisearch_client-0.1.5.tar` & `medisearch_client-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.240139 medisearch_client-0.1.5/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:19:51.240017 medisearch_client-0.1.5/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     3233 2023-08-06 03:06:58.000000 medisearch_client-0.1.5/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.239189 medisearch_client-0.1.5/medisearch_client/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.5/medisearch_client/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     4780 2023-08-06 03:18:15.000000 medisearch_client-0.1.5/medisearch_client/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.239858 medisearch_client-0.1.5/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 03:19:51.240174 medisearch_client-0.1.5/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 03:18:29.000000 medisearch_client-0.1.5/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.892015 medisearch_client-0.1.7/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4391 2023-08-06 04:13:00.891873 medisearch_client-0.1.7/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4117 2023-08-06 04:11:39.000000 medisearch_client-0.1.7/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.890994 medisearch_client-0.1.7/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.7/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4896 2023-08-06 04:08:57.000000 medisearch_client-0.1.7/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 04:13:00.891681 medisearch_client-0.1.7/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4391 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       50 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 04:13:00.000000 medisearch_client-0.1.7/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 04:13:00.892058 medisearch_client-0.1.7/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      597 2023-08-06 04:12:17.000000 medisearch_client-0.1.7/setup.py
```

### Comparing `medisearch_client-0.1.5/PKG-INFO` & `medisearch_client-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: medisearch_client
-Version: 0.1.5
-Summary: A simple client for the MediSearch API
-Home-page: https://github.com/MediSearch/medisearch_client_python
-Author: Michal Pandy
-Author-email: founders@medisearch.io
-Description-Content-Type: text/markdown
-
-
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
 ```bash
@@ -19,29 +9,29 @@
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
-  case if you do not already have one):
+case if you do not already have one):
 
 ```python
 from medisearch_client import MediSearchClient
 
 client = MediSearchClient(api_key="your_api_key")
 ```
 
 ### Sending User Messages and Making Follow-Up Queries
 
 To send a user message, first generate a unique conversation id (`your_conversation_id` below) for your conversation. Then, you may call the client as:
 
 ```python
 responses = client.send_user_message(
-    conversation=["Stomach pain"],
+    conversation=["By how much does sport increase life expectancy?"],
     conversation_id="your_conversation_id",
     should_stream_response=True
 )
 
 for response in responses:
     print(response)
 ```
@@ -63,15 +53,14 @@
 Always ensure the last message in the conversation is from the user.
 
 #### Streaming Option
 
 The `should_stream_response` flag controls how the client receives responses:
 
 - `True`: Stream the responses as they arrive. This is useful if you want to process each part of the response separately or if you want to display it to the user piece by piece.
-  
 - `False`: Wait until all parts of the response are collected and then return them as a list.
 
 ### Supported Languages
 
 MediSearch supports:
 
 - English
@@ -82,26 +71,73 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-#### Output structure
-The output of the call will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-d89474b50e6c4e4a80b2dcd2bdc8ed69) for a detailed description of all the events.
+
+### Interrupting generation
+
+You may interrupt the generation of the response by running:
+
+```python
+client.interrupt()
+```
+
+This is useful for implementing a 'stop-generate'-like button on your frontend.
+
+
+### Closing the connection
+
+To close the connection, simply run:
+
+```python
+client.close()
+```
+
+## Output structure
+
+In the following call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+`responses` will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-output-format-a4658341e38145669dac5c20aa6da279) for a detailed description of all the events.
 
 ## Error Handling
 
-MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
+If there is an error in the call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+then `responses` will contain an error event. This will be in the form of an element such as
+
+```
+{
+	event: "error",
+	error_code: "error_not_enough_articles",
+	id: "your_conversation_id"
+}
+```
+
+Some errors are part of how MediSearch API works. For example:
 
-- `error_auth`: Incorrect API key.
+- If we do not find enough relevant articles to a question, we will return `error_not_enough_articles`. For example, if the question is non-medical or does not make sense, MediSearch will throw this error.
+- If the conversation is too long, then we will return `error_out_of_tokens`. This happens rarely in practice. It can start happening if you ask MediSearch approximately 8 questions and get 8 responses in one conversation.
 
+Therefore, you should have at least some basic error handling mechanism to show your users a sensible message on your frontend when an error happens.
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
-  
-- `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
+Please see [our docs](https://mpmisko.notion.site/MediSearch-API-errors-format-396546e6a13d443a86243afa832bf1b2) for a detailed description of all the error events.
 
-For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
+If you ever think that there is a problem **do not hesitate to contact us: founders@medisearch.io.**
```

### Comparing `medisearch_client-0.1.5/README.md` & `medisearch_client-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: medisearch_client
+Version: 0.1.7
+Summary: A simple client for the MediSearch API
+Home-page: https://github.com/MediSearch/medisearch_client_python
+Author: Michal Pandy
+Author-email: founders@medisearch.io
+Description-Content-Type: text/markdown
 
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
@@ -10,29 +18,29 @@
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
-  case if you do not already have one):
+case if you do not already have one):
 
 ```python
 from medisearch_client import MediSearchClient
 
 client = MediSearchClient(api_key="your_api_key")
 ```
 
 ### Sending User Messages and Making Follow-Up Queries
 
 To send a user message, first generate a unique conversation id (`your_conversation_id` below) for your conversation. Then, you may call the client as:
 
 ```python
 responses = client.send_user_message(
-    conversation=["Stomach pain"],
+    conversation=["By how much does sport increase life expectancy?"],
     conversation_id="your_conversation_id",
     should_stream_response=True
 )
 
 for response in responses:
     print(response)
 ```
@@ -54,15 +62,14 @@
 Always ensure the last message in the conversation is from the user.
 
 #### Streaming Option
 
 The `should_stream_response` flag controls how the client receives responses:
 
 - `True`: Stream the responses as they arrive. This is useful if you want to process each part of the response separately or if you want to display it to the user piece by piece.
-  
 - `False`: Wait until all parts of the response are collected and then return them as a list.
 
 ### Supported Languages
 
 MediSearch supports:
 
 - English
@@ -73,26 +80,73 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-#### Output structure
-The output of the call will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-d89474b50e6c4e4a80b2dcd2bdc8ed69) for a detailed description of all the events.
+
+### Interrupting generation
+
+You may interrupt the generation of the response by running:
+
+```python
+client.interrupt()
+```
+
+This is useful for implementing a 'stop-generate'-like button on your frontend.
+
+
+### Closing the connection
+
+To close the connection, simply run:
+
+```python
+client.close()
+```
+
+## Output structure
+
+In the following call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+`responses` will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-output-format-a4658341e38145669dac5c20aa6da279) for a detailed description of all the events.
 
 ## Error Handling
 
-MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
+If there is an error in the call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+then `responses` will contain an error event. This will be in the form of an element such as
+
+```
+{
+	event: "error",
+	error_code: "error_not_enough_articles",
+	id: "your_conversation_id"
+}
+```
+
+Some errors are part of how MediSearch API works. For example:
 
-- `error_auth`: Incorrect API key.
+- If we do not find enough relevant articles to a question, we will return `error_not_enough_articles`. For example, if the question is non-medical or does not make sense, MediSearch will throw this error.
+- If the conversation is too long, then we will return `error_out_of_tokens`. This happens rarely in practice. It can start happening if you ask MediSearch approximately 8 questions and get 8 responses in one conversation.
 
+Therefore, you should have at least some basic error handling mechanism to show your users a sensible message on your frontend when an error happens.
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
-  
-- `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
+Please see [our docs](https://mpmisko.notion.site/MediSearch-API-errors-format-396546e6a13d443a86243afa832bf1b2) for a detailed description of all the error events.
 
-For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
+If you ever think that there is a problem **do not hesitate to contact us: founders@medisearch.io.**
```

### Comparing `medisearch_client-0.1.5/medisearch_client/client.py` & `medisearch_client-0.1.7/medisearch_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,13 +123,17 @@
 
   def _response_iterator(self):
     while True:
       if not self.socket.connected:
         self.reconnect()
       if self.interrupted:
         break
-      data = json.loads(self.socket.recv())
+      try:
+        data = json.loads(self.socket.recv())
+      except Exception as _:  # pylint: disable=broad-except
+        self.reconnect()
+        continue
       yield data
       if "event" in data and (data["event"] == "articles" or
                               data["event"] == "error"):
         break
     self.interrupted = False
```

### Comparing `medisearch_client-0.1.5/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.7/medisearch_client.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: medisearch-client
-Version: 0.1.5
+Version: 0.1.7
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
 
-
 # MediSearch API Client
 
 [MediSearch](https://medisearch.io/) API Client provides a Python interface for the MediSearch API. Easily send user messages and receive LLM responses, articles, and handle any errors that might arise.
 
 ## Installation
 
 ```bash
@@ -19,29 +18,29 @@
 ```
 
 ## Usage
 
 ### Initialization
 
 Initialize the client with your API key (email founders@medisearch.io with your use
-  case if you do not already have one):
+case if you do not already have one):
 
 ```python
 from medisearch_client import MediSearchClient
 
 client = MediSearchClient(api_key="your_api_key")
 ```
 
 ### Sending User Messages and Making Follow-Up Queries
 
 To send a user message, first generate a unique conversation id (`your_conversation_id` below) for your conversation. Then, you may call the client as:
 
 ```python
 responses = client.send_user_message(
-    conversation=["Stomach pain"],
+    conversation=["By how much does sport increase life expectancy?"],
     conversation_id="your_conversation_id",
     should_stream_response=True
 )
 
 for response in responses:
     print(response)
 ```
@@ -63,15 +62,14 @@
 Always ensure the last message in the conversation is from the user.
 
 #### Streaming Option
 
 The `should_stream_response` flag controls how the client receives responses:
 
 - `True`: Stream the responses as they arrive. This is useful if you want to process each part of the response separately or if you want to display it to the user piece by piece.
-  
 - `False`: Wait until all parts of the response are collected and then return them as a list.
 
 ### Supported Languages
 
 MediSearch supports:
 
 - English
@@ -82,26 +80,73 @@
 - Chinese
 - Japanese
 - Slovak
 - Arabic
 
 Set the `language` parameter in `send_user_message` accordingly.
 
-#### Output structure
-The output of the call will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-d89474b50e6c4e4a80b2dcd2bdc8ed69) for a detailed description of all the events.
+
+### Interrupting generation
+
+You may interrupt the generation of the response by running:
+
+```python
+client.interrupt()
+```
+
+This is useful for implementing a 'stop-generate'-like button on your frontend.
+
+
+### Closing the connection
+
+To close the connection, simply run:
+
+```python
+client.close()
+```
+
+## Output structure
+
+In the following call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+`responses` will be a list of MediSearch events. Please see [our docs](https://mpmisko.notion.site/MediSearch-API-documentation-output-format-a4658341e38145669dac5c20aa6da279) for a detailed description of all the events.
 
 ## Error Handling
 
-MediSearch API might occasionally return error events. Here are the common `error_code` values you might encounter:
+If there is an error in the call to our API
+
+```
+responses = client.send_user_message(
+    conversation=["By how much does sport increase life expectancy?"],
+    conversation_id="your_conversation_id",
+    should_stream_response=True
+)
+```
+
+then `responses` will contain an error event. This will be in the form of an element such as
+
+```
+{
+	event: "error",
+	error_code: "error_not_enough_articles",
+	id: "your_conversation_id"
+}
+```
+
+Some errors are part of how MediSearch API works. For example:
 
-- `error_auth`: Incorrect API key.
+- If we do not find enough relevant articles to a question, we will return `error_not_enough_articles`. For example, if the question is non-medical or does not make sense, MediSearch will throw this error.
+- If the conversation is too long, then we will return `error_out_of_tokens`. This happens rarely in practice. It can start happening if you ask MediSearch approximately 8 questions and get 8 responses in one conversation.
 
+Therefore, you should have at least some basic error handling mechanism to show your users a sensible message on your frontend when an error happens.
 
-- `error_internal`: An internal bug on MediSearch's end. If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_llm`: Issues with the Large Language Model (LLM). If persistent, consider contacting MediSearch support (email founders@medisearch.io).
-  
-- `error_not_enough_articles`: No relevant articles were found for the query. Might occur for non-medical or nonsensical queries. If you think we should have found relevant articles for a given query, please email founders@medisearch.io.
-  
-- `error_out_of_tokens`: The conversation's context became too lengthy. Typically occurs if the conversation consists of about 8 back-and-forths. Start a new conversation to resolve.
+Please see [our docs](https://mpmisko.notion.site/MediSearch-API-errors-format-396546e6a13d443a86243afa832bf1b2) for a detailed description of all the error events.
 
-For a deeper dive into the API's capabilities and events, refer to our [docs](https://mpmisko.notion.site/MediSearch-API-055d82267e06457cbf4e0be0cd628677).
+If you ever think that there is a problem **do not hesitate to contact us: founders@medisearch.io.**
```

### Comparing `medisearch_client-0.1.5/setup.py` & `medisearch_client-0.1.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1.5",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
-        "websocket-client",
+        "websocket-client", "pyasn1", "pyopenssl", "ndg-httpsclient"
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
     description="A simple client for the MediSearch API",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MediSearch/medisearch_client_python",
```

