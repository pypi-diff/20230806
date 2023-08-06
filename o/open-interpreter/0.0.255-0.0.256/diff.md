# Comparing `tmp/open_interpreter-0.0.255.tar.gz` & `tmp/open_interpreter-0.0.256.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.255.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.256.tar", max compression
```

## Comparing `open_interpreter-0.0.255.tar` & `open_interpreter-0.0.256.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.255/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.255/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.255/interpreter/__init__.py
--rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.255/interpreter/cli.py
--rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.255/interpreter/code_block.py
--rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.255/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    12059 2023-08-06 16:14:38.673244 open_interpreter-0.0.255/interpreter/interpreter.py
--rw-r--r--   0        0        0     2361 2023-08-06 18:04:51.788458 open_interpreter-0.0.255/interpreter/llama_2.py
--rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.255/interpreter/message_block.py
--rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.255/interpreter/system_message.txt
--rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.255/interpreter/utils.py
--rw-r--r--   0        0        0      585 2023-08-06 18:05:30.263176 open_interpreter-0.0.255/pyproject.toml
--rw-r--r--   0        0        0     7060 1970-01-01 00:00:00.000000 open_interpreter-0.0.255/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.256/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.256/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.256/interpreter/__init__.py
+-rw-r--r--   0        0        0     1080 2023-08-06 08:59:25.744545 open_interpreter-0.0.256/interpreter/cli.py
+-rw-r--r--   0        0        0     2515 2023-08-06 01:41:46.229915 open_interpreter-0.0.256/interpreter/code_block.py
+-rw-r--r--   0        0        0     7423 2023-08-06 01:15:32.535448 open_interpreter-0.0.256/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    12059 2023-08-06 16:14:38.673244 open_interpreter-0.0.256/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2361 2023-08-06 18:04:51.788458 open_interpreter-0.0.256/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1296 2023-08-06 05:21:08.025713 open_interpreter-0.0.256/interpreter/message_block.py
+-rw-r--r--   0        0        0     1480 2023-08-06 05:39:41.771321 open_interpreter-0.0.256/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3376 2023-08-06 04:36:54.894699 open_interpreter-0.0.256/interpreter/utils.py
+-rw-r--r--   0        0        0      604 2023-08-06 18:07:35.007990 open_interpreter-0.0.256/pyproject.toml
+-rw-r--r--   0        0        0     7100 1970-01-01 00:00:00.000000 open_interpreter-0.0.256/PKG-INFO
```

### Comparing `open_interpreter-0.0.255/LICENSE` & `open_interpreter-0.0.256/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/README.md` & `open_interpreter-0.0.256/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/__init__.py` & `open_interpreter-0.0.256/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/cli.py` & `open_interpreter-0.0.256/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/code_block.py` & `open_interpreter-0.0.256/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/code_interpreter.py` & `open_interpreter-0.0.256/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/interpreter.py` & `open_interpreter-0.0.256/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/llama_2.py` & `open_interpreter-0.0.256/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/message_block.py` & `open_interpreter-0.0.256/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/system_message.txt` & `open_interpreter-0.0.256/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/interpreter/utils.py` & `open_interpreter-0.0.256/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.255/pyproject.toml` & `open_interpreter-0.0.256/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.255"
+version = "0.0.256"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
 ipython = "^8.14.0"
 astor = "^0.8.1"
 git-python = "^1.0.3"
 tokentrim = "^0.1.2"
+appdirs = "^1.4.4"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `open_interpreter-0.0.255/PKG-INFO` & `open_interpreter-0.0.256/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.255
+Version: 0.0.256
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: git-python (>=1.0.3,<2.0.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tokentrim (>=0.1.2,<0.2.0)
```

