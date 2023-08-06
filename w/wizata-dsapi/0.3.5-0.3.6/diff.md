# Comparing `tmp/wizata-dsapi-0.3.5.tar.gz` & `tmp/wizata-dsapi-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.3.5.tar", last modified: Sat Aug  5 12:09:38 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.3.6.tar", last modified: Sat Aug  5 12:33:35 2023, max compression
```

## Comparing `wizata-dsapi-0.3.5.tar` & `wizata-dsapi-0.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:09:38.801330 wizata-dsapi-0.3.5/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:09:38.801207 wizata-dsapi-0.3.5/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-05 12:09:38.801375 wizata-dsapi-0.3.5/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-05 12:09:27.000000 wizata-dsapi-0.3.5/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:09:38.799820 wizata-dsapi-0.3.5/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.5/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5716 2023-08-05 12:09:27.000000 wizata-dsapi-0.3.5/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.5/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.5/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.5/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.5/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.5/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.5/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.5/wizata_dsapi/wizata_dsapi_client.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:09:38.801021 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:09:38.000000 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-05 12:09:38.000000 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-05 12:09:38.000000 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-05 12:09:38.000000 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-05 12:09:38.000000 wizata-dsapi-0.3.5/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.340900 wizata-dsapi-0.3.6/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:33:35.340791 wizata-dsapi-0.3.6/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-05 12:33:35.340939 wizata-dsapi-0.3.6/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-05 12:33:31.000000 wizata-dsapi-0.3.6/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.339957 wizata-dsapi-0.3.6/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.6/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5717 2023-08-05 12:33:31.000000 wizata-dsapi-0.3.6/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.6/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.6/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.6/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.6/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.6/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-05 12:33:35.340638 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-05 12:33:35.000000 wizata-dsapi-0.3.6/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.3.5/LICENSE.txt` & `wizata-dsapi-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/setup.py` & `wizata-dsapi-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.3.5',
+    version='0.3.6',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/__init__.py` & `wizata-dsapi-0.3.6/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.3.6/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/context.py` & `wizata-dsapi-0.3.6/wizata_dsapi/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         self.__new_model = ml_model
         return ml_model
 
     def get_model(self) -> MLModel:
         """
         get model to be added to the context.
         """
-        return self.__new_plot
+        return self.__new_model
 
     def reset(self):
         """
         reset context between step execution - remove all step info, but keep all data.
         """
         self.__new_plot = None
         self.__new_model = None
```

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.3.6/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.3.6/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.3.6/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.3.6/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/execution.py` & `wizata-dsapi-0.3.6/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/experiment.py` & `wizata-dsapi-0.3.6/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.3.6/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.3.6/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.3.6/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/plot.py` & `wizata-dsapi-0.3.6/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/request.py` & `wizata-dsapi-0.3.6/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/script.py` & `wizata-dsapi-0.3.6/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/template.py` & `wizata-dsapi-0.3.6/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/twin.py` & `wizata-dsapi-0.3.6/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.3.6/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.3.6/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.3.6/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.5/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.3.6/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

