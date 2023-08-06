# Comparing `tmp/open_interpreter-0.0.259.tar.gz` & `tmp/open_interpreter-0.0.260.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.259.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.260.tar", max compression
```

## Comparing `open_interpreter-0.0.259.tar` & `open_interpreter-0.0.260.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.259/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.259/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.259/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.259/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.259/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.259/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12760 2023-08-06 18:37:36.539276 open_interpreter-0.0.259/interpreter/interpreter.py
--rw-r--r--   0        0        0     2512 2023-08-06 18:41:51.053259 open_interpreter-0.0.259/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.259/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.259/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.259/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 18:50:16.536973 open_interpreter-0.0.259/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.259/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.260/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.260/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.260/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.260/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.260/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.260/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12820 2023-08-06 18:59:25.431754 open_interpreter-0.0.260/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2622 2023-08-06 18:57:30.883661 open_interpreter-0.0.260/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.260/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.260/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.260/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 19:00:11.763027 open_interpreter-0.0.260/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.260/PKG-INFO
```

### Comparing `open_interpreter-0.0.259/LICENSE` & `open_interpreter-0.0.260/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/README.md` & `open_interpreter-0.0.260/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/__init__.py` & `open_interpreter-0.0.260/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/cli.py` & `open_interpreter-0.0.260/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/code_block.py` & `open_interpreter-0.0.260/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/code_interpreter.py` & `open_interpreter-0.0.260/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/interpreter.py` & `open_interpreter-0.0.260/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,14 @@
     elif self.local:
       # Llama-2
       if self.llama_instance == None:
         
         # Find or install LLama-2
         self.llama_instance = get_llama_2_instance()
 
-        print("DEBUG GOT LLAMA", self.llama_instance)
-
         # If the user decided not to download it, exit gracefully
         if self.llama_instance == None:
           raise KeyboardInterrupt
 
     # If not auto_run, tell the user we'll ask permission to run code
     # We also tell them here how to exit Open Interpreter
     if not self.auto_run:
@@ -225,28 +223,29 @@
       response = self.llama_instance.create_chat_completion(
         messages=tt.trim(self.messages,
                          "gpt-3.5-turbo",
                          system_message=system_message),
         stream=True,
         temperature=self.temperature,
       )
-      print("DEBUG SENT RESPONSE")
+
+      print("DEBUG. MESSAGES:", tt.trim(self.messages,
+                         "gpt-3.5-turbo",
+                         system_message=system_message))
 
     # Initialize message, function call trackers, and active block
     self.messages.append({})
     in_function_call = False
     llama_function_call_finished = False
     self.active_block = None
 
     for chunk in response:
 
       delta = chunk.choices[0].delta
 
-      print("DEBUG CHUNK:", chunk)
-
       # Accumulate deltas into the last message in messages
       self.messages[-1] = merge_deltas(self.messages[-1], delta)
 
       # Check if we're in a function call
       if not self.local:
         condition = "function_call" in self.messages[-1]
       elif self.local:
@@ -381,7 +380,10 @@
           # Go around again
           self.respond()
 
         if chunk.choices[0].finish_reason != "function_call":
           # Done!
           self.active_block.end()
           return
+
+
+    print("DEBUG NO CHUNKS?")
```

### Comparing `open_interpreter-0.0.259/interpreter/llama_2.py` & `open_interpreter-0.0.260/interpreter/llama_2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
-import subprocess
 import appdirs
+import subprocess
+import contextlib
 from rich import print
 from rich.markdown import Markdown
 
+
 def confirm_action(message):
     # Print message with newlines on either side (aesthetic choice)
     print('', Markdown(f"{message} (y/n)"), '')
     response = input().strip().lower()
     print('') # <- Aesthetic choice
     return response == 'y'
 
@@ -61,10 +63,11 @@
             from llama_cpp import Llama
             print('', "Finished downloading Llama-2 interface.", '')
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     # Initialize and return Llama-2
-    print("DEBUG ABOUT TO GET IT")
-    llama_2 = Llama(model_path=model_path)
+    # Redirect its output into a fire because this prints a billion things
+    with contextlib.redirect_stdout(None):    
+        llama_2 = Llama(model_path=model_path)
     return llama_2
```

### Comparing `open_interpreter-0.0.259/interpreter/message_block.py` & `open_interpreter-0.0.260/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/system_message.txt` & `open_interpreter-0.0.260/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/interpreter/utils.py` & `open_interpreter-0.0.260/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.259/pyproject.toml` & `open_interpreter-0.0.260/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.259"
+version = "0.0.260"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.259/PKG-INFO` & `open_interpreter-0.0.260/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.259
+Version: 0.0.260
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

