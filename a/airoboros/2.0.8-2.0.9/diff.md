# Comparing `tmp/airoboros-2.0.8.tar.gz` & `tmp/airoboros-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-2.0.8.tar", last modified: Mon Jul 24 12:06:29 2023, max compression
+gzip compressed data, was "airoboros-2.0.9.tar", last modified: Mon Jul 24 15:26:39 2023, max compression
```

## Comparing `airoboros-2.0.8.tar` & `airoboros-2.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.371126 airoboros-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 12:06:16.000000 airoboros-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 12:06:29.371126 airoboros-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-24 12:06:16.000000 airoboros-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.363126 airoboros-2.0.8/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.367126 airoboros-2.0.8/airoboros/instructors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/counterfactual_contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/inline_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.371126 airoboros-2.0.8/airoboros/instructors/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/agent.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/card.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/coding.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/cot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/experience.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/general.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/orca.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/riddle.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/roleplay.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/trivia.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/wordgame.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/writing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/prompts/writing_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/riddle.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/roleplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/simple_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/trivia.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/wordgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/instructors/writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21035 2023-07-24 12:06:16.000000 airoboros-2.0.8/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:06:29.367126 airoboros-2.0.8/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 12:06:29.000000 airoboros-2.0.8/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:06:29.371126 airoboros-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-24 12:06:16.000000 airoboros-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:39.453345 airoboros-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 15:26:28.000000 airoboros-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 15:26:39.453345 airoboros-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-24 15:26:28.000000 airoboros-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:39.445345 airoboros-2.0.9/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:39.449345 airoboros-2.0.9/airoboros/instructors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/counterfactual_contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/inline_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:39.453345 airoboros-2.0.9/airoboros/instructors/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/agent.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/card.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/coding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/cot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/counterfactual_contextual.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/counterfactual_contextual_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/experience.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/general.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/orca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/riddle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/roleplay.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/trivia.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/wordgame.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/writing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/prompts/writing_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/riddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/roleplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/simple_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/trivia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/wordgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/instructors/writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21035 2023-07-24 15:26:28.000000 airoboros-2.0.9/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:39.445345 airoboros-2.0.9/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 15:26:39.000000 airoboros-2.0.9/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 15:26:39.453345 airoboros-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-24 15:26:28.000000 airoboros-2.0.9/setup.py
```

### Comparing `airoboros-2.0.8/LICENSE` & `airoboros-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/PKG-INFO` & `airoboros-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.8
+Version: 2.0.9
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.8/README.md` & `airoboros-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/entrypoint.py` & `airoboros-2.0.9/airoboros/entrypoint.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/coding.py` & `airoboros-2.0.9/airoboros/instructors/coding.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/contextual.py` & `airoboros-2.0.9/airoboros/instructors/contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/counterfactual_contextual.py` & `airoboros-2.0.9/airoboros/instructors/counterfactual_contextual.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/experience.py` & `airoboros-2.0.9/airoboros/instructors/experience.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/general.py` & `airoboros-2.0.9/airoboros/instructors/general.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/inline_qa.py` & `airoboros-2.0.9/airoboros/instructors/inline_qa.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/agent.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/agent.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/card.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/card.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/coding.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/coding.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/contextual.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/contextual_response.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/cot.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/cot.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/counterfactual_contextual.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/counterfactual_contextual_response.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/counterfactual_contextual_response.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/experience.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/experience.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/general.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/general.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/orca.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/orca.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/plan.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/plan.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/riddle.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/riddle.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,15 @@
 Example 6: QUESTION: Jackie has 3 brothers.  Each brother has 2 sisters.  How many sisters does Jackie have?
 ANSWER: Jackie has one sister.  If each brother has 2 sisters, assuming Jackie is a female, that would mean there are two total female siblings, of which Jackie is one, so 2 - 1 = 1.  The number of brothers is an extraneous detail.
 
 Please write 20 more examples of a similar format, with "QUESTION: [puzzle]" and "ANSWER: [answer]" with the correct answer, reasoning step-by-step for the answer when appropriate.
 
 All output text should be in {language}, but the exact terms "QUESTION" and "ANSWER" are special tokens that must not be translated.
 
+Try not to use common/well-known riddles; the puzzles/riddles should be highly diverse and unique.
+
 The output format should be:
 QUESTION: [first puzzle]
 ANSWER: [first puzzle's answer]
 
 QUESTION: [second puzzle]
 ANSWER: [second puzzle's answer]
```

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/roleplay.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/roleplay.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/trivia.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/trivia.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/wordgame.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/wordgame.txt`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/writing.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/writing.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - Create a short story somehow involving kayaks and snowy mountain peaks.
 - Compose a short story based on some of the following guidelines.  The main character is David Dorado, who wears an eye patch due to a tragic accident as a child involing a spork.  The other character in Cynthia Tulip, who is a quiet, French Canadian who speaks English but not particularly well.  She secretly loves David, but David isn't aware and doesn't return her affection.  David suddenly realizes he may actually be in love with her while they drink coffee at noon.
 - Write an email announcing a new breakthrough in tire technology by your company ("Atobormafi Tire Tech") which increases fuel efficiency by 7% on average.  The target of the email is investors, since we are seeking Series B funding.  Explain the profit possibilities with such a tire and ask for new investment.
 - Write the introduction and methodology sections of a research article in which the use of Psilocybin Cubensis reduced dependency on parmeson cheese by 82%.  Dosage was 0.5g/day, split between 3 dosages, administered orally.  Double blind, placebo controlled, 1812 participants.
 
 Make sure to include a wide variety of writing tasks, across a wide range of subjects.
 
+{style_extra}
+
 All output text should be in {language}.
 
 {topic_avoidance}
 
 Include exactly {batch_size} tasks in your response.
 
 Response format:
```

### Comparing `airoboros-2.0.8/airoboros/instructors/prompts/writing_response.txt` & `airoboros-2.0.9/airoboros/instructors/prompts/writing_response.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 Below is a user's instruction.
 
 I would would like you to following the following rules:
 - Always pay very close attention to the details in the instruction to make sure the output will be pleasing to the user.
 - When the instruction specifies a specific style (happy, sad, inspirational, etc.), be sure to apply that to your response.
-- If the instruction doesn't specify any particular ending style (happy, inspirational, etc.), and the instruction is to write a poem, story, song, or other creative/non-professional output, you will quietly randomly select from one of the following styles: happy, sad, surprising, open-ended, shocking, tragic.  Remember that not all stories need a resolution where the downtrodden somehow win - lessons can be learned from stories with bad/sad/tragic endings as well, so don't always select a happy ending.  Characters in the story can be friendly, mean, violent, or anything in between - remember, it's just a story, and complex character interactions make it more compelling.  Don't include any moralizing or explanation of what the lesson should be, just tell the story - the user is smart and will understand.
+- If the instruction doesn't specify any particular style (happy, inspirational, etc.), and the instruction is to write a poem, story, song, or other creative/non-professional output, you will quietly randomly select from one of the following styles: happy, sad, surprising, open-ended, shocking, tragic.  Remember that not all stories need a resolution where the downtrodden somehow win - lessons can be learned from stories with bad/sad/tragic endings as well, so don't always select a happy ending.  Characters in the story can be friendly, mean, violent, or anything in between - remember, it's just a story, and complex character interactions make it more compelling.  Don't include any moralizing or explanation of what the lesson should be, just tell the story - the user is smart and will understand.
 - If the instruction is to write an email or letter, do not start the body of the message with "I hope this [..] finds you ...".  Use a variety of introductory sentences without requiring some sort of nicety.
 
+The response should be in {language}.
+
 Instruction: {instruction}
```

### Comparing `airoboros-2.0.8/airoboros/instructors/simple_task.py` & `airoboros-2.0.9/airoboros/instructors/simple_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import os
 import re
 
 
-async def generate(instructor, category):
+async def generate(instructor, category, template_kwargs={}):
     """Generator for simple instruction response tasks (e.g. roleplay, wordgames)."""
     config = instructor.instructors.get(category)
     if not config:
         return
     target_count = config.get("count")
     if target_count is None:
         target_count = instructor.default_count
@@ -45,24 +45,22 @@
     if batch_size is None:
         batch_size = instructor.default_batch_size
     batch_size = int(batch_size)
     if category not in instructor.instructor_counts:
         instructor.instructor_counts[category] = 0
     language = config.get("language") or instructor.language
     while instructor.instructor_counts[category] < target_count:
+        format_args = {"batch_size": batch_size, "language": language}
+        for key, val in template_kwargs.items():
+            format_args[key] = val(instructor)
+        if "{topic_avoidance}" in template:
+            format_args["topic_avoidance"] = instructor.topic_avoidance
+
         # Get a batch of instructions.
-        prompt = (
-            template.format(batch_size=batch_size, language=language)
-            if "{topic_avoidance}" not in template
-            else template.format(
-                batch_size=batch_size,
-                language=language,
-                topic_avoidance=instructor.topic_avoidance,
-            )
-        )
+        prompt = template.format(**format_args)
         response = await instructor.generate_response(prompt, **api_params)
         if not response:
             continue
 
         # Parse instructions and generate responses.
         futures = []
         instructions = []
@@ -72,15 +70,17 @@
             if not instruction.strip() or await instructor.is_too_similar(
                 instruction, min_score=min_score
             ):
                 continue
             instructions.append(instruction)
             full_prompt = instruction
             if response_prompt:
-                full_prompt = response_prompt.format(instruction=instruction)
+                full_prompt = response_prompt.format(
+                    language=language, instruction=instruction
+                )
             futures.append(instructor.generate_response(full_prompt, **api_params))
         if not futures:
             continue
         responses = await asyncio.gather(*futures)
         for idx in range(len(responses)):
             response = responses[idx]
             if not response or not response.strip():
```

### Comparing `airoboros-2.0.8/airoboros/instructors/trivia.py` & `airoboros-2.0.9/airoboros/instructors/trivia.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros/self_instruct.py` & `airoboros-2.0.9/airoboros/self_instruct.py`

 * *Files identical despite different names*

### Comparing `airoboros-2.0.8/airoboros.egg-info/PKG-INFO` & `airoboros-2.0.9/airoboros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 2.0.8
+Version: 2.0.9
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-2.0.8/airoboros.egg-info/SOURCES.txt` & `airoboros-2.0.9/airoboros.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 airoboros/__init__.py
 airoboros/entrypoint.py
 airoboros/exceptions.py
 airoboros/self_instruct.py
 airoboros.egg-info/PKG-INFO
 airoboros.egg-info/SOURCES.txt
```

### Comparing `airoboros-2.0.8/setup.py` & `airoboros-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="2.0.8",
+    version="2.0.9",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros", "airoboros.instructors", "airoboros.instructors.prompts"],
```

