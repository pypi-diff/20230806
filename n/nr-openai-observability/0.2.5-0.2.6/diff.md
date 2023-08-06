# Comparing `tmp/nr_openai_observability-0.2.5.tar.gz` & `tmp/nr_openai_observability-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr_openai_observability-0.2.5.tar", max compression
+gzip compressed data, was "nr_openai_observability-0.2.6.tar", max compression
```

## Comparing `nr_openai_observability-0.2.5.tar` & `nr_openai_observability-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/LICENSE
--rw-r--r--   0        0        0     4227 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/README.md
--rw-r--r--   0        0        0      687 2023-05-09 07:47:11.122630 nr_openai_observability-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/src/nr_openai_observability/__init__.py
--rw-r--r--   0        0        0     5257 2023-05-09 07:46:55.066403 nr_openai_observability-0.2.5/src/nr_openai_observability/monitor.py
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 nr_openai_observability-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4454 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/README.md
+-rw-r--r--   0        0        0      687 2023-08-06 11:21:43.384739 nr_openai_observability-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/src/nr_openai_observability/__init__.py
+-rw-r--r--   0        0        0     5309 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/src/nr_openai_observability/build_events.py
+-rw-r--r--   0        0        0      355 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/src/nr_openai_observability/error_handling_decorator.py
+-rw-r--r--   0        0        0    12629 2023-08-06 11:21:23.675252 nr_openai_observability-0.2.6/src/nr_openai_observability/monitor.py
+-rw-r--r--   0        0        0     5269 1970-01-01 00:00:00.000000 nr_openai_observability-0.2.6/PKG-INFO
```

### Comparing `nr_openai_observability-0.2.5/LICENSE` & `nr_openai_observability-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nr_openai_observability-0.2.5/README.md` & `nr_openai_observability-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,35 +35,43 @@
 
 * Are you reporting data to the New Relic EU region? click [here](#eu-account-users) for more instructions.
 
 #### STEP 2: Add the following two lines to your code
 
 ```python
 from nr_openai_observability import monitor
-monitor.initialization()
+monitor.initialization(
+    application_name="OpenAI observability example"
+)
 ```
 
 #### Code example:
 
 ```python
 
 import os
 
 import openai
 from nr_openai_observability import monitor
 
-monitor.initialization()
+monitor.initialization(
+    application_name="OpenAI observability example"
+)
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
-openai.Completion.create(
-    model="text-davinci-003",
-    prompt="What is Observability?",
-    max_tokens=20,
-    temperature=0 
+response = openai.ChatCompletion.create(
+    model="gpt-3.5-turbo",
+    messages=[
+        {
+            "role": "user",
+            "content": "Write a rhythm about observability",
+        },
+    ],
 )
+print(response["choices"][0]["message"]["content"])
 ```
 
 #### STEP 3: Follow the instruction [here](https://one.newrelic.com/launcher/catalog-pack-details.launcher/?pane=eyJuZXJkbGV0SWQiOiJjYXRhbG9nLXBhY2stZGV0YWlscy5jYXRhbG9nLXBhY2stY29udGVudHMiLCJxdWlja3N0YXJ0SWQiOiI1ZGIyNWRiZC1hNmU5LTQ2ZmMtYTcyOC00Njk3ZjY3N2ZiYzYifQ==) to add the dashboard to your New Relic account.
 
 ### EU Account Users:
 
 If you are using an EU region account, you should also set your `EVENT_CLIENT_HOST`:
```

### Comparing `nr_openai_observability-0.2.5/pyproject.toml` & `nr_openai_observability-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nr-openai-observability"
-version = "0.2.5"
+version = "0.2.6"
 description = "A lightweight tool to monitor your OpenAI workload."
 authors = ["AIR <air-opensource@newrelic.com>"]
 repository = "https://github.com/newrelic/nr-openai-observability"
 readme = "README.md"
 homepage = "https://newrelic.com/instant-observability/openai"
 keywords = ["newrelic", "observability", "openai", "gpt", "chatGPT", "GPT-4", "monitor", "generative", "ai"]
```

### Comparing `nr_openai_observability-0.2.5/PKG-INFO` & `nr_openai_observability-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-openai-observability
-Version: 0.2.5
+Version: 0.2.6
 Summary: A lightweight tool to monitor your OpenAI workload.
 Home-page: https://newrelic.com/instant-observability/openai
 Keywords: newrelic,observability,openai,gpt,chatGPT,GPT-4,monitor,generative,ai
 Author: AIR
 Author-email: air-opensource@newrelic.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
@@ -54,35 +54,43 @@
 
 * Are you reporting data to the New Relic EU region? click [here](#eu-account-users) for more instructions.
 
 #### STEP 2: Add the following two lines to your code
 
 ```python
 from nr_openai_observability import monitor
-monitor.initialization()
+monitor.initialization(
+    application_name="OpenAI observability example"
+)
 ```
 
 #### Code example:
 
 ```python
 
 import os
 
 import openai
 from nr_openai_observability import monitor
 
-monitor.initialization()
+monitor.initialization(
+    application_name="OpenAI observability example"
+)
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
-openai.Completion.create(
-    model="text-davinci-003",
-    prompt="What is Observability?",
-    max_tokens=20,
-    temperature=0 
+response = openai.ChatCompletion.create(
+    model="gpt-3.5-turbo",
+    messages=[
+        {
+            "role": "user",
+            "content": "Write a rhythm about observability",
+        },
+    ],
 )
+print(response["choices"][0]["message"]["content"])
 ```
 
 #### STEP 3: Follow the instruction [here](https://one.newrelic.com/launcher/catalog-pack-details.launcher/?pane=eyJuZXJkbGV0SWQiOiJjYXRhbG9nLXBhY2stZGV0YWlscy5jYXRhbG9nLXBhY2stY29udGVudHMiLCJxdWlja3N0YXJ0SWQiOiI1ZGIyNWRiZC1hNmU5LTQ2ZmMtYTcyOC00Njk3ZjY3N2ZiYzYifQ==) to add the dashboard to your New Relic account.
 
 ### EU Account Users:
 
 If you are using an EU region account, you should also set your `EVENT_CLIENT_HOST`:
```

