# Comparing `tmp/open_interpreter-0.0.268.tar.gz` & `tmp/open_interpreter-0.0.269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.268.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.269.tar", max compression
```

## Comparing `open_interpreter-0.0.268.tar` & `open_interpreter-0.0.269.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.268/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.268/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.268/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.268/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.268/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.268/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13275 2023-08-06 19:50:41.588826 open_interpreter-0.0.268/interpreter/interpreter.py
--rw-r--r--   0        0        0     2488 2023-08-06 19:45:25.135471 open_interpreter-0.0.268/interpreter/llama_2.py
--rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.268/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.268/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.268/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 19:53:52.598544 open_interpreter-0.0.268/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.268/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.269/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.269/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.269/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.269/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.269/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.269/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13293 2023-08-06 20:16:31.042195 open_interpreter-0.0.269/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2490 2023-08-06 20:04:26.529346 open_interpreter-0.0.269/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.269/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.269/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.269/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 20:18:39.727783 open_interpreter-0.0.269/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.269/PKG-INFO
```

### Comparing `open_interpreter-0.0.268/LICENSE` & `open_interpreter-0.0.269/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/README.md` & `open_interpreter-0.0.269/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/__init__.py` & `open_interpreter-0.0.269/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/cli.py` & `open_interpreter-0.0.269/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/code_block.py` & `open_interpreter-0.0.269/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/code_interpreter.py` & `open_interpreter-0.0.269/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/interpreter.py` & `open_interpreter-0.0.269/interpreter/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,16 @@
       url = f"https://open-procedures.replit.app/search/?query={query}"
       relevant_procedure = requests.get(url).json()["procedure"]
       info += "\n\n[Related Recommended Procedure]\n" + relevant_procedure
 
     elif self.local:
 
       # Tell Llama-2 how to run code.
+      # (We actually don't use this because we overwrite the system message with a tiny, performant one.)
+      # (But someday, when Llama is fast enough, this should be how we handle it.)
       info += "\n\nTo run Python code, simply write a Python code block (i.e ```python) in markdown. When you close it with ```, it will be run. You'll then be given its output."
 
     return info
 
   def reset(self):
     self.messages = []
     self.code_interpreters = {}
@@ -203,55 +205,48 @@
 
   def respond(self):
     # Add relevant info to system_message
     # (e.g. current working directory, username, os, etc.)
     info = self.get_info_for_system_message()
     system_message = self.system_message + "\n\n" + info
 
+    # While Llama-2 is still so slow, we need to
+    # overwrite the system message with a tiny, performant one.
+    if self.local:
+      system_message = "You are an AI that executes Python code. Use ```python to run it."
+
     # Make LLM call
     if not self.local:
       # GPT-4
       model = "gpt-4-0613"
       response = openai.ChatCompletion.create(
         model=model,
         messages=tt.trim(self.messages, model, system_message=system_message),
         functions=[function_schema],
         stream=True,
         temperature=self.temperature,
       )
     elif self.local:
       # Llama-2
-      """
       response = self.llama_instance.create_chat_completion(
         messages=tt.trim(self.messages,
                          "gpt-3.5-turbo",
                          system_message=system_message),
         stream=True,
         temperature=self.temperature,
       )
-      """
-      response = self.llama_instance.create_chat_completion(
-        messages=[{"role": "system", "content": "You are an assistant."}, {"role": "user", "content": "Hello!"}],
-        stream=True,
-        temperature=self.temperature,
-      )
-      print("DEBUG SENT RESPONSE")
-      
 
     # Initialize message, function call trackers, and active block
     self.messages.append({})
     in_function_call = False
     llama_function_call_finished = False
     self.active_block = None
 
     for chunk in response:
 
-      if self.local:
-        print("DEBUG CHUNK:", chunk)
-
       delta = chunk["choices"][0]["delta"]
 
       # Accumulate deltas into the last message in messages
       self.messages[-1] = merge_deltas(self.messages[-1], delta)
 
       # Check if we're in a function call
       if not self.local:
@@ -392,11 +387,8 @@
 
           # Go around again
           self.respond()
 
         if chunk["choices"][0]["finish_reason"] != "function_call":
           # Done!
           self.active_block.end()
-          return
-
-
-    print("DEBUG NO CHUNKS?")
+          return
```

### Comparing `open_interpreter-0.0.268/interpreter/llama_2.py` & `open_interpreter-0.0.269/interpreter/llama_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             print('', "Finished downloading Llama-2 interface.", '')
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     # Initialize and return Llama-2
     llama_2 = Llama(model_path=model_path)
-    print("\n\nLlama loaded.\n\n")
+    print("\n✅ Llama-2 loaded.\n")
   
     return llama_2
 
 def confirm_action(message):
     # Print message with newlines on either side (aesthetic choice)
     print('', Markdown(f"{message} (y/n)"), '')
     response = input().strip().lower()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `open_interpreter-0.0.268/interpreter/message_block.py` & `open_interpreter-0.0.269/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/system_message.txt` & `open_interpreter-0.0.269/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/interpreter/utils.py` & `open_interpreter-0.0.269/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.268/pyproject.toml` & `open_interpreter-0.0.269/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.268"
+version = "0.0.269"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.268/PKG-INFO` & `open_interpreter-0.0.269/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.268
+Version: 0.0.269
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

