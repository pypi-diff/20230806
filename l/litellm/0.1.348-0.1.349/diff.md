# Comparing `tmp/litellm-0.1.348.tar.gz` & `tmp/litellm-0.1.349.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.348.tar", max compression
+gzip compressed data, was "litellm-0.1.349.tar", max compression
```

## Comparing `litellm-0.1.348.tar` & `litellm-0.1.349.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-06 04:58:45.580919 litellm-0.1.348/LICENSE
--rw-r--r--   0        0        0     2575 2023-08-06 04:58:45.580919 litellm-0.1.348/README.md
--rw-r--r--   0        0        0     6148 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/.DS_Store
--rw-r--r--   0        0        0     1962 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3548 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    13783 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2578 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4506 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5840 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1651 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/timeout.py
--rw-r--r--   0        0        0    23675 2023-08-06 04:58:45.584919 litellm-0.1.348/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-06 04:58:45.588919 litellm-0.1.348/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 litellm-0.1.348/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-06 05:15:19.111766 litellm-0.1.349/LICENSE
+-rw-r--r--   0        0        0     2575 2023-08-06 05:15:19.111766 litellm-0.1.349/README.md
+-rw-r--r--   0        0        0     6148 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/.DS_Store
+-rw-r--r--   0        0        0     2014 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    13947 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0      920 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2578 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4506 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5840 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1651 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-06 05:15:19.111766 litellm-0.1.349/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/timeout.py
+-rw-r--r--   0        0        0    23675 2023-08-06 05:15:19.115766 litellm-0.1.349/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-06 05:15:19.115766 litellm-0.1.349/pyproject.toml
+-rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 litellm-0.1.349/PKG-INFO
```

### Comparing `litellm-0.1.348/LICENSE` & `litellm-0.1.349/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/README.md` & `litellm-0.1.349/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/.DS_Store` & `litellm-0.1.349/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/__init__.py` & `litellm-0.1.349/litellm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,19 @@
         self.user = "Hello World"
 
 _thread_context = MyLocal()
 def identify(event_details):
     # Store user in thread local data
     if "user" in event_details:
         _thread_context.user = event_details["user"]
-####### PROXY PARAMS ################### configurable params if you use proxy models like Helicone
+####### ADDITIONAL PARAMS ################### configurable params if you use proxy models like Helicone, map spend to org id, etc.
 api_base = None
 headers = None
 api_version = None
+organization = None
 ####### Secret Manager #####################
 secret_manager_client = None
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   "gpt-4",
   "gpt-4-0613",
   "gpt-4-32k",
```

### Comparing `litellm-0.1.348/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.349/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.349/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.349/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.349/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/aispend.py` & `litellm-0.1.349/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/berrispend.py` & `litellm-0.1.349/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/helicone.py` & `litellm-0.1.349/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/integrations/supabase.py` & `litellm-0.1.349/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/main.py` & `litellm-0.1.349/litellm/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,16 @@
           messages = messages,
           **optional_params
         )
     elif model in litellm.open_ai_chat_completion_models:
       openai.api_type = "openai"
       openai.api_base = litellm.api_base if litellm.api_base is not None else "https://api.openai.com/v1"
       openai.api_version = None
+      if litellm.organization:
+        openai.organization = litellm.organization
       if api_key:
           openai.api_key = api_key
       elif litellm.openai_key:
           openai.api_key = litellm.openai_key
       else:
           openai.api_key = get_secret("OPENAI_API_KEY")
       ## LOGGING
@@ -122,14 +124,16 @@
       openai.api_version = None
       if api_key:
           openai.api_key = api_key
       elif litellm.openai_key:
           openai.api_key = litellm.openai_key
       else:
           openai.api_key = get_secret("OPENAI_API_KEY")
+      if litellm.organization:
+        openai.organization = litellm.organization
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       if litellm.headers:
         response = openai.Completion.create(
           model=model,
```

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.349/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_api_key_param.py` & `litellm-0.1.349/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_async_fn.py` & `litellm-0.1.349/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_bad_params.py` & `litellm-0.1.349/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.349/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_client.py` & `litellm-0.1.349/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_completion.py` & `litellm-0.1.349/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_exceptions.py` & `litellm-0.1.349/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_helicone_integration.py` & `litellm-0.1.349/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_logging.py` & `litellm-0.1.349/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_model_fallback.py` & `litellm-0.1.349/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_no_client.py` & `litellm-0.1.349/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_secrets.py` & `litellm-0.1.349/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_supabase_integration.py` & `litellm-0.1.349/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/tests/test_timeout.py` & `litellm-0.1.349/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/timeout.py` & `litellm-0.1.349/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/litellm/utils.py` & `litellm-0.1.349/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.348/pyproject.toml` & `litellm-0.1.349/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.348"
+version = "0.1.349"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.348/PKG-INFO` & `litellm-0.1.349/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.348
+Version: 0.1.349
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

