# Comparing `tmp/open_interpreter-0.0.264.tar.gz` & `tmp/open_interpreter-0.0.265.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.264.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.265.tar", max compression
```

## Comparing `open_interpreter-0.0.264.tar` & `open_interpreter-0.0.265.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.264/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.264/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.264/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.264/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.264/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.264/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13049 2023-08-06 19:27:18.202645 open_interpreter-0.0.264/interpreter/interpreter.py
--rw-r--r--   0        0        0     2630 2023-08-06 19:37:43.284629 open_interpreter-0.0.264/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.264/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.264/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.264/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 19:37:37.140059 open_interpreter-0.0.264/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.264/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.265/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.265/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.265/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.265/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.265/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.265/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13052 2023-08-06 19:41:10.023807 open_interpreter-0.0.265/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2758 2023-08-06 19:40:10.006240 open_interpreter-0.0.265/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.265/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.265/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.265/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 19:42:44.320554 open_interpreter-0.0.265/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.265/PKG-INFO
```

### Comparing `open_interpreter-0.0.264/LICENSE` & `open_interpreter-0.0.265/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/README.md` & `open_interpreter-0.0.265/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/__init__.py` & `open_interpreter-0.0.265/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/cli.py` & `open_interpreter-0.0.265/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/code_block.py` & `open_interpreter-0.0.265/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/code_interpreter.py` & `open_interpreter-0.0.265/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/interpreter.py` & `open_interpreter-0.0.265/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     self.active_block = None
 
     for chunk in response:
 
       if self.local:
         print("DEBUG CHUNK:", chunk)
 
-      delta = chunk["choices"][0].delta
+      delta = chunk["choices"][0]["delta"]
 
       # Accumulate deltas into the last message in messages
       self.messages[-1] = merge_deltas(self.messages[-1], delta)
 
       # Check if we're in a function call
       if not self.local:
         condition = "function_call" in self.messages[-1]
```

### Comparing `open_interpreter-0.0.264/interpreter/llama_2.py` & `open_interpreter-0.0.265/interpreter/llama_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import os
+import sys
 import appdirs
 import subprocess
 import contextlib
 from rich import print
 from rich.markdown import Markdown
 
 
-def confirm_action(message):
-    # Print message with newlines on either side (aesthetic choice)
-    print('', Markdown(f"{message} (y/n)"), '')
-    response = input().strip().lower()
-    print('') # <- Aesthetic choice
-    return response == 'y'
-
 def get_llama_2_instance():
 
     # Define the file name
     file_name = "llama-2-13b-chat.ggmlv3.q4_0.bin"
 
     # Get user data directory for your application
     user_data_dir = appdirs.user_data_dir("open-interpreter")
@@ -63,13 +57,27 @@
             print('', "Finished downloading Llama-2 interface.", '')
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     # Initialize and return Llama-2
     # Redirect its output into a fire because this prints a billion things
-    print("DEBUG 1")
-    with contextlib.redirect_stderr(None):  
-        print("DEBUG 2")
-        llama_2 = Llama(model_path=model_path)
-    print("DEBUG 3")
-    return llama_2
+    suppress_output()
+    llama_2 = Llama(model_path=model_path)
+    enable_output()
+  
+    return llama_2
+
+def confirm_action(message):
+    # Print message with newlines on either side (aesthetic choice)
+    print('', Markdown(f"{message} (y/n)"), '')
+    response = input().strip().lower()
+    print('') # <- Aesthetic choice
+    return response == 'y'
+
+def suppress_output():
+    sys.stdout = open(os.devnull, 'w')
+    sys.stderr = open(os.devnull, 'w')
+
+def enable_output():
+    sys.stdout = sys.__stdout__
+    sys.stderr = sys.__stderr__
```

### Comparing `open_interpreter-0.0.264/interpreter/message_block.py` & `open_interpreter-0.0.265/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/system_message.txt` & `open_interpreter-0.0.265/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/interpreter/utils.py` & `open_interpreter-0.0.265/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.264/pyproject.toml` & `open_interpreter-0.0.265/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.264"
+version = "0.0.265"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.264/PKG-INFO` & `open_interpreter-0.0.265/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.264
+Version: 0.0.265
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

