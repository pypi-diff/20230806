# Comparing `tmp/python-ta-2.5.0.tar.gz` & `tmp/python-ta-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ta-2.5.0.tar", last modified: Thu Apr 27 15:29:43 2023, max compression
+gzip compressed data, was "python-ta-2.6.0.tar", last modified: Sun Aug  6 17:09:02 2023, max compression
```

## Comparing `python-ta-2.5.0.tar` & `python-ta-2.6.0.tar`

### file list

```diff
@@ -1,147 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.890178 python-ta-2.5.0/
--rw-rw-rw-   0        0        0    35141 2020-09-24 17:22:04.000000 python-ta-2.5.0/LICENSE
--rw-rw-rw-   0        0        0      178 2022-04-18 16:52:09.000000 python-ta-2.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3457 2023-04-27 15:29:43.890178 python-ta-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3004 2023-01-30 20:58:29.000000 python-ta-2.5.0/README.md
--rw-rw-rw-   0        0        0      404 2021-08-24 20:57:44.000000 python-ta-2.5.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.759791 python-ta-2.5.0/python_ta/
--rw-rw-rw-   0        0        0    17406 2023-04-27 15:28:54.000000 python-ta-2.5.0/python_ta/__init__.py
--rw-rw-rw-   0        0        0     2322 2022-01-27 00:26:16.000000 python-ta-2.5.0/python_ta/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.825838 python-ta-2.5.0/python_ta/cfg/
--rw-rw-rw-   0        0        0       44 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/cfg/__init__.py
--rw-rw-rw-   0        0        0     6958 2023-04-08 02:58:51.000000 python-ta-2.5.0/python_ta/cfg/graph.py
--rw-rw-rw-   0        0        0    13501 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/cfg/visitor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.885765 python-ta-2.5.0/python_ta/checkers/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/checkers/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/forbidden_import_checker.py
--rw-rw-rw-   0        0        0     2872 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/forbidden_io_function_checker.py
--rw-rw-rw-   0        0        0     1623 2023-03-22 15:35:32.000000 python-ta-2.5.0/python_ta/checkers/forbidden_python_syntax_checker.py
--rw-rw-rw-   0        0        0     3571 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/global_variables_checker.py
--rw-rw-rw-   0        0        0     1635 2022-11-27 20:47:51.000000 python-ta-2.5.0/python_ta/checkers/invalid_for_target_checker.py
--rw-rw-rw-   0        0        0     2351 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/invalid_range_index_checker.py
--rw-rw-rw-   0        0        0     2479 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/missing_space_in_doctest_checker.py
--rw-rw-rw-   0        0        0     2506 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/one_iteration_checker.py
--rw-rw-rw-   0        0        0     6312 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/possibly_undefined_checker.py
--rw-rw-rw-   0        0        0     1419 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/pycodestyle_checker.py
--rw-rw-rw-   0        0        0     5721 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/redundant_assignment_checker.py
--rw-rw-rw-   0        0        0     1411 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/shadowing_in_comprehension_checker.py
--rw-rw-rw-   0        0        0     2627 2022-12-12 02:59:49.000000 python-ta-2.5.0/python_ta/checkers/top_level_code_checker.py
--rw-rw-rw-   0        0        0     3777 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/type_annotation_checker.py
--rw-rw-rw-   0        0        0     1249 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/checkers/type_inference_checker.py
--rw-rw-rw-   0        0        0     6273 2022-10-24 01:36:54.000000 python-ta-2.5.0/python_ta/checkers/unnecessary_indexing_checker.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.917094 python-ta-2.5.0/python_ta/config/
--rw-rw-rw-   0        0        0     4159 2022-12-07 20:53:21.000000 python-ta-2.5.0/python_ta/config/.pylintrc
--rw-rw-rw-   0        0        0    14352 2023-01-30 20:43:19.000000 python-ta-2.5.0/python_ta/config/messages_config.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.933160 python-ta-2.5.0/python_ta/contracts/
--rw-rw-rw-   0        0        0    22633 2023-01-31 18:38:30.000000 python-ta-2.5.0/python_ta/contracts/__init__.py
--rw-rw-rw-   0        0        0     3563 2021-11-06 03:28:14.000000 python-ta-2.5.0/python_ta/contracts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.964470 python-ta-2.5.0/python_ta/debug/
--rw-rw-rw-   0        0        0       50 2022-08-07 18:08:41.000000 python-ta-2.5.0/python_ta/debug/__init__.py
--rw-rw-rw-   0        0        0     6541 2022-12-12 02:59:49.000000 python-ta-2.5.0/python_ta/debug/accumulation_table.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.011294 python-ta-2.5.0/python_ta/patches/
--rw-rw-rw-   0        0        0      410 2022-12-07 17:07:10.000000 python-ta-2.5.0/python_ta/patches/__init__.py
--rw-rw-rw-   0        0        0     3921 2022-10-14 01:27:28.000000 python-ta-2.5.0/python_ta/patches/checkers.py
--rw-rw-rw-   0        0        0      933 2022-04-18 16:52:09.000000 python-ta-2.5.0/python_ta/patches/error_messages.py
--rw-rw-rw-   0        0        0      895 2022-06-30 13:49:27.000000 python-ta-2.5.0/python_ta/patches/messages.py
--rw-rw-rw-   0        0        0      864 2022-12-07 20:53:21.000000 python-ta-2.5.0/python_ta/patches/transforms.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.089856 python-ta-2.5.0/python_ta/reporters/
--rw-rw-rw-   0        0        0      296 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/reporters/__init__.py
--rw-rw-rw-   0        0        0     1937 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/color_reporter.py
--rw-rw-rw-   0        0        0    10213 2022-09-05 23:10:07.000000 python-ta-2.5.0/python_ta/reporters/core.py
--rw-rw-rw-   0        0        0     5864 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/html_reporter.py
--rw-rw-rw-   0        0        0     1156 2022-09-05 23:10:07.000000 python-ta-2.5.0/python_ta/reporters/json_reporter.py
--rw-rw-rw-   0        0        0     5368 2022-06-30 12:34:36.000000 python-ta-2.5.0/python_ta/reporters/node_printers.py
--rw-rw-rw-   0        0        0     3028 2022-07-07 23:34:28.000000 python-ta-2.5.0/python_ta/reporters/plain_reporter.py
--rw-rw-rw-   0        0        0      823 2023-04-27 15:16:56.000000 python-ta-2.5.0/python_ta/reporters/stat_reporter.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.199376 python-ta-2.5.0/python_ta/reporters/templates/
--rw-rw-rw-   0        0        0   160658 2023-01-09 17:16:14.000000 python-ta-2.5.0/python_ta/reporters/templates/jquery-3.2.1.min.js
--rw-rw-rw-   0        0        0    13773 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/reporters/templates/pyta_logo_markdown.png
--rw-rw-rw-   0        0        0     1435 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/reporters/templates/script.js
--rw-rw-rw-   0        0        0     9635 2021-08-23 23:35:24.000000 python-ta-2.5.0/python_ta/reporters/templates/stylesheet.css
--rw-rw-rw-   0        0        0    16873 2021-12-04 00:01:01.000000 python-ta-2.5.0/python_ta/reporters/templates/template.html.jinja
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.246824 python-ta-2.5.0/python_ta/transforms/
--rw-rw-rw-   0        0        0     5298 2022-08-24 00:15:57.000000 python-ta-2.5.0/python_ta/transforms/ExprWrapper.py
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/transforms/__init__.py
--rw-rw-rw-   0        0        0    24351 2023-03-22 15:29:31.000000 python-ta-2.5.0/python_ta/transforms/setendings.py
--rw-rw-rw-   0        0        0    43708 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/transforms/type_inference_visitor.py
--rw-rw-rw-   0        0        0     1999 2022-08-24 00:15:57.000000 python-ta-2.5.0/python_ta/transforms/z3_visitor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.293659 python-ta-2.5.0/python_ta/typecheck/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/typecheck/__init__.py
--rw-rw-rw-   0        0        0    40815 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/base.py
--rw-rw-rw-   0        0        0     6635 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/errors.py
--rw-rw-rw-   0        0        0     7147 2021-08-23 01:35:55.000000 python-ta-2.5.0/python_ta/typecheck/type_store.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.309294 python-ta-2.5.0/python_ta/typecheck/typeshed/
--rw-rw-rw-   0        0        0     1453 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/typecheck/typeshed/README.md
--rw-rw-rw-   0        0        0    70480 2022-04-07 16:59:30.000000 python-ta-2.5.0/python_ta/typecheck/typeshed/builtins.pyi
--rw-rw-rw-   0        0        0     3829 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/upload.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.327553 python-ta-2.5.0/python_ta/util/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/python_ta/util/__init__.py
--rw-rw-rw-   0        0        0     1078 2021-08-17 17:13:02.000000 python-ta-2.5.0/python_ta/util/monad.py
--rw-rw-rw-   0        0        0     1257 2022-10-14 01:27:28.000000 python-ta-2.5.0/python_ta/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:42.790990 python-ta-2.5.0/python_ta.egg-info/
--rw-rw-rw-   0        0        0     3457 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4592 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-09-26 00:08:53.000000 python-ta-2.5.0/python_ta.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      322 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-27 15:29:42.000000 python-ta-2.5.0/python_ta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.387583 python-ta-2.5.0/sample_usage/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/sample_usage/__init__.py
--rw-rw-rw-   0        0        0     2512 2023-04-27 15:16:56.000000 python-ta-2.5.0/sample_usage/draw_cfg.py
--rw-rw-rw-   0        0        0     3299 2021-08-23 01:35:55.000000 python-ta-2.5.0/sample_usage/draw_tnodes.py
--rw-rw-rw-   0        0        0     1547 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/print_ast.py
--rw-rw-rw-   0        0        0     3092 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/print_nodes.py
--rw-rw-rw-   0        0        0     2074 2022-08-08 17:55:51.000000 python-ta-2.5.0/sample_usage/print_table.py
--rw-rw-rw-   0        0        0     5758 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/pyta_stats.py
--rw-rw-rw-   0        0        0     5538 2021-08-17 17:13:02.000000 python-ta-2.5.0/sample_usage/stats_analysis.py
--rw-rw-rw-   0        0        0      999 2023-04-27 15:29:43.905867 python-ta-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2021-08-24 20:57:44.000000 python-ta-2.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.497490 python-ta-2.5.0/tests/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0    11609 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/custom_hypothesis_support.py
--rw-rw-rw-   0        0        0     7213 2023-01-30 20:43:19.000000 python-ta-2.5.0/tests/test_check.py
--rw-rw-rw-   0        0        0    11322 2022-12-09 22:37:04.000000 python-ta-2.5.0/tests/test_class_contracts.py
--rw-rw-rw-   0        0        0    19381 2023-01-31 18:38:30.000000 python-ta-2.5.0/tests/test_contracts.py
--rw-rw-rw-   0        0        0     4153 2023-01-28 01:41:43.000000 python-ta-2.5.0/tests/test_examples.py
--rw-rw-rw-   0        0        0    17767 2021-12-09 21:58:56.000000 python-ta-2.5.0/tests/test_setendings.py
--rw-rw-rw-   0        0        0     5330 2021-08-17 17:13:02.000000 python-ta-2.5.0/tests/test_subclass_contracts.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.528117 python-ta-2.5.0/tests/test_type_constraints/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.5.0/tests/test_type_constraints/__init__.py
--rw-rw-rw-   0        0        0    15992 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_constraints/test_tnode_structure.py
--rw-rw-rw-   0        0        0     6429 2021-08-17 17:13:02.000000 python-ta-2.5.0/tests/test_type_constraints/test_unify.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:29:43.890178 python-ta-2.5.0/tests/test_type_inference/
--rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.5.0/tests/test_type_inference/__init__.py
--rw-rw-rw-   0        0        0     8416 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_annassign.py
--rw-rw-rw-   0        0        0    11246 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_assign.py
--rw-rw-rw-   0        0        0     4353 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_assign_tuple.py
--rw-rw-rw-   0        0        0     6670 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_attribute.py
--rw-rw-rw-   0        0        0     3912 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_binops.py
--rw-rw-rw-   0        0        0     1290 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_boolops.py
--rw-rw-rw-   0        0        0     4907 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_classdef.py
--rw-rw-rw-   0        0        0     3068 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_compare.py
--rw-rw-rw-   0        0        0      651 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_const.py
--rw-rw-rw-   0        0        0     2514 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_dict.py
--rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_dictcomp.py
--rw-rw-rw-   0        0        0     2486 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_errors.py
--rw-rw-rw-   0        0        0     5710 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_for.py
--rw-rw-rw-   0        0        0     5265 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_annotation.py
--rw-rw-rw-   0        0        0     8871 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_def_inference.py
--rw-rw-rw-   0        0        0     4905 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_function_overload.py
--rw-rw-rw-   0        0        0    21649 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_functions.py
--rw-rw-rw-   0        0        0      555 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_ifexpr.py
--rw-rw-rw-   0        0        0     3749 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_imports.py
--rw-rw-rw-   0        0        0     2142 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_initializer.py
--rw-rw-rw-   0        0        0     4382 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_lambda.py
--rw-rw-rw-   0        0        0     3763 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_list.py
--rw-rw-rw-   0        0        0     2093 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_listcomp.py
--rw-rw-rw-   0        0        0      856 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_literals.py
--rw-rw-rw-   0        0        0      641 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_name.py
--rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_set.py
--rw-rw-rw-   0        0        0     1935 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_setcomp.py
--rw-rw-rw-   0        0        0     5197 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_starred.py
--rw-rw-rw-   0        0        0     5718 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_subscript.py
--rw-rw-rw-   0        0        0      586 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_tuple.py
--rw-rw-rw-   0        0        0     4614 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_typefail_reason.py
--rw-rw-rw-   0        0        0     1090 2021-08-23 01:35:55.000000 python-ta-2.5.0/tests/test_type_inference/test_unaryops.py
--rw-rw-rw-   0        0        0     1444 2022-08-24 00:15:57.000000 python-ta-2.5.0/tests/test_z3_visitor.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.564427 python-ta-2.6.0/
+-rw-rw-rw-   0        0        0    35141 2020-09-24 17:22:04.000000 python-ta-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0      178 2022-04-18 16:52:09.000000 python-ta-2.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3703 2023-08-06 17:09:02.564427 python-ta-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3026 2023-05-22 17:08:19.000000 python-ta-2.6.0/README.md
+-rw-rw-rw-   0        0        0     1770 2023-08-06 15:08:40.000000 python-ta-2.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.116483 python-ta-2.6.0/python_ta/
+-rw-rw-rw-   0        0        0    19929 2023-08-06 16:45:34.000000 python-ta-2.6.0/python_ta/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-06-24 16:15:59.000000 python-ta-2.6.0/python_ta/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.152876 python-ta-2.6.0/python_ta/cfg/
+-rw-rw-rw-   0        0        0       84 2023-05-31 00:24:38.000000 python-ta-2.6.0/python_ta/cfg/__init__.py
+-rw-rw-rw-   0        0        0     5554 2023-06-11 15:23:53.000000 python-ta-2.6.0/python_ta/cfg/cfg_generator.py
+-rw-rw-rw-   0        0        0     7112 2023-06-02 19:32:36.000000 python-ta-2.6.0/python_ta/cfg/graph.py
+-rw-rw-rw-   0        0        0    16275 2023-06-11 15:23:53.000000 python-ta-2.6.0/python_ta/cfg/visitor.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.222317 python-ta-2.6.0/python_ta/checkers/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.6.0/python_ta/checkers/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/forbidden_import_checker.py
+-rw-rw-rw-   0        0        0     2872 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/forbidden_io_function_checker.py
+-rw-rw-rw-   0        0        0     1623 2023-03-22 15:35:32.000000 python-ta-2.6.0/python_ta/checkers/forbidden_python_syntax_checker.py
+-rw-rw-rw-   0        0        0     3856 2023-06-02 19:32:36.000000 python-ta-2.6.0/python_ta/checkers/global_variables_checker.py
+-rw-rw-rw-   0        0        0     1635 2022-11-27 20:47:51.000000 python-ta-2.6.0/python_ta/checkers/invalid_for_target_checker.py
+-rw-rw-rw-   0        0        0    18338 2023-07-27 17:16:23.000000 python-ta-2.6.0/python_ta/checkers/invalid_name_checker.py
+-rw-rw-rw-   0        0        0     2351 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/invalid_range_index_checker.py
+-rw-rw-rw-   0        0        0     2479 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/missing_space_in_doctest_checker.py
+-rw-rw-rw-   0        0        0     2506 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/one_iteration_checker.py
+-rw-rw-rw-   0        0        0     6312 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/possibly_undefined_checker.py
+-rw-rw-rw-   0        0        0     1419 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/pycodestyle_checker.py
+-rw-rw-rw-   0        0        0     5721 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/redundant_assignment_checker.py
+-rw-rw-rw-   0        0        0     1411 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/shadowing_in_comprehension_checker.py
+-rw-rw-rw-   0        0        0     2800 2023-05-31 00:24:38.000000 python-ta-2.6.0/python_ta/checkers/top_level_code_checker.py
+-rw-rw-rw-   0        0        0     3777 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/type_annotation_checker.py
+-rw-rw-rw-   0        0        0     1249 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/checkers/type_inference_checker.py
+-rw-rw-rw-   0        0        0     6421 2023-06-08 21:54:22.000000 python-ta-2.6.0/python_ta/checkers/unnecessary_indexing_checker.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.231896 python-ta-2.6.0/python_ta/config/
+-rw-rw-rw-   0        0        0     4270 2023-07-27 17:16:23.000000 python-ta-2.6.0/python_ta/config/.pylintrc
+-rw-rw-rw-   0        0        0    14358 2023-05-22 19:05:08.000000 python-ta-2.6.0/python_ta/config/messages_config.toml
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.239370 python-ta-2.6.0/python_ta/contracts/
+-rw-rw-rw-   0        0        0    23519 2023-08-06 14:56:20.000000 python-ta-2.6.0/python_ta/contracts/__init__.py
+-rw-rw-rw-   0        0        0     3563 2021-11-06 03:28:14.000000 python-ta-2.6.0/python_ta/contracts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.243948 python-ta-2.6.0/python_ta/debug/
+-rw-rw-rw-   0        0        0       50 2022-08-07 18:08:41.000000 python-ta-2.6.0/python_ta/debug/__init__.py
+-rw-rw-rw-   0        0        0     6541 2022-12-12 02:59:49.000000 python-ta-2.6.0/python_ta/debug/accumulation_table.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.263172 python-ta-2.6.0/python_ta/patches/
+-rw-rw-rw-   0        0        0      410 2022-12-07 17:07:10.000000 python-ta-2.6.0/python_ta/patches/__init__.py
+-rw-rw-rw-   0        0        0     3921 2022-10-14 01:27:28.000000 python-ta-2.6.0/python_ta/patches/checkers.py
+-rw-rw-rw-   0        0        0      933 2022-04-18 16:52:09.000000 python-ta-2.6.0/python_ta/patches/error_messages.py
+-rw-rw-rw-   0        0        0      895 2023-07-03 15:15:59.000000 python-ta-2.6.0/python_ta/patches/messages.py
+-rw-rw-rw-   0        0        0      864 2022-12-07 20:53:21.000000 python-ta-2.6.0/python_ta/patches/transforms.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.295053 python-ta-2.6.0/python_ta/reporters/
+-rw-rw-rw-   0        0        0      296 2021-08-17 17:13:02.000000 python-ta-2.6.0/python_ta/reporters/__init__.py
+-rw-rw-rw-   0        0        0     1937 2022-07-07 23:34:28.000000 python-ta-2.6.0/python_ta/reporters/color_reporter.py
+-rw-rw-rw-   0        0        0    10723 2023-08-06 15:37:05.000000 python-ta-2.6.0/python_ta/reporters/core.py
+-rw-rw-rw-   0        0        0     5747 2023-06-06 18:54:44.000000 python-ta-2.6.0/python_ta/reporters/html_reporter.py
+-rw-rw-rw-   0        0        0     1825 2023-07-09 22:39:54.000000 python-ta-2.6.0/python_ta/reporters/json_reporter.py
+-rw-rw-rw-   0        0        0    10697 2023-06-24 16:15:59.000000 python-ta-2.6.0/python_ta/reporters/node_printers.py
+-rw-rw-rw-   0        0        0     3136 2023-07-09 22:39:54.000000 python-ta-2.6.0/python_ta/reporters/plain_reporter.py
+-rw-rw-rw-   0        0        0      823 2023-04-27 15:16:56.000000 python-ta-2.6.0/python_ta/reporters/stat_reporter.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.318812 python-ta-2.6.0/python_ta/reporters/templates/
+-rw-rw-rw-   0        0        0   160658 2023-01-09 17:16:14.000000 python-ta-2.6.0/python_ta/reporters/templates/jquery-3.2.1.min.js
+-rw-rw-rw-   0        0        0    13773 2020-09-24 17:22:04.000000 python-ta-2.6.0/python_ta/reporters/templates/pyta_logo_markdown.png
+-rw-rw-rw-   0        0        0     1435 2021-08-17 17:13:02.000000 python-ta-2.6.0/python_ta/reporters/templates/script.js
+-rw-rw-rw-   0        0        0     9675 2023-07-09 22:39:54.000000 python-ta-2.6.0/python_ta/reporters/templates/stylesheet.css
+-rw-rw-rw-   0        0        0    17485 2023-07-09 22:39:54.000000 python-ta-2.6.0/python_ta/reporters/templates/template.html.jinja
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.337003 python-ta-2.6.0/python_ta/transforms/
+-rw-rw-rw-   0        0        0     5298 2022-08-24 00:15:57.000000 python-ta-2.6.0/python_ta/transforms/ExprWrapper.py
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.6.0/python_ta/transforms/__init__.py
+-rw-rw-rw-   0        0        0    24351 2023-03-22 15:29:31.000000 python-ta-2.6.0/python_ta/transforms/setendings.py
+-rw-rw-rw-   0        0        0    43708 2021-08-23 01:35:55.000000 python-ta-2.6.0/python_ta/transforms/type_inference_visitor.py
+-rw-rw-rw-   0        0        0     1999 2022-08-24 00:15:57.000000 python-ta-2.6.0/python_ta/transforms/z3_visitor.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.356151 python-ta-2.6.0/python_ta/typecheck/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.6.0/python_ta/typecheck/__init__.py
+-rw-rw-rw-   0        0        0    40815 2021-08-23 01:35:55.000000 python-ta-2.6.0/python_ta/typecheck/base.py
+-rw-rw-rw-   0        0        0     6635 2021-08-23 01:35:55.000000 python-ta-2.6.0/python_ta/typecheck/errors.py
+-rw-rw-rw-   0        0        0     7147 2021-08-23 01:35:55.000000 python-ta-2.6.0/python_ta/typecheck/type_store.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.365319 python-ta-2.6.0/python_ta/typecheck/typeshed/
+-rw-rw-rw-   0        0        0     1453 2021-08-17 17:13:02.000000 python-ta-2.6.0/python_ta/typecheck/typeshed/README.md
+-rw-rw-rw-   0        0        0    70480 2022-04-07 16:59:30.000000 python-ta-2.6.0/python_ta/typecheck/typeshed/builtins.pyi
+-rw-rw-rw-   0        0        0     3829 2021-08-17 17:13:02.000000 python-ta-2.6.0/python_ta/upload.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.366689 python-ta-2.6.0/python_ta/util/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.6.0/python_ta/util/__init__.py
+-rw-rw-rw-   0        0        0     1078 2021-08-17 17:13:02.000000 python-ta-2.6.0/python_ta/util/monad.py
+-rw-rw-rw-   0        0        0     1257 2022-10-14 01:27:28.000000 python-ta-2.6.0/python_ta/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.137738 python-ta-2.6.0/python_ta.egg-info/
+-rw-rw-rw-   0        0        0     3703 2023-08-06 17:09:01.000000 python-ta-2.6.0/python_ta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4620 2023-08-06 17:09:02.000000 python-ta-2.6.0/python_ta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 17:09:01.000000 python-ta-2.6.0/python_ta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-08-06 17:09:01.000000 python-ta-2.6.0/python_ta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-09-26 00:08:53.000000 python-ta-2.6.0/python_ta.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      353 2023-08-06 17:09:01.000000 python-ta-2.6.0/python_ta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 17:09:01.000000 python-ta-2.6.0/python_ta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 17:09:02.573293 python-ta-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0       38 2021-08-24 20:57:44.000000 python-ta-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.418127 python-ta-2.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:04.000000 python-ta-2.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    11609 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/custom_hypothesis_support.py
+-rw-rw-rw-   0        0        0     7321 2023-06-24 18:11:58.000000 python-ta-2.6.0/tests/test_check.py
+-rw-rw-rw-   0        0        0    11203 2023-08-06 14:56:20.000000 python-ta-2.6.0/tests/test_class_contracts.py
+-rw-rw-rw-   0        0        0    19048 2023-08-06 14:56:20.000000 python-ta-2.6.0/tests/test_contracts.py
+-rw-rw-rw-   0        0        0     1006 2023-07-27 00:59:15.000000 python-ta-2.6.0/tests/test_contracts_attr_value_restoration.py
+-rw-rw-rw-   0        0        0      787 2023-07-09 22:39:54.000000 python-ta-2.6.0/tests/test_contracts_type_alias_abstract_network.py
+-rw-rw-rw-   0        0        0      367 2023-07-09 22:39:54.000000 python-ta-2.6.0/tests/test_contracts_type_alias_abstract_ring.py
+-rw-rw-rw-   0        0        0     4153 2023-01-28 01:41:43.000000 python-ta-2.6.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0    17767 2021-12-09 21:58:56.000000 python-ta-2.6.0/tests/test_setendings.py
+-rw-rw-rw-   0        0        0     5330 2021-08-17 17:13:02.000000 python-ta-2.6.0/tests/test_subclass_contracts.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.432263 python-ta-2.6.0/tests/test_type_constraints/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.6.0/tests/test_type_constraints/__init__.py
+-rw-rw-rw-   0        0        0    16001 2023-06-24 18:11:58.000000 python-ta-2.6.0/tests/test_type_constraints/test_tnode_structure.py
+-rw-rw-rw-   0        0        0     6429 2021-08-17 17:13:02.000000 python-ta-2.6.0/tests/test_type_constraints/test_unify.py
+drwxrwxrwx   0        0        0        0 2023-08-06 17:09:02.564427 python-ta-2.6.0/tests/test_type_inference/
+-rw-rw-rw-   0        0        0        0 2020-09-24 17:22:05.000000 python-ta-2.6.0/tests/test_type_inference/__init__.py
+-rw-rw-rw-   0        0        0     8416 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_annassign.py
+-rw-rw-rw-   0        0        0    11246 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_assign.py
+-rw-rw-rw-   0        0        0     4353 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_assign_tuple.py
+-rw-rw-rw-   0        0        0     6670 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_attribute.py
+-rw-rw-rw-   0        0        0     3912 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_binops.py
+-rw-rw-rw-   0        0        0     1290 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_boolops.py
+-rw-rw-rw-   0        0        0     4907 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_classdef.py
+-rw-rw-rw-   0        0        0     3068 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_compare.py
+-rw-rw-rw-   0        0        0      651 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_const.py
+-rw-rw-rw-   0        0        0     2514 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_dict.py
+-rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_dictcomp.py
+-rw-rw-rw-   0        0        0     2486 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_errors.py
+-rw-rw-rw-   0        0        0     5710 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_for.py
+-rw-rw-rw-   0        0        0     5265 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_function_annotation.py
+-rw-rw-rw-   0        0        0     8871 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_function_def_inference.py
+-rw-rw-rw-   0        0        0     4905 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_function_overload.py
+-rw-rw-rw-   0        0        0    21649 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_functions.py
+-rw-rw-rw-   0        0        0      555 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_ifexpr.py
+-rw-rw-rw-   0        0        0     3749 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_imports.py
+-rw-rw-rw-   0        0        0     2142 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_initializer.py
+-rw-rw-rw-   0        0        0     4382 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_lambda.py
+-rw-rw-rw-   0        0        0     3763 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_list.py
+-rw-rw-rw-   0        0        0     2093 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_listcomp.py
+-rw-rw-rw-   0        0        0      856 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_literals.py
+-rw-rw-rw-   0        0        0      641 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_name.py
+-rw-rw-rw-   0        0        0     1504 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_set.py
+-rw-rw-rw-   0        0        0     1935 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_setcomp.py
+-rw-rw-rw-   0        0        0     5197 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_starred.py
+-rw-rw-rw-   0        0        0     5718 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_subscript.py
+-rw-rw-rw-   0        0        0      586 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_tuple.py
+-rw-rw-rw-   0        0        0     4614 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_typefail_reason.py
+-rw-rw-rw-   0        0        0     1090 2021-08-23 01:35:55.000000 python-ta-2.6.0/tests/test_type_inference/test_unaryops.py
+-rw-rw-rw-   0        0        0     1288 2023-07-27 17:16:23.000000 python-ta-2.6.0/tests/test_validate_invariants.py
+-rw-rw-rw-   0        0        0     1444 2022-08-24 00:15:57.000000 python-ta-2.6.0/tests/test_z3_visitor.py
```

### Comparing `python-ta-2.5.0/LICENSE` & `python-ta-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/PKG-INFO` & `python-ta-2.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: python-ta
-Version: 2.5.0
+Version: 2.6.0
 Summary: Code checking tool for teaching Python
-Home-page: https://github.com/pyta-uoft/pyta
-Author: David Liu
-Author-email: david@cs.toronto.edu
+Author-email: David Liu <david@cs.toronto.edu>
 License: MIT
-Requires-Python: ~=3.8
+Project-URL: Homepage, https://github.com/pyta-uoft/pyta
+Project-URL: Documentation, https://www.cs.toronto.edu/~david/pyta/
+Project-URL: Repository, https://github.com/pyta-uoft/pyta.git
+Project-URL: Changelog, https://github.com/pyta-uoft/pyta/blob/master/CHANGELOG.md
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: z3
 License-File: LICENSE
 
 # PyTA
 
@@ -97,20 +99,22 @@
 Craig Katsube,
 Rebecca Kay,
 Christopher Koehler,
 David Kim,
 Simeon Krastnikov,
 Ryan Lee,
 Hayley Lin,
+Bruce Liu,
 Wendy Liu,
 Yibing (Amy) Lu,
 Shweta Mogalapalli,
 Ignas Panero Armoska,
 Justin Park,
 Harshkumar Patel,
 Amr Sharaf,
 Richard Shi,
 Kavin Singh,
 Alexey Strokach,
 Sophy Sun,
+Sarah Wang
 Jasmine Wu,
 Philippe Yu,
```

### Comparing `python-ta-2.5.0/README.md` & `python-ta-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,22 @@
 Craig Katsube,
 Rebecca Kay,
 Christopher Koehler,
 David Kim,
 Simeon Krastnikov,
 Ryan Lee,
 Hayley Lin,
+Bruce Liu,
 Wendy Liu,
 Yibing (Amy) Lu,
 Shweta Mogalapalli,
 Ignas Panero Armoska,
 Justin Park,
 Harshkumar Patel,
 Amr Sharaf,
 Richard Shi,
 Kavin Singh,
 Alexey Strokach,
 Sophy Sun,
+Sarah Wang
 Jasmine Wu,
 Philippe Yu,
```

### Comparing `python-ta-2.5.0/python_ta/__init__.py` & `python-ta-2.6.0/python_ta/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 
 Or, put the following code in your Python module:
 
 if __name__ == '__main__':
     import python_ta
     python_ta.check_all()
 """
-__version__ = "2.5.0"  # Version number
+__version__ = "2.6.0"  # Version number
 
 # First, remove underscore from builtins if it has been bound in the REPL.
 import builtins
 
+from pylint.config.config_file_parser import _ConfigurationFileParser
+from pylint.config.exceptions import _UnrecognizedOptionError
 from pylint.lint import PyLinter
 
 from .reporters.core import PythonTaReporter
 
 try:
     del builtins._
 except AttributeError:
@@ -61,45 +63,62 @@
 PYLINT_PATCHED = False
 
 
 def check_errors(
     module_name: Union[List[str], str] = "",
     config: Union[dict, str] = "",
     output: Optional[TextIO] = None,
+    load_default_config: bool = True,
 ) -> PythonTaReporter:
     """Check a module for errors, printing a report."""
-    return _check(module_name=module_name, level="error", local_config=config, output=output)
+    return _check(
+        module_name=module_name,
+        level="error",
+        local_config=config,
+        output=output,
+        load_default_config=load_default_config,
+    )
 
 
 def check_all(
     module_name: Union[List[str], str] = "",
     config: Union[dict, str] = "",
     output: Optional[TextIO] = None,
+    load_default_config: bool = True,
 ) -> PythonTaReporter:
     """Check a module for errors and style warnings, printing a report."""
-    return _check(module_name=module_name, level="all", local_config=config, output=output)
+    return _check(
+        module_name=module_name,
+        level="all",
+        local_config=config,
+        output=output,
+        load_default_config=load_default_config,
+    )
 
 
 def _check(
     module_name: Union[List[str], str] = "",
     level: str = "all",
     local_config: Union[dict, str] = "",
     output: Optional[TextIO] = None,
+    load_default_config: bool = True,
 ) -> PythonTaReporter:
     """Check a module for problems, printing a report.
 
     The `module_name` can take several inputs:
       - string of a directory, or file to check (`.py` extension optional).
       - list of strings of directories or files -- can have multiple.
       - no argument -- checks the python file containing the function call.
     `level` is used to specify which checks should be made.
     `local_config` is a dict of config options or string (config file name).
     `output` is an absolute or relative path to capture pyta data output. Default std out.
+    `load_default_config` is used to specify whether to load the default .pylintrc file that comes
+    with PythonTA. It will load it by default.
     """
-    linter = reset_linter(config=local_config)
+    linter = reset_linter(config=local_config, load_default_config=load_default_config)
     current_reporter = linter.reporter
     current_reporter.set_output(output)
     messages_config_path = linter.config.messages_config_path
     messages_config_default_path = linter._option_dicts["messages-config-path"]["default"]
     messages_config = _load_messages_config(messages_config_path, messages_config_default_path)
 
     global PYLINT_PATCHED
@@ -115,21 +134,38 @@
         for locations in _get_valid_files_to_check(module_name):
             f_paths = []  # Paths to files for data submission
             errs = []  # Errors caught in files for data submission
             config = {}  # Configuration settings for data submission
             for file_py in get_file_paths(locations):
                 if not _verify_pre_check(file_py):
                     continue  # Check the other files
-                # The current file can actually be checked so update the flag
-                is_any_file_checked = True
                 # Load config file in user location. Construct new linter each
                 # time, so config options don't bleed to unintended files.
                 # Reuse the same reporter each time to accumulate the results across different files.
-                linter = reset_linter(config=local_config, file_linted=file_py)
-                linter.set_reporter(current_reporter)
+                linter = reset_linter(
+                    config=local_config,
+                    file_linted=file_py,
+                    load_default_config=load_default_config,
+                )
+
+                if not is_any_file_checked:
+                    prev_output = current_reporter.out
+                    current_reporter = linter.reporter
+                    current_reporter.out = prev_output
+
+                    # At this point, the only possible errors are those from parsing the config file
+                    # so print them, if there are any.
+                    if current_reporter.messages:
+                        current_reporter.print_messages()
+                else:
+                    linter.set_reporter(current_reporter)
+
+                # The current file was checked so update the flag
+                is_any_file_checked = True
+
                 module_name = os.path.splitext(os.path.basename(file_py))[0]
                 if module_name in MANAGER.astroid_cache:  # Remove module from astroid cache
                     del MANAGER.astroid_cache[module_name]
                 linter.check([file_py])  # Lint !
                 current_reporter.print_messages(level)
                 if linter.config.pyta_file_permission:
                     f_paths.append(file_py)  # Appending paths for upload
@@ -189,14 +225,42 @@
 
 def _load_config(linter: PyLinter, config_location: AnyStr) -> None:
     """Load configuration into the linter."""
     _config_initialization(linter, args_list=[], config_file=config_location)
     linter.config_file = config_location
 
 
+def _override_config(linter: PyLinter, config_location: AnyStr) -> None:
+    """Override the default linter configuration options (if possible).
+
+    Snippets taken from pylint.config.config_initialization.
+    """
+    linter.set_current_module(config_location)
+
+    # Read the configuration file.
+    config_file_parser = _ConfigurationFileParser(verbose=True, linter=linter)
+    try:
+        _, config_args = config_file_parser.parse_config_file(file_path=config_location)
+    except OSError as ex:
+        print(ex, file=sys.stderr)
+        sys.exit(32)
+
+    # Override the config options by parsing the provided file.
+    try:
+        linter._parse_configuration_file(config_args)
+    except _UnrecognizedOptionError as exc:
+        unrecognized_options_message = ", ".join(exc.options)
+        linter.add_message("unrecognized-option", args=unrecognized_options_message, line=0)
+
+    # Everything has been set up already so emit any stashed messages.
+    linter._emit_stashed_messages()
+
+    linter.config_file = config_location
+
+
 def _load_messages_config(path: str, default_path: str) -> dict:
     """Given path (potentially) specified by user and default default_path
     of messages config file, merge the config files."""
     merge_into = toml.load(default_path)
 
     if Path(default_path).resolve() == Path(path).resolve():
         return merge_into
@@ -219,36 +283,38 @@
                 merge_into[category][checker][error_code] = merge_from[category][checker][
                     error_code
                 ]
     return merge_into
 
 
 def reset_linter(
-    config: Optional[Union[dict, str]] = None, file_linted: Optional[AnyStr] = None
+    config: Optional[Union[dict, str]] = None,
+    file_linted: Optional[AnyStr] = None,
+    load_default_config: bool = True,
 ) -> PyLinter:
     """Construct a new linter. Register config and checker plugins.
 
     To determine which configuration to use:
+    - If the option is enabled, load the default PythonTA config file,
     - If the config argument is a string, use the config found at that location,
     - Otherwise,
         - Try to use the config file at directory of the file being linted,
-        - Otherwise try to use default config file shipped with python_ta.
         - If the config argument is a dictionary, apply those options afterward.
     Do not re-use a linter object. Returns a new linter.
     """
     # Tuple of custom options. Note: 'type' must map to a value equal a key in the pylint/config/option.py `VALIDATORS` dict.
     new_checker_options = (
         (
             "pyta-type-check",
             {"default": False, "type": "yn", "metavar": "<yn>", "help": "Enable the type-checker."},
         ),
         (
             "pyta-number-of-messages",
             {
-                "default": 5,
+                "default": 0,  # If the value is 0, all messages are displayed.
                 "type": "int",
                 "metavar": "<number_messages>",
                 "help": "Display a certain number of messages to the user, without overwhelming them.",
             },
         ),
         (
             "pyta-template-file",
@@ -310,28 +376,33 @@
     # options in `.pylintrc` config file.
     # Options stored in linter: `linter._all_options`, `linter._external_opts`
     linter = pylint.lint.PyLinter(options=new_checker_options)
     linter.load_default_plugins()  # Load checkers, reporters
     linter.load_plugin_modules(custom_checkers)
     linter.load_plugin_modules(["python_ta.transforms.setendings"])
 
+    default_config_path = _find_local_config(os.path.dirname(__file__))
+    set_config = _load_config
+
+    if load_default_config:
+        _load_config(linter, default_config_path)
+        # If we do specify to load the default config, we just need to override the options later.
+        set_config = _override_config
+
     if isinstance(config, str) and config != "":
-        # Use config file at the specified path instead of the default.
-        _load_config(linter, config)
+        set_config(linter, config)
     else:
         # If available, use config file at directory of the file being linted.
         pylintrc_location = None
         if file_linted:
             pylintrc_location = _find_local_config(file_linted)
 
-        # Otherwise, use default config file shipped with python_ta package.
-        if not pylintrc_location:
-            pylintrc_location = _find_local_config(os.path.dirname(__file__))
-
-        _load_config(linter, pylintrc_location)
+        # Load or override the options if there is a config file in the current directory.
+        if pylintrc_location:
+            set_config(linter, pylintrc_location)
 
         # Override part of the default config, with a dict of config options.
         # Note: these configs are overridden by config file in user's codebase
         # location.
         if isinstance(config, dict):
             for key in config:
                 linter.set_option(key, config[key])
```

### Comparing `python-ta-2.5.0/python_ta/__main__.py` & `python-ta-2.6.0/python_ta/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
     if version:
         print(__version__)
         return
 
     # `config` is None if `-c` flag is not set
     if generate_config:
-        pylintrc_location = os.path.join(os.path.dirname(__file__), ".pylintrc")
+        pylintrc_location = os.path.join(os.path.dirname(__file__), "config/.pylintrc")
         with open(pylintrc_location, "r") as f:
             contents = f.read()
             print(contents)
             sys.exit(0)
 
     checker = check_errors if errors_only else check_all
     paths = [click.format_filename(fn) for fn in filenames]
```

### Comparing `python-ta-2.5.0/python_ta/cfg/graph.py` & `python-ta-2.6.0/python_ta/cfg/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 
 
 class ControlFlowGraph:
     """A graph representing the control flow of a Python program."""
 
     start: CFGBlock
     end: CFGBlock
+    # The unique id of this cfg. Defaults to 0 if not initialized in a CFGVisitor instance.
+    cfg_id: int
     # block_count is used as an "autoincrement" to ensure the block ids are unique.
     block_count: int
     # blocks (with at least one statement) that will never be executed in runtime.
     unreachable_blocks: Set[CFGBlock]
 
-    def __init__(self) -> None:
+    def __init__(self, cfg_id: int = 0) -> None:
         self.block_count = 0
+        self.cfg_id = cfg_id
         self.unreachable_blocks = set()
         self.start = self.create_block()
         self.end = self.create_block()
 
     def create_block(
         self, pred: Optional[CFGBlock] = None, edge_label: Optional[Any] = None
     ) -> CFGBlock:
```

### Comparing `python-ta-2.5.0/python_ta/cfg/visitor.py` & `python-ta-2.6.0/python_ta/cfg/visitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,70 +10,109 @@
 
     Initialize with an options dict to configure the visitor.
 
     Supported Options:
       - "separate-condition-blocks": bool
             This option specifies whether the test condition of an if statement gets merged with any
             preceding statements or placed in a new block. By default, it will merge them.
+      - "functions": list
+            This option specifies whether to restrict the creation of cfgs to just top-level
+            function definitions or methods provided in this list. By default, it will create the
+            cfg for the file as it normally would.
 
     Private Attributes:
     _control_boundaries: A stack of the boundaries the visitor is currently in.
         The top of the stack corresponds to the end of the list.
         (compound statement [while], {'Break'/'Continue': CFGBlock to link to})
     """
 
     cfgs: Dict[Union[nodes.FunctionDef, nodes.Module], ControlFlowGraph]
     options: Dict[str, Any]
+    # cfg_count is used as an "auto-increment" to ensure cfg ids are unique.
+    cfg_count: int
     _current_cfg: Optional[ControlFlowGraph]
     _current_block: Optional[CFGBlock]
     _control_boundaries: List[Tuple[nodes.NodeNG, Dict[str, CFGBlock]]]
 
     def __init__(self, options: Optional[Dict[str, Any]] = None) -> None:
         super().__init__()
         self.cfgs = {}
-        self.options = {"separate-condition-blocks": False}
+        self.options = {
+            "separate-condition-blocks": False,
+            "functions": [],
+        }
         if options is not None:
             self.options.update(options)
+        self.cfg_count = 0
         self._current_cfg = None
         self._current_block = None
         self._control_boundaries = []
 
     def __getattr__(self, attr: str):
         if attr.startswith("visit_"):
             return self.visit_generic
         else:
             raise AttributeError(f"'CFGVisitor' object has not attribute '{attr}'")
 
     def visit_generic(self, node: nodes.NodeNG) -> None:
         """By default, add the expression to the end of the current block."""
-        self._current_block.add_statement(node)
+        if self._current_block is not None:
+            self._current_block.add_statement(node)
 
     def visit_module(self, module: nodes.Module) -> None:
-        self.cfgs[module] = ControlFlowGraph()
+        # Modules shouldn't be considered if user specifies functions to render
+        functions_to_render = self.options.get("functions", [])
+        if functions_to_render:
+            for child in module.body:
+                # Check any classes or function definitions for the target function/method
+                if isinstance(child, nodes.FunctionDef) or isinstance(child, nodes.ClassDef):
+                    child.accept(self)
+            return
+
+        self.cfgs[module] = ControlFlowGraph(self.cfg_count)
+        self.cfg_count += 1
         self._current_cfg = self.cfgs[module]
         self._current_block = self._current_cfg.start
         module.cfg_block = self._current_cfg.start
 
         for child in module.body:
             child.accept(self)
 
         self._current_cfg.link_or_merge(self._current_block, self._current_cfg.end)
         self._current_cfg.update_block_reachability()
 
     def visit_classdef(self, node: nodes.ClassDef) -> None:
+        functions_to_render = self.options.get("functions", [])
         for child in node.body:
-            child.accept(self)
+            if functions_to_render:
+                if isinstance(child, nodes.FunctionDef):
+                    child.accept(self)
+            else:
+                child.accept(self)
 
     def visit_functiondef(self, func: nodes.FunctionDef) -> None:
-        self._current_block.add_statement(func)
+        # If user specifies to only render functions, check if the function/method name is listed
+        functions_to_render = self.options.get("functions", [])
+        scope_parent = func.scope().parent
+
+        if functions_to_render:
+            if (
+                isinstance(scope_parent, nodes.ClassDef)
+                and (scope_parent.name + "." + func.name) not in functions_to_render
+            ) or (isinstance(scope_parent, nodes.Module) and func.name not in functions_to_render):
+                return
+
+        if self._current_block is not None:
+            self._current_block.add_statement(func)
 
         previous_cfg = self._current_cfg
         previous_block = self._current_block
 
-        self.cfgs[func] = ControlFlowGraph()
+        self.cfgs[func] = ControlFlowGraph(self.cfg_count)
+        self.cfg_count += 1
         self._current_cfg = self.cfgs[func]
 
         self._control_boundaries.append(
             (
                 func,
                 {
                     nodes.Return.__name__: self._current_cfg.end,
@@ -95,14 +134,18 @@
         self._current_cfg.link_or_merge(self._current_block, self._current_cfg.end)
         self._current_cfg.update_block_reachability()
 
         self._current_block = previous_block
         self._current_cfg = previous_cfg
 
     def visit_if(self, node: nodes.If) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         separate_conditions = self.options.get("separate-condition-blocks", False)
         if separate_conditions:
             # Create a block for the test condition
             test_block = self._current_cfg.create_block(self._current_block)
             test_block.add_statement(node.test)
             self._current_block = test_block
         else:
@@ -137,14 +180,18 @@
             self._current_cfg.link_or_merge(end_else, after_if_block, edge_label="False")
         else:
             self._current_cfg.link_or_merge(end_else, after_if_block)
 
         self._current_block = after_if_block
 
     def visit_while(self, node: nodes.While) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         old_curr = self._current_block
 
         # Handle "test" block
         test_block = self._current_cfg.create_block()
         test_block.add_statement(node.test)
         node.cfg_block = test_block
         self._current_cfg.link_or_merge(old_curr, test_block)
@@ -177,14 +224,18 @@
             child.accept(self)
         end_else = self._current_block
 
         self._current_cfg.link_or_merge(end_else, after_while_block)
         self._current_block = after_while_block
 
     def visit_for(self, node: nodes.For) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         old_curr = self._current_block
         old_curr.add_statement(node.iter)
         node.cfg_block = old_curr
 
         # Handle "test" block
         test_block = self._current_cfg.create_block()
         test_block.add_statement(node.target)
@@ -229,14 +280,18 @@
 
     def visit_raise(self, node: nodes.Raise) -> None:
         self._visit_jump(node)
 
     def _visit_jump(
         self, node: Union[nodes.Break, nodes.Continue, nodes.Return, nodes.Raise]
     ) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         old_curr = self._current_block
         for boundary, exits in reversed(self._control_boundaries):
             if isinstance(node, nodes.Raise):
                 exc_name = _get_raise_exc(node)
 
                 if exc_name in exits:
                     self._current_cfg.link(old_curr, exits[exc_name])
@@ -252,14 +307,18 @@
                 f"'{type(node).__name__}' outside"
                 f' {"function" if isinstance(node, nodes.Return) else "loop"}'
             )
         unreachable_block = self._current_cfg.create_block()
         self._current_block = unreachable_block
 
     def visit_tryexcept(self, node: nodes.TryExcept) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         if self._current_block.statements != []:
             self._current_block = self._current_cfg.create_block(self._current_block)
 
         node.cfg_block = self._current_block
 
         # Construct the exception handlers first
         # Initialize a temporary block to later merge with end_body
@@ -318,14 +377,18 @@
             self._control_boundaries.pop()
 
         self._current_cfg.link_or_merge(temp, end_body)
         self._current_cfg.multiple_link_or_merge(end_body, after_body)
         self._current_block = end_block
 
     def visit_with(self, node: nodes.With) -> None:
+        # When only creating cfgs for functions, _current_cfg will only be None outside of functions
+        if self._current_cfg is None:
+            return
+
         for context_node, name in node.items:
             self._current_block.add_statement(context_node)
             if name is not None:
                 self._current_block.add_statement(name)
 
         for child in node.body:
             child.accept(self)
```

### Comparing `python-ta-2.5.0/python_ta/checkers/forbidden_import_checker.py` & `python-ta-2.6.0/python_ta/checkers/forbidden_import_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/forbidden_io_function_checker.py` & `python-ta-2.6.0/python_ta/checkers/forbidden_io_function_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/forbidden_python_syntax_checker.py` & `python-ta-2.6.0/python_ta/checkers/forbidden_python_syntax_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/global_variables_checker.py` & `python-ta-2.6.0/python_ta/checkers/global_variables_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """checker for global variables
 """
 import re
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.base import UpperCaseStyle
+from pylint.checkers.base.name_checker.checker import DEFAULT_PATTERNS
+from pylint.checkers.utils import is_builtin
 
 from python_ta.utils import _is_in_main
 
 
 class GlobalVariablesChecker(BaseChecker):
     name = "global_variables"
     msgs = {
         "E9997": (
-            "Global variables must be constants in CSC108/CSC148: " "%s",
+            "Global variables must be constants or type aliases in CSC108/CSC148: " "%s",
             "forbidden-global-variables",
             "",
         )
     }
 
     # this is important so that your checker is executed before others
     priority = -1
@@ -27,21 +29,21 @@
         self.import_names = []
 
     def visit_global(self, node):
         args = "the keyword 'global' is used on line {}".format(node.lineno)
         self.add_message("forbidden-global-variables", node=node, args=args)
 
     def visit_assignname(self, node):
-        """Allow global constant variables (uppercase), but issue messages for
+        """Allow global constant variables (uppercase) and type aliases (type alias pattern), but issue messages for
         all other globals.
         """
         self._inspect_vars(node)
 
     def visit_name(self, node):
-        """Allow global constant variables (uppercase), but issue messages for
+        """Allow global constant variables (uppercase) and type aliases (type alias pattern), but issue messages for
         all other globals.
         """
         self._inspect_vars(node)
 
     def visit_import(self, node):
         """Save the names of imports, to prevent mistaking for global vars."""
         self._store_name_or_alias(node)
@@ -54,15 +56,15 @@
         for name_tuple in node.names:
             if name_tuple[1] is not None:
                 self.import_names.append(name_tuple[1])  # aliased names
             else:
                 self.import_names.append(name_tuple[0])  # no alias
 
     def _inspect_vars(self, node):
-        """Allows constant, global variables (i.e. uppercase), but issue
+        """Allows constant, global variables (i.e. uppercase) and type aliases (i.e. type alias pattern), but issue
         messages for all other global variables.
         """
         if hasattr(node, "name") and node.name in self.import_names:
             return
         if isinstance(node.frame(), nodes.Module) and not _is_in_main(node):
             node_list = _get_child_disallowed_global_var_nodes(node)
             for node in node_list:
@@ -75,26 +77,27 @@
                         node.name, node.lineno
                     )
                 self.add_message("forbidden-global-variables", node=node, args=args)
 
 
 def _get_child_disallowed_global_var_nodes(node):
     """Return a list of all top-level Name or AssignName nodes for a given
-    global, non-constant variable.
-
-    TODO: use the configured NamingStyle instead of hard-coded SnakeCaseStyle
-    for the CONST_NAME_RGX value.
+    global, non-constant and non-type alias variable.
     """
     node_list = []
     if (
         (
             isinstance(node, (nodes.AssignName, nodes.Name))
             and not isinstance(node.parent, nodes.Call)
         )
-        and not re.match(UpperCaseStyle.CONST_NAME_RGX, node.name)
+        and not (
+            re.match(UpperCaseStyle.CONST_NAME_RGX, node.name)
+            or re.match(DEFAULT_PATTERNS["typealias"], node.name)
+        )
+        and not is_builtin(node.name)
         and node.scope() is node.root()
     ):
         return [node]
 
     for child_node in node.get_children():
         node_list += _get_child_disallowed_global_var_nodes(child_node)
     return node_list
```

### Comparing `python-ta-2.5.0/python_ta/checkers/invalid_for_target_checker.py` & `python-ta-2.6.0/python_ta/checkers/invalid_for_target_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/invalid_range_index_checker.py` & `python-ta-2.6.0/python_ta/checkers/invalid_range_index_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/missing_space_in_doctest_checker.py` & `python-ta-2.6.0/python_ta/checkers/missing_space_in_doctest_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/one_iteration_checker.py` & `python-ta-2.6.0/python_ta/checkers/one_iteration_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/possibly_undefined_checker.py` & `python-ta-2.6.0/python_ta/checkers/possibly_undefined_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/pycodestyle_checker.py` & `python-ta-2.6.0/python_ta/checkers/pycodestyle_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/redundant_assignment_checker.py` & `python-ta-2.6.0/python_ta/checkers/redundant_assignment_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/shadowing_in_comprehension_checker.py` & `python-ta-2.6.0/python_ta/checkers/shadowing_in_comprehension_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/top_level_code_checker.py` & `python-ta-2.6.0/python_ta/checkers/top_level_code_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 
 from astroid import nodes
 from pylint.checkers import BaseChecker
 from pylint.checkers.base import UpperCaseStyle
+from pylint.checkers.base.name_checker.checker import DEFAULT_PATTERNS
 from pylint.checkers.utils import only_required_for_messages
 
 
 class TopLevelCodeChecker(BaseChecker):
     name = "top_level_code"
     msgs = {
         "E9992": (
@@ -22,15 +23,15 @@
 
     @only_required_for_messages("forbidden-top-level-code")
     def visit_module(self, node):
         for statement in node.body:
             if not (
                 _is_import(statement)
                 or _is_definition(statement)
-                or _is_constant_assignment(statement)
+                or _is_allowed_assignment(statement)
                 or _is_main_block(statement)
             ):
                 self.add_message("forbidden-top-level-code", node=statement, args=statement.lineno)
 
 
 # Helper functions
 def _is_import(statement) -> bool:
@@ -43,26 +44,30 @@
 def _is_definition(statement) -> bool:
     """
     Return whether or not <statement> is a function definition or a class definition.
     """
     return isinstance(statement, (nodes.FunctionDef, nodes.ClassDef))
 
 
-def _is_constant_assignment(statement) -> bool:
+def _is_allowed_assignment(statement) -> bool:
     """
-    Return whether or not <statement> is a constant assignment.
+    Return whether or not <statement> is a constant assignment or type alias assignment.
     """
     if not isinstance(statement, nodes.Assign):
         return False
 
     names = []
     for target in statement.targets:
         names.extend(node.name for node in target.nodes_of_class(nodes.AssignName, nodes.Name))
 
-    return all(re.match(UpperCaseStyle.CONST_NAME_RGX, name) for name in names)
+    return all(
+        re.match(UpperCaseStyle.CONST_NAME_RGX, name)
+        or re.match(DEFAULT_PATTERNS["typealias"], name)
+        for name in names
+    )
 
 
 def _is_main_block(statement) -> bool:
     """
     Return whether or not <statement> is the main block.
     """
     return (
```

### Comparing `python-ta-2.5.0/python_ta/checkers/type_annotation_checker.py` & `python-ta-2.6.0/python_ta/checkers/type_annotation_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/type_inference_checker.py` & `python-ta-2.6.0/python_ta/checkers/type_inference_checker.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/checkers/unnecessary_indexing_checker.py` & `python-ta-2.6.0/python_ta/checkers/unnecessary_indexing_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class UnnecessaryIndexingChecker(BaseChecker):
     # name is the same as file name but without _checker part
     name = "unnecessary_indexing"
     # use dashes for connecting words in message symbol
     msgs = {
         "E9994": (
-            "Index variable `%s` can be simplified by accessing the elements directly in the for loop or "
+            "Loop/comprehension index `%s` can be simplified by accessing the elements directly in the for loop or "
             "comprehension, "
             "for example, `for my_variable in %s`.",
             "unnecessary-indexing",
             "Used when you have an index variable in a for loop/comprehension "
             "where its only usage is to index the iterable",
         )
     }
@@ -28,32 +28,34 @@
 
     # pass in message symbol as a parameter of only_required_for_messages
     @only_required_for_messages("unnecessary-indexing")
     def visit_for(self, node: nodes.For) -> None:
         # Check if the iterable of the for loop is of the form "range(len(<variable-name>))".
         iterable = _iterable_if_range(node.iter)
         if iterable is not None and _is_unnecessary_indexing(node):
-            args = node.target.name, iterable
+            args = node.target.as_string(), iterable
             self.add_message("unnecessary-indexing", node=node.target, args=args)
 
     @only_required_for_messages("unnecessary-indexing")
     def visit_comprehension(self, node: nodes.Comprehension) -> None:
         iterable = _iterable_if_range(node.iter)
         if iterable is not None and _is_unnecessary_indexing(node):
-            args = node.target.name, iterable
+            args = node.target.as_string(), iterable
             self.add_message("unnecessary-indexing", node=node.target, args=args)
 
 
 # Helper functions
 def _is_unnecessary_indexing(node: Union[nodes.For, nodes.Comprehension]) -> bool:
     """Return whether the index variable in the for loop/comprehension is ONLY used to index the iterable.
 
     True if unnecessary usage, False otherwise or if index variable not used at all.
     """
-    index_nodes = _index_name_nodes(node.target.name, node)
+    index_nodes = []
+    for assign_name_node in node.target.nodes_of_class((nodes.AssignName, nodes.Name)):
+        index_nodes.extend(_index_name_nodes(assign_name_node.name, node))
     return all(_is_redundant(index_node, node) for index_node in index_nodes) and index_nodes
 
 
 def _iterable_if_range(node: nodes.NodeNG) -> Optional[str]:
     """Return the iterable's name if this node is in "range" form, or None otherwise.
 
     Check for three forms:
```

### Comparing `python-ta-2.5.0/python_ta/config/.pylintrc` & `python-ta-2.6.0/python_ta/config/.pylintrc`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [CUSTOM PYTA OPTIONS]
 
 # Make sure to register custom options tuple first in `python_ta/__init__.py`
 # ===========================================================
-# Default max amount of messages for reporter to display.
-pyta-number-of-messages = 5
+# Default max amount of messages for reporter to display. If the value is 0, all messages are displayed.
+pyta-number-of-messages = 0
 
 # (DEPRECATED: Use output-format option below.) Set the [REPORTS] output-format option instead.
 # pyta-reporter = HTMLReporter
 
 # Set the location of the template for HTMLreporter.
 pyta-template-file = template.html.jinja
 
@@ -62,24 +62,24 @@
     E0402,
     E0603, E0604, E0605,
     E0703, W0707,
     E1124, E1125, E1132, E1139, E1142,
     E1200, E1201, E1205, E1206,
     E1300, E1301, E1302, E1303, E1304,
     W1406,
-    E1507,
+    E1507, E1519,
     E1700, E1701,
     E9900,
-    W0120, W0150, W0177,
-    W0235, W0236, W0238, W0244, W0246,
+    W0120, W0131, W0150, W0177,
+    W0213, W0235, W0236, W0238, W0244, W0246,
     W0601, W0602, W0614, W0640,
     W1113, W1115,
     W1300, W1301, W1302, W1306, W1307,
     W1502, W1503, W1505, W1506, W1507, W1508, W1509, W1510, W1511, W1512, W1513, W1514, W1518,
-    C0105, C0131, C0132,
+    C0103, C0105, C0131, C0132,
     C0200, C0202, C0203, C0204, C0205, C0206, C0207, C0208,
     C0327, C0328,
     R0202, R0203, R0206,
     R0901, R0903, R0904, R0911,
     R1703, R1705, R1706, R1708, R1709, R1711, R1717, R1718, R1719, R1720, R1722, R1723, R1724,
     R1728, R1729, R1730, R1731,
     C1803,
@@ -92,15 +92,15 @@
     lambda-expressions,
     similarities,
     spelling,
     threading,
     unnecessary-dunder-call,
     unsupported_version,
     E2502, E2510, E2511, E2512, E2513, E2514, E2515,
-    missing-timeout
+    missing-timeout, positional-only-arguments-expected
 
 
 # Enable single-letter identifiers
 function-rgx = (([a-z][a-z0-9_]{0,30})|(_[a-z0-9_]*))$
 variable-rgx = (([a-z][a-z0-9_]{0,30})|(_[a-z0-9_]*)|([A-Z_][A-Z0-9_]*))$
 const-rgx    = (([A-Z_][A-Z0-9_]*)|(__.*__))$
 attr-rgx     = (([a-z][a-z0-9_]{0,30})|(_[a-z0-9_]*))$
```

### Comparing `python-ta-2.5.0/python_ta/config/messages_config.toml` & `python-ta-2.6.0/python_ta/config/messages_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 E0211 = "Every instance method (including %r) requires at least one parameter 'self', referring to the object on which this method is called. "
 E0213 = "The first parameter of every instance method (including %r) should always be called 'self'. "
 E0241 = "This class %r should not inherit from the same class multiple times."
 R0205 = "All classes inherit from object by default, so you do not need to specify this in the header for %r."
 W0211 = "The static method %r should not have 'self' as the first parameter."
 W0212 = "Since %s starts with an underscore, it is considered private and so should not be accessed outside of the class in which it is defined."
 W0222 = "This method's parameters must have the same name, order, and default arguments as %s %r method."
-W0223 = "The abstract method %r in class %r must be overridden within a concrete subclass."
+W0223 = "The abstract method %r in class %r must be overridden within the concrete subclass %r."
 W0231 = "Subclass '__init__' method should call the '__init__' method from its superclass %r."
 W0233 = "Subclass '__init__' method should call the '__init__' method of the superclass rather than some unrelated class %r."
 
 ["pylint.checkers.classes".SpecialMethodsChecker]
 E0301 = "An '__iter__' method must return an iterator, i.e an object with a '__next__' method."
 E0302 = "The special method %r expects to take %s parameters, but %d %s given."
 
@@ -83,19 +83,19 @@
 E0701 = "'except' blocks are checked top to bottom, so generic exception types should come after specific exception types. Otherwise, the block for the specific exception type will never be reached. (%s)"
 E0702 = "'raise' is used to raise exceptions. Anything else will lead to an error. (Raising %s)"
 E0704 = "This 'raise' statement must have an exception class or instance."
 E0710 = "This 'raise' statement is using a class that is not a subclass of Exception."
 E0711 = "You mean to raise 'NotImplementedError', which indicates that a method is abstract. "
 E0712 = "'except' expects a class that is a subclass of the Exception class (%s is not)."
 W0702 = "It's bad practice to use the 'except' keyword without passing an exception, since any and all expressions will be caught, which may lead to undetected errors in your code."
-W0703 = "It's bad practice to use 'except: %s' since any and all expressions will be caught, which may lead to undetected errors in your code."
 W0705 = "'except' blocks are checked top to bottom, so if we try to catch the same exception %s multiple times, only the first 'except' block for the exception will be reached."
 W0706 = "If the 'except' block uses 'raise' as its first or only statement, it will just raise back the exception immediately."
 W0711 = "'except' can handle multiple exceptions, but they have to be written as a tuple. For example, use 'except (A, B)' instead of 'except A %s B'"
 W0716 = "This is not a valid operation on exceptions. %s"
+W0718 = "It's bad practice to use 'except: %s' since any and all expressions will be caught, which may lead to undetected errors in your code."
 
 ["pylint.checkers.format".FormatChecker]
 W0301 = "You should remove this semicolon. In Python, statements are separated by starting each one on a new line."
 C0301 = "This line is %s characters long, exceeding the limit of %s characters."
 C0303 = "Trailing whitespace is poor formatting, and should be removed."
 C0304 = "By convention, each Python file should end with a blank line. To fix this, go down to the bottom of your file and press Enter/Return to add an empty line."
 C0321 = "Avoid writing multiple statements on a single line. This makes your code harder to understand."
@@ -146,9 +146,9 @@
 W0604 = "Every global variable can be referenced from the module level, so using the 'global' keyword at the module level has no effect."
 W0611 = "The import %s is unused, and so can be removed."
 W0612 = "The variable %s is unused and can be removed. If you intended to use it, there may be a typo elsewhere in the code."
 W0613 = "The parameter %r is unused. This may indicate you misspelled a parameter name in the function body. Otherwise, the parameter can be removed from the function without altering the program."
 W0621 = "The variable name %r already refers to a variable in the outer scope defined on line %s. This makes your code harder to read due to having to keep track of which variable we're referencing."
 W0622 = "%r is the name of a built-in function, and should not be overridden."
 W0631 = "Variables defined by a loop are only accessible within the loop, meaning the variable %r is possibly undefined."
-W0632 = "The sequence%s is being used to assign %d variables but contains %d values."
+W0632 = "The sequence %s is being used to assign %d target%s but contains %d value%s."
 W0642 = "%s is a local variable within the function. Reassigning this variable doesn't mutate any objects, and so has no effect after the function ends."
```

### Comparing `python-ta-2.5.0/python_ta/contracts/__init__.py` & `python-ta-2.6.0/python_ta/contracts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,65 +133,53 @@
 
 def add_class_invariants(klass: type) -> None:
     """Modify the given class to check representation invariants and method contracts."""
     if not ENABLE_CONTRACT_CHECKING or "__representation_invariants__" in klass.__dict__:
         # This means the class has already been decorated
         return
 
-    # Update representation invariants from this class' docstring and those of its superclasses.
-    rep_invariants: List[Tuple[str, CodeType]] = []
+    _set_invariants(klass)
 
-    # Iterate over all inherited classes except builtins
-    for cls in reversed(klass.__mro__):
-        if "__representation_invariants__" in cls.__dict__:
-            rep_invariants.extend(cls.__representation_invariants__)
-        elif cls.__module__ != "builtins":
-            assertions = parse_assertions(cls, parse_token="Representation Invariant")
-            # Try compiling assertions
-            for assertion in assertions:
-                try:
-                    compiled = compile(assertion, "<string>", "eval")
-                except:
-                    _debug(
-                        f"Warning: representation invariant {assertion} could not be parsed as a valid Python expression"
-                    )
-                    continue
-                rep_invariants.append((assertion, compiled))
-
-    setattr(klass, "__representation_invariants__", rep_invariants)
+    klass_mod = _get_module(klass)
+    cls_annotations = typing.get_type_hints(klass, localns=klass_mod.__dict__)
 
     def new_setattr(self: klass, name: str, value: Any) -> None:
         """Set the value of the given attribute on self to the given value.
 
         Check representation invariants for this class when not within an instance method of the class.
         """
-        klass_mod = _get_module(klass)
-        cls_annotations = typing.get_type_hints(klass, globalns=klass_mod.__dict__)
-
+        if not ENABLE_CONTRACT_CHECKING:
+            super(klass, self).__setattr__(name, value)
+            return
         if name in cls_annotations:
             try:
                 _debug(f"Checking type of attribute {attr} for {klass.__qualname__} instance")
                 check_type(name, value, cls_annotations[name])
             except TypeError:
                 raise AssertionError(
                     f"Value {_display_value(value)} did not match type annotation for attribute "
                     f"{name}: {_display_annotation(cls_annotations[name])}"
                 ) from None
-
+        original_attr_value_exists = False
+        original_attr_value = None
+        if hasattr(super(klass, self), name):
+            original_attr_value_exists = True
+            original_attr_value = super(klass, self).__getattribute__(name)
         super(klass, self).__setattr__(name, value)
-        curframe = inspect.currentframe()
-        callframe = inspect.getouterframes(curframe, 2)
-        frame_locals = callframe[1].frame.f_locals
+        frame_locals = inspect.currentframe().f_back.f_locals
         if self is not frame_locals.get("self"):
             # Only validating if the attribute is not being set in a instance/class method
-            klass_mod = _get_module(klass)
-            if klass_mod is not None and ENABLE_CONTRACT_CHECKING:
+            if klass_mod is not None:
                 try:
                     _check_invariants(self, klass, klass_mod.__dict__)
                 except PyTAContractError as e:
+                    if original_attr_value_exists:
+                        super(klass, self).__setattr__(name, original_attr_value)
+                    else:
+                        super(klass, self).__delattr__(name)
                     raise AssertionError(str(e)) from None
 
     for attr, value in klass.__dict__.items():
         if inspect.isroutine(value):
             if isinstance(value, (staticmethod, classmethod)):
                 # Don't check rep invariants for staticmethod and classmethod
                 setattr(klass, attr, check_contracts(value))
@@ -361,15 +349,15 @@
 def _check_class_type_annotations(klass: type, instance: Any) -> None:
     """Check that the type annotations for the class still hold.
 
     Precondition:
         - isinstance(instance, klass)
     """
     klass_mod = _get_module(klass)
-    cls_annotations = typing.get_type_hints(klass, globalns=klass_mod.__dict__)
+    cls_annotations = typing.get_type_hints(klass, localns=klass_mod.__dict__)
 
     for attr, annotation in cls_annotations.items():
         value = getattr(instance, attr)
         try:
             _debug(f"Checking type of attribute {attr} for {klass.__qualname__} instance")
             check_type(attr, value, annotation)
         except TypeError:
@@ -594,7 +582,43 @@
 
     Do nothing if DEBUG_CONTRACTS is False.
     """
     if not DEBUG_CONTRACTS:
         return
 
     print("[PyTA]", msg, file=sys.stderr)
+
+
+def _set_invariants(klass: type) -> None:
+    """Retrieve and set the representation invariants of this class"""
+    # Update representation invariants from this class' docstring and those of its superclasses.
+    rep_invariants: List[Tuple[str, CodeType]] = []
+
+    # Iterate over all inherited classes except builtins
+    for cls in reversed(klass.__mro__):
+        if "__representation_invariants__" in cls.__dict__:
+            rep_invariants.extend(cls.__representation_invariants__)
+        elif cls.__module__ != "builtins":
+            assertions = parse_assertions(cls, parse_token="Representation Invariant")
+            # Try compiling assertions
+            for assertion in assertions:
+                try:
+                    compiled = compile(assertion, "<string>", "eval")
+                except:
+                    _debug(
+                        f"Warning: representation invariant {assertion} could not be parsed as a valid Python expression"
+                    )
+                    continue
+                rep_invariants.append((assertion, compiled))
+
+    setattr(klass, "__representation_invariants__", rep_invariants)
+
+
+def validate_invariants(obj: object) -> None:
+    """Check that the representation invariants of obj are satisfied."""
+    klass = obj.__class__
+    klass_mod = _get_module(klass)
+
+    try:
+        _check_invariants(obj, klass, klass_mod.__dict__)
+    except PyTAContractError as e:
+        raise AssertionError(str(e)) from None
```

### Comparing `python-ta-2.5.0/python_ta/contracts/__main__.py` & `python-ta-2.6.0/python_ta/contracts/__main__.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/debug/accumulation_table.py` & `python-ta-2.6.0/python_ta/debug/accumulation_table.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/patches/checkers.py` & `python-ta-2.6.0/python_ta/patches/checkers.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/patches/error_messages.py` & `python-ta-2.6.0/python_ta/patches/error_messages.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/patches/messages.py` & `python-ta-2.6.0/python_ta/patches/messages.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/patches/transforms.py` & `python-ta-2.6.0/python_ta/patches/transforms.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/color_reporter.py` & `python-ta-2.6.0/python_ta/reporters/color_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/core.py` & `python-ta-2.6.0/python_ta/reporters/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module provides the core functionality for all PythonTA reporters.
 """
 import os.path
 import sys
 from collections import defaultdict
+from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 from astroid import NodeNG
 from pylint.message import Message
 from pylint.message.message_definition import MessageDefinition
 from pylint.reporters import BaseReporter
 from pylint.reporters.ureports.nodes import BaseLayout
@@ -36,15 +37,22 @@
             # The following are DEPRECATED and will be removed in a future release.
             "line_end": self.message.end_line,
             "column_end": self.message.end_column,
         }
 
 
 # Messages without a source code line to highlight
-NO_SNIPPET = {"invalid-name"}
+NO_SNIPPET = {
+    "invalid-name",
+    "unknown-option-value",
+    "module-name-violation",
+    "config-parse-error",
+    "useless-option-value",
+    "unrecognized-option",
+}
 
 
 class PythonTaReporter(BaseReporter):
     """Abstract superclass for all PythonTA reporters.
 
     Reminder: see pylint BaseReporter for other instance variables.
     """
@@ -211,26 +219,33 @@
         By default, returns the text itself.
         """
         return text
 
     # Event callbacks
     def on_set_current_module(self, module: str, filepath: Optional[str]) -> None:
         """Hook called when a module starts to be analysed."""
+        # First, check if `module` is the name of a config file and if so, make filepath the
+        # corresponding path to that config file.
+        possible_config_path = Path(os.path.expandvars(module)).expanduser()
+
+        if possible_config_path.exists() and filepath is None:
+            filepath = str(possible_config_path)
+
         # Skip if filepath is None
         if filepath is None:
             return
 
         self.module_name = module
         self.current_file = filepath
 
         if self.current_file not in self.messages:
             self.messages[self.current_file] = []
 
         with open(filepath, encoding="utf-8") as f:
-            self.source_lines = [line.rstrip() for line in f.readlines()]
+            self.source_lines = [line.rstrip("\r\n") for line in f.readlines()]
 
     def on_close(self, stats, previous_stats):
         """Hook called when a module finished analyzing.
 
         Close the reporter's output stream (if not sys.stdout).
         """
         if self.out is not sys.stdout:
```

### Comparing `python-ta-2.5.0/python_ta/reporters/html_reporter.py` & `python-ta-2.6.0/python_ta/reporters/html_reporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,18 +128,16 @@
             file=sys.stderr,
         )
 
     @classmethod
     def _colourify(cls, colour_class: str, text: str) -> str:
         """Return a colourized version of text, using colour_class."""
         colour = cls._COLOURING[colour_class]
-        new_text = text.lstrip(" ")
-        space_count = len(text) - len(new_text)
-        new_text = new_text.replace(" ", cls._SPACE)
+        new_text = text.replace(" ", cls._SPACE)
         if "-line" not in colour_class:
             new_text = highlight(
                 new_text,
                 PythonLexer(),
                 HtmlFormatter(nowrap=True, lineseparator="", classprefix="pygments-"),
             )
 
-        return (space_count * cls._SPACE) + colour + new_text + cls._COLOURING["reset"]
+        return colour + new_text + cls._COLOURING["reset"]
```

### Comparing `python-ta-2.5.0/python_ta/reporters/json_reporter.py` & `python-ta-2.6.0/python_ta/reporters/json_reporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,12 +29,28 @@
         been aggregated.
         """
         output = []
         for k, msgs in self.messages.items():
             output.append(
                 {
                     "filename": k,
-                    "msgs": [msg.to_dict() for msg in msgs],
+                    "msgs": self._output_messages(msgs),
                 }
             )
 
         self.writeln(json.dumps(output, indent=4))
+
+    def _output_messages(self, msgs: List[NewMessage]) -> List[Dict]:
+        """Returns a list of dictionaries containing formatted error messages."""
+        max_messages = self.linter.config.pyta_number_of_messages
+        num_occurrences = {msg.message.msg_id: 0 for msg in msgs}
+        output_lst = []
+
+        for msg in msgs:
+            if max_messages == 0 or num_occurrences[msg.message.msg_id] < max_messages:
+                output_lst.append(msg.to_dict())
+            num_occurrences[msg.message.msg_id] += 1
+
+        for msg_dict in output_lst:
+            msg_dict["number_of_occurrences"] = num_occurrences[msg_dict["msg_id"]]
+
+        return output_lst
```

### Comparing `python-ta-2.5.0/python_ta/reporters/plain_reporter.py` & `python-ta-2.6.0/python_ta/reporters/plain_reporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,20 +55,24 @@
         max_messages = self.linter.config.pyta_number_of_messages
 
         result = ""
         for msg_id in messages:
             result += self._colourify("bold", msg_id)
             result += self._colourify("bold", " ({})  ".format(messages[msg_id][0].symbol))
             result += "Number of occurrences: {}.".format(len(messages[msg_id]))
-            if max_messages != float("inf") and max_messages < len(messages[msg_id]):
+            if (
+                max_messages != 0
+                and max_messages != float("inf")
+                and max_messages < len(messages[msg_id])
+            ):
                 result += " (First {} shown).".format(max_messages)
             result += self._BREAK
 
             for i, msg in enumerate(messages[msg_id]):
-                if i == max_messages:
+                if max_messages != 0 and i == max_messages:
                     break
 
                 # Use only explanation, without redundant accessory information
                 msg_truncated = msg.msg.split("\n")[0]
                 result += 2 * self._SPACE
                 result += (
                     self._colourify("bold", "[Line {}] {}".format(msg.line, msg_truncated))
```

### Comparing `python-ta-2.5.0/python_ta/reporters/stat_reporter.py` & `python-ta-2.6.0/python_ta/reporters/stat_reporter.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/templates/jquery-3.2.1.min.js` & `python-ta-2.6.0/python_ta/reporters/templates/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/templates/pyta_logo_markdown.png` & `python-ta-2.6.0/python_ta/reporters/templates/pyta_logo_markdown.png`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/templates/script.js` & `python-ta-2.6.0/python_ta/reporters/templates/script.js`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/reporters/templates/stylesheet.css` & `python-ta-2.6.0/python_ta/reporters/templates/stylesheet.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 body {
   margin: 0;
-  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto,
-    Helvetica Neue, Helvetica, Ubuntu, Arial, sans-serif;
+  font-family:
+    -apple-system,
+    BlinkMacSystemFont,
+    Segoe UI,
+    Roboto,
+    Helvetica Neue,
+    Helvetica,
+    Ubuntu,
+    Arial,
+    sans-serif;
   background: rgba(71, 118, 230, 0.77);
   background: -webkit-linear-gradient(
     0deg,
     rgba(49, 48, 178, 0.62),
     rgba(71, 128, 230, 0.77)
   );
   background: linear-gradient(
@@ -159,15 +167,17 @@
   align-items: center;
   margin-top: 7px;
 }
 
 .error-instance {
   display: grid;
   background: #fff;
-  box-shadow: 0 0 4px rgba(0, 0, 0, 0.1), 0 4px 7px rgba(0, 0, 0, 0.1);
+  box-shadow:
+    0 0 4px rgba(0, 0, 0, 0.1),
+    0 4px 7px rgba(0, 0, 0, 0.1);
   padding: 8px 16px;
   margin-bottom: 5px;
   border-radius: 3px;
 }
 
 .error-link {
   line-height: 35px;
```

### Comparing `python-ta-2.5.0/python_ta/reporters/templates/template.html.jinja` & `python-ta-2.6.0/python_ta/reporters/templates/template.html.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                                     {% if num_occurrences == 1 %}
                                      occurrence.
                                     {% else %}
                                      occurrences.
                                     {% endif %}
                                     </span>
                                     <span class="shown">
-                                    {% if limit < num_occurrences %}
+                                    {% if 0 < limit < num_occurrences %}
                                      (First {{ limit }} shown).
                                     {% endif %}
                                     </span>
                                     <span class="slider">
                                         <button>
                                             <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="30">
                                                 <g transform="scale(0.13 0.13)">
@@ -137,35 +137,37 @@
                                                 </g>
                                             </svg>
                                         </button>
                                     </span>
                                 </div>
                                 <div class="message-container collapsible expanded">
                                     {% for indiv in occurrences %}
-                                    <div class="message">
-                                        <p class="message-name">
-                                            [Line {{ indiv.line }}] {{ indiv.msg }}
-                                            <span class="slider">
-                                                <button style="float: right;">
-                                                    <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="20">
-                                                        <g transform="scale(0.13 0.13)">
-                                                            <path d="M 10 30 l 40 40 l 40 -40" stroke="#777777" stroke-width="15px" fill="transparent"/>
-                                                        </g>
-                                                    </svg>
-                                                </button>
-                                            </span>
-                                        </p>
-                                        {% if indiv.snippet != '' %}
-                                        <div class="collapsible expanded message-snippet-container">
-                                          <pre class="message-snippet">{{ indiv.snippet }}</pre>
-                                        </div>
-                                        {% else %}
-                                        <span class="empty-placeholder">{{ reporter.no_snippet }}</span>
-                                        {% endif %}
-                                    </div>
+                                        {% if limit == 0 or loop.index0 < limit %}
+                                            <div class="message">
+                                                <p class="message-name">
+                                                    [Line {{ indiv.line }}] {{ indiv.msg }}
+                                                    <span class="slider">
+                                                        <button style="float: right;">
+                                                            <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="20">
+                                                                <g transform="scale(0.13 0.13)">
+                                                                    <path d="M 10 30 l 40 40 l 40 -40" stroke="#777777" stroke-width="15px" fill="transparent"/>
+                                                                </g>
+                                                            </svg>
+                                                        </button>
+                                                    </span>
+                                                </p>
+                                                {% if indiv.snippet != '' %}
+                                                <div class="collapsible expanded message-snippet-container">
+                                                  <pre class="message-snippet">{{ indiv.snippet }}</pre>
+                                                </div>
+                                                {% else %}
+                                                <span class="empty-placeholder">{{ reporter.no_snippet }}</span>
+                                                {% endif %}
+                                            </div>
+                                       {% endif %}
                                     {% endfor %}
                                 </div>
                             </div>
                             {% else %}
                             <span class="empty-placeholder">{{ reporter.no_err_message }}</span>
                             {% endfor %}
                         </div>
@@ -197,52 +199,53 @@
                                         {% if num_occurrences == 1 %}
                                             occurrence.
                                         {% else %}
                                             occurrences.
                                         {% endif %}
                                     </span>
                                     <span class="shown">
-                                    {% if limit < num_occurrences %}
+                                    {% if 0 < limit < num_occurrences %}
                                      (First {{ limit }} shown).
                                     {% endif %}
                                     </span>
                                     <span class="slider">
                                         <button>
                                             <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="30">
                                                 <g transform="scale(0.13 0.13)">
                                                     <path d="M 10 30 l 40 40 l 40 -40" stroke="#3669c7" stroke-width="15px" fill="transparent"/>
                                                 </g>
                                             </svg>
                                         </button>
                                     </span>
                                 </div>
-
                                 <div class="message-container collapsible expanded">
                                     {% for indiv in occurrences %}
-                                    <div class="message">
-                                        <p class="message-name">
-                                            [Line {{ indiv.line }}] {{ indiv.msg }}
-                                            <span class="slider">
-                                                <button style="float: right;">
-                                                    <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="20">
-                                                        <g transform="scale(0.13 0.13)">
-                                                            <path d="M 10 30 l 40 40 l 40 -40" stroke="#777777" stroke-width="15px" fill="transparent"/>
-                                                        </g>
-                                                    </svg>
-                                                </button>
-                                            </span>
-                                        </p>
-                                        <div class="collapsible expanded message-snippet-container">
-                                          {% if indiv.snippet != '' %}
-                                          <pre class="message-snippet">{{ indiv.snippet }}</pre>
-                                          {% else %}
-                                          <span class="empty-placeholder">{{ reporter.no_snippet }}</span>
-                                          {% endif %}
-                                        </div>
-                                    </div>
+                                        {% if limit == 0 or loop.index0 < limit %}
+                                            <div class="message">
+                                                <p class="message-name">
+                                                    [Line {{ indiv.line }}] {{ indiv.msg }}
+                                                    <span class="slider">
+                                                        <button style="float: right;">
+                                                            <svg class="collapse-trigger" viewBox="0 1 10 10" width="60" height="20">
+                                                                <g transform="scale(0.13 0.13)">
+                                                                    <path d="M 10 30 l 40 40 l 40 -40" stroke="#777777" stroke-width="15px" fill="transparent"/>
+                                                                </g>
+                                                            </svg>
+                                                        </button>
+                                                    </span>
+                                                </p>
+                                                <div class="collapsible expanded message-snippet-container">
+                                                  {% if indiv.snippet != '' %}
+                                                  <pre class="message-snippet">{{ indiv.snippet }}</pre>
+                                                  {% else %}
+                                                  <span class="empty-placeholder">{{ reporter.no_snippet }}</span>
+                                                  {% endif %}
+                                                </div>
+                                            </div>
+                                        {% endif %}
                                     {% endfor %}
                                 </div>
 
                             </div>
                             {% else %}
                             <span class="empty-placeholder">{{ reporter.no_err_message }}</span>
                             {% endfor %}
```

#### html2text {}

```diff
@@ -20,38 +20,38 @@
 **** {{ reporter.code_err_title }}          ****
 {% for message_id in messages[0] %} {% set occurrences = messages[0]
 [message_id] %}
 }}>
 {% set mid = message_id.lower() %}  ❐_{{_message_id_}}_({{_occurrences
 [0].symbol_}})_(Learn_More)  {% set num_occurrences = occurrences|length %}  {
 { num_occurrences }} {% if num_occurrences == 1 %} occurrence. {% else %}
-occurrences. {% endif %}   {% if limit < num_occurrences %} (First {{ limit }}
-shown). {% endif %}
-{% for indiv in occurrences %}
+occurrences. {% endif %}   {% if 0 < limit < num_occurrences %} (First {{ limit
+}} shown). {% endif %}
+{% for indiv in occurrences %} {% if limit == 0 or loop.index0 < limit %}
 [Line {{ indiv.line }}] {{ indiv.msg }}
 {% if indiv.snippet != '' %}
 {{ indiv.snippet }}
 {% else %} {{ reporter.no_snippet }} {% endif %}
-{% endfor %}
+{% endif %} {% endfor %}
 {% else %} {{ reporter.no_err_message }} {% endfor %}
 
 **** {{ reporter.style_err_title }}          ****
 {% for message_id, occurrences in messages[1].items() %}
 }}>
 {% set mid = message_id.lower() %}  ❐_{{_message_id_}}_({{_occurrences
 [0].symbol_}})_(Learn_More)  {% set num_occurrences = occurrences|length %}  {
 { num_occurrences }} {% if num_occurrences == 1 %} occurrence. {% else %}
-occurrences. {% endif %}   {% if limit < num_occurrences %} (First {{ limit }}
-shown). {% endif %}
-{% for indiv in occurrences %}
+occurrences. {% endif %}   {% if 0 < limit < num_occurrences %} (First {{ limit
+}} shown). {% endif %}
+{% for indiv in occurrences %} {% if limit == 0 or loop.index0 < limit %}
 [Line {{ indiv.line }}] {{ indiv.msg }}
 {% if indiv.snippet != '' %}
 {{ indiv.snippet }}
 {% else %} {{ reporter.no_snippet }} {% endif %}
-{% endfor %}
+{% endif %} {% endfor %}
 {% else %} {{ reporter.no_err_message }} {% endfor %}
   {% endfor %}
 PythonTA is maintained by Professor David Liu and students at the University of
 Toronto.
 Found a bug? Report it to Prof._Liu!
 PyTA_Help_Documentation
 [PyTA_logo] ___
```

### Comparing `python-ta-2.5.0/python_ta/transforms/ExprWrapper.py` & `python-ta-2.6.0/python_ta/transforms/ExprWrapper.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/transforms/setendings.py` & `python-ta-2.6.0/python_ta/transforms/setendings.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/transforms/type_inference_visitor.py` & `python-ta-2.6.0/python_ta/transforms/type_inference_visitor.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/transforms/z3_visitor.py` & `python-ta-2.6.0/python_ta/transforms/z3_visitor.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/typecheck/base.py` & `python-ta-2.6.0/python_ta/typecheck/base.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/typecheck/errors.py` & `python-ta-2.6.0/python_ta/typecheck/errors.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/typecheck/type_store.py` & `python-ta-2.6.0/python_ta/typecheck/type_store.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/typecheck/typeshed/README.md` & `python-ta-2.6.0/python_ta/typecheck/typeshed/README.md`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/typecheck/typeshed/builtins.pyi` & `python-ta-2.6.0/python_ta/typecheck/typeshed/builtins.pyi`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/upload.py` & `python-ta-2.6.0/python_ta/upload.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/util/monad.py` & `python-ta-2.6.0/python_ta/util/monad.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta/utils.py` & `python-ta-2.6.0/python_ta/utils.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/python_ta.egg-info/PKG-INFO` & `python-ta-2.6.0/python_ta.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: python-ta
-Version: 2.5.0
+Version: 2.6.0
 Summary: Code checking tool for teaching Python
-Home-page: https://github.com/pyta-uoft/pyta
-Author: David Liu
-Author-email: david@cs.toronto.edu
+Author-email: David Liu <david@cs.toronto.edu>
 License: MIT
-Requires-Python: ~=3.8
+Project-URL: Homepage, https://github.com/pyta-uoft/pyta
+Project-URL: Documentation, https://www.cs.toronto.edu/~david/pyta/
+Project-URL: Repository, https://github.com/pyta-uoft/pyta.git
+Project-URL: Changelog, https://github.com/pyta-uoft/pyta/blob/master/CHANGELOG.md
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: z3
 License-File: LICENSE
 
 # PyTA
 
@@ -97,20 +99,22 @@
 Craig Katsube,
 Rebecca Kay,
 Christopher Koehler,
 David Kim,
 Simeon Krastnikov,
 Ryan Lee,
 Hayley Lin,
+Bruce Liu,
 Wendy Liu,
 Yibing (Amy) Lu,
 Shweta Mogalapalli,
 Ignas Panero Armoska,
 Justin Park,
 Harshkumar Patel,
 Amr Sharaf,
 Richard Shi,
 Kavin Singh,
 Alexey Strokach,
 Sophy Sun,
+Sarah Wang
 Jasmine Wu,
 Philippe Yu,
```

### Comparing `python-ta-2.5.0/python_ta.egg-info/SOURCES.txt` & `python-ta-2.6.0/python_ta.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 python_ta/__init__.py
 python_ta/__main__.py
 python_ta/upload.py
 python_ta/utils.py
 python_ta.egg-info/PKG-INFO
 python_ta.egg-info/SOURCES.txt
 python_ta.egg-info/dependency_links.txt
 python_ta.egg-info/entry_points.txt
 python_ta.egg-info/not-zip-safe
 python_ta.egg-info/requires.txt
 python_ta.egg-info/top_level.txt
 python_ta/cfg/__init__.py
+python_ta/cfg/cfg_generator.py
 python_ta/cfg/graph.py
 python_ta/cfg/visitor.py
 python_ta/checkers/__init__.py
 python_ta/checkers/forbidden_import_checker.py
 python_ta/checkers/forbidden_io_function_checker.py
 python_ta/checkers/forbidden_python_syntax_checker.py
 python_ta/checkers/global_variables_checker.py
 python_ta/checkers/invalid_for_target_checker.py
+python_ta/checkers/invalid_name_checker.py
 python_ta/checkers/invalid_range_index_checker.py
 python_ta/checkers/missing_space_in_doctest_checker.py
 python_ta/checkers/one_iteration_checker.py
 python_ta/checkers/possibly_undefined_checker.py
 python_ta/checkers/pycodestyle_checker.py
 python_ta/checkers/redundant_assignment_checker.py
 python_ta/checkers/shadowing_in_comprehension_checker.py
@@ -68,30 +69,26 @@
 python_ta/typecheck/base.py
 python_ta/typecheck/errors.py
 python_ta/typecheck/type_store.py
 python_ta/typecheck/typeshed/README.md
 python_ta/typecheck/typeshed/builtins.pyi
 python_ta/util/__init__.py
 python_ta/util/monad.py
-sample_usage/__init__.py
-sample_usage/draw_cfg.py
-sample_usage/draw_tnodes.py
-sample_usage/print_ast.py
-sample_usage/print_nodes.py
-sample_usage/print_table.py
-sample_usage/pyta_stats.py
-sample_usage/stats_analysis.py
 tests/__init__.py
 tests/custom_hypothesis_support.py
 tests/test_check.py
 tests/test_class_contracts.py
 tests/test_contracts.py
+tests/test_contracts_attr_value_restoration.py
+tests/test_contracts_type_alias_abstract_network.py
+tests/test_contracts_type_alias_abstract_ring.py
 tests/test_examples.py
 tests/test_setendings.py
 tests/test_subclass_contracts.py
+tests/test_validate_invariants.py
 tests/test_z3_visitor.py
 tests/test_type_constraints/__init__.py
 tests/test_type_constraints/test_tnode_structure.py
 tests/test_type_constraints/test_unify.py
 tests/test_type_inference/__init__.py
 tests/test_type_inference/test_annassign.py
 tests/test_type_inference/test_assign.py
```

### Comparing `python-ta-2.5.0/tests/custom_hypothesis_support.py` & `python-ta-2.6.0/tests/custom_hypothesis_support.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_check.py` & `python-ta-2.6.0/tests/test_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         assert "astroid-error" not in {
             msg.message.symbol for msg in messages
         }, f"astroid-error encountered for {filename}"
 
 
 def test_check_on_file():
     """Test files"""
-    _inputs = [["nodes/name.py"], ["nodes/dict.py", "nodes/const.py"]]
+    _inputs = [["examples/nodes/name.py"], ["examples/nodes/dict.py", "examples/nodes/const.py"]]
     for item in _inputs:
         python_ta.check_all(
             item,
             config={
                 "output-format": "python_ta.reporters.PlainReporter",
                 "pyta-error-permission": "no",
                 "pyta-file-permission": "no",
@@ -42,16 +42,16 @@
 def test_check_on_bad_input():
     """Test bad inputs. In all cases, pyta should recover.
     Any valid files, if any, should be checked.
     """
     _inputs = [
         [222],
         222,
-        ["nodes/dict.py nodes/const.py"],
-        [222, "examples/inline_config_comment.py", "nodes/dict.py"],
+        ["examples/nodes/dict.py examples/nodes/const.py"],
+        [222, "examples/inline_config_comment.py", "examples/nodes/dict.py"],
         ["file_does_not_exist"],
     ]
     for item in _inputs:
         python_ta.check_all(
             item,
             config={
                 "output-format": "python_ta.reporters.PlainReporter",
@@ -59,15 +59,15 @@
                 "pyta-file-permission": "no",
             },
         )
 
 
 def test_check_with_config():
     """Test inputs along with a config arg."""
-    _inputs = [["nodes/const.py"], ["nodes"]]
+    _inputs = [["examples/nodes/const.py"], ["examples/nodes"]]
     CONFIG = {
         # [ELIF]
         "max-nested-blocks": 4,
         # [FORMAT]
         "max-line-length": 80,
         # [FORBIDDEN IMPORT]
         "allowed-import-modules": ["doctest", "unittest", "hypothesis", "python_ta"],
@@ -168,15 +168,15 @@
     }
     for item in _inputs:
         python_ta.check_all(item, config=CONFIG)
 
 
 def test_check_saves_file() -> None:
     """Test whether or not specifiying an output properly saves a file"""
-    _inputs = [["nodes/name.py"]]
+    _inputs = [["examples/nodes/name.py"]]
     for item in _inputs:
         # Note that the reporter output will be created in the main directory
         python_ta.check_all(item, output="pyta_output.html")
 
     file_exists = path.exists("pyta_output.html")
 
     assert file_exists
@@ -191,15 +191,15 @@
     # To prevent any any browser/server code running when running Pytest to avoid CI timeouts
     import webbrowser
     from http.server import HTTPServer
 
     webbrowser.open = Mock(return_value=None)
     HTTPServer.handle_request = Mock(return_value=None)
 
-    _inputs = [["nodes/name.py"]]
+    _inputs = [["examples/nodes/name.py"]]
     for item in _inputs:
         # Note that the reporter output *would have been* created in the main directory
         python_ta.check_all(item)
 
     file_exists = path.exists("pyta_output.html")
 
     assert not file_exists
@@ -230,15 +230,15 @@
     output = subprocess.run(
         [
             sys.executable,
             "-m",
             "python_ta",
             "--config",
             "tests/test.pylintrc",
-            "nodes/name.py",
+            "examples/nodes/name.py",
         ]
     )
 
     assert output.returncode != 0
 
 
 def test_check_exit_zero() -> None:
@@ -249,15 +249,15 @@
         [
             sys.executable,
             "-m",
             "python_ta",
             "--exit-zero",
             "--config",
             "tests/test.pylintrc",
-            "nodes/name.py",
+            "examples/nodes/name.py",
         ]
     )
 
     assert output.returncode == 0
 
 
 def test_check_version() -> None:
```

### Comparing `python-ta-2.5.0/tests/test_class_contracts.py` & `python-ta-2.6.0/tests/test_class_contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,23 +236,21 @@
     assert (
         '"Pizza" representation invariant "len(self.ingredients) > 0" was violated for instance attributes {'
         "radius: 10, "
         "ingredients: []}" == msg
     )
 
 
-def test_pizza_invalid_disable_contract_checking() -> None:
+def test_pizza_invalid_disable_contract_checking(disable_contract_checking) -> None:
     """
     Test the Pizza representation invariant on an invalid instance but with ENABLE_CONTRACT_CHECKING = False so
     no error is raised.
     """
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
     pizza = Pizza(radius=10, ingredients=[])
     assert pizza.radius == 10 and pizza.ingredients == []
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True  # Reset default value to True
 
 
 def test_set_wrapper_valid() -> None:
     """
     Test the SetWrapper representation invariant on a valid instance.
     """
     my_set = SetWrapper(set={1, 2, 3})
```

### Comparing `python-ta-2.5.0/tests/test_contracts.py` & `python-ta-2.6.0/tests/test_contracts.py`

 * *Files 14% similar despite different names*

```diff
@@ -119,25 +119,23 @@
     def nullary() -> bool:
         return 1
 
     with pytest.raises(AssertionError):
         nullary()
 
 
-def test_nullary_int_bool_disable_contract_checking() -> None:
+def test_nullary_int_bool_disable_contract_checking(disable_contract_checking) -> None:
     """Calling a nullary function with incorrect return type and with ENABLE_CONTRACT_CHECKING disabled so no error
     is raised."""
 
     @check_contracts
     def nullary() -> int:
         return True
 
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
     nullary()
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True  # Reset default value to True
 
 
 def test_nullary_no_return_type() -> None:
     """Calling a nullary function with no specified return type passes."""
 
     @check_contracts
     def nullary():
@@ -229,22 +227,20 @@
     def parameter_bool(result: bool) -> None:
         return None
 
     with pytest.raises(AssertionError):
         parameter_bool(1)
 
 
-def test_parameter_int_bool_disable_contract_checking() -> None:
+def test_parameter_int_bool_disable_contract_checking(disable_contract_checking) -> None:
     @check_contracts
     def parameter_int(num: int) -> None:
         return None
 
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
     parameter_int(True)
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True  # Reset default value to True
 
 
 @check_contracts
 def _my_sum_one_precondition(numbers: List[int]) -> int:
     """Return the sum of a list of numbers.
 
     Precondition: len(numbers) > 2
@@ -270,20 +266,18 @@
     with pytest.raises(AssertionError) as excinfo:
         _my_sum_one_precondition([1])
 
     msg = str(excinfo.value)
     assert "len(numbers) > 2" in msg
 
 
-def test_my_sum_one_disable_contract_checking() -> None:
+def test_my_sum_one_disable_contract_checking(disable_contract_checking) -> None:
     """Calling _my_sum_one_precondition with a value that violates the precondition but with ENABLE_CONTRACT_CHECKING
     = False so no error is raised"""
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
     _my_sum_one_precondition([1])
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True  # Reset default value to True
 
 
 # Checking to see if functions we defined are in-scope for preconditions
 
 
 def is_even(lst: List[int]) -> bool:
     return all([(not x & 1) for x in lst])
@@ -445,21 +439,19 @@
     with pytest.raises(AssertionError) as excinfo:
         _get_double_invalid(5)
 
     msg = str(excinfo.value)
     assert "$return_value == num * 2" in msg
 
 
-def test_get_double_disabled_contract_checking() -> None:
+def test_get_double_disabled_contract_checking(disable_contract_checking) -> None:
     """Test that calling the invalid implementation of _get_double does NOT raise an AssertionError when
     ENABLE_CONTRACT_CHECKING is False.
     """
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
     assert _get_double_invalid(5) == 11
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True  # Reset default value to True
 
 
 # Test that postcondition checks involving function parameters pass and fail as expected
 @check_contracts
 def _add_to_set_valid(num_set: Set[int], new_num: int) -> None:
     """
     Add a number to the provided set if the number does not already exist in the set.
@@ -682,26 +674,31 @@
     """
     from tests.fixtures.contracts.modules_not_in_arg import run
 
     with pytest.raises(AssertionError):
         run()
 
 
-@pytest.fixture()
-def disable_contract_checking():
-    """Fixture for setting python_ta.contracts.ENABLE_CONTRACT_CHECKING = False."""
-    import python_ta.contracts
-
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = False
-    yield
-    python_ta.contracts.ENABLE_CONTRACT_CHECKING = True
-
-
 def test_enable_contract_checking_false(disable_contract_checking) -> None:
     """Test that check_contracts does nothing when ENABLE_CONTRACT_CHECKING is False."""
 
     @check_contracts
     def unary2(arg: int) -> int:
         return arg
 
     # No error should be raised even though the argument is the wrong type
     assert unary2("wrong type!") == "wrong type!"
+
+
+def test_invalid_attr_type_disable_contract_checking(disable_contract_checking) -> None:
+    """
+    Test that a Person object is created with an attribute value that doesn't match the specified type annotation but
+    with ENABLE_CONTRACT_CHECKING = False so no error is raised.
+    """
+
+    @check_contracts
+    class Person:
+        age: int
+
+    my_person = Person()
+    my_person.age = "John"
+    assert my_person.age == "John"
```

### Comparing `python-ta-2.5.0/tests/test_examples.py` & `python-ta-2.6.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_setendings.py` & `python-ta-2.6.0/tests/test_setendings.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_subclass_contracts.py` & `python-ta-2.6.0/tests/test_subclass_contracts.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_constraints/test_tnode_structure.py` & `python-ta-2.6.0/tests/test_type_constraints/test_tnode_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import *
 from typing import ForwardRef, _GenericAlias
 
 import pytest
 from astroid import nodes
 
+from examples.sample_usage.draw_tnodes import gen_graph_from_nodes
 from python_ta.typecheck.base import TypeConstraints, TypeFail, _TNode
-from sample_usage.draw_tnodes import gen_graph_from_nodes
 
 from .. import custom_hypothesis_support as cs
 
 
 def tc_to_disjoint(tc: TypeConstraints) -> List[Set[Union[type, str]]]:
     tnode_list = tc._nodes.copy()
     disjoint_set = []
```

### Comparing `python-ta-2.5.0/tests/test_type_constraints/test_unify.py` & `python-ta-2.6.0/tests/test_type_constraints/test_unify.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_annassign.py` & `python-ta-2.6.0/tests/test_type_inference/test_annassign.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_assign.py` & `python-ta-2.6.0/tests/test_type_inference/test_assign.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_assign_tuple.py` & `python-ta-2.6.0/tests/test_type_inference/test_assign_tuple.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_attribute.py` & `python-ta-2.6.0/tests/test_type_inference/test_attribute.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_binops.py` & `python-ta-2.6.0/tests/test_type_inference/test_binops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_boolops.py` & `python-ta-2.6.0/tests/test_type_inference/test_boolops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_classdef.py` & `python-ta-2.6.0/tests/test_type_inference/test_classdef.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_compare.py` & `python-ta-2.6.0/tests/test_type_inference/test_compare.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_const.py` & `python-ta-2.6.0/tests/test_type_inference/test_const.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_dict.py` & `python-ta-2.6.0/tests/test_type_inference/test_dict.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_dictcomp.py` & `python-ta-2.6.0/tests/test_type_inference/test_dictcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_errors.py` & `python-ta-2.6.0/tests/test_type_inference/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_for.py` & `python-ta-2.6.0/tests/test_type_inference/test_for.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_function_annotation.py` & `python-ta-2.6.0/tests/test_type_inference/test_function_annotation.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_function_def_inference.py` & `python-ta-2.6.0/tests/test_type_inference/test_function_def_inference.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_function_overload.py` & `python-ta-2.6.0/tests/test_type_inference/test_function_overload.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_functions.py` & `python-ta-2.6.0/tests/test_type_inference/test_functions.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_ifexpr.py` & `python-ta-2.6.0/tests/test_type_inference/test_ifexpr.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_imports.py` & `python-ta-2.6.0/tests/test_type_inference/test_imports.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_initializer.py` & `python-ta-2.6.0/tests/test_type_inference/test_initializer.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_lambda.py` & `python-ta-2.6.0/tests/test_type_inference/test_lambda.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_list.py` & `python-ta-2.6.0/tests/test_type_inference/test_list.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_listcomp.py` & `python-ta-2.6.0/tests/test_type_inference/test_listcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_literals.py` & `python-ta-2.6.0/tests/test_type_inference/test_literals.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_name.py` & `python-ta-2.6.0/tests/test_type_inference/test_name.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_set.py` & `python-ta-2.6.0/tests/test_type_inference/test_set.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_setcomp.py` & `python-ta-2.6.0/tests/test_type_inference/test_setcomp.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_starred.py` & `python-ta-2.6.0/tests/test_type_inference/test_starred.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_subscript.py` & `python-ta-2.6.0/tests/test_type_inference/test_subscript.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_tuple.py` & `python-ta-2.6.0/tests/test_type_inference/test_tuple.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_typefail_reason.py` & `python-ta-2.6.0/tests/test_type_inference/test_typefail_reason.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_type_inference/test_unaryops.py` & `python-ta-2.6.0/tests/test_type_inference/test_unaryops.py`

 * *Files identical despite different names*

### Comparing `python-ta-2.5.0/tests/test_z3_visitor.py` & `python-ta-2.6.0/tests/test_z3_visitor.py`

 * *Files identical despite different names*

