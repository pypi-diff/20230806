# Comparing `tmp/syft-0.8.2b7.tar.gz` & `tmp/syft-0.8.2b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b7.tar", last modified: Sat Aug  5 12:23:10 2023, max compression
+gzip compressed data, was "syft-0.8.2b8.tar", last modified: Sun Aug  6 12:22:15 2023, max compression
```

## Comparing `syft-0.8.2b7.tar` & `syft-0.8.2b8.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/
--rw-r--r--   0 om        (1001) users      (100)    11843 2023-08-05 12:21:46.000000 syft-0.8.2b7/LICENSE
--rw-r--r--   0 om        (1001) users      (100)       98 2023-08-05 12:21:46.000000 syft-0.8.2b7/MANIFEST.in
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-05 12:23:10.118659 syft-0.8.2b7/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)    16170 2023-08-05 12:21:46.000000 syft-0.8.2b7/README.md
--rw-r--r--   0 om        (1001) users      (100)      272 2023-08-05 12:21:46.000000 syft-0.8.2b7/pyproject.toml
--rw-r--r--   0 om        (1001) users      (100)     3210 2023-08-05 12:23:10.118659 syft-0.8.2b7/setup.cfg
--rw-r--r--   0 om        (1001) users      (100)      107 2023-08-05 12:21:46.000000 syft-0.8.2b7/setup.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.098659 syft-0.8.2b7/src/
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/
--rw-r--r--   0 om        (1001) users      (100)      580 2023-08-05 12:21:49.000000 syft-0.8.2b7/src/syft/VERSION
--rw-r--r--   0 om        (1001) users      (100)     5750 2023-08-05 12:21:49.000000 syft-0.8.2b7/src/syft/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       93 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/__main__.py
--rw-r--r--   0 om        (1001) users      (100)      790 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/abstract_node.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/capnp/
--rw-r--r--   0 om        (1001) users      (100)      270 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/__init__.py
--rw-r--r--   0 om        (1001) users      (100)       75 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      102 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 om        (1001) users      (100)      186 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/client/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    27127 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/api.py
--rw-r--r--   0 om        (1001) users      (100)    28998 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/client.py
--rw-r--r--   0 om        (1001) users      (100)      568 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/connection.py
--rw-r--r--   0 om        (1001) users      (100)      650 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/deploy.py
--rw-r--r--   0 om        (1001) users      (100)     9925 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/domain_client.py
--rw-r--r--   0 om        (1001) users      (100)     7000 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/enclave_client.py
--rw-r--r--   0 om        (1001) users      (100)     6404 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/gateway_client.py
--rw-r--r--   0 om        (1001) users      (100)    15257 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/registry.py
--rw-r--r--   0 om        (1001) users      (100)     2623 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/search.py
--rw-r--r--   0 om        (1001) users      (100)      549 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/client/user_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft/external/
--rw-r--r--   0 om        (1001) users      (100)     1735 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/external/oblv/
--rw-r--r--   0 om        (1001) users      (100)      860 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      284 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/auth.py
--rw-r--r--   0 om        (1001) users      (100)      212 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/constants.py
--rw-r--r--   0 om        (1001) users      (100)     4835 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/deployment.py
--rw-r--r--   0 om        (1001) users      (100)    12380 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 om        (1001) users      (100)     1800 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 om        (1001) users      (100)      489 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 om        (1001) users      (100)     2280 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7462 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 om        (1001) users      (100)    13949 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 om        (1001) users      (100)     1146 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/gevent_patch.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/img/
--rw-r--r--   0 om        (1001) users      (100)      297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/base64.py
--rw-r--r--   0 om        (1001) users      (100)    25535 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/logo.png
--rw-r--r--   0 om        (1001) users      (100)    41764 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/node/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2631 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/credentials.py
--rw-r--r--   0 om        (1001) users      (100)      152 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/domain.py
--rw-r--r--   0 om        (1001) users      (100)      259 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/enclave.py
--rw-r--r--   0 om        (1001) users      (100)      819 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/gateway.py
--rw-r--r--   0 om        (1001) users      (100)    34306 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/node.py
--rw-r--r--   0 om        (1001) users      (100)     6960 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/routes.py
--rw-r--r--   0 om        (1001) users      (100)     2064 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/run.py
--rw-r--r--   0 om        (1001) users      (100)     7737 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/server.py
--rw-r--r--   0 om        (1001) users      (100)      127 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/worker.py
--rw-r--r--   0 om        (1001) users      (100)     1228 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/node/worker_settings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/serde/
--rw-r--r--   0 om        (1001) users      (100)      159 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3597 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/array.py
--rw-r--r--   0 om        (1001) users      (100)     4099 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/arrow.py
--rw-r--r--   0 om        (1001) users      (100)      298 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/capnp.py
--rw-r--r--   0 om        (1001) users      (100)      722 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/deserialize.py
--rw-r--r--   0 om        (1001) users      (100)     1230 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/lib_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    11663 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 om        (1001) users      (100)      875 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/mock.py
--rw-r--r--   0 om        (1001) users      (100)    11639 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/recursive.py
--rw-r--r--   0 om        (1001) users      (100)    11054 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 om        (1001) users      (100)     1822 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/serializable.py
--rw-r--r--   0 om        (1001) users      (100)      369 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/serialize.py
--rw-r--r--   0 om        (1001) users      (100)     4959 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/signature.py
--rw-r--r--   0 om        (1001) users      (100)     4885 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/serde/third_party.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.106659 syft-0.8.2b7/src/syft/service/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/action/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      703 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 om        (1001) users      (100)    16706 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_graph.py
--rw-r--r--   0 om        (1001) users      (100)     6874 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 om        (1001) users      (100)    49572 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_object.py
--rw-r--r--   0 om        (1001) users      (100)     2502 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_permissions.py
--rw-r--r--   0 om        (1001) users      (100)    27533 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_service.py
--rw-r--r--   0 om        (1001) users      (100)    10264 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_store.py
--rw-r--r--   0 om        (1001) users      (100)     1165 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/action_types.py
--rw-r--r--   0 om        (1001) users      (100)     3889 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/numpy.py
--rw-r--r--   0 om        (1001) users      (100)     2233 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/pandas.py
--rw-r--r--   0 om        (1001) users      (100)     2920 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/plan.py
--rw-r--r--   0 om        (1001) users      (100)     4951 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/action/verification.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/blob_storage/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     3437 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/service.py
--rw-r--r--   0 om        (1001) users      (100)      594 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/code/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      236 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/code_parse.py
--rw-r--r--   0 om        (1001) users      (100)      102 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/unparse.py
--rw-r--r--   0 om        (1001) users      (100)    30430 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code.py
--rw-r--r--   0 om        (1001) users      (100)     1756 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 om        (1001) users      (100)    12538 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_service.py
--rw-r--r--   0 om        (1001) users      (100)     1446 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code/user_code_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/code_history/
--rw-r--r--   0 om        (1001) users      (100)     4297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history.py
--rw-r--r--   0 om        (1001) users      (100)     8729 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 om        (1001) users      (100)     2348 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 om        (1001) users      (100)     1782 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/context.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/data_subject/
--rw-r--r--   0 om        (1001) users      (100)       69 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     4076 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 om        (1001) users      (100)      870 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 om        (1001) users      (100)     3215 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 om        (1001) users      (100)     5006 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/dataset/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    23590 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset.py
--rw-r--r--   0 om        (1001) users      (100)     6603 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 om        (1001) users      (100)     1911 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/enclave/
--rw-r--r--   0 om        (1001) users      (100)     6039 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/metadata/
--rw-r--r--   0 om        (1001) users      (100)     1170 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 om        (1001) users      (100)     3774 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/network/
--rw-r--r--   0 om        (1001) users      (100)    18260 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/network_service.py
--rw-r--r--   0 om        (1001) users      (100)     3100 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/node_peer.py
--rw-r--r--   0 om        (1001) users      (100)     4657 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/network/routes.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/notification/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     7961 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notification_service.py
--rw-r--r--   0 om        (1001) users      (100)     4566 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3259 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/policy/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    22636 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/policy.py
--rw-r--r--   0 om        (1001) users      (100)     2081 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/policy_service.py
--rw-r--r--   0 om        (1001) users      (100)     1077 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.110659 syft-0.8.2b7/src/syft/service/project/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    47645 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project.py
--rw-r--r--   0 om        (1001) users      (100)    15374 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project_service.py
--rw-r--r--   0 om        (1001) users      (100)     1908 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/queue/
--rw-r--r--   0 om        (1001) users      (100)     2038 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/base_queue.py
--rw-r--r--   0 om        (1001) users      (100)     3006 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/queue.py
--rw-r--r--   0 om        (1001) users      (100)     4845 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 om        (1001) users      (100)     7754 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/request/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/__init__.py
--rw-r--r--   0 om        (1001) users      (100)    29652 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request.py
--rw-r--r--   0 om        (1001) users      (100)    10135 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request_service.py
--rw-r--r--   0 om        (1001) users      (100)     1410 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/request/request_stash.py
--rw-r--r--   0 om        (1001) users      (100)     3125 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/response.py
--rw-r--r--   0 om        (1001) users      (100)    13815 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/service.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/settings/
--rw-r--r--   0 om        (1001) users      (100)     1109 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings.py
--rw-r--r--   0 om        (1001) users      (100)     3608 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings_service.py
--rw-r--r--   0 om        (1001) users      (100)     1711 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/user/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      201 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/roles.py
--rw-r--r--   0 om        (1001) users      (100)     9666 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user.py
--rw-r--r--   0 om        (1001) users      (100)     3427 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_roles.py
--rw-r--r--   0 om        (1001) users      (100)    17595 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_service.py
--rw-r--r--   0 om        (1001) users      (100)     4510 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/service/vpn/
--rw-r--r--   0 om        (1001) users      (100)     1830 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     6789 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 om        (1001) users      (100)     5414 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/vpn/vpn.py
--rw-r--r--   0 om        (1001) users      (100)     5171 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/service/warnings.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/store/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/__init__.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/store/blob_storage/
--rw-r--r--   0 om        (1001) users      (100)     3961 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 om        (1001) users      (100)     2790 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 om        (1001) users      (100)     1036 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 om        (1001) users      (100)     3235 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/dict_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    23280 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/document_store.py
--rw-r--r--   0 om        (1001) users      (100)    22188 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/kv_document_store.py
--rw-r--r--   0 om        (1001) users      (100)     4326 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/linked_obj.py
--rw-r--r--   0 om        (1001) users      (100)    11840 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/locks.py
--rw-r--r--   0 om        (1001) users      (100)     8768 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_client.py
--rw-r--r--   0 om        (1001) users      (100)      846 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_codecs.py
--rw-r--r--   0 om        (1001) users      (100)    14031 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/mongo_document_store.py
--rw-r--r--   0 om        (1001) users      (100)    13136 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.114659 syft-0.8.2b7/src/syft/types/
--rw-r--r--   0 om        (1001) users      (100)        0 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      136 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/base.py
--rw-r--r--   0 om        (1001) users      (100)     2151 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/blob_storage.py
--rw-r--r--   0 om        (1001) users      (100)     1091 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/datetime.py
--rw-r--r--   0 om        (1001) users      (100)     5167 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/grid_url.py
--rw-r--r--   0 om        (1001) users      (100)      919 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/identity.py
--rw-r--r--   0 om        (1001) users      (100)     4807 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/syft_metaclass.py
--rw-r--r--   0 om        (1001) users      (100)    25449 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/syft_object.py
--rw-r--r--   0 om        (1001) users      (100)     8113 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/transforms.py
--rw-r--r--   0 om        (1001) users      (100)     2098 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/twin_object.py
--rw-r--r--   0 om        (1001) users      (100)     8038 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/types/uid.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/src/syft/util/
--rw-r--r--   0 om        (1001) users      (100)       67 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/__init__.py
--rw-r--r--   0 om        (1001) users      (100)      852 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/autoreload.py
--rw-r--r--   0 om        (1001) users      (100)      271 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/colors.py
--rw-r--r--   0 om        (1001) users      (100)       34 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/constants.py
--rw-r--r--   0 om        (1001) users      (100)     1514 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/decorators.py
--rw-r--r--   0 om        (1001) users      (100)      445 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/env.py
--rw-r--r--   0 om        (1001) users      (100)     1607 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/experimental_flags.py
--rw-r--r--   0 om        (1001) users      (100)     1327 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/filterwarnings.py
--rw-r--r--   0 om        (1001) users      (100)     2940 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/fonts.py
--rw-r--r--   0 om        (1001) users      (100)      153 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/jax_settings.py
--rw-r--r--   0 om        (1001) users      (100)     3779 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/logger.py
--rw-r--r--   0 om        (1001) users      (100)      752 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/markdown.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.118659 syft-0.8.2b7/src/syft/util/notebook_ui/
--rw-r--r--   0 om        (1001) users      (100)    27090 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 om        (1001) users      (100)       42 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/options.py
--rw-r--r--   0 om        (1001) users      (100)     5297 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/schema.py
--rw-r--r--   0 om        (1001) users      (100)     2771 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/telemetry.py
--rw-r--r--   0 om        (1001) users      (100)     6728 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/trace_decorator.py
--rw-r--r--   0 om        (1001) users      (100)    23185 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/util.py
--rw-r--r--   0 om        (1001) users      (100)     3123 2023-08-05 12:21:46.000000 syft-0.8.2b7/src/syft/util/version_compare.py
-drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-05 12:23:10.102659 syft-0.8.2b7/src/syft.egg-info/
--rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 om        (1001) users      (100)     6427 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 om        (1001) users      (100)       43 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 om        (1001) users      (100)        1 2023-08-05 12:23:09.000000 syft-0.8.2b7/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 om        (1001) users      (100)     1555 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/requires.txt
--rw-r--r--   0 om        (1001) users      (100)        5 2023-08-05 12:23:10.000000 syft-0.8.2b7/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.771318 syft-0.8.2b8/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-08-06 12:20:45.000000 syft-0.8.2b8/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-08-06 12:20:45.000000 syft-0.8.2b8/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-06 12:22:15.771318 syft-0.8.2b8/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-08-06 12:20:45.000000 syft-0.8.2b8/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-08-06 12:20:45.000000 syft-0.8.2b8/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-08-06 12:22:15.771318 syft-0.8.2b8/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-08-06 12:20:45.000000 syft-0.8.2b8/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.743318 syft-0.8.2b8/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.747318 syft-0.8.2b8/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-08-06 12:20:48.000000 syft-0.8.2b8/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5750 2023-08-06 12:20:48.000000 syft-0.8.2b8/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      790 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    27127 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    28998 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     9925 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     7000 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6404 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12380 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13949 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.755318 syft-0.8.2b8/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      819 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    34306 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6960 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     7737 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1228 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.755318 syft-0.8.2b8/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    11054 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.755318 syft-0.8.2b8/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.759318 syft-0.8.2b8/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    49572 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2502 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    27533 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.759318 syft-0.8.2b8/src/syft/service/blob_storage/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3437 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 om        (1001) users      (100)      594 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.759318 syft-0.8.2b8/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    30430 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    12538 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code/user_code_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.759318 syft-0.8.2b8/src/syft/service/code_history/
+-rw-r--r--   0 om        (1001) users      (100)     4297 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 om        (1001) users      (100)     8729 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 om        (1001) users      (100)     2348 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.759318 syft-0.8.2b8/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23590 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6603 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6039 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     1170 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3774 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    18260 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     3100 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4657 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22636 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    47645 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2038 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3006 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7754 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    29652 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10135 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3125 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13815 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.763318 syft-0.8.2b8/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)     1109 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3608 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.767318 syft-0.8.2b8/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     9666 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    17595 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4510 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.767318 syft-0.8.2b8/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1830 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/vpn/vpn.py
+-rw-r--r--   0 om        (1001) users      (100)     5171 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/service/warnings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.767318 syft-0.8.2b8/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.767318 syft-0.8.2b8/src/syft/store/blob_storage/
+-rw-r--r--   0 om        (1001) users      (100)     3961 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2790 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 om        (1001) users      (100)     1036 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    23280 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22188 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    14031 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.767318 syft-0.8.2b8/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     2151 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/blob_storage.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)      919 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/identity.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25449 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.771318 syft-0.8.2b8/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)      445 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/env.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.771318 syft-0.8.2b8/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    23185 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-08-06 12:20:45.000000 syft-0.8.2b8/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-08-06 12:22:15.751318 syft-0.8.2b8/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     6427 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-08-06 12:22:15.000000 syft-0.8.2b8/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b7/LICENSE` & `syft-0.8.2b8/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/PKG-INFO` & `syft-0.8.2b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b7
+Version: 0.8.2b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b7 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b8 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b7/README.md` & `syft-0.8.2b8/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/setup.cfg` & `syft-0.8.2b8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.7"
+version = attr: "0.8.2-beta.8"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.2b7/src/syft/VERSION` & `syft-0.8.2b8/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.7"
+__version__ = "0.8.2-beta.8"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b7/src/syft/__init__.py` & `syft-0.8.2b8/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2-beta.7"
+__version__ = "0.8.2-beta.8"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.2b7/src/syft/abstract_node.py` & `syft-0.8.2b8/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/api.py` & `syft-0.8.2b8/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/client.py` & `syft-0.8.2b8/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/connection.py` & `syft-0.8.2b8/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/deploy.py` & `syft-0.8.2b8/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/domain_client.py` & `syft-0.8.2b8/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/enclave_client.py` & `syft-0.8.2b8/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/gateway_client.py` & `syft-0.8.2b8/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/registry.py` & `syft-0.8.2b8/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/search.py` & `syft-0.8.2b8/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/client/user_settings.py` & `syft-0.8.2b8/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/__init__.py` & `syft-0.8.2b8/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/__init__.py` & `syft-0.8.2b8/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/deployment.py` & `syft-0.8.2b8/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b8/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b8/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b8/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b8/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b8/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/gevent_patch.py` & `syft-0.8.2b8/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/img/logo.png` & `syft-0.8.2b8/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b8/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/credentials.py` & `syft-0.8.2b8/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/gateway.py` & `syft-0.8.2b8/src/syft/node/gateway.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/node.py` & `syft-0.8.2b8/src/syft/node/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/routes.py` & `syft-0.8.2b8/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/run.py` & `syft-0.8.2b8/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/server.py` & `syft-0.8.2b8/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/node/worker_settings.py` & `syft-0.8.2b8/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/array.py` & `syft-0.8.2b8/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/arrow.py` & `syft-0.8.2b8/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/deserialize.py` & `syft-0.8.2b8/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/lib_permissions.py` & `syft-0.8.2b8/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b8/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/mock.py` & `syft-0.8.2b8/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/recursive.py` & `syft-0.8.2b8/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b8/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/serializable.py` & `syft-0.8.2b8/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/signature.py` & `syft-0.8.2b8/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/serde/third_party.py` & `syft-0.8.2b8/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b8/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_graph.py` & `syft-0.8.2b8/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b8/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_object.py` & `syft-0.8.2b8/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_permissions.py` & `syft-0.8.2b8/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_service.py` & `syft-0.8.2b8/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_store.py` & `syft-0.8.2b8/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/action_types.py` & `syft-0.8.2b8/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/numpy.py` & `syft-0.8.2b8/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/pandas.py` & `syft-0.8.2b8/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/plan.py` & `syft-0.8.2b8/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/action/verification.py` & `syft-0.8.2b8/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/blob_storage/service.py` & `syft-0.8.2b8/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/blob_storage/stash.py` & `syft-0.8.2b8/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code/user_code.py` & `syft-0.8.2b8/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b8/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code/user_code_service.py` & `syft-0.8.2b8/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b8/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code_history/code_history.py` & `syft-0.8.2b8/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code_history/code_history_service.py` & `syft-0.8.2b8/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.2b8/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/context.py` & `syft-0.8.2b8/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b8/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b8/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b8/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b8/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/dataset/dataset.py` & `syft-0.8.2b8/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b8/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b8/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/enclave/enclave_service.py` & `syft-0.8.2b8/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/metadata/metadata_service.py` & `syft-0.8.2b8/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b8/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/network/network_service.py` & `syft-0.8.2b8/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/network/node_peer.py` & `syft-0.8.2b8/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/network/routes.py` & `syft-0.8.2b8/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/notification/notification_service.py` & `syft-0.8.2b8/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/notification/notification_stash.py` & `syft-0.8.2b8/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/notification/notifications.py` & `syft-0.8.2b8/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/policy/policy.py` & `syft-0.8.2b8/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/policy/policy_service.py` & `syft-0.8.2b8/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b8/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/project/project.py` & `syft-0.8.2b8/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/project/project_service.py` & `syft-0.8.2b8/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/project/project_stash.py` & `syft-0.8.2b8/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/queue/base_queue.py` & `syft-0.8.2b8/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/queue/queue.py` & `syft-0.8.2b8/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b8/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b8/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/request/request.py` & `syft-0.8.2b8/src/syft/service/request/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/request/request_service.py` & `syft-0.8.2b8/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/request/request_stash.py` & `syft-0.8.2b8/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/response.py` & `syft-0.8.2b8/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/service.py` & `syft-0.8.2b8/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/settings/settings.py` & `syft-0.8.2b8/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/settings/settings_service.py` & `syft-0.8.2b8/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b8/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/user/user.py` & `syft-0.8.2b8/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/user/user_roles.py` & `syft-0.8.2b8/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/user/user_service.py` & `syft-0.8.2b8/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/user/user_stash.py` & `syft-0.8.2b8/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b8/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b8/src/syft/service/vpn/tailscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/vpn/vpn.py` & `syft-0.8.2b8/src/syft/service/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/service/warnings.py` & `syft-0.8.2b8/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/blob_storage/__init__.py` & `syft-0.8.2b8/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.2b8/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.2b8/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/dict_document_store.py` & `syft-0.8.2b8/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/document_store.py` & `syft-0.8.2b8/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/kv_document_store.py` & `syft-0.8.2b8/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/linked_obj.py` & `syft-0.8.2b8/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/locks.py` & `syft-0.8.2b8/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/mongo_client.py` & `syft-0.8.2b8/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/mongo_codecs.py` & `syft-0.8.2b8/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/mongo_document_store.py` & `syft-0.8.2b8/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b8/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/blob_storage.py` & `syft-0.8.2b8/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/datetime.py` & `syft-0.8.2b8/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/grid_url.py` & `syft-0.8.2b8/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/identity.py` & `syft-0.8.2b8/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/syft_metaclass.py` & `syft-0.8.2b8/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/syft_object.py` & `syft-0.8.2b8/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/transforms.py` & `syft-0.8.2b8/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/twin_object.py` & `syft-0.8.2b8/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/types/uid.py` & `syft-0.8.2b8/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/autoreload.py` & `syft-0.8.2b8/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/decorators.py` & `syft-0.8.2b8/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/experimental_flags.py` & `syft-0.8.2b8/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/filterwarnings.py` & `syft-0.8.2b8/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/fonts.py` & `syft-0.8.2b8/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/logger.py` & `syft-0.8.2b8/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/markdown.py` & `syft-0.8.2b8/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b8/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/schema.py` & `syft-0.8.2b8/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/telemetry.py` & `syft-0.8.2b8/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/trace_decorator.py` & `syft-0.8.2b8/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/util.py` & `syft-0.8.2b8/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft/util/version_compare.py` & `syft-0.8.2b8/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b8/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b7
+Version: 0.8.2b8
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b7 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b8 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b7/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b8/src/syft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b7/src/syft.egg-info/requires.txt` & `syft-0.8.2b8/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

