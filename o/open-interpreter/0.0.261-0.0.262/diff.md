# Comparing `tmp/open_interpreter-0.0.261.tar.gz` & `tmp/open_interpreter-0.0.262.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.261.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.262.tar", max compression
```

## Comparing `open_interpreter-0.0.261.tar` & `open_interpreter-0.0.262.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.261/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.261/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.261/interpreter/__init__.py
--rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.261/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.261/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.261/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13028 2023-08-06 19:04:59.315343 open_interpreter-0.0.261/interpreter/interpreter.py
--rw-r--r--   0        0        0     2687 2023-08-06 19:01:37.109057 open_interpreter-0.0.261/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.261/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.261/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.261/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-06 19:05:11.020170 open_interpreter-0.0.261/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.261/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.262/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.262/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.262/interpreter/__init__.py
+-rw-r--r--   0        0        0      737 2023-08-06 18:27:43.697388 open_interpreter-0.0.262/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.262/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.262/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13028 2023-08-06 19:06:19.873034 open_interpreter-0.0.262/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2687 2023-08-06 19:01:37.109057 open_interpreter-0.0.262/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.262/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.262/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.262/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-06 19:06:26.833526 open_interpreter-0.0.262/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.262/PKG-INFO
```

### Comparing `open_interpreter-0.0.261/LICENSE` & `open_interpreter-0.0.262/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/README.md` & `open_interpreter-0.0.262/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/__init__.py` & `open_interpreter-0.0.262/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/cli.py` & `open_interpreter-0.0.262/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/code_block.py` & `open_interpreter-0.0.262/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/code_interpreter.py` & `open_interpreter-0.0.262/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/interpreter.py` & `open_interpreter-0.0.262/interpreter/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                          "gpt-3.5-turbo",
                          system_message=system_message),
         stream=True,
         temperature=self.temperature,
       )
       """
       response = self.llama_instance.create_chat_completion(
-        messages=[{"role": "system", "content": "You are an assistant."}, {"role": "user", "content", "Hello!"}],
+        messages=[{"role": "system", "content": "You are an assistant."}, {"role": "user", "content": "Hello!"}],
         stream=True,
         temperature=self.temperature,
       )
       print("DEBUG SENT RESPONSE")
       
 
     # Initialize message, function call trackers, and active block
```

### Comparing `open_interpreter-0.0.261/interpreter/llama_2.py` & `open_interpreter-0.0.262/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/message_block.py` & `open_interpreter-0.0.262/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/system_message.txt` & `open_interpreter-0.0.262/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/interpreter/utils.py` & `open_interpreter-0.0.262/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.261/pyproject.toml` & `open_interpreter-0.0.262/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.261"
+version = "0.0.262"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.261/PKG-INFO` & `open_interpreter-0.0.262/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.261
+Version: 0.0.262
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

