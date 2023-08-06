# Comparing `tmp/specialist-0.5.1.tar.gz` & `tmp/specialist-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialist-0.5.1.tar", last modified: Wed Apr 26 20:08:43 2023, max compression
+gzip compressed data, was "specialist-0.6.0.tar", last modified: Sun Aug  6 00:34:58 2023, max compression
```

## Comparing `specialist-0.5.1.tar` & `specialist-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:43.802691 specialist-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 20:08:34.000000 specialist-0.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-26 20:08:43.802691 specialist-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-26 20:08:34.000000 specialist-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:08:43.802691 specialist-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-26 20:08:34.000000 specialist-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:43.802691 specialist-0.5.1/specialist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-26 20:08:34.000000 specialist-0.5.1/specialist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:34:58.179149 specialist-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-06 00:34:49.000000 specialist-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-06 00:34:58.179149 specialist-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-06 00:34:49.000000 specialist-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:34:58.179149 specialist-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-06 00:34:49.000000 specialist-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:34:58.175150 specialist-0.6.0/specialist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-08-06 00:34:49.000000 specialist-0.6.0/specialist.py
```

### Comparing `specialist-0.5.1/LICENSE.md` & `specialist-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specialist-0.5.1/PKG-INFO` & `specialist-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: specialist
-Version: 0.5.1
-Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
-Home-page: https://github.com/brandtbucher/specialist
-Author: Brandt Bucher
-Author-email: brandt@python.org
-License: MIT
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 <div align=center>
 
 
 Specialist
 ==========
 
 [![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/actions/workflow/status/brandtbucher/specialist/ci.yml.svg?style=for-the-badge&branch=main)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
@@ -26,28 +14,43 @@
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
 information to create visual representations of exactly *where* and *how* CPython
 3.11's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
+</div>
 
-Installation
-------------
+
+Getting Started
+---------------
 
 Specialist supports CPython 3.11+ on all platforms.
 
 To install, just run:
 
 ```sh
 $ pip install specialist
 ```
 
+If you normally use `pytest` to run your tests, then you can try using the
+following command to run them instead:
+
+```sh
+$ specialist --output report --targets '**/*.py' -m pytest # any additional pytest options here...
+```
+
+After your tests complete, `specialist` will create a directory named `report`
+and fill it with browsable HTML visualizations for each module in the current
+directory tree.
+
 
 Background
 ----------
 
 While CPython 3.11 is running your code, it identifies "hot" regions that are
 being run often enough to spend time optimizing. It occasionally "quickens"
 these regions, which `specialist` represents using color. **Dark, rich colors
@@ -72,15 +75,16 @@
 - If a specialization becomes invalid after some time (for example, if an
 expression that previously added two integers starts concatenating two strings
 instead), the specialized instruction may be converted back into an adaptive
 one. At this point, the cycle repeats itself.
 
 Specialist aims to provide insight into this process for the maintainers of
 CPython itself, as well as for users seeking an optimization profile for their
-own code.
+own code. If you're curious to learn more about specialization, check out [this
+talk from PyCon US 2023](https://youtu.be/shQtrn1v7sQ).
 
 
 Tutorial
 --------
 
 Suppose we have the following source file, `conversions.py`, which contains some
 utilities and tests for converting between Fahrenheit and Celsius:
@@ -119,16 +123,20 @@
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-1.png)
 
+</div>
+
 The green areas indicate regions of code that were successfully specialized,
 while the red areas indicate unsuccessful specializations (in the form of
 "adaptive" instructions). Mixed results are indicated by colors along the
 green-yellow-orange-red gradient, depending on the ratio of successes to
 failures. Regions of code that don't contain any attempted specializations are
 left white.
 
@@ -137,46 +145,42 @@
 specialize binary operators between mixed `float` and `int` values, which is
 exactly what the code here is doing.
 
 It can, however, specialize addition and subtraction between two `float` values!
 Replacing `32` with `32.0` results in successful specializations (confirmed by
 re-running `specialist`):
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-2.png)
 
+</div>
+
 We can see that something similar is happening with `float` and `int`
 multiplication as well. One option could be to continue converting constant
 values to `float`:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-3.png)
 
+</div>
+
 However, there's a better option! Notice that CPython doesn't attempt to
 specialize division at all (it's left white in the visualization). We can take
 advantage of CPython's constant folding optimizations by slightly changing the
 order of operations, which allows our scaling factors (`5 / 9` and `9 / 5`) to
 be computed at compile-time. When we do this, CPython is able to implement our
 converters *entirely* using native floating-point operations:
 
-![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
+<div align=center>
 
-A few notes on the remaining code:
+![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
 
-- The global lookup of `TEST_VALUES` is red because it hasn't had the
-opportunity to be specialized yet. Though CPython *was* able to identify
-`test_conversions` as "hot" code and quicken the body, this didn't happen until
-*after* `TEST_VALUES` was looked up (which happens only once). It would be
-wasteful to spend time optimizing code that is never run again!
-
-- Similarly, parts of the `assert` statements in `assert_round_trip` are red
-because they are "dead" code that never actually runs.
-
-- The calls to `math.is_close` are orange because it is implemented in C.
-C extensions can't be "inlined" the same way as pure-Python calls like`c_to_f`,
-`f_to_c`, and `assert_round_trip`, so most of the call sequence isn't able to be
-specialized.
+</div>
 
 
 Modes
 -----
 
 Like `python` itself, `specialist` can run code a few different ways. It can be
 given a file path:
```

### Comparing `specialist-0.5.1/README.md` & `specialist-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: specialist
+Version: 0.6.0
+Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
+Home-page: https://github.com/brandtbucher/specialist
+Author: Brandt Bucher
+Author-email: brandt@python.org
+License: MIT
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 <div align=center>
 
 
 Specialist
 ==========
 
 [![latest version](https://img.shields.io/github/release-pre/brandtbucher/specialist.svg?style=for-the-badge&label=latest)![latest release date](https://img.shields.io/github/release-date-pre/brandtbucher/specialist.svg?style=for-the-badge&label=released)](https://github.com/brandtbucher/specialist/releases)[![build status](https://img.shields.io/github/actions/workflow/status/brandtbucher/specialist/ci.yml.svg?style=for-the-badge&branch=main)](https://github.com/brandtbucher/specialist/actions)[![issues](https://img.shields.io/github/issues-raw/brandtbucher/specialist.svg?label=issues&style=for-the-badge)](https://github.com/brandtbucher/specialist/issues)
@@ -14,28 +26,43 @@
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
 information to create visual representations of exactly *where* and *how* CPython
 3.11's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
+</div>
 
-Installation
-------------
+
+Getting Started
+---------------
 
 Specialist supports CPython 3.11+ on all platforms.
 
 To install, just run:
 
 ```sh
 $ pip install specialist
 ```
 
+If you normally use `pytest` to run your tests, then you can try using the
+following command to run them instead:
+
+```sh
+$ specialist --output report --targets '**/*.py' -m pytest # any additional pytest options here...
+```
+
+After your tests complete, `specialist` will create a directory named `report`
+and fill it with browsable HTML visualizations for each module in the current
+directory tree.
+
 
 Background
 ----------
 
 While CPython 3.11 is running your code, it identifies "hot" regions that are
 being run often enough to spend time optimizing. It occasionally "quickens"
 these regions, which `specialist` represents using color. **Dark, rich colors
@@ -60,15 +87,16 @@
 - If a specialization becomes invalid after some time (for example, if an
 expression that previously added two integers starts concatenating two strings
 instead), the specialized instruction may be converted back into an adaptive
 one. At this point, the cycle repeats itself.
 
 Specialist aims to provide insight into this process for the maintainers of
 CPython itself, as well as for users seeking an optimization profile for their
-own code.
+own code. If you're curious to learn more about specialization, check out [this
+talk from PyCon US 2023](https://youtu.be/shQtrn1v7sQ).
 
 
 Tutorial
 --------
 
 Suppose we have the following source file, `conversions.py`, which contains some
 utilities and tests for converting between Fahrenheit and Celsius:
@@ -107,16 +135,20 @@
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-1.png)
 
+</div>
+
 The green areas indicate regions of code that were successfully specialized,
 while the red areas indicate unsuccessful specializations (in the form of
 "adaptive" instructions). Mixed results are indicated by colors along the
 green-yellow-orange-red gradient, depending on the ratio of successes to
 failures. Regions of code that don't contain any attempted specializations are
 left white.
 
@@ -125,46 +157,42 @@
 specialize binary operators between mixed `float` and `int` values, which is
 exactly what the code here is doing.
 
 It can, however, specialize addition and subtraction between two `float` values!
 Replacing `32` with `32.0` results in successful specializations (confirmed by
 re-running `specialist`):
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-2.png)
 
+</div>
+
 We can see that something similar is happening with `float` and `int`
 multiplication as well. One option could be to continue converting constant
 values to `float`:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-3.png)
 
+</div>
+
 However, there's a better option! Notice that CPython doesn't attempt to
 specialize division at all (it's left white in the visualization). We can take
 advantage of CPython's constant folding optimizations by slightly changing the
 order of operations, which allows our scaling factors (`5 / 9` and `9 / 5`) to
 be computed at compile-time. When we do this, CPython is able to implement our
 converters *entirely* using native floating-point operations:
 
-![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
+<div align=center>
 
-A few notes on the remaining code:
+![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
 
-- The global lookup of `TEST_VALUES` is red because it hasn't had the
-opportunity to be specialized yet. Though CPython *was* able to identify
-`test_conversions` as "hot" code and quicken the body, this didn't happen until
-*after* `TEST_VALUES` was looked up (which happens only once). It would be
-wasteful to spend time optimizing code that is never run again!
-
-- Similarly, parts of the `assert` statements in `assert_round_trip` are red
-because they are "dead" code that never actually runs.
-
-- The calls to `math.is_close` are orange because it is implemented in C.
-C extensions can't be "inlined" the same way as pure-Python calls like`c_to_f`,
-`f_to_c`, and `assert_round_trip`, so most of the call sequence isn't able to be
-specialized.
+</div>
 
 
 Modes
 -----
 
 Like `python` itself, `specialist` can run code a few different ways. It can be
 given a file path:
```

### Comparing `specialist-0.5.1/setup.py` & `specialist-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     license="MIT",
     long_description=README.read_text(),
     long_description_content_type="text/markdown",
     name="specialist",
     py_modules=["specialist"],
     python_requires=">=3.11",
     url="https://github.com/brandtbucher/specialist",
-    version="0.5.1",
+    version="0.6.0",
 )
```

### Comparing `specialist-0.5.1/specialist.egg-info/PKG-INFO` & `specialist-0.6.0/specialist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.5.1
+Version: 0.6.0
 Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -26,28 +26,43 @@
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
 information to create visual representations of exactly *where* and *how* CPython
 3.11's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
+</div>
+
 
-Installation
-------------
+Getting Started
+---------------
 
 Specialist supports CPython 3.11+ on all platforms.
 
 To install, just run:
 
 ```sh
 $ pip install specialist
 ```
 
+If you normally use `pytest` to run your tests, then you can try using the
+following command to run them instead:
+
+```sh
+$ specialist --output report --targets '**/*.py' -m pytest # any additional pytest options here...
+```
+
+After your tests complete, `specialist` will create a directory named `report`
+and fill it with browsable HTML visualizations for each module in the current
+directory tree.
+
 
 Background
 ----------
 
 While CPython 3.11 is running your code, it identifies "hot" regions that are
 being run often enough to spend time optimizing. It occasionally "quickens"
 these regions, which `specialist` represents using color. **Dark, rich colors
@@ -72,15 +87,16 @@
 - If a specialization becomes invalid after some time (for example, if an
 expression that previously added two integers starts concatenating two strings
 instead), the specialized instruction may be converted back into an adaptive
 one. At this point, the cycle repeats itself.
 
 Specialist aims to provide insight into this process for the maintainers of
 CPython itself, as well as for users seeking an optimization profile for their
-own code.
+own code. If you're curious to learn more about specialization, check out [this
+talk from PyCon US 2023](https://youtu.be/shQtrn1v7sQ).
 
 
 Tutorial
 --------
 
 Suppose we have the following source file, `conversions.py`, which contains some
 utilities and tests for converting between Fahrenheit and Celsius:
@@ -119,16 +135,20 @@
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-1.png)
 
+</div>
+
 The green areas indicate regions of code that were successfully specialized,
 while the red areas indicate unsuccessful specializations (in the form of
 "adaptive" instructions). Mixed results are indicated by colors along the
 green-yellow-orange-red gradient, depending on the ratio of successes to
 failures. Regions of code that don't contain any attempted specializations are
 left white.
 
@@ -137,46 +157,42 @@
 specialize binary operators between mixed `float` and `int` values, which is
 exactly what the code here is doing.
 
 It can, however, specialize addition and subtraction between two `float` values!
 Replacing `32` with `32.0` results in successful specializations (confirmed by
 re-running `specialist`):
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-2.png)
 
+</div>
+
 We can see that something similar is happening with `float` and `int`
 multiplication as well. One option could be to continue converting constant
 values to `float`:
 
+<div align=center>
+
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-3.png)
 
+</div>
+
 However, there's a better option! Notice that CPython doesn't attempt to
 specialize division at all (it's left white in the visualization). We can take
 advantage of CPython's constant folding optimizations by slightly changing the
 order of operations, which allows our scaling factors (`5 / 9` and `9 / 5`) to
 be computed at compile-time. When we do this, CPython is able to implement our
 converters *entirely* using native floating-point operations:
 
-![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
+<div align=center>
 
-A few notes on the remaining code:
+![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-4.png)
 
-- The global lookup of `TEST_VALUES` is red because it hasn't had the
-opportunity to be specialized yet. Though CPython *was* able to identify
-`test_conversions` as "hot" code and quicken the body, this didn't happen until
-*after* `TEST_VALUES` was looked up (which happens only once). It would be
-wasteful to spend time optimizing code that is never run again!
-
-- Similarly, parts of the `assert` statements in `assert_round_trip` are red
-because they are "dead" code that never actually runs.
-
-- The calls to `math.is_close` are orange because it is implemented in C.
-C extensions can't be "inlined" the same way as pure-Python calls like`c_to_f`,
-`f_to_c`, and `assert_round_trip`, so most of the call sequence isn't able to be
-specialized.
+</div>
 
 
 Modes
 -----
 
 Like `python` itself, `specialist` can run code a few different ways. It can be
 given a file path:
```

### Comparing `specialist-0.5.1/specialist.py` & `specialist-0.6.0/specialist.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,52 +32,69 @@
 import dis
 import html
 import http.server
 import importlib.util
 import itertools
 import opcode
 import os
+import re
 import runpy
 import shlex
 import sysconfig
 import tempfile
 import threading
 import typing
 import webbrowser
 
+_RE_WHITESPACE = re.compile(r"(\s*\n\s*)")
 _FIRST_POSTION = (1, 0)
 _LAST_POSITION = (sys.maxsize, 0)
+_CACHE_FORMAT = frozenset(opcode._cache_format)  # type: ignore [attr-defined] # pylint: disable = protected-access
 _SPECIALIZED_INSTRUCTIONS = frozenset(opcode._specialized_instructions)  # type: ignore [attr-defined] # pylint: disable = protected-access
-_SUPERDUPERINSTRUCTIONS = frozenset({"PRECALL_NO_KW_LIST_APPEND"})
-_SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | frozenset(
-    {
-        "BINARY_OP_INPLACE_ADD_UNICODE",
-        "COMPARE_OP_FLOAT_JUMP",
-        "COMPARE_OP_INT_JUMP",
-        "COMPARE_OP_STR_JUMP",
-        "LOAD_CONST__LOAD_FAST",
-        "LOAD_FAST__LOAD_CONST",
-        "LOAD_FAST__LOAD_FAST",
-        "PRECALL_BUILTIN_CLASS",
-        "PRECALL_BUILTIN_FAST_WITH_KEYWORDS",
-        "PRECALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS",
-        "PRECALL_NO_KW_BUILTIN_FAST",
-        "PRECALL_NO_KW_BUILTIN_O",
-        "PRECALL_NO_KW_ISINSTANCE",
-        "PRECALL_NO_KW_LEN",
-        "PRECALL_NO_KW_METHOD_DESCRIPTOR_FAST",
-        "PRECALL_NO_KW_METHOD_DESCRIPTOR_NOARGS",
-        "PRECALL_NO_KW_METHOD_DESCRIPTOR_O",
-        "PRECALL_NO_KW_STR_1",
-        "PRECALL_NO_KW_TUPLE_1",
-        "PRECALL_NO_KW_TYPE_1",
-        "STORE_FAST__LOAD_FAST",
-        "STORE_FAST__STORE_FAST",
-    }
-)
+if sys.version_info < (3, 12):  # pragma: no cover
+    _SUPERDUPERINSTRUCTIONS = frozenset({"PRECALL_NO_KW_LIST_APPEND"})
+    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | frozenset(
+        {
+            "BINARY_OP_INPLACE_ADD_UNICODE",
+            "COMPARE_OP_FLOAT_JUMP",
+            "COMPARE_OP_INT_JUMP",
+            "COMPARE_OP_STR_JUMP",
+            "LOAD_CONST__LOAD_FAST",
+            "LOAD_FAST__LOAD_CONST",
+            "LOAD_FAST__LOAD_FAST",
+            "PRECALL_BUILTIN_CLASS",
+            "PRECALL_BUILTIN_FAST_WITH_KEYWORDS",
+            "PRECALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS",
+            "PRECALL_NO_KW_BUILTIN_FAST",
+            "PRECALL_NO_KW_BUILTIN_O",
+            "PRECALL_NO_KW_ISINSTANCE",
+            "PRECALL_NO_KW_LEN",
+            "PRECALL_NO_KW_METHOD_DESCRIPTOR_FAST",
+            "PRECALL_NO_KW_METHOD_DESCRIPTOR_NOARGS",
+            "PRECALL_NO_KW_METHOD_DESCRIPTOR_O",
+            "PRECALL_NO_KW_STR_1",
+            "PRECALL_NO_KW_TUPLE_1",
+            "PRECALL_NO_KW_TYPE_1",
+            "STORE_FAST__LOAD_FAST",
+            "STORE_FAST__STORE_FAST",
+        }
+    )
+else:  # pragma: no cover
+    _SUPERDUPERINSTRUCTIONS: frozenset[str] = frozenset()
+    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | frozenset(
+        {
+            "BINARY_OP_INPLACE_ADD_UNICODE",
+            "CALL_NO_KW_LIST_APPEND",
+            "LOAD_CONST__LOAD_FAST",
+            "LOAD_FAST__LOAD_CONST",
+            "LOAD_FAST__LOAD_FAST",
+            "STORE_FAST__LOAD_FAST",
+            "STORE_FAST__STORE_FAST",
+        }
+    )
 _PURELIB = pathlib.Path(sysconfig.get_path("purelib")).resolve()
 assert _PURELIB.is_dir(), _PURELIB
 _STDLIB = pathlib.Path(sysconfig.get_path("stdlib")).resolve()
 assert _STDLIB.is_dir(), _STDLIB
 _TMP = pathlib.Path(tempfile.gettempdir()).resolve()
 assert _TMP.is_dir(), _TMP
 
@@ -100,17 +117,21 @@
         ]
 
     def add(self, source: str, stats: "_Stats") -> None:
         """Add a chunk of code to the output."""
         color = self._color(stats)
         attribute = "color" if self._dark else "background-color"
         source = html.escape(source)
-        if color != "#ffffff":
-            source = f"<span style='{attribute}:{color}'>{source}</span>"
-        self._parts.append(source)
+        if color == "#ffffff":
+            self._parts.append(source)
+        else:
+            for part in filter(None, _RE_WHITESPACE.split(source)):
+                if _RE_WHITESPACE.fullmatch(part) is None:
+                    part = f"<span style='{attribute}:{color}'>{part}</span>"
+                self._parts.append(part)
 
     def emit(self) -> str:
         """Emit the HTML."""
         return "".join([*self._parts, "</pre></body></html>"])
 
     def _color(self, stats: "_Stats") -> str:
         """Compute an RGB color code for this chunk."""
@@ -142,34 +163,44 @@
 
 
 def _is_superduperinstruction(instruction: dis.Instruction | None) -> bool:
     """Check if an instruction is a superduperinstruction."""
     return instruction is not None and instruction.opname in _SUPERDUPERINSTRUCTIONS
 
 
-def _adaptive_counter_value(instruction: dis.Instruction, raw_bytecode: bytes) -> int:
+def _adaptive_counter_value(
+    instruction: dis.Instruction, raw_bytecode: bytes
+) -> tuple[int, int]:
     """Get the value of the adaptive counter for this instruction."""
     next_code_unit = raw_bytecode[instruction.offset + 2 : instruction.offset + 4]
     counter = int.from_bytes(next_code_unit, sys.byteorder)
-    return counter >> 4
+    return counter >> 4, counter & 0b1111
 
 
 def _score_instruction(
     instruction: dis.Instruction,
     previous: dis.Instruction | None,
     previous_previous: dis.Instruction | None,
     raw_bytecode: bytes,
 ) -> "_Stats":
     """Return stats for the given instruction."""
     if _is_superinstruction(previous) or _is_superduperinstruction(previous_previous):
         return _Stats(specialized=True)
-    if instruction.opname in _SPECIALIZED_INSTRUCTIONS:
-        if not instruction.opname.endswith("_ADAPTIVE"):
+    if sys.version_info < (3, 12):  # pragma: no cover
+        if instruction.opname in _SPECIALIZED_INSTRUCTIONS:
+            if not instruction.opname.endswith("_ADAPTIVE"):
+                return _Stats(specialized=True)
+            if any(_adaptive_counter_value(instruction, raw_bytecode)):
+                return _Stats(adaptive=True)
+    else:  # pragma: no cover
+        if instruction.opname in _SPECIALIZED_INSTRUCTIONS:
             return _Stats(specialized=True)
-        if _adaptive_counter_value(instruction, raw_bytecode):
+        if instruction.opname in _CACHE_FORMAT and _adaptive_counter_value(
+            instruction, raw_bytecode
+        ) > (1, 1):
             return _Stats(adaptive=True)
     return _Stats(unquickened=True)
 
 
 @contextlib.contextmanager
 def _catch_exceptions() -> typing.Generator[list[BaseException], None, None]:
     """Suppress exceptions, and gather them into a list."""
@@ -352,16 +383,17 @@
     quickened = False
     for source, stats in _source_and_stats(path):
         if stats.specialized or stats.adaptive:
             quickened = True
         writer.add(source, stats)
     if not quickened:
         _stderr(
-            f"No quickened code found in {name or path}! Try modifying it to run "
-            f"longer, or use the --targets option to analyze different source files."
+            f"The current process contains no quickened code for {name or path}! Try "
+            f"modifying it to run longer, or use the --targets option to analyze "
+            f"different source files."
         )
         return False
     written = writer.emit()
     if out is not None:
         out.parent.mkdir(parents=True, exist_ok=True)
         out.unlink(missing_ok=True)
         out.write_text(written)
```

