# Comparing `tmp/bec_scan_server-0.9.1.tar.gz` & `tmp/bec_scan_server-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scan_server-0.9.1.tar", last modified: Mon Jul  3 16:23:58 2023, max compression
+gzip compressed data, was "bec_scan_server-0.9.2.tar", last modified: Tue Jul  4 13:48:09 2023, max compression
```

## Comparing `bec_scan_server-0.9.1.tar` & `bec_scan_server-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:58.274126 bec_scan_server-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     2560 2023-07-03 16:23:58.274126 bec_scan_server-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2115 2023-06-27 20:50:04.000000 bec_scan_server-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:58.274126 bec_scan_server-0.9.1/bec_scan_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2560 2023-07-03 16:23:58.000000 bec_scan_server-0.9.1/bec_scan_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-03 16:23:58.000000 bec_scan_server-0.9.1/bec_scan_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:23:58.000000 bec_scan_server-0.9.1/bec_scan_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-03 16:23:58.000000 bec_scan_server-0.9.1/bec_scan_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-03 16:23:58.000000 bec_scan_server-0.9.1/bec_scan_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:58.273126 bec_scan_server-0.9.1/scan_server/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-24 15:23:42.000000 bec_scan_server-0.9.1/scan_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-24 15:23:42.000000 bec_scan_server-0.9.1/scan_server/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-06-19 08:14:59.000000 bec_scan_server-0.9.1/scan_server/path_optimization.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scan_assembler.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scan_guard.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-07-02 18:58:28.000000 bec_scan_server-0.9.1/scan_server/scan_manager.py
--rw-r--r--   0 root         (0) root         (0)    30785 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scan_queue.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scan_server.py
--rw-r--r--   0 root         (0) root         (0)    13324 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scan_stubs.py
--rw-r--r--   0 root         (0) root         (0)    26660 2023-06-28 15:23:35.000000 bec_scan_server-0.9.1/scan_server/scan_worker.py
--rw-r--r--   0 root         (0) root         (0)    42711 2023-06-28 10:41:58.000000 bec_scan_server-0.9.1/scan_server/scans.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-07-03 16:23:58.275126 bec_scan_server-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 14:27:03.000000 bec_scan_server-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.588942 bec_scan_server-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-07-04 13:48:09.588942 bec_scan_server-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-27 20:50:04.000000 bec_scan_server-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.588942 bec_scan_server-0.9.2/bec_scan_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-07-04 13:48:09.000000 bec_scan_server-0.9.2/bec_scan_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-04 13:48:09.000000 bec_scan_server-0.9.2/bec_scan_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:48:09.000000 bec_scan_server-0.9.2/bec_scan_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-04 13:48:09.000000 bec_scan_server-0.9.2/bec_scan_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-04 13:48:09.000000 bec_scan_server-0.9.2/bec_scan_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:48:09.587942 bec_scan_server-0.9.2/scan_server/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-24 15:23:42.000000 bec_scan_server-0.9.2/scan_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-24 15:23:42.000000 bec_scan_server-0.9.2/scan_server/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-06-19 08:14:59.000000 bec_scan_server-0.9.2/scan_server/path_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-06-28 10:41:58.000000 bec_scan_server-0.9.2/scan_server/scan_assembler.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-04 13:47:41.000000 bec_scan_server-0.9.2/scan_server/scan_guard.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-07-02 18:58:28.000000 bec_scan_server-0.9.2/scan_server/scan_manager.py
+-rw-r--r--   0 root         (0) root         (0)    30785 2023-06-28 10:41:58.000000 bec_scan_server-0.9.2/scan_server/scan_queue.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-06-28 10:41:58.000000 bec_scan_server-0.9.2/scan_server/scan_server.py
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-06-28 10:41:58.000000 bec_scan_server-0.9.2/scan_server/scan_stubs.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2023-06-28 15:23:35.000000 bec_scan_server-0.9.2/scan_server/scan_worker.py
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-06-28 10:41:58.000000 bec_scan_server-0.9.2/scan_server/scans.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-04 13:48:09.589942 bec_scan_server-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 14:27:03.000000 bec_scan_server-0.9.2/setup.py
```

### Comparing `bec_scan_server-0.9.1/PKG-INFO` & `bec_scan_server-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_scan_server
-Version: 0.9.1
+Version: 0.9.2
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-0.9.1/README.md` & `bec_scan_server-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/bec_scan_server.egg-info/PKG-INFO` & `bec_scan_server-0.9.2/bec_scan_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-scan-server
-Version: 0.9.1
+Version: 0.9.2
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-0.9.1/bec_scan_server.egg-info/SOURCES.txt` & `bec_scan_server-0.9.2/bec_scan_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/path_optimization.py` & `bec_scan_server-0.9.2/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_assembler.py` & `bec_scan_server-0.9.2/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_guard.py` & `bec_scan_server-0.9.2/scan_server/scan_guard.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,15 @@
             self._check_valid_scan(request)
             self._check_baton(request)
             self._check_motors_movable(request)
             self._check_soft_limits(request)
         except Exception as error:
             content = traceback.format_exc()
             return ScanStatus(False, str(content))
-        else:
-            return ScanStatus()
+        return ScanStatus()
 
     def _check_valid_request(self, request) -> None:
         if request is None:
             raise ScanRejection("Invalid request.")
 
     def _check_valid_scan(self, request) -> None:
         avail_scans = msgpack.loads(self.producer.get(MessageEndpoints.available_scans()))
```

### Comparing `bec_scan_server-0.9.1/scan_server/scan_manager.py` & `bec_scan_server-0.9.2/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_queue.py` & `bec_scan_server-0.9.2/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_server.py` & `bec_scan_server-0.9.2/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_stubs.py` & `bec_scan_server-0.9.2/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scan_worker.py` & `bec_scan_server-0.9.2/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/scan_server/scans.py` & `bec_scan_server-0.9.2/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/setup.cfg` & `bec_scan_server-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.9.1/setup.py` & `bec_scan_server-0.9.2/setup.py`

 * *Files identical despite different names*

