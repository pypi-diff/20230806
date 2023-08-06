# Comparing `tmp/multilogue-0.0.8.tar.gz` & `tmp/multilogue-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.8.tar", last modified: Fri Aug  4 19:46:08 2023, max compression
+gzip compressed data, was "multilogue-0.0.9.tar", last modified: Sun Aug  6 01:38:16 2023, max compression
```

## Comparing `multilogue-0.0.8.tar` & `multilogue-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.8/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-04 19:46:08.600914 multilogue-0.0.8/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      119 2023-08-04 19:43:07.000000 multilogue-0.0.8/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      833 2023-08-04 19:43:58.000000 multilogue-0.0.8/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-08-04 19:46:08.600914 multilogue-0.0.8/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.596914 multilogue-0.0.8/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.596914 multilogue-0.0.8/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.8/src/multilogue/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.8/src/multilogue/entities.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.8/src/multilogue/participants.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/src/multilogue/utilities/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      439 2023-07-30 22:20:03.000000 multilogue-0.0.8/src/multilogue/utilities/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1849 2023-07-30 22:14:48.000000 multilogue-0.0.8/src/multilogue/utilities/chatgpt.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4562 2023-08-04 19:38:14.000000 multilogue-0.0.8/src/multilogue/utilities/githublog.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      440 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       49 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.8/tests/test_entities.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.9/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-06 01:38:16.774352 multilogue-0.0.9/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      119 2023-08-04 19:43:07.000000 multilogue-0.0.9/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      833 2023-08-06 01:37:11.000000 multilogue-0.0.9/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-08-06 01:38:16.774352 multilogue-0.0.9/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.9/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1863 2023-08-05 14:15:14.000000 multilogue-0.0.9/src/multilogue/entities.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4188 2023-08-05 14:15:14.000000 multilogue-0.0.9/src/multilogue/participants.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/src/multilogue/utilities/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      419 2023-08-06 00:26:18.000000 multilogue-0.0.9/src/multilogue/utilities/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     5151 2023-08-05 23:47:47.000000 multilogue-0.0.9/src/multilogue/utilities/chatgpt.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4562 2023-08-04 19:38:14.000000 multilogue-0.0.9/src/multilogue/utilities/githublog.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-06 01:38:16.000000 multilogue-0.0.9/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      462 2023-08-06 01:38:16.000000 multilogue-0.0.9/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-08-06 01:38:16.000000 multilogue-0.0.9/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       49 2023-08-06 01:38:16.000000 multilogue-0.0.9/src/multilogue.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-08-06 01:38:16.000000 multilogue-0.0.9/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-06 01:38:16.774352 multilogue-0.0.9/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1154 2023-08-06 01:35:41.000000 multilogue-0.0.9/tests/test_chatgpt.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.9/tests/test_entities.py
```

### Comparing `multilogue-0.0.8/LICENSE` & `multilogue-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.8/PKG-INFO` & `multilogue-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multilogue is a cooperative game of reasoning entities against ignorance, confusion and misunderstanding.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multilogue-0.0.8/pyproject.toml` & `multilogue-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Multilogue is a cooperative game of reasoning entities against ignorance, confusion and misunderstanding."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilogue-0.0.8/src/multilogue/entities.py` & `multilogue-0.0.9/src/multilogue/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,31 @@
         return f"""     Entity:
             instructions - {self.instructions},
             functions - {self.functions},
             python_code - {self.python_code},
             name - {self.name},
             role - {self.role},
             """
+
+
+class Human(object):
+    """ Human participating in the multilogue """
+    name:           str = ''
+    role:           str = ''
+
+    def __init__(self, *args, **kwargs):
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+        super(Human, self).__init__()
+
+    def __call__(self, **kwargs):
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+        return self
+
+    def answer(self, *args, **kwargs):
+        """ Answer the last statement """
+        pass
+
+    def listen(self, *args, **kwargs):
+        """ Listen to the last statement """
+        pass
```

### Comparing `multilogue-0.0.8/src/multilogue/utilities/githublog.py` & `multilogue-0.0.9/src/multilogue/utilities/githublog.py`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.8/src/multilogue.egg-info/PKG-INFO` & `multilogue-0.0.9/src/multilogue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.8
+Version: 0.0.9
 Summary: Multilogue is a cooperative game of reasoning entities against ignorance, confusion and misunderstanding.
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

