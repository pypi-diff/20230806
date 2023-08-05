# Comparing `tmp/syct-0.4.3.tar.gz` & `tmp/syct-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nadavo/dev/Timer/dist/tmpp3icfkj0/syct-0.4.3.tar", last modified: Thu Oct 21 23:01:56 2021, max compression
+gzip compressed data, was "syct-0.4.4.tar", last modified: Sat Aug  5 22:04:12 2023, max compression
```

## Comparing `syct-0.4.3.tar` & `syct-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2021-10-21 23:01:56.377540 syct-0.4.3/
--rw-r--r--   0 nadavo    (1000) nadavo    (1000)     1067 2018-07-10 23:49:51.000000 syct-0.4.3/LICENSE
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1488 2021-10-21 23:01:56.377540 syct-0.4.3/PKG-INFO
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1017 2021-10-17 09:43:24.000000 syct-0.4.3/README.md
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      104 2021-05-09 10:23:59.000000 syct-0.4.3/pyproject.toml
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)       38 2021-10-21 23:01:56.377540 syct-0.4.3/setup.cfg
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      744 2021-10-21 23:00:54.000000 syct-0.4.3/setup.py
-drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2021-10-21 23:01:56.377540 syct-0.4.3/src/
-drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2021-10-21 23:01:56.377540 syct-0.4.3/src/syct/
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)       68 2018-09-05 22:11:52.000000 syct-0.4.3/src/syct/__init__.py
--rw-r--r--   0 nadavo    (1000) nadavo    (1000)     3435 2021-10-21 22:59:38.000000 syct-0.4.3/src/syct/timer_module.py
-drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2021-10-21 23:01:56.377540 syct-0.4.3/src/syct.egg-info/
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1488 2021-10-21 23:01:56.000000 syct-0.4.3/src/syct.egg-info/PKG-INFO
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      215 2021-10-21 23:01:56.000000 syct-0.4.3/src/syct.egg-info/SOURCES.txt
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)        1 2021-10-21 23:01:56.000000 syct-0.4.3/src/syct.egg-info/dependency_links.txt
--rw-rw-r--   0 nadavo    (1000) nadavo    (1000)        5 2021-10-21 23:01:56.000000 syct-0.4.3/src/syct.egg-info/top_level.txt
+drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2023-08-05 22:04:12.699871 syct-0.4.4/
+-rw-r--r--   0 nadavo    (1000) nadavo    (1000)     1067 2018-07-10 23:49:51.000000 syct-0.4.4/LICENSE
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1452 2023-08-05 22:04:12.699871 syct-0.4.4/PKG-INFO
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1017 2021-10-17 09:43:24.000000 syct-0.4.4/README.md
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      104 2021-05-09 10:23:59.000000 syct-0.4.4/pyproject.toml
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)       38 2023-08-05 22:04:12.699871 syct-0.4.4/setup.cfg
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      744 2023-08-05 21:55:29.000000 syct-0.4.4/setup.py
+drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2023-08-05 22:04:12.699871 syct-0.4.4/src/
+drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2023-08-05 22:04:12.699871 syct-0.4.4/src/syct/
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)       68 2018-09-05 22:11:52.000000 syct-0.4.4/src/syct/__init__.py
+-rw-r--r--   0 nadavo    (1000) nadavo    (1000)     3755 2023-08-05 21:54:11.000000 syct-0.4.4/src/syct/timer_module.py
+drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2023-08-05 22:04:12.699871 syct-0.4.4/src/syct.egg-info/
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)     1452 2023-08-05 22:04:12.000000 syct-0.4.4/src/syct.egg-info/PKG-INFO
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      235 2023-08-05 22:04:12.000000 syct-0.4.4/src/syct.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)        1 2023-08-05 22:04:12.000000 syct-0.4.4/src/syct.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)        5 2023-08-05 22:04:12.000000 syct-0.4.4/src/syct.egg-info/top_level.txt
+drwxrwxr-x   0 nadavo    (1000) nadavo    (1000)        0 2023-08-05 22:04:12.699871 syct-0.4.4/tests/
+-rw-rw-r--   0 nadavo    (1000) nadavo    (1000)      739 2023-08-05 21:54:42.000000 syct-0.4.4/tests/test_timer.py
```

### Comparing `syct-0.4.3/LICENSE` & `syct-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syct-0.4.3/PKG-INFO` & `syct-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: syct
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Simple Yet Convenient Timer module for Python 3
 Home-page: https://github.com/nadavo/Timer.git
 Author: Nadav Oved
 Author-email: nadavo@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,8 +61,7 @@
 timer_test.stop()
 ```
 Will produce the following output:
 ```
 <timestamp> - Started Timer Testing
 <timestamp> - Timer Testing took 5.00 seconds to complete
 ```
-
```

### Comparing `syct-0.4.3/README.md` & `syct-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `syct-0.4.3/setup.py` & `syct-0.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='syct',
-     version='0.4.3',
+     version='0.4.4',
      author="Nadav Oved",
      author_email="nadavo@gmail.com",
      description="A Simple Yet Convenient Timer module for Python 3",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/nadavo/Timer.git",
      package_dir={"": "src"},
```

### Comparing `syct-0.4.3/src/syct/timer_module.py` & `syct-0.4.4/src/syct/timer_module.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,95 +1,120 @@
 from math import floor
 from typing import Optional
 from time import localtime, strftime
-from timeit import default_timer as time
+from timeit import default_timer
 import logging
 import functools
 
 
 class Timer:
     """
-    Simple Timer class which prints elapsed time since its creation
+    Simple (Yet Convenient) Timer class which logs elapsed runtime for any arbitrary piece of code
     """
 
     DEFAULT_TIME_FORMAT = "%H:%M:%S"
 
-    def __init__(self, name: str, logger: Optional[logging.Logger] = None, level: int = logging.INFO):
+    def __init__(
+        self,
+        name: str,
+        log_level: int = logging.INFO,
+        logger: Optional[logging.Logger] = None,
+    ):
         self.name = name
-        self.level = level
-        self.logger = self.init_logger(logger, level)
+        self.log_level = log_level
+        self.logger = self.init_logger(logger, log_level, name)
         self._start_time = self._start()
         self._end_time = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, var_type, value, traceback):
         self.stop()
 
     def _start(self) -> float:
-        self.logger.log(msg=f"Started {self.name}", level=self.level)
-        return time()
+        self.logger.log(msg=f"Started Timer for {self.name}", level=self.log_level)
+        return default_timer()
 
-    def _log_elapsed(self) -> None:
+    def _format_elapsed_msg(self) -> str:
         """
-        Internal function which logs a correctly formatted string according to elapsed time units
+        Internal function which correctly formats a log message according to elapsed time units
         """
         elapsed = self._end_time - self._start_time
         unit = "seconds"
-        if elapsed >= 3600.:
+        if elapsed >= 3600.0:
             unit = "minutes"
-            hours = elapsed / 3600.
-            minutes = hours % 60.
+            hours = elapsed / 3600.0
+            minutes = hours % 60.0
             hours = floor(hours)
-            self.logger.log(msg=f"{self.name} took {hours} hours and {minutes:.2f} {unit} to complete", level=self.level)
-        elif elapsed >= 60.:
-            minutes = floor(elapsed / 60.)
-            seconds = elapsed % 60.
-            self.logger.log(msg=f"{self.name} took {minutes} minutes and {seconds:.2f} {unit} to complete", level=self.level)
+            log_message = (
+                f"{self.name} took {hours} hours and {minutes:.2f} {unit} to complete"
+            )
+        elif elapsed >= 60.0:
+            minutes = floor(elapsed / 60.0)
+            seconds = elapsed % 60.0
+            log_message = f"{self.name} took {minutes} minutes and {seconds:.2f} {unit} to complete"
         elif elapsed < 0.1:
             unit = "ms"
-            self.logger.log(msg=f"{self.name} took {elapsed * 1000.:.2f} {unit} to complete", level=self.level)
+            log_message = f"{self.name} took {elapsed * 1000.:.2f} {unit} to complete"
         else:
-            self.logger.log(msg=f"{self.name} took {elapsed:.2f} {unit} to complete", level=self.level)
+            log_message = f"{self.name} took {elapsed:.2f} {unit} to complete"
+        return log_message
 
     def stop(self) -> None:
-        self._end_time = time()
-        self._log_elapsed()
+        self._end_time = default_timer()
+        self.logger.log(msg=self._format_elapsed_msg(), level=self.log_level)
 
     @staticmethod
-    def init_logger(logger: Optional[logging.Logger] = None, level: int = logging.INFO) -> logging.Logger:
+    def init_logger(
+        logger: Optional[logging.Logger] = None,
+        level: int = logging.INFO,
+        name: str = __name__,
+    ) -> logging.Logger:
         if logger is None:
-            logger = logging.getLogger(__name__)
+            logger = logging.getLogger(name)
             logger.setLevel(level)
             if not logger.hasHandlers():
-                formatter = logging.Formatter("{levelname} - {asctime} - {message}", datefmt=Timer.DEFAULT_TIME_FORMAT, style="{")
+                formatter = logging.Formatter(
+                    "{levelname} - {asctime} - {message}",
+                    datefmt=Timer.DEFAULT_TIME_FORMAT,
+                    style="{",
+                )
                 handler = logging.StreamHandler()
                 handler.setFormatter(formatter)
                 logger.addHandler(handler)
         return logger
 
     @staticmethod
     def get_default_timestamp() -> str:
-        return f"{strftime(Timer.DEFAULT_TIME_FORMAT, localtime(time()))} -"
+        return f"{strftime(Timer.DEFAULT_TIME_FORMAT, localtime(default_timer()))} -"
 
 
-def timer(_args=None, *, name: Optional[str] = None, logger: Optional[logging.Logger] = None, level: int = logging.INFO):
+def timer(
+    _args=None,
+    *,
+    name: Optional[str] = None,
+    logger: Optional[logging.Logger] = None,
+    log_level: Optional[int] = logging.INFO,
+):
     """
     Timer decorator which utilizes a Timer object for timing a given function's runtime
     """
+
     def timer_decorator(func):
         @functools.wraps(func)
         def wrapper_timer(*args, **kwargs):
             if name is None:
                 timer_name = func.__name__
             else:
                 timer_name = name
-            timer_wrapper = Timer(name=timer_name, logger=logger, level=level)
+            timer_wrapper = Timer(name=timer_name, logger=logger, log_level=log_level)
             func_ret_val = func(*args, **kwargs)
             timer_wrapper.stop()
             return func_ret_val
+
         return wrapper_timer
+
     if _args is None:
         return timer_decorator
     else:
         return timer_decorator(_args)
```

### Comparing `syct-0.4.3/src/syct.egg-info/PKG-INFO` & `syct-0.4.4/src/syct.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: syct
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Simple Yet Convenient Timer module for Python 3
 Home-page: https://github.com/nadavo/Timer.git
 Author: Nadav Oved
 Author-email: nadavo@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,8 +61,7 @@
 timer_test.stop()
 ```
 Will produce the following output:
 ```
 <timestamp> - Started Timer Testing
 <timestamp> - Timer Testing took 5.00 seconds to complete
 ```
-
```

