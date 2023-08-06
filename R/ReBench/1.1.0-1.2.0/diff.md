# Comparing `tmp/ReBench-1.1.0.tar.gz` & `tmp/ReBench-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReBench-1.1.0.tar", last modified: Tue Feb 21 08:23:13 2023, max compression
+gzip compressed data, was "ReBench-1.2.0.tar", last modified: Sun Aug  6 15:12:45 2023, max compression
```

## Comparing `ReBench-1.1.0.tar` & `ReBench-1.2.0.tar`

### file list

```diff
@@ -1,108 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.742092 ReBench-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-21 08:23:00.000000 ReBench-1.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-21 08:23:00.000000 ReBench-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-02-21 08:23:13.742092 ReBench-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-02-21 08:23:00.000000 ReBench-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.734091 ReBench-1.1.0/ReBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 08:23:13.000000 ReBench-1.1.0/ReBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.734091 ReBench-1.1.0/rebench/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/configuration_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21420 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.738092 ReBench-1.1.0/rebench/interop/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/jmh_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/multivariate_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/perf_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/perf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/plain_seconds_log_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/rebench_log_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/savina_log_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/test_vm_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/time_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/interop/validation_log_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.738092 ReBench-1.1.0/rebench/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/benchmark_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/build_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/exp_run_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/exp_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/profile_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/model/termination_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/rebench-schema.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    15941 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/rebench.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/rebenchdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/subprocess_kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/subprocess_with_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.734091 ReBench-1.1.0/rebench/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.738092 ReBench-1.1.0/rebench/tests/bugs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_111_report_ignores_warmup_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_111_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_112_invocations_setting_ignored_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_117_input_size_setting_ignored_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_27_invalid_run_not_handled_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_27_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_4_run_equality_and_params_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/issue_54_extra_args_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      296 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/bugs/vm-one-result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.742092 ReBench-1.1.0/rebench/tests/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/ignore_timeouts_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      402 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/ignore_timeouts_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_110_setup_run_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_15_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_15_warm_up_support_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_169_config_composition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_16_multiple_data_points_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_16_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_19_one_data_point_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_19_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_31_multivariate_data_points_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_31_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_32_jmh_support_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_34_accept_faulty_runs_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      379 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_34_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_42_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1218 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_42_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_57_binary_on_path_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_58_build_vm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_59_build_suite_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/features/issue_81_unicode_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.742092 ReBench-1.1.0/rebench/tests/interop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/interop/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/interop/plain_seconds_log_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/interop/rebench_log_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/interop/time_adapter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.742092 ReBench-1.1.0/rebench/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/model/runs_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:13.742092 ReBench-1.1.0/rebench/tests/perf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/perf/issue_166_profiling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/tests/perf/perf_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-02-21 08:23:00.000000 ReBench-1.1.0/rebench/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 08:23:13.742092 ReBench-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-21 08:23:00.000000 ReBench-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.705436 ReBench-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-06 15:12:33.000000 ReBench-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-06 15:12:33.000000 ReBench-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-08-06 15:12:45.705436 ReBench-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-08-06 15:12:33.000000 ReBench-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.697436 ReBench-1.2.0/ReBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 15:12:45.000000 ReBench-1.2.0/ReBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.697436 ReBench-1.2.0/rebench/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/configuration_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24151 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.701436 ReBench-1.2.0/rebench/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/jmh_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/multivariate_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/perf_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/perf_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/plain_seconds_log_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/rebench_log_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/savina_log_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/test_vm_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/time_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/interop/validation_log_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.701436 ReBench-1.2.0/rebench/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/benchmark_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/build_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/exp_run_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/exp_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/profile_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/model/termination_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/rebench-schema.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16739 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/rebench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/rebenchdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/subprocess_kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/subprocess_with_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.697436 ReBench-1.2.0/rebench/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.701436 ReBench-1.2.0/rebench/tests/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_111_report_ignores_warmup_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      460 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_111_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_112_invocations_setting_ignored_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_117_input_size_setting_ignored_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_27_invalid_run_not_handled_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_27_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_4_run_equality_and_params_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/issue_54_extra_args_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      258 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/bugs/vm-one-result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.705436 ReBench-1.2.0/rebench/tests/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/ignore_timeouts_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/ignore_timeouts_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_110_setup_run_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      405 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_15_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_15_warm_up_support_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_169_config_composition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_16_multiple_data_points_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_16_vm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      526 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_16_vm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_19_one_data_point_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      293 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_19_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_209_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_209_adapter2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_209_custom_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_216_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_216_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_31_multivariate_data_points_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      489 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_31_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_32_jmh_support_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_34_accept_faulty_runs_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_34_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_42_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_42_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_57_binary_on_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_58_build_vm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_59_build_suite_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/features/issue_81_unicode_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.705436 ReBench-1.2.0/rebench/tests/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/interop/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/interop/plain_seconds_log_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/interop/rebench_log_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/interop/time_adapter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.705436 ReBench-1.2.0/rebench/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/model/runs_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:45.705436 ReBench-1.2.0/rebench/tests/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/perf/issue_166_profiling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/tests/perf/perf_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-08-06 15:12:33.000000 ReBench-1.2.0/rebench/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 15:12:45.705436 ReBench-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-06 15:12:33.000000 ReBench-1.2.0/setup.py
```

### Comparing `ReBench-1.1.0/LICENSE` & `ReBench-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/PKG-INFO` & `ReBench-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReBench
-Version: 1.1.0
+Version: 1.2.0
 Summary: Execute and document benchmarks reproducibly.
 Home-page: https://github.com/smarr/ReBench
 Author: Stefan Marr
 Author-email: rebench@stefan-marr.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -94,15 +94,15 @@
 pip install rebench
 ```
 
 To reduce noise generated by the system, `rebench-denoise` depends on:
 
  - `sudo` rights. `rebench` will attempt to determine suitable configuration
    parameters and suggest them. This includes allowing the execution of `rebench-denoise`
-   via `sudo` without password.
+   via `sudo` without password and with the permission to set environment variables (`SETENV`).
  - [`cpuset`](https://github.com/lpechacek/cpuset/) to reserve cores for benchmarking.
    On Ubuntu: `apt install cpuset`
 
 Please note that `rebench-denoise` is only tested on Ubuntu. It is designed to degrade
 gracefully and report the expected implications when it cannot adapt system
 settings. See the [docs][denoise-docs] for details.
```

### Comparing `ReBench-1.1.0/README.md` & `ReBench-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 pip install rebench
 ```
 
 To reduce noise generated by the system, `rebench-denoise` depends on:
 
  - `sudo` rights. `rebench` will attempt to determine suitable configuration
    parameters and suggest them. This includes allowing the execution of `rebench-denoise`
-   via `sudo` without password.
+   via `sudo` without password and with the permission to set environment variables (`SETENV`).
  - [`cpuset`](https://github.com/lpechacek/cpuset/) to reserve cores for benchmarking.
    On Ubuntu: `apt install cpuset`
 
 Please note that `rebench-denoise` is only tested on Ubuntu. It is designed to degrade
 gracefully and report the expected implications when it cannot adapt system
 settings. See the [docs][denoise-docs] for details.
```

### Comparing `ReBench-1.1.0/ReBench.egg-info/PKG-INFO` & `ReBench-1.2.0/ReBench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReBench
-Version: 1.1.0
+Version: 1.2.0
 Summary: Execute and document benchmarks reproducibly.
 Home-page: https://github.com/smarr/ReBench
 Author: Stefan Marr
 Author-email: rebench@stefan-marr.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -94,15 +94,15 @@
 pip install rebench
 ```
 
 To reduce noise generated by the system, `rebench-denoise` depends on:
 
  - `sudo` rights. `rebench` will attempt to determine suitable configuration
    parameters and suggest them. This includes allowing the execution of `rebench-denoise`
-   via `sudo` without password.
+   via `sudo` without password and with the permission to set environment variables (`SETENV`).
  - [`cpuset`](https://github.com/lpechacek/cpuset/) to reserve cores for benchmarking.
    On Ubuntu: `apt install cpuset`
 
 Please note that `rebench-denoise` is only tested on Ubuntu. It is designed to degrade
 gracefully and report the expected implications when it cannot adapt system
 settings. See the [docs][denoise-docs] for details.
```

### Comparing `ReBench-1.1.0/ReBench.egg-info/SOURCES.txt` & `ReBench-1.2.0/ReBench.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -66,16 +66,22 @@
 rebench/tests/features/ignore_timeouts_vm.py
 rebench/tests/features/issue_110_setup_run_test.py
 rebench/tests/features/issue_15_vm.py
 rebench/tests/features/issue_15_warm_up_support_test.py
 rebench/tests/features/issue_169_config_composition_test.py
 rebench/tests/features/issue_16_multiple_data_points_test.py
 rebench/tests/features/issue_16_vm.py
+rebench/tests/features/issue_16_vm2.py
 rebench/tests/features/issue_19_one_data_point_test.py
 rebench/tests/features/issue_19_vm.py
+rebench/tests/features/issue_209_adapter.py
+rebench/tests/features/issue_209_adapter2.py
+rebench/tests/features/issue_209_custom_adapter_test.py
+rebench/tests/features/issue_216_test.py
+rebench/tests/features/issue_216_vm.py
 rebench/tests/features/issue_31_multivariate_data_points_test.py
 rebench/tests/features/issue_31_vm.py
 rebench/tests/features/issue_32_jmh_support_test.py
 rebench/tests/features/issue_34_accept_faulty_runs_test.py
 rebench/tests/features/issue_34_vm.py
 rebench/tests/features/issue_42_test.py
 rebench/tests/features/issue_42_vm.py
```

### Comparing `ReBench-1.1.0/rebench/configuration_error.py` & `ReBench-1.2.0/rebench/configuration_error.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/configurator.py` & `ReBench-1.2.0/rebench/configurator.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 import logging
-from os.path import dirname
+from os.path import dirname, abspath
 from pykwalify.core import Core
 from pykwalify.errors import SchemaError
 import yaml
 
 from .configuration_error import ConfigurationError
 from .model.experiment import Experiment
 from .model.exp_run_details import ExpRunDetails
@@ -126,14 +126,20 @@
         with open(file_name, 'r') as conf_file:  # pylint: disable=unspecified-encoding
             data = yaml.safe_load(conf_file)
             validator = Core(
                 source_data=data,
                 schema_files=[dirname(__file__) + "/rebench-schema.yml"])
             try:
                 validator.validate(raise_exception=True)
+                validate_gauge_adapters(data)
+
+                # add file name and directory to config to be able to use it when loading
+                # for instance gauge adapters
+                data['__file__'] = file_name
+                data['__dir__'] = dirname(abspath(file_name))
             except SchemaError as err:
                 errors = [escape_braces(val_err) for val_err in validator.validation_errors]
                 raise UIError(
                     "Validation of " + file_name + " failed.\n{ind}" +
                     "\n{ind}".join(errors) + "\n", err)
             return data
     except IOError as err:
@@ -143,24 +149,41 @@
                           % (file_name, err.strerror), err)
         raise UIError(str(err) + "\n", err)
     except yaml.YAMLError as err:
         raise UIError("Parsing of the config file "
                       + file_name + " failed.\nError " + str(err) + "\n", err)
 
 
+def validate_gauge_adapters(raw_config):
+    benchmark_suites = raw_config.get('benchmark_suites', {})
+    for suite_name, suite in benchmark_suites.items():
+        adapter = suite['gauge_adapter']
+        if not isinstance(adapter, (dict, str)):
+            raise UIError(("Gauge adapter for suite %s must be a string or a dictionary," +
+                           "but is %s.\n") % (suite_name, type(adapter).__name__), None)
+
+        if isinstance(adapter, dict) and len(adapter) != 1:
+            raise UIError("When specifying a custom gauge adapter," +
+                          " exactly one must to be specified." +
+                          " Currently there are %d. (%s)\n" % (len(adapter), adapter), None)
+    return True
+
+
 class Configurator(object):
 
     def __init__(self, raw_config, data_store, ui, cli_options=None, cli_reporter=None,
                  exp_name=None, data_file=None, build_log=None, run_filter=None):
         self._raw_config_for_debugging = raw_config  # kept around for debugging only
 
         self.build_log = build_log or raw_config.get('build_log', 'build.log')
         self.data_file = data_file or raw_config.get('default_data_file', 'rebench.data')
         self._exp_name = exp_name or raw_config.get('default_experiment', 'all')
         self.artifact_review = raw_config.get('artifact_review', False)
+        self.config_dir = raw_config.get('__dir__', None)
+        self.config_file = raw_config.get('__file__', None)
 
         self._rebench_db_connector = None
 
         # capture invocation and iteration settings and override when quick is selected
         invocations = cli_options.invocations if cli_options else None
         iterations = cli_options.iterations if cli_options else None
         if cli_options:
@@ -260,14 +283,18 @@
     def run_details(self):
         return self._root_run_details
 
     def has_executor(self, executor_name):
         return executor_name in self._executors
 
     def get_executor(self, executor_name, run_details, variables, action):
+        if executor_name not in self._executors:
+            raise ConfigurationError(
+                "An experiment tries to use an undefined executor: %s" % executor_name)
+
         executor = Executor.compile(
             executor_name, self._executors[executor_name],
             run_details, variables, self.build_commands, action)
         return executor
 
     def get_suite(self, suite_name):
         return self._suites_config[suite_name]
```

### Comparing `ReBench-1.1.0/rebench/denoise.py` & `ReBench-1.2.0/rebench/denoise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import print_function
-
 import getpass
 import json
 import os
 import subprocess
 import sys
 
 from argparse import ArgumentParser
@@ -16,19 +14,14 @@
 from .subprocess_kill import kill_process  # pylint: disable=cyclic-import
 
 try:
     from . import __version__ as rebench_version
 except ValueError:
     rebench_version = "unknown"
 
-try:
-    FileNotFoundError  # pylint: disable=used-before-assignment
-except NameError:
-    FileNotFoundError = IOError  # pylint: disable=redefined-builtin
-
 
 class DenoiseResult(object):
 
     def __init__(self, succeeded, warn_msg, use_nice, use_shielding, details):
         self.succeeded = succeeded
         self.warn_msg = warn_msg
         self.use_nice = use_nice
@@ -101,15 +94,15 @@
             except subprocess.CalledProcessError:
                 denoise_cmd = '$PATH_TO/rebench-denoise'
 
             msg += '{ind}Please make sure `sudo rebench-denoise`'\
                    + ' can be used without password.\n'
             msg += '{ind}To be able to run rebench-denoise without password,\n'
             msg += '{ind}add the following to the end of your sudoers file (using visudo):\n'
-            msg += '{ind}{ind}' + getpass.getuser() + ' ALL = (root) NOPASSWD: '\
+            msg += '{ind}{ind}' + getpass.getuser() + ' ALL = (root) NOPASSWD:SETENV: '\
                    + denoise_cmd + '\n'
         elif 'command not found' in output:
             msg += '{ind}Please make sure `rebench-denoise` is on the PATH\n'
         elif "No such file or directory: 'sudo'" in output:
             msg += '{ind}sudo is not available. Can\'t use rebench-denoise to manage the system.\n'
         else:
             msg += '{ind}Error: ' + escape_braces(output)
```

### Comparing `ReBench-1.1.0/rebench/environment.py` & `ReBench-1.2.0/rebench/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import getpass
 import os
 import subprocess
 
+from urllib.parse import urlparse
 from cpuinfo.cpuinfo import _get_cpu_info_internal
 from psutil import virtual_memory
 
 from .subprocess_with_timeout import output_as_str
 
-try:
-    from urllib.parse import urlparse
-except ImportError:
-    # Python 2.7
-    from urlparse import urlparse
-
 
 def _encode_str(out):
     as_string = output_as_str(out)
     if as_string and as_string[-1] == '\n':
         as_string = as_string[:-1]
     return as_string
 
@@ -110,23 +105,26 @@
     u_name = os.uname()
     result = {
         'userName': getpass.getuser(),
         'manualRun': not ('CI' in os.environ and os.environ['CI'] == 'true'),
         'hostName': u_name[1],
         'osType': u_name[0],
         'memory': virtual_memory().total,
-        'denoise': denoise_result.details
+        'denoise': {} if denoise_result is None else denoise_result.details
     }
 
     try:
         cpu_info = _get_cpu_info_internal()
         if cpu_info:
             result['cpu'] = cpu_info['brand_raw']
-            result['clockSpeed'] = (cpu_info['hz_advertised'][0]
-                                    * (10 ** cpu_info['hz_advertised'][1]))
+            if 'hz_advertised' in cpu_info:
+                result['clockSpeed'] = (cpu_info['hz_advertised'][0]
+                                        * (10 ** cpu_info['hz_advertised'][1]))
+            else:
+                result['clockSpeed'] = 0
     except ValueError:
         pass
 
     if 'cpu' not in result:
         ui.warning('Was not able to determine the type of CPU used and its clock speed.'
                    + ' Thus, these details will not be recorded with the data.')
```

### Comparing `ReBench-1.1.0/rebench/executor.py` & `ReBench-1.2.0/rebench/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,42 +13,42 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-from __future__ import with_statement
-
 from codecs import open as open_with_enc
 from collections import deque
 from math import floor
 from multiprocessing import cpu_count
 import os
 import random
 import subprocess
 from threading import Thread, RLock
 from time import time
 
 from . import subprocess_with_timeout as subprocess_timeout
-from .interop.adapter import ExecutionDeliveredNoResults, instantiate_adapter
+from .interop.adapter import ExecutionDeliveredNoResults, instantiate_adapter, OutputNotParseable, \
+    ResultsIndicatedAsInvalid
 from .ui import escape_braces
 
 
 class FailedBuilding(Exception):
     """The exception to be raised when building of the executor or suite failed."""
     def __init__(self, name, build_command):
         super(FailedBuilding, self).__init__()
         self._name = name
         self._build_command = build_command
 
 
 class RunScheduler(object):
 
-    def __init__(self, executor, ui):
+    def __init__(self, executor, ui, print_execution_plan):
+        self._print_execution_plan = print_execution_plan
         self._executor = executor
         self.ui = ui
         self._runs_completed = 0
         self._start_time = time()
         self._total_num_runs = 0
 
     @staticmethod
@@ -71,15 +71,15 @@
         etl = time_per_invocation * (self._total_num_runs - self._runs_completed)
         sec = etl % 60
         minute = (etl - sec) / 60 % 60
         hour = (etl - sec - minute) / 60 / 60
         return floor(hour), floor(minute), floor(sec)
 
     def _indicate_progress(self, completed_task, run):
-        if not self.ui.spinner_initialized():
+        if not self.ui.spinner_initialized() or self._print_execution_plan:
             return
 
         if completed_task:
             self._runs_completed += 1
 
         art_mean = run.get_mean_of_totals()
 
@@ -98,59 +98,76 @@
     def execute(self):
         self._total_num_runs = len(self._executor.runs)
         runs = self._filter_out_completed_runs(self._executor.runs, self.ui)
         completed_runs = self._total_num_runs - len(runs)
         self._runs_completed = completed_runs
 
         with self.ui.init_spinner(self._total_num_runs):
-            self.ui.step_spinner(completed_runs)
+            if not self._print_execution_plan:
+                self.ui.step_spinner(completed_runs)
             self._process_remaining_runs(runs)
 
 
 class BatchScheduler(RunScheduler):
 
     def _process_remaining_runs(self, runs):
-        for run_id in runs:
+        remaining_runs = list(runs)
+        while len(remaining_runs) > 0:
+            run_id = remaining_runs.pop(0)
             try:
                 completed = False
                 while not completed:
                     completed = self._executor.execute_run(run_id)
+                    if run_id.executable_missing:
+                        num_runs = len(remaining_runs)
+                        remaining_runs = self._executor.without_missing_binaries(
+                            run_id, remaining_runs)
+                        self._runs_completed += num_runs - len(remaining_runs)
                     self._indicate_progress(completed, run_id)
             except FailedBuilding:
                 pass
 
 
 class RoundRobinScheduler(RunScheduler):
 
     def _process_remaining_runs(self, runs):
         task_list = deque(runs)
-
         while task_list:
             try:
                 run = task_list.popleft()
                 completed = self._executor.execute_run(run)
-                self._indicate_progress(completed, run)
                 if not completed:
                     task_list.append(run)
+                elif run.executable_missing:
+                    num_runs = len(task_list)
+                    task_list = deque(self._executor.without_missing_binaries(
+                        run, task_list))
+                    self._runs_completed += num_runs - len(task_list)
+                self._indicate_progress(completed, run)
             except FailedBuilding:
                 pass
 
 
 class RandomScheduler(RunScheduler):
 
     def _process_remaining_runs(self, runs):
         task_list = list(runs)
-
         while task_list:
             run = random.choice(task_list)
             try:
                 completed = self._executor.execute_run(run)
-                self._indicate_progress(completed, run)
                 if completed:
                     task_list.remove(run)
+                    if run.executable_missing:
+                        num_runs = len(task_list)
+                        task_list = self._executor.without_missing_binaries(
+                            run, task_list)
+                        self._runs_completed += num_runs - len(task_list)
+                self._indicate_progress(completed, run)
+
             except FailedBuilding:
                 task_list.remove(run)
 
 
 class BenchmarkThread(Thread):
 
     def __init__(self, par_scheduler, num):
@@ -177,16 +194,16 @@
     def __init__(self, exceptions):
         super(BenchmarkThreadExceptions, self).__init__()
         self.exceptions = exceptions
 
 
 class ParallelScheduler(RunScheduler):
 
-    def __init__(self, executor, seq_scheduler_class, ui):
-        RunScheduler.__init__(self, executor, ui)
+    def __init__(self, executor, seq_scheduler_class, ui, print_execution_plan):
+        RunScheduler.__init__(self, executor, ui, print_execution_plan)
         self._seq_scheduler_class = seq_scheduler_class
         self._lock = RLock()
         self._num_worker_threads = self._number_of_threads()
         self._remaining_work = None
         self._worker_threads = None
 
     def _number_of_threads(self):
@@ -204,15 +221,15 @@
             else:
                 par_runs.append(run)
         return seq_runs, par_runs
 
     def _process_sequential_runs(self, runs):
         seq_runs, par_runs = self._split_runs(runs)
 
-        scheduler = self._seq_scheduler_class(self._executor, self.ui)
+        scheduler = self._seq_scheduler_class(self._executor, self.ui, self._print_execution_plan)
         scheduler._process_remaining_runs(seq_runs)
 
         return par_runs
 
     def _process_remaining_runs(self, runs):
         self._remaining_work = self._process_sequential_runs(runs)
 
@@ -238,15 +255,15 @@
         # different running times, without causing too much scheduling overhead
         k = len(self._remaining_work)
         per_thread = int(floor(float(k) / float(self._num_worker_threads)))
         per_thread = max(1, per_thread)  # take at least 1 run
         return per_thread
 
     def get_local_scheduler(self):
-        return self._seq_scheduler_class(self._executor, self.ui)
+        return self._seq_scheduler_class(self._executor, self.ui, self._print_execution_plan)
 
     def acquire_work(self):
         with self._lock:
             if not self._remaining_work:
                 return None
 
             num = self._determine_num_work_items_to_take()
@@ -258,54 +275,57 @@
 
 
 class Executor(object):
 
     def __init__(self, runs, do_builds, ui, include_faulty=False,
                  debug=False, scheduler=BatchScheduler, build_log=None,
                  artifact_review=False, use_nice=False, use_shielding=False,
-                 print_execution_plan=False):
+                 print_execution_plan=False, config_dir=None,
+                 use_denoise=True):
+        self.use_denoise = use_denoise
         self._runs = runs
 
         self._use_nice = use_nice
         self._use_shielding = use_shielding
-        self.use_denoise = use_nice or use_shielding
+        self.use_denoise = self.use_denoise and (use_nice or use_shielding)
 
         self._print_execution_plan = print_execution_plan
 
         self._do_builds = do_builds
         self.ui = ui
         self._include_faulty = include_faulty
         self.debug = debug
-        self._scheduler = self._create_scheduler(scheduler)
+        self._scheduler = self._create_scheduler(scheduler, print_execution_plan)
         self.build_log = build_log
         self._artifact_review = artifact_review
+        self.config_dir = config_dir
 
         num_runs = RunScheduler.number_of_uncompleted_runs(runs, ui)
         for run in runs:
             run.set_total_number_of_runs(num_runs)
 
-    def _create_scheduler(self, scheduler):
+    def _create_scheduler(self, scheduler, print_execution_plan):
         # figure out whether to use parallel scheduler
         if cpu_count() > 1:
             i = 0
             for run in self._runs:
                 if not run.execute_exclusively:
                     i += 1
             if i > 1:
-                return ParallelScheduler(self, scheduler, self.ui)
+                return ParallelScheduler(self, scheduler, self.ui, print_execution_plan)
 
-        return scheduler(self, self.ui)
+        return scheduler(self, self.ui, print_execution_plan)
 
     def _construct_cmdline(self, run_id, gauge_adapter):
         cmdline = ""
 
         if self.use_denoise:
             cmdline += "sudo "
             if run_id.env:
-                cmdline += "--preserve-env=" + ','.join(run_id.keys()) + " "
+                cmdline += "--preserve-env=" + ','.join(run_id.env.keys()) + " "
             cmdline += "rebench-denoise "
             if not self._use_nice:
                 cmdline += "--without-nice "
             if not self._use_shielding:
                 cmdline += "--without-shielding "
             if run_id.is_profiling():
                 cmdline += "--for-profiling "
@@ -397,14 +417,29 @@
             if stdout_result:
                 log_file.write(name + '|STD:')
                 log_file.write(stdout_result)
             if stderr_result:
                 log_file.write(name + '|ERR:')
                 log_file.write(stderr_result)
 
+    def without_missing_binaries(self, run_exe_missing, runs):
+        is_first = True
+        remaining_runs = []
+        for run in runs:
+            if run.has_same_executable(run_exe_missing):
+                run.fail_immediately()
+                run.report_run_failed(None, None, None)
+                run.report_run_completed(None)
+                if is_first:
+                    self.ui.warning("{ind}Aborting remaining benchmarks using %s." % run.executable)
+                    is_first = False
+            else:
+                remaining_runs.append(run)
+        return remaining_runs
+
     def execute_run(self, run_id):
         gauge_adapter = self._get_gauge_adapter_instance(run_id)
         if gauge_adapter is None:
             return True
 
         cmdline = self._construct_cmdline(run_id, gauge_adapter)
 
@@ -439,29 +474,30 @@
                     ("{ind}Warning: Low mean run time.\n"
                      + "{ind}{ind}The mean (%.1f) is lower than min_iteration_time (%d)\n")
                     % (mean_of_totals, run_id.min_iteration_time), run_id, cmdline)
 
         return terminate
 
     def _get_gauge_adapter_instance(self, run_id):
-        adapter_name = run_id.get_gauge_adapter_name()
-        adapter = instantiate_adapter(adapter_name,
+        adapter_cfg = run_id.get_gauge_adapter()
+        adapter = instantiate_adapter(adapter_cfg,
                                       self._include_faulty,
                                       self)
 
         if adapter is None:
             run_id.fail_immediately()
-            msg = "{ind}Couldn't find gauge adapter: %s\n" % adapter_name
+            msg = "{ind}Couldn't find gauge adapter: %s\n" % run_id.get_gauge_adapter_name()
             self.ui.error_once(msg, run_id)
 
         return adapter
 
     def _generate_data_point(self, cmdline, gauge_adapter, run_id,
                              termination_check):
-        # execute the external program here
+        assert not self._print_execution_plan
+        output = ""
 
         try:
             self.ui.debug_output_info("{ind}Starting run\n", run_id, cmdline)
 
             def _keep_alive(seconds):
                 self.ui.warning(
                     "Keep alive, current job runs for %dmin\n" % (seconds / 60), run_id, cmdline)
@@ -478,23 +514,27 @@
             if err.errno == 2:
                 msg = ("{ind}Failed executing run\n"
                        + "{ind}{ind}It failed with: %s.\n"
                        + "{ind}{ind}File name: %s\n") % (err.strerror, err.filename)
             else:
                 msg = str(err)
             self.ui.error(msg, run_id, cmdline)
+            run_id.report_run_failed(cmdline, 0, output)
             return True
 
         if return_code == 127:
+            run_id.fail_immediately()
             msg = ("{ind}Error: Could not execute %s.\n"
                    + "{ind}{ind}The command was not found.\n"
                    + "{ind}Return code: %d\n"
                    + "{ind}{ind}%s.\n") % (
                        run_id.benchmark.suite.executor.name, return_code, output.strip())
             self.ui.error(msg, run_id, cmdline)
+            run_id.report_run_failed(cmdline, return_code, output)
+            run_id.executable_missing = True
             return True
         elif return_code != 0 and not self._include_faulty and not (
                 return_code == subprocess_timeout.E_TIMEOUT and run_id.ignore_timeouts):
             run_id.indicate_failed_execution()
             run_id.report_run_failed(cmdline, return_code, output)
             if return_code == 126:
                 msg = ("{ind}Error: Could not execute %s.\n"
@@ -502,14 +542,16 @@
                        + "{ind}Return code: %d\n") % (
                            run_id.benchmark.suite.executor.name, return_code)
             elif return_code == subprocess_timeout.E_TIMEOUT:
                 msg = ("{ind}Run timed out.\n"
                        + "{ind}{ind}Return code: %d\n"
                        + "{ind}{ind}max_invocation_time: %s\n") % (
                            return_code, run_id.max_invocation_time)
+            elif return_code is None:
+                msg = "{ind}Run failed. Return code: None\n"
             else:
                 msg = "{ind}Run failed. Return code: %d\n" % return_code
 
             self.ui.error(msg, run_id, cmdline)
 
             if output and output.strip():
                 lines = escape_braces(output).split('\n')
@@ -546,15 +588,19 @@
                     if i >= num_points - num_points_to_show:
                         msg += "{ind}{ind}%4d\t%s%s\n" % (
                             i + 1, data_point.get_total_value(), data_point.get_total_unit())
                 i += 1
 
             run_id.indicate_successful_execution()
             self.ui.verbose_output_info(msg, run_id, cmdline)
-        except ExecutionDeliveredNoResults:
+        except ExecutionDeliveredNoResults as e:
+            if isinstance(e, OutputNotParseable):
+                self.ui.error("{ind}Output of run could not be parsed.\n", run_id, cmdline)
+            elif isinstance(e, ResultsIndicatedAsInvalid):
+                self.ui.error("{ind}Results were marked as invalid.\n", run_id, cmdline)
             run_id.indicate_failed_execution()
             run_id.report_run_failed(cmdline, 0, output)
 
     @staticmethod
     def _check_termination_condition(run_id, termination_check, cmd):
         return termination_check.should_terminate(
             run_id.get_number_of_data_points(), cmd)
```

### Comparing `ReBench-1.1.0/rebench/interop/adapter.py` & `ReBench-1.2.0/rebench/interop/adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 import re
 import pkgutil
 import sys
+from os.path import join
 
 
 class GaugeAdapter(object):
     """A GaugeAdapter implements a common interface to evaluate the output of
        benchmarks and to determine measured performance values.
        The GaugeAdapter class also provides some basic helper functionality.
     """
@@ -35,22 +36,22 @@
 
     def __init__(self, include_faulty, executor):
         self._include_faulty = include_faulty
         self._other_error_definitions = None
         self._executor = executor
 
     def acquire_command(self, run_id):
-        return run_id.cmdline()
+        return run_id.cmdline_for_next_invocation()
 
     def parse_data(self, data, run_id, invocation):
         raise NotImplementedError()
 
     def check_for_error(self, line):
         """Check whether the output line contains one of the common error
-           messages. If its an erroneous run, the result has to be discarded.
+           messages. If it's an erroneous run, the result has to be discarded.
         """
         if self._include_faulty:
             return False
 
         if self.re_error.search(line):
             return True
         if self.re_segfault.search(line):
@@ -78,26 +79,56 @@
     pass
 
 
 class ResultsIndicatedAsInvalid(ExecutionDeliveredNoResults):
     pass
 
 
-def instantiate_adapter(name, include_faulty, executor):
+def instantiate_adapter(adapter_cfg, include_faulty, executor):
+    if isinstance(adapter_cfg, str):
+        return _search_in_rebench_modules(adapter_cfg, include_faulty, executor)
+    return _load_directly(adapter_cfg, include_faulty, executor)
+
+
+def _search_in_rebench_modules(name, include_faulty, executor):
     adapter_name = name + "Adapter"
     root = sys.modules['rebench.interop'].__path__
 
     for _, module_name, _ in pkgutil.walk_packages(root):
         # depending on how ReBench was executed, name might one of the two
         try:
             mod = __import__("rebench.interop." + module_name, fromlist=adapter_name)
         except ImportError:
             try:
                 mod = __import__("interop." + module_name, fromlist=adapter_name)
             except ImportError:
                 mod = None
-        if mod is not None:
-            for key in dir(mod):
-                if key.lower() == adapter_name.lower():
-                    return getattr(mod, key)(include_faulty, executor)
+        adapter_cls = _get_adapter_case_insensitively_from_module(mod, adapter_name)
+        if adapter_cls is not None:
+            return adapter_cls(include_faulty, executor)
+
+    return None
+
+
+def _get_adapter_case_insensitively_from_module(mod, adapter_name):
+    if mod is not None:
+        keys = mod.keys() if isinstance(mod, dict) else dir(mod)
+        for key in keys:
+            if key.lower() == adapter_name.lower():
+                return mod[key] if isinstance(mod, dict) else getattr(mod, key)
+    return None
+
 
+def _load_directly(adapter_cfg, include_faulty, executor):
+    name, path = next(iter(adapter_cfg.items()))
+    full_path = join(executor.config_dir, path)
+    with open(full_path, 'r') as adapter_file:  # pylint: disable=unspecified-encoding
+        file_content = adapter_file.read()
+
+    module_globals = {'__name__': name}
+    code = compile(file_content, full_path, 'exec')
+    exec(code, module_globals)  # pylint: disable=exec-used
+
+    cls = _get_adapter_case_insensitively_from_module(module_globals, name)
+    if cls is not None:
+        return cls(include_faulty, executor)
     return None
```

### Comparing `ReBench-1.1.0/rebench/interop/jmh_adapter.py` & `ReBench-1.2.0/rebench/interop/jmh_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/multivariate_adapter.py` & `ReBench-1.2.0/rebench/interop/multivariate_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/perf_adapter.py` & `ReBench-1.2.0/rebench/interop/perf_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,8 +15,9 @@
         profiler = self._get_profiler(run_id)
         json = profiler.process_profile(run_id, self._executor)
 
         return [ProfileData(run_id, json, run_id.iterations, invocation)]
 
     def acquire_command(self, run_id):
         profiler = self._get_profiler(run_id)
-        return profiler.command + " " + profiler.record_args + " " + run_id.cmdline()
+        return (profiler.command + " " + profiler.record_args + " " +
+                run_id.cmdline_for_next_invocation())
```

### Comparing `ReBench-1.1.0/rebench/interop/perf_parser.py` & `ReBench-1.2.0/rebench/interop/perf_parser.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/plain_seconds_log_adapter.py` & `ReBench-1.2.0/rebench/interop/plain_seconds_log_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/rebench_log_adapter.py` & `ReBench-1.2.0/rebench/interop/rebench_log_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/savina_log_adapter.py` & `ReBench-1.2.0/rebench/interop/savina_log_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/test_adapter.py` & `ReBench-1.2.0/rebench/interop/test_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/test_vm_adapter.py` & `ReBench-1.2.0/rebench/interop/test_vm_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/interop/time_adapter.py` & `ReBench-1.2.0/rebench/interop/time_adapter.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,33 +34,60 @@
 
     # To be sure about how to parse the output, give custom format
     # This avoids issues with perhaps none-standard /bin/usr/time
     time_format = '"max rss (kb): %M\nwall-time (secounds): %e\n"'
     re_formatted_time = re.compile(r"^wall-time \(secounds\): (\d+\.\d+)")
     re_formatted_rss = re.compile(r"^max rss \(kb\): (\d+)")
 
+    _completed_time_availability_check = False
+    _use_formatted_time = False
+    _time_bin = None
+
     def __init__(self, include_faulty, executor):
         GaugeAdapter.__init__(self, include_faulty, executor)
-        self._use_formatted_time = False
+
+    def _create_command(self, command):
+        assert self._completed_time_availability_check
+        if self._use_formatted_time:
+            return "%s -f %s %s" % (self._time_bin, TimeAdapter.time_format, command)
+        else:
+            # use standard, but without info on memory
+            # TODO: add support for reading out memory info on OS X
+            return "/usr/bin/time -p %s" % command
 
     def acquire_command(self, run_id):
-        command = run_id.cmdline()
+        command = run_id.cmdline_for_next_invocation()
+
+        if not self._completed_time_availability_check:
+            self._check_which_time_command_is_available()
+
+        return self._create_command(command)
+
+    def _check_which_time_command_is_available(self):
+        time_bin = '/usr/bin/time'
         try:
             formatted_output = subprocess.call(
-                ['/usr/bin/time', '-f', TimeAdapter.time_format, '/bin/sleep', '1'],
+                ['/usr/bin/time', '-f', TimeAdapter.time_format, '/bin/sleep', '0'],
                 stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         except OSError:
             formatted_output = 1
-        if formatted_output == 0:
-            self._use_formatted_time = True
-            return "/usr/bin/time -f %s %s" % (TimeAdapter.time_format, command)
-        else:
-            # use standard, but without info on memory
-            # TODO: add support for reading out memory info on OS X
-            return "/usr/bin/time -p %s" % command
+
+        if formatted_output == 1:
+            try:
+                formatted_output = subprocess.call(
+                    ['/opt/local/bin/gtime', '-f', TimeAdapter.time_format, '/bin/sleep', '0'],
+                    stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                if formatted_output == 0:
+                    time_bin = '/opt/local/bin/gtime'
+            except OSError:
+                formatted_output = 1
+
+        TimeAdapter._use_formatted_time = formatted_output == 0
+        TimeAdapter._time_bin = time_bin
+        TimeAdapter._completed_time_availability_check = True
 
     def parse_data(self, data, run_id, invocation):
         iteration = 1
         data_points = []
         current = DataPoint(run_id)
         total_measure = None
 
@@ -116,8 +143,8 @@
 
 class TimeManualAdapter(TimeAdapter):
     """TimeManualPerformance works like TimePerformance but does expect the
        user to use the /usr/bin/time manually.
        This is useful for runs on remote machines like the Tilera or ARM boards.
     """
     def acquire_command(self, run_id):
-        return run_id.cmdline()
+        return run_id.cmdline_for_next_invocation()
```

### Comparing `ReBench-1.1.0/rebench/interop/validation_log_adapter.py` & `ReBench-1.2.0/rebench/interop/validation_log_adapter.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/__init__.py` & `ReBench-1.2.0/rebench/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/benchmark.py` & `ReBench-1.2.0/rebench/model/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,7 +103,10 @@
             'suite': self.suite.as_dict()
         }
 
     @classmethod
     def from_str_list(cls, data_store, str_list):
         return data_store.get_config(str_list[0], str_list[1], str_list[2],
                                      None if str_list[3] == '' else str_list[3])
+    @classmethod
+    def get_column_headers(cls):
+        return ["benchmark", "executor", "suite", "extraArgs"]
```

### Comparing `ReBench-1.1.0/rebench/model/benchmark_suite.py` & `ReBench-1.2.0/rebench/model/benchmark_suite.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/build_cmd.py` & `ReBench-1.2.0/rebench/model/build_cmd.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/data_point.py` & `ReBench-1.2.0/rebench/model/data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,7 +72,10 @@
         assert self.invocation == invocation
 
         return {
             'in': invocation,
             'it': iteration,
             'm': data
         }
+
+    def __repr__(self):
+        return "DataPoint(" + str(self.run_id) + ", " + str(self._measurements) + ")"
```

### Comparing `ReBench-1.1.0/rebench/model/executor.py` & `ReBench-1.2.0/rebench/model/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
     def __init__(self, name, path, executable, args, build, description,
                  profiler, run_details, variables, action, env):
         """Specializing the executor details in the run definitions with the settings from
            the executor definitions
         """
         self.name = name
-
         self.path = path
         self.executable = executable
         self.args = args
 
         self.build = build
         self.description = description
         self.profiler = profiler
```

### Comparing `ReBench-1.1.0/rebench/model/exp_run_details.py` & `ReBench-1.2.0/rebench/model/exp_run_details.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/exp_variables.py` & `ReBench-1.2.0/rebench/model/exp_variables.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/experiment.py` & `ReBench-1.2.0/rebench/model/experiment.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/measurement.py` & `ReBench-1.2.0/rebench/model/measurement.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,16 +54,23 @@
         value = float(str_list[2])
         unit = str_list[3]
         criterion = str_list[4]
         run_id = RunId.from_str_list(data_store, str_list[5:])
 
         return Measurement(invocation, iteration, value, unit, run_id,
                            criterion, line_number, filename)
+    @classmethod
+    def get_column_headers(cls):
+        run_id_headers = RunId.get_column_headers()
+        return ["invocation", "iteration", "value", "unit", "criterion"] + run_id_headers
 
     def as_dict(self):
         return {
             'c': self.criterion,
             'in': self.invocation,
             'it': self.iteration,
             'u': self.unit,
             'v': self.value
         }
+
+    def __repr__(self):
+        return "Measurement(%s, %s, %s)" % (self.value, self.unit, self.criterion)
```

### Comparing `ReBench-1.1.0/rebench/model/profile_data.py` & `ReBench-1.2.0/rebench/model/profile_data.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/profiler.py` & `ReBench-1.2.0/rebench/model/profiler.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/reporting.py` & `ReBench-1.2.0/rebench/model/reporting.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/model/run_id.py` & `ReBench-1.2.0/rebench/model/run_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,23 @@
             self.statistics = SampleCounter()
         else:
             self.statistics = StatisticProperties()
         self.total_unit = None
 
         self._termination_check = None
         self._cmdline = None
+        self.executable = None
+        self.executable_missing = False
         self.is_failed = True
 
         self._max_invocation = 0
 
+    def has_same_executable(self, other):
+        return self.executable == other.executable
+
     @property
     def warmup_iterations(self):
         return self.benchmark.run_details.warmup
 
     @property
     def min_iteration_time(self):
         return self.benchmark.run_details.min_iteration_time
@@ -106,21 +111,30 @@
 
     @property
     def location(self):
         if not self.benchmark.suite.location:
             return None
         return self._expand_vars(self.benchmark.suite.location)
 
-    def get_gauge_adapter_name(self):
+    def get_gauge_adapter(self):
         if self.is_profiling():
             # TODO: needs changing once we want to support different profilers
             perf_profile = self.benchmark.suite.executor.profiler[0]
             return perf_profile.gauge_adapter_name
         return self.benchmark.gauge_adapter
 
+    def get_gauge_adapter_name(self):
+        if self.is_profiling():
+            return self.get_gauge_adapter()
+
+        adapter = self.benchmark.gauge_adapter
+        if isinstance(adapter, str):
+            return adapter
+        return next(iter(adapter))  # get the first key in the dict
+
     def is_profiling(self):
         return self.benchmark.suite.executor.action == "profile"
 
     def build_commands(self):
         commands = set()
         builds = self.benchmark.suite.executor.build
         if builds:
@@ -231,14 +245,18 @@
     def _expand_vars(self, string):
         try:
             return string % {'benchmark': self.benchmark.command,
                              'cores': self.cores_as_str,
                              'executor': self.benchmark.suite.executor.name,
                              'input': self.input_size_as_str,
                              'iterations': self.iterations,
+
+                             # the invocation number needs to be set right before execution
+                             # we don't know it here, and it would change the RunId identity
+                             'invocation': '%(invocation)s',
                              'suite': self.benchmark.suite.name,
                              'variable': self.var_value_as_str,
                              'machine': self.machine_as_str,
                              'warmup': self.benchmark.run_details.warmup}
         except ValueError as err:
             self._report_format_issue_and_exit(string, err)
             return None
@@ -254,14 +272,18 @@
             raise UIError(msg, err)
 
     def cmdline(self):
         if self._cmdline:
             return self._cmdline
         return self._construct_cmdline()
 
+    def cmdline_for_next_invocation(self):
+        """Replace the invocation number in the command line"""
+        return self.cmdline() % {'invocation': self.completed_invocations + 1}
+
     def _construct_cmdline(self):
         cmdline = ""
         if self.benchmark.suite.executor.path:
             cmdline = self.benchmark.suite.executor.path + "/"
 
         cmdline += self.benchmark.suite.executor.executable
 
@@ -272,14 +294,15 @@
 
         if self.benchmark.extra_args:
             cmdline += " " + str(self.benchmark.extra_args)
 
         cmdline = self._expand_vars(cmdline)
 
         self._cmdline = cmdline.strip()
+        self.executable = cmdline.split(' ')[0]
         return self._cmdline
 
     def __eq__(self, other):
         return (isinstance(other, self.__class__) and
                 self.cmdline() == other.cmdline())
 
     def __ne__(self, other):
@@ -308,31 +331,37 @@
         result.append(self.input_size_as_str)
         result.append(self.var_value_as_str)
         result.append(self.machine_as_str)
 
         return result
 
     def as_dict(self):
+        extra_args = self.benchmark.extra_args
         return {
             'benchmark': self.benchmark.as_dict(),
             'cores': self.cores,
             'inputSize': self.input_size,
             'varValue': self.var_value,
             'machine': self.machine,
-            'extraArgs': str(self.benchmark.extra_args),
+            'extraArgs': extra_args if extra_args is None else str(extra_args),
             'cmdline': self.cmdline(),
             'location': self.location
         }
 
     @classmethod
     def from_str_list(cls, data_store, str_list):
         benchmark = Benchmark.from_str_list(data_store, str_list[:-4])
         return data_store.create_run_id(
             benchmark, str_list[-4], str_list[-3], str_list[-2], str_list[-1])
 
+    @classmethod
+    def get_column_headers(cls):
+        benchmark_headers = Benchmark.get_column_headers()
+        return benchmark_headers + ["cores", "inputSize", "varValue", "machine"]
+
     def __str__(self):
         return "RunId(%s, %s, %s, %s, %s, %s, %d)" % (
             self.benchmark.name,
             self.cores,
             self.benchmark.extra_args,
             self.input_size or '',
             self.var_value  or '',
```

### Comparing `ReBench-1.1.0/rebench/model/termination_check.py` & `ReBench-1.2.0/rebench/model/termination_check.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/persistence.py` & `ReBench-1.2.0/rebench/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,39 +300,45 @@
         if measurement.is_total():
             run_id.loaded_data_point(data_point,
                                      (measurement.iteration <= run_id.warmup_iterations
                                       if run_id.warmup_iterations else False))
             data_point = DataPoint(run_id)
         return data_point, previous_run_id
 
+    _SEP = "\t"  # separator between serialized parts of a measurement
+
     def _open_file_and_append_execution_comment(self):
         """
         Append a shebang (#!/path/to/executable) to the data file.
         This allows it theoretically to be executable.
         But more importantly also records execution metadata to reproduce the data.
         """
-        shebang_line = "#!%s\n" % (subprocess.list2cmdline(sys.argv))
-        shebang_line += _START_TIME_LINE + self._start_time + "\n"
-        shebang_line += "# Environment: " + json.dumps(determine_environment()) + "\n"
-        shebang_line += "# Source: " + json.dumps(
+        shebang_with_metadata = "#!%s\n" % (subprocess.list2cmdline(sys.argv))
+        shebang_with_metadata += _START_TIME_LINE + self._start_time + "\n"
+        shebang_with_metadata += "# Environment: " + json.dumps(determine_environment()) + "\n"
+        shebang_with_metadata += "# Source: " + json.dumps(
             determine_source_details(self._configurator)) + "\n"
 
+        csv_header = self._SEP.join(Measurement.get_column_headers()) + "\n"
+
         try:
             # pylint: disable-next=unspecified-encoding,consider-using-with
             data_file = open(self._data_filename, 'a+')
-            data_file.write(shebang_line)
+            is_empty = data_file.tell() == 0
+            data_file.write(shebang_with_metadata)
+            if is_empty:
+                data_file.write(csv_header)
             data_file.flush()
             return data_file
         except Exception as err:  # pylint: disable=broad-except
             raise UIError(
                 "Error: Was not able to open data file for writing.\n{ind}%s\n%s\n" % (
                     os.getcwd(), err),
                 err)
 
-    _SEP = "\t"  # separator between serialized parts of a measurement
 
     def _persists_data_point_in_open_file(self, data_point):
         for measurement in data_point.get_measurements():
             line = self._SEP.join(measurement.as_str_list())
             self._file.write(line + "\n")
 
     def persist_data_point(self, data_point):
```

### Comparing `ReBench-1.1.0/rebench/rebench-schema.yml` & `ReBench-1.2.0/rebench/rebench-schema.yml`

 * *Files 2% similar despite different names*

```diff
@@ -189,18 +189,20 @@
     - type: str
 
 schema;benchmark_suite_type:
   type: map
   mapping:
     <<: [ *EXP_RUN_DETAILS, *EXP_VARIABLES ]
     gauge_adapter:
-      type: str
+      type: any
       required: true
       desc: |
-        Name of the parser that interpreters the output of the benchmark harness
+        Either the name of the parser that interpreters the output of the benchmark harness,
+        or a map with one element, which is the name of the parser and the path
+        to the Python file with a custom parser.
     command:
       type: str
       required: true
       desc: |
         The command for the benchmark harness. It's going to be combined with the
         executor's command line. It supports various format variables, including:
          - benchmark (the benchmark's name)
```

### Comparing `ReBench-1.1.0/rebench/rebench.py` & `ReBench-1.2.0/rebench/rebench.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2.7
+#!/usr/bin/env python3
 # ReBench is a tool to run and document benchmarks.
 #
 # It is inspired by JavaStats implemented by Andy Georges.
 # JavaStats can be found here: http://www.elis.ugent.be/en/JavaStats
 #
 # ReBench goes beyond the goals of JavaStats, not only by broadening the scope
 # to not only Java VMs, but also by introducing facilities to evaluate
@@ -50,15 +50,15 @@
         self.version = rebench_version
         self.options = None
         self._config = None
         self.ui = UI()
 
     def shell_options(self):
         usage = """%(prog)s [options] <config> [exp_name] [e:$]* [s:$]* [m:$]*
-        
+
 Argument:
   config    required argument, file containing the experiment to be executed
   exp_name  optional argument, the name of an experiment definition
             from the config file
             If not provided, the configured default_experiment is used.
             If 'all' is given, all experiments will be executed.
 
@@ -121,14 +121,19 @@
                  'batch, round-robin, random [default: %(default)s]')
         execution.add_argument(
             '-E', '--no-execution', action='store_true', dest='no_execution',
             default=False,
             help='Disables execution.'
                  ' It allows to verify the configuration file and other parameters.')
         execution.add_argument(
+            '-D', '--no-denoise', action='store_false', dest='use_denoise',
+            default=True,
+            help='Disable use of denoise, and thus, ' +
+                 ' do not try to minimize interference from the system during benchmarking.')
+        execution.add_argument(
             '-p', '--execution-plan', action='store_true', dest='execution_plan',
             default=False,
             help='Print execution plan.'
                  ' This outputs all executions that would be performed, without executing them.')
 
         data = parser.add_argument_group(
             'Data and Reporting',
@@ -252,46 +257,50 @@
             raise UIError(exc.args[0] + "\n", exc)
 
         if args.report_completion:
             return self._report_completion()
 
         runs = self._config.get_runs()
         does_profiling = any(r.is_profiling() for r in runs)
-
-        denoise_result = None
-        show_denoise_warnings = not (self._config.artifact_review
-                                     or self._config.options.execution_plan)
-
-        try:
-            denoise_result = minimize_noise(show_denoise_warnings, self.ui, does_profiling)
-            init_environment(denoise_result, self.ui)
-
-            data_store.load_data(runs, self._config.options.do_rerun)
-
-            use_nice = denoise_result.use_nice
-            use_shielding = denoise_result.use_shielding
-
-            return self.execute_experiment(runs, use_nice, use_shielding)
-        finally:
-            restore_noise(denoise_result, show_denoise_warnings, self.ui)
+        if not self._config.options.use_denoise:
+            return self.load_data_and_execute_experiments(runs, data_store, False, False, None)
+        else:
+            denoise_result = None
+            show_denoise_warnings = not (self._config.artifact_review
+                                         or self._config.options.execution_plan)
+            try:
+                denoise_result = minimize_noise(show_denoise_warnings, self.ui, does_profiling)
+                use_nice = denoise_result.use_nice
+                use_shielding = denoise_result.use_shielding
+                return self.load_data_and_execute_experiments(
+                    runs, data_store, use_nice, use_shielding, denoise_result)
+            finally:
+                restore_noise(denoise_result, show_denoise_warnings, self.ui)
+
+    def load_data_and_execute_experiments(self, runs, data_store,
+                                          use_nice, use_shielding, denoise_result):
+        init_environment(denoise_result, self.ui)
+        data_store.load_data(runs, self._config.options.do_rerun)
+        return self.execute_experiment(runs, use_nice, use_shielding)
 
     def execute_experiment(self, runs, use_nice, use_shielding):
         self.ui.verbose_output_info("Execute experiment: " + self._config.experiment_name + "\n")
 
         scheduler_class = {'batch':       BatchScheduler,
                            'round-robin': RoundRobinScheduler,
                            'random':      RandomScheduler}.get(self._config.options.scheduler)
 
         executor = Executor(runs, self._config.do_builds,
                             self.ui,
                             self._config.options.include_faulty,
                             self._config.options.debug,
                             scheduler_class,
                             self._config.build_log, self._config.artifact_review,
-                            use_nice, use_shielding, self._config.options.execution_plan)
+                            use_nice, use_shielding, self._config.options.execution_plan,
+                            self._config.config_dir)
 
         if self._config.options.no_execution:
             return True
         else:
             if self._config.artifact_review:
                 self.ui.output("Executing benchmarks for Artifact Review"
                                 + " using the reported settings.")
```

### Comparing `ReBench-1.1.0/rebench/rebenchdb.py` & `ReBench-1.2.0/rebench/rebenchdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 import json
 from datetime import datetime
 from time import sleep
 
-from .ui import UIError
-
-try:
-    from http.client import HTTPException
-    from urllib.request import urlopen, Request as PutRequest
-except ImportError:
-    # Python 2.7
-    from httplib import HTTPException
-    from urllib2 import urlopen, Request
-
-
-    class PutRequest(Request):
-        def __init__(self, *args, **kwargs):
-            if 'method' in kwargs:
-                del kwargs['method']
-            Request.__init__(self, *args, **kwargs)
+from http.client import HTTPException
+from urllib.request import urlopen, Request as PutRequest
 
-        def get_method(self, *_args, **_kwargs):  # pylint: disable=arguments-differ
-            return 'PUT'
+from .ui import UIError
 
 
 def get_current_time():
     """Return the current time as string for use with ReBenchDB and other persistency backends."""
     return datetime.utcnow().isoformat() + "+00:00"
 
 
@@ -73,18 +58,17 @@
 
         return success, response
 
     @staticmethod
     def _send_payload(payload, url):
         req = PutRequest(url, payload,
                          {'Content-Type': 'application/json'}, method='PUT')
-        socket = urlopen(req)
-        response = socket.read()
-        socket.close()
-        return response
+        with urlopen(req) as socket:
+            response = socket.read()
+            return response
 
     def _send_to_rebench_db(self, payload_data, operation):
         payload_data['projectName'] = self._project_name
         payload_data['experimentName'] = self._experiment_name
         url = self._server_base_url + operation
 
         payload = json.dumps(payload_data, separators=(',', ':'), ensure_ascii=True)
```

### Comparing `ReBench-1.1.0/rebench/reporter.py` & `ReBench-1.2.0/rebench/reporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,34 +13,25 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-from __future__ import with_statement
-
 from time import time
 from operator import itemgetter
 import json
 import re
 
+from http.client import HTTPException
+from urllib.request import urlopen
+from urllib.parse import urlencode
 from humanfriendly.tables import format_pretty_table
 
 
-try:
-    from http.client import HTTPException
-    from urllib.request import urlopen
-    from urllib.parse import urlencode
-except ImportError:
-    from httplib import HTTPException
-    from urllib import urlencode # pylint: disable=ungrouped-imports
-    from urllib2 import urlopen
-
-
 class Reporter(object):
 
     def __init__(self):
         self._job_completion_reported = False
 
     def run_failed(self, _run_id, _cmdline, _return_code, _output):
         pass
@@ -205,18 +196,17 @@
                        'extra_args'  : run_id.benchmark.extra_args}
 
         result['benchmark'] = name
 
         return result
 
     def _send_payload(self, payload):
-        socket = urlopen(self._cfg.url, payload)
-        response = socket.read()
-        socket.close()
-        return response
+        with urlopen(self._cfg.url, payload) as socket:
+            response = socket.read()
+            return response
 
     def _send_to_codespeed(self, results, run_id):
         payload = urlencode({'json': json.dumps(results)})
 
         try:
             self._send_payload(payload)
         except (IOError, HTTPException):
```

### Comparing `ReBench-1.1.0/rebench/statistics.py` & `ReBench-1.2.0/rebench/statistics.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/subprocess_kill.py` & `ReBench-1.2.0/rebench/subprocess_kill.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,17 @@
 from os         import kill
 from signal     import SIGKILL
 from subprocess import PIPE, Popen
 
-IS_PY3 = None
-
-try:
-    _ = ProcessLookupError
-    IS_PY3 = True
-except NameError:
-    IS_PY3 = False
 
 # Indicate timeout with standard exit code
 E_TIMEOUT = -9
 
 
-def _kill_py2(proc_id, uses_sudo):
-    if uses_sudo:
-        from .denoise import deliver_kill_signal  # pylint: disable=import-outside-toplevel
-
-        deliver_kill_signal(proc_id)
-        return
-
-    try:
-        kill(proc_id, SIGKILL)
-    except IOError:
-        # there's a race condition, the process may have already terminated on its own
-        # so let's simply ignore it
-        pass
-
-
-def _kill_py3(proc_id, uses_sudo):
+def _kill(proc_id, uses_sudo):
     if uses_sudo:
         from .denoise import deliver_kill_signal  # pylint: disable=import-outside-toplevel
 
         deliver_kill_signal(proc_id)
         return
 
     try:
@@ -46,18 +24,15 @@
 
 def kill_process(pid, recursively, thread, uses_sudo):
     pids = [pid]
     if recursively:
         pids.extend(_get_process_children(pid))
 
     for proc_id in pids:
-        if IS_PY3:
-            _kill_py3(proc_id, uses_sudo)
-        else:
-            _kill_py2(proc_id, uses_sudo)
+        _kill(proc_id, uses_sudo)
 
     if thread:
         thread.join()
         return E_TIMEOUT, thread.stdout_result, thread.stderr_result
     return E_TIMEOUT, None, None
```

### Comparing `ReBench-1.1.0/rebench/subprocess_with_timeout.py` & `ReBench-1.2.0/rebench/subprocess_with_timeout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,27 @@
-from __future__ import print_function
-
 from select     import select
 from subprocess import PIPE, STDOUT, Popen
 from threading  import Thread, Condition
 from time       import time
 
 import sys
 import signal
 
 from .subprocess_kill import kill_process
 
-IS_PY3 = None
-
-try:
-    _ = ProcessLookupError
-    IS_PY3 = True
-except NameError:
-    IS_PY3 = False
 
 # Indicate timeout with standard exit code
 E_TIMEOUT = -9
 
-if IS_PY3:
-    def output_as_str(string_like):
-        if string_like is not None and type(string_like) != str:  # pylint: disable=unidiomatic-typecheck
-            return string_like.decode('utf-8')
-        else:
-            return string_like
-else:
-    def output_as_str(string_like):
-        if string_like is not None and type(string_like) == str:  # pylint: disable=unidiomatic-typecheck
-            return string_like.decode('utf-8')
-        else:
-            return string_like
+
+def output_as_str(string_like):
+    if string_like is not None and type(string_like) != str:  # pylint: disable=unidiomatic-typecheck
+        return string_like.decode('utf-8')
+    else:
+        return string_like
 
 _signals_setup = False
 
 
 def keyboard_interrupt_on_sigterm(signum, frame):
     raise KeyboardInterrupt()
```

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_111_report_ignores_warmup_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_111_report_ignores_warmup_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_112_invocations_setting_ignored_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_112_invocations_setting_ignored_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_117_input_size_setting_ignored_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_117_input_size_setting_ignored_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_27_invalid_run_not_handled_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_27_invalid_run_not_handled_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_4_run_equality_and_params_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_4_run_equality_and_params_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/bugs/issue_54_extra_args_test.py` & `ReBench-1.2.0/rebench/tests/bugs/issue_54_extra_args_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/ignore_timeouts_test.py` & `ReBench-1.2.0/rebench/tests/features/ignore_timeouts_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_110_setup_run_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_110_setup_run_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_15_warm_up_support_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_15_warm_up_support_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_169_config_composition_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_169_config_composition_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_16_multiple_data_points_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_216_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2009-2014 Stefan Marr <http://www.stefan-marr.de/>
+# Copyright (c) 2023 Naomi Grew, Stefan Marr
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to
 # deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,48 +20,34 @@
 from ...configurator           import Configurator, load_config
 from ...executor               import Executor
 from ...persistence            import DataStore
 from ..persistence import TestPersistence
 from ..rebench_test_case import ReBenchTestCase
 
 
-class Issue16MultipleDataPointsTest(ReBenchTestCase):
-    """
-    Add support to record multiple data points for same benchmark in one run.
-      - multiple measurements
-      - as well as multiple data points
-    """
+class Issue216CurrentInvocation(ReBenchTestCase):
 
     def setUp(self):
-        super(Issue16MultipleDataPointsTest, self).setUp()
+        super(Issue216CurrentInvocation, self).setUp()
         self._set_path(__file__)
 
     def _records_data_points(self, exp_name, num_data_points):
-        cnf = Configurator(load_config(self._path + '/issue_16.conf'), DataStore(self.ui),
+        cnf = Configurator(load_config(self._path + '/issue_216.conf'), DataStore(self.ui),
                            self.ui, exp_name=exp_name,
                            data_file=self._tmp_file)
-        runs = cnf.get_runs()
+        runs = list(cnf.get_runs())
+        self.assertEqual(1, len(runs))
+
         persistence = TestPersistence()
-        for run in runs:
-            run.add_persistence(persistence)
-        ex = Executor(cnf.get_runs(), False, self.ui)
+        persistence.use_on(runs)
+        ex = Executor(runs, False, self.ui)
         ex.execute()
-        self.assertEqual(1, len(cnf.get_runs()))
-        run = next(iter(cnf.get_runs()))
+
+        run = runs[0]
         self.assertEqual(num_data_points, run.get_number_of_data_points())
         return persistence.get_data_points()
 
-    def test_records_multiple_data_points_from_single_execution_10(self):
-        self._records_data_points('Test1', 10)
-
-    def test_records_multiple_data_points_from_single_execution_20(self):
-        self._records_data_points('Test2', 20)
-
     def test_associates_measurements_and_data_points_correctly(self):
-        data_points = self._records_data_points('Test1', 10)
-        for point, i in zip(data_points, list(range(0, 10))):
-            self.assertEqual(4, point.number_of_measurements())
-
-            for criterion, measurement in zip(["bar", "baz", "foo", "total"],
-                                              point.get_measurements()):
-                self.assertEqual(criterion, measurement.criterion)
-                self.assertEqual(i, int(measurement.value))
+        data_points = self._records_data_points('Test', 4)
+        for point, i in zip(data_points, range(4)):
+            self.assertEqual(1, len(point.get_measurements()))
+            self.assertEqual(i + 1, int(point.get_measurements()[0].value))
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_19_one_data_point_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_19_one_data_point_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
-
 from ...configurator     import Configurator, load_config
 from ...executor         import Executor, RoundRobinScheduler
 from ...persistence      import DataStore
 from ...reporter         import Reporter
 from ..rebench_test_case import ReBenchTestCase
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_31_multivariate_data_points_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_31_multivariate_data_points_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
-
 from ...configurator           import Configurator, load_config
 from ...executor               import Executor
 from ...persistence            import DataStore
 from ..persistence import TestPersistence
 from ..rebench_test_case import ReBenchTestCase
 
 
@@ -37,16 +35,15 @@
 
     def _records_data_points(self, exp_name, num_data_points):
         cnf = Configurator(load_config(self._path + '/issue_31.conf'), DataStore(self.ui),
                            self.ui, exp_name=exp_name,
                            data_file=self._tmp_file)
         runs = cnf.get_runs()
         persistence = TestPersistence()
-        for run in runs:
-            run.add_persistence(persistence)
+        persistence.use_on(runs)
 
         ex = Executor(runs, False, self.ui)
         ex.execute()
         self.assertEqual(1, len(cnf.get_runs()))
         run = next(iter(cnf.get_runs()))
         self.assertEqual(num_data_points, run.get_number_of_data_points())
         return persistence.get_data_points()
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_32_jmh_support_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_32_jmh_support_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_34_accept_faulty_runs_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_34_accept_faulty_runs_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_42_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_42_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
 import os
 import unittest
 from unittest import skip
 
 from ...configurator import Configurator, load_config
 from ...executor import Executor
+from ...interop.time_adapter import TimeManualAdapter
 from ...persistence import DataStore
 from ...reporter import Reporter
 from ..rebench_test_case import ReBenchTestCase
 
 
 class _TestFailedReporter(Reporter):
 
@@ -126,14 +126,32 @@
         ex.execute()
 
         log = self._read_log()
         parts = log.split('|', 2)
         self.assertEqual("E:exe-with-build-but-not-env", parts[0])
         self._assert_empty_standard_env(parts[1])
 
+    def test_construct_cmdline_env_vars_set_as_expected(self):
+        cnf = Configurator(load_config(self._path + '/issue_42.conf'), DataStore(self.ui),
+                           self.ui, data_file=self._tmp_file, exp_name='test-set-as-expected')
+        runs = list(cnf.get_runs())
+        ex = Executor(runs, True, self.ui, use_nice=True, use_shielding=True)
+
+        self.assertIn(" --preserve-env=IMPORTANT_ENV_VARIABLE,ALSO_IMPORTANT rebench-denoise",
+                      ex._construct_cmdline(runs[0], TimeManualAdapter(False, ex)))
+
+    def test_construct_cmdline_build_with_env(self):
+        cnf = Configurator(load_config(self._path + '/issue_42.conf'), DataStore(self.ui),
+                           self.ui, data_file=self._tmp_file, exp_name='build-with-env')
+        runs = list(cnf.get_runs())
+        ex = Executor(runs, True, self.ui, use_nice=True, use_shielding=True)
+
+        self.assertIn(" --preserve-env=VAR1,VAR3 rebench-denoise",
+                      ex._construct_cmdline(runs[0], TimeManualAdapter(False, ex)))
+
     def _assert_empty_standard_env(self, log_remainder):
         env_parts = log_remainder.split(':')
         self.assertEqual("STD", env_parts[0])
 
         env = sorted(env_parts[1].split('\n'))
         self.assertEqual('', env[0])
         self.assertTrue(env[1].startswith("PWD="))
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_42_vm.py` & `ReBench-1.2.0/rebench/tests/features/issue_42_vm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # simple script emulating an executor generating benchmark results
-from __future__ import print_function
-
 import random
 import os
 import sys
 
 test = sys.argv[2]
 
 env = os.environ.items()
 env = sorted(env, key=lambda el: el[0])
 print(test)
 print(env)
 
 known_envvars = ["PWD", "SHLVL", "VERSIONER_PYTHON_VERSION",
-                 "_", "__CF_USER_TEXT_ENCODING", "LC_CTYPE"]
+                 "_", "__CF_USER_TEXT_ENCODING", "LC_CTYPE",
+                 "CPATH", "LIBRARY_PATH", "MANPATH", "SDKROOT"]
 
 if test == "as-expected":
     if os.environ.get("IMPORTANT_ENV_VARIABLE", None) != "exists":
         sys.exit(1)
 
     if os.environ.get("ALSO_IMPORTANT", None) != "3":
         sys.exit(1)
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_57_binary_on_path_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_57_binary_on_path_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_58_build_vm_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_58_build_vm_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
 import os
 
 from ...configurator     import Configurator, load_config
 from ...executor         import Executor
 from ...persistence      import DataStore
 from ..rebench_test_case import ReBenchTestCase
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_59_build_suite_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_59_build_suite_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
 import os
 
 from ...configurator     import Configurator, load_config
 from ...executor         import Executor
 from ...persistence      import DataStore
 from ..rebench_test_case import ReBenchTestCase
```

### Comparing `ReBench-1.1.0/rebench/tests/features/issue_81_unicode_test.py` & `ReBench-1.2.0/rebench/tests/features/issue_81_unicode_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
-from __future__ import print_function
 import os
 
 from codecs import open as open_with_enc
 
 from ...configurator     import Configurator, load_config
 from ...executor         import Executor
 from ...persistence      import DataStore
@@ -49,18 +48,15 @@
         self.assertEqual(2, runs[0].get_number_of_data_points())
 
         self.assertTrue(os.path.exists(self._path + '/build.log'))
 
         with open_with_enc(self._path + '/build.log', 'r', encoding='utf-8') as build_file:
             log = build_file.read()
 
-        try:
-            unicode_char = unichr(22234)
-        except NameError:
-            unicode_char = chr(22234)
+        unicode_char = chr(22234)
 
         self.assertGreaterEqual(15, log.find(unicode_char))  # Executor:VM1|STD:
         self.assertGreaterEqual(log.find(unicode_char, 16), 36)  # Executor:VM1|ERR:
 
         self.assertGreaterEqual(log.find(unicode_char, 42), 61)  # S:Suite1|STD:
         self.assertGreaterEqual(log.find(unicode_char, 70), 86)  # S:Suite1|ERR:
```

### Comparing `ReBench-1.1.0/rebench/tests/interop/adapter_test.py` & `ReBench-1.2.0/rebench/tests/interop/adapter_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/interop/plain_seconds_log_adapter_test.py` & `ReBench-1.2.0/rebench/tests/interop/plain_seconds_log_adapter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ...interop.plain_seconds_log_adapter import PlainSecondsLogAdapter
 
 
 class PlainSecondsAdapterTest(TestCase):
 
     def test_acquire_command(self):
         class _TestRunId(object):
-            def cmdline(self):
+            def cmdline_for_next_invocation(self):
                 return "FOO"
         adapter = PlainSecondsLogAdapter(False, None)
         cmd = adapter.acquire_command(_TestRunId())
         self.assertEqual("FOO", cmd)
 
     def test_parse_data(self):
         data = """100
```

### Comparing `ReBench-1.1.0/rebench/tests/interop/rebench_log_adapter_test.py` & `ReBench-1.2.0/rebench/tests/interop/rebench_log_adapter_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/interop/time_adapter_test.py` & `ReBench-1.2.0/rebench/tests/interop/time_adapter_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 from unittest import TestCase
 
 from ...interop.adapter      import OutputNotParseable
 from ...interop.time_adapter import TimeAdapter, TimeManualAdapter
 
 
 class _TestRunId(object):
-    def cmdline(self):
+    def cmdline_for_next_invocation(self):
         return "FOO"
 
 
 class TimeAdapterTest(TestCase):
 
     def test_acquire_command(self):
         adapter = TimeAdapter(False, None)
         cmd = adapter.acquire_command(_TestRunId())
-        self.assertTrue(cmd.startswith("/usr/bin/time"))
+        self.assertRegex(cmd, r"^/.*/bin/g?time")
 
     def test_parse_data(self):
         data = """real        11.00
 user         5.00
 sys          1.00"""
         adapter = TimeAdapter(False, None)
+        TimeAdapter._use_formatted_time = False
         data = adapter.parse_data(data, None, 1)
         self.assertEqual(1, len(data))
 
         measurements = data[0].get_measurements()
         self.assertEqual(3, len(measurements))
         self.assertEqual(11000, data[0].get_total_value())
```

### Comparing `ReBench-1.1.0/rebench/tests/model/runs_config_test.py` & `ReBench-1.2.0/rebench/tests/model/runs_config_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/perf/issue_166_profiling_test.py` & `ReBench-1.2.0/rebench/tests/perf/issue_166_profiling_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/tests/perf/perf_parser_test.py` & `ReBench-1.2.0/rebench/tests/perf/perf_parser_test.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/rebench/ui.py` & `ReBench-1.2.0/rebench/ui.py`

 * *Files identical despite different names*

### Comparing `ReBench-1.1.0/setup.py` & `ReBench-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,35 +23,30 @@
 
 from setuptools import setup, find_packages
 from rebench import __version__ as rebench_version
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-if sys.version_info[0] < 3:
-    pykwalify_version = 'pykwalify==1.7.0'
-else:
-    pykwalify_version = 'pykwalify>=1.8.0'
-
 setup(name='ReBench',
       version=rebench_version,
       description='Execute and document benchmarks reproducibly.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Stefan Marr',
       author_email='rebench@stefan-marr.de',
       url='https://github.com/smarr/ReBench',
       packages=find_packages(exclude=['*.tests']),
       package_data={'rebench': ['rebench-schema.yml']},
       install_requires=[
-          'PyYAML>=3.12',
-          pykwalify_version,
-          'humanfriendly>=8.0',
-          'py-cpuinfo==7.0.0',
-          'psutil>=5.6.7'
+          'PyYAML>=6.0',
+          'pykwalify>=1.8.0',
+          'humanfriendly>=10.0',
+          'py-cpuinfo==9.0.0',
+          'psutil>=5.9.5'
       ],
       entry_points = {
           'console_scripts' : [
               'rebench = rebench.rebench:main_func',
               'rebench-denoise = rebench.denoise:main_func'
           ]
       },
```

