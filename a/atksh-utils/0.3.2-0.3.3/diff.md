# Comparing `tmp/atksh-utils-0.3.2.tar.gz` & `tmp/atksh-utils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.3.2.tar", last modified: Sun Aug  6 07:12:22 2023, max compression
+gzip compressed data, was "atksh-utils-0.3.3.tar", last modified: Sun Aug  6 07:13:15 2023, max compression
```

## Comparing `atksh-utils-0.3.2.tar` & `atksh-utils-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.727272 atksh-utils-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.727272 atksh-utils-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 07:12:22.000000 atksh-utils-0.3.2/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.727272 atksh-utils-0.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:22.731272 atksh-utils-0.3.2/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 07:12:12.000000 atksh-utils-0.3.2/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.490104 atksh-utils-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.482104 atksh-utils-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.486104 atksh-utils-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:13:15.490104 atksh-utils-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 07:13:15.490104 atksh-utils-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.482104 atksh-utils-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.486104 atksh-utils-0.3.3/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.486104 atksh-utils-0.3.3/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.486104 atksh-utils-0.3.3/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 07:13:15.000000 atksh-utils-0.3.3/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.482104 atksh-utils-0.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:15.490104 atksh-utils-0.3.3/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 07:13:03.000000 atksh-utils-0.3.3/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.3.2/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.3.3/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/.gitignore` & `atksh-utils-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/LICENSE` & `atksh-utils-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/PKG-INFO` & `atksh-utils-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.2
+Version: 0.3.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.2/README.md` & `atksh-utils-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/pyproject.toml` & `atksh-utils-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/src/atksh_utils/openai/api.py` & `atksh-utils-0.3.3/src/atksh_utils/openai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,14 @@
             user_prompt (str): The user prompt to use.
 
         Returns:
             Tuple[List[Dict[str, str]], str]: The messages returned by the OpenAI API and the final message.
             str: The final message returned by the OpenAI API.
         """
         messages = self.call(user_prompt, stream_callback=stream_callback)
-        print(messages)
         return messages, messages[-1]["content"]
 
     def __repr__(self) -> str:
         return f"OpenAI(model_name={self.model_name}, temperature={self.temperature}, top_p={self.top_p})"
 
     def set_browser_functions(self):
         web_search, visit_page = get_browser_functions(self)
```

### Comparing `atksh-utils-0.3.2/src/atksh_utils/openai/functional.py` & `atksh-utils-0.3.3/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.3.3/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/src/atksh_utils/openai/tool.py` & `atksh-utils-0.3.3/src/atksh_utils/openai/tool.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.3.3/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.3.2
+Version: 0.3.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.3.2/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.3.3/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/tests/openai/test_api.py` & `atksh-utils-0.3.3/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.3.2/tests/openai/test_functional.py` & `atksh-utils-0.3.3/tests/openai/test_functional.py`

 * *Files identical despite different names*

