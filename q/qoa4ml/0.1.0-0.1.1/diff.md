# Comparing `tmp/qoa4ml-0.1.0.tar.gz` & `tmp/qoa4ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.1.0.tar", last modified: Mon Jul 31 20:13:09 2023, max compression
+gzip compressed data, was "qoa4ml-0.1.1.tar", last modified: Sun Aug  6 11:20:43 2023, max compression
```

## Comparing `qoa4ml-0.1.0.tar` & `qoa4ml-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.726326 qoa4ml-0.1.0/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.0/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.0/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.0/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-07-31 20:13:09.726061 qoa4ml-0.1.0/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.0/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-07-31 20:12:59.000000 qoa4ml-0.1.0/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.0/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.719854 qoa4ml-0.1.0/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    14812 2023-07-31 19:42:41.000000 qoa4ml-0.1.0/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.0/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.721851 qoa4ml-0.1.0/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.0/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.0/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.724839 qoa4ml-0.1.0/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.0/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.0/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.0/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.0/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.0/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.0/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.725680 qoa4ml-0.1.0/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6842 2023-07-31 19:42:51.000000 qoa4ml-0.1.0/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4977 2023-07-31 19:51:07.000000 qoa4ml-0.1.0/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.0/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.0/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.721328 qoa4ml-0.1.0/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.0/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 20:13:09.726412 qoa4ml-0.1.0/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.0/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.473916 qoa4ml-0.1.1/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.1/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.1/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.1/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:20:43.473347 qoa4ml-0.1.1/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.1/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2023-08-06 11:19:37.000000 qoa4ml-0.1.1/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.1/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.465536 qoa4ml-0.1.1/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    14927 2023-08-06 11:14:28.000000 qoa4ml-0.1.1/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.1/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.468325 qoa4ml-0.1.1/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.1/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.1/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.470918 qoa4ml-0.1.1/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.1/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.1/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.1/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.1/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.1/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.1/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.472628 qoa4ml-0.1.1/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.1/qoa4ml/probes/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6842 2023-07-31 19:42:51.000000 qoa4ml-0.1.1/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4977 2023-07-31 19:51:07.000000 qoa4ml-0.1.1/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.1/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.1/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:20:43.467447 qoa4ml-0.1.1/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-08-06 11:20:43.000000 qoa4ml-0.1.1/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.1/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-08-06 11:20:43.474107 qoa4ml-0.1.1/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.1/setup.py
```

### Comparing `qoa4ml-0.1.0/CHANGELOG.txt` & `qoa4ml-0.1.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/LICENCE.txt` & `qoa4ml-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/PKG-INFO` & `qoa4ml-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.0/README.md` & `qoa4ml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/QoaClient.py` & `qoa4ml-0.1.1/qoa4ml/QoaClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,20 +235,23 @@
                 self.report(report=report,submit=True)
             except Exception as e:
                 print("[ERROR] - Error {} in send process report: {}".format(type(e),e.__traceback__))
                 traceback.print_exception(*sys.exc_info())
             time.sleep(interval)
 
 
-    def process_monitor(self, interval:int, pid:int = None):
+    def process_monitor_start(self, interval:int, pid:int = None):
         if (pid == None):
             pid = os.getpid()
+        self.procMonitorFlag = True
         sub_thread = Thread(target=self.process_report, args=(interval, pid))
         sub_thread.start()
 
+    def process_monitor_stop(self):
+        self.procMonitorFlag = False
     
     def asyn_report(self, report:dict, connectors:list=None):
         body_mess = json.dumps(report)
         self.lock.acquire()
         if connectors == None:
             # if connectors are not specify, use default
             self.connectorList[self.default_connector].send_data(body_mess,str(uuid.uuid4()))
```

### Comparing `qoa4ml-0.1.0/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.1.1/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.1.1/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.1.1/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.1.1/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.1.1/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/metric.py` & `qoa4ml-0.1.1/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/probes/dataquality.py` & `qoa4ml-0.1.1/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/probes/mlquality.py` & `qoa4ml-0.1.1/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/reports.py` & `qoa4ml-0.1.1/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml/utils.py` & `qoa4ml-0.1.1/qoa4ml/utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.0/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.1.1/qoa4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.1.0/setup.py` & `qoa4ml-0.1.1/setup.py`

 * *Files identical despite different names*

