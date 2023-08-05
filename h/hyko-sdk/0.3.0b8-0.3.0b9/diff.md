# Comparing `tmp/hyko_sdk-0.3.0b8.tar.gz` & `tmp/hyko_sdk-0.3.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b8.tar", last modified: Fri Aug  4 23:11:11 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b9.tar", last modified: Sat Aug  5 21:30:51 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b8.tar` & `hyko_sdk-0.3.0b9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b8/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       63 2023-08-04 19:54:46.000000 hyko_sdk-0.3.0b8/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b8/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b8/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1394 2023-08-04 23:10:51.000000 hyko_sdk-0.3.0b8/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:36:11.000000 hyko_sdk-0.3.0b8/hyko_sdk/py.typed
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b8/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 23:11:11.103898 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      304 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      114 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 23:11:11.000000 hyko_sdk-0.3.0b8/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b8/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      513 2023-08-04 23:11:11.107232 hyko_sdk-0.3.0b8/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-05 21:30:51.302500 hyko_sdk-0.3.0b9/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-05 21:30:51.302500 hyko_sdk-0.3.0b9/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b9/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-05 21:30:51.302500 hyko_sdk-0.3.0b9/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       63 2023-08-05 21:13:57.000000 hyko_sdk-0.3.0b9/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-05 18:38:42.000000 hyko_sdk-0.3.0b9/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1217 2023-08-05 21:14:26.000000 hyko_sdk-0.3.0b9/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 21:36:11.000000 hyko_sdk-0.3.0b9/hyko_sdk/py.typed
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2791 2023-08-05 21:18:31.000000 hyko_sdk-0.3.0b9/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-05 21:30:51.302500 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-05 21:30:51.000000 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-05 21:30:51.000000 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-05 21:30:51.000000 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      114 2023-08-05 21:30:51.000000 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-05 21:30:51.000000 hyko_sdk-0.3.0b9/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b9/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      513 2023-08-05 21:30:51.302500 hyko_sdk-0.3.0b9/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b8/hyko_sdk/io.py` & `hyko_sdk-0.3.0b9/hyko_sdk/io.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b8/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b9/hyko_sdk/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import AsyncIterator
+import json
+from typing import AsyncIterator, Callable
 from fastapi import HTTPException, status
 import httpx
+from hyko_sdk import CoreModel, MetaData
 import tqdm
 
 async def download_file(url: str) -> bytearray:
     async with httpx.AsyncClient(verify=False, http2=True) as client:
 
         # Get file size
         head_res = await client.head(url=url)
@@ -26,15 +28,15 @@
             with tqdm.tqdm(total=file_size, unit_scale=True, unit_divisor=1024, unit="B", desc=f"Downloading {url}") as progress:
                 data = bytearray()
                 async for chunk in response.aiter_bytes():
                     data += chunk
                     progress.update(len(chunk))
                 return data
 
-async def bytearray_aiter(data: bytearray, update_progress) -> AsyncIterator[bytearray]:
+async def bytearray_aiter(data: bytearray, update_progress: Callable[[float | None], bool | None]) -> AsyncIterator[bytearray]:
     step_size = int(len(data) / 100)
     if not step_size: step_size = 1
     for start in range(0, len(data), step_size):
         end = start + step_size
         if end > len(data):
             end = len(data)
         yield data[start:end]
@@ -46,8 +48,19 @@
         with tqdm.tqdm(total=file_size, unit_scale=True, unit_divisor=1024, unit="B", desc=f"Uploading {url}") as progress:
             res = await client.put(
                 url=url,
                 headers={"Content-Length": str(file_size)},
                 content=bytearray_aiter(data=data, update_progress=progress.update),
             )
             if not res.is_success:
-                raise Exception(f"Error while uploading, {res.text}")
+                raise Exception(f"Error while uploading, {res.text}")
+
+def metadata_to_docker_label(metadata: MetaData) -> str:
+    return metadata.model_dump_json(exclude_unset=True, exclude_none=True).replace('"', "'")
+
+    
+def docker_label_to_metadata(label: str) -> MetaData:
+    return MetaData(**json.loads(label.replace("'", '"')))
+
+def model_to_friendly_property_names(pydantic_model: CoreModel):
+    for _, field in pydantic_model.model_fields.items():
+        print(field.annotation)
```

### Comparing `hyko_sdk-0.3.0b8/setup.cfg` & `hyko_sdk-0.3.0b9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hyko_sdk
-version = 0.3.0b8
+version = 0.3.0b9
 author = Abdelmadjid Dahmani, Lotfi Lehamel
 author_email = amd2@big-mama.io, ll@big-mama.io
 url = https://hyko.ai
 
 [options]
 packages = find:
 python_requires = >=3.8
```

