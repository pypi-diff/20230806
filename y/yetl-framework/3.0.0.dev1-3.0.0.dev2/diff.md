# Comparing `tmp/yetl-framework-3.0.0.dev1.tar.gz` & `tmp/yetl-framework-3.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-3.0.0.dev1.tar", last modified: Sun Aug  6 10:48:11 2023, max compression
+gzip compressed data, was "yetl-framework-3.0.0.dev2.tar", last modified: Sun Aug  6 15:59:50 2023, max compression
```

## Comparing `yetl-framework-3.0.0.dev1.tar` & `yetl-framework-3.0.0.dev2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.879487 yetl-framework-3.0.0.dev1/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      216 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19653 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    12636 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    15064 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/resource/tables.xlsx
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-06 10:47:02.000000 yetl-framework-3.0.0.dev1/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 10:48:11.883487 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-06 10:48:11.000000 yetl-framework-3.0.0.dev1/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.105625 yetl-framework-3.0.0.dev2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 15:59:50.105625 yetl-framework-3.0.0.dev2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-06 15:59:50.105625 yetl-framework-3.0.0.dev2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.093625 yetl-framework-3.0.0.dev2/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1764 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.093625 yetl-framework-3.0.0.dev2/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.093625 yetl-framework-3.0.0.dev2/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17399 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.097625 yetl-framework-3.0.0.dev2/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4780 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2112 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      216 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9867 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19653 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.097625 yetl-framework-3.0.0.dev2/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5213 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6707 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4534 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.101625 yetl-framework-3.0.0.dev2/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    12876 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    15074 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.101625 yetl-framework-3.0.0.dev2/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1495 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.101625 yetl-framework-3.0.0.dev2/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-08-06 15:58:41.000000 yetl-framework-3.0.0.dev2/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-06 15:59:50.105625 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-08-06 15:59:50.000000 yetl-framework-3.0.0.dev2/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-3.0.0.dev1/PKG-INFO` & `yetl-framework-3.0.0.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 3.0.0.dev1
+Version: 3.0.0.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-3.0.0.dev1/README.md` & `yetl-framework-3.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/setup.py` & `yetl-framework-3.0.0.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="3.0.0.dev1",
+    version="3.0.0.dev2",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-3.0.0.dev1/yetl/__main__.py` & `yetl-framework-3.0.0.dev2/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/cli/_init.py` & `yetl-framework-3.0.0.dev2/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-3.0.0.dev2/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/__init__.py` & `yetl-framework-3.0.0.dev2/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_config.py` & `yetl-framework-3.0.0.dev2/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_decorators.py` & `yetl-framework-3.0.0.dev2/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_logging_config.py` & `yetl-framework-3.0.0.dev2/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_project.py` & `yetl-framework-3.0.0.dev2/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_spark_context.py` & `yetl-framework-3.0.0.dev2/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_tables.py` & `yetl-framework-3.0.0.dev2/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_timeslice.py` & `yetl-framework-3.0.0.dev2/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/_utils.py` & `yetl-framework-3.0.0.dev2/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/deltalake.py` & `yetl-framework-3.0.0.dev2/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/table/_deltalake.py` & `yetl-framework-3.0.0.dev2/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/table/_factory.py` & `yetl-framework-3.0.0.dev2/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/table/_read.py` & `yetl-framework-3.0.0.dev2/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/config/table/_table.py` & `yetl-framework-3.0.0.dev2/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/resource/__init__.py` & `yetl-framework-3.0.0.dev2/yetl/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9690104166666668%*

 * *Differences: {"'$defs'": "{'read': OrderedDict([('type', 'object'), ('description', 'read table type is used "*

 * *            'for spark read table properties, typically used for reading files in object '*

 * *            "storage'), ('properties', OrderedDict([('trigger', OrderedDict([('type', ['string', "*

 * *            "'null']), ('description', 'filemask patter to use as a trgger')])), ('trigger_type', "*

 * *            "OrderedDict([('type', ['string', 'null']), ('description', 'type of trgger')])), "*

 * *            "('container', O […]*

```diff
@@ -172,14 +172,94 @@
                 }
             },
             "type": [
                 "object",
                 "null"
             ]
         },
+        "read": {
+            "description": "read table type is used for spark read table properties, typically used for reading files in object storage",
+            "properties": {
+                "container": {
+                    "description": "type of trgger",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "filename": {
+                    "description": "filename mask",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "filename_date_format": {
+                    "description": "define a date format jinja variable for filename dates",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "format": {
+                    "description": "format of the landing file",
+                    "enum": [
+                        "cloudFiles",
+                        "csv",
+                        "json",
+                        "parquet"
+                    ],
+                    "type": "string"
+                },
+                "location": {
+                    "description": "file directory location",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "options": {
+                    "$ref": "#/$defs/options"
+                },
+                "path_date_format": {
+                    "description": "define a date format jinja variable for file paths",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "slice_date": {
+                    "description": "either the filename_date_format or the path_date_format used to shred the time period from the filename or path respectively",
+                    "enum": [
+                        "filename_date_format",
+                        "path_date_format"
+                    ],
+                    "type": "string"
+                },
+                "spark_schema": {
+                    "description": "relative path to where the spark definition is held",
+                    "type": "string"
+                },
+                "trigger": {
+                    "description": "filemask patter to use as a trgger",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
+                },
+                "trigger_type": {
+                    "description": "type of trgger",
+                    "type": [
+                        "string",
+                        "null"
+                    ]
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
@@ -222,92 +302,15 @@
             },
             "type": "object"
         },
         "landing": {
             "description": "definition of the landing stage and files",
             "properties": {
                 "read": {
-                    "description": "read table type is used for spark read table properties, typically used for reading files in object storage",
-                    "properties": {
-                        "container": {
-                            "description": "type of trgger",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "filename": {
-                            "description": "filename mask",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "filename_date_format": {
-                            "description": "define a date format jinja variable for filename dates",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "format": {
-                            "description": "format of the landing file",
-                            "enum": [
-                                "cloudFiles",
-                                "csv",
-                                "json",
-                                "parquet"
-                            ],
-                            "type": "string"
-                        },
-                        "location": {
-                            "description": "file directory location",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "options": {
-                            "$ref": "#/$defs/options"
-                        },
-                        "path_date_format": {
-                            "description": "define a date format jinja variable for file paths",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "slice_date": {
-                            "description": "either the filename_date_format or the path_date_format used to shred the time period from the filename or path respectively",
-                            "enum": [
-                                "filename_date_format",
-                                "path_date_format"
-                            ],
-                            "type": "string"
-                        },
-                        "spark_schema": {
-                            "description": "relative path to where the spark definition is held",
-                            "type": "string"
-                        },
-                        "trigger": {
-                            "description": "filemask patter to use as a trgger",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "trigger_type": {
-                            "description": "type of trgger",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
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
@@ -316,14 +319,38 @@
             "properties": {
                 "delta_lake": {
                     "$ref": "#/$defs/delta_lake"
                 }
             },
             "type": "object"
         },
+        "source": {
+            "description": "definition of the landing stage and files",
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

### Comparing `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-3.0.0.dev2/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444445%*

 * *Differences: {"'$defs'": "{'delta_lake_table': {'type': ['object', 'null']}}"}*

```diff
@@ -156,15 +156,18 @@
                             },
                             "type": "array",
                             "uniqueItems": true
                         }
                     ]
                 }
             },
-            "type": "object"
+            "type": [
+                "object",
+                "null"
+            ]
         },
         "delta_properties": {
             "description": "holds key value pairs of delta properties",
             "minProperties": 1,
             "properties": {
                 "delta.appendOnly": {
                     "description": "true for this Delta table to be append-only. If append-only, existing records cannot be deleted, and existing values cannot be updated.",
```

### Comparing `yetl-framework-3.0.0.dev1/yetl/resource/tables.xlsx` & `yetl-framework-3.0.0.dev2/yetl/resource/tables.xlsx`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/validation/_validate.py` & `yetl-framework-3.0.0.dev2/yetl/validation/_validate.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/workflow/_dlt.py` & `yetl-framework-3.0.0.dev2/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl/workflow/_multi_threaded.py` & `yetl-framework-3.0.0.dev2/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-3.0.0.dev1/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-3.0.0.dev2/yetl_framework.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 3.0.0.dev1
+Version: 3.0.0.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-3.0.0.dev1/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-3.0.0.dev2/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

