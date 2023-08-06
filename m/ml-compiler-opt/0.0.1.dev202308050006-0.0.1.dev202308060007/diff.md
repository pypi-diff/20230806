# Comparing `tmp/ml-compiler-opt-0.0.1.dev202308050006.tar.gz` & `tmp/ml-compiler-opt-0.0.1.dev202308060007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202308050006.tar", last modified: Sat Aug  5 00:06:46 2023, max compression
+gzip compressed data, was "ml-compiler-opt-0.0.1.dev202308060007.tar", last modified: Sun Aug  6 00:07:46 2023, max compression
```

## Comparing `ml-compiler-opt-0.0.1.dev202308050006.tar` & `ml-compiler-opt-0.0.1.dev202308060007.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.908521 ml-compiler-opt-0.0.1.dev202308050006/
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-05 00:06:46.908521 ml-compiler-opt-0.0.1.dev202308050006/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.896521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.896521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_chromium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_llvm_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmarking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/filter_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/gtest_executable_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/list_gtests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.896521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/buffered_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/buffered_scheduler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.896521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/local_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/local_worker_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.896521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48871 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/blackbox_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/blackbox_optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/gradient_ascent_optimization_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/policy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/policy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/package_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.900521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/agent_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/best_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/best_trajectory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/compilation_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/compilation_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant_value_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant_value_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_reader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.904521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_collect_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_eval_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_reverb_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_train_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/feature_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/feature_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/gin_external_configurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.904521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/inlining_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/local_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/local_data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/log_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/policy_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/policy_saver_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/problem_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/random_net_distillation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/random_net_distillation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.904521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.904521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/train_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/train_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.908521 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_default_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_default_trace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_test_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/merge_best_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:06:46.908521 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-05 00:06:46.000000 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-05 00:06:46.000000 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:06:46.000000 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 00:06:46.000000 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 00:06:46.000000 ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 00:06:32.000000 ml-compiler-opt-0.0.1.dev202308050006/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:06:46.908521 ml-compiler-opt-0.0.1.dev202308050006/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.427978 ml-compiler-opt-0.0.1.dev202308060007/
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-06 00:07:46.427978 ml-compiler-opt-0.0.1.dev202308060007/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.411977 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.411977 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_llvm_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmarking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/filter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/gtest_executable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/list_gtests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.411977 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/buffered_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/buffered_scheduler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.411977 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/local_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/local_worker_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.415977 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48871 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/blackbox_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/blackbox_optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/gradient_ascent_optimization_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/policy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/policy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/package_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.419978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/agent_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/best_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/best_trajectory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/compilation_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/compilation_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant_value_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant_value_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_reader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.419978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_collect_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_eval_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_reverb_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_train_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/feature_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/feature_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/gin_external_configurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.419978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/inlining_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/local_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/local_data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/log_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/policy_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/policy_saver_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/problem_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/random_net_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/random_net_distillation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.423978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.423978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/train_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/train_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.423978 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_default_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_default_trace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_test_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/merge_best_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:07:46.427978 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-06 00:07:46.000000 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-06 00:07:46.000000 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:07:46.000000 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-06 00:07:46.000000 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 00:07:46.000000 ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-06 00:07:13.000000 ml-compiler-opt-0.0.1.dev202308060007/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:07:46.427978 ml-compiler-opt-0.0.1.dev202308060007/setup.cfg
```

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/LICENSE` & `ml-compiler-opt-0.0.1.dev202308060007/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202308060007/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202308050006
+Version: 0.0.1.dev202308060007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/README.md` & `ml-compiler-opt-0.0.1.dev202308060007/README.md`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_chromium.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_chromium.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_llvm_test_suite.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_llvm_test_suite.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report_converter.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report_converter.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmark_report_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmark_report_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/benchmarking_utils.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/filter_tests.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/filter_tests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/gtest_executable_utils.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/gtest_executable_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/benchmark/list_gtests.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/benchmark/list_gtests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/buffered_scheduler.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/buffered_scheduler.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/buffered_scheduler_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/buffered_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/local_worker_manager.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/local_worker_manager.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/local/local_worker_manager_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/local/local_worker_manager_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/worker.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/distributed/worker_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/distributed/worker_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/blackbox_optimizers.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/blackbox_optimizers.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/blackbox_optimizers_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/blackbox_optimizers_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/gradient_ascent_optimization_algorithms.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/gradient_ascent_optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/policy_utils.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/policy_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/es/policy_utils_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/es/policy_utils_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/package_config.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/package_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/agent_config.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/agent_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/agent_config_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/agent_config_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/best_trajectory_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/best_trajectory_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/compilation_runner.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/compilation_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/compilation_runner_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/compilation_runner_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant_value_network.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant_value_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/constant_value_network_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/constant_value_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/corpus.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_collector.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_reader.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/data_reader_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/data_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/agent.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/agent.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/learner.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/learner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_collect.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_collect.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_collect_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_collect_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_eval.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_eval.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_eval_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_eval_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_reverb_server.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_reverb_server.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_reverb_server_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_train.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_train.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/distributed/ppo_train_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/distributed/ppo_train_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/env.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/env_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/env_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/feature_ops.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/feature_ops.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/feature_ops_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/feature_ops_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/gin_external_configurables.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/gin_external_configurables.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/config.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/env.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/inlining/inlining_runner.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/inlining/inlining_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/local_data_collector.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/local_data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/local_data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/local_data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/log_reader.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/log_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/log_reader_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/log_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/policy_saver.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/policy_saver.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/policy_saver_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/policy_saver_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/problem_configuration.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/problem_configuration.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/random_net_distillation.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/random_net_distillation.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/random_net_distillation_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/random_net_distillation_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/config.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_network.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_network_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc/regalloc_runner.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc/regalloc_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/config.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/registry.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/registry.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/train_bc.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/train_bc.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/train_locally.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/train_locally.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/trainer.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/trainer.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/rl/trainer_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/rl/trainer_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/__init__.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/combine_training_corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/combine_training_corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/extract_ir_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/extract_ir_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_graphs.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_graphs.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_utils.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/feature_importance_utils_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/feature_importance_utils_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_default_trace.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_default_trace.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_default_trace_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_default_trace_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_test_model.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_test_model.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_test_model_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_test_model_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/generate_vocab.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/generate_vocab.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus_lib.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/make_corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/make_corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/compiler_opt/tools/merge_best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202308060007/compiler_opt/tools/merge_best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202308050006
+Version: 0.0.1.dev202308060007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/ml_compiler_opt.egg-info/SOURCES.txt` & `ml-compiler-opt-0.0.1.dev202308060007/ml_compiler_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308050006/pyproject.toml` & `ml-compiler-opt-0.0.1.dev202308060007/pyproject.toml`

 * *Files identical despite different names*

