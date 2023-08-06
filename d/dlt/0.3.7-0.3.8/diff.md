# Comparing `tmp/dlt-0.3.7.tar.gz` & `tmp/dlt-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.7.tar", max compression
+gzip compressed data, was "dlt-0.3.8.tar", max compression
```

## Comparing `dlt-0.3.7.tar` & `dlt-0.3.8.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.7/LICENSE.txt
--rw-r--r--   0        0        0     4196 2023-07-21 12:57:39.118978 dlt-0.3.7/README.md
--rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17134 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15153 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2023-07-27 11:13:48.179808 dlt-0.3.7/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    19741 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9939 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2523 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2308 2023-07-20 14:41:03.294283 dlt-0.3.7/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.7/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.7/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20347 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-07-23 19:50:04.055755 dlt-0.3.7/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-07-21 12:45:34.138978 dlt-0.3.7/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6559 2023-07-20 23:10:47.941211 dlt-0.3.7/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.7/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6498 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     8427 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-21 12:58:04.898978 dlt-0.3.7/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    13629 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.7/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19564 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5032 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7234 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2798 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25586 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-07-29 11:30:56.572443 dlt-0.3.7/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23933 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     2321 2023-07-27 11:13:48.189808 dlt-0.3.7/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-07-20 16:42:01.694283 dlt-0.3.7/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     2129 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    14652 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0     2019 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     2302 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     4238 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6386 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.7/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     5105 2023-07-21 12:58:04.898978 dlt-0.3.7/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4759 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2935 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     5618 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1390 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     4772 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    19938 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.7/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     2246 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/motherduck/__init__.py
--rw-r--r--   0        0        0     2070 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/motherduck/configuration.py
--rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/motherduck/motherduck.py
--rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/motherduck/sql_client.py
--rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     2305 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     4188 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     5484 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     2230 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      894 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     8521 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     2241 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/snowflake/__init__.py
--rw-r--r--   0        0        0     4347 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/destinations/snowflake/configuration.py
--rw-r--r--   0        0        0     9851 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/snowflake/snowflake.py
--rw-r--r--   0        0        0     6820 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/snowflake/sql_client.py
--rw-r--r--   0        0        0     8198 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    12350 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.7/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.7/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     9379 2023-07-29 11:30:56.572443 dlt-0.3.7/dlt/extract/extract.py
--rw-r--r--   0        0        0    19337 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35424 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.7/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13867 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13214 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/load/exceptions.py
--rw-r--r--   0        0        0    24642 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.7/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.7/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    17202 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13834 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.7/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8753 2023-07-21 12:58:04.908978 dlt-0.3.7/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    65295 2023-07-30 20:32:44.418673 dlt-0.3.7/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     9132 2023-07-20 14:41:03.304283 dlt-0.3.7/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5060 2023-07-26 18:57:08.058358 dlt-0.3.7/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.7/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.7/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.7/dlt/version.py
--rw-r--r--   0        0        0     4479 2023-07-31 14:14:22.284085 dlt-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 dlt-0.3.7/setup.py
--rw-r--r--   0        0        0     7840 1970-01-01 00:00:00.000000 dlt-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.8/LICENSE.txt
+-rw-r--r--   0        0        0     4366 2023-08-04 07:54:12.881323 dlt-0.3.8/README.md
+-rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17134 2023-08-05 22:22:32.541127 dlt-0.3.8/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15365 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    15902 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1944 2023-07-27 11:13:48.179808 dlt-0.3.8/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    19741 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9939 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     2523 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/cli/requirements.py
+-rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2017 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.8/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.8/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20347 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.8/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2897 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-07-23 19:50:04.055755 dlt-0.3.8/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.8/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2403 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12537 2023-08-03 19:14:51.872550 dlt-0.3.8/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6559 2023-07-20 23:10:47.941211 dlt-0.3.8/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6898 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6498 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8427 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-21 12:58:04.898978 dlt-0.3.8/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    13629 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.8/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.8/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.8/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-08-06 15:28:48.364333 dlt-0.3.8/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19564 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5032 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7234 2023-07-20 14:41:03.304283 dlt-0.3.8/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2798 2023-07-20 14:41:03.304283 dlt-0.3.8/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25586 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-07-29 11:30:56.572443 dlt-0.3.8/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    24174 2023-08-04 07:54:12.881323 dlt-0.3.8/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     2321 2023-07-27 11:13:48.189808 dlt-0.3.8/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-07-20 16:42:01.694283 dlt-0.3.8/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     4332 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/common/time.py
+-rw-r--r--   0        0        0     5740 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/utils.py
+-rw-r--r--   0        0        0     4838 2023-08-04 07:54:12.881323 dlt-0.3.8/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     2129 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    14652 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0     2019 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10825 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     2302 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4238 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6481 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.8/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     5105 2023-07-21 12:58:04.898978 dlt-0.3.8/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4759 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2935 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     5327 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1390 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     4772 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    19938 2023-08-04 23:06:59.024754 dlt-0.3.8/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.8/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     2246 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/motherduck/__init__.py
+-rw-r--r--   0        0        0     2070 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/motherduck/configuration.py
+-rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/motherduck/sql_client.py
+-rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     2305 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     4188 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     5484 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     2230 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     8521 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     2241 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4347 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0     9851 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     6820 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     8198 2023-08-04 23:07:16.464754 dlt-0.3.8/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    12350 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.8/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.8/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     9379 2023-07-29 11:30:56.572443 dlt-0.3.8/dlt/extract/extract.py
+-rw-r--r--   0        0        0    26389 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35424 2023-07-20 14:41:03.304283 dlt-0.3.8/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9774 2023-08-04 07:54:12.881323 dlt-0.3.8/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/extract/typing.py
+-rw-r--r--   0        0        0      583 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.8/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    14291 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13214 2023-07-20 14:41:03.304283 dlt-0.3.8/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    24690 2023-08-06 17:53:38.412451 dlt-0.3.8/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.8/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.8/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    17202 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13834 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.8/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8753 2023-07-21 12:58:04.908978 dlt-0.3.8/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    65295 2023-07-30 20:32:44.418673 dlt-0.3.8/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     9132 2023-07-20 14:41:03.304283 dlt-0.3.8/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5060 2023-07-26 18:57:08.058358 dlt-0.3.8/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.8/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.8/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.8/dlt/version.py
+-rw-r--r--   0        0        0     4513 2023-08-06 17:53:38.422451 dlt-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 dlt-0.3.8/setup.py
+-rw-r--r--   0        0        0     8010 1970-01-01 00:00:00.000000 dlt-0.3.8/PKG-INFO
```

### Comparing `dlt-0.3.7/LICENSE.txt` & `dlt-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/README.md` & `dlt-0.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 <h1 align="center">
     <strong>data load tool (dlt) — the open-source Python library for data loading</strong>
 </h1>
 <p align="center">
 Be it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.
 </p>
 
+
+<h3 align="center">
+
+🚀 Join our thriving community of likeminded developers and build the future together!
+
+</h3>
+
 <div align="center">
   <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">
-    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />
+    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" style="width: 260px;"  />
   </a>
+</div>
+<div align="center">
   <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
     <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">
   </a>
   <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
     <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">
   </a>
 </div>
```

### Comparing `dlt-0.3.7/dlt/__init__.py` & `dlt-0.3.8/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/_dlt.py` & `dlt-0.3.8/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/config_toml_writer.py` & `dlt-0.3.8/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/deploy_command.py` & `dlt-0.3.8/dlt/cli/deploy_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,40 +193,45 @@
             self.repo_storage.create_folder(utils.AIRFLOW_DAGS_FOLDER)
 
         if not self.repo_storage.has_folder(utils.AIRFLOW_BUILD_FOLDER):
             self.repo_storage.create_folder(utils.AIRFLOW_BUILD_FOLDER)
 
         # save cloudbuild.yaml only if not exist to allow to run the deploy command for many different pipelines
         dest_cloud_build = os.path.join(utils.AIRFLOW_BUILD_FOLDER, AIRFLOW_CLOUDBUILD_YAML)
-        if not os.path.exists(dest_cloud_build):
+        if not self.repo_storage.has_file(dest_cloud_build):
             self.repo_storage.save(
                 dest_cloud_build,
                 self.artifacts["cloudbuild_file"]
-        )
+            )
+        else:
+            fmt.warning(f"{AIRFLOW_CLOUDBUILD_YAML} already created. Delete the file and run the deploy command again to re-create.")
+
+        dest_dag_script = os.path.join(utils.AIRFLOW_DAGS_FOLDER, self.artifacts["dag_script_name"])
         self.repo_storage.save(
-            os.path.join(utils.AIRFLOW_DAGS_FOLDER, self.artifacts["dag_script_name"]),
+            dest_dag_script,
             self.artifacts["dag_file"]
         )
 
+
     def _echo_instructions(self, *args: Optional[Any]) -> None:
         fmt.echo("Your %s deployment for pipeline %s is ready!" % (
             fmt.bold(self.deployment_method), fmt.bold(self.state["pipeline_name"]),
         ))
         fmt.echo("* The airflow %s file was created in %s." % (
             fmt.bold(AIRFLOW_CLOUDBUILD_YAML), fmt.bold(utils.AIRFLOW_BUILD_FOLDER)
         ))
         fmt.echo("* The %s script was created in %s." % (
             fmt.bold(self.artifacts["dag_script_name"]), fmt.bold(utils.AIRFLOW_DAGS_FOLDER)
         ))
         fmt.echo()
 
-        fmt.echo("You must prepare your repository first:")
+        fmt.echo("You must prepare your DAG first:")
 
-        fmt.echo("1. Import your sources in %s, change default_args if necessary." % (fmt.bold(self.artifacts["dag_script_name"])))
-        fmt.echo("2. Run airflow pipeline locally.\nSee Airflow getting started: %s" % (fmt.bold(AIRFLOW_GETTING_STARTED)))
+        fmt.echo("1. Import your sources in %s, configure the DAG ans tasks as needed." % (fmt.bold(self.artifacts["dag_script_name"])))
+        fmt.echo("2. Test the DAG with Airflow locally .\nSee Airflow getting started: %s" % (fmt.bold(AIRFLOW_GETTING_STARTED)))
         fmt.echo()
 
         fmt.echo("If you are planning run the pipeline with Google Cloud Composer, follow the next instructions:\n")
         fmt.echo("1. Read this doc and set up the Environment: %s" % (
             fmt.bold(DLT_AIRFLOW_GCP_DOCS_URL)
         ))
         fmt.echo("2. Set _BUCKET_NAME up in %s/%s file. " % (
```

### Comparing `dlt-0.3.7/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.8/dlt/cli/deploy_command_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from itertools import chain
 from typing import List, Optional, Sequence, Tuple, Any, Dict
 from astunparse import unparse
 import cron_descriptor
 
 import dlt
 
+from dlt.common import git
 from dlt.common.configuration.exceptions import LookupTrace
 from dlt.common.configuration.providers import ConfigTomlProvider, EnvironProvider
 from dlt.common.git import get_origin, get_repo, Repo
 from dlt.common.configuration.specs.run_configuration import get_default_pipeline_name
 from dlt.common.typing import StrAny
 from dlt.common.reflection.utils import evaluate_node_literal
-from dlt.common.pipeline import LoadInfo, TPipelineState
+from dlt.common.pipeline import LoadInfo, TPipelineState, get_dlt_repos_dir
 from dlt.common.storages import FileStorage
 from dlt.common.utils import set_working_dir
 
 from dlt.pipeline.pipeline import Pipeline
 from dlt.pipeline.trace import PipelineTrace
 from dlt.reflection import names as n
 from dlt.reflection.script_visitor import PipelineScriptVisitor
@@ -80,15 +81,15 @@
         # convert to path relative to repo
         self.repo_pipeline_script_path = self.repo_storage.from_wd_to_relative_path(self.pipeline_script_path)
         # load a pipeline script and extract full_refresh and pipelines_dir args
         self.pipeline_script = self.repo_storage.load(self.repo_pipeline_script_path)
         # validate schedule
         self.schedule_description = self._get_schedule_description()
         fmt.echo("Looking up the deployment template scripts in %s...\n" % fmt.bold(self.repo_location))
-        self.template_storage = utils.clone_command_repo(self.repo_location, self.branch)
+        self.template_storage = git.get_fresh_repo_files(self.repo_location, get_dlt_repos_dir(), branch=self.branch)
         self.working_directory = os.path.split(self.pipeline_script_path)[0]
 
     def _get_schedule_description(self) -> Optional[Any]:
         return None if self.schedule is None else cron_descriptor.get_description(self.schedule)
 
     def _get_origin(self) -> str:
         try:
@@ -102,29 +103,42 @@
 
     def run_deployment(self) -> None:
         with get_repo(self.pipeline_script_path) as repo:
             self.repo = repo
             self._prepare_deployment()
             # go through all once launched pipelines
             visitors = get_visitors(self.pipeline_script, self.pipeline_script_path)
-            pipeline_name, pipelines_dir = parse_pipeline_info(visitors)
+            possible_pipelines = parse_pipeline_info(visitors)
+            pipeline_name: str = None
+            pipelines_dir: str = None
+
+            uniq_possible_pipelines = {t[0]:t for t in possible_pipelines}
+            if len(uniq_possible_pipelines) == 1:
+                pipeline_name, pipelines_dir = possible_pipelines[0]
+            elif len(uniq_possible_pipelines) > 1:
+                choices = list(uniq_possible_pipelines.keys())
+                choices_str = "".join([str(i+1) for i in range(len(choices))])
+                choices_selection = [f"{idx+1}-{name}" for idx, name in enumerate(choices)]
+                sel = fmt.prompt("Several pipelines found in script, please select one: " + ", ".join(choices_selection), choices=choices_str)
+                pipeline_name, pipelines_dir = uniq_possible_pipelines[choices[int(sel) - 1]]
 
             if pipelines_dir:
                 self.pipelines_dir = os.path.abspath(pipelines_dir)
             if pipeline_name:
                 self.pipeline_name = pipeline_name
 
             # change the working dir to the script working dir
             with set_working_dir(self.working_directory):
                 # use script name to derive pipeline name
                 if not self.pipeline_name:
                     self.pipeline_name = dlt.config.get("pipeline_name")
                     if not self.pipeline_name:
                         self.pipeline_name = get_default_pipeline_name(self.pipeline_script_path)
                         fmt.warning(f"Using default pipeline name {self.pipeline_name}. The pipeline name is not passed as argument to dlt.pipeline nor configured via config provides ie. config.toml")
+                # fmt.echo("Generating deployment for pipeline %s" % fmt.bold(self.pipeline_name))
 
                 # attach to pipeline name, get state and trace
                 pipeline = dlt.attach(pipeline_name=self.pipeline_name, pipelines_dir=self.pipelines_dir)
                 self.state, trace = get_state_and_trace(pipeline)
                 self._update_envs(trace)
 
             self._generate_workflow()
@@ -195,40 +209,42 @@
 def get_visitors(pipeline_script: str, pipeline_script_path: str) -> PipelineScriptVisitor:
     visitor = utils.parse_init_script("deploy", pipeline_script, pipeline_script_path)
     if n.RUN not in visitor.known_calls:
         raise CliCommandException("deploy", f"The pipeline script {pipeline_script_path} does not seem to run the pipeline.")
     return visitor
 
 
-def parse_pipeline_info(visitor: PipelineScriptVisitor) -> Tuple[Optional[str], Optional[str]]:
-    pipeline_name, pipelines_dir = None, None
+def parse_pipeline_info(visitor: PipelineScriptVisitor) -> List[Tuple[str, Optional[str]]]:
+    pipelines: List[Tuple[str, Optional[str]]] = []
     if n.PIPELINE in visitor.known_calls:
         for call_args in visitor.known_calls[n.PIPELINE]:
+            pipeline_name, pipelines_dir = None, None
             f_r_node = call_args.arguments.get("full_refresh")
             if f_r_node:
                 f_r_value = evaluate_node_literal(f_r_node)
                 if f_r_value is None:
                     fmt.warning(f"The value of `full_refresh` in call to `dlt.pipeline` cannot be determined from {unparse(f_r_node).strip()}. We assume that you know what you are doing :)")
                 if f_r_value is True:
                     if fmt.confirm("The value of 'full_refresh' is set to True. Do you want to abort to set it to False?", default=True):
-                        return None, None
+                        return pipelines
 
             p_d_node = call_args.arguments.get("pipelines_dir")
             if p_d_node:
                 pipelines_dir = evaluate_node_literal(p_d_node)
                 if pipelines_dir is None:
                     raise CliCommandException("deploy", f"The value of 'pipelines_dir' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipelines-dir option.")
 
             p_n_node = call_args.arguments.get("pipeline_name")
             if p_n_node:
                 pipeline_name = evaluate_node_literal(p_n_node)
                 if pipeline_name is None:
                     raise CliCommandException("deploy", f"The value of 'pipeline_name' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipeline-name option.")
+            pipelines.append((pipeline_name, pipelines_dir))
 
-    return pipeline_name, pipelines_dir
+    return pipelines
 
 
 def str_representer(dumper: yaml.Dumper, data: str) -> yaml.ScalarNode:
     # format multiline strings as blocks with the exception of placeholders
     # that will be expanded as yaml
     if len(data.splitlines()) > 1 and "{{ toYaml" not in data:  # check for multiline string
         return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
```

### Comparing `dlt-0.3.7/dlt/cli/echo.py` & `dlt-0.3.8/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/init_command.py` & `dlt-0.3.8/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/pipeline_command.py` & `dlt-0.3.8/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/pipeline_files.py` & `dlt-0.3.8/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/requirements.py` & `dlt-0.3.8/dlt/cli/requirements.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/source_detection.py` & `dlt-0.3.8/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/telemetry_command.py` & `dlt-0.3.8/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/cli/utils.py` & `dlt-0.3.8/dlt/cli/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,21 +21,14 @@
 GITHUB_WORKFLOWS_DIR = os.path.join(".github", "workflows")
 AIRFLOW_DAGS_FOLDER = os.path.join("dags")
 AIRFLOW_BUILD_FOLDER = os.path.join("build")
 LOCAL_COMMAND_REPO_FOLDER = "repos"
 MODULE_INIT = "__init__.py"
 
 
-def clone_command_repo(repo_location: str, branch: str) -> FileStorage:
-    template_dir = tempfile.mkdtemp()
-    # TODO: handle ImportError (no git command available) gracefully
-    with git.clone_repo(repo_location, template_dir, branch=branch):
-        return FileStorage(template_dir)
-
-
 def parse_init_script(command: str, script_source: str, init_script_name: str) -> PipelineScriptVisitor:
     # parse the script first
     tree = ast.parse(source=script_source)
     set_ast_parents(tree)
     visitor = PipelineScriptVisitor(script_source)
     visitor.visit_passes(tree)
     if len(visitor.mod_aliases) == 0:
```

### Comparing `dlt-0.3.7/dlt/common/arithmetics.py` & `dlt-0.3.8/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/accessors.py` & `dlt-0.3.8/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/container.py` & `dlt-0.3.8/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/exceptions.py` & `dlt-0.3.8/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/inject.py` & `dlt-0.3.8/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/paths.py` & `dlt-0.3.8/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.8/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/context.py` & `dlt-0.3.8/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.8/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/environ.py` & `dlt-0.3.8/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.8/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/provider.py` & `dlt-0.3.8/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/providers/toml.py` & `dlt-0.3.8/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/resolve.py` & `dlt-0.3.8/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.8/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.8/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.8/dlt/common/configuration/specs/aws_credentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,76 @@
-from typing import Optional, TYPE_CHECKING, Dict, Any
+from typing import Optional, Dict, Any
 
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import TSecretStrValue
 from dlt.common.configuration.specs import CredentialsConfiguration, CredentialsWithDefault, configspec
+from dlt.common.configuration.specs.exceptions import InvalidBoto3Session
 from dlt import version
 
 
 @configspec
 class AwsCredentialsWithoutDefaults(CredentialsConfiguration):
     # credentials without boto implementation
     aws_access_key_id: str = None
     aws_secret_access_key: TSecretStrValue = None
     aws_session_token: Optional[TSecretStrValue] = None
-    aws_profile: Optional[str] = None
+    profile_name: Optional[str] = None
+    region_name: Optional[str] = None
 
     def to_s3fs_credentials(self) -> Dict[str, Optional[str]]:
         """Dict of keyword arguments that can be passed to s3fs"""
         return dict(
             key=self.aws_access_key_id,
             secret=self.aws_secret_access_key,
             token=self.aws_session_token,
-            profile=self.aws_profile
+            profile=self.profile_name
         )
 
     def to_native_representation(self) -> Dict[str, Optional[str]]:
         """Return a dict that can be passed as kwargs to boto3 session"""
-        d = dict(self)
-        d['profile_name'] = d.pop('aws_profile')  # boto3 argument doesn't match env var name
-        return d
+        return dict(self)
 
 
 @configspec
 class AwsCredentials(AwsCredentialsWithoutDefaults, CredentialsWithDefault):
 
     def on_partial(self) -> None:
         # Try get default credentials
         session = self._to_session()
-        self.aws_profile = session.profile_name
-        default = session.get_credentials()
-        if not default:
-            return None
-        self.aws_access_key_id = default.access_key
-        self.aws_secret_access_key = default.secret_key
-        self.aws_session_token = default.token
-        if not self.is_partial():
+        if self._from_session(session) and not self.is_partial():
             self.resolve()
 
     def _to_session(self) -> Any:
         try:
             import boto3
         except ImportError:
             raise MissingDependencyException(self.__class__.__name__, [f"{version.DLT_PKG_NAME}[s3]"])
         return boto3.Session(**self.to_native_representation())
 
+    def _from_session(self, session: Any) -> Any:
+        """Sets the credentials properties from boto3 `session` and return session's credentials if found"""
+        import boto3
+        assert isinstance(session, boto3.Session)
+        self.profile_name = session.profile_name
+        self.region_name = session.region_name
+        default = session.get_credentials()
+        if not default:
+            return None
+        self.aws_access_key_id = default.access_key
+        self.aws_secret_access_key = default.secret_key
+        self.aws_session_token = default.token
+        return default
+
     def to_native_credentials(self) -> Optional[Any]:
         return self._to_session().get_credentials()
+
+    def parse_native_representation(self, native_value: Any) -> None:
+        """Import external boto session"""
+        try:
+            import boto3
+            if isinstance(native_value, boto3.Session):
+                if self._from_session(native_value):
+                    self.__is_resolved__ = True
+            else:
+                raise InvalidBoto3Session(self.__class__, native_value)
+        except ImportError:
+            pass
```

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.8/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.8/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.8/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.8/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.8/dlt/common/configuration/specs/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,7 +38,13 @@
         super().__init__(spec, native_value, msg)
 
 
 class InvalidGoogleOauth2Json(NativeValueError):
     def __init__(self, spec: Type[Any], native_value: Any):
         msg = f"The expected representation for {spec.__name__} is a string with serialized oauth2 user info and may be wrapped in 'install'/'web' node - depending of oauth2 app type."
         super().__init__(spec, native_value, msg)
+
+
+class InvalidBoto3Session(NativeValueError):
+    def __init__(self, spec: Type[Any], native_value: Any):
+        msg = f"The expected representation for {spec.__name__} is and instance of boto3.Session containing credentials"
+        super().__init__(spec, native_value, msg)
```

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.8/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.8/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.8/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/configuration/utils.py` & `dlt-0.3.8/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/data_types/type_helpers.py` & `dlt-0.3.8/dlt/common/data_types/type_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import binascii
 import base64
 import datetime  # noqa: I251
 from collections.abc import Mapping as C_Mapping, Sequence as C_Sequence
-from typing import Any, Type, Literal, Union, Optional, cast
+from typing import Any, Type, Literal, Union, cast
 
 from dlt.common import pendulum, json, Decimal, Wei
 from dlt.common.json import custom_pua_remove
 from dlt.common.json._simplejson import custom_encode as json_custom_encode
 from dlt.common.arithmetics import InvalidOperation
 from dlt.common.data_types.typing import TDataType
-from dlt.common.time import parse_iso_like_datetime, ensure_datetime, ensure_date
+from dlt.common.time import ensure_pendulum_datetime, parse_iso_like_datetime, ensure_pendulum_date
 from dlt.common.utils import map_nested_in_place, str2bool
 
 
 def py_type_to_sc_type(t: Type[Any]) -> TDataType:
     # start with most popular types
     if t is str:
         return "text"
@@ -53,15 +53,15 @@
     raise TypeError(t)
 
 
 def complex_to_str(value: Any) -> str:
     return json.dumps(map_nested_in_place(custom_pua_remove, value))
 
 
-def coerce_date_types(
+def coerce_to_date_types(
     to_type: Literal["timestamp", "date"], from_type: TDataType, value: Any
 ) -> Union[datetime.datetime, datetime.date]:
     result: Union[datetime.datetime, datetime.date]
     try:
         if from_type in ["bigint", "double"]:
             # returns ISO datetime with timezone
             result = pendulum.from_timestamp(value)
@@ -85,16 +85,33 @@
         # id that is not possible OverflowError is raised and text cannot be represented as datetime
         raise ValueError(value)
     except Exception:
         # catch all problems in pendulum
         raise ValueError(value)
     # Pendulum ISO parsing may result in either datetime or date
     if to_type == "date":
-        return ensure_date(result)
-    return ensure_datetime(result)
+        return ensure_pendulum_date(result)
+    return ensure_pendulum_datetime(result)
+
+
+def coerce_from_date_types(
+    to_type: TDataType, value: datetime.datetime
+) -> Union[datetime.datetime, datetime.date, int, float, str]:
+    v = ensure_pendulum_datetime(value)
+    if to_type == "timestamp":
+        return v
+    if to_type == "text":
+        return v.isoformat()
+    if to_type == "bigint":
+        return v.int_timestamp  # type: ignore
+    if to_type == "double":
+        return v.timestamp()  # type: ignore
+    if to_type == "date":
+        return ensure_pendulum_date(v)
+    raise TypeError(f"Cannot convert timestamp to {to_type}")
 
 
 def coerce_value(to_type: TDataType, from_type: TDataType, value: Any) -> Any:
     if to_type == from_type:
         if to_type == "complex":
             # complex types need custom encoding to be removed
             return map_nested_in_place(custom_pua_remove, value)
@@ -161,15 +178,15 @@
             else:
                 try:
                     return decimal_cls(trim_value)
                 except InvalidOperation:
                     raise ValueError(trim_value)
 
     if to_type in ["timestamp", "date"]:
-        return coerce_date_types(cast(Literal["timestamp", "date"], to_type), from_type, value)
+        return coerce_to_date_types(cast(Literal["timestamp", "date"], to_type), from_type, value)
 
     if to_type == "bool":
         if from_type == "text":
             return str2bool(value)
         if from_type not in ["complex", "binary", "timestamp"]:
             # all the numeric types will convert to bool on 0 - False, 1 - True
             return bool(value)
```

### Comparing `dlt-0.3.7/dlt/common/data_writers/buffered.py` & `dlt-0.3.8/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/data_writers/escape.py` & `dlt-0.3.8/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/data_writers/exceptions.py` & `dlt-0.3.8/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/data_writers/writers.py` & `dlt-0.3.8/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/destination/capabilities.py` & `dlt-0.3.8/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/destination/reference.py` & `dlt-0.3.8/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/exceptions.py` & `dlt-0.3.8/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/git.py` & `dlt-0.3.8/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/json/__init__.py` & `dlt-0.3.8/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/json/_orjson.py` & `dlt-0.3.8/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/json/_simplejson.py` & `dlt-0.3.8/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/jsonpath.py` & `dlt-0.3.8/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/libs/pyarrow.py` & `dlt-0.3.8/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/configuration.py` & `dlt-0.3.8/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.8/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/json/relational.py` & `dlt-0.3.8/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.8/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.8/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.8/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.8/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.8/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/normalizers/utils.py` & `dlt-0.3.8/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/pipeline.py` & `dlt-0.3.8/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/reflection/spec.py` & `dlt-0.3.8/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/reflection/utils.py` & `dlt-0.3.8/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/configuration.py` & `dlt-0.3.8/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/pool_runner.py` & `dlt-0.3.8/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/runnable.py` & `dlt-0.3.8/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/stdout.py` & `dlt-0.3.8/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/synth_pickle.py` & `dlt-0.3.8/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runners/venv.py` & `dlt-0.3.8/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/collector.py` & `dlt-0.3.8/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/exec_info.py` & `dlt-0.3.8/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/init.py` & `dlt-0.3.8/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/logger.py` & `dlt-0.3.8/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/prometheus.py` & `dlt-0.3.8/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/segment.py` & `dlt-0.3.8/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/sentry.py` & `dlt-0.3.8/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/signals.py` & `dlt-0.3.8/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/slack.py` & `dlt-0.3.8/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/runtime/telemetry.py` & `dlt-0.3.8/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/schema/detections.py` & `dlt-0.3.8/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/schema/exceptions.py` & `dlt-0.3.8/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/schema/schema.py` & `dlt-0.3.8/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/schema/typing.py` & `dlt-0.3.8/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/schema/utils.py` & `dlt-0.3.8/dlt/common/schema/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from dlt.common import json
 from dlt.common.data_types import TDataType
 from dlt.common.exceptions import DictValidationException
 from dlt.common.normalizers import default_normalizers
 from dlt.common.normalizers.naming import NamingConvention
 from dlt.common.typing import DictStrAny, REPattern
-from dlt.common.validation import TCustomValidator, validate_dict
+from dlt.common.validation import TCustomValidator, validate_dict, validate_dict_ignoring_xkeys
 from dlt.common.schema import detections
 from dlt.common.schema.typing import (SCHEMA_ENGINE_VERSION, LOADS_TABLE_NAME, SIMPLE_REGEX_PREFIX, VERSION_TABLE_NAME, TColumnName, TPartialTableSchema, TSchemaTables, TSchemaUpdate,
                                       TSimpleRegex, TStoredSchema, TTableSchema, TTableSchemaColumns, TColumnSchemaBase, TColumnSchema, TColumnProp,
                                       TColumnHint, TTypeDetectionFunc, TTypeDetections, TWriteDisposition)
 from dlt.common.schema.exceptions import CannotCoerceColumnException, ParentTableNotFoundException, SchemaEngineNoUpgradePathException, SchemaException, TablePropertiesConflictException
 
 # RE_LEADING_DIGITS = re.compile(r"^\d+")
@@ -164,15 +164,20 @@
     if not pattern:  # Don't create an empty pattern that matches everything
         raise ValueError("Cannot create a regex pattern from empty sequence")
     return re.compile(pattern)
 
 
 def validate_stored_schema(stored_schema: TStoredSchema) -> None:
     # use lambda to verify only non extra fields
-    validate_dict(TStoredSchema, stored_schema, ".", lambda k: not k.startswith("x-"), simple_regex_validator)
+    validate_dict_ignoring_xkeys(
+        spec=TStoredSchema,
+        doc=stored_schema,
+        path=".",
+        validator_f=simple_regex_validator
+    )
     # check child parent relationships
     for table_name, table in stored_schema["tables"].items():
         parent_table_name = table.get("parent")
         if parent_table_name:
             if parent_table_name not in stored_schema["tables"]:
                 raise ParentTableNotFoundException(table_name, parent_table_name)
 
@@ -560,27 +565,37 @@
         assert write_disposition is None
         assert resource is None
     else:
         # set write disposition only for root tables
         table["write_disposition"] = write_disposition or DEFAULT_WRITE_DISPOSITION
         table["resource"] = resource or table_name
     if validate_schema:
-        validate_dict(TTableSchema, table, f"new_table/{table_name}")
+        validate_dict_ignoring_xkeys(
+            spec=TColumnSchema,
+            doc=table["columns"],
+            path=f"new_table/{table_name}",
+        )
+
     return table
 
 
 def new_column(column_name: str, data_type: TDataType = None, nullable: bool = True, validate_schema: bool = False) -> TColumnSchema:
     column = add_missing_hints({
                 "name": column_name,
                 "nullable": nullable
             })
     if data_type:
         column["data_type"] = data_type
     if validate_schema:
-        validate_dict(TColumnSchema, column, f"new_column/{column_name}")
+        validate_dict_ignoring_xkeys(
+            spec=TColumnSchema,
+            doc=column,
+            path=f"new_column/{column_name}",
+        )
+
     return column
 
 
 def standard_hints() -> Dict[TColumnHint, List[TSimpleRegex]]:
     return None
```

### Comparing `dlt-0.3.7/dlt/common/source.py` & `dlt-0.3.8/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/__init__.py` & `dlt-0.3.8/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/configuration.py` & `dlt-0.3.8/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/data_item_storage.py` & `dlt-0.3.8/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/exceptions.py` & `dlt-0.3.8/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/file_storage.py` & `dlt-0.3.8/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.8/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/load_storage.py` & `dlt-0.3.8/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/normalize_storage.py` & `dlt-0.3.8/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/schema_storage.py` & `dlt-0.3.8/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/transactional_file.py` & `dlt-0.3.8/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/storages/versioned_storage.py` & `dlt-0.3.8/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/typing.py` & `dlt-0.3.8/dlt/common/typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from collections.abc import Mapping as C_Mapping, Sequence as C_Sequence
+from datetime import datetime, date  # noqa: I251
 import inspect
 from re import Pattern as _REPattern
-from typing import Callable, Dict, Any, Final, Literal, List, Mapping, NewType, Tuple, Type, TypeVar, Generic, Protocol, TYPE_CHECKING, Union, runtime_checkable, get_args, get_origin
+from typing import Callable, Dict, Any, Final, Literal, List, Mapping, NewType, Optional, Tuple, Type, TypeVar, Generic, Protocol, TYPE_CHECKING, Union, runtime_checkable, get_args, get_origin
 from typing_extensions import TypeAlias, ParamSpec, Concatenate
 
-from dlt.common.pendulum import timedelta
+from dlt.common.pendulum import timedelta, pendulum
+
+
 
 
 if TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
     # from typing_extensions import ParamSpec
     from typing import _TypedDict
     REPattern = _REPattern[str]
@@ -31,14 +34,15 @@
 TAnyClass = TypeVar("TAnyClass", bound=object)
 TimedeltaSeconds = Union[int, float, timedelta]
 # represent secret value ie. coming from Kubernetes/Docker secrets or other providers
 TSecretValue = NewType("TSecretValue", Any)  # type: ignore
 TSecretStrValue = NewType("TSecretValue", str)  # type: ignore
 TDataItem: TypeAlias = Any  # a single data item as extracted from data source
 TDataItems: TypeAlias = Union[TDataItem, List[TDataItem]]  # a single or many data items as extracted from the data source
+TAnyDateTime = Union[pendulum.DateTime, pendulum.Date, datetime, date, str]
 
 ConfigValue: None = None  # a value of type None indicating argument that may be injected by config provider
 
 TVariantBase = TypeVar("TVariantBase", covariant=True)
 TVariantRV = Tuple[str, Any]
 VARIANT_FIELD_FORMAT = "v_%s"
 
@@ -125,7 +129,27 @@
         # descend into supertypes of NewType
         return extract_inner_type(hint.__supertype__, preserve_new_types)
     return hint
 
 
 def get_all_types_of_class_in_union(hint: Type[Any], cls: Type[TAny]) -> List[Type[TAny]]:
     return [t for t in get_args(hint) if inspect.isclass(t) and issubclass(t, cls)]
+
+
+def get_generic_type_argument_from_instance(instance: Any, sample_value: Optional[Any]) -> Type[Any]:
+    """Infers type argument of a Generic class from an `instance` of that class using optional `sample_value` of the argument type
+
+    Inference depends on the presence of __orig_class__ attribute in instance, if not present - sample_Value will be used
+
+    Args:
+        instance (Any): instance of Generic class
+        sample_value (Optional[Any]): instance of type of generic class, optional
+
+    Returns:
+        Type[Any]: type argument or Any if not known
+    """
+    orig_param_type = Any
+    if hasattr(instance, "__orig_class__"):
+        orig_param_type = get_args(instance.__orig_class__)[0]
+    if orig_param_type is Any and sample_value is not None:
+        orig_param_type = type(sample_value)
+    return orig_param_type  # type: ignore
```

### Comparing `dlt-0.3.7/dlt/common/utils.py` & `dlt-0.3.8/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/common/validation.py` & `dlt-0.3.8/dlt/common/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,39 @@
+import functools
 from typing import Callable, Any, Type, get_type_hints, get_args
 
 from dlt.common.exceptions import DictValidationException
 from dlt.common.typing import StrAny, extract_optional_type, is_literal_type, is_optional_type, is_typeddict, is_list_generic_type, is_dict_generic_type, _TypedDict
 
 
 TFilterFunc = Callable[[str], bool]
 TCustomValidator = Callable[[str, str, Any, Any], bool]
 
 
 def validate_dict(spec: Type[_TypedDict], doc: StrAny, path: str, filter_f: TFilterFunc = None, validator_f: TCustomValidator = None) -> None:
+    """Validate the `doc` dictionary based on the given typed dictionary specification `spec`.
+
+    Args:
+        spec (Type[_TypedDict]): The typed dictionary that `doc` should conform to.
+        doc (StrAny): The dictionary to validate.
+        path (str): The string representing the location of the dictionary
+            in a hierarchical data structure.
+        filter_f (TFilterFunc, optional): A function to filter keys in `doc`. It should
+            return `True` for keys to be kept. Defaults to a function that keeps all keys.
+        validator_f (TCustomValidator, optional): A function to perform additional validation
+            for types not covered by this function. It should return `True` if the validation passes.
+            Defaults to a function that rejects all such types.
+
+    Raises:
+        DictValidationException: If there are missing required fields, unexpected fields,
+            type mismatches or unvalidated types in `doc` compared to `spec`.
+
+    Returns:
+        None
+    """
     # pass through filter
     filter_f = filter_f or (lambda _: True)
     # cannot validate anything
     validator_f = validator_f or (lambda p, pk, pv, t: False)
 
     allowed_props = get_type_hints(spec)
     required_props = {k: v for k, v in allowed_props.items() if not is_optional_type(v)}
@@ -63,8 +84,14 @@
             pass
         else:
             if not validator_f(path, pk, pv, t):
                 raise DictValidationException(f"In {path}: field {pk} has expected type {t.__name__} which lacks validator", path, pk)
 
     # check allowed props
     for pk, pv in props.items():
-        verify_prop(pk, pv, allowed_props[pk])
+        verify_prop(pk, pv, allowed_props[pk])
+
+
+validate_dict_ignoring_xkeys = functools.partial(
+    validate_dict,
+    filter_f=lambda k: not k.startswith("x-")
+)
```

### Comparing `dlt-0.3.7/dlt/common/wei.py` & `dlt-0.3.8/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.8/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.8/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/bigquery/configuration.py` & `dlt-0.3.8/dlt/destinations/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.8/dlt/destinations/bigquery/sql_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,14 +222,18 @@
                     return DatabaseTerminalException(ex)
                 elif isinstance(ex, dbapi_exceptions.ProgrammingError):
                     return DatabaseTransientException(ex)
             if reason == "notFound":
                 return DatabaseUndefinedRelation(ex)
             if reason == "invalidQuery" and "was not found" in str(ex) and "Dataset" in str(ex):
                 return DatabaseUndefinedRelation(ex)
+            if reason == "invalidQuery" and "Not found" in str(ex) and ("Dataset" in str(ex) or "Table" in str(ex)):
+                return DatabaseUndefinedRelation(ex)
+            if reason == "accessDenied" and "Dataset" in str(ex) and "not exist" in str(ex):
+                return DatabaseUndefinedRelation(ex)
             if reason == "invalidQuery" and ("Unrecognized name" in str(ex) or "cannot be null" in str(ex)):
                 # unknown column, inserting NULL into required field
                 return DatabaseTerminalException(ex)
             if reason in BQ_TERMINAL_REASONS:
                 return DatabaseTerminalException(ex)
             # anything else is transient
             return DatabaseTransientException(ex)
```

### Comparing `dlt-0.3.7/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.8/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.8/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/duckdb/duck.py` & `dlt-0.3.8/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.8/dlt/destinations/duckdb/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,16 @@
         return self.capabilities.escape_identifier(self.dataset_name) if escape else self.dataset_name
 
     @classmethod
     def _make_database_exception(cls, ex: Exception) -> Exception:
         if isinstance(ex, (duckdb.CatalogException)):
             raise DatabaseUndefinedRelation(ex)
         elif isinstance(ex, duckdb.InvalidInputException):
+            if "Catalog Error" in str(ex):
+                raise DatabaseUndefinedRelation(ex)
             # duckdb raises TypeError on malformed query parameters
             return DatabaseTransientException(duckdb.ProgrammingError(ex))
         elif isinstance(ex, (duckdb.OperationalError, duckdb.InternalError, duckdb.SyntaxException, duckdb.ParserException)):
             term = cls._maybe_make_terminal_exception_from_data_error(ex)
             if term:
                 return term
             else:
```

### Comparing `dlt-0.3.7/dlt/destinations/dummy/__init__.py` & `dlt-0.3.8/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/dummy/configuration.py` & `dlt-0.3.8/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/dummy/dummy.py` & `dlt-0.3.8/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/exceptions.py` & `dlt-0.3.8/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.8/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.8/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.8/dlt/destinations/filesystem/filesystem.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 class LoadFilesystemJob(LoadJob):
     def __init__(
             self,
             local_path: str,
             dataset_path: str,
             *,
             config: FilesystemClientConfiguration,
-            write_disposition: TWriteDisposition,
-            has_merge_keys: bool,
             schema_name: str,
             load_id: str
     ) -> None:
         file_name = FileStorage.get_file_name_from_file_path(local_path)
         self.config = config
         self.dataset_path = dataset_path
         self.destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
@@ -97,21 +95,18 @@
         self.fs_client.makedirs(self.dataset_path, exist_ok=True)
 
     def is_storage_initialized(self) -> bool:
         return self.fs_client.isdir(self.dataset_path)  # type: ignore[no-any-return]
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         cls = FollowupFilesystemJob if self.config.as_staging else LoadFilesystemJob
-        has_merge_keys = any(col['merge_key'] or col['primary_key'] for col in table['columns'].values())
         return cls(
             file_path,
             self.dataset_path,
             config=self.config,
-            write_disposition=table['write_disposition'],
-            has_merge_keys=has_merge_keys,
             schema_name=self.schema.name,
             load_id=load_id
         )
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
```

### Comparing `dlt-0.3.7/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.8/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/insert_job_client.py` & `dlt-0.3.8/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/job_client_impl.py` & `dlt-0.3.8/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/job_impl.py` & `dlt-0.3.8/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/motherduck/__init__.py` & `dlt-0.3.8/dlt/destinations/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/motherduck/configuration.py` & `dlt-0.3.8/dlt/destinations/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/motherduck/motherduck.py` & `dlt-0.3.8/dlt/destinations/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/motherduck/sql_client.py` & `dlt-0.3.8/dlt/destinations/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/postgres/__init__.py` & `dlt-0.3.8/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/postgres/configuration.py` & `dlt-0.3.8/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/postgres/postgres.py` & `dlt-0.3.8/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.8/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/redshift/README.md` & `dlt-0.3.8/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/redshift/__init__.py` & `dlt-0.3.8/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/redshift/configuration.py` & `dlt-0.3.8/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/redshift/redshift.py` & `dlt-0.3.8/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/snowflake/__init__.py` & `dlt-0.3.8/dlt/destinations/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/snowflake/configuration.py` & `dlt-0.3.8/dlt/destinations/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/snowflake/snowflake.py` & `dlt-0.3.8/dlt/destinations/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/snowflake/sql_client.py` & `dlt-0.3.8/dlt/destinations/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/sql_client.py` & `dlt-0.3.8/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/sql_jobs.py` & `dlt-0.3.8/dlt/destinations/sql_jobs.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/destinations/typing.py` & `dlt-0.3.8/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/decorators.py` & `dlt-0.3.8/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/exceptions.py` & `dlt-0.3.8/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/extract.py` & `dlt-0.3.8/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/incremental.py` & `dlt-0.3.8/dlt/extract/incremental.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from typing import Generic, TypeVar, Any, Optional, Callable, List, TypedDict, get_origin, Sequence
+import os
+from typing import Generic, TypeVar, Any, Optional, Callable, List, TypedDict, get_args, get_origin, Sequence, Type
 import inspect
 from functools import wraps
 from datetime import datetime  # noqa: I251
 
 import dlt
+from dlt.common import pendulum, logger
 from dlt.common.json import json
 from dlt.common.jsonpath import compile_path, find_values, JSONPath
-from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
+from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, get_generic_type_argument_from_instance, is_optional_type
 from dlt.common.schema.typing import TColumnKey
 from dlt.common.configuration import configspec, ConfigurationValueError
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.pipeline import resource_state
 from dlt.common.utils import digest128
+from dlt.common.data_types.type_helpers import coerce_from_date_types, coerce_value, py_type_to_sc_type
+
 from dlt.extract.exceptions import IncrementalUnboundError, PipeException
 from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
-from dlt.common import pendulum
+
+from dlt.common.time import ensure_pendulum_datetime
 
 
 TCursorValue = TypeVar("TCursorValue", bound=Any)
 LastValueFunc = Callable[[Sequence[TCursorValue]], Any]
 
 
 class IncrementalColumnState(TypedDict):
@@ -74,39 +79,46 @@
         cursor_path: The name or a JSON path to an cursor field. Uses the same names of fields as in your JSON document, before they are normalized to store in the database.
         initial_value: Optional value used for `last_value` when no state is available, e.g. on the first run of the pipeline. If not provided `last_value` will be `None` on the first run.
         last_value_func: Callable used to determine which cursor value to save in state. It is called with a list of the stored state value and all cursor vals from currently processing items. Default is `max`
         primary_key: Optional primary key used to deduplicate data. If not provided, a primary key defined by the resource will be used. Pass a tuple to define a compound key. Pass empty tuple to disable unique checks
         end_value: Optional value used to load a limited range of records between `initial_value` and `end_value`.
             Use in conjunction with `initial_value`, e.g. load records from given month `incremental(initial_value="2022-01-01T00:00:00Z", end_value="2022-02-01T00:00:00Z")`
             Note, when this is set the incremental filtering is stateless and `initial_value` always supersedes any previous incremental value in state.
+        allow_external_schedulers: If set to True, allows dlt to look for external schedulers from which it will take "initial_value" and "end_value" resulting in loading only
+            specified range of data. Currently Airflow scheduler is detected: "data_interval_start" and "data_interval_end" are taken from the context and passed Incremental class.
+            The values passed explicitly to Incremental will be ignored.
+            Note that if logical "end date" is present then also "end_value" will be set which means that resource state is not used and exactly this range of date will be loaded
     """
     cursor_path: str = None
     # TODO: Support typevar here
     initial_value: Optional[Any] = None
     end_value: Optional[Any] = None
 
     def __init__(
             self,
             cursor_path: str = dlt.config.value,
             initial_value: Optional[TCursorValue]=None,
             last_value_func: Optional[LastValueFunc[TCursorValue]]=max,
             primary_key: Optional[TTableHintTemplate[TColumnKey]] = None,
-            end_value: Optional[TCursorValue] = None
+            end_value: Optional[TCursorValue] = None,
+            allow_external_schedulers: bool = False
     ) -> None:
         self.cursor_path = cursor_path
         if self.cursor_path:
             self.cursor_path_p: JSONPath = compile_path(cursor_path)
         self.last_value_func = last_value_func
         self.initial_value = initial_value
         """Initial value of last_value"""
         self.end_value = end_value
         self.start_value: Any = initial_value
         """Value of last_value at the beginning of current pipeline run"""
         self.resource_name: Optional[str] = None
         self.primary_key: Optional[TTableHintTemplate[TColumnKey]] = primary_key
+        self.allow_external_schedulers = allow_external_schedulers
+
         self._cached_state: IncrementalColumnState = None
         """State dictionary cached on first access"""
         super().__init__(self.transform)
 
         self.end_out_of_range: bool = False
         """Becomes true on the first item that is out of range of `end_value`. I.e. when using `max` function this means a value that is equal or higher"""
         self.start_out_of_range: bool = False
@@ -117,33 +129,47 @@
         """Create Incremental instance from existing state."""
         state = Incremental._get_state(resource_name, cursor_path)
         i = cls(cursor_path, state["initial_value"])
         i.resource_name = resource_name
         return i
 
     def copy(self) -> "Incremental[TCursorValue]":
-        return self.__class__(
-            self.cursor_path, initial_value=self.initial_value, last_value_func=self.last_value_func, primary_key=self.primary_key, end_value=self.end_value
+        # preserve Generic param information
+        constructor = self.__orig_class__ if hasattr(self, "__orig_class__") else self.__class__
+        return constructor(  # type: ignore
+            self.cursor_path,
+            initial_value=self.initial_value,
+            last_value_func=self.last_value_func,
+            primary_key=self.primary_key,
+            end_value=self.end_value,
+            allow_external_schedulers=self.allow_external_schedulers
         )
 
     def merge(self, other: "Incremental[TCursorValue]") -> "Incremental[TCursorValue]":
         """Create a new incremental instance which merges the two instances.
         Only properties which are not `None` from `other` override the current instance properties.
 
         This supports use cases with partial overrides, such as:
         >>> def my_resource(updated=incremental('updated', initial_value='1970-01-01'))
         >>>     ...
         >>>
         >>> my_resource(updated=incremental(initial_value='2023-01-01', end_value='2023-02-01'))
         """
         kwargs = dict(self, last_value_func=self.last_value_func, primary_key=self.primary_key)
-        for key, value in dict(other, last_value_func=other.last_value_func, primary_key=other.primary_key).items():
+        for key, value in dict(
+                other,
+                last_value_func=other.last_value_func, primary_key=other.primary_key).items():
             if value is not None:
                 kwargs[key] = value
-        return self.__class__(**kwargs)
+        # preserve Generic param information
+        if hasattr(self, "__orig_class__"):
+            constructor = self.__orig_class__
+        else:
+            constructor = other.__orig_class__ if hasattr(other, "__orig_class__") else other.__class__
+        return constructor(**kwargs)  # type: ignore
 
     def on_resolved(self) -> None:
         self.cursor_path_p = compile_path(self.cursor_path)
         if self.end_value is not None and self.initial_value is None:
             raise ConfigurationValueError(
                 "Incremental 'end_value' was specified without 'initial_value'. 'initial_value' is required when using 'end_value'."
             )
@@ -273,38 +299,109 @@
             incremental_state["last_value"] = new_value
             unique_value = self.unique_value(row)
             if unique_value:
                 incremental_state["unique_hashes"] = [unique_value]
 
         return True
 
+    def get_incremental_value_type(self) -> Type[Any]:
+        """Infers the type of incremental value from a class of an instance if those preserve the Generic arguments information."""
+        return get_generic_type_argument_from_instance(self, self.initial_value)
+
+    def _join_external_scheduler(self) -> None:
+        """Detects existence of external scheduler from which `start_value` and `end_value` are taken. Detects Airflow and environment variables.
+           The logical "start date" coming from external scheduler will set the `initial_value` in incremental. if additionally logical "end date" is
+           present then also "end_value" will be set which means that resource state is not used and exactly this range of date will be loaded
+        """
+        # fit the pendulum into incremental type
+        param_type = self.get_incremental_value_type()
+
+        try:
+            if param_type is not Any:
+                data_type = py_type_to_sc_type(param_type)
+        except Exception as ex:
+            logger.warning(f"Specified Incremental last value type {param_type} is not supported. Please use DateTime, Date, float, int or str to join external schedulers.({ex})")
+
+        if param_type is Any:
+            logger.warning("Could not find the last value type of Incremental class participating in external schedule. "
+                           "Please add typing when declaring incremental argument in your resource or pass initial_value from which the type can be inferred.")
+            return
+
+        def _ensure_airflow_end_date(start_date: pendulum.DateTime, end_date: pendulum.DateTime) -> Optional[pendulum.DateTime]:
+            """if end_date is in the future or same as start date (manual run), set it to None so dlt state is used for incremental loading"""
+            now = pendulum.now()
+            if end_date is None or end_date > now or start_date == end_date:
+                return now
+            return end_date
+
+        try:
+            # we can move it to separate module when we have more of those
+            from airflow.operators.python import get_current_context  # noqa
+            context = get_current_context()
+            start_date = context["data_interval_start"]
+            end_date = _ensure_airflow_end_date(start_date, context["data_interval_end"])
+            self.initial_value = coerce_from_date_types(data_type, start_date)
+            if end_date is not None:
+                self.end_value = coerce_from_date_types(data_type, end_date)
+            else:
+                self.end_value = None
+            logger.info(f"Found Airflow scheduler: initial value: {self.initial_value} from data_interval_start {context['data_interval_start']}, end value: {self.end_value} from data_interval_end {context['data_interval_end']}")
+            return
+        except TypeError as te:
+            logger.warning(f"Could not coerce Airflow execution dates into the last value type {param_type}. ({te})")
+        except Exception:
+            pass
+
+        if start_value := os.environ.get("DLT_START_VALUE"):
+            self.initial_value = coerce_value(data_type, "text", start_value)
+            if end_value := os.environ.get("DLT_END_VALUE"):
+                self.end_value = coerce_value(data_type, "text", end_value)
+            else:
+                self.end_value = None
+            return
+
     def bind(self, pipe: SupportsPipe) -> "Incremental[TCursorValue]":
-        "Called by pipe just before evaluation"
+        """Called by pipe just before evaluation"""
         # bind the resource/pipe name
         if self.is_partial():
             raise IncrementalCursorPathMissing(pipe.name, None, None)
         self.resource_name = pipe.name
+        # try to join external scheduler
+        if self.allow_external_schedulers:
+            self._join_external_scheduler()
         # set initial value from last value, in case of a new state those are equal
         self.start_value = self.last_value
+        logger.info(f"Bind incremental on {self.resource_name} with initial_value: {self.initial_value}, start_value: {self.start_value}, end_value: {self.end_value}")
         # cache state
         self._cached_state = self.get_state()
         return self
 
     def __str__(self) -> str:
         return f"Incremental at {id(self)} for resource {self.resource_name} with cursor path: {self.cursor_path} initial {self.initial_value} lv_func {self.last_value_func}"
 
 
 class IncrementalResourceWrapper(FilterItem):
     _incremental: Optional[Incremental[Any]] = None
     """Keeps the injectable incremental"""
 
     def __init__(self, resource_name: str, primary_key: Optional[TTableHintTemplate[TColumnKey]] = None) -> None:
+        """Creates a wrapper over a resource function that accepts Incremental instance in its argument to perform incremental loading.
+
+        The wrapper delays instantiation of the Incremental to the moment of actual execution and is currently used by `dlt.resource` decorator.
+        The wrapper explicitly (via `resource_name`) parameter binds the Incremental state to a resource state.
+        Note that wrapper implements `FilterItem` transform interface and functions as a processing step in the before-mentioned resource pipe.
+
+        Args:
+            resource_name (str): A name of resource to which the Incremental will be bound at execution
+            primary_key (TTableHintTemplate[TColumnKey], optional): A primary key to be passed to Incremental Instance at execution. Defaults to None.
+        """
         self.resource_name = resource_name
         self.primary_key = primary_key
         self.incremental_state: IncrementalColumnState = None
+        self._allow_external_schedulers: bool = None
 
     @staticmethod
     def should_wrap(sig: inspect.Signature) -> bool:
         return IncrementalResourceWrapper.get_incremental_arg(sig) is not None
 
     @staticmethod
     def get_incremental_arg(sig: inspect.Signature) -> Optional[inspect.Parameter]:
@@ -342,34 +439,52 @@
                 elif isinstance(p.default, Incremental):
                     # Passing only initial value explicitly updates the default instance
                     new_incremental = p.default.copy()
                     new_incremental.initial_value = explicit_value
             elif isinstance(p.default, Incremental):
                 new_incremental = p.default.copy()
 
-
             if not new_incremental or new_incremental.is_partial():
                 if is_optional_type(p.annotation):
                     bound_args.arguments[p.name] = None  # Remove partial spec
                     return func(*bound_args.args, **bound_args.kwargs)
                 raise ValueError(f"{p.name} Incremental has no default")
+            # pass Generic information from annotation to new_incremental
+            if not hasattr(new_incremental, "__orig_class__") and p.annotation and get_args(p.annotation):
+                new_incremental.__orig_class__ = p.annotation  # type: ignore
+
             # set the incremental only if not yet set or if it was passed explicitly
             # NOTE: the _incremental may be also set by applying hints to the resource see `set_template` in `DltResource`
             if p.name in bound_args.arguments or not self._incremental:
                 self._incremental = new_incremental
             self._incremental.resolve()
             # in case of transformers the bind will be called before this wrapper is set: because transformer is called for a first time late in the pipe
             self._incremental.bind(Pipe(self.resource_name))
             bound_args.arguments[p.name] = self._incremental
             return func(*bound_args.args, **bound_args.kwargs)
 
         return _wrap  # type: ignore
 
+    @property
+    def allow_external_schedulers(self) -> bool:
+        """Allows the Incremental instance to get its initial and end values from external schedulers like Airflow"""
+        if self._incremental:
+            return self._incremental.allow_external_schedulers
+        return self._allow_external_schedulers
+
+    @allow_external_schedulers.setter
+    def allow_external_schedulers(self, value: bool) -> None:
+        self._allow_external_schedulers = value
+        if self._incremental:
+            self._incremental.allow_external_schedulers = value
+
     def bind(self, pipe: SupportsPipe) -> "IncrementalResourceWrapper":
         if self._incremental:
+            if self._allow_external_schedulers is not None:
+                self._incremental.allow_external_schedulers = self._allow_external_schedulers
             self._incremental.bind(pipe)
         return self
 
     def __call__(self, item: TDataItems, meta: Any = None) -> Optional[TDataItems]:
         if not self._incremental:
             return item
         if self._incremental.primary_key is None:
```

### Comparing `dlt-0.3.7/dlt/extract/pipe.py` & `dlt-0.3.8/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/schema.py` & `dlt-0.3.8/dlt/extract/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from copy import copy, deepcopy
 from collections.abc import Mapping as C_Mapping
 from typing import List, TypedDict, cast, Any
 
 from dlt.common.schema.utils import DEFAULT_WRITE_DISPOSITION, merge_columns, new_column, new_table
 from dlt.common.schema.typing import TColumnKey, TColumnProp, TColumnSchema, TPartialTableSchema, TTableSchemaColumns, TWriteDisposition
 from dlt.common.typing import TDataItem
-from dlt.common.validation import validate_dict
+from dlt.common.validation import validate_dict_ignoring_xkeys
 
 from dlt.extract.incremental import Incremental
 from dlt.extract.typing import TFunHintTemplate, TTableHintTemplate
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, InconsistentTableTemplate, TableNameMissing
 
 
 class TTableSchemaTemplate(TypedDict, total=False):
@@ -63,15 +63,19 @@
         if self._table_name_hint_fun and item is None:
             raise DataItemRequiredForDynamicTableHints(self._name)
         # resolve
         resolved_template: TTableSchemaTemplate = {k: self._resolve_hint(item, v) for k, v in table_template.items()}  # type: ignore
         resolved_template.pop("incremental", None)
         table_schema = self._merge_keys(resolved_template)
         table_schema["resource"] = self._name
-        validate_dict(TPartialTableSchema, table_schema, f"new_table/{self._name}")
+        validate_dict_ignoring_xkeys(
+            spec=TPartialTableSchema,
+            doc=table_schema,
+            path=f"new_table/{self._name}",
+        )
         return table_schema
 
     def apply_hints(
         self,
         table_name: TTableHintTemplate[str] = None,
         parent_table_name: TTableHintTemplate[str] = None,
         write_disposition: TTableHintTemplate[TWriteDisposition] = None,
```

### Comparing `dlt-0.3.7/dlt/extract/source.py` & `dlt-0.3.8/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/typing.py` & `dlt-0.3.8/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/extract/utils.py` & `dlt-0.3.8/dlt/extract/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List, Any, Sequence
+from typing import Union, List, Any
 
 from dlt.extract.typing import TTableHintTemplate, TDataItem
 from dlt.common.schema.typing import TColumnKey
 
 
 def resolve_column_value(column_hint: TTableHintTemplate[TColumnKey], item: TDataItem) -> Union[Any, List[Any]]:
     """Extract values from the data item given a column hint.
```

### Comparing `dlt-0.3.7/dlt/helpers/airflow_helper.py` & `dlt-0.3.8/dlt/helpers/airflow_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from tempfile import gettempdir
-from typing import Any, Callable, List, Literal, Sequence
+from typing import Any, Callable, List, Literal, Optional, Sequence, Tuple
 from tenacity import retry_if_exception, wait_exponential, stop_after_attempt, Retrying, RetryCallState
 
+from dlt.common import pendulum
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.runtime.telemetry import with_telemetry
 
 try:
     from airflow.configuration import conf
     from airflow.utils.task_group import TaskGroup
     from airflow.operators.python import PythonOperator
@@ -252,7 +253,16 @@
             else:
                 raise ValueError(decompose)
 
     def add_fun(self, f: Callable[..., Any], **kwargs: Any) -> Any:
         """Will execute a function `f` inside an Airflow task. It is up to the function to create pipeline and source(s)"""
         raise NotImplementedError()
 
+
+def airflow_get_execution_dates() -> Tuple[pendulum.DateTime, Optional[pendulum.DateTime]]:
+    # prefer logging to task logger
+    try:
+        from airflow.operators.python import get_current_context  # noqa
+        context = get_current_context()
+        return context["data_interval_start"], context["data_interval_end"]
+    except Exception:
+        return None, None
```

### Comparing `dlt-0.3.7/dlt/helpers/dbt/__init__.py` & `dlt-0.3.8/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/dbt/configuration.py` & `dlt-0.3.8/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.8/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.8/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.8/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/dbt/runner.py` & `dlt-0.3.8/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/pandas_helper.py` & `dlt-0.3.8/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/helpers/streamlit_helper.py` & `dlt-0.3.8/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/load/configuration.py` & `dlt-0.3.8/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/load/exceptions.py` & `dlt-0.3.8/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/load/load.py` & `dlt-0.3.8/dlt/load/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,22 +289,23 @@
         # initialize analytical storage ie. create dataset required by passed schema
         job_client: JobClientBase
         with self.get_destination_client(schema) as job_client:
             expected_update = self.load_storage.begin_schema_update(load_id)
             if expected_update is not None:
                 # update the default dataset
                 logger.info(f"Client for {job_client.config.destination_name} will start initialize storage")
-                truncate_tables = self.get_table_chain_tables_for_write_disposition(load_id, schema, job_client.get_truncate_destination_table_dispositions())
-                job_client.initialize_storage(truncate_tables=truncate_tables)
+                job_client.initialize_storage()
                 logger.info(f"Client for {job_client.config.destination_name} will update schema to package schema")
                 all_jobs = self.get_new_jobs_info(load_id, schema)
                 all_tables = set(job.table_name for job in all_jobs)
                 dlt_tables = set(t["name"] for t in schema.dlt_tables())
                 # only update tables that are present in the load package
                 applied_update = job_client.update_storage_schema(only_tables=all_tables | dlt_tables, expected_update=expected_update)
+                truncate_tables = self.get_table_chain_tables_for_write_disposition(load_id, schema, job_client.get_truncate_destination_table_dispositions())
+                job_client.initialize_storage(truncate_tables=truncate_tables)
                 # update the staging dataset if client supports this
                 if isinstance(job_client, StagingJobClientBase):
                     if staging_tables := self.get_table_chain_tables_for_write_disposition(load_id, schema, job_client.get_stage_dispositions()):
                         with job_client.with_staging_dataset():
                             logger.info(f"Client for {job_client.config.destination_name} will start initialize STAGING storage")
                             job_client.initialize_storage()
                             logger.info(f"Client for {job_client.config.destination_name} will UPDATE STAGING SCHEMA to package schema")
```

### Comparing `dlt-0.3.7/dlt/normalize/configuration.py` & `dlt-0.3.8/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/normalize/normalize.py` & `dlt-0.3.8/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/__init__.py` & `dlt-0.3.8/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/configuration.py` & `dlt-0.3.8/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/dbt.py` & `dlt-0.3.8/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/exceptions.py` & `dlt-0.3.8/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/helpers.py` & `dlt-0.3.8/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/pipeline.py` & `dlt-0.3.8/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/progress.py` & `dlt-0.3.8/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/state_sync.py` & `dlt-0.3.8/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/trace.py` & `dlt-0.3.8/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/pipeline/track.py` & `dlt-0.3.8/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/reflection/names.py` & `dlt-0.3.8/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/reflection/script_inspector.py` & `dlt-0.3.8/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/reflection/script_visitor.py` & `dlt-0.3.8/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.8/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.8/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/sources/helpers/requests/session.py` & `dlt-0.3.8/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/sources/helpers/transform.py` & `dlt-0.3.8/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/dlt/version.py` & `dlt-0.3.8/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.7/pyproject.toml` & `dlt-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.7"
+version = "0.3.8"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -122,14 +122,15 @@
 pandas = "^1.5.3"
 sqlfluff = "^1.4.5"
 google-auth-oauthlib = "^1.0.0"
 types-deprecated = "^1.2.9.2"
 tqdm = "^4.65.0"
 enlighten = "^1.11.2"
 alive-progress = "^3.1.1"
+pytest-console-scripts = "^1.4.1"
 
 [tool.poetry.group.airflow]
 optional = true
 
 [tool.poetry.group.airflow.dependencies]
 apache-airflow = "^2.5.3"
```

### Comparing `dlt-0.3.7/setup.py` & `dlt-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,17 @@
  'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
-    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nimport requests\n# Create a dlt pipeline that will load\n# chess player data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'player_data\'\n)\n# Grab some player data from Chess.com API\ndata = []\nfor player in [\'magnuscarlsen\', \'rpragchess\']:\n    response = requests.get(f\'https://api.chess.com/pub/player/{player}\')\n    response.raise_for_status()\n    data.append(response.json())\n# Extract, normalize, and load the data\npipeline.run(data, table_name=\'player\')\n```\n\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
+    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n\n<h3 align="center">\n\n🚀 Join our thriving community of likeminded developers and build the future together!\n\n</h3>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" style="width: 260px;"  />\n  </a>\n</div>\n<div align="center">\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nimport requests\n# Create a dlt pipeline that will load\n# chess player data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'player_data\'\n)\n# Grab some player data from Chess.com API\ndata = []\nfor player in [\'magnuscarlsen\', \'rpragchess\']:\n    response = requests.get(f\'https://api.chess.com/pub/player/{player}\')\n    response.raise_for_status()\n    data.append(response.json())\n# Extract, normalize, and load the data\npipeline.run(data, table_name=\'player\')\n```\n\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlt-0.3.7/PKG-INFO` & `dlt-0.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.7
+Version: 0.3.8
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -84,18 +84,27 @@
 <h1 align="center">
     <strong>data load tool (dlt) — the open-source Python library for data loading</strong>
 </h1>
 <p align="center">
 Be it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.
 </p>
 
+
+<h3 align="center">
+
+🚀 Join our thriving community of likeminded developers and build the future together!
+
+</h3>
+
 <div align="center">
   <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">
-    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />
+    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" style="width: 260px;"  />
   </a>
+</div>
+<div align="center">
   <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
     <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">
   </a>
   <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">
     <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">
   </a>
 </div>
```

