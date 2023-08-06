# Comparing `tmp/pypomes_scheduling-0.2.4.tar.gz` & `tmp/pypomes_scheduling-0.2.6.tar.gz`

## Comparing `pypomes_scheduling-0.2.4.tar` & `pypomes_scheduling-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/__init__.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/__threaded_scheduler.py
--rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/src/pypomes_scheduling/scheduling_pomes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/src/pypomes_scheduling/__init__.py
+-rw-r--r--   0        0        0     9751 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/src/pypomes_scheduling/scheduling_pomes.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/src/pypomes_scheduling/threaded_scheduler.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 pypomes_scheduling-0.2.6/PKG-INFO
```

### Comparing `pypomes_scheduling-0.2.4/src/pypomes_scheduling/__threaded_scheduler.py` & `pypomes_scheduling-0.2.6/src/pypomes_scheduling/threaded_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from apscheduler.schedulers.blocking import BlockingScheduler
 from apscheduler.triggers.cron import CronTrigger
 import logging
 import pytz
 import threading
 
 
-class __ThreadedScheduler(threading.Thread):
+class _ThreadedScheduler(threading.Thread):
     """
     A scalable implementation of *APScheduler*'s *BlockingScheduler*.
 
     This implementation may run as single or multiple instances, each on its own thread.
     """
     _scheduler: BlockingScheduler
     _logger: logging.Logger
@@ -79,15 +79,15 @@
                 cron_expr = job_cron
 
         aps_trigger: CronTrigger | None = None
         # has the CRON expression been defined ?
         if cron_expr is not None:
             # yes, build the trigger: <minute> <hour> <day-of-month> <month> <day-of-week>
             vals: list[str] = cron_expr.split()
-            vals = [None if val == '?' else val for val in vals]
+            vals = [None if val == "?" else val for val in vals]
             aps_trigger = CronTrigger(minute=vals[0],
                                       hour=vals[1],
                                       day=vals[2],
                                       month=vals[3],
                                       day_of_week=vals[4],
                                       start_date=job_start)
         self._scheduler.add_job(func=job,
```

### Comparing `pypomes_scheduling-0.2.4/src/pypomes_scheduling/scheduling_pomes.py` & `pypomes_scheduling-0.2.6/src/pypomes_scheduling/scheduling_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from datetime import datetime
 from pypomes_core import exc_format
 from typing import Final
 import logging
 import pytz
 import re
 import sys
-from .__threaded_scheduler import __ThreadedScheduler
+from .threaded_scheduler import _ThreadedScheduler
 
 __DEFAULT_BADGE: Final[str] = "__default__"
 
 __REGEX_VERIFY_CRON: Final[str] = (
     "/(@(annually|yearly|monthly|weekly|daily|hourly|reboot))|"
     "(@every (\d+(ns|us|µs|ms|s|m|h))+)|((((\d+,)+\d+|(\d+(\/|-)\d+)|\d+|\*) ?){5,7})"
 )
 
 # dict holding the schedulers created:
-#   { <badge-1>: <scheduler-instance-1>,
+#   <{ <badge-1>: <scheduler-instance-1>,
 #     ...
 #     <badge-n>: <scheduler-instance-n>
-#   }
+#   }>
 __schedulers: dict = {}
 
 
 def scheduler_create(errors: list[str], timezone: pytz.BaseTzInfo,
                      retry_interval: int, logger: logging.Logger = None, badge: str = None) -> bool:
     """
-    Create the threaded job scheduler. This is a wrapper around the package *APScheduler*.
+    Create the threaded job scheduler.
+
+    This is a wrapper around the package *APScheduler*.
 
     :param errors: incidental errors
     :param timezone: the timezone to be used
     :param retry_interval: interval between retry attempts, in minutes
     :param logger: optional logger object
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler was created, or False otherwise
@@ -40,15 +42,15 @@
     # define the badge
     curr_badge: str = badge or __DEFAULT_BADGE
     
     # has the scheduler been created ?
     if __get_scheduler(errors, curr_badge, False) is None:
         # no, create it
         try:
-            __schedulers[curr_badge] = __ThreadedScheduler(timezone, retry_interval, logger)
+            __schedulers[curr_badge] = _ThreadedScheduler(timezone, retry_interval, logger)
             __schedulers[curr_badge].daemon = True
             result = True
         except Exception as e:
             errors.append(f"Error creating the job scheduler '{curr_badge}': "
                           f"{exc_format(e, sys.exc_info())}")
 
     return result
@@ -58,18 +60,20 @@
     """
     Destroy the scheduler identified by *badge*. *Noop* if the scheduler does not exist.
 
     :param badge:  optional badge identifying the scheduler
     """
     # define the badge
     curr_badge: str = badge or __DEFAULT_BADGE
+    scheduler: _ThreadedScheduler = __schedulers.get(curr_badge)
 
     # does the scheduler exist ?
-    if __schedulers.get(curr_badge) is not None:
-        # yes, discard it
+    if scheduler is not None:
+        # yes, stop and discard it
+        scheduler.stop()
         __schedulers.pop(curr_badge)
 
 
 def scheduler_start(errors: list[str], badge: str = None) -> bool:
     """
     Start the scheduler.
 
@@ -77,15 +81,15 @@
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler has been started, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # retrieve the scheduler
-    scheduler: __ThreadedScheduler = __get_scheduler(errors, badge)
+    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
 
     # proceed, if the scheduler was retrieved
     if scheduler is not None:
         try:
             scheduler.start()
             result = True
         except Exception as e:
@@ -103,15 +107,15 @@
     :param badge: optional badge identifying the scheduler
     :return: True if the scheduler has been stopped, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # retrieve the scheduler
-    scheduler: __ThreadedScheduler = __get_scheduler(errors, badge)
+    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
 
     # proceed, if the scheduler was retrieved
     if scheduler is not None:
         scheduler.stop()
         result = True
 
     return result
@@ -139,15 +143,15 @@
     :param badge: optional badge identifying the scheduler
     :return: True if the job was successfully scheduled, or False otherwise
     """
     # initialize the return variable
     result: bool = False
     
     # retrieve the scheduler
-    scheduler: __ThreadedScheduler = __get_scheduler(errors, badge)
+    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
     
     # proceed, if the scheduler was retrieved
     if scheduler is not None:
         result = __scheduler_add_job(errors, scheduler, job, job_id, job_name,
                                      job_cron, job_start, job_args, job_kwargs)
 
     return result
@@ -168,15 +172,15 @@
     :param badge: optional badge identifying the scheduler
     :return: the number of jobs effectively scheduled
     """
     # initialize the return variable
     result: int = 0
 
     # retrieve the scheduler
-    scheduler: __ThreadedScheduler = __get_scheduler(errors, badge)
+    scheduler: _ThreadedScheduler = __get_scheduler(errors, badge)
     
     # proceed, if the scheduler was retrieved
     if scheduler is not None:
         # traverse the job list and attempt the scheduling
         for job in jobs:
             # process the optional arguments
             job_cron: str = job[3] if len(job) > 3 else None
@@ -187,32 +191,32 @@
             if __scheduler_add_job(errors, scheduler, job[0], job[1], job[2],
                                    job_cron, job_start, job_args, job_kwargs):
                 result += 1
 
     return result
 
 
-def __get_scheduler(errors: list[str], badge: str, must_exist: bool = True) -> __ThreadedScheduler:
+def __get_scheduler(errors: list[str], badge: str, must_exist: bool = True) -> _ThreadedScheduler:
     """
     Retrieve the scheduler identified by *badge*.
 
     :param errors: incidental errors
     :param badge: optional badge identifying the scheduler
     :param must_exist: True if scheduler must exist
     :return: the scheduler retrieved, or None otherwise
     """
     curr_badge = badge or __DEFAULT_BADGE
-    result: __ThreadedScheduler = __schedulers.get(curr_badge)
+    result: _ThreadedScheduler = __schedulers.get(curr_badge)
     if must_exist and result is None:
         errors.append(f"Job scheduler '{curr_badge}' has not been created")
         
     return result
 
 
-def __scheduler_add_job(errors: list[str], scheduler: __ThreadedScheduler,
+def __scheduler_add_job(errors: list[str], scheduler: _ThreadedScheduler,
                         job: callable, job_id: str, job_name: str,
                         job_cron: str = None, job_start: datetime = None,
                         job_args: tuple = None, job_kwargs: dict = None) -> bool:
     """
     Use *scheduler* to schedule the job identified as *job_id* and named as *job_name*.
 
     The scheduling is performed with the *CRON* expression *job_cron*, starting at the timestamp *job_start*.
```

### Comparing `pypomes_scheduling-0.2.4/LICENSE` & `pypomes_scheduling-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_scheduling-0.2.4/pyproject.toml` & `pypomes_scheduling-0.2.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_scheduling"
-version = "0.2.4"
+version = "0.2.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (scheduling module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.2.1",
-    "pypomes_core>=0.2.2",
+    "pypomes_core>=0.2.3",
     "APScheduler>=3.10.1",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Scheduling"
```

### Comparing `pypomes_scheduling-0.2.4/PKG-INFO` & `pypomes_scheduling-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pypomes_scheduling
-Version: 0.2.4
+Version: 0.2.6
 Summary: A collection of Python pomes, pennyeach (scheduling module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Scheduling
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Scheduling/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: apscheduler>=3.10.1
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.2
+Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

