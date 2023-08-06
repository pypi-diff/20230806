# Comparing `tmp/bec_ipython_client-0.9.1.tar.gz` & `tmp/bec_ipython_client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_ipython_client-0.9.1.tar", last modified: Mon Jul  3 16:23:43 2023, max compression
+gzip compressed data, was "bec_ipython_client-0.9.2.tar", last modified: Tue Jul  4 13:47:55 2023, max compression
```

## Comparing `bec_ipython_client-0.9.1.tar` & `bec_ipython_client-0.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.857579 bec_ipython_client-0.9.1/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-03 16:23:43.857579 bec_ipython_client-0.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.853579 bec_ipython_client-0.9.1/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/beamline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/bec_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.1/bec_client/bec_magics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.856579 bec_ipython_client-0.9.1/bec_client/bin/
--rwxr-xr-x   0 root         (0) root         (0)      184 2023-07-02 18:14:52.000000 bec_ipython_client-0.9.1/bec_client/bin/bec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.854579 bec_ipython_client-0.9.1/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7462 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/callbacks/ipython_live_updates.py
--rw-r--r--   0 root         (0) root         (0)     9275 2023-06-28 15:23:35.000000 bec_ipython_client-0.9.1/bec_client/callbacks/live_table.py
--rw-r--r--   0 root         (0) root         (0)     4549 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/callbacks/move_device.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.854579 bec_ipython_client-0.9.1/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.855579 bec_ipython_client-0.9.1/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5519 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.1/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/plugins/LamNI/load_additional_correction.py
--rw-r--r--   0 root         (0) root         (0)    54643 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.855579 bec_ipython_client-0.9.1/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.855579 bec_ipython_client-0.9.1/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.856579 bec_ipython_client-0.9.1/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.1/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)     8455 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.1/bec_client/progressbar.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.1/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 16:23:43.857579 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-03 16:23:43.000000 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-03 16:23:43.000000 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 16:23:43.000000 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-03 16:23:43.000000 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-03 16:23:43.000000 bec_ipython_client-0.9.1/bec_ipython_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-03 16:23:43.858579 bec_ipython_client-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-28 14:27:03.000000 bec_ipython_client-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.793366 bec_ipython_client-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-04 13:47:55.793366 bec_ipython_client-0.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.786367 bec_ipython_client-0.9.2/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/beamline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.2/bec_client/bec_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.2/bec_client/bec_magics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.792366 bec_ipython_client-0.9.2/bec_client/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      184 2023-07-02 18:14:52.000000 bec_ipython_client-0.9.2/bec_client/bin/bec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.787366 bec_ipython_client-0.9.2/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-04 13:47:41.000000 bec_ipython_client-0.9.2/bec_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0 root         (0) root         (0)     9275 2023-06-28 15:23:35.000000 bec_ipython_client-0.9.2/bec_client/callbacks/live_table.py
+-rw-r--r--   0 root         (0) root         (0)     4549 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.2/bec_client/callbacks/move_device.py
+-rw-r--r--   0 root         (0) root         (0)     3728 2023-07-04 13:47:41.000000 bec_ipython_client-0.9.2/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.789366 bec_ipython_client-0.9.2/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.790366 bec_ipython_client-0.9.2/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5519 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.2/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-r--r--   0 root         (0) root         (0)    54643 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.2/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.791366 bec_ipython_client-0.9.2/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.791366 bec_ipython_client-0.9.2/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.791366 bec_ipython_client-0.9.2/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.2/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)     8455 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.2/bec_client/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.2/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 13:47:55.793366 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-04 13:47:55.000000 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-04 13:47:55.000000 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 13:47:55.000000 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-04 13:47:55.000000 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-04 13:47:55.000000 bec_ipython_client-0.9.2/bec_ipython_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-04 13:47:55.793366 bec_ipython_client-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-28 14:27:03.000000 bec_ipython_client-0.9.2/setup.py
```

### Comparing `bec_ipython_client-0.9.1/bec_client/beamline_mixin.py` & `bec_ipython_client-0.9.2/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/bec_client.py` & `bec_ipython_client-0.9.2/bec_client/bec_client.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/bec_magics.py` & `bec_ipython_client-0.9.2/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-0.9.2/bec_client/callbacks/ipython_live_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,27 @@
         except ScanInterruption as scan_interr:
             self._interrupted_request = (request, scan_report_type)
             raise scan_interr
 
     def _process_queue(
         self, queue: QueueItem, request: BECMessage.ScanQueueMessage, req_id: str
     ) -> bool:
+        """
+        Process the queue and return True if the scan is completed.
+
+        Args:
+            queue(QueueItem): The queue item to process.
+            request(BECMessage.ScanQueueMessage): The request message.
+            req_id(str): The request ID.
+
+        Returns:
+            bool: True if the scan is completed.
+        """
         check_alarms(self.client)
-        if not queue.request_blocks:
+        if not queue.request_blocks or not queue.status:
             return False
         if queue.status == "PENDING" and queue.queue_position > 0:
             status = self.client.queue.queue_storage.current_scan_queue.get("primary", {}).get(
                 "status"
             )
             print(
                 f"Scan is enqueued and is waiting for execution. Current position in queue: {queue.queue_position + 1}. Queue status: {status}.",
```

### Comparing `bec_ipython_client-0.9.1/bec_client/callbacks/live_table.py` & `bec_ipython_client-0.9.2/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/callbacks/move_device.py` & `bec_ipython_client-0.9.2/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/callbacks/utils.py` & `bec_ipython_client-0.9.2/bec_client/callbacks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,14 @@
 
         await self._wait_for_scan_request_decision()
         check_alarms(self.bec)
 
         while self.scan_queue_request.accepted is None:
             await asyncio.sleep(0.01)
 
-        while self.request_storage.storage[0].queue is None:
-            await asyncio.sleep(0.01)
-
         if not self.scan_queue_request.accepted[0]:
             raise ScanRequestError(
                 f"Scan was rejected by the server: {self.scan_queue_request.response.content.get('message')}"
             )
+
+        while self.scan_queue_request.queue is None:
+            await asyncio.sleep(0.01)
```

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_ipython_client-0.9.2/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_ipython_client-0.9.2/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_ipython_client-0.9.2/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/SLS/sls_info.py` & `bec_ipython_client-0.9.2/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-0.9.2/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/plugins/cSAXS/beamline_info.py` & `bec_ipython_client-0.9.2/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/prettytable.py` & `bec_ipython_client-0.9.2/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/progressbar.py` & `bec_ipython_client-0.9.2/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_client/signals.py` & `bec_ipython_client-0.9.2/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/bec_ipython_client.egg-info/SOURCES.txt` & `bec_ipython_client-0.9.2/bec_ipython_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/setup.cfg` & `bec_ipython_client-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.9.1/setup.py` & `bec_ipython_client-0.9.2/setup.py`

 * *Files identical despite different names*

