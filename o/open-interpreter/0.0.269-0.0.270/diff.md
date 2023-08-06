# Comparing `tmp/open_interpreter-0.0.269.tar.gz` & `tmp/open_interpreter-0.0.270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.269.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.270.tar", max compression
```

## Comparing `open_interpreter-0.0.269.tar` & `open_interpreter-0.0.270.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.269/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.269/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.269/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.269/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.269/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.269/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13293 2023-08-06 20:16:31.042195 open_interpreter-0.0.269/interpreter/interpreter.py
--rw-r--r--   0        0        0     2490 2023-08-06 20:04:26.529346 open_interpreter-0.0.269/interpreter/llama_2.py
--rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.269/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.269/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.269/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 20:18:39.727783 open_interpreter-0.0.269/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.269/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.270/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.270/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.270/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.270/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.270/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.270/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13559 2023-08-06 20:58:45.519021 open_interpreter-0.0.270/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2506 2023-08-06 21:09:55.632947 open_interpreter-0.0.270/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.270/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.270/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.270/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 21:10:07.113803 open_interpreter-0.0.270/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.270/PKG-INFO
```

### Comparing `open_interpreter-0.0.269/LICENSE` & `open_interpreter-0.0.270/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/README.md` & `open_interpreter-0.0.270/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/__init__.py` & `open_interpreter-0.0.270/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/cli.py` & `open_interpreter-0.0.270/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/code_block.py` & `open_interpreter-0.0.270/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/code_interpreter.py` & `open_interpreter-0.0.270/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/interpreter.py` & `open_interpreter-0.0.270/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
       if 'OPENAI_API_KEY' in os.environ:
         self.api_key = os.environ['OPENAI_API_KEY']
       else:
         # Print message with newlines on either side (aesthetic choice)
         print('', Markdown(missing_api_key_message), '')
         self.api_key = input("Enter an OpenAI API key for this session:\n")
 
+    openai.api_key = self.api_key
+
   def end_active_block(self):
     if self.active_block:
       self.active_block.end()
       self.active_block = None
 
   def respond(self):
     # Add relevant info to system_message
@@ -296,14 +298,19 @@
 
         elif self.local:
           # Llama-2
           # Get contents of current code block and save to parsed_arguments, under function_call
           if "content" in self.messages[-1]:
             current_code_block = self.messages[-1]["content"].split("```")[-1]
             arguments = {"language": "python", "code": current_code_block}
+            
+            # Llama-2 won't make a "function_call" property for us to store this under, so:
+            if "function_call" not in self.messages[-1]:
+              self.messages[-1]["function_call"] = {}
+              
             self.messages[-1]["function_call"]["parsed_arguments"] = arguments
 
       else:
         # We are not in a function call.
 
         # Check if we just left a function call
         if in_function_call == True:
```

### Comparing `open_interpreter-0.0.269/interpreter/llama_2.py` & `open_interpreter-0.0.270/interpreter/llama_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         path = os.path.join(directory, file_name)
         if os.path.exists(path):
             model_path = path
             break
     else:
         # If the file was not found, ask for confirmation to download it
         download_path = os.path.join(default_path, file_name)
-        message = f"Llama-2 not found. Would you like to download it to `{download_path}`?"
+        message = f"Llama-2 not found. Would you like to download the `6.9GB` file to `{download_path}`?"
         if confirm_action(message):
             url = "https://huggingface.co/TheBloke/Llama-2-13B-chat-GGML/resolve/main/llama-2-13b-chat.ggmlv3.q4_0.bin"
-            subprocess.run(f"curl -L '{url}' -o {download_path}", shell=True)
+            subprocess.run(f"curl -L '{url}' -o '{download_path}'", shell=True)
             model_path = download_path
             print('\n', "Finished downloading Llama-2.", '\n')
         else:
             print('\n', "Download cancelled. Exiting.", '\n')
             return None
 
     try:
```

### Comparing `open_interpreter-0.0.269/interpreter/message_block.py` & `open_interpreter-0.0.270/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/system_message.txt` & `open_interpreter-0.0.270/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/interpreter/utils.py` & `open_interpreter-0.0.270/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.269/pyproject.toml` & `open_interpreter-0.0.270/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.269"
+version = "0.0.270"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.269/PKG-INFO` & `open_interpreter-0.0.270/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.269
+Version: 0.0.270
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

