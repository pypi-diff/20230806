# Comparing `tmp/databroker-2.0.0b8.tar.gz` & `tmp/databroker-2.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/databroker-2.0.0b8.tar", last modified: Fri Aug  5 21:06:45 2022, max compression
+gzip compressed data, was "databroker-2.0.0b9.tar", last modified: Tue Sep 13 21:02:22 2022, max compression
```

## Comparing `databroker-2.0.0b8.tar` & `databroker-2.0.0b9.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.438037 databroker-2.0.0b8/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1590 2022-04-05 21:10:57.000000 databroker-2.0.0b8/LICENSE
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2022-04-05 21:10:57.000000 databroker-2.0.0b8/MANIFEST.in
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5073 2022-08-05 21:06:45.438037 databroker-2.0.0b8/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4245 2022-04-05 21:10:57.000000 databroker-2.0.0b8/README.rst
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.438037 databroker-2.0.0b8/databroker/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2590 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    71174 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/_core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      386 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/_factory_map.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1091 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/_legacy_images.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      499 2022-08-05 21:06:45.438037 databroker-2.0.0b8/databroker/_version.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/assets/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    30106 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/base_registry.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8449 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/column_hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12173 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4054 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/file_writers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    17448 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/handlers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      563 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/handlers_base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6592 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/mongo.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2439 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/mongo_core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1191 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/path_only_handlers.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/assets/readers/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/readers/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9148 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/readers/spe.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/assets/schemas/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      239 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/schemas/AD_HDF5_datum.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      394 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/schemas/AD_HDF5_resource.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      239 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/schemas/AD_SPE_datum.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      704 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/schemas/AD_SPE_resource.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14260 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/sqlite.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/assets/tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2244 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1645 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_asset.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1178 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_fs.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8470 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/assets/tests/test_fs_mutate.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13071 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/assets/tests/test_handlers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      656 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_mongo_details.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2843 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_reader.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4560 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_retrieve.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5216 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/test_write.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2080 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/tests/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3118 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/assets/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      209 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/broker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10472 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/client.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2088 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/common.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1755 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/databroker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5345 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/document.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/eventsource/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       20 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/eventsource/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9584 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/eventsource/archiver.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    17338 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/eventsource/shim.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/eventsource/tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/eventsource/tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1502 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/eventsource/tests/test_archiver.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      574 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/eventsource/tests/test_broker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      261 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/eventsource/tests/test_shim.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3113 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/eventsource/tests/utils.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/experimental/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/experimental/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2674 2022-08-04 17:29:06.000000 databroker-2.0.0b8/databroker/experimental/schemas.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18326 2022-08-04 17:29:06.000000 databroker-2.0.0b8/databroker/experimental/server_ext.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4891 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/from_files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      444 2022-07-19 21:08:22.000000 databroker-2.0.0b8/databroker/glue.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.434037 databroker-2.0.0b8/databroker/headersource/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       20 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/headersource/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18777 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/headersource/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27642 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/headersource/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7888 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/headersource/hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8453 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/headersource/mongo.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12044 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/headersource/mongo_core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3785 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/headersource/mongoquery.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1865 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/headersource/shim.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11895 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/headersource/sqlite.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7439 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/in_memory.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    82513 2022-08-05 21:05:45.000000 databroker-2.0.0b8/databroker/mongo_normalized.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1859 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/pims_readers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6767 2022-05-27 16:15:25.000000 databroker-2.0.0b8/databroker/pivot.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    17305 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/projector.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14941 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1978 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/server.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.438037 databroker-2.0.0b8/databroker/tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3481 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    35733 2022-05-27 16:54:05.000000 databroker-2.0.0b8/databroker/tests/test_broker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3183 2022-04-18 20:56:09.000000 databroker-2.0.0b8/databroker/tests/test_config.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2617 2022-04-18 20:56:09.000000 databroker-2.0.0b8/databroker/tests/test_document.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8145 2022-08-04 17:29:06.000000 databroker-2.0.0b8/databroker/tests/test_experimental.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      538 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_glue.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3533 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_humantime_munging.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1973 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_lazymap.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18956 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_mds.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4927 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_pivot.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7296 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tests/test_projector.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4188 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/tests/test_queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3592 2022-04-18 20:56:09.000000 databroker-2.0.0b8/databroker/tests/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3685 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/tutorial_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13188 2022-04-18 20:56:09.000000 databroker-2.0.0b8/databroker/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       49 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/v0.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    47465 2022-08-04 16:38:04.000000 databroker-2.0.0b8/databroker/v1.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      647 2022-04-05 21:10:57.000000 databroker-2.0.0b8/databroker/v2.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.430036 databroker-2.0.0b8/databroker.egg-info/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5073 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3149 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/SOURCES.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/dependency_links.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      186 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/entry_points.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      796 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/requires.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       11 2022-08-05 21:06:45.000000 databroker-2.0.0b8/databroker.egg-info/top_level.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       29 2022-04-18 20:56:09.000000 databroker-2.0.0b8/requirements-back-compat.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       52 2022-08-04 16:38:04.000000 databroker-2.0.0b8/requirements-client.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      173 2022-08-04 16:38:04.000000 databroker-2.0.0b8/requirements-server.txt
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2022-08-05 21:06:45.438037 databroker-2.0.0b8/scripts/
--rwxrwxr-x   0 dallan    (1000) dallan    (1000)     3417 2022-04-18 20:56:09.000000 databroker-2.0.0b8/scripts/fs_rename
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      213 2022-08-05 21:06:45.438037 databroker-2.0.0b8/setup.cfg
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2926 2022-08-04 16:38:04.000000 databroker-2.0.0b8/setup.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    68573 2022-08-04 16:38:04.000000 databroker-2.0.0b8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.786228 databroker-2.0.0b9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-09-13 21:02:13.000000 databroker-2.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-09-13 21:02:13.000000 databroker-2.0.0b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-09-13 21:02:22.786228 databroker-2.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-09-13 21:02:13.000000 databroker-2.0.0b9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.786228 databroker-2.0.0b9/databroker/
+-rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71174 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/_factory_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/_legacy_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-13 21:02:22.786228 databroker-2.0.0b9/databroker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/assets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30106 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/base_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8449 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/column_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4054 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/file_writers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17448 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/handlers_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/mongo_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/path_only_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/assets/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9148 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/readers/spe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/assets/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/schemas/AD_HDF5_datum.json
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/schemas/AD_HDF5_resource.json
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/schemas/AD_SPE_datum.json
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/schemas/AD_SPE_resource.json
+-rw-r--r--   0 runner    (1001) docker     (121)    14260 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/assets/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8470 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_fs_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13071 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_mongo_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5216 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/assets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10472 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/databroker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/document.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/eventsource/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9584 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17338 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/shim.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/eventsource/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/tests/test_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/tests/test_shim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/eventsource/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.782227 databroker-2.0.0b9/databroker/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/experimental/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18481 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/experimental/server_ext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4891 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/from_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/glue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.786228 databroker-2.0.0b9/databroker/headersource/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18777 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27642 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7888 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8453 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12044 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/mongo_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/mongoquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/shim.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11895 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/headersource/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    82513 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/mongo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/pims_readers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6767 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17305 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/projector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14941 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.786228 databroker-2.0.0b9/databroker/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3481 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35733 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8299 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_glue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_humantime_munging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_lazymap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18956 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_mds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7296 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_projector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4188 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/test_temp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/tutorial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13188 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/v0.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47465 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-09-13 21:02:13.000000 databroker-2.0.0b9/databroker/v2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.778227 databroker-2.0.0b9/databroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-13 21:02:22.000000 databroker-2.0.0b9/databroker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-13 21:02:13.000000 databroker-2.0.0b9/requirements-back-compat.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-13 21:02:13.000000 databroker-2.0.0b9/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-13 21:02:13.000000 databroker-2.0.0b9/requirements-server.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-13 21:02:22.786228 databroker-2.0.0b9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3417 2022-09-13 21:02:13.000000 databroker-2.0.0b9/scripts/fs_rename
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-09-13 21:02:22.786228 databroker-2.0.0b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-09-13 21:02:13.000000 databroker-2.0.0b9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68573 2022-09-13 21:02:13.000000 databroker-2.0.0b9/versioneer.py
```

### Comparing `databroker-2.0.0b8/LICENSE` & `databroker-2.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/MANIFEST.in` & `databroker-2.0.0b9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/PKG-INFO` & `databroker-2.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: databroker
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Unification of NSLS-II data sources
 Home-page: https://github.com/NSLS-II/databroker
 Author: Brookhaven National Laboratory
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -128,9 +127,7 @@
 .. _MongoDB query language: https://docs.mongodb.com/manual/reference/operator/query/
 
 .. _Bluesky Data Model: https://blueskyproject.io/event-model/data-model.html
 
 .. _Suitcase: https://blueskyproject.io/suitcase/
 
 .. _Intake: https://intake.readthedocs.io/en/latest/
-
-
```

### Comparing `databroker-2.0.0b8/README.rst` & `databroker-2.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/__init__.py` & `databroker-2.0.0b9/databroker/__init__.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/_core.py` & `databroker-2.0.0b9/databroker/_core.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/_legacy_images.py` & `databroker-2.0.0b9/databroker/_legacy_images.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/base_registry.py` & `databroker-2.0.0b9/databroker/assets/base_registry.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/column_hdf5.py` & `databroker-2.0.0b9/databroker/assets/column_hdf5.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/core.py` & `databroker-2.0.0b9/databroker/assets/core.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/file_writers.py` & `databroker-2.0.0b9/databroker/assets/file_writers.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/handlers.py` & `databroker-2.0.0b9/databroker/assets/handlers.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/handlers_base.py` & `databroker-2.0.0b9/databroker/assets/handlers_base.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/mongo.py` & `databroker-2.0.0b9/databroker/assets/mongo.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/mongo_core.py` & `databroker-2.0.0b9/databroker/assets/mongo_core.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/path_only_handlers.py` & `databroker-2.0.0b9/databroker/assets/path_only_handlers.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/readers/spe.py` & `databroker-2.0.0b9/databroker/assets/readers/spe.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/schemas/AD_SPE_resource.json` & `databroker-2.0.0b9/databroker/assets/schemas/AD_SPE_resource.json`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/sqlite.py` & `databroker-2.0.0b9/databroker/assets/sqlite.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/conftest.py` & `databroker-2.0.0b9/databroker/assets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_asset.py` & `databroker-2.0.0b9/databroker/assets/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_fs.py` & `databroker-2.0.0b9/databroker/assets/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_fs_mutate.py` & `databroker-2.0.0b9/databroker/assets/tests/test_fs_mutate.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_handlers.py` & `databroker-2.0.0b9/databroker/assets/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_mongo_details.py` & `databroker-2.0.0b9/databroker/assets/tests/test_mongo_details.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_reader.py` & `databroker-2.0.0b9/databroker/assets/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_retrieve.py` & `databroker-2.0.0b9/databroker/assets/tests/test_retrieve.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/test_write.py` & `databroker-2.0.0b9/databroker/assets/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/tests/utils.py` & `databroker-2.0.0b9/databroker/assets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/assets/utils.py` & `databroker-2.0.0b9/databroker/assets/utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/client.py` & `databroker-2.0.0b9/databroker/client.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/common.py` & `databroker-2.0.0b9/databroker/common.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/databroker.py` & `databroker-2.0.0b9/databroker/databroker.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/document.py` & `databroker-2.0.0b9/databroker/document.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/eventsource/archiver.py` & `databroker-2.0.0b9/databroker/eventsource/archiver.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/eventsource/shim.py` & `databroker-2.0.0b9/databroker/eventsource/shim.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/eventsource/tests/test_archiver.py` & `databroker-2.0.0b9/databroker/eventsource/tests/test_archiver.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/eventsource/tests/test_broker.py` & `databroker-2.0.0b9/databroker/eventsource/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/eventsource/tests/utils.py` & `databroker-2.0.0b9/databroker/eventsource/tests/utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/experimental/schemas.py` & `databroker-2.0.0b9/databroker/experimental/schemas.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/experimental/server_ext.py` & `databroker-2.0.0b9/databroker/experimental/server_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy
 import pymongo
 import sparse
 import zarr
 import zarr.storage
 
 from tiled.adapters.array import slice_and_shape_from_block_and_chunks
+from tiled.adapters.array import ArrayAdapter
 from tiled.adapters.dataframe import DataFrameAdapter
 from tiled.adapters.mapping import MapAdapter
 from tiled.adapters.utils import IndexersMixin, tree_repr
 from tiled.iterviews import KeysView, ItemsView, ValuesView
 from tiled.queries import (
     Contains,
     Comparison,
@@ -157,14 +158,17 @@
     def metadata(self):
         return self.doc.metadata
 
     @property
     def specs(self):
         return self.doc.specs
 
+    def __getitem__(self, key):
+        return ArrayAdapter(self.dataframe_adapter.read([key])[key].values)
+
     def read(self, *args, **kwargs):
         return self.dataframe_adapter.read(*args, **kwargs)
 
     def read_partition(self, *args, **kwargs):
         return self.dataframe_adapter.read_partition(*args, **kwargs)
 
     def microstructure(self):
```

### Comparing `databroker-2.0.0b8/databroker/from_files.py` & `databroker-2.0.0b9/databroker/from_files.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/base.py` & `databroker-2.0.0b9/databroker/headersource/base.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/core.py` & `databroker-2.0.0b9/databroker/headersource/core.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/hdf5.py` & `databroker-2.0.0b9/databroker/headersource/hdf5.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/mongo.py` & `databroker-2.0.0b9/databroker/headersource/mongo.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/mongo_core.py` & `databroker-2.0.0b9/databroker/headersource/mongo_core.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/mongoquery.py` & `databroker-2.0.0b9/databroker/headersource/mongoquery.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/shim.py` & `databroker-2.0.0b9/databroker/headersource/shim.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/headersource/sqlite.py` & `databroker-2.0.0b9/databroker/headersource/sqlite.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/in_memory.py` & `databroker-2.0.0b9/databroker/in_memory.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/mongo_normalized.py` & `databroker-2.0.0b9/databroker/mongo_normalized.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/pims_readers.py` & `databroker-2.0.0b9/databroker/pims_readers.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/pivot.py` & `databroker-2.0.0b9/databroker/pivot.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/projector.py` & `databroker-2.0.0b9/databroker/projector.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/queries.py` & `databroker-2.0.0b9/databroker/queries.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/server.py` & `databroker-2.0.0b9/databroker/server.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/conftest.py` & `databroker-2.0.0b9/databroker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_broker.py` & `databroker-2.0.0b9/databroker/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_config.py` & `databroker-2.0.0b9/databroker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_document.py` & `databroker-2.0.0b9/databroker/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_experimental.py` & `databroker-2.0.0b9/databroker/tests/test_experimental.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,17 @@
     client.write_dataframe(test_dataframe, metadata=metadata, specs=specs)
 
     results = client.search(Key("scan_id") == 1)
     result = results.values().first()
     result_dataframe = result.read()
 
     pandas.testing.assert_frame_equal(result_dataframe, test_dataframe)
+    # slicing into DataFrameClient returns ArrayClient
+    result_array = result["Column1"][:]
+    assert numpy.array_equal(result_array, dummy_array[0])
     assert result.metadata == metadata
     # TODO In the future this will be accessible via result.specs.
     assert result.item["attributes"]["specs"] == specs
 
 
 def test_queries(tmpdir):
```

### Comparing `databroker-2.0.0b8/databroker/tests/test_glue.py` & `databroker-2.0.0b9/databroker/tests/test_glue.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_humantime_munging.py` & `databroker-2.0.0b9/databroker/tests/test_humantime_munging.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_lazymap.py` & `databroker-2.0.0b9/databroker/tests/test_lazymap.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_mds.py` & `databroker-2.0.0b9/databroker/tests/test_mds.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_pivot.py` & `databroker-2.0.0b9/databroker/tests/test_pivot.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_projector.py` & `databroker-2.0.0b9/databroker/tests/test_projector.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/test_queries.py` & `databroker-2.0.0b9/databroker/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tests/utils.py` & `databroker-2.0.0b9/databroker/tests/utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/tutorial_utils.py` & `databroker-2.0.0b9/databroker/tutorial_utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/utils.py` & `databroker-2.0.0b9/databroker/utils.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/v1.py` & `databroker-2.0.0b9/databroker/v1.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/databroker/v2.py` & `databroker-2.0.0b9/databroker/v2.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 def temp():
     """
     Create a temporary Catalog backed by transient storage.
 
     This is intended for testing, teaching, an demos. The data does not
     persistent. Do not use this for anything important.
     """
-    from .mongo_normalized import Catalog
-    from tiled.client import from_catalog
+    from .mongo_normalized import MongoAdapter
+    from tiled.client import from_tree
 
-    catalog = Catalog.from_mongomock()  # service-side Catalog
-    client = from_catalog(catalog)  # client-side Catalog
+    catalog = MongoAdapter.from_mongomock()  # service-side Catalog
+    client = from_tree(catalog)  # client-side Catalog
     return client
```

### Comparing `databroker-2.0.0b8/databroker.egg-info/PKG-INFO` & `databroker-2.0.0b9/databroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: databroker
-Version: 2.0.0b8
+Version: 2.0.0b9
 Summary: Unification of NSLS-II data sources
 Home-page: https://github.com/NSLS-II/databroker
 Author: Brookhaven National Laboratory
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -128,9 +127,7 @@
 .. _MongoDB query language: https://docs.mongodb.com/manual/reference/operator/query/
 
 .. _Bluesky Data Model: https://blueskyproject.io/event-model/data-model.html
 
 .. _Suitcase: https://blueskyproject.io/suitcase/
 
 .. _Intake: https://intake.readthedocs.io/en/latest/
-
-
```

### Comparing `databroker-2.0.0b8/databroker.egg-info/SOURCES.txt` & `databroker-2.0.0b9/databroker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,9 +95,10 @@
 databroker/tests/test_glue.py
 databroker/tests/test_humantime_munging.py
 databroker/tests/test_lazymap.py
 databroker/tests/test_mds.py
 databroker/tests/test_pivot.py
 databroker/tests/test_projector.py
 databroker/tests/test_queries.py
+databroker/tests/test_temp.py
 databroker/tests/utils.py
 scripts/fs_rename
```

### Comparing `databroker-2.0.0b8/databroker.egg-info/requires.txt` & `databroker-2.0.0b9/databroker.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/scripts/fs_rename` & `databroker-2.0.0b9/scripts/fs_rename`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/setup.py` & `databroker-2.0.0b9/setup.py`

 * *Files identical despite different names*

### Comparing `databroker-2.0.0b8/versioneer.py` & `databroker-2.0.0b9/versioneer.py`

 * *Files identical despite different names*

