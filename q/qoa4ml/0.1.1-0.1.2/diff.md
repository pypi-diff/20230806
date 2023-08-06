# Comparing `tmp/qoa4ml-0.1.1.tar.gz` & `tmp/qoa4ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.1.1.tar", last modified: Sun Aug  6 11:20:43 2023, max compression
+gzip compressed data, was "qoa4ml-0.1.2.tar", last modified: Sun Aug  6 11:52:41 2023, max compression
```

## Comparing `qoa4ml-0.1.1.tar` & `qoa4ml-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.473916 qoa4ml-0.1.1/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.1/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.1/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.1/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:20:43.473347 qoa4ml-0.1.1/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.1/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2023-08-06 11:19:37.000000 qoa4ml-0.1.1/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.1/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.465536 qoa4ml-0.1.1/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    14927 2023-08-06 11:14:28.000000 qoa4ml-0.1.1/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.1/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.468325 qoa4ml-0.1.1/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.1/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.1/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.470918 qoa4ml-0.1.1/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.1/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.1/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.1/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.1/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.1/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.1/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.472628 qoa4ml-0.1.1/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.1/qoa4ml/probes/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6842 2023-07-31 19:42:51.000000 qoa4ml-0.1.1/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4977 2023-07-31 19:51:07.000000 qoa4ml-0.1.1/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.1/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.1/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.467447 qoa4ml-0.1.1/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.1/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-08-06 11:20:43.474107 qoa4ml-0.1.1/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.1/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.374900 qoa4ml-0.1.2/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.2/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.2/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.2/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:52:41.374440 qoa4ml-0.1.2/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.2/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-08-06 11:48:12.000000 qoa4ml-0.1.2/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.2/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.366471 qoa4ml-0.1.2/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    15049 2023-08-06 11:52:27.000000 qoa4ml-0.1.2/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.2/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.369905 qoa4ml-0.1.2/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.2/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.2/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.372422 qoa4ml-0.1.2/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.2/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.2/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.2/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.2/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.2/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.2/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.373812 qoa4ml-0.1.2/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.2/qoa4ml/probes/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6935 2023-08-06 11:47:58.000000 qoa4ml-0.1.2/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     5064 2023-08-06 11:44:47.000000 qoa4ml-0.1.2/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.2/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.2/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:52:41.369126 qoa4ml-0.1.2/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-08-06 11:52:41.000000 qoa4ml-0.1.2/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.2/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-08-06 11:52:41.375042 qoa4ml-0.1.2/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.2/setup.py
```

### Comparing `qoa4ml-0.1.1/CHANGELOG.txt` & `qoa4ml-0.1.2/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/LICENCE.txt` & `qoa4ml-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/PKG-INFO` & `qoa4ml-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.1/README.md` & `qoa4ml-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/QoaClient.py` & `qoa4ml-0.1.2/qoa4ml/QoaClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,18 @@
             for connector in connectors:
                 print(connector)
         self.lock.release()
 
     def report(self, metrics:list=None, report: dict = None, connectors:list=None, submit=False,reset=True):
         if (report == None):
             report = self.qoaReport.generateReport(metrics, reset=reset)
+        else:
+            report["metadata"] = self.clientConf
+            report["metadata"]["timestamp"] = time.time()
+
         if submit:
             if self.default_connector != None:
                 sub_thread = Thread(target=self.asyn_report, args=(report, connectors))
                 sub_thread.start()
             else:
                 logging.warning("No connector available")
         return report
```

### Comparing `qoa4ml-0.1.1/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.1.2/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.1.2/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.1.2/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.1.2/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.1.2/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/metric.py` & `qoa4ml-0.1.2/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/probes/dataquality.py` & `qoa4ml-0.1.2/qoa4ml/probes/dataquality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This library is built based on ydata_quality: https://github.com/ydataai/ydata-quality
 import pandas as pd 
 import numpy as np
-import traceback, sys, logging
+import traceback, sys, logging, pathlib
 from ydata_quality.erroneous_data import ErroneousDataIdentifier
 from ydata_quality.missings import MissingsProfiler
 from ydata_quality.labelling import LabelInspector
 from ydata_quality.duplicates import DuplicateChecker
 from PIL import Image
 import PIL, io
+p_dir = pathlib.Path(__file__).parent.parent.absolute()
+sys.path.append(str(p_dir))
 import utils
 
 # Define metric names, return formats: dictionary {metric name} {sub-element}
 # Return error/debugging
 ################################################ DATA QUALITY ########################################################
```

### Comparing `qoa4ml-0.1.1/qoa4ml/probes/mlquality.py` & `qoa4ml-0.1.2/qoa4ml/probes/mlquality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This library is built based on ydata_quality: https://github.com/ydataai/ydata-quality
 import pandas as pd 
 import numpy as np
 import tensorflow as tf
-import traceback, sys
-from dataquality import is_numpyarray
+import traceback, sys, pathlib
+p_dir = pathlib.Path(__file__).parent.parent.absolute()
+sys.path.append(str(p_dir))
+from utils import is_numpyarray
 
 ################################################ ML QUALITY ########################################################
 
 def timeseries_metric(model):
     metrics = {}
     try:
         if isinstance(model, tf.keras.Sequential):
```

### Comparing `qoa4ml-0.1.1/qoa4ml/reports.py` & `qoa4ml-0.1.2/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml/utils.py` & `qoa4ml-0.1.2/qoa4ml/utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.1.2/qoa4ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.1/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.1.2/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.1/setup.py` & `qoa4ml-0.1.2/setup.py`

 * *Files identical despite different names*

