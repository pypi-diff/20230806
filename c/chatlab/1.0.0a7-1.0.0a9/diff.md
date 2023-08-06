# Comparing `tmp/chatlab-1.0.0a7.tar.gz` & `tmp/chatlab-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-1.0.0a7.tar", max compression
+gzip compressed data, was "chatlab-1.0.0a9.tar", max compression
```

## Comparing `chatlab-1.0.0a7.tar` & `chatlab-1.0.0a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1504 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     6009 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/README.md
--rw-r--r--   0        0        0     2324 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/__init__.py
--rw-r--r--   0        0        0       30 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/_version.py
--rw-r--r--   0        0        0      407 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/__init__.py
--rw-r--r--   0        0        0     7628 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/noteable.py
--rw-r--r--   0        0        0     8330 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/builtins/python.py
--rw-r--r--   0        0        0    14242 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/conversation.py
--rw-r--r--   0        0        0     2358 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/decorators.py
--rw-r--r--   0        0        0     8006 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/display.py
--rw-r--r--   0        0        0      114 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/errors.py
--rw-r--r--   0        0        0     3304 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/markdown.py
--rw-r--r--   0        0        0     3290 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/messaging.py
--rw-r--r--   0        0        0     1869 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/models.py
--rw-r--r--   0        0        0      174 2023-07-25 14:05:00.801150 chatlab-1.0.0a7/chatlab/prompts.py
--rw-r--r--   0        0        0     8158 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/chatlab/registry.py
--rw-r--r--   0        0        0     2814 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/__init__.py
--rw-r--r--   0        0        0      357 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_chatlab.py
--rw-r--r--   0        0        0     1103 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_decorators.py
--rw-r--r--   0        0        0     1066 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_messaging.py
--rw-r--r--   0        0        0     6052 2023-07-25 14:05:00.805150 chatlab-1.0.0a7/tests/test_registry.py
--rw-r--r--   0        0        0     7703 1970-01-01 00:00:00.000000 chatlab-1.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     6009 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/README.md
+-rw-r--r--   0        0        0     2324 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/_version.py
+-rw-r--r--   0        0        0      407 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/builtins/__init__.py
+-rw-r--r--   0        0        0     7958 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/builtins/noteable.py
+-rw-r--r--   0        0        0     8330 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/builtins/python.py
+-rw-r--r--   0        0        0    14242 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/conversation.py
+-rw-r--r--   0        0        0     2358 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/decorators.py
+-rw-r--r--   0        0        0     8006 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/models.py
+-rw-r--r--   0        0        0      174 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/prompts.py
+-rw-r--r--   0        0        0     8158 2023-07-25 14:40:37.559203 chatlab-1.0.0a9/chatlab/registry.py
+-rw-r--r--   0        0        0     2814 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/tests/test_messaging.py
+-rw-r--r--   0        0        0     6052 2023-07-25 14:40:37.563203 chatlab-1.0.0a9/tests/test_registry.py
+-rw-r--r--   0        0        0     7703 1970-01-01 00:00:00.000000 chatlab-1.0.0a9/PKG-INFO
```

### Comparing `chatlab-1.0.0a7/LICENSE` & `chatlab-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/README.md` & `chatlab-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/__init__.py` & `chatlab-1.0.0a9/chatlab/__init__.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/builtins/noteable.py` & `chatlab-1.0.0a9/chatlab/builtins/noteable.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,21 +105,30 @@
             existing_cells = rtu_client.cell_ids
             if existing_cells and len(existing_cells) > 0:
                 after_cell_id = existing_cells[-1]
 
         if cell_id is None:
             cell_id = str(ulid.ULID())
 
+        cell = None
+
         if cell_type == "markdown":
-            cell = await rtu_client.add_cell(MarkdownCell(source=source, id=cell_id))
-            return cell
+            cell = MarkdownCell(source=source, id=cell_id)
+        elif cell_type == "code":
+            cell = CodeCell(source=source, id=cell_id)
+        elif cell_type == "sql":
+            cell = CodeCell(source=source, id=cell_id)
+            cell.metadata.update({"noteable": {"cell_type": "sql"}})
+
+        if cell is None:
+            return f"Unknown cell type {cell_type}. Valid types are: markdown, code, sql."
 
-        cell = await rtu_client.add_cell(CodeCell(source=source, id=cell_id), after_id=after_cell_id)
+        cell = await rtu_client.add_cell(cell, after_id=after_cell_id)
 
-        if not and_run:
+        if cell.cell_type != "code" or not and_run:
             return cell
 
         try:
             return await self.run_cell(cell.id)
         except Exception as e:
             return f"Cell created successfully. An error happened during run: {e}"
```

### Comparing `chatlab-1.0.0a7/chatlab/builtins/python.py` & `chatlab-1.0.0a9/chatlab/builtins/python.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/conversation.py` & `chatlab-1.0.0a9/chatlab/conversation.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/decorators.py` & `chatlab-1.0.0a9/chatlab/decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/display.py` & `chatlab-1.0.0a9/chatlab/display.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/markdown.py` & `chatlab-1.0.0a9/chatlab/markdown.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/messaging.py` & `chatlab-1.0.0a9/chatlab/messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/models.py` & `chatlab-1.0.0a9/chatlab/models.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/chatlab/registry.py` & `chatlab-1.0.0a9/chatlab/registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/pyproject.toml` & `chatlab-1.0.0a9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "1.0.0-alpha.7"
+version = "1.0.0-alpha.9"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 3 - Alpha',
```

### Comparing `chatlab-1.0.0a7/tests/test_decorators.py` & `chatlab-1.0.0a9/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/tests/test_messaging.py` & `chatlab-1.0.0a9/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/tests/test_registry.py` & `chatlab-1.0.0a9/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `chatlab-1.0.0a7/PKG-INFO` & `chatlab-1.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 1.0.0a7
+Version: 1.0.0a9
 Summary: Chat Plugin Experiments, Simplified. Create agents and give them superpowers in your notebooks.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 3 - Alpha
```

