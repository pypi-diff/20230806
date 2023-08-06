# Comparing `tmp/open_interpreter-0.0.270.tar.gz` & `tmp/open_interpreter-0.0.271.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.270.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.271.tar", max compression
```

## Comparing `open_interpreter-0.0.270.tar` & `open_interpreter-0.0.271.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.270/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.270/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.270/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.270/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.270/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.270/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13559 2023-08-06 20:58:45.519021 open_interpreter-0.0.270/interpreter/interpreter.py
--rw-r--r--   0        0        0     2506 2023-08-06 21:09:55.632947 open_interpreter-0.0.270/interpreter/llama_2.py
--rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.270/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.270/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.270/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 21:10:07.113803 open_interpreter-0.0.270/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.270/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.271/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.271/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.271/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.271/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.271/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.271/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13559 2023-08-06 20:58:45.519021 open_interpreter-0.0.271/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.271/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.271/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.271/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.271/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 21:28:19.437777 open_interpreter-0.0.271/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.271/PKG-INFO
```

### Comparing `open_interpreter-0.0.270/LICENSE` & `open_interpreter-0.0.271/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/README.md` & `open_interpreter-0.0.271/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/__init__.py` & `open_interpreter-0.0.271/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/cli.py` & `open_interpreter-0.0.271/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/code_block.py` & `open_interpreter-0.0.271/interpreter/code_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,28 +32,34 @@
         self.language = parsed_arguments.get("language")
         self.code = parsed_arguments.get("code")
 
         if self.code and self.language:
           self.refresh()
 
   def end(self):
+    self.refresh(cursor=False)
     # Destroys live display
     self.live.stop()
 
-  def refresh(self):
+  def refresh(self, cursor=True):
     # Create a table for the code
     code_table = Table(show_header=False,
                        show_footer=False,
                        box=None,
                        padding=0,
                        expand=True)
     code_table.add_column()
 
+    # Get code and add cursor
+    code = self.code
+    if cursor:
+      code += "█"
+
     # Add each line of code to the table
-    code_lines = self.code.strip().split('\n')
+    code_lines = code.strip().split('\n')
     for i, line in enumerate(code_lines, start=1):
       if i == self.active_line:
         # This is the active line, print it with a white background
         syntax = Syntax(line, self.language, line_numbers=False, theme="bw")
         code_table.add_row(syntax, style="black on white")
       else:
         # This is not the active line, print it normally
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `open_interpreter-0.0.270/interpreter/code_interpreter.py` & `open_interpreter-0.0.271/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/interpreter.py` & `open_interpreter-0.0.271/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/llama_2.py` & `open_interpreter-0.0.271/interpreter/llama_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             print('', "Finished downloading Llama-2 interface.", '')
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     # Initialize and return Llama-2
     llama_2 = Llama(model_path=model_path)
-    print("\n✅ Llama-2 loaded.\n")
+    print("\n✅ Llama-2 loaded.", '')
   
     return llama_2
 
 def confirm_action(message):
     # Print message with newlines on either side (aesthetic choice)
     print('', Markdown(f"{message} (y/n)"), '')
     response = input().strip().lower()
```

### Comparing `open_interpreter-0.0.270/interpreter/message_block.py` & `open_interpreter-0.0.271/interpreter/message_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,26 @@
 
   def update_from_message(self, message):
     self.content = message.get("content", "")
     if self.content:
       self.refresh()
 
   def end(self):
+    self.refresh(cursor=False)
     self.live.stop()
 
-  def refresh(self):
-    markdown = Markdown(textify_markdown_code_blocks(self.content))
+  def refresh(self, cursor=True):
+    # De-stylize any code blocks in markdown,
+    # to differentiate from our Code Blocks
+    content = textify_markdown_code_blocks(self.content)
+    
+    if cursor:
+      content += "█"
+      
+    markdown = Markdown(content)
     panel = Panel(markdown, box=MINIMAL)
     self.live.update(panel)
     self.live.refresh()
 
 
 def textify_markdown_code_blocks(text):
   """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `open_interpreter-0.0.270/interpreter/system_message.txt` & `open_interpreter-0.0.271/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/interpreter/utils.py` & `open_interpreter-0.0.271/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.270/pyproject.toml` & `open_interpreter-0.0.271/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.270"
+version = "0.0.271"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.270/PKG-INFO` & `open_interpreter-0.0.271/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.270
+Version: 0.0.271
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

