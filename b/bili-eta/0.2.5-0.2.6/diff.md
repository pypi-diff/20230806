# Comparing `tmp/bili_eta-0.2.5.tar.gz` & `tmp/bili_eta-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili_eta-0.2.5.tar", max compression
+gzip compressed data, was "bili_eta-0.2.6.tar", max compression
```

## Comparing `bili_eta-0.2.5.tar` & `bili_eta-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.5/README.md
--rw-r--r--   0        0        0       80 2023-08-06 11:04:35.152398 bili_eta-0.2.5/bili_eta/.env.prod
--rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.5/bili_eta/__init__.py
--rw-r--r--   0        0        0     1000 2023-07-30 14:24:12.062711 bili_eta-0.2.5/bili_eta/__main__.py
--rw-r--r--   0        0        0      281 2023-08-06 11:05:28.059962 bili_eta-0.2.5/bili_eta/bot.py
--rw-r--r--   0        0        0      363 2023-08-06 11:04:35.884392 bili_eta-0.2.5/bili_eta/plugins/__pycache__/new.cpython-310.pyc
--rw-r--r--   0        0        0      214 2023-07-30 14:37:06.096555 bili_eta-0.2.5/bili_eta/plugins/new.py
--rw-r--r--   0        0        0      562 2023-08-06 11:05:57.115731 bili_eta-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.6/README.md
+-rw-r--r--   0        0        0       80 2023-08-06 11:04:35.152398 bili_eta-0.2.6/bili_eta/.env.prod
+-rw-r--r--   0        0        0        0 2023-07-30 08:24:01.466868 bili_eta-0.2.6/bili_eta/__init__.py
+-rw-r--r--   0        0        0     1001 2023-08-06 11:09:09.170333 bili_eta-0.2.6/bili_eta/__main__.py
+-rw-r--r--   0        0        0      281 2023-08-06 11:05:28.059962 bili_eta-0.2.6/bili_eta/bot.py
+-rw-r--r--   0        0        0      363 2023-08-06 11:04:35.884392 bili_eta-0.2.6/bili_eta/plugins/__pycache__/new.cpython-310.pyc
+-rw-r--r--   0        0        0      214 2023-07-30 14:37:06.096555 bili_eta-0.2.6/bili_eta/plugins/new.py
+-rw-r--r--   0        0        0      562 2023-08-06 11:09:12.002313 bili_eta-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 bili_eta-0.2.6/PKG-INFO
```

### Comparing `bili_eta-0.2.5/bili_eta/__main__.py` & `bili_eta-0.2.6/bili_eta/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pass
 
 
 @click.command()
 def start():
     creat_config()
     creat_plugins_dir()
-    from bot import run
+    from .bot import run
     run()
 
 
 main.add_command(start)
 
 
 def creat_config():
```

### Comparing `bili_eta-0.2.5/pyproject.toml` & `bili_eta-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bili-eta"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["Polyisoprene <lzxder@outlook.com>"]
 readme = "README.md"
 packages = [{include = "bili_eta"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `bili_eta-0.2.5/PKG-INFO` & `bili_eta-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-eta
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: Polyisoprene
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

