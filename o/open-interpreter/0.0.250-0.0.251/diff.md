# Comparing `tmp/open_interpreter-0.0.250.tar.gz` & `tmp/open_interpreter-0.0.251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.250.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.251.tar", max compression
```

## Comparing `open_interpreter-0.0.250.tar` & `open_interpreter-0.0.251.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.250/LICENSE
--rw-r--r--   0        0        0     6396 2023-08-02 00:13:19.900301 open_interpreter-0.0.250/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.250/interpreter/__init__.py
--rw-r--r--   0        0        0      870 2023-08-05 20:49:13.634295 open_interpreter-0.0.250/interpreter/cli.py
--rw-r--r--   0        0        0     2497 2023-08-05 18:13:24.110098 open_interpreter-0.0.250/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.250/interpreter/code_interpreter.py
--rw-r--r--   0        0        0     8669 2023-08-06 00:57:03.012527 open_interpreter-0.0.250/interpreter/interpreter.py
--rw-r--r--   0        0        0     7023 2023-08-05 18:23:33.196206 open_interpreter-0.0.250/interpreter/json_utils.py
--rw-r--r--   0        0        0     1111 2023-08-05 09:45:06.755389 open_interpreter-0.0.250/interpreter/message_block.py
--rw-r--r--   0        0        0     2544 2023-08-06 01:17:07.439355 open_interpreter-0.0.250/interpreter/system_message.txt
--rw-r--r--   0        0        0      585 2023-08-06 01:18:15.635289 open_interpreter-0.0.250/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 open_interpreter-0.0.250/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.251/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.251/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.251/interpreter/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.251/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.251/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.251/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12104 2023-08-06 08:59:49.792515 open_interpreter-0.0.251/interpreter/interpreter.py
+-rw-r--r--   0        0        0     1313 2023-08-06 08:57:47.868669 open_interpreter-0.0.251/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.251/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.251/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.251/interpreter/utils.py
+-rw-r--r--   0        0        0      585 2023-08-06 09:10:01.981914 open_interpreter-0.0.251/pyproject.toml
+-rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.251/PKG-INFO
```

### Comparing `open_interpreter-0.0.250/LICENSE` & `open_interpreter-0.0.251/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.250/README.md` & `open_interpreter-0.0.251/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 ## Safety Notice
 
 Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
 
 **⚠️ Open Interpreter will ask for user confirmation before executing code.**
 
-You can run `interpreter -y` or set `interpreter.no_confirm = True` to bypass this confirmation, in which case:
+You can run `interpreter -y` or set `interpreter.auto_run = True` to bypass this confirmation, in which case:
 
 - Be cautious when requesting commands that modify files or system settings.
 - Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
 - Consider running Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
 
 Open Interpreter also respects `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default.
```

### Comparing `open_interpreter-0.0.250/interpreter/cli.py` & `open_interpreter-0.0.251/interpreter/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,24 @@
   """
 
   parser = argparse.ArgumentParser(description='Chat with Open Interpreter.')
   parser.add_argument('-y',
                       '--yes',
                       action='store_true',
                       help='execute code without user confirmation')
+  parser.add_argument('-l',
+                      '--local',
+                      action='store_true',
+                      help='run fully local with llama-2')
   args = parser.parse_args()
 
   if args.yes:
     interpreter.auto_run = True
   else:
     # Print message with newlines on either side (aesthetic choice)
     print('', Markdown(confirm_mode_message), '')
 
+  if args.local:
+    interpreter.local = True
+
   # Now run the chat method
   interpreter.chat()
```

### Comparing `open_interpreter-0.0.250/interpreter/code_block.py` & `open_interpreter-0.0.251/interpreter/code_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,18 +19,22 @@
     self.code = ""
     self.active_line = None
 
     self.live = Live(auto_refresh=False, console=Console())
     self.live.start()
 
   def update_from_message(self, message):
-    if "function_call" in message and "parsed_args" in message["function_call"]:
-      if message["function_call"]["parsed_args"] != None:
-        self.language = message["function_call"]["parsed_args"].get("language")
-        self.code = message["function_call"]["parsed_args"].get("code")
+    if "function_call" in message and "parsed_arguments" in message[
+        "function_call"]:
+
+      parsed_arguments = message["function_call"]["parsed_arguments"]
+
+      if parsed_arguments != None:
+        self.language = parsed_arguments.get("language")
+        self.code = parsed_arguments.get("code")
 
         if self.code and self.language:
           self.refresh()
 
   def end(self):
     # Destroys live display
     self.live.stop()
@@ -74,8 +78,8 @@
     group = Group(
       code_panel,
       output_panel,
     )
 
     # Update the live display
     self.live.update(group)
-    self.live.refresh()
+    self.live.refresh()
```

### Comparing `open_interpreter-0.0.250/interpreter/code_interpreter.py` & `open_interpreter-0.0.251/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.250/interpreter/interpreter.py` & `open_interpreter-0.0.251/interpreter/interpreter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from .code_interpreter import CodeInterpreter
-from .code_block import CodeBlock
+from .cli import cli
+from .utils import merge_deltas, parse_partial_json
 from .message_block import MessageBlock
-from .json_utils import JsonAccumulator, close_and_parse_json
-import openai
-import tokentrim as tt
+from .code_block import CodeBlock
+from .code_interpreter import CodeInterpreter
+
 import os
+import openai
+import getpass
+import requests
 import readline
-from .cli import cli
+import tokentrim as tt
 from rich import print
 from rich.markdown import Markdown
 
-# Function schema for function-calling GPTs
+# Function schema for GPT-4
 function_schema = {
   "name": "run_code",
   "description":
   "Executes code in various programming languages and returns the output.",
   "parameters": {
     "type": "object",
     "properties": {
@@ -44,52 +47,92 @@
 """
 
 
 class Interpreter:
 
   def __init__(self):
     self.messages = []
-    self.system_message = self.generate_system_message()
     self.temperature = 0.01
     self.api_key = None
     self.auto_run = False
+    self.local = False
+
+    # Get default system message
+    # here = os.path.abspath(os.path.dirname(__file__))
+    # with open(os.path.join(here, 'system_message.txt'), 'r') as f:
+    with open('./interpreter/system_message.txt', 'r') as f:
+      self.system_message = f.read().strip()
 
     # Store Code Interpreter instances for each language
     self.code_interpreters = {}
 
     # No active block to start
     # (blocks are visual representation of messages on the terminal)
     self.active_block = None
 
+    # Note: While Open Interpreter can use Llama, we will prioritize GPT-4.
+    # GPT-4 is faster, smarter, can call functions, and is all-around easier to use.
+    # This makes GPT-4 better aligned with Open Interpreters priority to be easy to use.
+    self.llama_instance = None
+
   def cli(self):
     # The cli takes the current instance of Interpreter,
     # modifies it according to command line flags, then runs chat.
     cli(self)
 
-  def generate_system_message(self):
+  def get_info_for_system_message(self):
     """
-    Adds relevent information to system_message.txt.
+    Gets relevent information for the system message.
     """
 
-    # First get the baseline system message from system_message.txt
-    here = os.path.abspath(os.path.dirname(__file__))
-    with open(os.path.join(here, 'system_message.txt'), 'r') as f:
-      system_message = f.read().strip()
+    info = ""
+
+    # Add user info
+    username = getpass.getuser()
+    current_working_directory = os.getcwd()
+    operating_system = os.name if os.name != 'nt' else os.uname().sysname
+    info += f"\n\n[User Info]\nName: {username}\nCWD: {current_working_directory}\nOS: {operating_system}"
+
+    if not self.local:
+      
+      # Open Procedures is an open-source database of tiny, structured coding tutorials.
+      # We can query it semantically and append relevant tutorials to our system message:
+      
+      # Get a procedure that's relevant to the last message
+      query = str(self.messages[-1])
+      url = f"https://open-procedures.replit.app/search/?query={query}"
+      relevant_procedure = requests.get(url).json()["procedure"]
+      info += "\n\n[Related Recommended Procedure]\n" + relevant_procedure
 
-    return system_message
+    elif self.local:
+
+      # Tell Llama-2 how to run code.
+      info += "\n\nTo run Python code, simply write a Python code block (i.e ```python) in markdown. When you close it with ```, it will be run. You'll then be given its output."
+
+    return info
 
   def reset(self):
     self.messages = []
     self.code_interpreters = {}
 
   def load(self, messages):
     self.messages = messages
 
   def chat(self, message=None, return_messages=False):
-    self.verify_api_key()
+
+    # Connect to an LLM
+    if not self.local:
+      # GPT-4
+      self.verify_api_key()
+    elif self.local:
+      # Llama-2
+      if self.llama_instance == None:
+        # Find or install LLama-2
+        from .llama_2 import llama_2
+        self.llama_instance = llama_2
 
     # Message won't be None if we're passing one in via interpreter.chat(message)
     # In that case, we respond non-interactivley and return:
     if message:
       self.messages.append({"role": "user", "content": message})
       self.respond()
       return
@@ -139,43 +182,65 @@
 
   def end_active_block(self):
     if self.active_block:
       self.active_block.end()
       self.active_block = None
 
   def respond(self):
+    # Add relevant info to system_message
+    # (e.g. current working directory, username, os, etc.)
+    info = self.get_info_for_system_message()
+    system_message = self.system_message + "\n\n" + info
+
+    # Make LLM call
+    if not self.local:
+      # GPT-4
+      model = "gpt-4-0613"
+      response = openai.ChatCompletion.create(
+        model=model,
+        messages=tt.trim(self.messages,
+                         model,
+                         system_message=system_message),
+        functions=[function_schema],
+        stream=True,
+        temperature=self.temperature,
+      )
+    elif self.local:
+      # Llama-2
+      response = self.llama_instance.create_chat_completion(
+        messages=tt.trim(self.messages,
+                         "gpt-3.5-turbo",
+                         system_message=system_message),
+        stream=True,
+        temperature=self.temperature,
+      )
 
-    # Make OpenAI call
-    model = "gpt-4-0613"
-    response = openai.ChatCompletion.create(
-      model=model,
-      messages=tt.trim(self.messages,
-                       model,
-                       system_message=self.system_message),
-      functions=[function_schema],
-      stream=True,
-      temperature=self.temperature,
-    )
-
-    # Initialize
+    # Initialize message, function call trackers, and active block
     self.messages.append({})
-    json_accumulator = JsonAccumulator()
     in_function_call = False
+    llama_function_call_finished = False
     self.active_block = None
 
     for chunk in response:
 
       delta = chunk.choices[0].delta
 
       # Accumulate deltas into the last message in messages
-      json_accumulator.receive_delta(delta)
-      self.messages[-1] = json_accumulator.accumulated_json
+      self.messages[-1] = merge_deltas(self.messages[-1], delta)
 
       # Check if we're in a function call
-      if "function_call" in self.messages[-1]:
+      if not self.local:
+        condition = "function_call" in self.messages[-1]
+      elif self.local:
+        # Since Llama-2 can't call functions, we just check if we're in a code block.
+        # This simply returns true if the number of "```" in the message is odd.
+        condition = self.messages[-1]["content"].count("```") % 2 == 1
+      
+      if condition:
+        # We are in a function call.
 
         # Check if we just entered a function call
         if in_function_call == False:
 
           # If so, end the last block,
           self.end_active_block()
 
@@ -187,39 +252,59 @@
 
           # then create a new code block
           self.active_block = CodeBlock()
 
         # Remember we're in a function_call
         in_function_call = True
 
-        # Parse arguments and save to parsed_args, under function_call
-        if "arguments" in self.messages[-1]["function_call"]:
-          args = self.messages[-1]["function_call"]["arguments"]
-
-          # There are some common errors made in GPT function calls.
-          new_parsed_args = close_and_parse_json(args)
-
-          if new_parsed_args:
-            # Only overwrite what we have if it's not None (which means it failed to parse)
-            self.messages[-1]["function_call"]["parsed_args"] = new_parsed_args
+        # Now let's parse the function's arguments:
+
+        if not self.local:
+          # GPT-4
+          # Parse arguments and save to parsed_arguments, under function_call
+          if "arguments" in self.messages[-1]["function_call"]:
+            arguments = self.messages[-1]["function_call"]["arguments"]
+            new_parsed_arguments = parse_partial_json(arguments)
+            if new_parsed_arguments:
+              # Only overwrite what we have if it's not None (which means it failed to parse)
+              self.messages[-1]["function_call"]["parsed_arguments"] = new_parsed_arguments
+        
+        elif self.local:
+          # Llama-2
+          # Get contents of current code block and save to parsed_arguments, under function_call
+          current_code_block = self.messages[-1]["content"].split("```")[-1]
+          arguments = {"language": "python", "code": current_code_block}
+          self.messages[-1]["function_call"]["parsed_arguments"] = arguments
 
       else:
+        # We are not in a function call.
+
+        # Check if we just left a function call
+        if in_function_call == True:
+
+          if self.local:
+            # This is the same as when GPT-4 gives finish_reason as function_call.
+            # We have just finished a code block, so now we should run it.
+            llama_function_call_finished = True
+
+        # Remember we're not in a function_call
+        in_function_call = False
 
-        # If we're not in a function call and there's no active block,
+        # If there's no active block,
         if self.active_block == None:
 
           # Create a message block
           self.active_block = MessageBlock()
 
       # Update active_block
       self.active_block.update_from_message(self.messages[-1])
 
       # Check if we're finished
-      if chunk.choices[0].finish_reason:
-        if chunk.choices[0].finish_reason == "function_call":
+      if chunk.choices[0].finish_reason or llama_function_call_finished:
+        if chunk.choices[0].finish_reason == "function_call" or llama_function_call_finished:
           # Time to call the function!
           # (Because this is Open Interpreter, we only have one function.)
 
           # Ask for user confirmation to run code
           if self.auto_run == False:
 
             # End the active block so you can run input() below it
@@ -248,16 +333,15 @@
                 "run_code",
                 "content":
                 "User decided not to run this code."
               })
               return
 
           # Create or retrieve a Code Interpreter for this language
-          language = self.messages[-1]["function_call"]["parsed_args"][
-            "language"]
+          language = self.messages[-1]["function_call"]["parsed_arguments"]["language"]
           if language not in self.code_interpreters:
             self.code_interpreters[language] = CodeInterpreter(language)
           code_interpreter = self.code_interpreters[language]
 
           # Let Code Interpreter control the active_block
           code_interpreter.active_block = self.active_block
           code_interpreter.run()
@@ -274,8 +358,8 @@
 
           # Go around again
           self.respond()
 
         if chunk.choices[0].finish_reason != "function_call":
           # Done!
           self.active_block.end()
-          return
+          return
```

### Comparing `open_interpreter-0.0.250/interpreter/system_message.txt` & `open_interpreter-0.0.251/interpreter/system_message.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,31 +14,8 @@
 
 When a user refers to a filename, they're likely referring to an existing file in the directory you're currently in (run_code executes on the user's machine).
 
 Write messages to the user in Markdown.
 
 In general, try to make plans with as few steps as possible. Just write code that should generally work, then make sure it did. In general we want to run as few code blocks per user request as possible.
 
-Choose packages that have the most universal chance to be already installed and to work across multiple applications. Things like ffmpeg, pandoc, that are well-supported, famous, and powerful.
-
-[Preferred Packages]
-Audio effects: `pedalboard`
-YouTube downloading: `yt-dlp`
-Video: `ffmpeg`
-OS actions like reading emails, opening files: (If Mac user) Write Applescript in a multiline string then use `subprocess` to run it.
-File conversion: `pandoc`
-
-Note: Selenium has been updated to no longer require webdriver_manager. Just use `driver = webdriver.Chrome()`.
-
-[Traceback Protocol]
-If you encounter an error, do not try to use an alternative method yet. Instead:
-
-**Write a message to the user explaining what happened and theorizing why. Do not try to run_code immediatly after run_code has errored.**
-
-If a solution is apparent (and is not simply changing methods / using a new package) attempt it.
-If not, list these steps in a message to the user, then follow them one-by-one:
-
-1. Create and run a minimal reproducible example.
-2. Use dir() to verify correct imports. There may be a better object to import from the module.
-3. Print docstrings of functions/classes using print(func.__doc__).
-
-Only then are you permitted to use an alternative method.
+Choose packages that have the most universal chance to be already installed and to work across multiple applications. Things like ffmpeg, pandoc, that are well-supported, famous, and powerful.
```

### Comparing `open_interpreter-0.0.250/pyproject.toml` & `open_interpreter-0.0.251/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.250"
+version = "0.0.251"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.250/PKG-INFO` & `open_interpreter-0.0.251/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.250
+Version: 0.0.251
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -168,15 +168,15 @@
 
 ## Safety Notice
 
 Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
 
 **⚠️ Open Interpreter will ask for user confirmation before executing code.**
 
-You can run `interpreter -y` or set `interpreter.no_confirm = True` to bypass this confirmation, in which case:
+You can run `interpreter -y` or set `interpreter.auto_run = True` to bypass this confirmation, in which case:
 
 - Be cautious when requesting commands that modify files or system settings.
 - Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
 - Consider running Open Interpreter in a restricted environment like Google Colab or Replit. These environments are more isolated, reducing the risks associated with executing arbitrary code.
 
 Open Interpreter also respects `interpreter.forbidden_commands`, a list of potentially harmful commands that are disallowed by default.
```

