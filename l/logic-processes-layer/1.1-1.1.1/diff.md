# Comparing `tmp/logic_processes_layer-1.1.tar.gz` & `tmp/logic_processes_layer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logic_processes_layer-1.1.tar", last modified: Sat Jul 22 16:38:40 2023, max compression
+gzip compressed data, was "logic_processes_layer-1.1.1.tar", last modified: Sun Aug  6 11:12:33 2023, max compression
```

## Comparing `logic_processes_layer-1.1.tar` & `logic_processes_layer-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 gefest     (501) staff       (20)        0 2023-07-22 16:38:40.546482 logic_processes_layer-1.1/
--rw-r--r--   0 gefest     (501) staff       (20)     1073 2023-07-22 08:18:37.000000 logic_processes_layer-1.1/LICENSE
--rw-r--r--   0 gefest     (501) staff       (20)     8940 2023-07-22 16:38:40.546055 logic_processes_layer-1.1/PKG-INFO
--rw-r--r--   0 gefest     (501) staff       (20)     7320 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/README.md
-drwxr-xr-x   0 gefest     (501) staff       (20)        0 2023-07-22 16:38:40.541447 logic_processes_layer-1.1/logic_processes_layer/
--rw-r--r--   0 gefest     (501) staff       (20)       98 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/__init__.py
-drwxr-xr-x   0 gefest     (501) staff       (20)        0 2023-07-22 16:38:40.545196 logic_processes_layer-1.1/logic_processes_layer/abc/
--rw-r--r--   0 gefest     (501) staff       (20)        0 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/abc/__init__.py
--rw-r--r--   0 gefest     (501) staff       (20)      652 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/abc/abc_chain.py
--rw-r--r--   0 gefest     (501) staff       (20)      409 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/abc/abc_mapper.py
--rw-r--r--   0 gefest     (501) staff       (20)      882 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/abc/abc_pipeline.py
--rw-r--r--   0 gefest     (501) staff       (20)      175 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/context.py
--rw-r--r--   0 gefest     (501) staff       (20)      885 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/decorators.py
--rw-r--r--   0 gefest     (501) staff       (20)      342 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/meta.py
--rw-r--r--   0 gefest     (501) staff       (20)      667 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/processors.py
--rw-r--r--   0 gefest     (501) staff       (20)      301 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/results.py
--rw-r--r--   0 gefest     (501) staff       (20)      122 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/logic_processes_layer/structures.py
-drwxr-xr-x   0 gefest     (501) staff       (20)        0 2023-07-22 16:38:40.543305 logic_processes_layer-1.1/logic_processes_layer.egg-info/
--rw-r--r--   0 gefest     (501) staff       (20)     8940 2023-07-22 16:38:40.000000 logic_processes_layer-1.1/logic_processes_layer.egg-info/PKG-INFO
--rw-r--r--   0 gefest     (501) staff       (20)      618 2023-07-22 16:38:40.000000 logic_processes_layer-1.1/logic_processes_layer.egg-info/SOURCES.txt
--rw-r--r--   0 gefest     (501) staff       (20)        1 2023-07-22 16:38:40.000000 logic_processes_layer-1.1/logic_processes_layer.egg-info/dependency_links.txt
--rw-r--r--   0 gefest     (501) staff       (20)       22 2023-07-22 16:38:40.000000 logic_processes_layer-1.1/logic_processes_layer.egg-info/top_level.txt
--rw-r--r--   0 gefest     (501) staff       (20)     3306 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/pyproject.toml
--rw-r--r--   0 gefest     (501) staff       (20)       38 2023-07-22 16:38:40.546662 logic_processes_layer-1.1/setup.cfg
--rw-r--r--   0 gefest     (501) staff       (20)      625 2023-07-22 16:31:27.000000 logic_processes_layer-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:33.064317 logic_processes_layer-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-08-06 11:12:33.064317 logic_processes_layer-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:33.060317 logic_processes_layer-1.1.1/logic_processes_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:33.064317 logic_processes_layer-1.1.1/logic_processes_layer/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/abc/abc_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/abc/abc_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/abc/abc_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/logic_processes_layer/sub_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:12:33.064317 logic_processes_layer-1.1.1/logic_processes_layer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-08-06 11:12:33.000000 logic_processes_layer-1.1.1/logic_processes_layer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-06 11:12:33.000000 logic_processes_layer-1.1.1/logic_processes_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:12:33.000000 logic_processes_layer-1.1.1/logic_processes_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 11:12:33.000000 logic_processes_layer-1.1.1/logic_processes_layer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:12:33.064317 logic_processes_layer-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-06 11:12:18.000000 logic_processes_layer-1.1.1/setup.py
```

### Comparing `logic_processes_layer-1.1/LICENSE` & `logic_processes_layer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logic_processes_layer-1.1/PKG-INFO` & `logic_processes_layer-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logic_processes_layer
-Version: 1.1
+Version: 1.1.1
 Summary: Abstractions for create business logic
 Home-page: https://github.com/GefMar/logic_layer
 Author: Sergei (Gefest) Romanchuk
 License: MIT License
         
         Copyright (c) 2023 Sergey Romanchuk
         
@@ -43,15 +43,15 @@
 - **Flexibility**: Processes can be easily added, removed, or modified without affecting the rest of your program.
 
 - **Ease of testing**: By isolating each process, you can write more focused and effective unit tests.
 
 ## Installation
 
 You can install the logic_processes_layer package via pip:
-
+pip install logic-processes-layer==1.1
 
 ## Basic Usage
 
 Here is a basic example of how to use the logic_processes_layer package:
 
 ```python
 import dataclasses
```

### Comparing `logic_processes_layer-1.1/README.md` & `logic_processes_layer-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - **Flexibility**: Processes can be easily added, removed, or modified without affecting the rest of your program.
 
 - **Ease of testing**: By isolating each process, you can write more focused and effective unit tests.
 
 ## Installation
 
 You can install the logic_processes_layer package via pip:
-
+pip install logic-processes-layer==1.1
 
 ## Basic Usage
 
 Here is a basic example of how to use the logic_processes_layer package:
 
 ```python
 import dataclasses
```

### Comparing `logic_processes_layer-1.1/logic_processes_layer/abc/abc_chain.py` & `logic_processes_layer-1.1.1/logic_processes_layer/abc/abc_chain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 from abc import ABC, abstractmethod
 
-from ..structures import AttrsData
-from .abc_pipeline import AbstractPipelineStep
+if typing.TYPE_CHECKING:
+    from ..structures import AttrsData
+    from .abc_pipeline import AbstractPipelineStep
 
 
 class AbstractChainPipeline(ABC):
     def __call__(self):
         return self.run()
 
     @property
```

### Comparing `logic_processes_layer-1.1/logic_processes_layer/abc/abc_pipeline.py` & `logic_processes_layer-1.1.1/logic_processes_layer/abc/abc_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import typing
 from abc import ABC, abstractmethod
 
-from ..processors import BaseProcessor
-from ..structures import AttrsData
-from .abc_mapper import AbstractMapper
+if typing.TYPE_CHECKING:
+    from ..processors import BaseProcessor
+    from ..structures import AttrsData
+    from .abc_mapper import AbstractMapper
 
 
 @dataclasses.dataclass
 class AbstractPipelineStep(ABC):
     start_attrs: AttrsData
 
     def __call__(self, prev_results=None):
```

### Comparing `logic_processes_layer-1.1/logic_processes_layer/decorators.py` & `logic_processes_layer-1.1.1/logic_processes_layer/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,22 @@
     "make_run",
     "run_subprocesses",
 )
 
 import typing
 from functools import wraps
 
-from . import context
+if typing.TYPE_CHECKING:
+    from . import context
+    from .sub_processors import BaseSubprocessor
 
 
-def run_subprocesses(processor: typing.Callable, context_instance: "context.BaseProcessorContext"):
+def run_subprocesses(
+    processor: typing.Union[typing.Callable, "BaseSubprocessor"], context_instance: "context.BaseProcessorContext"
+):
     kwargs = {}
     if getattr(processor, "allow_context", False):
         processor.context = context_instance  # type: ignore
         kwargs["context"] = context_instance
     return processor(**kwargs)
```

### Comparing `logic_processes_layer-1.1/logic_processes_layer/processors.py` & `logic_processes_layer-1.1.1/logic_processes_layer/processors.py`

 * *Files identical despite different names*

### Comparing `logic_processes_layer-1.1/logic_processes_layer.egg-info/PKG-INFO` & `logic_processes_layer-1.1.1/logic_processes_layer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logic-processes-layer
-Version: 1.1
+Version: 1.1.1
 Summary: Abstractions for create business logic
 Home-page: https://github.com/GefMar/logic_layer
 Author: Sergei (Gefest) Romanchuk
 License: MIT License
         
         Copyright (c) 2023 Sergey Romanchuk
         
@@ -43,15 +43,15 @@
 - **Flexibility**: Processes can be easily added, removed, or modified without affecting the rest of your program.
 
 - **Ease of testing**: By isolating each process, you can write more focused and effective unit tests.
 
 ## Installation
 
 You can install the logic_processes_layer package via pip:
-
+pip install logic-processes-layer==1.1
 
 ## Basic Usage
 
 Here is a basic example of how to use the logic_processes_layer package:
 
 ```python
 import dataclasses
```

### Comparing `logic_processes_layer-1.1/logic_processes_layer.egg-info/SOURCES.txt` & `logic_processes_layer-1.1.1/logic_processes_layer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 logic_processes_layer/__init__.py
 logic_processes_layer/context.py
 logic_processes_layer/decorators.py
 logic_processes_layer/meta.py
 logic_processes_layer/processors.py
 logic_processes_layer/results.py
 logic_processes_layer/structures.py
+logic_processes_layer/sub_processors.py
 logic_processes_layer.egg-info/PKG-INFO
 logic_processes_layer.egg-info/SOURCES.txt
 logic_processes_layer.egg-info/dependency_links.txt
 logic_processes_layer.egg-info/top_level.txt
 logic_processes_layer/abc/__init__.py
 logic_processes_layer/abc/abc_chain.py
 logic_processes_layer/abc/abc_mapper.py
```

### Comparing `logic_processes_layer-1.1/pyproject.toml` & `logic_processes_layer-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "logic_processes_layer"
-version = "1.1"
+version = "1.1.1"
 description = "Abstractions for create business logic"
 readme = "README.md"
 authors = [
     { name = "Sergei (Gefest) Romanchuk" }
 ]
 license = { file = "LICENSE" }
 urls = { homepage = "https://github.com/GefMar/logic_layer" }
```

### Comparing `logic_processes_layer-1.1/setup.py` & `logic_processes_layer-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="logic_processes_layer",
-    version="1.1",
+    version="1.1.1",
     description="Abstractions for create business logic",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GefMar/logic_layer",
     author="Sergei (Gefest) Romanchuk",
     license="MIT",
     packages=find_packages(),
```

