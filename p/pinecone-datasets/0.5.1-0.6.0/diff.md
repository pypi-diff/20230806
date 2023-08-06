# Comparing `tmp/pinecone_datasets-0.5.1.tar.gz` & `tmp/pinecone_datasets-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_datasets-0.5.1.tar", max compression
+gzip compressed data, was "pinecone_datasets-0.6.0.tar", max compression
```

## Comparing `pinecone_datasets-0.5.1.tar` & `pinecone_datasets-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     9002 2023-06-27 19:27:57.256133 pinecone_datasets-0.5.1/README.md
--rw-r--r--   0        0        0      221 2023-06-27 19:27:57.256477 pinecone_datasets-0.5.1/pinecone_datasets/__init__.py
--rw-r--r--   0        0        0     3471 2023-06-27 19:27:57.256891 pinecone_datasets-0.5.1/pinecone_datasets/catalog.py
--rw-r--r--   0        0        0     1185 2023-06-27 19:27:57.257561 pinecone_datasets-0.5.1/pinecone_datasets/cfg.py
--rw-r--r--   0        0        0    21934 2023-06-27 19:30:18.407338 pinecone_datasets-0.5.1/pinecone_datasets/dataset.py
--rw-r--r--   0        0        0      969 2023-06-27 19:27:57.258399 pinecone_datasets-0.5.1/pinecone_datasets/fs.py
--rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.5.1/pinecone_datasets/public.py
--rw-r--r--   0        0        0      881 2023-06-27 19:31:34.790867 pinecone_datasets-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9967 1970-01-01 00:00:00.000000 pinecone_datasets-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10419 2023-08-06 20:58:35.873252 pinecone_datasets-0.6.0/README.md
+-rw-r--r--   0        0        0      221 2023-08-06 20:58:35.873573 pinecone_datasets-0.6.0/pinecone_datasets/__init__.py
+-rw-r--r--   0        0        0     3471 2023-06-27 19:27:57.256891 pinecone_datasets-0.6.0/pinecone_datasets/catalog.py
+-rw-r--r--   0        0        0     1185 2023-06-27 19:27:57.257561 pinecone_datasets-0.6.0/pinecone_datasets/cfg.py
+-rw-r--r--   0        0        0    24775 2023-08-06 20:58:35.874038 pinecone_datasets-0.6.0/pinecone_datasets/dataset.py
+-rw-r--r--   0        0        0      969 2023-06-27 19:27:57.258399 pinecone_datasets-0.6.0/pinecone_datasets/fs.py
+-rw-r--r--   0        0        0     1657 2023-05-31 11:31:31.876795 pinecone_datasets-0.6.0/pinecone_datasets/public.py
+-rw-r--r--   0        0        0      862 2023-08-06 20:58:35.874386 pinecone_datasets-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11633 1970-01-01 00:00:00.000000 pinecone_datasets-0.6.0/setup.py
+-rw-r--r--   0        0        0    11343 1970-01-01 00:00:00.000000 pinecone_datasets-0.6.0/PKG-INFO
```

### Comparing `pinecone_datasets-0.5.1/pinecone_datasets/catalog.py` & `pinecone_datasets-0.6.0/pinecone_datasets/catalog.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.1/pinecone_datasets/cfg.py` & `pinecone_datasets-0.6.0/pinecone_datasets/cfg.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.1/pinecone_datasets/dataset.py` & `pinecone_datasets-0.6.0/pinecone_datasets/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import glob
+import sys
 import os
 import itertools
 import time
 import json
 import asyncio
 import warnings
 from urllib.parse import urlparse
@@ -25,15 +25,15 @@
 if version("pinecone-client").startswith("3"):
     from pinecone import Client as pc, Index
 elif version("pinecone-client").startswith("2"):
     import pinecone as pc
 
     try:
         from pinecone import GRPCIndex as Index
-    except:
+    except ImportError:
         from pinecone import Index
 else:
     warnings.warn(
         message="Pinecone client version not supported or non-existent,"
         + "please use pip ineall pinecone-client to install v2 or "
         + "pip install pinecone-datasets[clientv3] to install v3"
     )
@@ -78,17 +78,14 @@
     @classmethod
     def from_path(cls, dataset_path, **kwargs):
         """
         Create a Dataset object from local or cloud storage
         Args:
             dataset_path (str): a path to a local or cloud storage path containing a valid dataset.
 
-        Keyword Args:
-            engine (str): the engine to use for loading the dataset. Options are ['polars', 'pandas']. Defaults to 'pandas'.
-
         Returns:
             Dataset: a Dataset object
         """
         return cls(dataset_path=dataset_path, **kwargs)
 
     @classmethod
     def from_catalog(cls, dataset_id, catalog_base_path: str = "", **kwargs):
@@ -160,15 +157,15 @@
             column_mapping (Dict[str, str]): a dictionary mapping the columns of the DataFrame to the Pinecone Datasets Schema (col_name, pinecone_name)
             schema (List[Tuple[str, bool]]): the schema to validate against (column_name, is_nullable)
 
         Returns:
             pd.DataFrame: the validated, renamed DataFrame
         """
         if df is None or df.empty:
-            return pd.DataFrame(columns=[column_name for column_name, _ in schema])
+            return pd.DataFrame(columns=[column_name for column_name, _, _ in schema])
         else:
             if column_mapping is not None:
                 df.rename(columns=column_mapping, inplace=True)
             for column_name, is_nullable, null_value in schema:
                 if column_name not in df.columns and not is_nullable:
                     raise ValueError(
                         f"error, file is not matching Pinecone Datasets Schmea: {column_name} not found"
@@ -212,28 +209,45 @@
             if not self._fs.exists(self._dataset_path):
                 raise FileNotFoundError(
                     "Dataset does not exist. Please check the path or dataset_id"
                 )
         else:
             self._fs = None
             self._dataset_path = None
-        self._documents = pd.DataFrame(
-            columns=getattr(self._config.Schema.Names, "documents")
-        )
-        self._queries = pd.DataFrame(
-            columns=getattr(self._config.Schema.Names, "queries")
-        )
-        self._metadata = DatasetMetadata.empty()
+        self._documents = None
+        self._queries = None
+        self._metadata = None
         self._pinecone_client = None
 
     def _is_datatype_exists(self, data_type: str) -> bool:
         if not self._fs:
             raise DatasetInitializationError()
         return self._fs.exists(os.path.join(self._dataset_path, data_type))
 
+    @staticmethod
+    def _convert_metadata_from_dict_to_json(metadata: Optional[dict]) -> str:
+        if pd.isna(metadata):
+            return None
+        if metadata and not isinstance(metadata, dict):
+            raise TypeError(
+                f"metadata must be a dict but its {type(metadata)} meta = {metadata}"
+            )
+        return json.dumps(metadata, ensure_ascii=False)
+
+    @staticmethod
+    def _convert_metadata_from_json_to_dict(metadata: Optional[str]) -> dict:
+        if metadata is None:
+            return None
+        if not isinstance(metadata, str):
+            if isinstance(metadata, dict):
+                return metadata
+            else:
+                raise TypeError("metadata must be a string or dict")
+        return json.loads(metadata)
+
     def _safe_read_from_path(self, data_type: str) -> pd.DataFrame:
         if not self._fs:
             raise DatasetInitializationError()
 
         read_path_str = os.path.join(self._dataset_path, data_type, "*.parquet")
         read_path = self._fs.glob(read_path_str)
         if self._is_datatype_exists(data_type):
@@ -251,14 +265,25 @@
                 elif column_name not in dataset_schema_names and is_nullable:
                     columns_to_null.append((column_name, null_value))
                 else:
                     columns_not_null.append(column_name)
             try:
                 # TODO: use of the columns_not_null and columns_to_null is only a workaround for proper schema validation and versioning
                 df = dataset.read_pandas(columns=columns_not_null).to_pandas()
+
+                # metadta supposed to be a dict [if legacy] or string
+                if data_type == "documents":
+                    df["metadata"] = df["metadata"].apply(
+                        self._convert_metadata_from_json_to_dict
+                    )
+                elif data_type == "queries":
+                    df["filter"] = df["filter"].apply(
+                        self._convert_metadata_from_json_to_dict
+                    )
+
                 for column_name, null_value in columns_to_null:
                     df[column_name] = null_value
                 return df
             # TODO: add more specific error handling, explain what is wrong
             except Exception as e:
                 print("error, no exception: {}".format(e), file=sys.stderr)
                 raise (e)
@@ -266,15 +291,19 @@
             warnings.warn(
                 "WARNING: No data found at: {}. Returning empty DF".format(
                     read_path_str
                 ),
                 UserWarning,
                 stacklevel=0,
             )
-            return pd.DataFrame(columns=getattr(self._config.Schema.Names, data_type))
+            return pd.DataFrame(
+                columns=[
+                    col[0] for col in getattr(self._config.Schema.Names, data_type)
+                ]
+            )
 
     def _load_metadata(self) -> DatasetMetadata:
         if not self._fs:
             raise DatasetInitializationError()
 
         with self._fs.open(
             os.path.join(self._dataset_path, "metadata.json"), "rb"
@@ -294,15 +323,15 @@
             raise KeyError("Dataset does not have key: {}".format(key))
 
     def __len__(self) -> int:
         return self.documents.shape[0]
 
     @property
     def documents(self) -> pd.DataFrame:
-        if self._documents.empty:
+        if self._documents is None:
             self._documents = self._safe_read_from_path("documents")
         return self._documents
 
     def iter_documents(
         self, batch_size: int = 1, return_indexes=False
     ) -> Iterator[List[Dict[str, Any]]]:
         """
@@ -327,15 +356,15 @@
                 return_indexes=return_indexes,
             )
         else:
             raise ValueError("batch_size must be greater than 0")
 
     @property
     def queries(self) -> pd.DataFrame:
-        if self._queries.empty:
+        if self._queries is None:
             self._queries = self._safe_read_from_path("queries")
         return self._queries
 
     def iter_queries(self) -> Iterator[Dict[str, Any]]:
         """
         Iterates over the queries in the dataset.
 
@@ -349,15 +378,15 @@
         """
         return iter_pandas_dataframe_single(
             self.queries[self._config.Schema.queries_select_columns]
         )
 
     @property
     def metadata(self) -> DatasetMetadata:
-        if self._metadata.is_empty():
+        if self._metadata is None:
             self._metadata = self._load_metadata()
         return self._metadata
 
     def head(self, n: int = 5) -> pd.DataFrame:
         return self.documents.head(n)
 
     def to_path(self, dataset_path: str, **kwargs):
@@ -365,30 +394,45 @@
         Saves the dataset to a local or cloud storage path.
         """
         fs = get_cloud_fs(dataset_path, **kwargs)
 
         # save documents
         documents_path = os.path.join(dataset_path, "documents")
         fs.makedirs(documents_path, exist_ok=True)
-        self.documents.to_parquet(
-            os.path.join(documents_path, "part-0.parquet"),
-            engine="pyarrow",
-            index=False,
-            filesystem=fs,
-        )
-        # save queries
-        if not self.queries.empty:
-            queries_path = os.path.join(dataset_path, "queries")
-            fs.makedirs(queries_path, exist_ok=True)
-            self.queries.to_parquet(
-                os.path.join(queries_path, "part-0.parquet"),
+
+        documents_metadta_copy = self.documents["metadata"].copy()
+        try:
+            self.documents["metadata"] = self.documents["metadata"].apply(
+                self._convert_metadata_from_dict_to_json
+            )
+            self.documents.to_parquet(
+                os.path.join(documents_path, "part-0.parquet"),
                 engine="pyarrow",
                 index=False,
                 filesystem=fs,
             )
+        finally:
+            self.documents["metadata"] = documents_metadta_copy
+        # save queries
+        if not self.queries.empty:
+            queries_path = os.path.join(dataset_path, "queries")
+            fs.makedirs(queries_path, exist_ok=True)
+            queries_filter_copy = self.queries["filter"].copy()
+            try:
+                self.queries["filter"] = self.queries["filter"].apply(
+                    self._convert_metadata_from_dict_to_json
+                )
+                self.queries.to_parquet(
+                    os.path.join(queries_path, "part-0.parquet"),
+                    engine="pyarrow",
+                    index=False,
+                    filesystem=fs,
+                )
+            finally:
+                self.queries["filter"] = queries_filter_copy
         else:
             warnings.warn("Queries are empty, not saving queries")
 
         # save metadata
         with fs.open(os.path.join(dataset_path, "metadata.json"), "w") as f:
             json.dump(self.metadata.dict(), f)
 
@@ -408,29 +452,33 @@
             catalog_base_path
             if catalog_base_path
             else os.environ.get("DATASETS_CATALOG_BASEPATH", cfg.Storage.endpoint)
         )
         dataset_path = os.path.join(catalog_base_path, f"{dataset_id}")
         self.to_path(dataset_path, **kwargs)
 
-    async def _async_upsert(self, index_name: str, batch_size: int, concurrency: int):
+    async def _async_upsert(
+        self, index_name: str, namespace: str, batch_size: int, concurrency: int
+    ):
         pinecone_index = (
             self._pinecone_client.get_index(index_name=index_name)
             if version("pinecone-client").startswith("3")
             else Index(index_name=index_name)
         )
 
         sem = asyncio.Semaphore(concurrency)
 
         pinecone_failed_batches = []
 
         async def send_batch(i, batch):
             async with sem:
                 try:
-                    return await pinecone_index.upsert(vectors=batch, async_req=True)
+                    return await pinecone_index.upsert(
+                        vectors=batch, namespace=namespace, async_req=True
+                    )
                 except Exception as pe:
                     if i in pinecone_failed_batches:
                         raise pe
                     else:
                         pinecone_failed_batches.append(i)
                         return UpsertResponse(upserted_count=0)
 
@@ -462,27 +510,34 @@
         for task in asyncio.as_completed(failed_tasks):
             res = await task
             total_upserted_count += res.upserted_count
             pbar.update(res.upserted_count)
 
         return {"upserted_count": total_upserted_count}
 
-    def _create_index(
+    def _set_pinecone_index(
         self,
-        index_name: str,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
         **kwargs,
-    ) -> Index:
+    ) -> None:
         if version("pinecone-client").startswith("3"):
             self._pinecone_client = pc(api_key=api_key, region=environment, **kwargs)
         elif version("pinecone-client").startswith("2"):
             pc.init(api_key=api_key, environment=environment, **kwargs)
             self._pinecone_client = pc
 
+    def _create_index(
+        self,
+        index_name: str,
+        api_key: Optional[str] = None,
+        environment: Optional[str] = None,
+        **kwargs,
+    ) -> Index:
+        self._set_pinecone_index(api_key=api_key, environment=environment)
         pinecone_index_list = self._pinecone_client.list_indexes()
 
         if index_name in pinecone_index_list:
             raise ValueError(
                 f"index {index_name} already exists, Pinecone Datasets can only be upserted to a new indexe"
             )
         else:
@@ -499,14 +554,16 @@
             except Exception as e:
                 print(f"error creating index: {e}")
                 return False
 
     def to_pinecone_index(
         self,
         index_name: str,
+        namespace: Optional[str] = "",
+        should_create_index: bool = True,
         batch_size: int = 100,
         concurrency: int = 10,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
         **kwargs,
     ):
         """
@@ -517,14 +574,15 @@
         - PINECONE_ENVIRONMENT
 
         Then, it will init a Pinecone Client and will perform an upsert to the index.
         The upsert will be using async batches to increase performance.
 
         Args:
             index_name (str): the name of the index to upsert to
+            namespace (str, optional): the namespace to use for the upsert. Defaults to "".
             batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
             concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
             see available parameters here: https://docs.pinecone.io/reference/create_index
 
@@ -533,40 +591,49 @@
             UpsertResponse: an object containing the upserted_count
 
         Examples:
             ```python
             result = dataset.to_pinecone_index(index_name="my_index")
             ```
         """
-
-        loop = asyncio.get_event_loop()
-        if loop.is_running():
-            raise RuntimeError(
-                "You are running inside a Jupyter Notebook or another Asyncio context. "
-                + "Plesae use the function to_pinecone_index_async instead. "
-                + "example: `await dataset.to_pinecone_index_async(index_name)`"
-            )
-
-        if not self._create_index(
-            index_name, api_key=api_key, environment=environment, **kwargs
-        ):
-            raise RuntimeError("index creation failed")
+        try:
+            loop = asyncio.get_event_loop()
+            if loop.is_running():
+                raise RuntimeError(
+                    "You are running inside a Jupyter Notebook or another Asyncio context. "
+                    + "Plesae use the function to_pinecone_index_async instead. "
+                    + "example: `await dataset.to_pinecone_index_async(index_name)`"
+                )
+        except:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+
+        if should_create_index:
+            if not self._create_index(
+                index_name, api_key=api_key, environment=environment, **kwargs
+            ):
+                raise RuntimeError("index creation failed")
+        else:
+            self._set_pinecone_index(api_key=api_key, environment=environment, **kwargs)
 
         # TODO: add concurrency = 0 as sync loop (def _upsert...) and add sync loop
 
         cor = self._async_upsert(
             index_name=index_name,
+            namespace=namespace,
             batch_size=batch_size,
             concurrency=concurrency,
         )
         return asyncio.run(cor)
 
     async def to_pinecone_index_async(
         self,
         index_name: str,
+        namespace: str = "",
+        should_create_index: bool = True,
         batch_size: int = 100,
         concurrency: int = 10,
         api_key: Optional[str] = None,
         environment: Optional[str] = None,
         **kwargs,
     ):
         """
@@ -577,14 +644,15 @@
         - PINECONE_ENVIRONMENT
 
         Then, it will init a Pinecone Client and will perform an upsert to the index.
         The upsert will be using async batches to increase performance.
 
         Args:
             index_name (str): the name of the index to upsert to
+            namespace (str, optional): the namespace to use for the upsert. Defaults to "".
             batch_size (int, optional): the batch size to use for the upsert. Defaults to 100.
             concurrency (int, optional): the concurrency to use for the upsert. Defaults to 10.
 
         Keyword Args:
             kwargs (Dict): additional arguments to pass to the Pinecone Client constructor when creating the index.
             see available parameters here: https://docs.pinecone.io/reference/create_index
 
@@ -593,19 +661,23 @@
             UpsertResponse: an object containing the upserted_count
 
         Examples:
             ```python
             result = await dataset.to_pinecone_index_async(index_name="my_index")
             ```
         """
-        if not self._create_index(
-            index_name, api_key=api_key, environment=environment, **kwargs
-        ):
-            raise RuntimeError("index creation failed")
+        if should_create_index:
+            if not self._create_index(
+                index_name, api_key=api_key, environment=environment, **kwargs
+            ):
+                raise RuntimeError("index creation failed")
+        else:
+            self._set_pinecone_index(api_key=api_key, environment=environment, **kwargs)
 
         res = await self._async_upsert(
             index_name=index_name,
+            namespace=namespace,
             batch_size=batch_size,
             concurrency=concurrency,
         )
 
         return res
```

### Comparing `pinecone_datasets-0.5.1/pinecone_datasets/fs.py` & `pinecone_datasets-0.6.0/pinecone_datasets/fs.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.1/pinecone_datasets/public.py` & `pinecone_datasets-0.6.0/pinecone_datasets/public.py`

 * *Files identical despite different names*

### Comparing `pinecone_datasets-0.5.1/pyproject.toml` & `pinecone_datasets-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "pinecone-datasets"
-version = "0.5.1"
+version = "0.6.0"
 description = "Pinecone Datasets lets you easily load datasets into your Pinecone index."
 authors = ["Pinecone"]
 maintainers = [
     "Roy Miara <miararoy@gmail.com>",
 ]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-polars = "^0.16.4"
 pyarrow = "^11.0.0"
 fsspec = "^2023.1.0"
 gcsfs = "^2023.1.0"
 s3fs = "^2023.1.0"
 pydantic = "^1.10.5"
 pandas = "^2.0.0"
 tqdm = "^4.65.0"
```

### Comparing `pinecone_datasets-0.5.1/PKG-INFO` & `pinecone_datasets-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-datasets
-Version: 0.5.1
+Version: 0.6.0
 Summary: Pinecone Datasets lets you easily load datasets into your Pinecone index.
 Author: Pinecone
 Maintainer: Roy Miara
 Maintainer-email: miararoy@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: clientv3
 Requires-Dist: fsspec (>=2023.1.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.1.0,<2024.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pinecone-client (==3.0.0rc2) ; extra == "clientv3"
-Requires-Dist: polars (>=0.16.4,<0.17.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Pinecone Datasets
@@ -104,14 +103,15 @@
     dense_model={"name": "bert", "dimension": 3},
     sparse_model={"name": "bm25"},
 )
 ```
 
 full metadata schema can be found in `pinecone_datasets.catalog.DatasetMetadata.schema`
 
+
 ### Loading your own dataset from catalog
 
 To set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
 
 ```bash
 export DATASETS_CATALOG_BASEPATH="s3://my-bucket/my-subdir"
 ```
@@ -122,35 +122,49 @@
 list_datasets()
 
 # ["my-dataset", ... ]
 
 dataset = load_dataset("my-dataset")
 ```
 
+additionally, you can load a dataset from the Dataset class
+
+```python
+
+from pinecone_datasets import Dataset
+
+dataset = Dataset.from_catalog("my-dataset")
+```
+
+
 ### Loading your own dataset from path
 
 You can load your own dataset from a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
 
 ```python
 from pinecone_datasets import Dataset
 
-dataset = Dataset("s3://my-bucket/my-subdir/my-dataset")
+dataset = Dataset.from_path("s3://my-bucket/my-subdir/my-dataset")
 ```
 
+This assumes that the path is structured as described in the Expected dataset structure section
+
 ### Loading from a pandas dataframe
 
 Pinecone Datasets enables you to load a dataset from a pandas dataframe. This is useful for loading a dataset from a local file and saving it to a remote storage.
 The minimal required data is a documents dataset, and the minimal required columns are `id` and `values`. The `id` column is a unique identifier for the document, and the `values` column is a list of floats representing the document vector.
 
 ```python
 import pandas as pd
 
 df = pd.read_parquet("my-dataset.parquet")
 
-dataset = Dataset.from_pandas(df)
+metadata = DatasetMetadata(**metadata_dict)
+
+dataset = Dataset.from_pandas(documents = df, quries = None, metadata = metadata)
 ```
 
 Please check the documentation for more information on the expected dataframe schema. There's also a column mapping variable that can be used to map the dataframe columns to the expected schema.
 
 
 ## Usage - Accessing data
 
@@ -188,44 +202,81 @@
 
 ```python
 from pinecone_datasets import import_documents_keys_from_blob_to_metadata
 
 new_dataset = import_documents_keys_from_blob_to_metadata(dataset, keys=["text"])
 ```
 
+## Usage saving
+
+you can save your dataset to a catalog managed by you or to a local path or a remote path (GCS or S3). 
+
+### Saving to Catalog
+
+To set you own catalog endpoint, set the environment variable `DATASETS_CATALOG_BASEPATH` to your bucket. Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
+
+After this environment variable is set you can save your dataset to the catalog using the `save` function
+
+```python
+from pinecone_datasets import Dataset
+
+metadata = DatasetMetadata(**{"name": "my-dataset", ...})
+```
+
+---
+
+🚨 *NOTE* Dataset name in the metadata must match the `dataset_id` parameter you pass to the catalog, in this example 'my-dataset'
+
+---
+
+```python
+dataset = Dataset.from_pandas(documents, queries, metadata)
+dataset.to_catalog("my-dataset")
+```
+
+### Saving to Path
+
+You can save your dataset to a local path or a remote path (GCS or S3). Note that pinecone uses the default authentication method for the storage type (gcsfs for GCS and s3fs for S3).
+
+```python
+dataset = Dataset.from_pandas(documents, queries, metadata)
+dataset.to_path("s3://my-bucket/my-subdir/my-dataset")
+```
 
 ### upserting to Index
 
 When upserting a Dataset to an Index, only the document data will be upserted to the index. The queries data will be ignored. 
 
 TODO: add example for API Key adn Environment Variables
 
 ```python
 ds = load_dataset("dataset_name")
 
-# If index exists
-ds.to_index("index_name")
+ds.to_pinecone_index("index_name")
+
+# or, if you run in notebook environment
 
-# If index does not exist use create_index=True, this will create the index with the default pinecone settings and dimension from the dataset metadata.
-ds.to_index("index_name", create_index=True)
+await ds.to_pinecone_index_async("index_name")
 
 ```
 
 the `to_index` function also accepts additional parameters
 
 * `batch_size` and `concurrency` - for controlling the upserting process
 * `kwargs` - for passing additional parameters to the index creation process
 
 
+
 ## For developers
 
 This project is using poetry for dependency managemet. supported python version are 3.8+. To start developing, on project root directory run:
 
 ```bash
 poetry install --with dev
 ```
 
 To run test locally run 
 
 ```bash
 poetry run pytest --cov pinecone_datasets
 ```
+
```

