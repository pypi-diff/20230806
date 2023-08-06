# Comparing `tmp/creart-graia-0.1.4.tar.gz` & `tmp/creart-graia-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creart-graia-0.1.4.tar", last modified: Sat Jun 25 07:51:38 2022, max compression
+gzip compressed data, was "creart-graia-0.1.5.tar", last modified: Fri Jul  1 04:21:13 2022, max compression
```

## Comparing `creart-graia-0.1.4.tar` & `creart-graia-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-25 07:51:18.503503 creart-graia-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-25 07:51:18.503503 creart-graia-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-25 07:51:18.503503 creart-graia-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 07:51:18.503503 creart-graia-0.1.4/src/graia/creart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-06-25 07:51:18.503503 creart-graia-0.1.4/src/graia/creart/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-06-25 07:51:18.503503 creart-graia-0.1.4/src/graia/creart/saya.py
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-06-25 07:51:18.503503 creart-graia-0.1.4/src/graia/creart/scheduler.py
--rw-------   0 runner    (1001) docker     (121)      229 2022-06-25 07:51:38.343775 creart-graia-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-07-01 04:21:00.552307 creart-graia-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-01 04:21:00.552307 creart-graia-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-07-01 04:21:00.552307 creart-graia-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/saya.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-07-01 04:21:00.552307 creart-graia-0.1.5/src/graia/creart/scheduler.py
+-rw-------   0 runner    (1001) docker     (121)      229 2022-07-01 04:21:13.936357 creart-graia-0.1.5/PKG-INFO
```

### Comparing `creart-graia-0.1.4/LICENSE` & `creart-graia-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `creart-graia-0.1.4/pyproject.toml` & `creart-graia-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "creart-graia"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "creart>=0.1.0",
 ]
@@ -13,14 +13,15 @@
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 
 [project.entry-points."creart.creators"]
+loop = "graia.creart.broadcast:EventLoopCreator"
 broadcast = "graia.creart.broadcast:BroadcastCreator"
 broadcast_behaviour = "graia.creart.broadcast:BroadcastBehaviourCreator"
 saya = "graia.creart.saya:SayaCreator"
 scheduler = "graia.creart.scheduler:SchedulerCreator"
 scheduler_behaviour = "graia.creart.scheduler:SchedulerBehaviourCreator"
 
 [tool.pdm]
```

### Comparing `creart-graia-0.1.4/src/graia/creart/broadcast.py` & `creart-graia-0.1.5/src/graia/creart/broadcast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 from __future__ import annotations
 
+import asyncio
+from asyncio import AbstractEventLoop
 from typing import TYPE_CHECKING
 
 from creart import AbstractCreator, CreateTargetInfo, exists_module, it, mixin
 
 if TYPE_CHECKING:
     from graia.broadcast import Broadcast
     from graia.broadcast.interrupt import InterruptControl
     from graia.saya.builtins.broadcast.behaviour import BroadcastBehaviour
 
 
+class EventLoopCreator(AbstractCreator):
+    targets = (CreateTargetInfo("asyncio.events", "AbstractEventLoop"),)
+
+    @staticmethod
+    def create(_: type[AbstractEventLoop]) -> AbstractEventLoop:
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        return loop
+
+
 class BroadcastCreator(AbstractCreator):
     targets = (
         CreateTargetInfo(
             module="graia.broadcast",
             identify="Broadcast",
             humanized_name="Broadcast Control",
             description="<common,graia,broadcast> a high performance, highly customizable, elegantly designed event system based on asyncio",
@@ -36,19 +48,15 @@
     def create(
         create_type: type[Broadcast | InterruptControl],
     ) -> Broadcast | InterruptControl:
         from graia.broadcast import Broadcast
         from graia.broadcast.interrupt import InterruptControl
 
         if issubclass(create_type, Broadcast):
-            import asyncio
-
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-            return create_type(loop=loop)
+            return create_type(loop=it(AbstractEventLoop))
         elif issubclass(create_type, InterruptControl):
             return create_type(it(Broadcast))
 
 
 class BroadcastBehaviourCreator(AbstractCreator):
     targets = (
         CreateTargetInfo(
```

### Comparing `creart-graia-0.1.4/src/graia/creart/saya.py` & `creart-graia-0.1.5/src/graia/creart/saya.py`

 * *Files identical despite different names*

### Comparing `creart-graia-0.1.4/src/graia/creart/scheduler.py` & `creart-graia-0.1.5/src/graia/creart/scheduler.py`

 * *Files identical despite different names*

