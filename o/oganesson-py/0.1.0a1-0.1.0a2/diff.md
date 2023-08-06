# Comparing `tmp/oganesson_py-0.1.0a1.tar.gz` & `tmp/oganesson_py-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson_py-0.1.0a1.tar", max compression
+gzip compressed data, was "oganesson_py-0.1.0a2.tar", max compression
```

## Comparing `oganesson_py-0.1.0a1.tar` & `oganesson_py-0.1.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      106 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/README.md
--rw-r--r--   0        0        0        0 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/__init__.py
--rw-r--r--   0        0        0       95 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analyser/__init__.py
--rw-r--r--   0        0        0      580 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analyser/analyser.py
--rw-r--r--   0        0        0     1531 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analyser/builder.py
--rw-r--r--   0        0        0     2207 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analyser/cyclomatic_complexity.py
--rw-r--r--   0        0        0     1391 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analyser/maintainability_index.py
--rw-r--r--   0        0        0      764 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/analysis.py
--rw-r--r--   0        0        0      127 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/exceptions.py
--rw-r--r--   0        0        0      991 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/filetree.py
--rw-r--r--   0        0        0     2774 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/main.py
--rw-r--r--   0        0        0      404 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/reporter.py
--rw-r--r--   0        0        0      697 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/oganesson_py/validators.py
--rw-r--r--   0        0        0      511 2023-08-06 15:21:45.758414 oganesson_py-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 oganesson_py-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     3638 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/__init__.py
+-rw-r--r--   0        0        0       95 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analyser/__init__.py
+-rw-r--r--   0        0        0      570 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analyser/analyser.py
+-rw-r--r--   0        0        0     1503 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analyser/builder.py
+-rw-r--r--   0        0        0     2179 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analyser/cyclomatic_complexity.py
+-rw-r--r--   0        0        0     1328 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analyser/maintainability_index.py
+-rw-r--r--   0        0        0      754 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/analysis.py
+-rw-r--r--   0        0        0      127 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/exceptions.py
+-rw-r--r--   0        0        0      991 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/filetree.py
+-rw-r--r--   0        0        0     2774 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/main.py
+-rw-r--r--   0        0        0      404 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/reporter.py
+-rw-r--r--   0        0        0      769 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/oganesson_py/validators.py
+-rw-r--r--   0        0        0      535 2023-08-06 16:08:17.948588 oganesson_py-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 oganesson_py-0.1.0a2/PKG-INFO
```

### Comparing `oganesson_py-0.1.0a1/LICENSE` & `oganesson_py-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson_py-0.1.0a1/oganesson_py/analyser/analyser.py` & `oganesson_py-0.1.0a2/oganesson_py/analyser/analyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Optional, Protocol
+from typing import Protocol
 
 
 class Result(Protocol):
     def pretty(self) -> str:
         ...
```

### Comparing `oganesson_py-0.1.0a1/oganesson_py/analyser/builder.py` & `oganesson_py-0.1.0a2/oganesson_py/analyser/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from typing import Optional
 
 from oganesson_py.analyser.maintainability_index import MIAnalyser
 
 from .analyser import Analyser, RootAnalyser
 from .cyclomatic_complexity import CCAnalyser
```

### Comparing `oganesson_py-0.1.0a1/oganesson_py/analyser/cyclomatic_complexity.py` & `oganesson_py-0.1.0a2/oganesson_py/analyser/cyclomatic_complexity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from pydoc import classname
 
 from typing import Optional
 from pydantic import BaseModel
 
 from colorama import Fore
 
 from radon.complexity import cc_visit
```

### Comparing `oganesson_py-0.1.0a1/oganesson_py/analyser/maintainability_index.py` & `oganesson_py-0.1.0a2/oganesson_py/analyser/maintainability_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
-from pydoc import classname
 
 from typing import Optional
 from pydantic import BaseModel
 
 from colorama import Fore
 
 from radon.metrics import mi_visit
-from radon.visitors import Function
 
 from .analyser import Analyser, Result
 
 
 class MIAnalyser:
     def __init__(
         self,
@@ -26,15 +24,15 @@
     def set_next(self, next_analyser: Analyser):
         self.next = next_analyser
 
     def __call__(self, file: str) -> list[Result]:
         other_results = self.next(file) if self.next else []
 
         result = mi_visit(file, multi=self.multi_as_comments)
-        if result < self.threshold:
+        if result <= self.threshold:
             other_results.append(MIResult(mi=result))
 
         return other_results
 
 
 class MIResult(BaseModel):
     mi: float
```

### Comparing `oganesson_py-0.1.0a1/oganesson_py/analysis.py` & `oganesson_py-0.1.0a2/oganesson_py/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List, Protocol
+from typing import List
 from pathlib import Path
 
 
 from .analyser import Analyser, Result
 
 
 @dataclass
```

### Comparing `oganesson_py-0.1.0a1/oganesson_py/filetree.py` & `oganesson_py-0.1.0a2/oganesson_py/filetree.py`

 * *Files identical despite different names*

### Comparing `oganesson_py-0.1.0a1/oganesson_py/main.py` & `oganesson_py-0.1.0a2/oganesson_py/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     max_cc: int,
     min_mi: float,
     mi_multiline_comments: bool,
     trigger: bool,
     ignore: set[str],
 ):
     """
-    # Pyquality
+    # Oganesson
 
     A CLI for running quality metrics on Python code.  Currently a wrapper
     around Radon, with intent to add a few extra metrics in time.
 
     Whereas radon has flake8 support, and xenon is designed to work in a CI for
     cyclometric complexity, the maintainability index isn't supported in CI out
     of the box.  This tool produces a report to the stdout of all instances
```

