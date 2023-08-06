# Comparing `tmp/bec_lib-0.9.1.tar.gz` & `tmp/bec_lib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-0.9.1.tar", last modified: Mon Jul  3 16:23:57 2023, max compression
+gzip compressed data, was "bec_lib-0.9.2.tar", last modified: Tue Jul  4 13:48:09 2023, max compression
```

## Comparing `bec_lib-0.9.1.tar` & `bec_lib-0.9.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:57.657145 bec_lib-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     3049 2023-07-03 16:23:57.657145 bec_lib-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2616 2023-06-28 10:41:58.000000 bec_lib-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:57.651145 bec_lib-0.9.1/bec_lib/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/alarm_handler.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/callback_handler.py
--rw-r--r--   0 root         (0) root         (0)     7316 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:57.656145 bec_lib-0.9.1/bec_lib/core/
--rw-r--r--   0 root         (0) root         (0)    26694 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/BECMessage.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/bec_errors.py
--rw-r--r--   0 root         (0) root         (0)     8789 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/bec_service.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/channel_monitor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/config_helper.py
--rw-r--r--   0 root         (0) root         (0)     5100 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/connector.py
--rw-r--r--   0 root         (0) root         (0)    27512 2023-07-03 16:23:30.000000 bec_lib-0.9.1/bec_lib/core/devicemanager.py
--rw-r--r--   0 root         (0) root         (0)    21582 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/endpoints.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/init_config.py
--rw-r--r--   0 root         (0) root         (0)     2329 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/logbook_connector.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/logger.py
--rw-r--r--   0 root         (0) root         (0)     2981 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/numpy_encoder.py
--rw-r--r--   0 root         (0) root         (0)     4820 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/observer.py
--rw-r--r--   0 root         (0) root         (0)     2696 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/pdf_writer.py
--rw-r--r--   0 root         (0) root         (0)    11309 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/redis_connector.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/service_config.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/session_manager.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/timeout.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/core/utils.py
--rw-r--r--   0 root         (0) root         (0)    12126 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/devicemanager_client.py
--rw-r--r--   0 root         (0) root         (0)     7632 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/queue_items.py
--rw-r--r--   0 root         (0) root         (0)     5420 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/request_items.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/scan_items.py
--rw-r--r--   0 root         (0) root         (0)    11556 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/scan_manager.py
--rw-r--r--   0 root         (0) root         (0)    10918 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/scans.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-06-28 10:41:58.000000 bec_lib-0.9.1/bec_lib/user_scripts_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:57.657145 bec_lib-0.9.1/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3049 2023-07-03 16:23:57.000000 bec_lib-0.9.1/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-03 16:23:57.000000 bec_lib-0.9.1/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:23:57.000000 bec_lib-0.9.1/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-03 16:23:57.000000 bec_lib-0.9.1/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 16:23:57.000000 bec_lib-0.9.1/bec_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-03 16:23:57.658145 bec_lib-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 14:27:03.000000 bec_lib-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.162955 bec_lib-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-04 13:48:09.162955 bec_lib-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-06-28 10:41:58.000000 bec_lib-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.158955 bec_lib-0.9.2/bec_lib/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/alarm_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/callback_handler.py
+-rw-r--r--   0 root         (0) root         (0)     7316 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.161955 bec_lib-0.9.2/bec_lib/core/
+-rw-r--r--   0 root         (0) root         (0)    26694 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/BECMessage.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/bec_errors.py
+-rw-r--r--   0 root         (0) root         (0)     8789 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/bec_service.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/channel_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/config_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5100 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/connector.py
+-rw-r--r--   0 root         (0) root         (0)    27668 2023-07-04 13:47:41.000000 bec_lib-0.9.2/bec_lib/core/devicemanager.py
+-rw-r--r--   0 root         (0) root         (0)    21582 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/endpoints.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/init_config.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/logbook_connector.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/numpy_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     4820 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/observer.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/pdf_writer.py
+-rw-r--r--   0 root         (0) root         (0)    11309 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/redis_connector.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/service_config.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/session_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/timeout.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12126 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/devicemanager_client.py
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/queue_items.py
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/request_items.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/scan_items.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/scan_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10918 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/scans.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-06-28 10:41:58.000000 bec_lib-0.9.2/bec_lib/user_scripts_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.162955 bec_lib-0.9.2/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-04 13:48:09.000000 bec_lib-0.9.2/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-04 13:48:09.000000 bec_lib-0.9.2/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:48:09.000000 bec_lib-0.9.2/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-04 13:48:09.000000 bec_lib-0.9.2/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-04 13:48:09.000000 bec_lib-0.9.2/bec_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-04 13:48:09.163955 bec_lib-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 14:27:03.000000 bec_lib-0.9.2/setup.py
```

### Comparing `bec_lib-0.9.1/PKG-INFO` & `bec_lib-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_lib-0.9.1/README.md` & `bec_lib-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/alarm_handler.py` & `bec_lib-0.9.2/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/callback_handler.py` & `bec_lib-0.9.2/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/client.py` & `bec_lib-0.9.2/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/BECMessage.py` & `bec_lib-0.9.2/bec_lib/core/BECMessage.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/__init__.py` & `bec_lib-0.9.2/bec_lib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/bec_service.py` & `bec_lib-0.9.2/bec_lib/core/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/channel_monitor.py` & `bec_lib-0.9.2/bec_lib/core/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/config_helper.py` & `bec_lib-0.9.2/bec_lib/core/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/connector.py` & `bec_lib-0.9.2/bec_lib/core/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/devicemanager.py` & `bec_lib-0.9.2/bec_lib/core/devicemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,18 @@
                     self[k] = v
 
         if kwargs:
             for k, v in kwargs.items():
                 self[k] = v
 
     def __getattr__(self, attr):
-        if attr == "__wrapped__":
+        if attr.startswith("__"):
+            # if dunder attributes are would not be caught, they
+            # would raise a DeviceConfigError and kill the
+            # IPython completer
             return self.get(attr)
         dev = self.get(attr)
         if not dev:
             raise DeviceConfigError(f"Device {attr} does not exist.")
         return dev
 
     def __setattr__(self, key, value):
```

### Comparing `bec_lib-0.9.1/bec_lib/core/endpoints.py` & `bec_lib-0.9.2/bec_lib/core/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/init_config.py` & `bec_lib-0.9.2/bec_lib/core/init_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/logbook_connector.py` & `bec_lib-0.9.2/bec_lib/core/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/logger.py` & `bec_lib-0.9.2/bec_lib/core/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/numpy_encoder.py` & `bec_lib-0.9.2/bec_lib/core/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/observer.py` & `bec_lib-0.9.2/bec_lib/core/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/pdf_writer.py` & `bec_lib-0.9.2/bec_lib/core/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/redis_connector.py` & `bec_lib-0.9.2/bec_lib/core/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/service_config.py` & `bec_lib-0.9.2/bec_lib/core/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/core/timeout.py` & `bec_lib-0.9.2/bec_lib/core/timeout.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/devicemanager_client.py` & `bec_lib-0.9.2/bec_lib/devicemanager_client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/queue_items.py` & `bec_lib-0.9.2/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/request_items.py` & `bec_lib-0.9.2/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/scan_items.py` & `bec_lib-0.9.2/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/scan_manager.py` & `bec_lib-0.9.2/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/scans.py` & `bec_lib-0.9.2/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib/user_scripts_mixin.py` & `bec_lib-0.9.2/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/bec_lib.egg-info/PKG-INFO` & `bec_lib-0.9.2/bec_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 0.9.1
+Version: 0.9.2
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_lib-0.9.1/bec_lib.egg-info/SOURCES.txt` & `bec_lib-0.9.2/bec_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_lib-0.9.1/setup.py` & `bec_lib-0.9.2/setup.py`

 * *Files identical despite different names*

