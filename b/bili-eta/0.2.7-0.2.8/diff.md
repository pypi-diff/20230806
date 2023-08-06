# Comparing `tmp/bili_eta-0.2.7.tar.gz` & `tmp/bili_eta-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.2.7.tar", max compression
+gzip compressed data, was "bili_eta-0.2.8.tar", max compression
```

## Comparing `bili_eta-0.2.7.tar` & `bili_eta-0.2.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.7/README.md
--rw-r--r--   0        0        0       80 2023-08-06 11:04:35.152398 bili_eta-0.2.7/bili_eta/.env.prod
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.7/bili_eta/__init__.py
--rw-r--r--   0        0        0     1000 2023-08-06 11:11:16.213506 bili_eta-0.2.7/bili_eta/__main__.py
--rw-r--r--   0        0        0      275 2023-08-06 11:11:04.677579 bili_eta-0.2.7/bili_eta/bot.py
--rw-r--r--   0        0        0      363 2023-08-06 11:04:35.884392 bili_eta-0.2.7/bili_eta/plugins/__pycache__/new.cpython-310.pyc
--rw-r--r--   0        0        0      214 2023-07-30 14:37:06.096555 bili_eta-0.2.7/bili_eta/plugins/new.py
--rw-r--r--   0        0        0      562 2023-08-06 11:12:07.673189 bili_eta-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.8/README.md
+-rw-r--r--   0        0        0       80 2023-08-06 11:04:35.152398 bili_eta-0.2.8/bili_eta/.env.prod
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.8/bili_eta/__init__.py
+-rw-r--r--   0        0        0     1020 2023-08-06 11:14:46.064263 bili_eta-0.2.8/bili_eta/__main__.py
+-rw-r--r--   0        0        0      279 2023-08-06 11:14:26.916371 bili_eta-0.2.8/bili_eta/bot.py
+-rw-r--r--   0        0        0      363 2023-08-06 11:04:35.884392 bili_eta-0.2.8/bili_eta/plugins/__pycache__/new.cpython-310.pyc
+-rw-r--r--   0        0        0      214 2023-07-30 14:37:06.096555 bili_eta-0.2.8/bili_eta/plugins/new.py
+-rw-r--r--   0        0        0      562 2023-08-06 11:15:05.884152 bili_eta-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.8/PKG-INFO
```

### Comparing `bili_eta-0.2.7/bili_eta/__main__.py` & `bili_eta-0.2.8/bili_eta/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import click
-from os import path, getcwd,mkdir,listdir
+from os import path, getcwd,mkdir
 import dotenv
+import nonebot
+from .bot import app
+
 
 env = {
     'HOST':'127.0.0.1',
     'PORT': '8080',
     'SUPERUSERS': [],
     'DynTextFont':'',
     'DynEmojiFont':'',
@@ -18,16 +21,15 @@
     pass
 
 
 @click.command()
 def start():
     creat_config()
     creat_plugins_dir()
-    from bot import run
-    run()
+    nonebot.run(app=app)
 
 
 main.add_command(start)
 
 
 def creat_config():
     env_file_path = path.join(getcwd(), ".env.prod")
```

### Comparing `bili_eta-0.2.7/pyproject.toml` & `bili_eta-0.2.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bili_eta-0.2.7/PKG-INFO` & `bili_eta-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

