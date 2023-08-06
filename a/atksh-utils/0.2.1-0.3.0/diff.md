# Comparing `tmp/atksh-utils-0.2.1.tar.gz` & `tmp/atksh-utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.2.1.tar", last modified: Sat Jul  1 05:54:42 2023, max compression
+gzip compressed data, was "atksh-utils-0.3.0.tar", last modified: Sun Aug  6 06:40:50 2023, max compression
```

## Comparing `atksh-utils-0.2.1.tar` & `atksh-utils-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10340 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 05:54:42.000000 atksh-utils-0.2.1/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.872316 atksh-utils-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 05:54:42.876316 atksh-utils-0.2.1/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-01 05:54:32.000000 atksh-utils-0.2.1/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 06:40:50.906942 atksh-utils-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 06:40:50.000000 atksh-utils-0.3.0/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:40:50.902942 atksh-utils-0.3.0/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-06 06:40:40.000000 atksh-utils-0.3.0/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.2.1/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.3.0/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/.gitignore` & `atksh-utils-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/LICENSE` & `atksh-utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/PKG-INFO` & `atksh-utils-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.2.1
+Version: 0.3.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.2.1/README.md` & `atksh-utils-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/pyproject.toml` & `atksh-utils-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/src/atksh_utils/openai/functional.py` & `atksh-utils-0.3.0/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/src/atksh_utils/openai/tool.py` & `atksh-utils-0.3.0/src/atksh_utils/openai/tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import json
+import subprocess
+import tempfile
 import time
 from itertools import islice
 
 import requests
 from bs4 import BeautifulSoup as bs4
 from duckduckgo_search import DDGS
 
-from .prompt import SUMMARIZE_PROMPT
+from .prompt import SEARCH_RESULT_SUMMARIZE_PROMPT, VISIT_PAGE_SUMMARIZE_PROMPT
 
 MAX_ATTEMPTS = 3
 MAX_SEARCH_RESULTS = 8
 
 
 def get_browser_functions(ai: "OpenAI"):
-    child = ai.make_child(model_name="gpt-3.5-turbo-16k")
-    child.set_system_prompt(
-        SUMMARIZE_PROMPT + "\nPlease include URL links; otherwise, the following will fail."
-    )
+    search_result_child = ai.make_child(model_name="gpt-3.5-turbo-16k")
+    search_result_child.set_system_prompt(SEARCH_RESULT_SUMMARIZE_PROMPT)
+    visit_page_child = ai.make_child(model_name="gpt-3.5-turbo-16k")
+    visit_page_child.set_system_prompt(VISIT_PAGE_SUMMARIZE_PROMPT)
 
-    def _summarize(query_text: str, results: str) -> str:
+    def _search_summarize(query_text: str, results: str) -> str:
         """Summarizes the query text and results."""
-        return child(f"Query: {query_text}\nResults: {results}\nSummary: ")[1]
+        return search_result_child(f"Query: {query_text}\nResults: {results}\nSummary: ")[1]
+
+    def _page_summarize(query_text: str, page: str) -> str:
+        """Summarizes the query text and page."""
+        return visit_page_child(f"Query: {query_text}\nPage: {page}\nSummary: ")[1]
 
     def web_search(query_text: str) -> str:
         """Searches the web for the query text.
 
         :param query_text: The text to query.
         :type query_text: str
         :return: json dumped results (string)
@@ -38,30 +44,48 @@
             result = ddgs.text(query_text, region="ja-ja", safesearch="Off")
             search_results = list(islice(result, MAX_SEARCH_RESULTS))
             if search_results:
                 break
             attempts += 1
 
         results = json.dumps(search_results, ensure_ascii=False, indent=2)
-        ret = _summarize(query_text, results)
+        ret = _search_summarize(query_text, results)
         return ret
 
     def visit_page(query_text: str, url: str) -> str:
         """Visits the page at the url and summarizes the text with respect to the query text. Recommended to use after web_search for each url.
 
         :param query_text: The text to query for summarization.
         :type query_text: str
-        :param url: The url to visit (must be a valid url like `https://commerce-flow.com/request_brochure/`)
+        :param url: The url to visit (must be a valid url like `https://www.google.com`).
         :type url: str
         :return: The summarized text of the page.
         :rtype: str
         """
         try:
             response = requests.get(url)
             soup = bs4(response.text, "html.parser")
             body = soup.find("body").text.strip()
-            ret = _summarize(query_text, body[:10000])
+            ret = _page_summarize(query_text, body[:10000])
         except Exception as e:
             ret = f"Error: {e}.\nPlease try again or try another url."
         return ret
 
     return web_search, visit_page
+
+
+def exec_python_code(code: str) -> str:
+    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
+
+    :param code: Python code of multiple lines. You must print the result. For example, `value = 2 + 3; print(value)`.
+    :type code: str
+    :return: The result of the execution of the Python code (stdout by print)
+    :rtype: str
+    """
+    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
+        f.write(code)
+        f.flush()
+        result = subprocess.check_output(["python", f.name])
+    result = result.decode("utf-8").strip()
+    if not result:
+        result = "NotPrintedError('The result is not printed.')"
+    return result
```

### Comparing `atksh-utils-0.2.1/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.3.0/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.2.1
+Version: 0.3.0
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.2.1/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.3.0/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/tests/openai/test_api.py` & `atksh-utils-0.3.0/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.2.1/tests/openai/test_functional.py` & `atksh-utils-0.3.0/tests/openai/test_functional.py`

 * *Files identical despite different names*

