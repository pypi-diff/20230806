# Comparing `tmp/open_interpreter-0.0.252.tar.gz` & `tmp/open_interpreter-0.0.253.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.252.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.253.tar", max compression
```

## Comparing `open_interpreter-0.0.252.tar` & `open_interpreter-0.0.253.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.252/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.252/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.252/interpreter/__init__.py
--rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.252/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.252/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.252/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12039 2023-08-06 09:11:34.948517 open_interpreter-0.0.252/interpreter/interpreter.py
--rw-r--r--   0        0        0     1313 2023-08-06 08:57:47.868669 open_interpreter-0.0.252/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.252/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.252/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.252/interpreter/utils.py
--rw-r--r--   0        0        0      585 2023-08-06 09:11:45.937298 open_interpreter-0.0.252/pyproject.toml
--rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.252/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.253/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.253/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.253/interpreter/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.253/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.253/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.253/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12059 2023-08-06 16:14:38.673244 open_interpreter-0.0.253/interpreter/interpreter.py
+-rw-r--r--   0        0        0     1376 2023-08-06 16:14:10.663265 open_interpreter-0.0.253/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.253/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.253/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.253/interpreter/utils.py
+-rw-r--r--   0        0        0      585 2023-08-06 16:14:46.333785 open_interpreter-0.0.253/pyproject.toml
+-rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.253/PKG-INFO
```

### Comparing `open_interpreter-0.0.252/LICENSE` & `open_interpreter-0.0.253/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/README.md` & `open_interpreter-0.0.253/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/__init__.py` & `open_interpreter-0.0.253/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/cli.py` & `open_interpreter-0.0.253/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/code_block.py` & `open_interpreter-0.0.253/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/code_interpreter.py` & `open_interpreter-0.0.253/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/interpreter.py` & `open_interpreter-0.0.253/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .cli import cli
 from .utils import merge_deltas, parse_partial_json
 from .message_block import MessageBlock
 from .code_block import CodeBlock
 from .code_interpreter import CodeInterpreter
+from .llama_2 import get_llama_2_instance
 
 import os
 import openai
 import getpass
 import requests
 import readline
 import tokentrim as tt
@@ -122,16 +123,15 @@
     if not self.local:
       # GPT-4
       self.verify_api_key()
     elif self.local:
       # Llama-2
       if self.llama_instance == None:
         # Find or install LLama-2
-        from .llama_2 import llama_2
-        self.llama_instance = llama_2
+        self.llama_instance = get_llama_2_instance()
 
     # Message won't be None if we're passing one in via interpreter.chat(message)
     # In that case, we respond non-interactivley and return:
     if message:
       self.messages.append({"role": "user", "content": message})
       self.respond()
       return
```

### Comparing `open_interpreter-0.0.252/interpreter/llama_2.py` & `open_interpreter-0.0.253/interpreter/llama_2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import os
 import time
 import subprocess
 
-# Define the file name to search for
-file_name = "llama-2-13b-chat.ggmlv3.q4_0.bin"
 
-# Start the timer
-start_time = time.time()
+def get_llama_2_instance():
 
-# Check for the file in each path
-for path in [os.path.expanduser("~"), os.getcwd()]:
+  # Define the file name to search for
+  file_name = "llama-2-13b-chat.ggmlv3.q4_0.bin"
+
+  # Start the timer
+  start_time = time.time()
+
+  # Check for the file in each path
+  for path in [os.path.expanduser("~"), os.getcwd()]:
     print(f"Searching for Llama-2 in {path} ...")
     for root, _, files in os.walk(path):
-        if time.time() - start_time > 5:
-            print("Search timed out after 5 seconds.")
-            break
-        if file_name in files:
-            model_path = os.path.join(root, file_name)
-            print(f"Found Llama-2 at {model_path}")
-            break
+      if time.time() - start_time > 5:
+        print("Search timed out after 5 seconds.")
+        break
+      if file_name in files:
+        model_path = os.path.join(root, file_name)
+        print(f"Found Llama-2 at {model_path}")
+        break
     else:
-        continue
+      continue
     break
-else:
+  else:
     # If the file was not found, download it
     download_path = os.path.expanduser("~") + "/llama-2/" + file_name
     print(f"Llama-2 not found. Downloading it to {download_path} ...")
     url = "https://huggingface.co/TheBloke/Llama-2-13B-chat-GGML/resolve/main/llama-2-13b-chat.ggmlv3.q4_0.bin"
     subprocess.run(f"curl -L '{url}' -o {download_path}", shell=True)
     model_path = download_path
 
-try:
-  from llama_cpp import Llama
-except:
-  print("Downloading Llama-2 interface (llama-cpp-python)...")
-  subprocess.run(["pip", "install", "llama-cpp-python"])
-  from llama_cpp import Llama
+  try:
+    from llama_cpp import Llama
+  except:
+    print("Downloading Llama-2 interface (llama-cpp-python)...")
+    subprocess.run(["pip", "install", "llama-cpp-python"])
+    from llama_cpp import Llama
 
-# Initialize Llama-2
-llama_2 = Llama(model_path=model_path)
+  # Initialize and return Llama-2
+  llama_2 = Llama(model_path=model_path)
+  return llama_2
```

### Comparing `open_interpreter-0.0.252/interpreter/message_block.py` & `open_interpreter-0.0.253/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/system_message.txt` & `open_interpreter-0.0.253/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/interpreter/utils.py` & `open_interpreter-0.0.253/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.252/pyproject.toml` & `open_interpreter-0.0.253/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.252"
+version = "0.0.253"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.252/PKG-INFO` & `open_interpreter-0.0.253/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.252
+Version: 0.0.253
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

