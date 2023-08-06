# Comparing `tmp/qoa4ml-0.1.2.tar.gz` & `tmp/qoa4ml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.1.2.tar", last modified: Sun Aug  6 11:52:41 2023, max compression
+gzip compressed data, was "qoa4ml-0.1.3.tar", last modified: Sun Aug  6 15:54:45 2023, max compression
```

## Comparing `qoa4ml-0.1.2.tar` & `qoa4ml-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.374900 qoa4ml-0.1.2/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.2/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.2/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.2/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:52:41.374440 qoa4ml-0.1.2/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.2/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-08-06 11:48:12.000000 qoa4ml-0.1.2/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.2/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.366471 qoa4ml-0.1.2/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    15049 2023-08-06 11:52:27.000000 qoa4ml-0.1.2/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.2/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.369905 qoa4ml-0.1.2/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.2/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.2/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.372422 qoa4ml-0.1.2/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.2/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.2/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.2/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.2/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.2/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.2/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.373812 qoa4ml-0.1.2/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.2/qoa4ml/probes/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6935 2023-08-06 11:47:58.000000 qoa4ml-0.1.2/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     5064 2023-08-06 11:44:47.000000 qoa4ml-0.1.2/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.2/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.2/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.369126 qoa4ml-0.1.2/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.2/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-08-06 11:52:41.375042 qoa4ml-0.1.2/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.2/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.034719 qoa4ml-0.1.3/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.3/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.3/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.3/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 15:54:45.034330 qoa4ml-0.1.3/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.3/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-08-06 15:54:33.000000 qoa4ml-0.1.3/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.3/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.022820 qoa4ml-0.1.3/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    15070 2023-08-06 15:44:20.000000 qoa4ml-0.1.3/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.3/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.026241 qoa4ml-0.1.3/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.3/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.3/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.030827 qoa4ml-0.1.3/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.3/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.3/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.3/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.3/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.3/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.3/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.033269 qoa4ml-0.1.3/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.3/qoa4ml/probes/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6935 2023-08-06 11:47:58.000000 qoa4ml-0.1.3/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     5064 2023-08-06 11:44:47.000000 qoa4ml-0.1.3/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.3/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.3/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 15:54:45.025319 qoa4ml-0.1.3/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 15:54:44.000000 qoa4ml-0.1.3/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-08-06 15:54:44.000000 qoa4ml-0.1.3/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-08-06 15:54:44.000000 qoa4ml-0.1.3/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-08-06 15:54:44.000000 qoa4ml-0.1.3/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-08-06 15:54:44.000000 qoa4ml-0.1.3/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.3/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-08-06 15:54:45.034890 qoa4ml-0.1.3/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.3/setup.py
```

### Comparing `qoa4ml-0.1.2/CHANGELOG.txt` & `qoa4ml-0.1.3/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/LICENCE.txt` & `qoa4ml-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/PKG-INFO` & `qoa4ml-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.2/README.md` & `qoa4ml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/QoaClient.py` & `qoa4ml-0.1.3/qoa4ml/QoaClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .metric import Gauge, Counter, Summary, Histogram
 import json, uuid
 import threading
 from threading import Thread
 import time, uuid, requests
 from datetime import datetime
 import logging
-import os, sys, traceback
+import os, sys, traceback, copy
 from .utils import get_proc_cpu, get_proc_mem, load_config
 from .reports import QoaReport
 from .probes.dataquality import eva_duplicate, eva_erronous, eva_missing, eva_none, image_quality
 from .probes.mlquality import *
 
 headers = {
     'Content-Type': 'application/json'
@@ -261,15 +261,15 @@
                 print(connector)
         self.lock.release()
 
     def report(self, metrics:list=None, report: dict = None, connectors:list=None, submit=False,reset=True):
         if (report == None):
             report = self.qoaReport.generateReport(metrics, reset=reset)
         else:
-            report["metadata"] = self.clientConf
+            report["metadata"] = copy.deepcopy(self.clientConf)
             report["metadata"]["timestamp"] = time.time()
 
         if submit:
             if self.default_connector != None:
                 sub_thread = Thread(target=self.asyn_report, args=(report, connectors))
                 sub_thread.start()
             else:
```

### Comparing `qoa4ml-0.1.2/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.1.3/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.1.3/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.1.3/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.1.3/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.1.3/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/metric.py` & `qoa4ml-0.1.3/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/probes/dataquality.py` & `qoa4ml-0.1.3/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/probes/mlquality.py` & `qoa4ml-0.1.3/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/reports.py` & `qoa4ml-0.1.3/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml/utils.py` & `qoa4ml-0.1.3/qoa4ml/utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.1.3/qoa4ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.2/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.1.3/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.2/setup.py` & `qoa4ml-0.1.3/setup.py`

 * *Files identical despite different names*

