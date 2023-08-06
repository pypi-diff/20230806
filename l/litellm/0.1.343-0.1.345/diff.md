# Comparing `tmp/litellm-0.1.343.tar.gz` & `tmp/litellm-0.1.345.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.343.tar", max compression
+gzip compressed data, was "litellm-0.1.345.tar", max compression
```

## Comparing `litellm-0.1.343.tar` & `litellm-0.1.345.tar`

### file list

```diff
@@ -1,34 +1,40 @@
--rw-r--r--   0        0        0     1065 2023-08-05 20:42:04.161228 litellm-0.1.343/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 20:42:04.161228 litellm-0.1.343/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/.DS_Store
--rw-r--r--   0        0        0     2059 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    13723 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4506 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1651 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      530 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/timeout.py
--rw-r--r--   0        0        0    18672 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-05 20:42:04.165228 litellm-0.1.343/pyproject.toml
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 litellm-0.1.343/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 23:32:01.881235 litellm-0.1.345/LICENSE
+-rw-r--r--   0        0        0     2575 2023-08-05 23:32:01.881235 litellm-0.1.345/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/.DS_Store
+-rw-r--r--   0        0        0     2059 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4682 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    13723 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      789 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2578 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4506 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1651 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      530 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/timeout.py
+-rw-r--r--   0        0        0    21896 2023-08-05 23:32:01.885235 litellm-0.1.345/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-05 23:32:01.889235 litellm-0.1.345/pyproject.toml
+-rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 litellm-0.1.345/PKG-INFO
```

### Comparing `litellm-0.1.343/LICENSE` & `litellm-0.1.345/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/README.md` & `litellm-0.1.345/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,23 @@
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
 pip install litellm==0.1.1
 ```
 
+## Streaming Queries
+liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
+```python
+response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
+for chunk in response:
+    print(chunk['choices'][0]['delta'])
+```
+
 # hosted version
 - [Grab time if you want access 👋](https://calendly.com/d/4mp-gd3-k5k/berriai-1-1-onboarding-litellm-hosted-version)
 
-# why did I build this 
-- **Need for simplicity**: My code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
+# why did we build this 
+- **Need for simplicity**: Our code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
 
 # Support
 Contact us at ishaan@berri.ai / krrish@berri.ai
```

### Comparing `litellm-0.1.343/litellm/.DS_Store` & `litellm-0.1.345/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/__init__.py` & `litellm-0.1.345/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/integrations/helicone.py` & `litellm-0.1.345/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/main.py` & `litellm-0.1.345/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.345/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_api_key_param.py` & `litellm-0.1.345/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_async_fn.py` & `litellm-0.1.345/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_bad_params.py` & `litellm-0.1.345/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_client.py` & `litellm-0.1.345/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_completion.py` & `litellm-0.1.345/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_exceptions.py` & `litellm-0.1.345/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_helicone_integration.py` & `litellm-0.1.345/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_logging.py` & `litellm-0.1.345/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_model_fallback.py` & `litellm-0.1.345/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_no_client.py` & `litellm-0.1.345/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_secrets.py` & `litellm-0.1.345/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/tests/test_timeout.py` & `litellm-0.1.345/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/timeout.py` & `litellm-0.1.345/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.343/litellm/utils.py` & `litellm-0.1.345/litellm/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import dotenv, json, traceback, threading
 import subprocess, os 
 import litellm, openai 
 import random, uuid, requests
-import datetime
+import datetime, time
+from anthropic import Anthropic
+import tiktoken
+encoding = tiktoken.get_encoding("cl100k_base")
 from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, ServiceUnavailableError, OpenAIError
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 sentry_sdk_instance = None
 capture_exception = None
 add_breadcrumb = None
 posthog = None
 slack_app = None
 alerts_channel = None
 heliconeLogger = None
+aispendLogger = None
+berrispendLogger = None
 callback_list = []
 user_logger_fn = None
 additional_details = {}
 
 def print_verbose(print_statement):
   if litellm.set_verbose:
     print(f"LiteLLM: {print_statement}")
@@ -85,27 +90,29 @@
         if "logger_fn" in kwargs:
            user_logger_fn = kwargs["logger_fn"]
       except: # DO NOT BLOCK running the function because of this
         print_verbose(f"[Non-Blocking] {traceback.format_exc()}")
       pass
 
     def wrapper(*args, **kwargs):
+        start_time = None
         try:
           function_setup(*args, **kwargs)
           ## MODEL CALL
           start_time = datetime.datetime.now()
           result = original_function(*args, **kwargs)
           end_time = datetime.datetime.now()
           ## LOG SUCCESS 
           my_thread = threading.Thread(target=handle_success, args=(args, kwargs, result, start_time, end_time)) # don't interrupt execution of main thread
           my_thread.start()
           return result
         except Exception as e:
           traceback_exception = traceback.format_exc()
-          my_thread = threading.Thread(target=handle_failure, args=(e, traceback_exception, args, kwargs)) # don't interrupt execution of main thread
+          end_time = datetime.datetime.now()
+          my_thread = threading.Thread(target=handle_failure, args=(e, traceback_exception, start_time, end_time, args, kwargs)) # don't interrupt execution of main thread
           my_thread.start()
           raise e
     return wrapper
 
 ####### HELPER FUNCTIONS ################
 def get_optional_params(
     # 12 optional params
@@ -149,15 +156,15 @@
   if user != "":
       optional_params["user"] = user
   if deployment_id != None:
       optional_params["deployment_id"] = user
   return optional_params
 
 def set_callbacks(callback_list):
-  global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger
+  global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger, aispendLogger, berrispendLogger
   try:
     for callback in callback_list:
       if callback == "sentry":
         try:
             import sentry_sdk
         except ImportError:
             print_verbose("Package 'sentry_sdk' is missing. Installing it...")
@@ -189,22 +196,27 @@
           token=os.environ.get("SLACK_API_TOKEN"),
           signing_secret=os.environ.get("SLACK_API_SECRET")
         )
         alerts_channel = os.environ["SLACK_API_CHANNEL"]
         print_verbose(f"Initialized Slack App: {slack_app}")
       elif callback == "helicone":
         from .integrations.helicone import HeliconeLogger
-
         heliconeLogger = HeliconeLogger()
+      elif callback == "aispend":
+        from .integrations.aispend import AISpendLogger
+        aispendLogger = AISpendLogger()
+      elif callback == "berrispend": 
+        from .integrations.berrispend import BerriSpendLogger
+        berrispendLogger = BerriSpendLogger()
   except:
     pass
 
 
-def handle_failure(exception, traceback_exception, args, kwargs):
-    global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel
+def handle_failure(exception, traceback_exception, start_time, end_time, args, kwargs):
+    global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, aispendLogger, berrispendLogger
     try:
       # print_verbose(f"handle_failure args: {args}")
       # print_verbose(f"handle_failure kwargs: {kwargs}")
       
       success_handler = additional_details.pop("success_handler", None)
       failure_handler = additional_details.pop("failure_handler", None)
       
@@ -244,14 +256,41 @@
             print_verbose(f"PostHog Event Name: {event_name}")
             if "user_id" in additional_details:
               posthog.capture(additional_details["user_id"], event_name, ph_obj)
             else: # PostHog calls require a unique id to identify a user - https://posthog.com/docs/libraries/python
               unique_id = str(uuid.uuid4())
               posthog.capture(unique_id, event_name)
               print_verbose(f"successfully logged to PostHog!")
+          elif callback == "berrispend": 
+              print_verbose("reaches berrispend for logging!")
+              model = args[0] if len(args) > 0 else kwargs["model"]
+              messages = args[1] if len(args) > 1 else kwargs["messages"]
+              result = {
+                 "model": model,
+                 "created": time.time(),
+                 "error": traceback_exception,
+                 "usage": {
+                    "prompt_tokens": prompt_token_calculator(model, messages=messages),
+                    "completion_tokens": 0
+                 }
+              }
+              berrispendLogger.log_event(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
+          elif callback == "aispend":
+              print_verbose("reaches aispend for logging!")
+              model = args[0] if len(args) > 0 else kwargs["model"]
+              messages = args[1] if len(args) > 1 else kwargs["messages"]
+              result = {
+                 "model": model,
+                 "created": time.time(),
+                 "usage": {
+                    "prompt_tokens": prompt_token_calculator(model, messages=messages),
+                    "completion_tokens": 0
+                 }
+              }
+              aispendLogger.log_event(model=model, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
         except:
           print_verbose(f"Error Occurred while logging failure: {traceback.format_exc()}")
           pass
       
       if failure_handler and callable(failure_handler):
         call_details = {
           "exception": exception,
@@ -260,16 +299,29 @@
         failure_handler(call_details)
       pass
     except Exception as e:
       ## LOGGING
       logging(logger_fn=user_logger_fn, exception=e)
       pass
 
+def prompt_token_calculator(model, messages):
+  # use tiktoken or anthropic's tokenizer depending on the model
+  text = " ".join(message["content"] for message in messages)
+  num_tokens = 0
+  if "claude" in model:
+    anthropic = Anthropic()
+    num_tokens = anthropic.count_tokens(text)
+  else:
+    num_tokens = len(encoding.encode(text))
+  return num_tokens
+  
+      
+
 def handle_success(args, kwargs, result, start_time, end_time):
-  global heliconeLogger
+  global heliconeLogger, aispendLogger
   try:
     success_handler = additional_details.pop("success_handler", None)
     failure_handler = additional_details.pop("failure_handler", None)
     additional_details["Event_Name"] = additional_details.pop("successful_event_name", "litellm.succes_query")
     for callback in litellm.success_callback:
       try:
         if callback == "posthog":
@@ -289,25 +341,36 @@
             slack_msg += f"{detail}: {additional_details[detail]}\n"
           slack_app.client.chat_postMessage(channel=alerts_channel, text=slack_msg)
         elif callback == "helicone":
           print_verbose("reaches helicone for logging!")
           model = args[0] if len(args) > 0 else kwargs["model"]
           messages = args[1] if len(args) > 1 else kwargs["messages"]
           heliconeLogger.log_success(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
-      except:
-        print_verbose(f"Success Callback Error - {traceback.format_exc()}")
+        elif callback == "aispend":
+          print_verbose("reaches aispend for logging!")
+          model = args[0] if len(args) > 0 else kwargs["model"]
+          aispendLogger.log_event(model=model, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
+        elif callback == "berrispend":
+          print_verbose("reaches berrispend for logging!")
+          model = args[0] if len(args) > 0 else kwargs["model"]
+          messages = args[1] if len(args) > 1 else kwargs["messages"]
+          berrispendLogger.log_event(model=model, messages=messages, response_obj=result, start_time=start_time, end_time=end_time, print_verbose=print_verbose)
+      except Exception as e:
+        ## LOGGING
+        logging(logger_fn=user_logger_fn, exception=e)
+        print_verbose(f"[Non-Blocking] Success Callback Error - {traceback.format_exc()}")
         pass
 
     if success_handler and callable(success_handler):
       success_handler(args, kwargs)
     pass
   except Exception as e:
     ## LOGGING
     logging(logger_fn=user_logger_fn, exception=e)
-    print_verbose(f"Success Callback Error - {traceback.format_exc()}")
+    print_verbose(f"[Non-Blocking] Success Callback Error - {traceback.format_exc()}")
     pass
 
 
 def exception_type(model, original_exception):
     global user_logger_fn
     exception_mapping_worked = False
     try:
```

### Comparing `litellm-0.1.343/pyproject.toml` & `litellm-0.1.345/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.343"
+version = "0.1.345"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.343/PKG-INFO` & `litellm-0.1.345/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.343
+Version: 0.1.345
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -70,16 +70,24 @@
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
 pip install litellm==0.1.1
 ```
 
+## Streaming Queries
+liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
+```python
+response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
+for chunk in response:
+    print(chunk['choices'][0]['delta'])
+```
+
 # hosted version
 - [Grab time if you want access 👋](https://calendly.com/d/4mp-gd3-k5k/berriai-1-1-onboarding-litellm-hosted-version)
 
-# why did I build this 
-- **Need for simplicity**: My code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
+# why did we build this 
+- **Need for simplicity**: Our code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
 
 # Support
 Contact us at ishaan@berri.ai / krrish@berri.ai
```

