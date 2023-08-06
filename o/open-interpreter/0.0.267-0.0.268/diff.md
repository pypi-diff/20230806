# Comparing `tmp/open_interpreter-0.0.267.tar.gz` & `tmp/open_interpreter-0.0.268.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.267.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.268.tar", max compression
```

## Comparing `open_interpreter-0.0.267.tar` & `open_interpreter-0.0.268.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.267/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.267/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.267/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.267/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.267/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.267/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13275 2023-08-06 19:50:41.588826 open_interpreter-0.0.267/interpreter/interpreter.py
--rw-r--r--   0        0        0     2488 2023-08-06 19:45:25.135471 open_interpreter-0.0.267/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.267/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.267/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.267/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 19:50:48.237442 open_interpreter-0.0.267/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.267/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.268/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.268/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.268/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.268/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 19:53:28.336293 open_interpreter-0.0.268/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.268/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13275 2023-08-06 19:50:41.588826 open_interpreter-0.0.268/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2488 2023-08-06 19:45:25.135471 open_interpreter-0.0.268/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1323 2023-08-06 19:53:45.705905 open_interpreter-0.0.268/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.268/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.268/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 19:53:52.598544 open_interpreter-0.0.268/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.268/PKG-INFO
```

### Comparing `open_interpreter-0.0.267/LICENSE` & `open_interpreter-0.0.268/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/README.md` & `open_interpreter-0.0.268/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/__init__.py` & `open_interpreter-0.0.268/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/cli.py` & `open_interpreter-0.0.268/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/code_block.py` & `open_interpreter-0.0.268/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/code_interpreter.py` & `open_interpreter-0.0.268/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/interpreter.py` & `open_interpreter-0.0.268/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/llama_2.py` & `open_interpreter-0.0.268/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/message_block.py` & `open_interpreter-0.0.268/interpreter/message_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
   def __init__(self):
     self.live = Live(auto_refresh=False, console=Console())
     self.live.start()
     self.content = ""
 
   def update_from_message(self, message):
-    self.content = message.get("content")
-    self.refresh()
+    self.content = message.get("content", "")
+    if self.content:
+      self.refresh()
 
   def end(self):
     self.live.stop()
 
   def refresh(self):
     markdown = Markdown(textify_markdown_code_blocks(self.content))
     panel = Panel(markdown, box=MINIMAL)
```

### Comparing `open_interpreter-0.0.267/interpreter/system_message.txt` & `open_interpreter-0.0.268/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/interpreter/utils.py` & `open_interpreter-0.0.268/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.267/pyproject.toml` & `open_interpreter-0.0.268/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.267"
+version = "0.0.268"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.267/PKG-INFO` & `open_interpreter-0.0.268/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.267
+Version: 0.0.268
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

