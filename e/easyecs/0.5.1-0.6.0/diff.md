# Comparing `tmp/easyecs-0.5.1.tar.gz` & `tmp/easyecs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.5.1.tar", max compression
+gzip compressed data, was "easyecs-0.6.0.tar", max compression
```

## Comparing `easyecs-0.5.1.tar` & `easyecs-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     2230 2023-08-05 13:35:35.058413 easyecs-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/__init__.py
--rwxr-xr-x   0        0        0     9052 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0       90 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/client.py
--rw-r--r--   0        0        0     3522 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0        0 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/stack/create.py
--rw-r--r--   0        0        0     1131 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/stack/delete.py
--rw-r--r--   0        0        0     3274 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/stack/update.py
--rw-r--r--   0        0        0     8573 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0    12373 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/command/__init__.py
--rw-r--r--   0        0        0     2173 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2292 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     3272 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     2804 2023-08-05 13:35:35.078413 easyecs-0.5.1/easyecs/model/ecs.py
--rw-r--r--   0        0        0      607 2023-08-05 13:35:35.078413 easyecs-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-08-06 18:23:23.367814 easyecs-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     9052 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0       90 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/client.py
+-rw-r--r--   0        0        0     3522 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/stack/create.py
+-rw-r--r--   0        0        0     1131 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/stack/delete.py
+-rw-r--r--   0        0        0     3274 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/stack/update.py
+-rw-r--r--   0        0        0     5469 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0     7379 2023-08-06 18:23:23.383814 easyecs-0.6.0/easyecs/cloudformation/template/task_definition.py
+-rw-r--r--   0        0        0    12373 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     2188 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2292 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     3272 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     3220 2023-08-06 18:23:23.387814 easyecs-0.6.0/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      607 2023-08-06 18:23:23.387814 easyecs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.6.0/PKG-INFO
```

### Comparing `easyecs-0.5.1/README.md` & `easyecs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/cli.py` & `easyecs-0.6.0/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/cloudformation/fetch.py` & `easyecs-0.6.0/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/cloudformation/stack/create.py` & `easyecs-0.6.0/easyecs/cloudformation/stack/create.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/cloudformation/stack/delete.py` & `easyecs-0.6.0/easyecs/cloudformation/stack/delete.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/cloudformation/stack/update.py` & `easyecs-0.6.0/easyecs/cloudformation/stack/update.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/command/__init__.py` & `easyecs-0.6.0/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/docker/__init__.py` & `easyecs-0.6.0/easyecs/docker/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,12 +55,13 @@
     push_cmd = f"docker push {image_name}"
     if show_docker_logs:
         res = subprocess.Popen(push_cmd, shell=True)
     else:
         res = subprocess.Popen(
             push_cmd, shell=True, stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL
         )
+    res.wait()
     if res.poll() != 0:
         raise Exception(
             "There was an issue pushing the docker image. Use --show-docker-logs to get"
             " more information!"
         )
```

### Comparing `easyecs-0.5.1/easyecs/helpers/common.py` & `easyecs-0.6.0/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/helpers/loader.py` & `easyecs-0.6.0/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/helpers/selector.py` & `easyecs-0.6.0/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/helpers/settings.py` & `easyecs-0.6.0/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.5.1/easyecs/model/ecs.py` & `easyecs-0.6.0/easyecs/model/ecs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Union
 from pydantic import BaseModel, computed_field, field_validator
 
 
 class EcsFileMetadataModel(BaseModel):
     appname: str
     user: str = os.environ["USER"]
 
@@ -64,27 +64,39 @@
 
 class EcsFileVolumeModel(BaseModel):
     name: str
     id: str
     mount_point: str
 
 
+class EcsFileContainerHealthCheckModel(BaseModel):
+    command: Union[List[str], str]
+    interval: int
+    retries: int
+    start_period: int
+    timeout: int
+
+
 class EcsFileContainerModel(BaseModel):
     name: str
     image: str
     user: str = "root"
     tty: bool = False
-    command: Optional[str] = None
+    essential: bool = True
+    entry_point: Union[Optional[str], Optional[List[str]]] = None
+    command: Union[Optional[str], Optional[List[str]]] = None
     resources: EcsFileResourcesModel
     build: Optional[EcsFileBuildModel] = None
     synchronize: Optional[EcsFileSynchronizeModel] = None
     port_forward: List[str] = []
     env: List[EcsFileEnvModel] = []
     secrets: List[EcsFileSecretModel] = []
     volumes: List[EcsFileVolumeModel] = []
+    healthcheck: Optional[EcsFileContainerHealthCheckModel] = None
+    depends_on: Optional[Dict[str, Dict[str, str]]] = None
 
 
 class EcsTaskDefinitionModel(BaseModel):
     resources: EcsFileResourcesModel
     containers: List[EcsFileContainerModel]
 
     @field_validator("containers")
```

### Comparing `easyecs-0.5.1/pyproject.toml` & `easyecs-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyecs"
-version = "0.5.1"
+version = "0.6.0"
 description = ""
 authors = ["BONVARLET Benjamin <benjaminbonvarlet96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.6"
```

### Comparing `easyecs-0.5.1/PKG-INFO` & `easyecs-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

