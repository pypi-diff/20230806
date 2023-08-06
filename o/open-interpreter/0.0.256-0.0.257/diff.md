# Comparing `tmp/open_interpreter-0.0.256.tar.gz` & `tmp/open_interpreter-0.0.257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.256.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.257.tar", max compression
```

## Comparing `open_interpreter-0.0.256.tar` & `open_interpreter-0.0.257.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.256/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.256/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.256/interpreter/__init__.py
--rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.256/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.256/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.256/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12059 2023-08-06 16:14:38.673244 open_interpreter-0.0.256/interpreter/interpreter.py
--rw-r--r--   0        0        0     2361 2023-08-06 18:04:51.788458 open_interpreter-0.0.256/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.256/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.256/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.256/interpreter/utils.py
--rw-r--r--   0        0        0      604 2023-08-06 18:07:35.007990 open_interpreter-0.0.256/pyproject.toml
--rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 open_interpreter-0.0.256/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.257/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.257/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.257/interpreter/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.257/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.257/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.257/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12067 2023-08-06 18:11:21.011958 open_interpreter-0.0.257/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2376 2023-08-06 18:10:48.621669 open_interpreter-0.0.257/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.257/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.257/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.257/interpreter/utils.py
+-rw-r--r--   0        0        0      604 2023-08-06 18:12:21.796252 open_interpreter-0.0.257/pyproject.toml
+-rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 open_interpreter-0.0.257/PKG-INFO
```

### Comparing `open_interpreter-0.0.256/LICENSE` & `open_interpreter-0.0.257/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/README.md` & `open_interpreter-0.0.257/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/__init__.py` & `open_interpreter-0.0.257/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/cli.py` & `open_interpreter-0.0.257/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/code_block.py` & `open_interpreter-0.0.257/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/code_interpreter.py` & `open_interpreter-0.0.257/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/interpreter.py` & `open_interpreter-0.0.257/interpreter/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
             language = self.active_block.language
             code = self.active_block.code
 
             # Prompt user
             response = input("  Would you like to run this code? (y/n) \n\n  ")
             print("") # <- Aesthetic choice
 
-            if response.lower() == "y":
+            if response.strip().lower() == "y":
               # Create a new, identical block where the code will actually be run
               self.active_block = CodeBlock()
               self.active_block.language = language
               self.active_block.code = code
               
             else:
               # User declined to run code.
```

### Comparing `open_interpreter-0.0.256/interpreter/llama_2.py` & `open_interpreter-0.0.257/interpreter/llama_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import subprocess
 import appdirs
 from rich import print
 from rich.markdown import Markdown
 
 def confirm_action(message):
-    print(Markdown(f"### {message}"))
+    print('', Markdown(f"### {message}"), '')
     response = input("Proceed? (y/n): ").strip().lower()
     return response == 'y'
 
 def get_llama_2_instance():
 
     # Define the file name
     file_name = "llama-2-13b-chat.ggmlv3.q4_0.bin"
 
     # Get user data directory for your application
-    user_data_dir = appdirs.user_data_dir("llama.cpp")
+    user_data_dir = appdirs.user_data_dir("open-interpreter")
     default_path = os.path.join(user_data_dir, "models")
 
     # Ensure the directory exists
     os.makedirs(default_path, exist_ok=True)
 
     # Define the directories to check
     directories_to_check = [
```

### Comparing `open_interpreter-0.0.256/interpreter/message_block.py` & `open_interpreter-0.0.257/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/system_message.txt` & `open_interpreter-0.0.257/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/interpreter/utils.py` & `open_interpreter-0.0.257/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.256/pyproject.toml` & `open_interpreter-0.0.257/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.256"
+version = "0.0.257"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.256/PKG-INFO` & `open_interpreter-0.0.257/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.256
+Version: 0.0.257
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

