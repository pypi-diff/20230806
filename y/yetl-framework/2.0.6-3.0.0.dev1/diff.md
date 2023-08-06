# Comparing `tmp/yetl-framework-2.0.6.tar.gz` & `tmp/yetl-framework-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-2.0.6.tar", last modified: Tue Aug  1 19:00:43 2023, max compression
+gzip compressed data, was "yetl-framework-3.0.0.dev1.tar", last modified: Sun Aug  6 10:48:11 2023, max compression
```

## Comparing `yetl-framework-2.0.6.tar` & `yetl-framework-3.0.0.dev1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.351111 yetl-framework-2.0.6/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-08-01 19:00:43.351111 yetl-framework-2.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-01 19:00:43.351111 yetl-framework-2.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1539 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.339111 yetl-framework-2.0.6/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.339111 yetl-framework-2.0.6/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.339111 yetl-framework-2.0.6/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.343111 yetl-framework-2.0.6/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19653 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.343111 yetl-framework-2.0.6/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.347111 yetl-framework-2.0.6/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14625 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/sibytes_yetl_tables_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/resource/tables.xlsx
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.347111 yetl-framework-2.0.6/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.351111 yetl-framework-2.0.6/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-01 18:59:41.000000 yetl-framework-2.0.6/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-01 19:00:43.351111 yetl-framework-2.0.6/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-01 19:00:43.000000 yetl-framework-2.0.6/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      216 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19653 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    15064 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-2.0.6/PKG-INFO` & `yetl-framework-3.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.6
+Version: 3.0.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.6/README.md` & `yetl-framework-3.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/setup.py` & `yetl-framework-3.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="2.0.6",
+    version="3.0.0.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-2.0.6/yetl/__main__.py` & `yetl-framework-3.0.0.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/cli/_init.py` & `yetl-framework-3.0.0.dev1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/__init__.py` & `yetl-framework-3.0.0.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_config.py` & `yetl-framework-3.0.0.dev1/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_decorators.py` & `yetl-framework-3.0.0.dev1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_logging_config.py` & `yetl-framework-3.0.0.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_project.py` & `yetl-framework-3.0.0.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_spark_context.py` & `yetl-framework-3.0.0.dev1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_tables.py` & `yetl-framework-3.0.0.dev1/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_timeslice.py` & `yetl-framework-3.0.0.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/_utils.py` & `yetl-framework-3.0.0.dev1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/deltalake.py` & `yetl-framework-3.0.0.dev1/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/table/_deltalake.py` & `yetl-framework-3.0.0.dev1/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/table/_factory.py` & `yetl-framework-3.0.0.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/table/_read.py` & `yetl-framework-3.0.0.dev1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/config/table/_table.py` & `yetl-framework-3.0.0.dev1/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/resource/__init__.py` & `yetl-framework-3.0.0.dev1/yetl/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9752604166666666%*

 * *Differences: {"'$defs'": "{'read': OrderedDict([('type', 'object'), ('description', 'read table type is used "*

 * *            'for spark read table properties, typically used for reading files in object '*

 * *            "storage'), ('minProperties', 1), ('maxProperties', 1), ('patternProperties', "*

 * *            "OrderedDict([('^\\\\S+$', OrderedDict([('type', 'object'), ('description', 'name of "*

 * *            "the volume holding the files'), ('minProperties', 1), ('patternProperties', "*

 * *            "OrderedDict([('^\\\\S+$', Or […]*

```diff
@@ -265,14 +265,36 @@
                         "string",
                         "boolean"
                     ]
                 }
             },
             "type": "object"
         },
+        "read": {
+            "description": "read table type is used for spark read table properties, typically used for reading files in object storage",
+            "maxProperties": 1,
+            "minProperties": 1,
+            "patternProperties": {
+                "^\\S+$": {
+                    "description": "name of the volume holding the files",
+                    "minProperties": 1,
+                    "patternProperties": {
+                        "^\\S+$": {
+                            "description": "name or partname of the file that indicates the data table e.g. customers_20201001.csv would be customers",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        }
+                    },
+                    "type": "object"
+                }
+            },
+            "type": "object"
+        },
         "thresholds": {
             "description": "table etl thresholds",
             "properties": {
                 "invalid_ratio": {
                     "description": "decimal between 0 and 1 specifying the ratio of invalid rows to valid rows threshold",
                     "exclusiveMinimum": 0,
                     "maximum": 1,
@@ -315,34 +337,15 @@
             },
             "type": "object"
         },
         "landing": {
             "description": "definition of the landing stage and files",
             "properties": {
                 "read": {
-                    "description": "read table type is used for spark read table properties, typically used for reading files in object storage",
-                    "maxProperties": 1,
-                    "minProperties": 1,
-                    "patternProperties": {
-                        "^\\S+$": {
-                            "description": "name of the volume holding the files",
-                            "minProperties": 1,
-                            "patternProperties": {
-                                "^\\S+$": {
-                                    "description": "name or partname of the file that indicates the data table e.g. customers_20201001.csv would be customers",
-                                    "type": [
-                                        "string",
-                                        "null"
-                                    ]
-                                }
-                            },
-                            "type": "object"
-                        }
-                    },
-                    "type": "object"
+                    "$ref": "#/$defs/read"
                 }
             },
             "required": [
                 "read"
             ],
             "type": "object"
         },
@@ -351,14 +354,38 @@
             "properties": {
                 "delta_lake": {
                     "$ref": "#/$defs/delta_lake"
                 }
             },
             "type": "object"
         },
+        "source": {
+            "description": "definition of the source stage",
+            "oneOf": [
+                {
+                    "required": [
+                        "read"
+                    ]
+                },
+                {
+                    "required": [
+                        "delta_lake"
+                    ]
+                }
+            ],
+            "properties": {
+                "delta_lake": {
+                    "$ref": "#/$defs/delta_lake"
+                },
+                "read": {
+                    "$ref": "#/$defs/read"
+                }
+            },
+            "type": "object"
+        },
         "version": {
             "description": "version of yetl that the configuration is compatible with",
             "pattern": "^(\\d+\\.)?(\\d+\\.)?(\\*|\\d+)$",
             "type": "string"
         }
     },
     "required": [
```

### Comparing `yetl-framework-2.0.6/yetl/resource/tables.xlsx` & `yetl-framework-3.0.0.dev1/yetl/resource/tables.xlsx`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/validation/_validate.py` & `yetl-framework-3.0.0.dev1/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/workflow/_dlt.py` & `yetl-framework-3.0.0.dev1/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl/workflow/_multi_threaded.py` & `yetl-framework-3.0.0.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-2.0.6/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-3.0.0.dev1/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 2.0.6
+Version: 3.0.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-2.0.6/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-3.0.0.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

