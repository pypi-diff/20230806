# Comparing `tmp/open_interpreter-0.0.263.tar.gz` & `tmp/open_interpreter-0.0.264.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.263.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.264.tar", max compression
```

## Comparing `open_interpreter-0.0.263.tar` & `open_interpreter-0.0.264.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.263/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.263/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.263/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.263/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.263/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.263/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13049 2023-08-06 19:27:18.202645 open_interpreter-0.0.263/interpreter/interpreter.py
--rw-r--r--   0        0        0     2629 2023-08-06 19:24:48.944799 open_interpreter-0.0.263/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.263/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.263/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.263/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 19:28:03.470844 open_interpreter-0.0.263/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.263/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.264/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.264/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.264/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.264/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.264/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.264/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13049 2023-08-06 19:27:18.202645 open_interpreter-0.0.264/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2630 2023-08-06 19:37:43.284629 open_interpreter-0.0.264/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.264/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.264/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.264/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 19:37:37.140059 open_interpreter-0.0.264/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.264/PKG-INFO
```

### Comparing `open_interpreter-0.0.263/LICENSE` & `open_interpreter-0.0.264/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/README.md` & `open_interpreter-0.0.264/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/__init__.py` & `open_interpreter-0.0.264/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/cli.py` & `open_interpreter-0.0.264/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/code_block.py` & `open_interpreter-0.0.264/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/code_interpreter.py` & `open_interpreter-0.0.264/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/interpreter.py` & `open_interpreter-0.0.264/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/llama_2.py` & `open_interpreter-0.0.264/interpreter/llama_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,12 +64,12 @@
         else:
             print('', "Installation cancelled. Exiting.", '')
             return None
 
     # Initialize and return Llama-2
     # Redirect its output into a fire because this prints a billion things
     print("DEBUG 1")
-    with contextlib.redirect_sterr(None):  
+    with contextlib.redirect_stderr(None):  
         print("DEBUG 2")
         llama_2 = Llama(model_path=model_path)
     print("DEBUG 3")
     return llama_2
```

### Comparing `open_interpreter-0.0.263/interpreter/message_block.py` & `open_interpreter-0.0.264/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/system_message.txt` & `open_interpreter-0.0.264/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/interpreter/utils.py` & `open_interpreter-0.0.264/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.263/pyproject.toml` & `open_interpreter-0.0.264/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.263"
+version = "0.0.264"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.263/PKG-INFO` & `open_interpreter-0.0.264/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.263
+Version: 0.0.264
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

