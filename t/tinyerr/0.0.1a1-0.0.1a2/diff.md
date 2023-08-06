# Comparing `tmp/tinyerr-0.0.1a1.tar.gz` & `tmp/tinyerr-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyerr-0.0.1a1.tar", last modified: Sun May 28 08:02:09 2023, max compression
+gzip compressed data, was "tinyerr-0.0.1a2.tar", last modified: Sun Aug  6 09:53:39 2023, max compression
```

## Comparing `tinyerr-0.0.1a1.tar` & `tinyerr-0.0.1a2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.361466 tinyerr-0.0.1a1/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-05-15 09:32:44.000000 tinyerr-0.0.1a1/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-05-28 08:02:09.361327 tinyerr-0.0.1a1/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1183 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      441 2023-05-28 08:01:43.000000 tinyerr-0.0.1a1/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-05-28 08:02:09.361512 tinyerr-0.0.1a1/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.359089 tinyerr-0.0.1a1/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.360463 tinyerr-0.0.1a1/src/tinyerr/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       43 2023-05-15 06:51:07.000000 tinyerr-0.0.1a1/src/tinyerr/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      468 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/src/tinyerr/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3013 2023-05-28 07:57:36.000000 tinyerr-0.0.1a1/src/tinyerr/anchor.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     7680 2023-05-28 07:59:15.000000 tinyerr-0.0.1a1/src/tinyerr/errors.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1342 2023-05-17 08:13:53.000000 tinyerr-0.0.1a1/src/tinyerr/exechook.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2807 2023-05-17 06:55:24.000000 tinyerr-0.0.1a1/src/tinyerr/frames.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-05-28 08:02:09.361156 tinyerr-0.0.1a1/src/tinyerr.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      348 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       45 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        8 2023-05-28 08:02:09.000000 tinyerr-0.0.1a1/src/tinyerr.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-08-06 09:53:39.904547 tinyerr-0.0.1a2/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2023-05-15 09:32:44.000000 tinyerr-0.0.1a2/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-08-06 09:53:39.904411 tinyerr-0.0.1a2/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1183 2023-05-17 08:13:53.000000 tinyerr-0.0.1a2/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      441 2023-06-16 07:07:25.000000 tinyerr-0.0.1a2/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-08-06 09:53:39.904589 tinyerr-0.0.1a2/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-08-06 09:53:39.900466 tinyerr-0.0.1a2/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-08-06 09:53:39.903385 tinyerr-0.0.1a2/src/tinyerr/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       43 2023-05-15 06:51:07.000000 tinyerr-0.0.1a2/src/tinyerr/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1402 2023-06-17 01:51:23.000000 tinyerr-0.0.1a2/src/tinyerr/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3013 2023-05-28 07:57:36.000000 tinyerr-0.0.1a2/src/tinyerr/anchor.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      558 2023-08-06 07:37:36.000000 tinyerr-0.0.1a2/src/tinyerr/config.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     7580 2023-06-17 01:32:49.000000 tinyerr-0.0.1a2/src/tinyerr/errors.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1049 2023-06-16 09:44:40.000000 tinyerr-0.0.1a2/src/tinyerr/exechook.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2971 2023-06-16 09:52:25.000000 tinyerr-0.0.1a2/src/tinyerr/frames.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-08-06 09:53:39.904191 tinyerr-0.0.1a2/src/tinyerr.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2687 2023-08-06 09:53:39.000000 tinyerr-0.0.1a2/src/tinyerr.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      370 2023-08-06 09:53:39.000000 tinyerr-0.0.1a2/src/tinyerr.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-08-06 09:53:39.000000 tinyerr-0.0.1a2/src/tinyerr.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       45 2023-08-06 09:53:39.000000 tinyerr-0.0.1a2/src/tinyerr.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        8 2023-08-06 09:53:39.000000 tinyerr-0.0.1a2/src/tinyerr.egg-info/top_level.txt
```

### Comparing `tinyerr-0.0.1a1/LICENSE` & `tinyerr-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyerr-0.0.1a1/PKG-INFO` & `tinyerr-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyerr
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Tiny Errors that remove the clutter
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tinyerr-0.0.1a1/README.md` & `tinyerr-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `tinyerr-0.0.1a1/src/tinyerr/anchor.py` & `tinyerr-0.0.1a2/src/tinyerr/anchor.py`

 * *Files identical despite different names*

### Comparing `tinyerr-0.0.1a1/src/tinyerr/errors.py` & `tinyerr-0.0.1a2/src/tinyerr/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
-from pathlib import Path
 from re import Pattern
 from traceback import FrameSummary, StackSummary, extract_tb
 from types import TracebackType
 from typing import Self, Type, TypeVar
 
+from tinyerr.config import ExecHandling
 from tinyerr.frames import format_frame, frame_is_raise_statement
 
 Err = TypeVar("Err", bound=BaseException)
 
 COMMON_TYPE_NAMES = {
     "builtin_function_or_method": "function",
     "method-wrapper": "method",
@@ -19,66 +19,49 @@
     return COMMON_TYPE_NAMES.get(name, name)
 
 
 class Error:
     type: Type[Exception] = Exception
     pattern: Pattern = re.compile(".")
 
-    def __init__(
-            self,
-            exception: Err,
-            stack: StackSummary,
-            traceback_limit: int,
-            frame_context: Path | None = None
-    ):
+    def __init__(self, exception: Err, stack: StackSummary):
         self.exception = exception
         self.stack = stack
-        self.traceback_limit = traceback_limit
-        self.frame_context = frame_context
 
         context = exception.__context__
         suppress_context = exception.__suppress_context__
         cause = exception.__cause__
 
         self.context = None
         if context is not None and not suppress_context:
-            self.context = Error.from_exception(
-                context, context.__traceback__, traceback_limit, frame_context,
-            )
+            self.context = Error.from_exception(context, context.__traceback__)
 
         self.cause = None
         if cause is not None:
-            self.cause = Error.from_exception(
-                cause, cause.__traceback__, traceback_limit, frame_context
-            )
+            self.cause = Error.from_exception(cause, cause.__traceback__)
 
     @classmethod
-    def from_exception(
-            cls,
-            exception: Err,
-            traceback: TracebackType,
-            traceback_limit: int,
-            context: Path | None = None,
-    ) -> Self:
+    def from_exception(cls, exception: Err, traceback: TracebackType) -> Self:
         stack = extract_tb(traceback)
         for subtype in cls.__subclasses__():
             if (isinstance(exception, subtype.type)
                     and subtype.pattern.match(str(exception))):
-                return subtype(exception, stack, traceback_limit, context)
-        return cls(exception, stack, traceback_limit, context)
+                return subtype(exception, stack)
+        return cls(exception, stack)
 
     def frames(self) -> StackSummary:
         frames = self.stack
-        frames = StackSummary.from_list(
-            [f for f in frames if not frame_is_raise_statement(f)]
-        )
-        if self.frame_context is not None:
+        if ExecHandling.suppress_raise:
+            frames = StackSummary.from_list(
+                [f for f in frames if not frame_is_raise_statement(f)]
+            )
+        if ExecHandling.parent_context is not None:
             idx = next(
                 (i for i, frame in enumerate(self.stack)
-                 if self.frame_context.samefile(frame.filename)),
+                 if ExecHandling.parent_context.samefile(frame.filename)),
                 -1
             )
             return frames[idx + 1:]
         return frames
 
     def formatted_frames(self, limit: int = 1) -> str:
         return "\n\n".join(
@@ -110,15 +93,15 @@
                 "The following occurred while handling the above exception:"
             )
         result.append(self.formatted_frames(limit))
         result.append(self.message_with_type())
         return "\n\n".join(r for r in result if r)
 
     def __str__(self):
-        return self.trace(self.traceback_limit)
+        return self.trace(ExecHandling.traceback_limit)
 
 
 class SyntaxErr(Error):
     type = SyntaxError
     pattern = re.compile(".*")
 
     def frames(self) -> StackSummary:
@@ -254,7 +237,20 @@
     )
 
     def message(self) -> str:
         # TODO – come up with something better
         # No type information is in the error or trace – making it difficult
         # to provide a nice error message. Misses __index__ as valid slice item
         return f"Slice indices must be of type <int> or left blank"
+
+
+class ImportNameError(Error):
+    type = ImportError
+    pattern = re.compile(
+        "cannot import name '(?P<name>.*)' from '(?P<module>.*)' .*"
+    )
+
+    def message(self) -> str:
+        return (
+            f"`{self.groups['name']}` not found in "
+            f"module `{self.groups['module']}`"
+        )
```

### Comparing `tinyerr-0.0.1a1/src/tinyerr/exechook.py` & `tinyerr-0.0.1a2/src/tinyerr/exechook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 import sys
-from pathlib import Path
 from types import TracebackType
 from typing import Type
 
+from tinyerr.config import Formatting
 from tinyerr.errors import Error
 
-PARENT_CONTEXT: Path | None = None
-TRACEBACK_LIMIT = 0
 
-
-def activate(file: str | None = None, traceback_limit: int | None = None):
+def activate():
     """
     Changes sys.excepthook to use TinyErr exception handling
 
     The file parameter specifies a "cutoff" file for frames in traceback
     stacks. Any frames above and including the first frame whose file
     location is the given parameter file will not be included in TinyErr
     tracebacks. This is useful when using tinyerr to run other user given code.
     """
-    global PARENT_CONTEXT
-    global TRACEBACK_LIMIT
-    if file is not None:
-        PARENT_CONTEXT = Path(file)
-    if traceback_limit is not None:
-        TRACEBACK_LIMIT = traceback_limit
     sys.excepthook = excepthook
 
 
 def deactivate():
     """Reverts sys.excepthook to the Python default"""
     sys.excepthook = sys.__excepthook__
 
 
 def excepthook(
         except_type: Type[Exception],
         except_value: Exception,
         tracebac: TracebackType,
 ):
     """TinyErrs custom excepthook"""
-    err = Error.from_exception(
-        except_value, tracebac, TRACEBACK_LIMIT, PARENT_CONTEXT,
-    )
-    print(red(str(err)), file=sys.stderr)
+    err = Error.from_exception(except_value, tracebac)
+    err = red(str(err)) if Formatting.is_red else str(err)
+    print(err, file=sys.stderr)
 
 
 def red(msg: str) -> str:
     return f"\x1b[31m{msg}\x1b[0m"
```

### Comparing `tinyerr-0.0.1a1/src/tinyerr/frames.py` & `tinyerr-0.0.1a2/src/tinyerr/frames.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 import linecache
 import textwrap
 from pathlib import Path
 from traceback import FrameSummary
 
 from tinyerr.anchor import Anchor
+from tinyerr.config import Formatting
 
 
 def get_offsets(frame: FrameSummary, line: str) -> tuple[int, int]:
     """
     Returns the offsets associated with the given frame and line (not lstripped)
     """
     start_offset = frame.colno + 1
@@ -60,15 +61,19 @@
 
 def frame_location(frame: FrameSummary) -> str:
     """
     Returns a readable string describing the location of the frame.
     Uses relative paths where possible
     """
     path = _short_path(frame.filename)
-    return f"File \"{path}\", line {frame.lineno}, in {frame.name}"
+    return Formatting.frame_info.format(
+        file=path, name=frame.name,
+        lineno=frame.lineno, end_lineno=frame.end_lineno,
+        colno=frame.colno, end_colno=frame.end_colno
+    )
 
 
 def format_frame(frame: FrameSummary) -> str:
     """
     Returns a formatted text block of the frame location and code line::
 
         File "<path>", line <line>, in <scope>
```

### Comparing `tinyerr-0.0.1a1/src/tinyerr.egg-info/PKG-INFO` & `tinyerr-0.0.1a2/src/tinyerr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyerr
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Tiny Errors that remove the clutter
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

