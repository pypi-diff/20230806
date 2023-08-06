# Comparing `tmp/trilium_alchemy-0.1.0.tar.gz` & `tmp/trilium_alchemy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trilium_alchemy-0.1.0.tar", max compression
+gzip compressed data, was "trilium_alchemy-0.1.1.tar", max compression
```

## Comparing `trilium_alchemy-0.1.0.tar` & `trilium_alchemy-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0    34523 2023-08-06 08:10:58.000000 trilium_alchemy-0.1.0/LICENSE
--rwxr-xr-x   0        0        0      146 2023-08-06 08:21:03.000000 trilium_alchemy-0.1.0/README.md
--rwxr-xr-x   0        0        0      873 2023-08-06 08:13:24.000000 trilium_alchemy-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      312 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.0/trilium_alchemy/__init__.py
--rwxr-xr-x   0        0        0      809 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.0/trilium_alchemy/_rollup.py
--rwxr-xr-x   0        0        0     1169 2023-08-05 02:10:57.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/__init__.py
--rwxr-xr-x   0        0        0      275 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/__init__.py
--rwxr-xr-x   0        0        0     9643 2023-08-05 02:12:24.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/attribute.py
--rwxr-xr-x   0        0        0     1740 2023-08-05 01:06:30.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/label.py
--rwxr-xr-x   0        0        0     3194 2023-08-05 05:53:46.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/relation.py
--rwxr-xr-x   0        0        0      103 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/branch/__init__.py
--rwxr-xr-x   0        0        0    12041 2023-08-05 07:43:52.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/branch/branch.py
--rwxr-xr-x   0        0        0     7103 2023-08-04 21:25:46.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/cache.py
--rwxr-xr-x   0        0        0     8185 2023-08-05 07:43:52.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/declarative.py
--rwxr-xr-x   0        0        0      135 2023-07-31 01:36:44.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/entity/__init__.py
--rwxr-xr-x   0        0        0    15818 2023-08-05 06:59:17.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/entity/entity.py
--rwxr-xr-x   0        0        0    17791 2023-08-05 01:02:01.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/entity/model.py
--rwxr-xr-x   0        0        0      510 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/entity/types.py
--rwxr-xr-x   0        0        0      861 2023-08-05 07:02:21.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/exceptions.py
--rwxr-xr-x   0        0        0      180 2023-08-02 17:01:44.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/__init__.py
--rwxr-xr-x   0        0        0    13837 2023-08-05 07:46:17.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/attributes.py
--rwxr-xr-x   0        0        0    12043 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/branches.py
--rwxr-xr-x   0        0        0     8215 2023-08-05 07:37:51.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/content.py
--rwxr-xr-x   0        0        0     8082 2023-08-05 17:45:57.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/extension.py
--rwxr-xr-x   0        0        0    42088 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/note/note.py
--rwxr-xr-x   0        0        0    19871 2023-08-06 04:28:20.000000 trilium_alchemy-0.1.0/trilium_alchemy/core/session.py
--rwxr-xr-x   0        0        0      335 2023-07-30 06:37:20.000000 trilium_alchemy-0.1.0/trilium_alchemy/ext/__init__.py
--rwxr-xr-x   0        0        0      157 2023-08-05 05:49:22.000000 trilium_alchemy-0.1.0/trilium_alchemy/ext/assets/system.css
--rwxr-xr-x   0        0        0     9728 2023-08-06 01:42:47.000000 trilium_alchemy-0.1.0/trilium_alchemy/ext/helpers.py
--rwxr-xr-x   0        0        0      651 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.0/trilium_alchemy/ext/types.py
--rwxr-xr-x   0        0        0      450 2023-07-30 06:37:20.000000 trilium_alchemy-0.1.0/trilium_alchemy/sync/__init__.py
--rwxr-xr-x   0        0        0     2171 2023-06-19 18:25:31.000000 trilium_alchemy-0.1.0/trilium_alchemy/sync/notes.txt
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 trilium_alchemy-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    34523 2023-08-06 08:10:58.000000 trilium_alchemy-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0      145 2023-08-06 08:42:55.000000 trilium_alchemy-0.1.1/README.md
+-rwxr-xr-x   0        0        0      873 2023-08-06 08:48:44.000000 trilium_alchemy-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      312 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.1/trilium_alchemy/__init__.py
+-rwxr-xr-x   0        0        0      809 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.1/trilium_alchemy/_rollup.py
+-rwxr-xr-x   0        0        0     1102 2023-08-06 08:46:34.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/__init__.py
+-rwxr-xr-x   0        0        0      275 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/__init__.py
+-rwxr-xr-x   0        0        0     9643 2023-08-05 02:12:24.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/attribute.py
+-rwxr-xr-x   0        0        0     1740 2023-08-05 01:06:30.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/label.py
+-rwxr-xr-x   0        0        0     3194 2023-08-05 05:53:46.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/relation.py
+-rwxr-xr-x   0        0        0      103 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/branch/__init__.py
+-rwxr-xr-x   0        0        0    12041 2023-08-05 07:43:52.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/branch/branch.py
+-rwxr-xr-x   0        0        0     7103 2023-08-04 21:25:46.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/cache.py
+-rwxr-xr-x   0        0        0     8185 2023-08-05 07:43:52.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/declarative.py
+-rwxr-xr-x   0        0        0      135 2023-07-31 01:36:44.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/entity/__init__.py
+-rwxr-xr-x   0        0        0    15818 2023-08-05 06:59:17.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/entity/entity.py
+-rwxr-xr-x   0        0        0    17791 2023-08-05 01:02:01.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/entity/model.py
+-rwxr-xr-x   0        0        0      510 2023-07-30 06:37:19.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/entity/types.py
+-rwxr-xr-x   0        0        0      861 2023-08-05 07:02:21.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/exceptions.py
+-rwxr-xr-x   0        0        0      180 2023-08-02 17:01:44.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/__init__.py
+-rwxr-xr-x   0        0        0    13837 2023-08-05 07:46:17.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/attributes.py
+-rwxr-xr-x   0        0        0    12043 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/branches.py
+-rwxr-xr-x   0        0        0     8215 2023-08-05 07:37:51.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/content.py
+-rwxr-xr-x   0        0        0     8082 2023-08-05 17:45:57.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/extension.py
+-rwxr-xr-x   0        0        0    42088 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/note/note.py
+-rwxr-xr-x   0        0        0    19961 2023-08-06 08:48:26.000000 trilium_alchemy-0.1.1/trilium_alchemy/core/session.py
+-rwxr-xr-x   0        0        0      335 2023-07-30 06:37:20.000000 trilium_alchemy-0.1.1/trilium_alchemy/ext/__init__.py
+-rwxr-xr-x   0        0        0      157 2023-08-05 05:49:22.000000 trilium_alchemy-0.1.1/trilium_alchemy/ext/assets/system.css
+-rwxr-xr-x   0        0        0     9728 2023-08-06 01:42:47.000000 trilium_alchemy-0.1.1/trilium_alchemy/ext/helpers.py
+-rwxr-xr-x   0        0        0      651 2023-08-06 08:02:21.000000 trilium_alchemy-0.1.1/trilium_alchemy/ext/types.py
+-rwxr-xr-x   0        0        0      450 2023-07-30 06:37:20.000000 trilium_alchemy-0.1.1/trilium_alchemy/sync/__init__.py
+-rwxr-xr-x   0        0        0     2171 2023-06-19 18:25:31.000000 trilium_alchemy-0.1.1/trilium_alchemy/sync/notes.txt
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 trilium_alchemy-0.1.1/PKG-INFO
```

### Comparing `trilium_alchemy-0.1.0/LICENSE` & `trilium_alchemy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/pyproject.toml` & `trilium_alchemy-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project.urls]
 "Homepage" = "https://github.com/mm21/trilium-alchemy"
 
 [tool.poetry]
 name = "trilium-alchemy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python SDK and CLI toolkit for Trilium Notes"
 authors = ["mm21 <mm21.apps@gmail.com>"]
 readme = "README.md"
 packages = [{include = "trilium_alchemy"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/_rollup.py` & `trilium_alchemy-0.1.1/trilium_alchemy/_rollup.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/__init__.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 This module implements ORM access to Trilium and fundamental note capabilities.
 
-For a discussion of ORM concepts as applied here, see TODO_DOC.
-
 Examples in this module assume you have created a {obj}`Session`
 and that you will either invoke {obj}`Session.flush` or use a context manager
 to commit the changes.
 
 For example:
 
 ```
```

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/attribute.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/attribute.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/label.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/label.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/attribute/relation.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/attribute/relation.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/branch/branch.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/branch/branch.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/cache.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/cache.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/declarative.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/declarative.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/entity/entity.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/entity/entity.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/entity/model.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/entity/model.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/exceptions.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/note/attributes.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/note/attributes.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/note/branches.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/note/branches.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/note/content.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/note/content.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/note/extension.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/note/extension.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/note/note.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/note/note.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/core/session.py` & `trilium_alchemy-0.1.1/trilium_alchemy/core/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
         (identified with `#inbox` label) or a day note in a journal.
 
         :param date: Date object, e.g. `datetime.date(2023, 7, 5)`{l=python}
         """
 
     def get_app_info(self) -> AppInfo:
         """
-        Returns app info. See TODO_DOC for its definition.
+        Returns app info. See <https://github.com/mm21/trilium-client/blob/main/docs/AppInfo.md> for its definition.
         """
 
         app_info: AppInfo = self.api.get_app_info()
         return app_info
 
     def refresh_note_ordering(
         self, note: trilium_alchemy.core.note.Note
@@ -553,15 +553,15 @@
         """
         return self._host
 
     @property
     def api(self) -> DefaultApi:
         """
         ETAPI client object. Used internally and exposed for manual
-        low-level operations. For its documentation, see: TODO_DOC
+        low-level operations. For its documentation, see: <https://github.com/mm21/trilium-client>
         """
         assert self._api is not None
         return self._api
 
     @property
     def _base_path(self) -> str:
         """
```

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/ext/helpers.py` & `trilium_alchemy-0.1.1/trilium_alchemy/ext/helpers.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/ext/types.py` & `trilium_alchemy-0.1.1/trilium_alchemy/ext/types.py`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/trilium_alchemy/sync/notes.txt` & `trilium_alchemy-0.1.1/trilium_alchemy/sync/notes.txt`

 * *Files identical despite different names*

### Comparing `trilium_alchemy-0.1.0/PKG-INFO` & `trilium_alchemy-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: trilium-alchemy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK and CLI toolkit for Trilium Notes
 Author: mm21
 Author-email: mm21.apps@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: trilium-client (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # trilium-alchemy
 Python SDK and CLI toolkit for Trilium Notes.
 
-Work in progress. Read the docs here: <https://mm21.github.com/trilium-alchemy/>
+Work in progress. Read the docs here: <https://mm21.github.io/trilium-alchemy/>
```

