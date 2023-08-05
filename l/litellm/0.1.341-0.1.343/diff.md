# Comparing `tmp/litellm-0.1.341.tar.gz` & `tmp/litellm-0.1.343.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.341.tar", max compression
+gzip compressed data, was "litellm-0.1.343.tar", max compression
```

## Comparing `litellm-0.1.341.tar` & `litellm-0.1.343.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1065 2023-08-05 19:21:37.549398 litellm-0.1.341/LICENSE
--rw-r--r--   0        0        0     2285 2023-08-05 19:21:37.549398 litellm-0.1.341/README.md
--rw-r--r--   0        0        0     6148 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/.DS_Store
--rw-r--r--   0        0        0     1985 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3548 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/integrations/helicone.py
--rw-r--r--   0        0        0    13738 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     2578 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4506 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0      530 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-05 19:21:37.549398 litellm-0.1.341/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/timeout.py
--rw-r--r--   0        0        0    17992 2023-08-05 19:21:37.553398 litellm-0.1.341/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-05 19:21:37.553398 litellm-0.1.341/pyproject.toml
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 litellm-0.1.341/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 20:42:04.161228 litellm-0.1.343/LICENSE
+-rw-r--r--   0        0        0     2285 2023-08-05 20:42:04.161228 litellm-0.1.343/README.md
+-rw-r--r--   0        0        0     6148 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/.DS_Store
+-rw-r--r--   0        0        0     2059 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3548 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0    13723 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     2578 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4506 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1651 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      530 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/timeout.py
+-rw-r--r--   0        0        0    18672 2023-08-05 20:42:04.165228 litellm-0.1.343/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-05 20:42:04.165228 litellm-0.1.343/pyproject.toml
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 litellm-0.1.343/PKG-INFO
```

### Comparing `litellm-0.1.341/LICENSE` & `litellm-0.1.343/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/README.md` & `litellm-0.1.343/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/.DS_Store` & `litellm-0.1.343/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/__init__.py` & `litellm-0.1.343/litellm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     'claude-2': 100000,
     'command-nightly': 4096,
     'replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1': 4096,
 }
 ####### PROXY PARAMS ################### configurable params if you use proxy models like Helicone
 api_base = None
 headers = None
+####### Secret Manager #####################
+secret_manager_client = None
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   "gpt-4",
   "gpt-4-0613",
   "gpt-4-32k",
   "gpt-4-32k-0613",
   #################
```

### Comparing `litellm-0.1.341/litellm/integrations/helicone.py` & `litellm-0.1.343/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/main.py` & `litellm-0.1.343/litellm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import tiktoken
 encoding = tiktoken.get_encoding("cl100k_base")
 from tenacity import (
     retry,
     stop_after_attempt,
     wait_random_exponential,
 )  # for exponential backoff
+from litellm.utils import get_secret
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 new_response = {
         "choices": [
           {
             "finish_reason": "stop",
@@ -61,22 +62,22 @@
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
-      openai.api_base = litellm.api_base if litellm.api_base is not None else os.environ.get("AZURE_API_BASE")
-      openai.api_version = os.environ.get("AZURE_API_VERSION")
+      openai.api_base = litellm.api_base if litellm.api_base is not None else get_secret("AZURE_API_BASE")
+      openai.api_version = get_secret("AZURE_API_VERSION")
       if api_key:
           openai.api_key = api_key
       elif litellm.azure_key:
           openai.api_key = litellm.azure_key
       else:
-          openai.api_key = os.environ.get("AZURE_API_KEY")
+          openai.api_key = get_secret("AZURE_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
          response = openai.ChatCompletion.create(
             engine=model,
             messages = messages,
@@ -94,15 +95,15 @@
       openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
       if api_key:
           openai.api_key = api_key
       elif litellm.openai_key:
           openai.api_key = litellm.openai_key
       else:
-          openai.api_key = os.environ.get("OPENAI_API_KEY")
+          openai.api_key = get_secret("OPENAI_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
          response = openai.ChatCompletion.create(
           model=model,
           messages = messages,
@@ -120,15 +121,15 @@
       openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
       if api_key:
           openai.api_key = api_key
       elif litellm.openai_key:
           openai.api_key = litellm.openai_key
       else:
-          openai.api_key = os.environ.get("OPENAI_API_KEY")
+          openai.api_key = get_secret("OPENAI_API_KEY")
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
         response = openai.Completion.create(
           model=model,
@@ -148,16 +149,16 @@
       model_response["created"] = response["created"]
       model_response["model"] = model
       model_response["usage"] = response["usage"]
       response = model_response
     elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
-      if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
-        replicate_api_token = os.environ.get("REPLICATE_API_KEY")
+      if not get_secret("REPLICATE_API_TOKEN") and get_secret("REPLICATE_API_KEY"):
+        replicate_api_token = get_secret("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       elif api_key:
          os.environ["REPLICATE_API_TOKEN"] = api_key
       elif litellm.replicate_key:
          os.environ["REPLICATE_API_TOKEN"] = litellm.replicate_key
 
       prompt = " ".join([message["content"] for message in messages])
@@ -236,15 +237,15 @@
       response = model_response
     elif model in litellm.cohere_models:
       if api_key:
         cohere_key = api_key
       elif litellm.cohere_key:
         cohere_key = litellm.cohere_key
       else:
-        cohere_key = os.environ.get("COHERE_API_KEY")
+        cohere_key = get_secret("COHERE_API_KEY")
       co = cohere.Client(cohere_key)
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = co.generate(  
         model=model,
@@ -282,27 +283,27 @@
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def embedding(model, input=[], azure=False, force_timeout=60, logger_fn=None):
   try:
     response = None
     if azure == True:
       # azure configs
       openai.api_type = "azure"
-      openai.api_base = os.environ.get("AZURE_API_BASE")
-      openai.api_version = os.environ.get("AZURE_API_VERSION")
-      openai.api_key = os.environ.get("AZURE_API_KEY")
+      openai.api_base = get_secret("AZURE_API_BASE")
+      openai.api_version = get_secret("AZURE_API_VERSION")
+      openai.api_key = get_secret("AZURE_API_KEY")
       ## LOGGING
       logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
       ## EMBEDDING CALL
       response = openai.Embedding.create(input=input, engine=model)
       print_verbose(f"response_value: {str(response)[:50]}")
     elif model in litellm.open_ai_embedding_models:
       openai.api_type = "openai"
       openai.api_base = "https://api.openai.com/v1"
       openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      openai.api_key = get_secret("OPENAI_API_KEY")
       ## LOGGING
       logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
       ## EMBEDDING CALL
       response = openai.Embedding.create(input=input, model=model)
       print_verbose(f"response_value: {str(response)[:50]}")
     else: 
       logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
```

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.343/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_api_key_param.py` & `litellm-0.1.343/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_async_fn.py` & `litellm-0.1.343/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_bad_params.py` & `litellm-0.1.343/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_client.py` & `litellm-0.1.343/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_completion.py` & `litellm-0.1.343/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_exceptions.py` & `litellm-0.1.343/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_helicone_integration.py` & `litellm-0.1.343/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_logging.py` & `litellm-0.1.343/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_model_fallback.py` & `litellm-0.1.343/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_no_client.py` & `litellm-0.1.343/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/tests/test_timeout.py` & `litellm-0.1.343/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/timeout.py` & `litellm-0.1.343/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.341/litellm/utils.py` & `litellm-0.1.343/litellm/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,8 +399,25 @@
     }
     try:
       # Make the POST request to localhost:3000
       response = requests.post('https://litellm.berri.ai/logging', json=payload)
       response.raise_for_status()  # Raise an exception for HTTP errors
     except requests.exceptions.RequestException as e:
         # Handle any errors in the request
-        pass
+        pass
+
+######### Secret Manager ############################
+# checks if user has passed in a secret manager client
+# if passed in then checks the secret there
+def get_secret(secret_name):
+  if litellm.secret_manager_client != None:
+     # TODO: check which secret manager is being used
+     # currently only supports Infisical
+     secret = litellm.secret_manager_client.get_secret(secret_name).secret_value
+     if secret != None:
+        # if secret manager fails default to using .env variables
+        os.environ[secret_name] = secret # set to env to be safe
+        return secret
+     else:
+      return os.environ.get(secret_name)
+  else:
+    return os.environ.get(secret_name)
```

### Comparing `litellm-0.1.341/pyproject.toml` & `litellm-0.1.343/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.341"
+version = "0.1.343"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.341/PKG-INFO` & `litellm-0.1.343/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.341
+Version: 0.1.343
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

