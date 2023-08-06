# Comparing `tmp/loggingx-py-0.3.1.tar.gz` & `tmp/loggingx-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingx-py-0.3.1.tar", last modified: Fri Jul 21 10:54:01 2023, max compression
+gzip compressed data, was "loggingx-py-0.4.0.tar", last modified: Sun Aug  6 15:49:19 2023, max compression
```

## Comparing `loggingx-py-0.3.1.tar` & `loggingx-py-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.598028 loggingx-py-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.598028 loggingx-py-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/.tool-versions
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/loggingx/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/loggingx/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/loggingx_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 10:54:01.000000 loggingx-py-0.3.1/loggingx_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    78091 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)    22624 2023-07-21 10:53:42.000000 loggingx-py-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:54:01.602028 loggingx-py-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:19.853136 loggingx-py-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:19.849136 loggingx-py-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:19.849136 loggingx-py-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-06 15:49:19.853136 loggingx-py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:19.853136 loggingx-py-0.4.0/loggingx/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/loggingx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:49:19.853136 loggingx-py-0.4.0/loggingx_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-08-06 15:49:19.000000 loggingx-py-0.4.0/loggingx_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 15:49:19.000000 loggingx-py-0.4.0/loggingx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:49:19.000000 loggingx-py-0.4.0/loggingx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:49:19.000000 loggingx-py-0.4.0/loggingx_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 15:49:19.000000 loggingx-py-0.4.0/loggingx_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78091 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-08-06 15:49:01.000000 loggingx-py-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 15:49:19.853136 loggingx-py-0.4.0/setup.cfg
```

### Comparing `loggingx-py-0.3.1/.github/workflows/publish.yaml` & `loggingx-py-0.4.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/.gitignore` & `loggingx-py-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/LICENSE` & `loggingx-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/PKG-INFO` & `loggingx-py-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: loggingx-py
-Version: 0.3.1
-Summary: Helper for Contextual and Structured Logging in Python with logging
+Version: 0.4.0
+Summary: Drop-in replacement for Python's built-in `logging` module
 Author-email: Hyeonki Hong <hhk7734@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hyeonki Hong <hhk7734@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,45 +40,53 @@
 python3 -m pip install loggingx-py
 ```
 
 ### Additional Format
 
 - https://docs.python.org/3/library/logging.html#logrecord-attributes
 
-| Attribute name | Format | Description |
-| --- | --- | --- |
-| caller | %(caller)s | Caller(`<pathname>:<lineno>`) |
-| ctxFields | %(ctxFields)s | Context fields |
+| Attribute name | Format        | Description                   |
+| -------------- | ------------- | ----------------------------- |
+| caller         | %(caller)s    | Caller(`<pathname>:<lineno>`) |
+| ctxFields      | %(ctxFields)s | Context fields                |
+
+### Optimization
+
+| Configuration                | Description                                                    |
+| ---------------------------- | -------------------------------------------------------------- |
+| `logging.logThreads`         | If `False`, Record will not collect `thread` and `threadName`. |
+| `logging.logProcesses`       | If `False`, Record will not collect `process`.                 |
+| `logging.logMultiprocessing` | If `False`, Record will not collect `processName`.             |
 
 
 ### Context
 
 ```python
-import loggingx
+import loggingx as logging
 
-loggingx.basicConfig(
-    level=loggingx.INFO,
+logging.basicConfig(
+    level=logging.INFO,
     format="%(asctime)s\t%(levelname)s\t%(caller)s\t%(message)s\t%(ctxFields)s",
 )
 
 
 def A() -> None:
-    loggingx.info("A")
-    with loggingx.addFields(A="a"):
+    logging.info("A")
+    with logging.addFields(A="a"):
         B()
 
 
 def B() -> None:
-    loggingx.info("B")
-    with loggingx.addFields(B="b"):
+    logging.info("B")
+    with logging.addFields(B="b"):
         C()
 
 
 def C() -> None:
-    loggingx.info("C")
+    logging.info("C")
 
 
 if __name__ == "__main__":
     A()
 ```
 
 ```shell
@@ -86,23 +94,23 @@
 2023-07-19 01:15:33,981 INFO    loggingx.py/main.py:16  B       {'A': 'a'}
 2023-07-19 01:15:33,982 INFO    loggingx.py/main.py:22  C       {'A': 'a', 'B': 'b'}
 ```
 
 ### JSONFormatter
 
 ```python
-import loggingx
+import loggingx as logging
 
-handler = loggingx.StreamHandler()
-handler.setFormatter(loggingx.JSONFormatter())
-loggingx.basicConfig(level=loggingx.INFO, handlers=[handler])
+handler = logging.StreamHandler()
+handler.setFormatter(logging.JSONFormatter())
+logging.basicConfig(level=logging.INFO, handlers=[handler])
 
 if __name__ == "__main__":
-    with loggingx.addFields(ctx="ctx"):
-        loggingx.info("test", extra={"extra": "extra"})
+    with logging.addFields(ctx="ctx"):
+        logging.info("test", extra={"extra": "extra"})
 ```
 
 ```json
 {"time": 1689697694.9980711, "level": "info", "caller": "loggingx.py/main.py:9", "msg": "test", "ctx": "ctx", "extra": "extra"}
 ```
 
 ### With `logging`
```

### Comparing `loggingx-py-0.3.1/loggingx/context.py` & `loggingx-py-0.4.0/loggingx/context.py`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/loggingx/formatter.py` & `loggingx-py-0.4.0/loggingx/formatter.py`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/loggingx_py.egg-info/PKG-INFO` & `loggingx-py-0.4.0/loggingx_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: loggingx-py
-Version: 0.3.1
-Summary: Helper for Contextual and Structured Logging in Python with logging
+Version: 0.4.0
+Summary: Drop-in replacement for Python's built-in `logging` module
 Author-email: Hyeonki Hong <hhk7734@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hyeonki Hong <hhk7734@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -40,45 +40,53 @@
 python3 -m pip install loggingx-py
 ```
 
 ### Additional Format
 
 - https://docs.python.org/3/library/logging.html#logrecord-attributes
 
-| Attribute name | Format | Description |
-| --- | --- | --- |
-| caller | %(caller)s | Caller(`<pathname>:<lineno>`) |
-| ctxFields | %(ctxFields)s | Context fields |
+| Attribute name | Format        | Description                   |
+| -------------- | ------------- | ----------------------------- |
+| caller         | %(caller)s    | Caller(`<pathname>:<lineno>`) |
+| ctxFields      | %(ctxFields)s | Context fields                |
+
+### Optimization
+
+| Configuration                | Description                                                    |
+| ---------------------------- | -------------------------------------------------------------- |
+| `logging.logThreads`         | If `False`, Record will not collect `thread` and `threadName`. |
+| `logging.logProcesses`       | If `False`, Record will not collect `process`.                 |
+| `logging.logMultiprocessing` | If `False`, Record will not collect `processName`.             |
 
 
 ### Context
 
 ```python
-import loggingx
+import loggingx as logging
 
-loggingx.basicConfig(
-    level=loggingx.INFO,
+logging.basicConfig(
+    level=logging.INFO,
     format="%(asctime)s\t%(levelname)s\t%(caller)s\t%(message)s\t%(ctxFields)s",
 )
 
 
 def A() -> None:
-    loggingx.info("A")
-    with loggingx.addFields(A="a"):
+    logging.info("A")
+    with logging.addFields(A="a"):
         B()
 
 
 def B() -> None:
-    loggingx.info("B")
-    with loggingx.addFields(B="b"):
+    logging.info("B")
+    with logging.addFields(B="b"):
         C()
 
 
 def C() -> None:
-    loggingx.info("C")
+    logging.info("C")
 
 
 if __name__ == "__main__":
     A()
 ```
 
 ```shell
@@ -86,23 +94,23 @@
 2023-07-19 01:15:33,981 INFO    loggingx.py/main.py:16  B       {'A': 'a'}
 2023-07-19 01:15:33,982 INFO    loggingx.py/main.py:22  C       {'A': 'a', 'B': 'b'}
 ```
 
 ### JSONFormatter
 
 ```python
-import loggingx
+import loggingx as logging
 
-handler = loggingx.StreamHandler()
-handler.setFormatter(loggingx.JSONFormatter())
-loggingx.basicConfig(level=loggingx.INFO, handlers=[handler])
+handler = logging.StreamHandler()
+handler.setFormatter(logging.JSONFormatter())
+logging.basicConfig(level=logging.INFO, handlers=[handler])
 
 if __name__ == "__main__":
-    with loggingx.addFields(ctx="ctx"):
-        loggingx.info("test", extra={"extra": "extra"})
+    with logging.addFields(ctx="ctx"):
+        logging.info("test", extra={"extra": "extra"})
 ```
 
 ```json
 {"time": 1689697694.9980711, "level": "info", "caller": "loggingx.py/main.py:9", "msg": "test", "ctx": "ctx", "extra": "extra"}
 ```
 
 ### With `logging`
```

### Comparing `loggingx-py-0.3.1/poetry.lock` & `loggingx-py-0.4.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `loggingx-py-0.3.1/pyproject.toml` & `loggingx-py-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "loggingx-py"
-description = "Helper for Contextual and Structured Logging in Python with logging"
+description = "Drop-in replacement for Python's built-in `logging` module"
 authors = [{ name = "Hyeonki Hong", email = "hhk7734@gmail.com" }]
 requires-python = ">=3.10,<4.0"
 
 dynamic = ["version"]
 
 license = { file = "LICENSE" }
 readme = "README.md"
@@ -19,16 +19,22 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
+[tool.setuptools]
+zip-safe = false
+
+[tool.setuptools.package-data]
+"*" = ["py.typed", "*.pyi"]
+
 [tool.setuptools.packages.find]
-include = ["loggingx"]
+include = ["loggingx", "loggingx.*"]
 
 [tool.poetry]
 name = "loggingx-py"
 version = "0"
 description = ""
 authors = ["Hyeonki Hong <hhk7734@gmail.com>"]
```

