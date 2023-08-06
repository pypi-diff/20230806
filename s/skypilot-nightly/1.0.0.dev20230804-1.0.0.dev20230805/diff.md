# Comparing `tmp/skypilot-nightly-1.0.0.dev20230804.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230805.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230804.tar", last modified: Fri Aug  4 10:40:26 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230805.tar", last modified: Sat Aug  5 10:40:33 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230804.tar` & `skypilot-nightly-1.0.0.dev20230805.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.210019 skypilot-nightly-1.0.0.dev20230804/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:40:26.210019 skypilot-nightly-1.0.0.dev20230804/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.182019 skypilot-nightly-1.0.0.dev20230804/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.182019 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   116682 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   207600 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   173874 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   110767 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46508 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.178019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   145911 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.094109 skypilot-nightly-1.0.0.dev20230805/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-05 10:40:33.094109 skypilot-nightly-1.0.0.dev20230805/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:40:33.094109 skypilot-nightly-1.0.0.dev20230805/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-05 10:40:25.000000 skypilot-nightly-1.0.0.dev20230805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.066108 skypilot-nightly-1.0.0.dev20230805/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-05 10:40:25.000000 skypilot-nightly-1.0.0.dev20230805/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.070108 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.070108 skypilot-nightly-1.0.0.dev20230805/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116682 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207983 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.070108 skypilot-nightly-1.0.0.dev20230805/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.070108 skypilot-nightly-1.0.0.dev20230805/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173874 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.070108 skypilot-nightly-1.0.0.dev20230805/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110767 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.074108 skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46508 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-05 10:40:25.000000 skypilot-nightly-1.0.0.dev20230805/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.062108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.078108 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.082109 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.086109 skypilot-nightly-1.0.0.dev20230805/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.090109 skypilot-nightly-1.0.0.dev20230805/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.090109 skypilot-nightly-1.0.0.dev20230805/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.090109 skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.090109 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 10:40:33.000000 skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:40:33.094109 skypilot-nightly-1.0.0.dev20230805/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145911 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-05 10:40:20.000000 skypilot-nightly-1.0.0.dev20230805/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/LICENSE` & `skypilot-nightly-1.0.0.dev20230805/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230805/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230805/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230804
+Version: 1.0.0.dev20230805
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230804
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230805
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/README.md` & `skypilot-nightly-1.0.0.dev20230805/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230805/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/setup.py` & `skypilot-nightly-1.0.0.dev20230805/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = 'ca2a092a1cc26d26fb49f94a11cfe5f369df0f25'
-__version__ = '1.0.0-dev20230804'
+__commit__ = 'e9be60a4e0ce0802ff356b696a649e0809a48711'
+__version__ = '1.0.0-dev20230805'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/kubernetes.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230805/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230805/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/cloud_vm_ray_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -2244,15 +2244,15 @@
             head_port = backend_utils.get_head_ssh_port(
                 self, use_cache=False, max_attempts=max_attempts)
             # TODO(romilb): Multinode doesn't work with Kubernetes yet.
             worker_ports = [22] * (self.launched_nodes - 1)
             ports = [head_port] + worker_ports
         else:
             # Use port 22 for other clouds
-            ports = [22] * self.launched_nodes
+            ports = [22] * self.num_node_ips
         self.stable_ssh_ports = ports
 
     def _update_stable_cluster_ips(self, max_attempts: int = 1) -> None:
         cluster_external_ips = backend_utils.get_node_ips(
             self.cluster_yaml,
             self.launched_nodes,
             handle=self,
@@ -2346,14 +2346,24 @@
     @property
     def head_ssh_port(self):
         external_ssh_ports = self.external_ssh_ports()
         if external_ssh_ports:
             return external_ssh_ports[0]
         return None
 
+    @property
+    def num_node_ips(self) -> int:
+        """Returns number of IPs of the cluster, correctly handling TPU Pod."""
+        is_tpu_vm_pod = tpu_utils.is_tpu_vm_pod(self.launched_resources)
+        if is_tpu_vm_pod:
+            num_ips = tpu_utils.get_num_tpu_devices(self.launched_resources)
+        else:
+            num_ips = self.launched_nodes
+        return num_ips
+
     def __setstate__(self, state):
         self._version = self._VERSION
 
         version = state.pop('_version', None)
         if version is None:
             version = -1
             state.pop('cluster_region', None)
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230805/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/check.py` & `skypilot-nightly-1.0.0.dev20230805/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230805/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230805/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/kubernetes.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230805/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/core.py` & `skypilot-nightly-1.0.0.dev20230805/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230805/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230805/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230805/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230805/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230805/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230805/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230805/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230805/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230805/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230805/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230805/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230805/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230805/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/task.py` & `skypilot-nightly-1.0.0.dev20230805/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/kubernetes-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230805/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230805/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230805/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/create_cluster.sh` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/delete_cluster.sh` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/generate_kind_config.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/tpu_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 def is_tpu_vm_pod(resources: Optional[resources_lib.Resources]) -> bool:
     if resources is None or not is_tpu_vm(resources):
         return False
     acc, _ = list(resources.accelerators.items())[0]
     return acc not in ['tpu-v2-8', 'tpu-v3-8', 'tpu-v4-8']
 
 
-def get_num_tpu_devices(
-        resources: Optional[resources_lib.Resources]) -> Optional[int]:
+def get_num_tpu_devices(resources: Optional[resources_lib.Resources]) -> int:
     if resources is None or not is_tpu(resources):
-        return None
+        raise ValueError('resources must be a valid TPU resource.')
     acc, _ = list(resources.accelerators.items())[0]
     num_tpu_devices = int(int(acc.split('-')[2]) / 8)
     return num_tpu_devices
 
 
 def check_gcp_cli_include_tpu_vm() -> None:
     # TPU VM API available with gcloud version >= 382.0.0
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230805/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230804
+Version: 1.0.0.dev20230805
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230804
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230805
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230805/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230804/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230805/tests/test_wheels.py`

 * *Files identical despite different names*

