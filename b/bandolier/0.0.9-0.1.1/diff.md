# Comparing `tmp/bandolier-0.0.9.tar.gz` & `tmp/bandolier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandolier-0.0.9.tar", last modified: Sun Aug  6 07:58:35 2023, max compression
+gzip compressed data, was "bandolier-0.1.1.tar", last modified: Sun Aug  6 09:22:34 2023, max compression
```

## Comparing `bandolier-0.0.9.tar` & `bandolier-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.809219 bandolier-0.0.9/
--rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.0.9/LICENSE
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:58:35.809074 bandolier-0.0.9/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.0.9/README.md
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.807893 bandolier-0.0.9/bandolier/
--rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.0.9/bandolier/__init__.py
--rw-r--r--   0 jlb        (501) staff       (20)     4403 2023-08-06 07:57:25.000000 bandolier-0.0.9/bandolier/bandolier.py
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.808856 bandolier-0.0.9/bandolier.egg-info/
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/SOURCES.txt
--rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/dependency_links.txt
--rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/requires.txt
--rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/top_level.txt
--rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 07:58:35.809263 bandolier-0.0.9/setup.cfg
--rw-r--r--   0 jlb        (501) staff       (20)     1190 2023-08-06 07:57:47.000000 bandolier-0.0.9/setup.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 09:22:34.426478 bandolier-0.1.1/
+-rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.1.1/LICENSE
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 09:22:34.426322 bandolier-0.1.1/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.1.1/README.md
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 09:22:34.425275 bandolier-0.1.1/bandolier/
+-rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.1.1/bandolier/__init__.py
+-rw-r--r--   0 jlb        (501) staff       (20)     4593 2023-08-06 08:48:58.000000 bandolier-0.1.1/bandolier/bandolier.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 09:22:34.426118 bandolier-0.1.1/bandolier.egg-info/
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 09:22:34.000000 bandolier-0.1.1/bandolier.egg-info/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 09:22:34.000000 bandolier-0.1.1/bandolier.egg-info/SOURCES.txt
+-rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 09:22:34.000000 bandolier-0.1.1/bandolier.egg-info/dependency_links.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 09:22:34.000000 bandolier-0.1.1/bandolier.egg-info/requires.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 09:22:34.000000 bandolier-0.1.1/bandolier.egg-info/top_level.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 09:22:34.426526 bandolier-0.1.1/setup.cfg
+-rw-r--r--   0 jlb        (501) staff       (20)     1190 2023-08-06 09:21:44.000000 bandolier-0.1.1/setup.py
```

### Comparing `bandolier-0.0.9/LICENSE` & `bandolier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.9/PKG-INFO` & `bandolier-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.9
+Version: 0.1.1
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.9/README.md` & `bandolier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.9/bandolier/bandolier.py` & `bandolier-0.1.1/bandolier/bandolier.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,48 +89,49 @@
     def add_user_message(self, content):
         "convience method for adding a user message"
         self.add_message({"role": "user", "content": content})
 
     def call(self, function_name, arguments):
         arguments = json.loads(arguments)
         function = self.functions[function_name]
-        return {
-            "role": "function",
-            "name": function_name,
-            "content": json.dumps(function(**arguments)),
-        }
+        return Box(
+            {
+                "role": "function",
+                "name": function_name,
+                "content": json.dumps(function(**arguments)),
+            }
+        )
 
     def get_function_metadata(self):
         return self.function_metadata
 
-    def run(self, debug=False):
+    def run(self):
         response = self.completion_fn(self.messages, self.get_function_metadata())
         message = response.message
         self.add_message(message)
 
+        # TODO FIXME this code makes the assumption that function call will not have message content,
+        # but that's not actually true.  It's possible to return a mesage with both content and a function call.
+        # This needs to be refactored so that run can return multiple messages.
+        messages = [message]
         while response.finish_reason == "function_call":
-            if debug:
-                print("function_call")
-                print(json.dumps(response, indent=2))
             message = self.call(
                 message.function_call.name, message.function_call.arguments
             )
-            if debug:
-                print("function call response")
-                print(json.dumps(message, indent=2))
             self.add_message(message)
+            messages.append(message)
 
             response = self.completion_fn(self.messages, self.get_function_metadata())
             message = response.message
             self.add_message(message)
+            messages.append(message)
 
         if response.finish_reason != "stop":
             raise Exception(f"Unexpected finish reason: {response.finish_reason}")
-
-        return message
+        return messages
 
     def _trim_messages(self):
         # I'm not sure how accurate this is, but I encode each message to json and then count
         # the tokens in the result.
 
         token_count = sum(len(self.encoding.encode(m.to_json())) for m in self.messages)
         while token_count > self.max_tokens:
```

### Comparing `bandolier-0.0.9/bandolier.egg-info/PKG-INFO` & `bandolier-0.1.1/bandolier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.9
+Version: 0.1.1
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.9/setup.py` & `bandolier-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
     readme = readme.split("\n")
     readme = [line for line in readme if "<img" not in line]
     readme = "\n".join(readme)
 
 setup(
     name="bandolier",
-    version="0.0.9",
+    version="0.1.1",
     description="A helper for OpenAI functions",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/johnnysands/bandolier",
     author="Johnny Sands",
     author_email="johnnysands@users.noreply.github.com",
     license="MIT",
```

