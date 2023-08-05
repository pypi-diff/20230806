# Comparing `tmp/openc3-5.10.0.tar.gz` & `tmp/openc3-5.9.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openc3-5.10.0.tar", last modified: Sat Aug  5 23:48:51 2023, max compression
+gzip compressed data, was "openc3-5.9.2b0.tar", last modified: Fri Aug  4 17:12:46 2023, max compression
```

## Comparing `openc3-5.10.0.tar` & `openc3-5.9.2b0.tar`

### file list

```diff
@@ -1,143 +1,132 @@
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.301353 openc3-5.10.0/
--rw-r--r--   0 ryanmelt   (501) staff       (20)    37778 2023-08-05 02:26:43.000000 openc3-5.10.0/LICENSE.txt
--rw-r--r--   0 ryanmelt   (501) staff       (20)      105 2023-08-05 02:26:43.000000 openc3-5.10.0/MANIFEST.in
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2573 2023-08-05 23:48:51.301454 openc3-5.10.0/PKG-INFO
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1863 2023-08-05 02:26:43.000000 openc3-5.10.0/README.md
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.273228 openc3-5.10.0/examples/
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2000 2023-08-05 02:26:43.000000 openc3-5.10.0/examples/cosmos_v5_enterprise_example.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1958 2023-08-05 02:26:43.000000 openc3-5.10.0/examples/cosmos_v5_example.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2345 2023-08-05 02:26:43.000000 openc3-5.10.0/examples/cosmos_v5_stream_example.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      247 2023-08-05 02:26:43.000000 openc3-5.10.0/examples/test.txt
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.274300 openc3-5.10.0/openc3/
--rw-r--r--   0 ryanmelt   (501) staff       (20)      198 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      574 2023-08-05 02:27:52.000000 openc3-5.10.0/openc3/__version__.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.275583 openc3-5.10.0/openc3/accessors/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/accessors/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2248 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/accessors/accessor.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    47297 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/accessors/binary_accessor.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.277883 openc3-5.10.0/openc3/api/
--rw-r--r--   0 ryanmelt   (501) staff       (20)      795 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      764 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/authorized_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    19507 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/cmd_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     6215 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/interface_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1928 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/stash_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    20397 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/api/tlm_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     5827 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/environment.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.279434 openc3-5.10.0/openc3/io/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2062 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/io_multiplexer.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     7318 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/json_api_object.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     6018 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/json_drb_object.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    10670 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/json_rpc.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1109 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/stderr.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1110 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/io/stdout.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.280987 openc3-5.10.0/openc3/models/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    12403 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/cvt_model.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1920 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/interface_model.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     6015 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/model.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3237 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/reducer_model.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1698 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/stash_model.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4134 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/models/target_model.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.283367 openc3-5.10.0/openc3/packets/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    12363 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/commands.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     7710 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/limits.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3467 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/packet.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    26300 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/packet_config.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.283956 openc3-5.10.0/openc3/packets/parsers/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/parsers/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4256 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/parsers/packet_parser.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    23615 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/structure.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    15419 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/structure_item.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    17940 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/packets/telemetry.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.288510 openc3-5.10.0/openc3/script/
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1735 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    37372 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/api_shared.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     7123 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/authorization.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     9796 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/commands.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     9444 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/cosmos_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1677 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/decorators.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      799 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/exceptions.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1470 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/internal_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1350 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/limits.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4492 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/metadata.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4396 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/screen.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3648 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/server_proxy.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     6556 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/storage.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     7417 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/stream.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4432 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/stream_shared.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    18113 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/suite.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     5272 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/suite_results.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    10614 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/suite_runner.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3194 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/script/telemetry.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.289252 openc3-5.10.0/openc3/stream_api/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/stream_api/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1565 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/stream_api/base_client.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4588 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/stream_api/data_extractor_client.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3030 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/stream_api/log_message_client.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.289869 openc3-5.10.0/openc3/system/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/system/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     5056 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/system/system.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     8505 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/system/target.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3716 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/top_level.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.291443 openc3-5.10.0/openc3/topics/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3517 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/command_decom_topic.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3894 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/command_topic.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2695 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/decom_interface_topic.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1532 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/interface_topic.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1586 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/topics/topic.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.295551 openc3-5.10.0/openc3/utilities/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     5991 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/authentication.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1497 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/authorization.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     8776 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/aws_bucket.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3898 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/bucket.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4672 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/bucket_utilities.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1342 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/connection_pool.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     8481 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/extract.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      746 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/local_bucket.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1032 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/local_mode.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     4951 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/logger.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3889 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/message_log.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1545 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/script_shared.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1608 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/sleeper.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     8345 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/store.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1697 2023-08-05 02:26:43.000000 openc3-5.10.0/openc3/utilities/target_file.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.275081 openc3-5.10.0/openc3.egg-info/
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2573 2023-08-05 23:48:51.000000 openc3-5.10.0/openc3.egg-info/PKG-INFO
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3372 2023-08-05 23:48:51.000000 openc3-5.10.0/openc3.egg-info/SOURCES.txt
--rw-r--r--   0 ryanmelt   (501) staff       (20)        1 2023-08-05 23:48:51.000000 openc3-5.10.0/openc3.egg-info/dependency_links.txt
--rw-r--r--   0 ryanmelt   (501) staff       (20)       12 2023-08-05 23:48:51.000000 openc3-5.10.0/openc3.egg-info/top_level.txt
--rw-r--r--   0 ryanmelt   (501) staff       (20)       67 2023-08-05 23:48:51.301725 openc3-5.10.0/setup.cfg
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3834 2023-08-05 02:26:43.000000 openc3-5.10.0/setup.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.297119 openc3-5.10.0/test/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/__init__.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.298616 openc3-5.10.0/test/accessors/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/accessors/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    42817 2023-08-05 02:26:43.000000 openc3-5.10.0/test/accessors/test_binary_accessor_read.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    95302 2023-08-05 02:26:43.000000 openc3-5.10.0/test/accessors/test_binary_accessor_write.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.299341 openc3-5.10.0/test/api/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/api/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     6472 2023-08-05 02:26:43.000000 openc3-5.10.0/test/api/test_cmd_api.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2395 2023-08-05 02:26:43.000000 openc3-5.10.0/test/api/test_tlm_api.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.299717 openc3-5.10.0/test/config/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/config/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    22765 2023-08-05 02:26:43.000000 openc3-5.10.0/test/config/test_config_parser.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.300359 openc3-5.10.0/test/packets/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/packets/__init__.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.300671 openc3-5.10.0/test/packets/parsers/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/packets/parsers/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     3888 2023-08-05 02:26:43.000000 openc3-5.10.0/test/packets/parsers/test_packet_parser.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    27524 2023-08-05 02:26:43.000000 openc3-5.10.0/test/packets/test_structure.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)    11123 2023-08-05 02:26:43.000000 openc3-5.10.0/test/packets/test_structure_item.py
-drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-05 23:48:51.301173 openc3-5.10.0/test/script/
--rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-08-05 02:26:43.000000 openc3-5.10.0/test/script/__init__.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2586 2023-08-05 02:26:43.000000 openc3-5.10.0/test/script/test_api_shared.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2414 2023-08-05 02:26:43.000000 openc3-5.10.0/test/script/test_telemetry.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2654 2023-08-05 02:26:43.000000 openc3-5.10.0/test/test_authorization.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     1329 2023-08-05 02:26:43.000000 openc3-5.10.0/test/test_helper.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)      959 2023-08-05 02:26:43.000000 openc3-5.10.0/test/test_json_rpc_error.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2278 2023-08-05 02:26:43.000000 openc3-5.10.0/test/test_json_rpc_request.py
--rw-r--r--   0 ryanmelt   (501) staff       (20)     2858 2023-08-05 02:26:43.000000 openc3-5.10.0/test/test_json_rpc_response.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.398862 openc3-5.9.2b0/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    37778 2023-07-27 22:17:09.000000 openc3-5.9.2b0/LICENSE.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      105 2023-07-27 22:17:09.000000 openc3-5.9.2b0/MANIFEST.in
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2574 2023-08-04 17:12:46.398959 openc3-5.9.2b0/PKG-INFO
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1863 2023-07-27 22:17:09.000000 openc3-5.9.2b0/README.md
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.370315 openc3-5.9.2b0/examples/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2000 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_enterprise_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1958 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2345 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/cosmos_v5_stream_example.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      247 2023-07-27 22:17:09.000000 openc3-5.9.2b0/examples/test.txt
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.371092 openc3-5.9.2b0/openc3/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      198 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      579 2023-08-04 14:20:46.000000 openc3-5.9.2b0/openc3/__version__.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.372671 openc3-5.9.2b0/openc3/accessors/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/openc3/accessors/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2248 2023-08-01 16:42:30.000000 openc3-5.9.2b0/openc3/accessors/accessor.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    47372 2023-08-04 14:01:26.000000 openc3-5.9.2b0/openc3/accessors/binary_accessor.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.374922 openc3-5.9.2b0/openc3/api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      795 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      764 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/api/authorized_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    19507 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/cmd_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6215 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/interface_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1928 2023-08-04 13:58:29.000000 openc3-5.9.2b0/openc3/api/stash_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    20397 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/api/tlm_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5827 2023-08-04 01:56:57.000000 openc3-5.9.2b0/openc3/environment.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.376877 openc3-5.9.2b0/openc3/io/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2062 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/io/io_multiplexer.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7318 2023-08-04 03:14:31.000000 openc3-5.9.2b0/openc3/io/json_api_object.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6037 2023-08-04 03:07:34.000000 openc3-5.9.2b0/openc3/io/json_drb_object.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    10670 2023-08-01 16:42:30.000000 openc3-5.9.2b0/openc3/io/json_rpc.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1109 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/stderr.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1110 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/io/stdout.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.378193 openc3-5.9.2b0/openc3/models/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    12403 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/cvt_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1920 2023-08-01 23:35:45.000000 openc3-5.9.2b0/openc3/models/interface_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6015 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3237 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/reducer_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1698 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/models/stash_model.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4134 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/models/target_model.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.381046 openc3-5.9.2b0/openc3/packets/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    12363 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/commands.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7710 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/limits.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3467 2023-07-31 15:36:25.000000 openc3-5.9.2b0/openc3/packets/packet.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    25953 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/packet_config.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.381422 openc3-5.9.2b0/openc3/packets/parsers/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/parsers/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4264 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/packets/parsers/packet_parser.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    23560 2023-08-04 03:14:31.000000 openc3-5.9.2b0/openc3/packets/structure.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    15419 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/packets/structure_item.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    17940 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/packets/telemetry.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.386409 openc3-5.9.2b0/openc3/script/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1735 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    37372 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/api_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7123 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     9796 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/commands.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     9444 2023-08-02 00:19:22.000000 openc3-5.9.2b0/openc3/script/cosmos_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1677 2023-08-01 23:37:42.000000 openc3-5.9.2b0/openc3/script/decorators.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      799 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/exceptions.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1470 2023-08-02 00:19:40.000000 openc3-5.9.2b0/openc3/script/internal_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1350 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/limits.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4492 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/metadata.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4396 2023-08-02 03:25:30.000000 openc3-5.9.2b0/openc3/script/screen.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3648 2023-08-04 02:39:26.000000 openc3-5.9.2b0/openc3/script/server_proxy.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6556 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/storage.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     7417 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/stream.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4432 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/script/stream_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    18113 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/script/suite.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5272 2023-08-01 23:41:45.000000 openc3-5.9.2b0/openc3/script/suite_results.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    10614 2023-08-02 00:20:56.000000 openc3-5.9.2b0/openc3/script/suite_runner.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3194 2023-08-02 00:21:33.000000 openc3-5.9.2b0/openc3/script/telemetry.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.387311 openc3-5.9.2b0/openc3/stream_api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1565 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/base_client.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4588 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/stream_api/data_extractor_client.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3030 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/stream_api/log_message_client.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.389507 openc3-5.9.2b0/openc3/system/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/system/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5056 2023-08-01 23:42:17.000000 openc3-5.9.2b0/openc3/system/system.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8505 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/system/target.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3716 2023-08-01 17:27:18.000000 openc3-5.9.2b0/openc3/top_level.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.390802 openc3-5.9.2b0/openc3/topics/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3517 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/command_decom_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3894 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/topics/command_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2695 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/decom_interface_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1532 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/topics/interface_topic.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1586 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/topics/topic.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.394107 openc3-5.9.2b0/openc3/utilities/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     5990 2023-08-04 03:15:28.000000 openc3-5.9.2b0/openc3/utilities/authentication.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1497 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8776 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/aws_bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3898 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4672 2023-08-01 20:44:09.000000 openc3-5.9.2b0/openc3/utilities/bucket_utilities.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1342 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/connection_pool.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8481 2023-08-01 23:44:42.000000 openc3-5.9.2b0/openc3/utilities/extract.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      746 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/local_bucket.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1032 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/local_mode.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     4951 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/logger.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3889 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/message_log.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1545 2023-08-01 23:19:42.000000 openc3-5.9.2b0/openc3/utilities/script_shared.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1608 2023-07-27 22:17:09.000000 openc3-5.9.2b0/openc3/utilities/sleeper.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     8345 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/store.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1697 2023-08-02 22:48:03.000000 openc3-5.9.2b0/openc3/utilities/target_file.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.371958 openc3-5.9.2b0/openc3.egg-info/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2574 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/PKG-INFO
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3119 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        1 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)       12 2023-08-04 17:12:46.000000 openc3-5.9.2b0/openc3.egg-info/top_level.txt
+-rw-r--r--   0 ryanmelt   (501) staff       (20)       67 2023-08-04 17:12:46.399243 openc3-5.9.2b0/setup.cfg
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     3834 2023-08-04 17:06:36.000000 openc3-5.9.2b0/setup.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.395294 openc3-5.9.2b0/test/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/__init__.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.396639 openc3-5.9.2b0/test/accessors/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/accessors/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    42817 2023-08-04 03:14:31.000000 openc3-5.9.2b0/test/accessors/test_binary_accessor_read.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)   101175 2023-08-04 03:14:31.000000 openc3-5.9.2b0/test/accessors/test_binary_accessor_write.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.397925 openc3-5.9.2b0/test/api/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/api/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     6472 2023-08-02 22:48:03.000000 openc3-5.9.2b0/test/api/test_cmd_api.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2395 2023-08-02 22:48:03.000000 openc3-5.9.2b0/test/api/test_tlm_api.py
+drwxr-xr-x   0 ryanmelt   (501) staff       (20)        0 2023-08-04 17:12:46.398437 openc3-5.9.2b0/test/config/
+-rw-r--r--   0 ryanmelt   (501) staff       (20)        0 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/config/__init__.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)    22765 2023-07-31 15:36:25.000000 openc3-5.9.2b0/test/config/test_config_parser.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2654 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/test_authorization.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     1329 2023-07-27 22:17:09.000000 openc3-5.9.2b0/test/test_helper.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)      959 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_error.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2278 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_request.py
+-rw-r--r--   0 ryanmelt   (501) staff       (20)     2858 2023-08-01 16:42:30.000000 openc3-5.9.2b0/test/test_json_rpc_response.py
```

### Comparing `openc3-5.10.0/LICENSE.txt` & `openc3-5.9.2b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/PKG-INFO` & `openc3-5.9.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openc3
-Version: 5.10.0
+Version: 5.9.2b0
 Summary: Python Support for OpenC3 COSMOS v5
 Home-page: https://github.com/OpenC3/cosmos
 Author: Ryan Melton
 Author-email: ryan@openc3.com
 License: AGPLv3, Nonstandard
 Keywords: openc3 cosmos
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openc3-5.10.0/README.md` & `openc3-5.9.2b0/README.md`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/examples/cosmos_v5_enterprise_example.py` & `openc3-5.9.2b0/examples/cosmos_v5_enterprise_example.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/examples/cosmos_v5_example.py` & `openc3-5.9.2b0/examples/cosmos_v5_example.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/examples/cosmos_v5_stream_example.py` & `openc3-5.9.2b0/examples/cosmos_v5_stream_example.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/__version__.py` & `openc3-5.9.2b0/openc3/__version__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #
 # This file may also be used under the terms of a commercial license
 # if purchased from OpenC3, Inc.
 
 __title__ = "openc3"
 __description__ = "Python Support for OpenC3 COSMOS v5"
 __url__ = "https://github.com/OpenC3/cosmos"
-__version__ = "5.10.0"
+__version__ = "5.9.2-beta0"
```

### Comparing `openc3-5.10.0/openc3/accessors/accessor.py` & `openc3-5.9.2b0/openc3/accessors/accessor.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/accessors/binary_accessor.py` & `openc3-5.9.2b0/openc3/accessors/binary_accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1136,22 +1136,23 @@
     # @param data_type [Symbol] {DATA_TYPES}
     # @param overflow [Symbol] {OVERFLOW_TYPES}
     # @return [Array[Integer]] Potentially modified values
     @classmethod
     def check_overflow_array(
         cls, values, min_value, max_value, hex_max_value, bit_size, data_type, overflow
     ):
-        for index, value in enumerate(values):
-            values[index] = cls.check_overflow(
-                value,
-                min_value,
-                max_value,
-                hex_max_value,
-                bit_size,
-                data_type,
-                overflow,
-            )
+        if overflow != "TRUNCATE":
+            for index, value in enumerate(values):
+                values[index] = cls.check_overflow(
+                    value,
+                    min_value,
+                    max_value,
+                    hex_max_value,
+                    bit_size,
+                    data_type,
+                    overflow,
+                )
         return values
 
 
 # Store the host endianness so that it only has to be determined once
 BinaryAccessor.HOST_ENDIANNESS = BinaryAccessor.get_host_endianness()
```

### Comparing `openc3-5.10.0/openc3/api/__init__.py` & `openc3-5.9.2b0/openc3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/api/authorized_api.py` & `openc3-5.9.2b0/openc3/api/authorized_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/api/cmd_api.py` & `openc3-5.9.2b0/openc3/api/cmd_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/api/interface_api.py` & `openc3-5.9.2b0/openc3/api/interface_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/api/stash_api.py` & `openc3-5.9.2b0/openc3/api/stash_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/api/tlm_api.py` & `openc3-5.9.2b0/openc3/api/tlm_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/environment.py` & `openc3-5.9.2b0/openc3/environment.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/io/io_multiplexer.py` & `openc3-5.9.2b0/openc3/io/io_multiplexer.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/io/json_api_object.py` & `openc3-5.9.2b0/openc3/io/json_api_object.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/io/json_drb_object.py` & `openc3-5.9.2b0/openc3/io/json_drb_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from openc3.io.json_api_object import JsonApiObject, JsonApiError
 from .json_rpc import (
     JsonRpcRequest,
     JsonRpcResponse,
     JsonRpcSuccessResponse,
     JsonRpcErrorResponse,
 )
-from openc3.top_level import HazardousError  # noqa: F401
+from openc3.top_level import HazardousError  # Needed for error_class lookup
 
 
 class JsonDrbUnknownError(Exception):
     pass
 
 
 # The Ruby side implements from_hash directly on Exception but Python says:
@@ -41,15 +41,15 @@
     def from_hash(cls, hash):
         # Hash contains class, message, backtrace, and instance_variables
         error_class = None
         try:
             error_class = globals()[hash["class"]]
         except KeyError:
             error_class = RuntimeError
-            if "message" not in hash and "class" in hash:
+            if not "message" in hash and "class" in hash:
                 hash["message"] = hash["class"]
         error = None
         if error_class == RuntimeError and "message" in hash:
             error = error_class(hash["message"])
         else:
             error = error_class()
         if "instance_variables" in hash:
```

### Comparing `openc3-5.10.0/openc3/io/json_rpc.py` & `openc3-5.9.2b0/openc3/io/json_rpc.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/io/stderr.py` & `openc3-5.9.2b0/openc3/io/stderr.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/io/stdout.py` & `openc3-5.9.2b0/openc3/io/stdout.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/cvt_model.py` & `openc3-5.9.2b0/openc3/models/cvt_model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/interface_model.py` & `openc3-5.9.2b0/openc3/models/interface_model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/model.py` & `openc3-5.9.2b0/openc3/models/model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/reducer_model.py` & `openc3-5.9.2b0/openc3/models/reducer_model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/stash_model.py` & `openc3-5.9.2b0/openc3/models/stash_model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/models/target_model.py` & `openc3-5.9.2b0/openc3/models/target_model.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/packets/commands.py` & `openc3-5.9.2b0/openc3/packets/commands.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/packets/limits.py` & `openc3-5.9.2b0/openc3/packets/limits.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/packets/packet.py` & `openc3-5.9.2b0/openc3/packets/packet.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/packets/packet_config.py` & `openc3-5.9.2b0/openc3/packets/packet_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,57 +262,53 @@
     #         file.puts ""
 
     #  # def to_config
 
     # def to_xtce(output_dir)
     #   XtceConverter.convert(self.commands, self.telemetry, output_dir)
 
-    # Add current packet into hash if it exists
-    def finish_packet(self):
-        self.finish_item()
-        if self.current_packet:
-            self.warnings += self.current_packet.check_bit_offsets
-            if self.current_cmd_or_tlm == PacketConfig.COMMAND:
-                PacketParser.check_item_data_types(self.current_packet)
-                self.commands[self.current_packet.target_name][
-                    self.current_packet.packet_name
-                ] = self.current_packet
-                hash = self.cmd_id_value_hash[self.current_packet.target_name]
-                if not hash:
-                    hash = {}
-                self.cmd_id_value_hash[self.current_packet.target_name] = hash
-                self.update_id_value_hash(hash)
-            else:
-                self.telemetry[self.current_packet.target_name][
-                    self.current_packet.packet_name
-                ] = self.current_packet
-                hash = self.tlm_id_value_hash[self.current_packet.target_name]
-                if not hash:
-                    hash = {}
-                self.tlm_id_value_hash[self.current_packet.target_name] = hash
-                self.update_id_value_hash(hash)
-
-            self.current_packet = None
-            self.current_item = None
-
-    def update_id_value_hash(self, hash):
-        if self.current_packet.id_items.length > 0:
-            key = []
-            for item in self.current_packet.id_items:
-                key << item.id_value
-
-            hash[key] = self.current_packet
-        else:
-            hash["CATCHALL"] = self.current_packet
-
-    def reset_processing_variables(self):
-        self.current_cmd_or_tlm = None
-        self.current_packet = None
-        self.current_item = None
-        self.current_limits_group = None
+    # # Add current packet into hash if it exists
+    # def finish_packet
+    #   finish_item()
+    #   if self.current_packet
+    #     self.warnings += self.current_packet.check_bit_offsets
+    #     if self.current_cmd_or_tlm == COMMAND
+    #       PacketParser.check_item_data_types(self.current_packet)
+    #       self.commands[self.current_packet.target_name][self.current_packet.packet_name] = self.current_packet
+    #       hash = self.cmd_id_value_hash[self.current_packet.target_name]
+    #       hash = {} unless hash
+    #       self.cmd_id_value_hash[self.current_packet.target_name] = hash
+    #       update_id_value_hash(hash)
+    #     else
+    #       self.telemetry[self.current_packet.target_name][self.current_packet.packet_name] = self.current_packet
+    #       hash = self.tlm_id_value_hash[self.current_packet.target_name]
+    #       hash = {} unless hash
+    #       self.tlm_id_value_hash[self.current_packet.target_name] = hash
+    #       update_id_value_hash(hash)
+
+    #     self.current_packet = None
+    #     self.current_item = None
+
+    # protected
+
+    # def update_id_value_hash(hash)
+    #   if self.current_packet.id_items.length > 0
+    #     key = []
+    #     self.current_packet.id_items.each do |item|
+    #       key << item.id_value
+
+    #     hash[key] = self.current_packet
+    #   else
+    #     hash['CATCHALL'.freeze] = self.current_packet
+
+    # def reset_processing_variables
+    #   self.current_cmd_or_tlm = None
+    #   self.current_packet = None
+    #   self.current_item = None
+    #   self.current_limits_group = None
 
     # def process_current_packet(parser, keyword, params)
     #   case keyword
 
     #   # Select or delete an item in the current packet
     #   when 'SELECT_PARAMETER', 'SELECT_ITEM', 'DELETE_PARAMETER', 'DELETE_ITEM'
     #     if (self.current_cmd_or_tlm == COMMAND) && (keyword.split('_')[1] == 'ITEM')
@@ -572,23 +568,22 @@
     #     parser.verify_num_parameters(0, 0, 'OVERLAP')
     #     self.current_item.overlap = True
 
     #   when 'KEY'
     #     parser.verify_num_parameters(1, 1, 'KEY <key or path into data>')
     #     self.current_item.key = params[0]
 
-    # def start_item(self, parser):
-    #   self.finish_item()
+    # def start_item(parser)
+    #   finish_item()
     #   self.current_item = PacketItemParser.parse(parser, self.current_packet, self.current_cmd_or_tlm, self.warnings)
 
-    # Finish updating packet item
-    def finish_item(self):
-        if self.current_item:
-            self.current_packet.set_item(self.current_item)
-            if self.current_cmd_or_tlm == PacketConfig.TELEMETRY:
-                target_latest_data = self.latest_data[self.current_packet.target_name]
-                if not target_latest_data.get(self.current_item.name):
-                    target_latest_data[self.current_item.name] = []
-                latest_data_packets = target_latest_data[self.current_item.name]
-                if self.current_packet not in latest_data_packets:
-                    latest_data_packets.append(self.current_packet)
-            self.current_item = None
+    # # Finish updating packet item
+    # def finish_item
+    #   if self.current_item
+    #     self.current_packet.set_item(self.current_item)
+    #     if self.current_cmd_or_tlm == TELEMETRY
+    #       target_latest_data = self.latest_data[self.current_packet.target_name]
+    #       target_latest_data[self.current_item.name] ||= []
+    #       latest_data_packets = target_latest_data[self.current_item.name]
+    #       latest_data_packets << self.current_packet unless latest_data_packets.include?(self.current_packet)
+
+    #     self.current_item = None
```

### Comparing `openc3-5.10.0/openc3/packets/parsers/packet_parser.py` & `openc3-5.9.2b0/openc3/packets/parsers/packet_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 from openc3.packets.packet import Packet
 from openc3.utilities.logger import Logger
 
 
 class PacketParser:
     @classmethod
     def parse_command(cls, parser, target_name, commands, warnings):
-        parser = PacketParser(parser)
+        parser = PacketParser.new(parser)
         parser.verify_parameters()
         parser.create_command(target_name, commands, warnings)
 
     @classmethod
     def parse_telemetry(cls, parser, target_name, telemetry, latest_data, warnings):
-        parser = PacketParser(parser)
+        parser = PacketParser.new(parser)
         parser.verify_parameters()
         parser.create_telemetry(target_name, telemetry, latest_data, warnings)
 
     @classmethod
     def check_item_data_types(cls, packet):
         try:
             for item in packet.sorted_items:
```

### Comparing `openc3-5.10.0/openc3/packets/structure.py` & `openc3-5.9.2b0/openc3/packets/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,20 +518,21 @@
     def clone(self):
         return copy.deepcopy(self)
 
     # Enable the ability to read and write item values as if they were methods
     # to the class
     def __getattr__(self, func):
         # Prevent recursion in deepcopy
-        if func in ["__deepcopy__", "__getstate__", "__setstate__"]:
+        if func in ["__deepcopy__", "__setstate__"]:
             raise AttributeError()
-        if self.items.get(func.upper()):
-            return self.read(func.upper())
-        else:
-            raise AttributeError(f"Unknown item: {func}")
+
+        def method(*args, **kwargs):
+            return getattr(self, func)(*args, **kwargs)
+
+        return method
 
     # TODO:
     # def __setattr__(self, func, value):
     #     return setattr(self, func, value)
 
     MUTEX = threading.Lock()
```

### Comparing `openc3-5.10.0/openc3/packets/structure_item.py` & `openc3-5.9.2b0/openc3/packets/structure_item.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/packets/telemetry.py` & `openc3-5.9.2b0/openc3/packets/telemetry.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/__init__.py` & `openc3-5.9.2b0/openc3/script/__init__.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/api_shared.py` & `openc3-5.9.2b0/openc3/script/api_shared.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/authorization.py` & `openc3-5.9.2b0/openc3/script/authorization.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/commands.py` & `openc3-5.9.2b0/openc3/script/commands.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/cosmos_api.py` & `openc3-5.9.2b0/openc3/script/cosmos_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/decorators.py` & `openc3-5.9.2b0/openc3/script/decorators.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/exceptions.py` & `openc3-5.9.2b0/openc3/script/exceptions.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/internal_api.py` & `openc3-5.9.2b0/openc3/script/internal_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/limits.py` & `openc3-5.9.2b0/openc3/script/limits.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/metadata.py` & `openc3-5.9.2b0/openc3/script/metadata.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/screen.py` & `openc3-5.9.2b0/openc3/script/screen.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/server_proxy.py` & `openc3-5.9.2b0/openc3/script/server_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def generate_timeout(self):
         """pull openc3-cosmos-cmd-tlm-api timeout from environment variables"""
         return float(OPENC3_API_TIMEOUT)
 
     # generate the auth object
     def generate_auth(self):
-        if OPENC3_API_TOKEN is None and OPENC3_API_USER is None:
+        if OPENC3_API_TOKEN == None and OPENC3_API_USER == None:
             if OPENC3_API_PASSWORD or OPENC3_SERVICE_PASSWORD:
                 return OpenC3Authentication()
             else:
                 return None
         else:
             return OpenC3KeycloakAuthentication(OPENC3_KEYCLOAK_URL)
```

### Comparing `openc3-5.10.0/openc3/script/storage.py` & `openc3-5.9.2b0/openc3/script/storage.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/stream.py` & `openc3-5.9.2b0/openc3/script/stream.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/stream_shared.py` & `openc3-5.9.2b0/openc3/script/stream_shared.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/suite.py` & `openc3-5.9.2b0/openc3/script/suite.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/suite_results.py` & `openc3-5.9.2b0/openc3/script/suite_results.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/suite_runner.py` & `openc3-5.9.2b0/openc3/script/suite_runner.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/script/telemetry.py` & `openc3-5.9.2b0/openc3/script/telemetry.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/stream_api/base_client.py` & `openc3-5.9.2b0/openc3/stream_api/base_client.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/stream_api/data_extractor_client.py` & `openc3-5.9.2b0/openc3/stream_api/data_extractor_client.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/stream_api/log_message_client.py` & `openc3-5.9.2b0/openc3/stream_api/log_message_client.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/system/system.py` & `openc3-5.9.2b0/openc3/system/system.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/system/target.py` & `openc3-5.9.2b0/openc3/system/target.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/top_level.py` & `openc3-5.9.2b0/openc3/top_level.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/topics/command_decom_topic.py` & `openc3-5.9.2b0/openc3/topics/command_decom_topic.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/topics/command_topic.py` & `openc3-5.9.2b0/openc3/topics/command_topic.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/topics/decom_interface_topic.py` & `openc3-5.9.2b0/openc3/topics/decom_interface_topic.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/topics/interface_topic.py` & `openc3-5.9.2b0/openc3/topics/interface_topic.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/topics/topic.py` & `openc3-5.9.2b0/openc3/topics/topic.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/authentication.py` & `openc3-5.9.2b0/openc3/utilities/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         self.http = Session()
 
     # Load the token from the environment
     def token(self):
         with self.auth_mutex:
             self.log = [None, None]
             current_time = time.time()
-            if self._token is None:
+            if self._token == None:
                 self._make_token(current_time)
             elif self.refresh_expires_at < current_time:
                 self._make_token(current_time)
             elif self.expires_at < current_time:
                 self._refresh_token(current_time)
         return f"Bearer {self._token}"
 
@@ -101,15 +101,15 @@
             # Username and password
             data = f"username={OPENC3_API_USER}&password={OPENC3_API_PASSWORD}&client_id={client_id}&grant_type=password&scope=openid"
             headers = {
                 "Content-Type": "application/x-www-form-urlencoded",
                 "User-Agent": OPENC3_USER_AGENT,
             }
             oath = self._make_request(headers, data)
-            self._token = oath["access_token"]
+            self_token = oath["access_token"]
             self.refresh_token = oath["refresh_token"]
             self.expires_at = (
                 current_time + oath["expires_in"] - self.REFRESH_OFFSET_SECONDS
             )
             self.refresh_expires_at = (
                 current_time + oath["refresh_expires_in"] - self.REFRESH_OFFSET_SECONDS
             )
```

### Comparing `openc3-5.10.0/openc3/utilities/authorization.py` & `openc3-5.9.2b0/openc3/utilities/authorization.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/aws_bucket.py` & `openc3-5.9.2b0/openc3/utilities/aws_bucket.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/bucket.py` & `openc3-5.9.2b0/openc3/utilities/bucket.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/bucket_utilities.py` & `openc3-5.9.2b0/openc3/utilities/bucket_utilities.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/connection_pool.py` & `openc3-5.9.2b0/openc3/utilities/connection_pool.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/extract.py` & `openc3-5.9.2b0/openc3/utilities/extract.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/local_bucket.py` & `openc3-5.9.2b0/openc3/utilities/local_bucket.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/local_mode.py` & `openc3-5.9.2b0/openc3/utilities/local_mode.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/logger.py` & `openc3-5.9.2b0/openc3/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/message_log.py` & `openc3-5.9.2b0/openc3/utilities/message_log.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/script_shared.py` & `openc3-5.9.2b0/openc3/utilities/script_shared.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/sleeper.py` & `openc3-5.9.2b0/openc3/utilities/sleeper.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/store.py` & `openc3-5.9.2b0/openc3/utilities/store.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3/utilities/target_file.py` & `openc3-5.9.2b0/openc3/utilities/target_file.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/openc3.egg-info/PKG-INFO` & `openc3-5.9.2b0/openc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openc3
-Version: 5.10.0
+Version: 5.9.2b0
 Summary: Python Support for OpenC3 COSMOS v5
 Home-page: https://github.com/OpenC3/cosmos
 Author: Ryan Melton
 Author-email: ryan@openc3.com
 License: AGPLv3, Nonstandard
 Keywords: openc3 cosmos
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openc3-5.10.0/openc3.egg-info/SOURCES.txt` & `openc3-5.9.2b0/openc3.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -105,16 +105,8 @@
 test/accessors/__init__.py
 test/accessors/test_binary_accessor_read.py
 test/accessors/test_binary_accessor_write.py
 test/api/__init__.py
 test/api/test_cmd_api.py
 test/api/test_tlm_api.py
 test/config/__init__.py
-test/config/test_config_parser.py
-test/packets/__init__.py
-test/packets/test_structure.py
-test/packets/test_structure_item.py
-test/packets/parsers/__init__.py
-test/packets/parsers/test_packet_parser.py
-test/script/__init__.py
-test/script/test_api_shared.py
-test/script/test_telemetry.py
+test/config/test_config_parser.py
```

### Comparing `openc3-5.10.0/setup.py` & `openc3-5.9.2b0/setup.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/accessors/test_binary_accessor_read.py` & `openc3-5.9.2b0/test/accessors/test_binary_accessor_read.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/accessors/test_binary_accessor_write.py` & `openc3-5.9.2b0/test/accessors/test_binary_accessor_write.py`

 * *Files 7% similar despite different names*

```diff
@@ -2607,96 +2607,150 @@
 
     def test_truncates_block(self):
         BinaryAccessor.write_array(
             [b"abcde"], 0, 32, "BLOCK", 32, self.data, "BIG_ENDIAN", "TRUNCATE"
         )
         self.assertEqual(self.data[0:5], b"abcd\x00")
 
-    def test_truncates_ints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2 ** (bit_size - 1)
-            truncated_value = -value
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "TRUNCATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                truncated_value,
-            )
-
-    def test_truncates_uints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2**bit_size + 1
-            truncated_value = 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "TRUNCATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                truncated_value,
-            )
-
-    def test_saturates_ints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "INT"
-            value = 2 ** (bit_size - 1)
-            saturated_value = value - 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "SATURATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                saturated_value,
-            )
-
-    def test_saturates_uints(self):
-        for bit_size in [3, 5, 8, 16, 32, 64]:
-            data_type = "UINT"
-            value = 2**bit_size
-            saturated_value = value - 1
-            BinaryAccessor.write_array(
-                [value],
-                0,
-                bit_size,
-                data_type,
-                bit_size,
-                self.data,
-                "BIG_ENDIAN",
-                "SATURATE",
-            )
-            self.assertEqual(
-                BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
-                saturated_value,
-            )
+    # def test_truncates_ints(self):
+    #     for bit_size in [3, 5, 8, 16, 32, 64]:
+    #         data_type = "INT"
+    #         value = 2 ** (bit_size - 1)
+    #         truncated_value = -value
+    #         BinaryAccessor.write_array(
+    #             [value],
+    #             0,
+    #             bit_size,
+    #             data_type,
+    #             bit_size,
+    #             self.data,
+    #             "BIG_ENDIAN",
+    #             "TRUNCATE",
+    #         )
+    #         self.assertEqual(
+    #             BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
+    #             truncated_value,
+    #         )
+
+    # def test_truncates_8_bit_int(self):
+    #     bit_size = 8
+    #     data_type = "INT"
+    #     value = 2 ** (bit_size - 1)
+    #     truncated_value = -value
+    #     BinaryAccessor.write_array(
+    #         [value],
+    #         0,
+    #         bit_size,
+    #         data_type,
+    #         bit_size,
+    #         self.data,
+    #         "BIG_ENDIAN",
+    #         "TRUNCATE",
+    #     )
+    #     self.assertEqual(
+    #         BinaryAccessor.read(0, bit_size, data_type, self.data, "BIG_ENDIAN"),
+    #         truncated_value,
+    #     )
+
+    # def test_truncates_16_bit_int(self):
+    #       bit_size = 16; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+    # def test_truncates_32_bit_int(self):
+    #       bit_size = 32; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+    # def test_truncates_64_bit_int(self):
+    #       bit_size = 64; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+    #       BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+    #       self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+
+#     def test_truncates_3_bit_int(self):
+#           bit_size = 3; data_type = 'INT'; value = 2**(bit_size - 1); truncated_value = -value
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_8_bit_uint(self):
+#           bit_size = 8; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_16_bit_uint(self):
+#           bit_size = 16; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_32_bit_uint(self):
+#           bit_size = 32; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_64_bit_uint(self):
+#           bit_size = 64; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_truncates_3_bit_uint(self):
+#           bit_size = 3; data_type = 'UINT'; value = 2**bit_size + 1; truncated_value = 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'TRUNCATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), truncated_value)
+
+#     def test_saturates_8_bit_int(self):
+#           bit_size = 8; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_16_bit_int(self):
+#           bit_size = 16; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_32_bit_int(self):
+#           bit_size = 32; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_64_bit_int(self):
+#           bit_size = 64; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_3_bit_int(self):
+#           bit_size = 3; data_type = 'INT'; value = 2**(bit_size - 1); saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_8_bit_uint(self):
+#           bit_size = 8; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_16_bit_uint(self):
+#           bit_size = 16; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_32_bit_uint(self):
+#           bit_size = 32; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_64_bit_uint(self):
+#           bit_size = 64; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
+
+#     def test_saturates_3_bit_uint(self):
+#           bit_size = 3; data_type = 'UINT'; value = 2**bit_size; saturated_value = value - 1
+#           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'SATURATE')
+#           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), saturated_value)
 
-
-# TODO: Do we need these?
 #     def test_allows_hex_value_entry_of_8_bit_int(self):
 #           bit_size = 8; data_type = 'INT'; value = 2**bit_size - 1; allowed_value = -1
 #           BinaryAccessor.write_array([value], 0, bit_size, data_type, bit_size, self.data, 'BIG_ENDIAN', 'ERROR_ALLOW_HEX')
 #           self.assertEqual(BinaryAccessor.read(0, bit_size, data_type, self.data, 'BIG_ENDIAN'), allowed_value)
 
 #     def test_allows_hex_value_entry_of_16_bit_int(self):
 #           bit_size = 16; data_type = 'INT'; value = 2**bit_size - 1; allowed_value = -1
```

### Comparing `openc3-5.10.0/test/api/test_cmd_api.py` & `openc3-5.9.2b0/test/api/test_cmd_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/api/test_tlm_api.py` & `openc3-5.9.2b0/test/api/test_tlm_api.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/config/test_config_parser.py` & `openc3-5.9.2b0/test/config/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/test_authorization.py` & `openc3-5.9.2b0/test/test_authorization.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/test_helper.py` & `openc3-5.9.2b0/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/test_json_rpc_error.py` & `openc3-5.9.2b0/test/test_json_rpc_error.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/test_json_rpc_request.py` & `openc3-5.9.2b0/test/test_json_rpc_request.py`

 * *Files identical despite different names*

### Comparing `openc3-5.10.0/test/test_json_rpc_response.py` & `openc3-5.9.2b0/test/test_json_rpc_response.py`

 * *Files identical despite different names*

