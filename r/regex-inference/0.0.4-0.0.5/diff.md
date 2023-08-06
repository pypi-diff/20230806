# Comparing `tmp/regex-inference-0.0.4.tar.gz` & `tmp/regex-inference-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-inference-0.0.4.tar", last modified: Sun Aug  6 02:51:27 2023, max compression
+gzip compressed data, was "regex-inference-0.0.5.tar", last modified: Sun Aug  6 04:13:07 2023, max compression
```

## Comparing `regex-inference-0.0.4.tar` & `regex-inference-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 02:51:09.000000 regex-inference-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 02:51:27.851202 regex-inference-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 02:51:09.000000 regex-inference-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/inference/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 02:51:27.851202 regex-inference-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 02:51:09.000000 regex-inference-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 04:12:48.000000 regex-inference-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 04:13:07.333952 regex-inference-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 04:12:48.000000 regex-inference-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.329952 regex-inference-0.0.5/regex_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/regex_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/inference/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/regex_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 04:13:07.333952 regex-inference-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 04:12:48.000000 regex-inference-0.0.5/setup.py
```

### Comparing `regex-inference-0.0.4/LICENSE` & `regex-inference-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.4/PKG-INFO` & `regex-inference-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.4
+Version: 0.0.5
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.4/regex_inference/inference/engine.py` & `regex-inference-0.0.5/regex_inference/inference/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,203 +17,182 @@
             model='text-davinci-003',  # https://platform.openai.com/docs/models/gpt-3-5
             client='regex_inference'
         )
         self._mismatch_tolerance = mismatch_tolerance
         self._max_iteration = max_iteration
         self._setup_lang_chains()
 
-    def _setup_lang_chains(self):
-        self._regex_alter_chain = LLMChain(
-            prompt=self.alter_regex_prompt,
-            llm=self._openai_llm
-        )
-        self._regex_revise_chain = LLMChain(
-            prompt=self.revise_regex_prompt,
-            llm=self._openai_llm
-        )
-        self._new_inference_chain = LLMChain(
-            prompt=self.new_inference_prompt,
-            llm=self._openai_llm
-        )
-        self._regex_simplify_chain = LLMChain(
-            prompt=self.simplify_regex_prompt,
-            llm=self._openai_llm
-        )
-
     def run(self, patterns: List[str], regex: Optional[str] = None) -> str:
+        assert len(
+            patterns) > 0, '`patterns` input to `run` should no be an empty list'
         if regex is None:
             regex = self._run(patterns)
         regex = self._run_simplify_regex(regex, patterns)
-        failed_patterns = self._get_failed_patterns(patterns, regex)
+        failed_patterns = self._get_mismatching_patterns(patterns, regex)
         while failed_patterns:
             failed_regex = self._run(failed_patterns)
             regex = f'{regex}|{failed_regex}'
             regex = self._run_simplify_regex(regex, patterns)
-            failed_patterns = self._get_failed_patterns(patterns, regex)
+            failed_patterns = self._get_mismatching_patterns(patterns, regex)
         return regex
 
     def _run(self, patterns: List[str], regex: Optional[str] = None) -> str:
         if regex:
             regex_result = self._run_alter_regex(regex, patterns)
         else:
             regex_result = self._run_new_inference(patterns)
-        regex_result = self._revise_regex(patterns, regex_result)
         return regex_result
 
+    @staticmethod
+    def _convert_patterns_to_prompt(patterns: List[str]) -> str:
+        return '\n'.join(map(lambda x: f'"{x}"', patterns))
+
     def _run_alter_regex(self, regex: str, patterns: List[str]) -> str:
         for _ in range(self._max_iteration):
             result = self._regex_alter_chain.run(
                 regex=regex,
-                strings='\n'.join(patterns)).strip()
+                strings=Engine._convert_patterns_to_prompt(patterns)
+            ).strip()
             try:
                 re.compile(result)
                 break
             except BaseException:
                 pass
         return result
 
     def _run_simplify_regex(self, regex: str, patterns: List[str]) -> str:
         for _ in range(self._max_iteration):
             result = self._regex_simplify_chain.run(
                 regex=regex,
-                strings='\n'.join(patterns)).strip()
+                strings=Engine._convert_patterns_to_prompt(patterns)
+            ).strip()
             try:
                 re.compile(result)
                 break
             except BaseException:
                 pass
         return result
 
     def _run_new_inference(self, patterns: List[str]) -> str:
         for _ in range(self._max_iteration):
-            result = self._new_inference_chain.run('\n'.join(patterns)).strip()
+            result = self._new_inference_chain.run(
+                Engine._convert_patterns_to_prompt(patterns)
+            ).strip()
             try:
                 re.compile(result)
                 break
             except BaseException:
                 pass
         return result
 
-    def _run_revise_regex(self, regex: str, patterns: List[str]) -> str:
-        for _ in range(self._max_iteration):
-            result = self._regex_revise_chain.run(
-                regex=regex,
-                strings='\n'.join(patterns)).strip()
-            try:
-                re.compile(result)
-                break
-            except BaseException:
-                pass
-        return result
+    def explain(self, regex: str) -> None:
+        result = self._regex_explain_chain.run(regex)
+        print(result)
 
-    def _revise_regex(self, patterns: List[str], regex: str) -> str:
-        mismtach_patterns = self._get_failed_patterns(patterns, regex)
-        iter_count = 0
-        while len(mismtach_patterns) / \
-                len(patterns) >= self._mismatch_tolerance:
-            regex = self._run_revise_regex(regex, patterns)
-            mismtach_patterns = self._get_failed_patterns(patterns, regex)
-            iter_count += 1
-            if iter_count > self._max_iteration:
-                break
-        return regex
-
-    def _get_failed_patterns(
+    def _get_mismatching_patterns(
             self, patterns: List[str], result_regex: str) -> List[str]:
         try:
             re_com = re.compile(result_regex)
         except BaseException as e:
             print('syntax error in result_regex:', result_regex)
             raise e
         result = list(filter(lambda x: re_com.fullmatch(x) is None, patterns))
         return result
 
+    def _setup_lang_chains(self):
+        self._regex_alter_chain = LLMChain(
+            prompt=self.alter_regex_prompt,
+            llm=self._openai_llm
+        )
+        self._new_inference_chain = LLMChain(
+            prompt=self.new_inference_prompt,
+            llm=self._openai_llm
+        )
+        self._regex_simplify_chain = LLMChain(
+            prompt=self.simplify_regex_prompt,
+            llm=self._openai_llm
+        )
+        self._regex_explain_chain = LLMChain(
+            prompt=self.explain_regex_prompt,
+            llm=self._openai_llm
+        )
+
     @property
     def new_inference_prompt(self) -> PromptTemplate:
         template = """Question: Show me the best and shortest regex that can fully match the strings that I provide to you.
 Note that:
 *. The regex should be made more generalized (e.g., use \\d to represent digit rather than using [0-9]) and shorter than the original regex.
 *. Match sure the resulting regex does not have syntax error.
 *. The character count of the resulting regex should not be larger than 30.
 *. Use \\d to replace [0-9].
 *. Try to focus more on the global pattern rather than the local patterns.
-Now, the patterns should be fully matched is provided line-by-line as follows:
+Now, each instance of the strings that should be fully matched is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
-Note: Provide the resulting regex without wrapping it in quote
+Note that:
+1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
+2. Provide the resulting regex without wrapping it in quote
+
 The resulting regex is: """
         prompt = PromptTemplate(
             template=template,
             input_variables=['strings']
         )
         return prompt
 
     @property
     def alter_regex_prompt(self) -> PromptTemplate:
         template = """Question: Alter the regex "{regex}" such that the following requirements is matched:
 *. The pattern fully match the regex still fully match the regex.
 *. The strings that I provide to you also fully match.
 *. The character count of the resulting regex should not be larger than 30.
 *. The regex should be made more generalized (e.g., use \\d to represent digit rather than using [0-9]) and shorter than the original regex.
-Each string of the strings is provided line-by-line as follows:
+Now, each instance of the strings is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
-Note: Provide the resulting regex without wrapping it in quote
+Note that:
+1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
+2. Provide the resulting regex without wrapping it in quote
+
 The resulting altered regex is: """
         prompt = PromptTemplate(
             template=template,
             input_variables=['regex', 'strings']
         )
         return prompt
 
     @property
     def simplify_regex_prompt(self) -> PromptTemplate:
         template = """
 Please revise the regex "{regex}"
 such that
 *. It becomes as short as possible.
 *. It still fully match all the strings full matched the original regex
-*. It still fully match each of the following strings:
-
+*. It still fully match each of the strings I provided to you.
+Now, each instance of the strings is provided line-by-line and wrapped by double quotes as follows:
 {strings}
 
-Note: Provide the resulting regex without wrapping it in quote
-The resulting revise regex is:
-"""
-        prompt = PromptTemplate(
-            template=template,
-            input_variables=['regex', 'strings']
-        )
-        return prompt
-
-    @property
-    def revise_regex_prompt(self) -> PromptTemplate:
-        template = """Question: Revise the regex "{regex}" such that the following requirements is matched:
-*. The patterns fully match the regex still fully match the revised regex.
-*. The regex should be made more generalized (e.g., use \\d to represent digit rather than using [0-9]) and shorter than the original regex.
-*. Match sure the resulting regex does not have syntax error.
-*. Use \\d to replace [0-9].
-*. Try to focus more on the global pattern rather than the local patterns.
-*. The character count of the resulting regex should not be larger than 30.
-*. The regex should be revised such that the provided mis-matched strings should be fully matched.
 
-Each string of the mis-matched strings is provided line-by-line as follows:
-{strings}
+Note that:
+1. The double quote is not part of the string instance. Ignore the double quote during inferencing the regex.
+2. Provide the resulting regex without wrapping it in quote
 
-Note: Provide the resulting regex without wrapping it in quote
-The resulting altered regex is: """
+The resulting revise regex is:
+"""
         prompt = PromptTemplate(
             template=template,
             input_variables=['regex', 'strings']
         )
         return prompt
 
     @property
     def explain_regex_prompt(self) -> PromptTemplate:
-        template = """Question: Explain the regex "{regex}" such that the role of each character in the regex is elaberated
+        template = """Question: Explain the regex "{regex}" such that
+1. The role of each character in the regex is elaberated.
+2. Provide 5 most interpretive example strings that fullmatch the regex.
 
 The explaination is: """
         prompt = PromptTemplate(
             template=template,
             input_variables=['regex']
         )
         return prompt
```

### Comparing `regex-inference-0.0.4/regex_inference.egg-info/PKG-INFO` & `regex-inference-0.0.5/regex_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-inference
-Version: 0.0.4
+Version: 0.0.5
 Summary: Regex Inference Engine based on ChatGPT
 Home-page: https://github.com/jeffrey82221/regex_inference
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `regex-inference-0.0.4/setup.py` & `regex-inference-0.0.5/setup.py`

 * *Files identical despite different names*

