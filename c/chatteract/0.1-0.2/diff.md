# Comparing `tmp/chatteract-0.1.tar.gz` & `tmp/chatteract-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatteract-0.1.tar", last modified: Wed Aug  2 13:32:54 2023, max compression
+gzip compressed data, was "chatteract-0.2.tar", last modified: Sun Aug  6 15:24:06 2023, max compression
```

## Comparing `chatteract-0.1.tar` & `chatteract-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-02 13:32:54.184198 chatteract-0.1/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-02 13:32:54.183653 chatteract-0.1/PKG-INFO
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     6661 2023-08-02 13:22:02.000000 chatteract-0.1/README.md
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-02 13:32:54.170563 chatteract-0.1/chatteract/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      120 2023-08-02 11:44:07.000000 chatteract-0.1/chatteract/__init__.py
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     5143 2023-08-02 11:43:47.000000 chatteract-0.1/chatteract/handle_openai_response_and_execute_functions.py
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     2816 2023-08-01 17:29:49.000000 chatteract-0.1/chatteract/send_api_request.py
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-02 13:32:54.182671 chatteract-0.1/chatteract.egg-info/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-02 13:32:53.000000 chatteract-0.1/chatteract.egg-info/PKG-INFO
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      300 2023-08-02 13:32:54.000000 chatteract-0.1/chatteract.egg-info/SOURCES.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)        1 2023-08-02 13:32:53.000000 chatteract-0.1/chatteract.egg-info/dependency_links.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       18 2023-08-02 13:32:54.000000 chatteract-0.1/chatteract.egg-info/requires.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       11 2023-08-02 13:32:54.000000 chatteract-0.1/chatteract.egg-info/top_level.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       38 2023-08-02 13:32:54.184412 chatteract-0.1/setup.cfg
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     1730 2023-08-02 13:32:44.000000 chatteract-0.1/setup.py
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:24:06.175139 chatteract-0.2/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-06 15:24:06.174570 chatteract-0.2/PKG-INFO
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     7728 2023-08-06 15:21:10.000000 chatteract-0.2/README.md
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:24:06.140844 chatteract-0.2/chatteract/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      120 2023-08-02 11:44:07.000000 chatteract-0.2/chatteract/__init__.py
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     5730 2023-08-06 15:10:03.000000 chatteract-0.2/chatteract/handle_openai_response_and_execute_functions.py
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     2816 2023-08-01 17:29:49.000000 chatteract-0.2/chatteract/send_api_request.py
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:24:06.172980 chatteract-0.2/chatteract.egg-info/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-06 15:24:05.000000 chatteract-0.2/chatteract.egg-info/PKG-INFO
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      300 2023-08-06 15:24:05.000000 chatteract-0.2/chatteract.egg-info/SOURCES.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)        1 2023-08-06 15:24:05.000000 chatteract-0.2/chatteract.egg-info/dependency_links.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       18 2023-08-06 15:24:05.000000 chatteract-0.2/chatteract.egg-info/requires.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       11 2023-08-06 15:24:05.000000 chatteract-0.2/chatteract.egg-info/top_level.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       38 2023-08-06 15:24:06.175309 chatteract-0.2/setup.cfg
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     1730 2023-08-06 15:10:17.000000 chatteract-0.2/setup.py
```

### Comparing `chatteract-0.1/PKG-INFO` & `chatteract-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatteract
-Version: 0.1
+Version: 0.2
 Summary: A package to handle OpenAI responses and execute function calls.
 Home-page: https://github.com/aspelund/chatter-act
 Author: Mattias Aspelund
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `chatteract-0.1/README.md` & `chatteract-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # ChatterAct
 
 ChatterAct is a Python package developed to streamline the integration of OpenAI's GPT-4 function calling capabilities into your applications. Its primary goal is to provide a simplified, yet flexible mechanism for exposing numerous functions to the AI model with minimal effort. ChatterAct handles the execution and piping, enabling you to start simple with one or two AI functions and expand as the complexity of your project grows.
 
 Basically, what you need to do to get started is to follow a simple pattern for the functions that you want to expose to GPT, and to use the wrapper for the GPT calling.
 
+## Installation
+
+Use pip to install it and then try one of the examples described below:
+
+```
+pip install chatteract
+```
+
 ## Background
 
 With the function calling capability of the models `gpt-4-0613` and `gpt-3.5-turbo-0613` it is simple to make it easy to integrate GPT into your own applications. With it, you can expose the AI to your own functions without having to ask it to provide the output in the form of json (as this is done automatically).
 
 When implementing some initial functions, my own first project's integration to the API got a bit unmanagable. At the same time I wanted to keep my integrations lightweight and not dependent on large automation frameworks for LLM's. Given this I created this lightweight solution that makes it easy to create new functions that GPT can call to talk directly to my applications.
 
 It was also obvious that the API's for this new functionality was a bit unstable, as I could see that I got responses that included invalid json and also frequent 500 responses from the API.
@@ -71,20 +79,22 @@
 
 # OpenAI settings
 openai_settings = {
     "model": "gpt-4-0613",
     "url": "https://api.openai.com/v1/chat/completions",
     "max_retries": 3,
     "retry_delay": 3,
+    "max_consecutive_function_calls": 1,
     "max_tokens": 8000,
     "headers": {
         "Authorization": f"Bearer {os.getenv('OPENAI_API_KEY')}",
     }
 }
 
+
 # Start the conversation with a system message
 messages = [
     {
         'role': 'system',
         'content': 'This is a system message to start the conversation.'
     },
     {
@@ -155,10 +165,32 @@
 
 # Create the AI function
 hello_world_ai_function = get_ai_function('hello_world', hello_world, hello_world_arg_process, hello_world_description)
 ```
 
 This code block creates an AI function `hello_world`, which can be used in `handle_openai_response_and_execute_functions` to process and handle OpenAI's responses.
 
+## OpenAI Settings
+
+Here is an example openai settings that works.
+
+```
+openai_settings = {
+    "model": "gpt-4-0613",
+    "url": "https://api.openai.com/v1/chat/completions",
+    "max_retries": 3,
+    "retry_delay": 3,
+    "max_consecutive_function_calls": 1,
+    "max_tokens": 8000,
+    "headers": {
+        "Authorization": f"Bearer {os.getenv('OPENAI_API_KEY')}",
+    }
+}
+```
+
+`max_retries` is the number of times the script tries to call the API when the response contains badly formatted json in the arguments.
+`retry_delay` is the number of seconds that the AI should wait if an error occurs before trying again.
+`max_consecutive_function_calls` is used to make sure that the AI doesn't end up in a strange loop. This sometimes happens, and the AI sort of start giving itself content together with the function call, and leads to the AI making a new function call based on its own instructions.
+
 # Collaboration
 
 if you want to help out, feel free to raise tickets or create your own pull requests. I am also planning to add some handy out of the box functions.
```

### Comparing `chatteract-0.1/chatteract/handle_openai_response_and_execute_functions.py` & `chatteract-0.2/chatteract/handle_openai_response_and_execute_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,19 @@
         return False
 
 
 def handle_openai_response_and_execute_functions(messages, ai_functions, api_settings):
     pipeline = prepare_pipeline(ai_functions)
     new_messages = []
     max_retries = api_settings.get("max_retries", 3)
+    max_consecutive_function_calls = api_settings.get("max_consecutive_function_calls", 3)
+    num_cons_function_calls = 0
     while True:
+        if num_cons_function_calls >= max_consecutive_function_calls:
+            raise AIFunctionCallsExceedingMaxConsecutiveError()
         for i in range(max_retries):
             try:
                 with (open("logs/messages.txt", "w")) as f:
                     f.write(json.dumps(messages, indent=2))
                 o_response = send_api_request(
                     messages, api_settings, pipeline['descriptions'])
                 o_response['content'] = "" if o_response['content'] is None else o_response['content']
@@ -27,14 +31,15 @@
                 o_response = json.loads(json.dumps(o_response))
                 if is_function_call(o_response):
                     try:
                         result = execute_function_call(
                             o_response, pipeline['processes'])
                         messages.append(result)
                         new_messages.append(result)
+                        num_cons_function_calls += 1
                     except FunctionExecutionError as fee:
                         raise fee  # Re-raise the exception to be handled by the caller
                 else:
                     break
             except json.JSONDecodeError:
                 if i < max_retries - 1:  # i is zero indexed
                     # Add a new message to inform the AI about the error
@@ -125,10 +130,15 @@
     """
 
     def __init__(self, function_name):
         super().__init__(self,
                          f"Function call did not complete successfully. Result is None for function {function_name}.")
 
 
+class AIFunctionCallsExceedingMaxConsecutiveError(Exception):
+    def __init__(self, max_consecutive_function_calls):
+        super().__init__(self,
+                         f"Number of consecutive AI function calls exceeded the maximum of {max_consecutive_function_calls}.")
+
 class OpenAIResponseError(Exception):
     """Custom exception to indicate an error in the OpenAI response."""
     pass
```

### Comparing `chatteract-0.1/chatteract/send_api_request.py` & `chatteract-0.2/chatteract/send_api_request.py`

 * *Files identical despite different names*

### Comparing `chatteract-0.1/chatteract.egg-info/PKG-INFO` & `chatteract-0.2/chatteract.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatteract
-Version: 0.1
+Version: 0.2
 Summary: A package to handle OpenAI responses and execute function calls.
 Home-page: https://github.com/aspelund/chatter-act
 Author: Mattias Aspelund
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `chatteract-0.1/setup.py` & `chatteract-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatteract',  # The name of your package
-    version='0.1',  # The current version of your package
+    version='0.2',  # The current version of your package
     packages=find_packages(),  # List of all python packages to include. find_packages() automatically detects all packages and subpackages.
     author='Mattias Aspelund',  # Your name    
     description='A package to handle OpenAI responses and execute function calls.',  # A brief description of your package
     long_description="""ChatterAct is a Python package developed to streamline the integration of OpenAI\'s GPT-4 function calling capabilities into your applications. Its primary goal is to provide a simplified, yet flexible mechanism for exposing numerous functions to the AI model with minimal effort. ChatterAct handles the execution and piping, enabling you to start simple with one or two AI functions and expand as the complexity of your project grows.
 
 Basically, what you need to do to get started is to follow a simple pattern for the functions that you want to expose to GPT, and to use the wrapper for the GPT calling.""",
     url='https://github.com/aspelund/chatter-act',  # Link to the github repo or website
```

