# Comparing `tmp/zcc-helper-3.2.dev1.tar.gz` & `tmp/zcc-helper-3.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcc-helper-3.2.dev1.tar", last modified: Fri Aug  4 05:27:22 2023, max compression
+gzip compressed data, was "zcc-helper-3.2.dev2.tar", last modified: Sun Aug  6 07:02:55 2023, max compression
```

## Comparing `zcc-helper-3.2.dev1.tar` & `zcc-helper-3.2.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-04 05:27:22.353145 zcc-helper-3.2.dev1/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-04 05:27:22.352495 zcc-helper-3.2.dev1/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev1/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-04 05:27:22.353193 zcc-helper-3.2.dev1/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev1/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-04 05:27:22.350501 zcc-helper-3.2.dev1/zcc/
--rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev1/zcc/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev1/zcc/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-04 05:23:38.000000 zcc-helper-3.2.dev1/zcc/constants.py
--rw-r--r--   0 mark       (501) staff       (20)    17909 2023-08-04 05:25:28.000000 zcc-helper-3.2.dev1/zcc/controller.py
--rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev1/zcc/description.py
--rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev1/zcc/device.py
--rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev1/zcc/discovery.py
--rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev1/zcc/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-04 05:23:59.000000 zcc-helper-3.2.dev1/zcc/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     6372 2022-06-18 00:10:40.000000 zcc-helper-3.2.dev1/zcc/socket.py
--rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev1/zcc/trace.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev1/zcc/watchdog.py
--rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev1/zcc.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-04 05:27:22.351867 zcc-helper-3.2.dev1/zcc_helper.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-04 05:27:22.000000 zcc-helper-3.2.dev1/zcc_helper.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-04 05:27:22.000000 zcc-helper-3.2.dev1/zcc_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-04 05:27:22.000000 zcc-helper-3.2.dev1/zcc_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-04 05:27:22.000000 zcc-helper-3.2.dev1/zcc_helper.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.298365 zcc-helper-3.2.dev2/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-06 07:02:55.298135 zcc-helper-3.2.dev2/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.2.dev2/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-06 07:02:55.298420 zcc-helper-3.2.dev2/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.2.dev2/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.296324 zcc-helper-3.2.dev2/zcc/
+-rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.2.dev2/zcc/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.2.dev2/zcc/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)      248 2023-08-06 07:02:49.000000 zcc-helper-3.2.dev2/zcc/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)    17921 2023-08-06 07:02:41.000000 zcc-helper-3.2.dev2/zcc/controller.py
+-rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/description.py
+-rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/device.py
+-rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-26 06:43:27.000000 zcc-helper-3.2.dev2/zcc/discovery.py
+-rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.2.dev2/zcc/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     3767 2023-08-06 06:56:34.000000 zcc-helper-3.2.dev2/zcc/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     6384 2023-08-06 07:00:14.000000 zcc-helper-3.2.dev2/zcc/socket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev2/zcc/trace.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.2.dev2/zcc/watchdog.py
+-rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.2.dev2/zcc.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-06 07:02:55.297737 zcc-helper-3.2.dev2/zcc_helper.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    10155 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      351 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        4 2023-08-06 07:02:55.000000 zcc-helper-3.2.dev2/zcc_helper.egg-info/top_level.txt
```

### Comparing `zcc-helper-3.2.dev1/PKG-INFO` & `zcc-helper-3.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev1
+Version: 3.2.dev2
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `zcc-helper-3.2.dev1/README.md` & `zcc-helper-3.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/setup.py` & `zcc-helper-3.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/__main__.py` & `zcc-helper-3.2.dev2/zcc/__main__.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/controller.py` & `zcc-helper-3.2.dev2/zcc/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class ControlPoint:
     '''Represents the ZCC controller which connects to individual devices'''
 
     def __init__(self, description: ControlPointDescription = None,
                  timeout: int = 2, verbosity: int = 0):
 
-        self.logger = logging.getLogger('ControlPoint')
+        self.logger = logging.getLogger(f'ControlPoint@{id(self)}')
         if verbosity > 2:
             verbosity = 2
         self.logger.setLevel(LEVEL_BY_VERBOSITY[verbosity])
 
         self.host = description.host
         self.port = description.port
```

### Comparing `zcc-helper-3.2.dev1/zcc/device.py` & `zcc-helper-3.2.dev2/zcc/device.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/discovery.py` & `zcc-helper-3.2.dev2/zcc/discovery.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/protocol.py` & `zcc-helper-3.2.dev2/zcc/protocol.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/socket.py` & `zcc-helper-3.2.dev2/zcc/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.listen_task: asyncio.Task = None
 
         self.listen_queu = queue.Queue()
         self.send_queu = queue.Queue()
 
         self.loop = asyncio.get_event_loop()
 
-        self.logger = logging.getLogger('ControlPointSocket')
+        self.logger = logging.getLogger(f'ControlPointSocket@{id(self)}')
         self.logger.setLevel(LEVEL_BY_VERBOSITY[verbosity])
 
         self.sock: socket.socket = None
         self.reader: StreamReader = None
         self.writer: StreamWriter = None
 
         self.timeout = timeout
```

### Comparing `zcc-helper-3.2.dev1/zcc/trace.py` & `zcc-helper-3.2.dev2/zcc/trace.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc/watchdog.py` & `zcc-helper-3.2.dev2/zcc/watchdog.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.2.dev1/zcc_helper.egg-info/PKG-INFO` & `zcc-helper-3.2.dev2/zcc_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.2.dev1
+Version: 3.2.dev2
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

