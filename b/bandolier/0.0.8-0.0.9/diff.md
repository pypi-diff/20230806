# Comparing `tmp/bandolier-0.0.8.tar.gz` & `tmp/bandolier-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandolier-0.0.8.tar", last modified: Sun Aug  6 07:40:11 2023, max compression
+gzip compressed data, was "bandolier-0.0.9.tar", last modified: Sun Aug  6 07:58:35 2023, max compression
```

## Comparing `bandolier-0.0.8.tar` & `bandolier-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.042694 bandolier-0.0.8/
--rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.0.8/LICENSE
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:40:11.042511 bandolier-0.0.8/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.0.8/README.md
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.041447 bandolier-0.0.8/bandolier/
--rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.0.8/bandolier/__init__.py
--rw-r--r--   0 jlb        (501) staff       (20)     4152 2023-08-04 08:58:41.000000 bandolier-0.0.8/bandolier/bandolier.py
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.042212 bandolier-0.0.8/bandolier.egg-info/
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/SOURCES.txt
--rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/dependency_links.txt
--rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/requires.txt
--rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/top_level.txt
--rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 07:40:11.042748 bandolier-0.0.8/setup.cfg
--rw-r--r--   0 jlb        (501) staff       (20)     1370 2023-08-06 07:40:08.000000 bandolier-0.0.8/setup.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.809219 bandolier-0.0.9/
+-rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.0.9/LICENSE
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:58:35.809074 bandolier-0.0.9/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.0.9/README.md
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.807893 bandolier-0.0.9/bandolier/
+-rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.0.9/bandolier/__init__.py
+-rw-r--r--   0 jlb        (501) staff       (20)     4403 2023-08-06 07:57:25.000000 bandolier-0.0.9/bandolier/bandolier.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:58:35.808856 bandolier-0.0.9/bandolier.egg-info/
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/SOURCES.txt
+-rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/dependency_links.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/requires.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 07:58:35.000000 bandolier-0.0.9/bandolier.egg-info/top_level.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 07:58:35.809263 bandolier-0.0.9/setup.cfg
+-rw-r--r--   0 jlb        (501) staff       (20)     1190 2023-08-06 07:57:47.000000 bandolier-0.0.9/setup.py
```

### Comparing `bandolier-0.0.8/LICENSE` & `bandolier-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.8/PKG-INFO` & `bandolier-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.8
+Version: 0.0.9
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.8/README.md` & `bandolier-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.8/bandolier/bandolier.py` & `bandolier-0.0.9/bandolier/bandolier.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,23 +98,29 @@
             "name": function_name,
             "content": json.dumps(function(**arguments)),
         }
 
     def get_function_metadata(self):
         return self.function_metadata
 
-    def run(self):
+    def run(self, debug=False):
         response = self.completion_fn(self.messages, self.get_function_metadata())
         message = response.message
         self.add_message(message)
 
         while response.finish_reason == "function_call":
+            if debug:
+                print("function_call")
+                print(json.dumps(response, indent=2))
             message = self.call(
                 message.function_call.name, message.function_call.arguments
             )
+            if debug:
+                print("function call response")
+                print(json.dumps(message, indent=2))
             self.add_message(message)
 
             response = self.completion_fn(self.messages, self.get_function_metadata())
             message = response.message
             self.add_message(message)
 
         if response.finish_reason != "stop":
```

### Comparing `bandolier-0.0.8/bandolier.egg-info/PKG-INFO` & `bandolier-0.0.9/bandolier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.8
+Version: 0.0.9
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.8/setup.py` & `bandolier-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 readme = ""
 with open("README.md") as f:
     readme = f.read()
     readme = readme.split("\n")
     readme = [line for line in readme if "<img" not in line]
     readme = "\n".join(readme)
 
-# with open("requirements.txt", "r") as f:
-#    requirements = f.read().splitlines()
-
-# with open("requirements-dev.txt", "r") as f:
-#    requirements_dev = f.read().splitlines()
-
 setup(
     name="bandolier",
-    version="0.0.8",
+    version="0.0.9",
     description="A helper for OpenAI functions",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/johnnysands/bandolier",
     author="Johnny Sands",
     author_email="johnnysands@users.noreply.github.com",
     license="MIT",
```

