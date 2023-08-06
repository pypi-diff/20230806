# Comparing `tmp/wizata-dsapi-0.3.6.tar.gz` & `tmp/wizata-dsapi-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.3.6.tar", last modified: Sat Aug  5 12:33:35 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.3.7.tar", last modified: Sun Aug  6 12:16:50 2023, max compression
```

## Comparing `wizata-dsapi-0.3.6.tar` & `wizata-dsapi-0.3.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.340900 wizata-dsapi-0.3.6/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:33:35.340791 wizata-dsapi-0.3.6/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-05 12:33:35.340939 wizata-dsapi-0.3.6/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-05 12:33:31.000000 wizata-dsapi-0.3.6/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.339957 wizata-dsapi-0.3.6/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.6/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5717 2023-08-05 12:33:31.000000 wizata-dsapi-0.3.6/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.6/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.6/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.6/wizata_dsapi/wizata_dsapi_client.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.340638 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-06 12:16:50.020310 wizata-dsapi-0.3.7/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-06 12:16:50.020200 wizata-dsapi-0.3.7/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-06 12:16:50.020352 wizata-dsapi-0.3.7/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-06 12:16:46.000000 wizata-dsapi-0.3.7/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-06 12:16:50.018967 wizata-dsapi-0.3.7/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1058 2023-08-06 12:16:46.000000 wizata-dsapi-0.3.7/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6703 2023-08-06 12:16:46.000000 wizata-dsapi-0.3.7/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.7/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      121 2023-08-06 12:16:46.000000 wizata-dsapi-0.3.7/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.7/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.7/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.7/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.7/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.7/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.7/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-06 12:16:50.020042 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-06 12:16:49.000000 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      778 2023-08-06 12:16:49.000000 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-06 12:16:49.000000 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-06 12:16:49.000000 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-06 12:16:49.000000 wizata-dsapi-0.3.7/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.3.6/LICENSE.txt` & `wizata-dsapi-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/setup.py` & `wizata-dsapi-0.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.3.6',
+    version='0.3.7',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/__init__.py` & `wizata-dsapi-0.3.7/wizata_dsapi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 # Legacy
 from .dsapi_json_encoder import DSAPIEncoder
 from .wizard_function import WizardStep, WizardFunction
 
 # Pipeline Entities (Dto)
 from .pipeline import Pipeline, PipelineStep, StepType, WriteConfig, VarType
 from .context import Context
+from .ilogger import ILogger
```

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.3.7/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/context.py` & `wizata-dsapi-0.3.7/wizata_dsapi/context.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 import uuid
 import pandas
 
 from .mlmodel import MLModel
 from .plot import Plot
+from .ilogger import ILogger
 
 
-class Context:
+class Context(ILogger):
     """
     Context defines all properties, dataframes, models and other data passed through pipeline steps.
-    :ivar key_mapping: mapping between key:step and value:pipeline IDs
+    - properties are accessible on properties property.
+    - output dataframe(s) use return statement.
+    - input dataframe(s) get them by parameters or use dataframe property directly.
+    - for model use the set_model statement : support only one model per script.
+    - for plot use the set_model statement : support only one plot per script.
+    - dataframes, models and additional plots used within the pipelines can also be accessed, read-only.
     """
 
     def __init__(self,
                  pipeline_id: uuid.UUID = None,
                  execution_id: uuid.UUID = None):
         self.pipeline_id = pipeline_id
         self.execution_id = execution_id
 
         self.models = {}
         self.dataframes = {}
         self.properties = {}
         self.plots = {}
 
+        self._logger = None
+
         self.__key_mapping = None
         self.__primary_key = None
         self.__temporary_dataframe = None
 
         self.__new_plot = None
         self.__new_model = None
 
+    def write_log(self, message: str, level: int = 7):
+        """
+        write log in console (only in experiment mode) - if running locally it will print in the console.
+        :param message: message to write.
+        :param level: from 7=DEBUG, 6=INFO, 3=ERROR to 1=CRITICAL
+        """
+        if self._logger is None:
+            print(message)
+        else:
+            self._logger.write_log(message=message, level=level)
+
     @property
     def dataframe(self):
+        """
+        dataframe - use for single input only - for output use return statement
+        """
         if self.__primary_key is not None and self.__key_mapping is not None and self.__primary_key in self.__key_mapping and self.__key_mapping[self.__primary_key] in self.dataframes:
             return self.dataframes[self.__key_mapping[self.__primary_key]]
         elif self.__temporary_dataframe is not None:
             return self.__temporary_dataframe
         else:
             return None
```

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.3.7/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.3.7/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.3.7/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.3.7/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/execution.py` & `wizata-dsapi-0.3.7/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/experiment.py` & `wizata-dsapi-0.3.7/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.3.7/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.3.7/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.3.7/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/plot.py` & `wizata-dsapi-0.3.7/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/request.py` & `wizata-dsapi-0.3.7/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/script.py` & `wizata-dsapi-0.3.7/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/template.py` & `wizata-dsapi-0.3.7/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/twin.py` & `wizata-dsapi-0.3.7/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.3.7/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.3.7/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.3.7/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 wizata_dsapi/context.py
 wizata_dsapi/dataframe_toolkit.py
 wizata_dsapi/datapoint.py
 wizata_dsapi/ds_dataframe.py
 wizata_dsapi/dsapi_json_encoder.py
 wizata_dsapi/execution.py
 wizata_dsapi/experiment.py
+wizata_dsapi/ilogger.py
 wizata_dsapi/mlmodel.py
 wizata_dsapi/model_toolkit.py
 wizata_dsapi/pipeline.py
 wizata_dsapi/plot.py
 wizata_dsapi/request.py
 wizata_dsapi/script.py
 wizata_dsapi/template.py
```

### Comparing `wizata-dsapi-0.3.6/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.3.7/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

