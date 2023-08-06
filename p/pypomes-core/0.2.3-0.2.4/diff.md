# Comparing `tmp/pypomes_core-0.2.3.tar.gz` & `tmp/pypomes_core-0.2.4.tar.gz`

## Comparing `pypomes_core-0.2.3.tar` & `pypomes_core-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27417 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/README.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27417 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pypomes_core-0.2.4/PKG-INFO
```

### Comparing `pypomes_core-0.2.3/src/pypomes_core/.ruff.toml` & `pypomes_core-0.2.4/src/pypomes_core/.ruff.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # environment
 cache-dir = "~/.cache/ruff"
 force-exclude = true
-required-version = "0.0.280"
+required-version = "0.0.282"
 target-version = "py310"
 respect-gitignore = true
 task-tags = ["TODO", "FIXME", "HACK"]
 select = [
     # flake8 group
     "A",     # flake8-builtins - prevent shadowing of python builtins
     "ANN",   # flake8-annotations - enforce PEP 3107-style function
@@ -77,14 +77,15 @@
     "D204",     # 1 blank line required after class docstring
     "D210",     # whitespaces surrounding docstring text
     "G004",     # logging statement uses f-string
     "PLR2004",  # magic value used in comparison, consider replacing it with a constant variable
     "PTH118",   # os.{module}.join() should be replaced by Path with / operator
     "D212",     # multi-line docstring summary to start at the second line
     "RUF013",   # implicit Optional in type annotations when the default parameter value is None
+    "S301",     # 'pickle' and modules that wrap it can be unsafe when used to deserialize untrusted data
     "S608",     # possible SQL injection vector through string-based query construction
     "SIM108",   # use ternary operator instead of if-else-block
 ]
 
 # rules
 line-length = 120
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
@@ -96,18 +97,18 @@
 max-string-length = 60      # maximum string length for string literals in exception messages
 
 [flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "double"
 multiline-quotes = "double"
 
-
 [mccabe]
-max-complexity = 20      # upper limit for McCabe code complexity
+max-complexity = 20         # upper limit for McCabe code complexity
 
 [pycodestyle]
 max-doc-length = 120
 
 [pylint]
 max-args = 10
 max-branches = 32
-max-returns = 1
+max-returns = 1
+max-statements = 60
```

### Comparing `pypomes_core-0.2.3/src/pypomes_core/__init__.py` & `pypomes_core-0.2.4/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/email_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/env_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/file_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/http_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/http_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/json_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/list_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/str_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.2.4/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/LICENSE` & `pypomes_core-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.3/pyproject.toml` & `pypomes_core-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.2.3/PKG-INFO` & `pypomes_core-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

