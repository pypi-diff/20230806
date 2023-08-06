# Comparing `tmp/shaped_target_clickhouse-0.0.5.tar.gz` & `tmp/shaped_target_clickhouse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaped_target_clickhouse-0.0.5.tar", max compression
+gzip compressed data, was "shaped_target_clickhouse-0.0.6.tar", max compression
```

## Comparing `shaped_target_clickhouse-0.0.5.tar` & `shaped_target_clickhouse-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-08-01 17:47:34.294683 shaped_target_clickhouse-0.0.5/LICENSE
--rw-r--r--   0        0        0     4397 2023-08-01 17:47:34.294683 shaped_target_clickhouse-0.0.5/README.md
--rw-r--r--   0        0        0     1413 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       29 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/__init__.py
--rw-r--r--   0        0        0     5422 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/sinks.py
--rw-r--r--   0        0        0      849 2023-08-01 17:47:34.298683 shaped_target_clickhouse-0.0.5/target_clickhouse/target.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4397 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/README.md
+-rw-r--r--   0        0        0     1423 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/target_clickhouse/__init__.py
+-rw-r--r--   0        0        0     6551 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/target_clickhouse/sinks.py
+-rw-r--r--   0        0        0      849 2023-08-06 01:47:53.593351 shaped_target_clickhouse-0.0.6/target_clickhouse/target.py
+-rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.6/PKG-INFO
```

### Comparing `shaped_target_clickhouse-0.0.5/LICENSE` & `shaped_target_clickhouse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.5/README.md` & `shaped_target_clickhouse-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.5/pyproject.toml` & `shaped_target_clickhouse-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "shaped-target-clickhouse"
-version = "0.0.5"
+version = "0.0.6"
 description = "`target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Ben Theunissen"]
 keywords = [
     "ELT",
     "clickhouse",
 ]
 license = "Apache-2.0"
 packages = [
     { include = "target_clickhouse" },
 ]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = { version="^0.28.0" }
+singer-sdk = { version=">=0.28,<0.31" }
 fs-s3fs = { version = "^1.1.1", optional = true }
 clickhouse-sqlalchemy = "^0.2.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 tox = "^3.25.0"
 ruff = "^0.0.278"
-singer-sdk = { version="^0.28.0", extras = ["testing"] }
+singer-sdk = { version=">=0.28,<0.31", extras = ["testing"] }
 
 [tool.poetry.extras]
 s3 = ["fs-s3fs"]
 
 [tool.ruff]
 ignore = [
     "ANN101",  # missing-type-self
```

### Comparing `shaped_target_clickhouse-0.0.5/target_clickhouse/sinks.py` & `shaped_target_clickhouse-0.0.6/target_clickhouse/sinks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """clickhouse target sink class, which handles writing streams."""
 
 from __future__ import annotations
 
+import json
 import typing
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Iterable
 
 import sqlalchemy.types
 from clickhouse_sqlalchemy import (
     Table,
     engines,
 )
 from singer_sdk import typing as th
@@ -150,7 +151,36 @@
             return self.config.get("table_name")
 
         return self.connector.get_fully_qualified_name(
             table_name=self.table_name,
             schema_name=self.schema_name,
             db_name=self.database_name,
         )
+
+    def bulk_insert_records(
+            self,
+            full_table_name: str,
+            schema: dict,
+            records: Iterable[dict[str, Any]],
+        ) -> int | None:
+        """Bulk insert records to an existing destination table.
+
+        The default implementation uses a generic SQLAlchemy bulk insert operation.
+        This method may optionally be overridden by developers in order to provide
+        faster, native bulk uploads.
+
+        Args:
+            full_table_name: the target table name.
+            schema: the JSON schema for the new table, to be used when inferring column
+                names.
+            records: the input records.
+
+        Returns:
+            True if table exists, False if not, None if unsure or undetectable.
+        """
+        # Need to convert any records with a dict type to a JSON string.
+        for record in records:
+            for key, value in record.items():
+                if isinstance(value, dict):
+                    record[key] = json.dumps(value)
+
+        return super().bulk_insert_records(full_table_name, schema, records)
```

### Comparing `shaped_target_clickhouse-0.0.5/target_clickhouse/target.py` & `shaped_target_clickhouse-0.0.6/target_clickhouse/target.py`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.5/PKG-INFO` & `shaped_target_clickhouse-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: shaped-target-clickhouse
-Version: 0.0.5
+Version: 0.0.6
 Summary: `target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,clickhouse
 Author: Ben Theunissen
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: s3
 Requires-Dist: clickhouse-sqlalchemy (>=0.2.4,<0.3.0)
 Requires-Dist: fs-s3fs (>=1.1.1,<2.0.0) ; extra == "s3"
-Requires-Dist: singer-sdk (>=0.28.0,<0.29.0)
+Requires-Dist: singer-sdk (>=0.28,<0.31)
 Description-Content-Type: text/markdown
 
 # target-clickhouse
 
 `target-clickhouse` is a Singer target for clickhouse.
 
 Build with the [Meltano Target SDK](https://sdk.meltano.com).
```

