# Comparing `tmp/graia_scheduler-0.2.0.tar.gz` & `tmp/graia_scheduler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graia_scheduler-0.2.0.tar", last modified: Sat Aug  5 13:20:46 2023, max compression
+gzip compressed data, was "graia_scheduler-0.3.0.tar", last modified: Sun Aug  6 13:35:28 2023, max compression
```

## Comparing `graia_scheduler-0.2.0.tar` & `graia_scheduler-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1273 2023-08-05 13:20:29.729066 graia_scheduler-0.2.0/README.md
--rw-r--r--   0        0        0     1151 2023-08-05 13:20:46.945672 graia_scheduler-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2521 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/__init__.py
--rw-r--r--   0        0        0     1692 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/creator.py
--rw-r--r--   0        0        0       91 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/exception.py
--rw-r--r--   0        0        0      129 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/__init__.py
--rw-r--r--   0        0        0     1330 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/behaviour.py
--rw-r--r--   0        0        0      471 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/saya/schema.py
--rw-r--r--   0        0        0     1113 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/service.py
--rw-r--r--   0        0        0     4760 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/task.py
--rw-r--r--   0        0        0     3679 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/timers.py
--rw-r--r--   0        0        0     1524 2023-08-05 13:20:29.733066 graia_scheduler-0.2.0/src/graia/scheduler/utilles.py
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 graia_scheduler-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/README.md
+-rw-r--r--   0        0        0     1151 2023-08-06 13:35:28.675331 graia_scheduler-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2521 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/__init__.py
+-rw-r--r--   0        0        0     1692 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/creator.py
+-rw-r--r--   0        0        0       91 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/exception.py
+-rw-r--r--   0        0        0      129 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/saya/__init__.py
+-rw-r--r--   0        0        0     1330 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/saya/behaviour.py
+-rw-r--r--   0        0        0      471 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/saya/schema.py
+-rw-r--r--   0        0        0     1107 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/service.py
+-rw-r--r--   0        0        0     4760 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/task.py
+-rw-r--r--   0        0        0     3679 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/timers.py
+-rw-r--r--   0        0        0     1524 2023-08-06 13:35:13.179038 graia_scheduler-0.3.0/src/graia/scheduler/utilles.py
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 graia_scheduler-0.3.0/PKG-INFO
```

### Comparing `graia_scheduler-0.2.0/README.md` & `graia_scheduler-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/pyproject.toml` & `graia_scheduler-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 authors = [
     { name = "GreyElaina", email = "31543961+GreyElaina@users.noreply.github.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "graia-broadcast~=0.23.0",
     "croniter<2.0.0,>=1.0.0",
-    "launart~=0.6.4",
+    "launart>=0.7.0",
     "creart~=0.3.0",
 ]
 name = "graia-scheduler"
-version = "0.2.0"
+version = "0.3.0"
 description = "a scheduler for graia framework"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
```

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/__init__.py` & `graia_scheduler-0.3.0/src/graia/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/creator.py` & `graia_scheduler-0.3.0/src/graia/scheduler/creator.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/saya/behaviour.py` & `graia_scheduler-0.3.0/src/graia/scheduler/saya/behaviour.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/service.py` & `graia_scheduler-0.3.0/src/graia/scheduler/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal, Set
-from launart import Launchable, Launart
+from launart import Service, Launart
 from . import GraiaScheduler
 import asyncio
 
 
-class SchedulerService(Launchable):
+class SchedulerService(Service):
     """GraiaScheduler 的 Launart 服务
 
     Args:
         scheduler (GraiaScheduler): 任务计划器
     """
 
     id = "scheduler.service"
```

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/task.py` & `graia_scheduler-0.3.0/src/graia/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/timers.py` & `graia_scheduler-0.3.0/src/graia/scheduler/timers.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/src/graia/scheduler/utilles.py` & `graia_scheduler-0.3.0/src/graia/scheduler/utilles.py`

 * *Files identical despite different names*

### Comparing `graia_scheduler-0.2.0/PKG-INFO` & `graia_scheduler-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: graia-scheduler
-Version: 0.2.0
+Version: 0.3.0
 Summary: a scheduler for graia framework
 Author-Email: GreyElaina <31543961+GreyElaina@users.noreply.github.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Requires-Dist: graia-broadcast~=0.23.0
 Requires-Dist: croniter<2.0.0,>=1.0.0
-Requires-Dist: launart~=0.6.4
+Requires-Dist: launart>=0.7.0
 Requires-Dist: creart~=0.3.0
 Requires-Dist: graia-saya<0.1,>=0.0.16; extra == "saya"
 Provides-Extra: saya
 Description-Content-Type: text/markdown
 
 # Graia Scheduler
```

