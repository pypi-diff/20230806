# Comparing `tmp/open_interpreter-0.0.257.tar.gz` & `tmp/open_interpreter-0.0.258.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.257.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.258.tar", max compression
```

## Comparing `open_interpreter-0.0.257.tar` & `open_interpreter-0.0.258.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.257/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.257/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.257/interpreter/__init__.py
--rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.257/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.257/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.257/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12067 2023-08-06 18:11:21.011958 open_interpreter-0.0.257/interpreter/interpreter.py
--rw-r--r--   0        0        0     2376 2023-08-06 18:10:48.621669 open_interpreter-0.0.257/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.257/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.257/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.257/interpreter/utils.py
--rw-r--r--   0        0        0      604 2023-08-06 18:12:21.796252 open_interpreter-0.0.257/pyproject.toml
--rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 open_interpreter-0.0.257/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.258/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.258/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.258/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.258/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.258/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.258/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12760 2023-08-06 18:37:36.539276 open_interpreter-0.0.258/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2492 2023-08-06 18:35:43.491288 open_interpreter-0.0.258/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.258/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.258/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.258/interpreter/utils.py
+-rw-r--r--   0        0        0      604 2023-08-06 18:38:00.965001 open_interpreter-0.0.258/pyproject.toml
+-rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 open_interpreter-0.0.258/PKG-INFO
```

### Comparing `open_interpreter-0.0.257/LICENSE` & `open_interpreter-0.0.258/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/README.md` & `open_interpreter-0.0.258/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/__init__.py` & `open_interpreter-0.0.258/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/code_block.py` & `open_interpreter-0.0.258/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/code_interpreter.py` & `open_interpreter-0.0.258/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/interpreter.py` & `open_interpreter-0.0.258/interpreter/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 **OpenAI API key not found.** You can [get one here](https://platform.openai.com/account/api-keys).
 
 To use Open Interpreter in your terminal, set the environment variable using `export OPENAI_API_KEY=your_api_key` on Unix-based systems, or `setx OPENAI_API_KEY your_api_key` on Windows.
 
 ---
 """
 
+confirm_mode_message = """
+**Open Interpreter** will require approval before running code. Use `interpreter -y` to bypass this.
+
+Press `CTRL-C` to exit.
+"""
+
 
 class Interpreter:
 
   def __init__(self):
     self.messages = []
     self.temperature = 0.01
     self.api_key = None
@@ -89,18 +95,18 @@
     # Add user info
     username = getpass.getuser()
     current_working_directory = os.getcwd()
     operating_system = os.name if os.name != 'nt' else os.uname().sysname
     info += f"\n\n[User Info]\nName: {username}\nCWD: {current_working_directory}\nOS: {operating_system}"
 
     if not self.local:
-      
+
       # Open Procedures is an open-source database of tiny, structured coding tutorials.
       # We can query it semantically and append relevant tutorials to our system message:
-      
+
       # Get a procedure that's relevant to the last message
       query = str(self.messages[-1])
       url = f"https://open-procedures.replit.app/search/?query={query}"
       relevant_procedure = requests.get(url).json()["procedure"]
       info += "\n\n[Related Recommended Procedure]\n" + relevant_procedure
 
     elif self.local:
@@ -115,25 +121,38 @@
     self.code_interpreters = {}
 
   def load(self, messages):
     self.messages = messages
 
   def chat(self, message=None, return_messages=False):
 
-    # Connect to an LLM
+    # Connect to an LLM (an large language model)
     if not self.local:
       # GPT-4
       self.verify_api_key()
     elif self.local:
       # Llama-2
       if self.llama_instance == None:
+        
         # Find or install LLama-2
         self.llama_instance = get_llama_2_instance()
 
-    # Message won't be None if we're passing one in via interpreter.chat(message)
+        print("DEBUG GOT LLAMA", self.llama_instance)
+
+        # If the user decided not to download it, exit gracefully
+        if self.llama_instance == None:
+          raise KeyboardInterrupt
+
+    # If not auto_run, tell the user we'll ask permission to run code
+    # We also tell them here how to exit Open Interpreter
+    if not self.auto_run:
+      # Print message with newlines on either side (aesthetic choice)
+      print('', Markdown(confirm_mode_message), '')
+
+    # `message` won't be None if we're passing one in via interpreter.chat(message)
     # In that case, we respond non-interactivley and return:
     if message:
       self.messages.append({"role": "user", "content": message})
       self.respond()
       return
 
     # Start interactive chat
@@ -192,52 +211,53 @@
 
     # Make LLM call
     if not self.local:
       # GPT-4
       model = "gpt-4-0613"
       response = openai.ChatCompletion.create(
         model=model,
-        messages=tt.trim(self.messages,
-                         model,
-                         system_message=system_message),
+        messages=tt.trim(self.messages, model, system_message=system_message),
         functions=[function_schema],
         stream=True,
         temperature=self.temperature,
       )
     elif self.local:
       # Llama-2
       response = self.llama_instance.create_chat_completion(
         messages=tt.trim(self.messages,
                          "gpt-3.5-turbo",
                          system_message=system_message),
         stream=True,
         temperature=self.temperature,
       )
+      print("DEBUG SENT RESPONSE")
 
     # Initialize message, function call trackers, and active block
     self.messages.append({})
     in_function_call = False
     llama_function_call_finished = False
     self.active_block = None
 
     for chunk in response:
 
       delta = chunk.choices[0].delta
 
+      print("DEBUG CHUNK:", chunk)
+
       # Accumulate deltas into the last message in messages
       self.messages[-1] = merge_deltas(self.messages[-1], delta)
 
       # Check if we're in a function call
       if not self.local:
         condition = "function_call" in self.messages[-1]
       elif self.local:
         # Since Llama-2 can't call functions, we just check if we're in a code block.
         # This simply returns true if the number of "```" in the message is odd.
         condition = self.messages[-1]["content"].count("```") % 2 == 1
-      
+
       if condition:
         # We are in a function call.
 
         # Check if we just entered a function call
         if in_function_call == False:
 
           # If so, end the last block,
@@ -261,16 +281,17 @@
           # GPT-4
           # Parse arguments and save to parsed_arguments, under function_call
           if "arguments" in self.messages[-1]["function_call"]:
             arguments = self.messages[-1]["function_call"]["arguments"]
             new_parsed_arguments = parse_partial_json(arguments)
             if new_parsed_arguments:
               # Only overwrite what we have if it's not None (which means it failed to parse)
-              self.messages[-1]["function_call"]["parsed_arguments"] = new_parsed_arguments
-        
+              self.messages[-1]["function_call"][
+                "parsed_arguments"] = new_parsed_arguments
+
         elif self.local:
           # Llama-2
           # Get contents of current code block and save to parsed_arguments, under function_call
           current_code_block = self.messages[-1]["content"].split("```")[-1]
           arguments = {"language": "python", "code": current_code_block}
           self.messages[-1]["function_call"]["parsed_arguments"] = arguments
 
@@ -295,52 +316,54 @@
           self.active_block = MessageBlock()
 
       # Update active_block
       self.active_block.update_from_message(self.messages[-1])
 
       # Check if we're finished
       if chunk.choices[0].finish_reason or llama_function_call_finished:
-        if chunk.choices[0].finish_reason == "function_call" or llama_function_call_finished:
+        if chunk.choices[
+            0].finish_reason == "function_call" or llama_function_call_finished:
           # Time to call the function!
           # (Because this is Open Interpreter, we only have one function.)
 
           # Ask for user confirmation to run code
           if self.auto_run == False:
 
             # End the active block so you can run input() below it
             # Save language and code so we can create a new block in a moment
             self.active_block.end()
             language = self.active_block.language
             code = self.active_block.code
 
             # Prompt user
-            response = input("  Would you like to run this code? (y/n) \n\n  ")
-            print("") # <- Aesthetic choice
+            response = input("  Would you like to run this code? (y/n)\n\n  ")
+            print("")  # <- Aesthetic choice
 
             if response.strip().lower() == "y":
               # Create a new, identical block where the code will actually be run
               self.active_block = CodeBlock()
               self.active_block.language = language
               self.active_block.code = code
-              
+
             else:
               # User declined to run code.
               self.active_block.end()
               self.messages.append({
                 "role":
                 "function",
                 "name":
                 "run_code",
                 "content":
                 "User decided not to run this code."
               })
               return
 
           # Create or retrieve a Code Interpreter for this language
-          language = self.messages[-1]["function_call"]["parsed_arguments"]["language"]
+          language = self.messages[-1]["function_call"]["parsed_arguments"][
+            "language"]
           if language not in self.code_interpreters:
             self.code_interpreters[language] = CodeInterpreter(language)
           code_interpreter = self.code_interpreters[language]
 
           # Let Code Interpreter control the active_block
           code_interpreter.active_block = self.active_block
           code_interpreter.run()
@@ -357,8 +380,8 @@
 
           # Go around again
           self.respond()
 
         if chunk.choices[0].finish_reason != "function_call":
           # Done!
           self.active_block.end()
-          return
+          return
```

### Comparing `open_interpreter-0.0.257/interpreter/llama_2.py` & `open_interpreter-0.0.258/interpreter/llama_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import subprocess
 import appdirs
 from rich import print
 from rich.markdown import Markdown
 
 def confirm_action(message):
-    print('', Markdown(f"### {message}"), '')
-    response = input("Proceed? (y/n): ").strip().lower()
+    # Print message with newlines on either side (aesthetic choice)
+    print('', Markdown(f"{message} (y/n)"), '')
+    response = input().strip().lower()
+    print('') # <- Aesthetic choice
     return response == 'y'
 
 def get_llama_2_instance():
 
     # Define the file name
     file_name = "llama-2-13b-chat.ggmlv3.q4_0.bin"
 
@@ -40,30 +42,28 @@
         download_path = os.path.join(default_path, file_name)
         message = f"Llama-2 not found. Would you like to download it to `{download_path}`?"
         if confirm_action(message):
             print(f"Downloading Llama-2 to {download_path} ...")
             url = "https://huggingface.co/TheBloke/Llama-2-13B-chat-GGML/resolve/main/llama-2-13b-chat.ggmlv3.q4_0.bin"
             subprocess.run(f"curl -L '{url}' -o {download_path}", shell=True)
             model_path = download_path
+            print('', "Finished downloading Llama-2.", '')
         else:
-            print("Download cancelled. Exiting.")
+            print('', "Download cancelled. Exiting.", '')
             return None
 
     try:
         from llama_cpp import Llama
     except:
         # Ask for confirmation to install the required pip package
-        message = "Llama-2 interface not found. Would you like to install the `llama-cpp-python` package?"
+        message = "Llama-2 interface package not found. Install `llama-cpp-python` package?"
         if confirm_action(message):
-            print("Downloading Llama-2 interface...")
             subprocess.run(["pip", "install", "llama-cpp-python"])
             from llama_cpp import Llama
+            print('', "Finished downloading Llama-2 interface.", '')
         else:
-            print("Installation cancelled. Exiting.")
+            print('', "Installation cancelled. Exiting.", '')
             return None
 
-    print("Llama", Llama)
-    print("model_path", model_path)
-
     # Initialize and return Llama-2
-    llama_2 = Llama(model_path=model_path)
+    llama_2 = Llama(model_path=model_path, verbose=False)
     return llama_2
```

### Comparing `open_interpreter-0.0.257/interpreter/message_block.py` & `open_interpreter-0.0.258/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/system_message.txt` & `open_interpreter-0.0.258/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/interpreter/utils.py` & `open_interpreter-0.0.258/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.257/pyproject.toml` & `open_interpreter-0.0.258/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.257"
+version = "0.0.258"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.257/PKG-INFO` & `open_interpreter-0.0.258/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.257
+Version: 0.0.258
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

