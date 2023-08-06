# Comparing `tmp/open_interpreter-0.0.251.tar.gz` & `tmp/open_interpreter-0.0.252.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.251.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.252.tar", max compression
```

## Comparing `open_interpreter-0.0.251.tar` & `open_interpreter-0.0.252.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.251/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.251/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.251/interpreter/__init__.py
--rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.251/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.251/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.251/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12104 2023-08-06 08:59:49.792515 open_interpreter-0.0.251/interpreter/interpreter.py
--rw-r--r--   0        0        0     1313 2023-08-06 08:57:47.868669 open_interpreter-0.0.251/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.251/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.251/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.251/interpreter/utils.py
--rw-r--r--   0        0        0      585 2023-08-06 09:10:01.981914 open_interpreter-0.0.251/pyproject.toml
--rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.251/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.252/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.252/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.252/interpreter/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.252/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.252/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.252/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12039 2023-08-06 09:11:34.948517 open_interpreter-0.0.252/interpreter/interpreter.py
+-rw-r--r--   0        0        0     1313 2023-08-06 08:57:47.868669 open_interpreter-0.0.252/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.252/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.252/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.252/interpreter/utils.py
+-rw-r--r--   0        0        0      585 2023-08-06 09:11:45.937298 open_interpreter-0.0.252/pyproject.toml
+-rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.252/PKG-INFO
```

### Comparing `open_interpreter-0.0.251/LICENSE` & `open_interpreter-0.0.252/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/README.md` & `open_interpreter-0.0.252/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/__init__.py` & `open_interpreter-0.0.252/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/cli.py` & `open_interpreter-0.0.252/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/code_block.py` & `open_interpreter-0.0.252/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/code_interpreter.py` & `open_interpreter-0.0.252/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/interpreter.py` & `open_interpreter-0.0.252/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,16 @@
     self.messages = []
     self.temperature = 0.01
     self.api_key = None
     self.auto_run = False
     self.local = False
 
     # Get default system message
-    # here = os.path.abspath(os.path.dirname(__file__))
-    # with open(os.path.join(here, 'system_message.txt'), 'r') as f:
-    with open('./interpreter/system_message.txt', 'r') as f:
+    here = os.path.abspath(os.path.dirname(__file__))
+    with open(os.path.join(here, 'system_message.txt'), 'r') as f:
       self.system_message = f.read().strip()
 
     # Store Code Interpreter instances for each language
     self.code_interpreters = {}
 
     # No active block to start
     # (blocks are visual representation of messages on the terminal)
```

### Comparing `open_interpreter-0.0.251/interpreter/llama_2.py` & `open_interpreter-0.0.252/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/message_block.py` & `open_interpreter-0.0.252/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/system_message.txt` & `open_interpreter-0.0.252/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/interpreter/utils.py` & `open_interpreter-0.0.252/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.251/pyproject.toml` & `open_interpreter-0.0.252/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.251"
+version = "0.0.252"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.251/PKG-INFO` & `open_interpreter-0.0.252/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.251
+Version: 0.0.252
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

