# Comparing `tmp/aporia-3.4.0.tar.gz` & `tmp/aporia-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-3.4.0.tar", max compression
+gzip compressed data, was "aporia-3.5.0.tar", max compression
```

## Comparing `aporia-3.4.0.tar` & `aporia-3.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2968 2023-07-04 13:25:22.345978 aporia-3.4.0/README.md
--rw-r--r--   0        0        0      829 2023-07-04 13:25:22.349979 aporia-3.4.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/__init__.py
--rw-r--r--   0        0        0      925 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/__init__.py
--rw-r--r--   0        0        0     1025 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/base.py
--rw-r--r--   0        0        0     1706 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/custom_metrics.py
--rw-r--r--   0        0        0     2370 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/data_source.py
--rw-r--r--   0        0        0     7465 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/dataset.py
--rw-r--r--   0        0        0     4660 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/model.py
--rw-r--r--   0        0        0    12069 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/monitor.py
--rw-r--r--   0        0        0     3052 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/segment.py
--rw-r--r--   0        0        0     2187 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/resources/version.py
--rw-r--r--   0        0        0    37860 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/as_code/stack.py
--rw-r--r--   0        0        0        0 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/__init__.py
--rw-r--r--   0        0        0     3233 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/aporia_api.py
--rw-r--r--   0        0        0      723 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/base.py
--rw-r--r--   0        0        0     1531 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/client.py
--rw-r--r--   0        0        0     2148 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/custom_metrics.py
--rw-r--r--   0        0        0     1822 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/dashboards.py
--rw-r--r--   0        0        0     3610 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/data_sources.py
--rw-r--r--   0        0        0     6709 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/datasets.py
--rw-r--r--   0        0        0     1844 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/messaging.py
--rw-r--r--   0        0        0     6108 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/metrics.py
--rw-r--r--   0        0        0     6326 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/models.py
--rw-r--r--   0        0        0    86057 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/monitors.py
--rw-r--r--   0        0        0     3506 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/segments.py
--rw-r--r--   0        0        0     3048 2023-07-04 13:25:22.349979 aporia-3.4.0/src/aporia/sdk/versions.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-07-10 15:30:27.273254 aporia-3.5.0/README.md
+-rw-r--r--   0        0        0      829 2023-07-10 15:30:27.273254 aporia-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/__init__.py
+-rw-r--r--   0        0        0      949 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0     1025 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1706 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     2370 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7465 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     4898 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0    12069 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     3052 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     2187 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    37860 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     3233 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      723 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1531 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2148 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1822 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3610 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6709 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     1844 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/messaging.py
+-rw-r--r--   0        0        0     6108 2023-07-10 15:30:27.273254 aporia-3.5.0/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     6599 2023-07-10 15:30:27.277254 aporia-3.5.0/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    86057 2023-07-10 15:30:27.277254 aporia-3.5.0/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     3506 2023-07-10 15:30:27.277254 aporia-3.5.0/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     3048 2023-07-10 15:30:27.277254 aporia-3.5.0/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.5.0/PKG-INFO
```

### Comparing `aporia-3.4.0/README.md` & `aporia-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/pyproject.toml` & `aporia-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aporia"
-version = "3.4.0"
+version = "3.5.0"
 description = ""
 authors = ["Aporia <support@aporia.com>"]
 readme = "README.md"
 packages = [
     { include = "aporia", from = "src" }
 ]
```

### Comparing `aporia-3.4.0/src/aporia/as_code/__init__.py` & `aporia-3.5.0/src/aporia/as_code/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from aporia.as_code.resources.segment import Segment
 from aporia.as_code.resources.version import Version
 from aporia.as_code.stack import Stack
 
 # Consts
 from aporia.sdk.data_sources import DataSourceType
 from aporia.sdk.datasets import DatasetType
-from aporia.sdk.models import ModelColor, ModelIcon, ModelType
+from aporia.sdk.models import ModelColor, ModelIcon, ModelType, ModelAggregationPeriod
 from aporia.sdk.monitors import (
     AverageMethod,
     BaselineConfiguration,
     DetectionMethod,
     FocalConfiguration,
     MessagingIntegrationType,
     MetricType,
```

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/base.py` & `aporia-3.5.0/src/aporia/as_code/resources/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/custom_metrics.py` & `aporia-3.5.0/src/aporia/as_code/resources/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/data_source.py` & `aporia-3.5.0/src/aporia/as_code/resources/data_source.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/dataset.py` & `aporia-3.5.0/src/aporia/as_code/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/model.py` & `aporia-3.5.0/src/aporia/as_code/resources/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.as_code.resources.custom_metrics import CustomMetric
 from aporia.as_code.resources.monitor import Monitor
 from aporia.as_code.resources.segment import Segment
 from aporia.as_code.resources.version import Version
 from aporia.sdk.client import Client
 from aporia.sdk.models import Model as _Model
-from aporia.sdk.models import ModelColor, ModelIcon, ModelType, NoOwner
+from aporia.sdk.models import ModelColor, ModelIcon, ModelType, NoOwner, ModelAggregationPeriod
 
 
 class Model(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
@@ -20,14 +20,15 @@
         # Model args
         type: Union[ModelType, str],
         name: Optional[str] = None,
         description: Optional[str] = None,
         icon: Optional[ModelIcon] = None,
         color: Optional[ModelColor] = None,
         owner: Optional[Union[str, NoOwner]] = NoOwner(),
+        aggregation_period: Optional[Union[ModelAggregationPeriod, str]] = None,
         # Model sub-resources
         versions: Optional[List[Version]] = None,
         segments: Optional[List[Segment]] = None,
         custom_metrics: Optional[List[CustomMetric]] = None,
         monitors: Optional[List[Monitor]] = None,
     ):
         self.sub_resources = []
@@ -44,14 +45,16 @@
             icon = ModelIcon(icon)
             self._args["icon"] = icon
         if color is not None:
             color = ModelColor(color)
             self._args["color"] = color
         if not isinstance(owner, NoOwner):
             self._args["owner"] = owner
+        if aggregation_period is not None:
+            self._args["aggregation_period"] = ModelAggregationPeriod(aggregation_period)
 
         for version in versions or []:
             self.sub_resources.append(
                 (version, lambda data, version: version.setarg("model_id", data["id"]))
             )
         for segment in segments or []:
             self.sub_resources.append(
```

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/monitor.py` & `aporia-3.5.0/src/aporia/as_code/resources/monitor.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/segment.py` & `aporia-3.5.0/src/aporia/as_code/resources/segment.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/resources/version.py` & `aporia-3.5.0/src/aporia/as_code/resources/version.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/as_code/stack.py` & `aporia-3.5.0/src/aporia/as_code/stack.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/aporia_api.py` & `aporia-3.5.0/src/aporia/sdk/aporia_api.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/base.py` & `aporia-3.5.0/src/aporia/sdk/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/client.py` & `aporia-3.5.0/src/aporia/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/custom_metrics.py` & `aporia-3.5.0/src/aporia/sdk/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/dashboards.py` & `aporia-3.5.0/src/aporia/sdk/dashboards.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/data_sources.py` & `aporia-3.5.0/src/aporia/sdk/data_sources.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/datasets.py` & `aporia-3.5.0/src/aporia/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/messaging.py` & `aporia-3.5.0/src/aporia/sdk/messaging.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/metrics.py` & `aporia-3.5.0/src/aporia/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/models.py` & `aporia-3.5.0/src/aporia/sdk/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     LIGHT_TEAL = "#39DAA3"
     PINK = "#EC87C0"
     PURPLE = "#AF72FD"
     GOLD = "#FFCE54"
     ORANGE = "#FC6E51"
 
 
+class ModelAggregationPeriod(Enum):
+    DAILY = "daily"
+    HOURLY = "hourly"
+
+
 class NoOwner:
     pass
 
 
 class Model(BaseAporiaResource):
     def __init__(self, client: Client, data: Dict):
         self.client = client
@@ -80,28 +85,31 @@
         client: Client,
         name: str,
         model_type: ModelType,
         description: Optional[str] = None,
         icon: Optional[ModelIcon] = None,
         color: Optional[ModelColor] = None,
         owner: Optional[Union[str, NoOwner]] = NoOwner(),
+        aggregation_period: Optional[ModelAggregationPeriod] = None,
     ) -> "Model":
         """Creates a new model in Aporia, and returns a new model descriptor."""
         model_type = ModelType(model_type)
 
         creation_parameters = {"name": name, "type": model_type.value}
 
         if description is not None:
             creation_parameters["description"] = description
         if icon is not None:
             creation_parameters["icon"] = icon.value
         if color is not None:
             creation_parameters["color"] = color.value
         if not isinstance(owner, NoOwner):
             creation_parameters["owner"] = owner
+        if aggregation_period is not None:
+            creation_parameters["aggregation_period"] = aggregation_period.value
 
         response = client.send_request(
             "/models",
             "POST",
             creation_parameters,
         )
```

### Comparing `aporia-3.4.0/src/aporia/sdk/monitors.py` & `aporia-3.5.0/src/aporia/sdk/monitors.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/segments.py` & `aporia-3.5.0/src/aporia/sdk/segments.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/src/aporia/sdk/versions.py` & `aporia-3.5.0/src/aporia/sdk/versions.py`

 * *Files identical despite different names*

### Comparing `aporia-3.4.0/PKG-INFO` & `aporia-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 3.4.0
+Version: 3.5.0
 Summary: 
 Author: Aporia
 Author-email: support@aporia.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

