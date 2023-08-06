# Comparing `tmp/atksh-utils-0.3.0.tar.gz` & `tmp/atksh-utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.3.0.tar", last modified: Sun Aug  6 06:40:50 2023, max compression
+gzip compressed data, was "atksh-utils-0.3.1.tar", last modified: Sun Aug  6 06:54:27 2023, max compression
```

## Comparing `atksh-utils-0.3.0.tar` & `atksh-utils-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.816158 atksh-utils-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.816158 atksh-utils-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 06:54:27.000000 atksh-utils-0.3.1/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.816158 atksh-utils-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:54:27.820158 atksh-utils-0.3.1/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 06:54:17.000000 atksh-utils-0.3.1/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.3.0/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.3.1/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/.gitignore` & `atksh-utils-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/LICENSE` & `atksh-utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/PKG-INFO` & `atksh-utils-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.0/README.md` & `atksh-utils-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/pyproject.toml` & `atksh-utils-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/src/atksh_utils/openai/api.py` & `atksh-utils-0.3.1/src/atksh_utils/openai/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,21 @@
         Returns:
             List[Dict[str, str]]: The messages returned by the OpenAI API.
         """
         if messages is None:
             messages = []
             messages.append({"role": "system", "content": self.system_prompt})
             messages.append({"role": "user", "content": user_prompt})
+            messages.append(
+                {
+                    "role": "system",
+                    "content": f"Certainly. I'll answer your question, `{user_prompt}` with my best knowledge.",
+                }
+            )
+            messages.append({"role": "user", "content": "Thank you. Please answer my question."})
         if len(self.functions) > 0:
             functions = self.get_functions()
             response = self.openai.ChatCompletion.create(
                 model=self.model_name,
                 messages=messages,
                 functions=functions,
                 function_call="auto",
```

### Comparing `atksh-utils-0.3.0/src/atksh_utils/openai/functional.py` & `atksh-utils-0.3.1/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.3.1/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/src/atksh_utils/openai/tool.py` & `atksh-utils-0.3.1/src/atksh_utils/openai/tool.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.3.1/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.0/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.3.1/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/tests/openai/test_api.py` & `atksh-utils-0.3.1/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.0/tests/openai/test_functional.py` & `atksh-utils-0.3.1/tests/openai/test_functional.py`

 * *Files identical despite different names*

