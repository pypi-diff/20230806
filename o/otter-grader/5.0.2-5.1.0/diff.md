# Comparing `tmp/otter-grader-5.0.2.tar.gz` & `tmp/otter-grader-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-5.0.2.tar", last modified: Fri Jul 28 01:46:35 2023, max compression
+gzip compressed data, was "otter-grader-5.1.0.tar", last modified: Sun Aug  6 03:43:54 2023, max compression
```

## Comparing `otter-grader-5.0.2.tar` & `otter-grader-5.1.0.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 01:46:05.000000 otter-grader-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-28 01:46:05.000000 otter-grader-5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 01:46:35.260630 otter-grader-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-28 01:46:05.000000 otter-grader-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.248629 otter-grader-5.0.2/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-28 01:46:32.000000 otter-grader-5.0.2/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/execute/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.252629 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.244629 otter-grader-5.0.2/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/common/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/common/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/common/run_otter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-28 01:46:05.000000 otter-grader-5.0.2/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-28 01:46:33.000000 otter-grader-5.0.2/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.256630 otter-grader-5.0.2/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-28 01:46:35.000000 otter-grader-5.0.2/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 01:46:34.000000 otter-grader-5.0.2/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-28 01:46:05.000000 otter-grader-5.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 01:46:35.260630 otter-grader-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-28 01:46:05.000000 otter-grader-5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_assign/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_assign/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_check/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_execute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_execute/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_export/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_generate/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_grade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-28 01:46:32.000000 otter-grader-5.0.2/test/test_grade/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:35.260630 otter-grader-5.0.2/test/test_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_run/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-28 01:46:05.000000 otter-grader-5.0.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.328333 otter-grader-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-06 03:43:04.000000 otter-grader-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-06 03:43:04.000000 otter-grader-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-06 03:43:54.328333 otter-grader-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-06 03:43:04.000000 otter-grader-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.304332 otter-grader-5.1.0/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.304332 otter-grader-5.1.0/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.308333 otter-grader-5.1.0/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.308333 otter-grader-5.1.0/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19532 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.308333 otter-grader-5.1.0/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.308333 otter-grader-5.1.0/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/execute/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/execute/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.308333 otter-grader-5.1.0/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.300332 otter-grader-5.1.0/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/generate/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/templates/common/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/templates/common/run_otter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.312332 otter-grader-5.1.0/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.316332 otter-grader-5.1.0/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.320332 otter-grader-5.1.0/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.320332 otter-grader-5.1.0/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-06 03:43:04.000000 otter-grader-5.1.0/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-06 03:43:51.000000 otter-grader-5.1.0/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.320332 otter-grader-5.1.0/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-06 03:43:53.000000 otter-grader-5.1.0/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-08-06 03:43:54.000000 otter-grader-5.1.0/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 03:43:53.000000 otter-grader-5.1.0/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-06 03:43:53.000000 otter-grader-5.1.0/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-06 03:43:53.000000 otter-grader-5.1.0/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 03:43:53.000000 otter-grader-5.1.0/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-06 03:43:04.000000 otter-grader-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 03:43:54.328333 otter-grader-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-06 03:43:04.000000 otter-grader-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_assign/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_assign/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_check/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_check/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_check/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_execute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_execute/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_execute/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_export/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_generate/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_grade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_grade/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:54.324333 otter-grader-5.1.0/test/test_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_run/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 03:43:04.000000 otter-grader-5.1.0/test/test_utils.py
```

### Comparing `otter-grader-5.0.2/LICENSE` & `otter-grader-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/PKG-INFO` & `otter-grader-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.2
+Version: 5.1.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.2/README.md` & `otter-grader-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/api.py` & `otter-grader-5.1.0/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/__init__.py` & `otter-grader-5.1.0/otter/assign/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/assignment.py` & `otter-grader-5.1.0/otter/assign/assignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,28 @@
         )
 
         files: list = fica.Key(
             description="a list of other files to include in the student submissions' zip file",
             default=[],
         )
 
+        class RequireNoPDFAckValue(fica.Config):
+
+            message: str = fica.Key(
+                description="a message to show to students if a PDF is meant to be included in " \
+                    "the submission but cannot be generated",
+            )
+
+        require_no_pdf_ack: Union[bool, RequireNoPDFAckValue] = fica.Key(
+            description="whether to require students to acknowledge that a PDF could not be " \
+                "created if one is meant to be included in the submission zip file",
+            default=False,
+            subkey_container=RequireNoPDFAckValue,
+        )
+
     export_cell: ExportCellValue = fica.Key(
         description="whether to include an Otter export cell in the output notebooks",
         subkey_container=ExportCellValue,
     )
 
     class SeedValue(fica.Config):
 
@@ -240,28 +254,32 @@
     since it contians a timestamp
     """
 
     def __init__(self, user_config: Dict[str, Any] = {}, **kwargs) -> None:
         self._logger.debug(f"Initializing with config: {user_config}")
         super().__init__(user_config, **kwargs)
 
-        # convert a boolean to a config object for self.generate if indicated
+        # convert true values masking subkey contains to those containers
         if self.generate is True:
             self.generate = AutograderConfig()
+        if self.export_cell is True:
+            self.export_cell = type(self).ExportCellValue()
 
         if self.variables:
             warnings.warn(
                 "The variables key of the assignment config is deprecated and will be removed in " \
                     "v6.0.0. Please use generate.seed_variables instead.", DeprecationWarning)
 
     def update(self, user_config: Dict[str, Any]):
         self._logger.debug(f"Updating config: {user_config}")
         ret = super().update(user_config)
         if self.generate is True:
             self.generate = AutograderConfig()
+        if self.export_cell is True:
+            self.export_cell = type(self).ExportCellValue()
         return ret
 
     @property
     def is_r(self):
         """
         Whether the language of the assignment is R
         """
```

### Comparing `otter-grader-5.0.2/otter/assign/blocks.py` & `otter-grader-5.1.0/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/cell_factory.py` & `otter-grader-5.1.0/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/feature_toggle.py` & `otter-grader-5.1.0/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/notebook_transformer.py` & `otter-grader-5.1.0/otter/assign/notebook_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,32 @@
 from .blocks import BlockType, get_cell_config, is_assignment_config_cell, is_block_boundary_cell
 from .cell_factory import CellFactory
 from .feature_toggle import FeatureToggle
 from .plugins import replace_plugins_with_calls
 from .question_config import QuestionConfig
 from .r_adapter import rmarkdown_converter
 from .r_adapter.cell_factory import RCellFactory
-from .solutions import has_seed, SOLUTION_CELL_TAG, overwrite_seed_vars, strip_ignored_lines, \
-    strip_solutions_and_output
+from .solutions import (
+    has_seed,
+    SOLUTION_CELL_TAG,
+    overwrite_seed_vars,
+    strip_ignored_lines,
+    strip_solutions_and_output,
+)
 from .tests_manager import AssignmentTestsManager
-from .utils import add_tag, add_assignment_name_to_notebook, AssignNotebookFormatException, \
-    get_source, is_cell_type, is_ignore_cell, lock, remove_cell_ids
+from .utils import (
+    add_tag,
+    add_assignment_name_to_notebook,
+    add_require_no_pdf_ack_to_notebook,
+    AssignNotebookFormatException,
+    get_source,
+    is_cell_type,
+    is_ignore_cell,
+    lock,
+)
 
 
 class NotebookTransformer:
     """
     A transformer for master notebooks that converts them to autograder- and
     student-formatted notebooks.
 
@@ -105,35 +118,29 @@
         if self.assignment.init_cell:
             transformed_cells = self.cell_factory.create_init_cells() + transformed_cells
 
         if self.assignment.check_all_cell:
             transformed_cells += self.cell_factory.create_check_all_cells()
 
         if self.assignment.export_cell:
-            export_cell = self.assignment.export_cell
-            if export_cell is True:
-                export_cell = {}
-
             transformed_cells += self.cell_factory.create_export_cells()
 
         transformed_nb = copy.deepcopy(nb)
         transformed_nb['cells'] = transformed_cells
 
         # replace plugins
         transformed_nb = replace_plugins_with_calls(transformed_nb)
 
         # strip out ignored lines
         transformed_nb = strip_ignored_lines(transformed_nb)
 
-        # TODO: this is a bad practice and only a monkey-patch for #340. we should do some better
-        # parsing of the nbformat version info to determine if this is necessary.
-        remove_cell_ids(transformed_nb)
-
         add_assignment_name_to_notebook(transformed_nb, self.assignment)
 
+        add_require_no_pdf_ack_to_notebook(transformed_nb, self.assignment)
+
         return TransformedNotebookContainer(transformed_nb, self)
 
     def _get_transformed_cells(self, cells):
         """
         Takes in a list of cells from the master notebook and returns a list of cells for the
         autograder notebook.
```

### Comparing `otter-grader-5.0.2/otter/assign/output.py` & `otter-grader-5.1.0/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/plugins.py` & `otter-grader-5.1.0/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/question_config.py` & `otter-grader-5.1.0/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/r_adapter/cell_factory.py` & `otter-grader-5.1.0/otter/assign/r_adapter/cell_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,30 +25,41 @@
     def create_check_all_cells(self):
         return []
 
     def create_export_cells(self):
         if not self.assignment.export_cell:
             return []
 
+        force_save = not self.assignment.is_rmd and self.assignment.export_cell.force_save
+
         instructions = nbformat.v4.new_markdown_cell()
         instructions.source = "## Submission\n\nMake sure you have run all cells in your " \
             "notebook in order before running the cell below, so that all images/graphs appear " \
-            "in the output. The cell below will generate a zip file for you to submit. **Please " \
-            "save before exporting!**"
+            "in the output. The cell below will generate a zip file for you to submit."
+
+        if not force_save: instructions.source += " **Please save before exporting!**"
 
         if self.assignment.export_cell.instructions:
             instructions.source += '\n\n' + self.assignment.export_cell.instructions
 
-        pdf_arg = ""
+        args = []
         if self.assignment.export_cell.pdf:
-            pdf_arg = ", pdf = TRUE"
+            args.append("pdf = TRUE")
+        if force_save:
+            args.append("force_save = TRUE")
+
+        if args:
+            args = ", " + ", ".join(args)
+        else:
+            args = ""
 
         export = nbformat.v4.new_code_cell()
-        source_lines = ["# Save your notebook first, then run this cell to export your submission."]
-        source_lines.append(f'ottr::export("{self.assignment.notebook_basename}"{pdf_arg})')
+        source_lines = [] if force_save else \
+            ["# Save your notebook first, then run this cell to export your submission."]
+        source_lines.append(f'ottr::export("{self.assignment.notebook_basename}"{args})')
         export.source = "\n".join(source_lines)
 
         lock(instructions)
         lock(export)
 
         cells = [instructions, export]
         if self.check_feature_toggle(FeatureToggle.EMPTY_MD_BOUNDARY_CELLS):
```

### Comparing `otter-grader-5.0.2/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-5.1.0/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/r_adapter/solutions.py` & `otter-grader-5.1.0/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/r_adapter/tests_manager.py` & `otter-grader-5.1.0/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/solutions.py` & `otter-grader-5.1.0/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/tests_manager.py` & `otter-grader-5.1.0/otter/assign/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/assign/utils.py` & `otter-grader-5.1.0/otter/assign/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Utilities for Otter Assign"""
 
 import copy
+import fica
 import json
 import os
 import pathlib
 import re
 import shutil
 
-from contextlib import redirect_stdout, redirect_stderr
-from io import StringIO
 from textwrap import indent
 
 from ..api import grade_submission
 from ..generate import main as generate_autograder
-from ..utils import get_source, NOTEBOOK_METADATA_KEY, loggers
+from ..run import capture_run_output
+from ..utils import (
+    get_source,
+    loggers,
+    NO_PDF_EXPORT_MESSAGE_KEY,
+    NOTEBOOK_METADATA_KEY,
+    REQUIRE_CONFIRMATION_NO_PDF_EXPORT_KEY,
+)
 
 
 LOGGER = loggers.get_logger(__name__)
 
 
 class EmptyCellException(Exception):
     """
@@ -88,26 +94,14 @@
     for cell in nb['cells']:
         if 'outputs' in cell:
             cell['outputs'] = []
         if 'execution_count' in cell:
             cell['execution_count'] = None
 
 
-def remove_cell_ids(nb):
-    """
-    Remove all cell IDs from a notebook in-place.
-
-    Args:
-        nb (``nbformat.NotebookNode``): a notebook
-    """
-    for cell in nb['cells']:
-        if 'id' in cell:
-            cell.pop('id')
-
-
 def lock(cell):
     """
     Make a cell non-editable and non-deletable in-place.
 
     Args:
         cell (``nbformat.NotebookNode``): cell to be locked
     """
@@ -199,23 +193,22 @@
     Args:
         assignment (``otter.assgin.assignment.Assignment``): the assignment config
         debug (``bool``): whether to throw errors instead of swallowing them during grading
 
     Raises:
         ``RuntimeError``: if the grade received by the notebook is not 100%
     """
-    stdout = StringIO()
-    with redirect_stdout(stdout), redirect_stderr(stdout):
+    with capture_run_output() as run_output:
         results = grade_submission(
             str(assignment.ag_notebook_path),
             str(assignment.ag_zip_path),
             debug=debug,
         )
 
-    LOGGER.debug(f"Otter Run output:\n{stdout.getvalue()}")
+    LOGGER.debug(f"Otter Run output:\n{run_output.getvalue()}")
 
     if results.total != results.possible:
         raise RuntimeError(f"Some autograder tests failed in the autograder notebook:\n" + \
             indent(results.summary(), '    '))
 
 
 def write_otter_config_file(assignment):
@@ -348,7 +341,25 @@
         nb (``nbformat.NotebookNode``): the notebook to add the name to
         assignment (``otter.assign.assignment.Assignment``): the assignment config
     """
     if assignment.name is not None:
         if NOTEBOOK_METADATA_KEY not in nb["metadata"]:
             nb["metadata"][NOTEBOOK_METADATA_KEY] = {}
         nb["metadata"][NOTEBOOK_METADATA_KEY]["assignment_name"] = assignment.name
+
+
+def add_require_no_pdf_ack_to_notebook(nb, assignment):
+    """
+    Add the no PDF ACK configurtion from the assignment config to the provided notebook's metadata
+    in-place.
+
+    Args:
+        nb (``nbformat.NotebookNode``): the notebook to add the name to
+        assignment (``otter.assign.assignment.Assignment``): the assignment config
+    """
+    if assignment.export_cell and assignment.export_cell.require_no_pdf_ack:
+        if NOTEBOOK_METADATA_KEY not in nb["metadata"]:
+            nb["metadata"][NOTEBOOK_METADATA_KEY] = {}
+        nb["metadata"][NOTEBOOK_METADATA_KEY][REQUIRE_CONFIRMATION_NO_PDF_EXPORT_KEY] = True
+        if isinstance(assignment.export_cell.require_no_pdf_ack, fica.Config):
+            nb["metadata"][NOTEBOOK_METADATA_KEY][NO_PDF_EXPORT_MESSAGE_KEY] = \
+                assignment.export_cell.require_no_pdf_ack.message
```

### Comparing `otter-grader-5.0.2/otter/check/__init__.py` & `otter-grader-5.1.0/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/check/logs.py` & `otter-grader-5.1.0/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/check/notebook.py` & `otter-grader-5.1.0/otter/check/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,36 @@
 import zipfile
 
 from glob import glob
 from IPython.display import display, HTML
 from textwrap import indent
 
 from .logs import LogEntry, EventType, Log
-from .utils import grade_zip_file, grading_mode_disabled, incompatible_with, IPythonInterpreter, \
-    list_available_tests, logs_event, resolve_test_info, save_notebook
+from .utils import (
+    display_pdf_confirmation_widget,
+    grade_zip_file,
+    grading_mode_disabled,
+    incompatible_with,
+    IPythonInterpreter,
+    list_available_tests,
+    logs_event,
+    resolve_test_info,
+    save_notebook,
+)
 
 from ..execute import Checker
 from ..export import export_notebook
 from ..plugins import PluginCollection
 from ..test_files import GradingResults
-from ..utils import Loggable
+from ..utils import (
+    Loggable,
+    NO_PDF_EXPORT_MESSAGE_KEY,
+    NOTEBOOK_METADATA_KEY,
+    REQUIRE_CONFIRMATION_NO_PDF_EXPORT_KEY,
+)
 
 
 _OTTER_LOG_FILENAME = ".OTTER_LOG"
 _SHELVE = False
 _ZIP_NAME_FILENAME = "__zip_filename__"
 
 
@@ -68,14 +82,17 @@
             raise ValueError(f"Tests directory {tests_dir} does not exist")
 
         if type(self)._tests_dir_override is not None:
             self._path = type(self)._tests_dir_override
         else:
             self._path = tests_dir
 
+        # TODO: clean up logic for handling nb path; this can be determined in __init__ instead of
+        # begin computed every time. Maybe require it as an argument so it can be removed from other
+        # methods?
         self._notebook = nb_path
         self._tests_url_prefix = tests_url_prefix
         self._addl_files = []
         self._plugin_collections = {}
 
         # assume using otter service if there is a .otter file
         otter_configs = glob("*.otter")
@@ -339,84 +356,102 @@
                     "Couldn't automatically save the notebook; we recommend using File > Save & "
                     "Checkpoint and then re-running this cell. The zip file returned by this call "
                     "will use the last saved version of this notebook."
                 )
             else:
                 self._logger.debug("Force-save successful")
 
+        otter_nb_config = {}
         with open(nb_path, "r", encoding="utf-8") as f:
             if len(f.read().strip()) == 0:
                 raise ValueError(f"Notebook '{nb_path}' is empty. Please save and checkpoint your "
                     "notebook and rerun this cell.")
 
+            f.seek(0)
+            # TODO: turn the notebook metadata configs into a fica.Config
+            otter_nb_config = json.load(f).get("metadata", {}).get(NOTEBOOK_METADATA_KEY, {})
+
         timestamp = dt.datetime.now().strftime("%Y_%m_%dT%H_%M_%S_%f")
         if export_path is None:
             zip_path = ".".join(nb_path.split(".")[:-1]) + "_" + timestamp + ".zip"
         else:
             zip_path = export_path
 
         self._logger.debug(f"Determined export zip path: {zip_path}")
 
         zf = zipfile.ZipFile(zip_path, mode="w")
         zf.write(nb_path)
 
+        pdf_created = True
         if pdf:
             pdf_path = export_notebook(nb_path, filtering=filtering, pagebreaks=pagebreaks)
             if os.path.isfile(pdf_path):
+                pdf_created = True
                 zf.write(pdf_path)
                 self._logger.debug(f"Wrote PDF to zip file: {pdf_path}")
             else:
+                pdf_created = False
                 warnings.warn("Could not locate a PDF to include")
 
-        if os.path.isfile(_OTTER_LOG_FILENAME):
-            zf.write(_OTTER_LOG_FILENAME)
-            self._logger.debug("Added Otter log to zip file")
-
-        zip_basename = os.path.basename(zip_path)
-        zf.writestr(_ZIP_NAME_FILENAME, zip_basename)
-        self._logger.debug(f"Added {_ZIP_NAME_FILENAME} to zip file: '{zip_basename}'")
-
-        dot_otter = glob("*.otter")
-        if dot_otter:
-            if len(dot_otter) != 1:
-                raise ValueError("Too many .otter files (max 1 allowed)")
-            dot_otter = dot_otter[0]
-            zf.write(dot_otter)
-            self._logger.debug(f"Added .otter file to zip file: {dot_otter}")
-
-        for file in files:
-            if os.path.isdir(file):
-                sub_files = glob(f"./{file}/**/*.*")
-                for sub_file in sub_files:
-                    zf.write(sub_file)
-            else:
+        def continue_export():
+            if os.path.isfile(_OTTER_LOG_FILENAME):
+                zf.write(_OTTER_LOG_FILENAME)
+                self._logger.debug("Added Otter log to zip file")
+
+            zip_basename = os.path.basename(zip_path)
+            zf.writestr(_ZIP_NAME_FILENAME, zip_basename)
+            self._logger.debug(f"Added {_ZIP_NAME_FILENAME} to zip file: '{zip_basename}'")
+
+            dot_otter = glob("*.otter")
+            if dot_otter:
+                if len(dot_otter) != 1:
+                    raise ValueError("Too many .otter files (max 1 allowed)")
+                dot_otter = dot_otter[0]
+                zf.write(dot_otter)
+                self._logger.debug(f"Added .otter file to zip file: {dot_otter}")
+
+            for file in files:
+                if os.path.isdir(file):
+                    sub_files = glob(f"{file}/**/*.*", recursive=True)
+                    for sub_file in sub_files:
+                        zf.write(sub_file)
+                else:
+                    zf.write(file)
+                self._logger.debug(f"Added file to zip file: {file}")
+
+            for file in self._addl_files:
                 zf.write(file)
-            self._logger.debug(f"Added file to zip file: {file}")
+                self._logger.debug(f"Added plugin file to zip file: {file}")
 
-        for file in self._addl_files:
-            zf.write(file)
-            self._logger.debug(f"Added plugin file to zip file: {file}")
-
-        zf.close()
-
-        if run_tests:
-            print("Running your submission against local test cases...\n")
-            results = grade_zip_file(zip_path, nb_path, self._path)
-            print(
-                "Your submission received the following results when run against " + \
-                "available test cases:\n\n" + indent(results.summary(), "    "))
+            zf.close()
 
-        if display_link:
-            # create and display output HTML
-            out_html = """
-            <p>Your submission has been exported. Click <a href="{}" download="{}" target="_blank">here</a>
-            to download the zip file.</p>
-            """.format(zip_path, zip_path)
+            if run_tests:
+                print("Running your submission against local test cases...\n")
+                results = grade_zip_file(zip_path, nb_path, self._path)
+                print(
+                    "Your submission received the following results when run against " + \
+                    "available test cases:\n\n" + indent(results.summary(), "    "))
+
+            if display_link:
+                # create and display output HTML
+                out_html = f"""
+                    <p>
+                        Your submission has been exported. Click
+                        <a href="{zip_path}" downloadzip_path target="_blank">here</a> to download
+                        the zip file.
+                    </p>
+                """
 
-            display(HTML(out_html))
+                display(HTML(out_html))
+
+        if pdf_created or not otter_nb_config.get(REQUIRE_CONFIRMATION_NO_PDF_EXPORT_KEY, False):
+            continue_export()
+        else:
+            display_pdf_confirmation_widget(
+                otter_nb_config.get(NO_PDF_EXPORT_MESSAGE_KEY), continue_export)
 
     @grading_mode_disabled
     @logs_event(EventType.END_CHECK_ALL)
     def check_all(self):
         """
         Runs all tests on this notebook. Tests are run against the current global environment, so any
         tests with variable name collisions will fail.
```

### Comparing `otter-grader-5.0.2/otter/check/utils.py` & `otter-grader-5.1.0/otter/check/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Utilities for Otter Check"""
 
+import ipylab
 import nbformat as nbf
 import os
-import requests
 import sys
 import tempfile
 import time
 import wrapt
 
 from enum import Enum
 from glob import glob
 from IPython import get_ipython
 from IPython.display import display, Javascript
+from ipywidgets import Button, HTML, Output, VBox
 from subprocess import run, PIPE
 
 from .logs import EventType
 
 from ..utils import import_or_raise, NBFORMAT_VERSION, NOTEBOOK_METADATA_KEY
 
 
@@ -29,23 +30,28 @@
 
     Returns
         ``bool``: whether the notebook was saved successfully
     """
     if get_ipython() is not None:
         orig_mod_time = os.path.getmtime(filename)
         start = time.time()
+
+        # For classic notebooks
         display(Javascript("""
             if (typeof Jupyter !== 'undefined') {
                 Jupyter.notebook.save_checkpoint();
             }
-            else {
-                document.querySelector('[data-command="docmanager:save"]').click();
-            }
         """))
 
+        # For JupyterLab
+        try:
+            app = ipylab.JupyterFrontEnd()
+            app.commands.execute("docmanager:save")
+        except: pass
+
         while time.time() - start < timeout:
             curr_mod_time = os.path.getmtime(filename)
             if orig_mod_time < curr_mod_time and os.path.getsize(filename) > 0:
                 return True
 
             time.sleep(0.2)
 
@@ -67,16 +73,19 @@
             sys.executable, "-m", "otter.check.validate_export",
             "--zip-path", zip_path,
             "--nb-arcname", nb_arcname,
             "--tests-dir", tests_dir,
             "--results-path", results_path,
         ]
 
+        # this environment variable is needed to fix #686
+        subprocess_env = {**os.environ, "PYDEVD_DISABLE_FILE_VALIDATION": "1"}
+
         # run the command
-        results = run(command, stdout=PIPE, stderr=PIPE)
+        results = run(command, env=subprocess_env, stdout=PIPE, stderr=PIPE)
 
         # TODO: remove
         print(results.stdout.decode("utf-8"))
         print(results.stderr.decode("utf-8"))
 
         if results.stderr:
             raise RuntimeError(results.stderr)
@@ -288,7 +297,32 @@
         if nb_path is None:
             raise ValueError("Tests directory does not exist and no notebook path provided")
 
         test_path = nb_path
         test_name = question
 
     return test_path, test_name
+
+
+def display_pdf_confirmation_widget(message, callback):
+    """
+    Display a widget to the user to acknowledge that a PDF will not be included in their submission
+    zip.
+
+    Args:
+        message (``str | None``): a custom message to use
+        callback (``callable[]``): a callback function to execute after the user ACKs
+    """
+    o = Output()
+    def wrapped_callback(*args):
+        with o: callback()
+
+    if not message:
+        message = "Your notebook could not be exported as a PDF. To continue exporting your " \
+            "submission, please click the button below."
+
+    t = HTML(f"""<p style="margin: 0">{message}</p>""")
+    b = Button(description="Continue export", button_style="warning")
+    b.on_click(wrapped_callback)
+    m = HTML("""<div style="height: 10px; width: 100%"></div>""")
+    
+    display(VBox([t, b, m, o]))
```

### Comparing `otter-grader-5.0.2/otter/check/validate_export/__main__.py` & `otter-grader-5.1.0/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/cli.py` & `otter-grader-5.1.0/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/execute/__init__.py` & `otter-grader-5.1.0/otter/execute/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import nbformat
 import pickle
 import tempfile
 
 from traitlets.config import Config
 
 from .checker import Checker
+from .logging import start_server
 from .preprocessor import GradingPreprocessor
 
 from ..test_files import GradingResults
 from ..utils import NBFORMAT_VERSION
 
 
 def grade_notebook(
@@ -65,33 +66,39 @@
 
     if plugin_collection is not None:
         nb = plugin_collection.before_execution(nb)
 
     with tempfile.NamedTemporaryFile() as ntf:
         c = Config()
 
+        (host, port), stop_server = start_server()
+
         # GradingPreprocessor config
         c.GradingPreprocessor.cwd = cwd
         c.GradingPreprocessor.test_dir = test_dir
         c.GradingPreprocessor.tests_glob = tests_glob
         c.GradingPreprocessor.results_path = ntf.name
         c.GradingPreprocessor.seed = seed
         c.GradingPreprocessor.seed_variable = seed_variable
         c.GradingPreprocessor.otter_log = log
         c.GradingPreprocessor.variables = variables
+        c.GradingPreprocessor.logging_server_host = host
+        c.GradingPreprocessor.logging_server_port = port
 
         # ExecutePreprocessor config
         c.ExecutePreprocessor.allow_errors = ignore_errors
 
         gp = GradingPreprocessor(config=c)
         ep = ExecutePreprocessor(config=c)
 
         nb, _ = gp.preprocess(nb)
         executed_nb, _ = ep.preprocess(nb)
 
+        stop_server()
+
         gp.cleanup()
 
         results = pickle.load(ntf)
 
     if not isinstance(results, GradingResults):
         raise TypeError("Results deserialized from grading notebook were not a GradingResults instance")
```

### Comparing `otter-grader-5.0.2/otter/execute/checker.py` & `otter-grader-5.1.0/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/execute/preprocessor.py` & `otter-grader-5.1.0/otter/execute/preprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from otter import Notebook as {notebook_name}
 {notebook_name}.init_grading_mode("{test_dir}")
 
 # set up Otter's logging
 import logging
 from otter.utils import loggers
 loggers.set_level(logging.DEBUG)
+loggers.send_logs("{logging_server_host}", {logging_server_port})
 """
 
 EXPORT_CELL_SOURCE = """\
 from otter.execute import Checker
 for t in {tests_glob_json}:
     Checker.check_if_not_already_checked(t)
 
@@ -63,14 +64,18 @@
 
     variables = Dict(value_trait=Unicode(), key_trait=Unicode(), allow_none=True).tag(config=True)
 
     _notebook_name: str
 
     _log_temp_file: Optional[Tuple[int, str]] = None
 
+    logging_server_host = Unicode().tag(config=True)
+
+    logging_server_port = Integer().tag(config=True)
+
     @property
     def from_log(self):
         return self.otter_log is not None
 
     def preprocess(self, nb, resources = None):
         self._notebook_name = f"notebook_{id_generator()}"
         self.filter_ignored_cells(nb)
@@ -79,15 +84,19 @@
         self.add_seeds(nb)
         self.add_cwd_to_path(nb)
         self.add_init_and_export_cells(nb)  # this should always be the last call
         return nb, resources
 
     def add_init_and_export_cells(self, nb):
         nb.cells.insert(0, nbf.v4.new_code_cell(INIT_CELL_SOURCE.format(
-            notebook_name = self._notebook_name, test_dir = self.test_dir)))
+            notebook_name = self._notebook_name,
+            test_dir = self.test_dir,
+            logging_server_host = self.logging_server_host,
+            logging_server_port = self.logging_server_port,
+        )))
         nb.cells.append(nbf.v4.new_code_cell(EXPORT_CELL_SOURCE.format(
             tests_glob_json = json.dumps(self.tests_glob), results_path = self.results_path)))
 
     def add_cwd_to_path(self, nb):
         if self.cwd:
             nb.cells.insert(
                 0, nbf.v4.new_code_cell(f"import sys\nsys.path.append(r\"{self.cwd}\")"))
```

### Comparing `otter-grader-5.0.2/otter/export/__init__.py` & `otter-grader-5.1.0/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/__init__.py` & `otter-grader-5.1.0/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/base_exporter.py` & `otter-grader-5.1.0/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-5.1.0/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_html.tpl` & `otter-grader-5.1.0/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-5.1.0/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-5.1.0/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-5.1.0/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/utils.py` & `otter-grader-5.1.0/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/via_html.py` & `otter-grader-5.1.0/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/export/exporters/via_latex.py` & `otter-grader-5.1.0/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/generate/__init__.py` & `otter-grader-5.1.0/otter/generate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from ..run.run_autograder.autograder_config import AutograderConfig
 from ..utils import dump_yaml, load_default_file
 from ..version import __version__
 
 
 DEFAULT_PYTHON_VERSION = "3.9"
 OTTER_ENV_NAME = "otter-env"
-OTTR_VERSION = "1.2.0"
+OTTR_VERSION = "1.4.0"
 TEMPLATE_DIR = pkg_resources.resource_filename(__name__, "templates")
 GENERAL_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "general")
 
 
 @dataclass
 class CondaEnvironment:
```

### Comparing `otter-grader-5.0.2/otter/generate/templates/python/setup.sh` & `otter-grader-5.1.0/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/generate/templates/r/setup.sh` & `otter-grader-5.1.0/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/generate/token.py` & `otter-grader-5.1.0/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/generate/utils.py` & `otter-grader-5.1.0/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/grade/Dockerfile` & `otter-grader-5.1.0/otter/grade/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ARG BASE_IMAGE=ubuntu:22.04
 
 FROM ${BASE_IMAGE}
+ARG DEBIAN_FRONTEND=noninteractive
 
 RUN apt-get update && \
     apt-get install -y curl unzip dos2unix && \
     apt-get clean && \
     rm -rf /var/lib/apt/lists/* /var/tmp/*
 
 RUN mkdir -p /autograder/source && \
```

### Comparing `otter-grader-5.0.2/otter/grade/__init__.py` & `otter-grader-5.1.0/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/grade/containers.py` & `otter-grader-5.1.0/otter/grade/containers.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/grade/utils.py` & `otter-grader-5.1.0/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/__init__.py` & `otter-grader-5.1.0/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/abstract_plugin.py` & `otter-grader-5.1.0/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-5.1.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/builtin/grade_override.py` & `otter-grader-5.1.0/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/plugins/builtin/rate_limiting.py` & `otter-grader-5.1.0/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/run/__init__.py` & `otter-grader-5.1.0/otter/run/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import os
 import shutil
 import tempfile
 import zipfile
 
-from .run_autograder import main as run_autograder_main
+from .run_autograder import capture_run_output, main as run_autograder_main
 
 from ..utils import import_or_raise
 
 
 def main(submission, *, autograder="./autograder.zip", output_dir="./", no_logo=False, debug=False):
     """
     Grades a single submission using the autograder configuration ``autograder`` without
```

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/__init__.py` & `otter-grader-5.1.0/otter/run/run_autograder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import pandas as pd
 import zipfile
 
 from glob import glob
 
 from .runners import create_runner
-from .utils import OtterRuntimeError
+from .utils import capture_run_output, OtterRuntimeError, print_output
 from ...version import LOGO_WITH_VERSION
 from ...utils import chdir, import_or_raise, loggers
 
 
 LOGGER = loggers.get_logger(__name__)
 
 
@@ -43,15 +43,15 @@
         loggers.set_level(runner.get_option("log_level"))
         # TODO: log above calls
         # TODO: use loggers.level_context
 
     if runner.get_option("logo"):
         # ASCII 8207 is an invisible non-whitespace character; this should prevent gradescope from
         # incorrectly left-stripping the whitespace at the beginning of the logo
-        print(f"{chr(8207)}\n", LOGO_WITH_VERSION, "\n", sep="")
+        print_output(f"{chr(8207)}\n", LOGO_WITH_VERSION, "\n", sep="")
 
     abs_ag_path = os.path.abspath(runner.get_option("autograder_dir"))
     with chdir(abs_ag_path):
         try:
             if runner.get_option("zips"):
                 with chdir("./submission"):
                     zips = glob("*.zip")
@@ -82,28 +82,28 @@
             raise e
 
         finally:
             if "output" in vars():
                 with open("./results/results.json", "w+") as f:
                     json.dump(output, f, indent=4)                
 
-    print("\n\n", end="")
+    print_output("\n\n", end="")
 
     df = pd.DataFrame(output["tests"])
 
     if runner.get_option("print_score"):
         total, possible = df["score"].sum(), df["max_score"].sum()
         if "score" in output:
             total, possible = output["score"], runner.get_option("points_possible") or possible
         perc = total / possible * 100
-        print(f"Total Score: {total:.3f} / {possible:.3f} ({perc:.3f}%)\n")
+        print_output(f"Total Score: {total:.3f} / {possible:.3f} ({perc:.3f}%)\n")
 
     if runner.get_option("print_summary"):
         pd.set_option("display.max_rows", None)  # print all rows of the dataframe
         if "output" in df.columns:
             df.drop(columns=["output"], inplace=True)
         if "visibility" in df.columns:
             df.drop(columns=["visibility"], inplace=True)
         if "status" in df.columns:
             df.drop(columns=["status"], inplace=True)
 
-        print(df)
+        print_output(df)
```

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/autograder_config.py` & `otter-grader-5.1.0/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/runners/__init__.py` & `otter-grader-5.1.0/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-5.1.0/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import shutil
 import tempfile
 
 from abc import ABC, abstractmethod
 
 from ..autograder_config import AutograderConfig
-from ..utils import OtterRuntimeError, write_blank_page_to_stare_at_before_you
+from ..utils import OtterRuntimeError, print_output, write_blank_page_to_stare_at_before_you
 
 from ....utils import NOTEBOOK_METADATA_KEY
 
 
 class AbstractLanguageRunner(ABC):
     """
     A class defining the logic of running the autograder and generating grading results.
@@ -124,19 +124,19 @@
         try:
             pdf_path = self.write_pdf(submission_path)
 
             if submit:
                 self.submit_pdf(client, pdf_path)
 
         except Exception as e:
-            print(f"\n\nError encountered while generating and submitting PDF:\n{e}")
+            print_output(f"\n\nError encountered while generating and submitting PDF:\n{e}")
             scores.set_pdf_error(e)
 
             if self.ag_config.submit_blank_pdf_on_export_failure and submit:
-                print("\nUploading a blank PDF due to export failure")
+                print_output("\nUploading a blank PDF due to export failure")
                 with tempfile.NamedTemporaryFile(suffix=".pdf") as ntf:
                     write_blank_page_to_stare_at_before_you(ntf.name)
                     self.submit_pdf(client, ntf.name)
 
     def submit_pdf(self, client, pdf_path):
         """
         Upload the PDF at ``pdf_path`` to the Gradescope assignment specified in the config. Does
@@ -158,15 +158,15 @@
             client.upload_pdf_submission(
                 self.ag_config.course_id,
                 self.ag_config.assignment_id,
                 student_email,
                 pdf_path,
             )
 
-        print("\n\nSuccessfully uploaded submissions for: {}".format(
+        print_output("\n\nSuccessfully uploaded submissions for: {}".format(
             ", ".join(student_emails)))
 
     @abstractmethod
     def validate_submission(self, submission_path):
         """
         Validate the submission, raising an error/warning if appropriate.
```

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-5.1.0/otter/run/run_autograder/runners/python_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import nbformat as nbf
 import os
 
 from glob import glob
 
 from .abstract_runner import AbstractLanguageRunner
 
-from ..utils import OtterRuntimeError
+from ..utils import OtterRuntimeError, print_output
 
 from ....check.logs import Log
 from ....check.notebook import _OTTER_LOG_FILENAME
 from ....execute import grade_notebook
 from ....export import export_notebook
 from ....generate.token import APIClient
 from ....plugins import PluginCollection
@@ -109,15 +109,15 @@
                     log = Log.from_file(_OTTER_LOG_FILENAME, ascending=False)
 
                 except Exception as e:
                     if self.ag_config.grade_from_log:
                         raise e
 
                     else:
-                        print(f"Could not deserialize the log due to an error:\n{e}")
+                        print_output(f"Could not deserialize the log due to an error:\n{e}")
                         log = None
 
             else:
                 if self.ag_config.grade_from_log:
                     raise OtterRuntimeError("Grade from log indicated but log not found")
 
                 log = None
@@ -134,31 +134,35 @@
                 variables = self.ag_config.serialized_variables,
                 plugin_collection = plugin_collection,
                 script = os.path.splitext(subm_path)[1] == ".py",
             )
 
             # verify the scores against the log
             if self.ag_config.print_summary:
-                print("\n\n\n\n", end="")
-                print_full_width("-", mid_text="GRADING SUMMARY")
-                print()
+                print_output("\n\n\n\n", end="")
+                s = print_full_width("-", mid_text="GRADING SUMMARY", ret_str=True)
+                print_output(s)
+                print_output()
                 if log is not None:
                     try:
-                        found_discrepancy = scores.verify_against_log(log)
-                        if not found_discrepancy and self.ag_config.print_summary:
-                            print("No discrepancies found while verifying scores against the log.")
+                        discrepancies = scores.verify_against_log(log)
+                        if self.ag_config.print_summary:
+                            if not discrepancies:
+                                print_output("No discrepancies found while verifying scores against the log.")
+                            else:
+                                for d in discrepancies: print_output(d)
 
                     except BaseException as e:
-                        print(f"Error encountered while trying to verify scores with log:\n{e}")
+                        print_output(f"Error encountered while trying to verify scores with log:\n{e}")
 
                 else:
-                    print("No log found with which to verify student scores.")
+                    print_output("No log found with which to verify student scores.")
 
             if generate_pdf:
                 self.write_and_maybe_submit_pdf(client, subm_path, has_token, scores)
 
             if plugin_collection:
                 report = plugin_collection.generate_report()
                 if report.strip():
-                    print("\n\n" + report)
+                    print_output("\n\n" + report)
 
         return scores
```

### Comparing `otter-grader-5.0.2/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-5.1.0/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/test_files/__init__.py` & `otter-grader-5.1.0/otter/test_files/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import math
 import nbformat
 import os
 import pickle
 
 from collections import namedtuple
+from typing import List
 
 from .abstract_test import OK_FORMAT_VARNAME, TestCase, TestCaseResult, TestFile
 from .exception_test import ExceptionTestFile, test_case
 from .metadata_test import NotebookMetadataExceptionTestFile, NotebookMetadataOKTestFile
 from .ok_test import OKTestFile
 from .ottr_test import OttrTestFile
 
@@ -267,30 +268,30 @@
         Set a PDF generation error to be displayed as a failed (0-point) test on Gradescope.
 
         Args:
             error (``Exception``): the error thrown
         """
         self.pdf_error = error
 
-    def verify_against_log(self, log, ignore_hidden=True):
+    def verify_against_log(self, log, ignore_hidden=True) -> List[str]:
         """
         Verifies these scores against the results stored in this log using the results returned by 
-        ``Log.get_results`` for comparison. Prints a message if the scores differ by more than the 
-        default tolerance of ``math.isclose``. If ``ignore_hidden`` is ``True``, hidden tests are
-        ignored when verifying scores.
+        ``Log.get_results`` for comparison. A discrepancy occurs if the scores differ by more than
+        the default tolerance of ``math.isclose``. If ``ignore_hidden`` is ``True``, hidden tests
+        are ignored when verifying scores.
 
         Args:
             log (``otter.check.logs.Log``): the log to verify against
             ignore_hidden  (``bool``, optional): whether to ignore hidden tests during verification
 
         Returns:
-            ``bool``: whether a discrepancy was found
+            ``list[str]``: a list of error messages for discrepancies; if none were found, the list
+                is empty
         """
-        found_discrepancy = False
-        # for test_name in  self.test_cases:
+        l = []
         for test_name, test_file in self.results.items():
             if ignore_hidden:
                 tcrs = [
                     test_case_result
                     for test_case_result in test_file.test_case_results
                     if not test_case_result.test_case.hidden
                 ]
@@ -298,22 +299,20 @@
             else:
                 score = test_file.score
             try:
                 result = log.get_results(test_name)
                 # TODO fix
                 logged_score = result.score
                 if not math.isclose(score, logged_score):
-                    print("Score for {} ({:.3f}) differs from logged score ({:.3f})".format(
-                        test_name, score, logged_score
-                    ))
-                    found_discrepancy = True
+                    l.append(
+                        f"Score for {test_name} ({score:.3f}) differs from logged score " \
+                        f"({logged_score:.3f})")
             except QuestionNotInLogException:
-                print(f"No score for {test_name} found in this log")
-                found_discrepancy = True
-        return found_discrepancy
+                l.append(f"No score for {test_name} found in this log")
+        return l
 
     def to_report_str(self):
         """
         Returns these results as a report string generated using the ``__repr__`` of the ``TestFile``
         class.
 
         Returns:
```

### Comparing `otter-grader-5.0.2/otter/test_files/abstract_test.py` & `otter-grader-5.1.0/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/test_files/exception_test.py` & `otter-grader-5.1.0/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/test_files/metadata_test.py` & `otter-grader-5.1.0/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/test_files/ok_test.py` & `otter-grader-5.1.0/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/otter/utils.py` & `otter-grader-5.1.0/otter/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Various utilities for Otter-Grader"""
 
 import importlib
 import logging
+import logging.handlers
 import os
 import pathlib
 import random
 import re
 import string
 import shutil
 import tempfile
@@ -19,14 +20,26 @@
 # TODO: migrate other uses to this constant
 NBFORMAT_VERSION = 4
 """the version of the Jupyter notebook format to use"""
 
 NOTEBOOK_METADATA_KEY = "otter"
 """the key used for all Otter metadata added to a notebook"""
 
+REQUIRE_CONFIRMATION_NO_PDF_EXPORT_KEY = "require_no_pdf_confirmation"
+"""
+the key in Otter's notebook metadata for requiring students to acknowledge that their notebook could
+not be exported as a PDF before creating the submission zip file
+"""
+
+NO_PDF_EXPORT_MESSAGE_KEY = "export_pdf_failure_message"
+"""
+the key in Otter's notebook metadata for the message to show if a notebook cannot be exported as a
+PDF
+"""
+
 
 @contextmanager
 def hide_outputs():
     """
     Context manager for hiding outputs from ``display()`` calls. IPython handles matplotlib outputs 
     specially, so those are supressed too.
     """
@@ -236,37 +249,49 @@
         pdf_path = os.path.abspath(pdf_path)
         rmarkdown = importr("rmarkdown")
         rmarkdown.render(ntf.name, "pdf_document", pdf_path)
 
 
 class loggers:
 
-    _format = "[%(levelname)s %(name)s.%(funcName)s] %(message)s"
     _instances = {}
     _log_level = logging.WARNING
+    _formatter = logging.Formatter("[%(levelname)s %(name)s.%(funcName)s] %(message)s")
+    _socket_handler = None
 
     @staticmethod
     def __new__(cls, *args, **kwargs):
         raise NotImplementedError("This class is not meant to be instantiated")
+    
+    @classmethod
+    def send_logs(cls, host, port):
+        """
+        Add a ``SocketHandler`` to all loggers that sends their logs to a TCP socket at the
+        specified host and port.
+        """
+        cls._socket_handler = logging.handlers.SocketHandler(host, port)
+        for logger in cls._instances.values():
+            logger.addHandler(cls._socket_handler)
 
     @classmethod
     def get_logger(cls, name):
         """
         Retrieve ``logging.Logger`` with name ``name`` and return it, setting the log level to the 
         class log level.
         """
         if name in cls._instances:
             return cls._instances[name]
         logger = logging.getLogger(name)
         logger.propagate = False  # prevent child loggers from inheriting the handler
         logger.setLevel(cls._log_level)
         handler = logging.StreamHandler()
-        formatter = logging.Formatter(cls._format)
-        handler.setFormatter(formatter)
+        handler.setFormatter(cls._formatter)
         logger.addHandler(handler)
+        if cls._socket_handler:
+            logger.addHandler(cls._socket_handler)
         cls._instances[name] = logger
         return logger
 
     @classmethod
     def get_level(cls):
         """
         Return the current log level of these loggers.
```

### Comparing `otter-grader-5.0.2/otter/version.py` & `otter-grader-5.1.0/otter/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "5.0.2"
+__version__ = "5.1.0"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-5.0.2/otter_grader.egg-info/PKG-INFO` & `otter-grader-5.1.0/otter_grader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 5.0.2
+Version: 5.1.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-5.0.2/otter_grader.egg-info/SOURCES.txt` & `otter-grader-5.1.0/otter_grader.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 otter/check/logs.py
 otter/check/notebook.py
 otter/check/utils.py
 otter/check/validate_export/__init__.py
 otter/check/validate_export/__main__.py
 otter/execute/__init__.py
 otter/execute/checker.py
+otter/execute/logging.py
 otter/execute/preprocessor.py
 otter/export/__init__.py
 otter/export/utils.py
 otter/export/exporters/__init__.py
 otter/export/exporters/base_exporter.py
 otter/export/exporters/utils.py
 otter/export/exporters/via_html.py
```

### Comparing `otter-grader-5.0.2/setup.py` & `otter-grader-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_api.py` & `otter-grader-5.1.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_assign/test_integration.py` & `otter-grader-5.1.0/test/test_assign/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -233,7 +233,43 @@
         "tests": {"url_prefix": "https://domain.tld/tests/"}
     })
     assign_and_check_output(
         master_nb_path,
         FILE_MANAGER.get_path("jupyterlite-correct"),
         assert_dirs_equal_kwargs=dict(variable_path_exts=[".zip"]),
     )
+
+
+def test_require_no_pdf_ack(generate_master_notebook):
+    """
+    Tests that Otter Assign produces correct notebooks when configured to require students to
+    acknowledge when a PDF cannot be included in their submission zip.
+    """
+    master_nb_path = generate_master_notebook({
+        "export_cell": {
+            "require_no_pdf_ack": True,
+        },
+    })
+    assign_and_check_output(
+        master_nb_path,
+        FILE_MANAGER.get_path("no-pdf-ack-correct"),
+        assert_dirs_equal_kwargs=dict(variable_path_exts=[".zip"]),
+    )
+
+
+# TODO: this format of test makes the repo bloated with several golden files. Can these files be
+# eliminated?
+def test_require_no_pdf_ack_with_message(generate_master_notebook):
+    """
+    Tests that Otter Assign produces correct notebooks when configured to require students to
+    acknowledge when a PDF cannot be included in their submission zip with a custom message.
+    """
+    master_nb_path = generate_master_notebook({
+        "export_cell": {
+            "require_no_pdf_ack": {"message": "no pdf could be created"},
+        },
+    })
+    assign_and_check_output(
+        master_nb_path,
+        FILE_MANAGER.get_path("no-pdf-ack-with-message-correct"),
+        assert_dirs_equal_kwargs=dict(variable_path_exts=[".zip"]),
+    )
```

### Comparing `otter-grader-5.0.2/test/test_check/test_cli.py` & `otter-grader-5.1.0/test/test_check/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_check/test_logs.py` & `otter-grader-5.1.0/test/test_check/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_cli.py` & `otter-grader-5.1.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_execute/test_checker.py` & `otter-grader-5.1.0/test/test_execute/test_checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_execute/test_integration.py` & `otter-grader-5.1.0/test/test_execute/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_export/test_integration.py` & `otter-grader-5.1.0/test/test_export/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_generate/test_autograder.py` & `otter-grader-5.1.0/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_generate/test_token.py` & `otter-grader-5.1.0/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_generate/test_utils.py` & `otter-grader-5.1.0/test/test_generate/test_utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_grade/test_integration.py` & `otter-grader-5.1.0/test/test_grade/test_integration.py`

 * *Files identical despite different names*

### Comparing `otter-grader-5.0.2/test/test_run/test_integration.py` & `otter-grader-5.1.0/test/test_run/test_integration.py`

 * *Files identical despite different names*

