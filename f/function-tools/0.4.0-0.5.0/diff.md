# Comparing `tmp/function-tools-0.4.0.tar.gz` & `tmp/function-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-tools-0.4.0.tar", last modified: Fri Aug  4 12:26:56 2023, max compression
+gzip compressed data, was "function-tools-0.5.0.tar", last modified: Sun Aug  6 20:45:53 2023, max compression
```

## Comparing `function-tools-0.4.0.tar` & `function-tools-0.5.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.373155 function-tools-0.4.0/
--rw-r--r--   0 root         (0) root         (0)    12614 2023-08-04 12:26:47.000000 function-tools-0.4.0/CHANGES.md
--rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    21062 2023-08-04 12:26:56.374155 function-tools-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.342155 function-tools-0.4.0/function_tools/
--rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      257 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/apps.py
--rw-r--r--   0 root         (0) root         (0)    19868 2022-07-13 10:58:16.000000 function-tools-0.4.0/function_tools/caches.py
--rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/consts.py
--rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/decorators.py
--rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/enums.py
--rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.345155 function-tools-0.4.0/function_tools/function_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.362155 function-tools-0.4.0/function_tools/function_templates/function_sync_template/
--rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/README.md
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/__init__.py-tpl
--rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/apps.py-tpl
--rw-r--r--   0 root         (0) root         (0)      651 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/caches.py-tpl
--rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/consts.py-tpl
--rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/enums.py-tpl
--rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/errors.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2831 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/functions.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/helpers.py-tpl
--rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/managers.py-tpl
--rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/presenters.py-tpl
--rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/results.py-tpl
--rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/runners.py-tpl
--rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/strings.py-tpl
--rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/tests.py-tpl
--rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.4.0/function_tools/function_templates/function_sync_template/validators.py-tpl
--rw-r--r--   0 root         (0) root         (0)    10489 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/functions.py
--rw-r--r--   0 root         (0) root         (0)     5362 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/general.py
--rw-r--r--   0 root         (0) root         (0)     2244 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.364155 function-tools-0.4.0/function_tools/management/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.368155 function-tools-0.4.0/function_tools/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/management/commands/register_entities.py
--rw-r--r--   0 root         (0) root         (0)    17850 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/management/commands/startfunction.py
--rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/management/consts.py
--rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/management/strategies.py
--rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.373155 function-tools-0.4.0/function_tools/migrations/
--rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0002_registeredfunction_tags.py
--rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0003_implementationstrategy.py
--rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/migrations/0004_implementationstrategy_order_number.py
--rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/migrations/0005_auto_20220724_0050.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.4.0/function_tools/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/mixins.py
--rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.4.0/function_tools/models.py
--rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/presenters.py
--rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.4.0/function_tools/receivers.py
--rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/results.py
--rw-r--r--   0 root         (0) root         (0)    12097 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/runners.py
--rw-r--r--   0 root         (0) root         (0)    11758 2023-08-04 12:26:47.000000 function-tools-0.4.0/function_tools/storages.py
--rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.4.0/function_tools/strategies.py
--rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/strings.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/types.py
--rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.4.0/function_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.4.0/function_tools/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 12:26:56.344155 function-tools-0.4.0/function_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21062 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2679 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-04 12:26:56.000000 function-tools-0.4.0/function_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-08-04 12:26:56.374155 function-tools-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1707 2023-08-04 12:26:47.000000 function-tools-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.050897 function-tools-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)    13457 2023-08-06 20:45:45.000000 function-tools-0.5.0/CHANGES.md
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-02-16 11:53:12.000000 function-tools-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      275 2022-07-12 08:20:24.000000 function-tools-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21905 2023-08-06 20:45:53.051897 function-tools-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7804 2022-02-16 11:53:12.000000 function-tools-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.010897 function-tools-0.5.0/function_tools/
+-rw-r--r--   0 root         (0) root         (0)       63 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      257 2023-08-04 12:26:47.000000 function-tools-0.5.0/function_tools/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-08-04 12:26:47.000000 function-tools-0.5.0/function_tools/apps.py
+-rw-r--r--   0 root         (0) root         (0)    21559 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/caches.py
+-rw-r--r--   0 root         (0) root         (0)      114 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/consts.py
+-rw-r--r--   0 root         (0) root         (0)      458 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      245 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/enums.py
+-rw-r--r--   0 root         (0) root         (0)      451 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.012897 function-tools-0.5.0/function_tools/function_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.038897 function-tools-0.5.0/function_tools/function_templates/function_sync_template/
+-rw-r--r--   0 root         (0) root         (0)      271 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/README.md
+-rw-r--r--   0 root         (0) root         (0)       92 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/__init__.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      329 2022-07-13 10:58:16.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/apps.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/caches.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/consts.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       93 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/enums.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      257 2022-07-12 08:20:24.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/errors.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/functions.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1310 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/helpers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     1601 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/managers.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      326 2022-07-12 08:20:24.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/presenters.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      609 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/results.py-tpl
+-rw-r--r--   0 root         (0) root         (0)     2841 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/runners.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      181 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/strings.py-tpl
+-rw-r--r--   0 root         (0) root         (0)       59 2022-07-05 13:57:48.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/tests.py-tpl
+-rw-r--r--   0 root         (0) root         (0)      911 2022-07-13 12:17:45.000000 function-tools-0.5.0/function_tools/function_templates/function_sync_template/validators.py-tpl
+-rw-r--r--   0 root         (0) root         (0)    11415 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5573 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/general.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.041897 function-tools-0.5.0/function_tools/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.044897 function-tools-0.5.0/function_tools/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2022-07-27 13:25:54.000000 function-tools-0.5.0/function_tools/management/commands/register_entities.py
+-rw-r--r--   0 root         (0) root         (0)    17850 2023-08-04 12:26:47.000000 function-tools-0.5.0/function_tools/management/commands/startfunction.py
+-rw-r--r--   0 root         (0) root         (0)       52 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/management/consts.py
+-rw-r--r--   0 root         (0) root         (0)      598 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/management/strategies.py
+-rw-r--r--   0 root         (0) root         (0)     4957 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/managers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.050897 function-tools-0.5.0/function_tools/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1124 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/migrations/0002_registeredfunction_tags.py
+-rw-r--r--   0 root         (0) root         (0)      795 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/migrations/0003_implementationstrategy.py
+-rw-r--r--   0 root         (0) root         (0)      477 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/migrations/0004_implementationstrategy_order_number.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/migrations/0005_auto_20220724_0050.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-12 12:03:22.000000 function-tools-0.5.0/function_tools/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2022-11-01 12:27:02.000000 function-tools-0.5.0/function_tools/models.py
+-rw-r--r--   0 root         (0) root         (0)      685 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      369 2022-07-27 13:25:54.000000 function-tools-0.5.0/function_tools/receivers.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/results.py
+-rw-r--r--   0 root         (0) root         (0)    13093 2023-08-06 20:45:45.000000 function-tools-0.5.0/function_tools/runners.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2023-08-04 12:26:47.000000 function-tools-0.5.0/function_tools/storages.py
+-rw-r--r--   0 root         (0) root         (0)    17851 2022-07-25 11:47:49.000000 function-tools-0.5.0/function_tools/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      693 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/strings.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/types.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2022-03-03 06:03:15.000000 function-tools-0.5.0/function_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)      408 2022-02-16 11:53:12.000000 function-tools-0.5.0/function_tools/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:45:53.012897 function-tools-0.5.0/function_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21905 2023-08-06 20:45:52.000000 function-tools-0.5.0/function_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-08-06 20:45:52.000000 function-tools-0.5.0/function_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:45:52.000000 function-tools-0.5.0/function_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-06 20:45:52.000000 function-tools-0.5.0/function_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-06 20:45:52.000000 function-tools-0.5.0/function_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2022-07-05 13:57:48.000000 function-tools-0.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-06 20:45:53.051897 function-tools-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-08-06 20:45:45.000000 function-tools-0.5.0/setup.py
```

### Comparing `function-tools-0.4.0/CHANGES.md` & `function-tools-0.5.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,35 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.5.0] - 2023-08-06
+ 
+Добавление точек расширения для увеличения гибкости реализуемых решений. Добавлена функциональность отложенного 
+заполнения кешей.
+ 
+### Добавлено
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлена функциональность отложенного заполнения кешей.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлен интерфейс кешей для унификации их структуры.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлены точки расширения RunnableObject.
+ 
+### Изменено
+ 
+### Исправлено
+
+
 ## [0.4.0] - 2023-08-04
  
 Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
  
 ### Добавлено
 - [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
   MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
```

### Comparing `function-tools-0.4.0/LICENSE` & `function-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/PKG-INFO` & `function-tools-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -122,14 +122,35 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.5.0] - 2023-08-06
+ 
+Добавление точек расширения для увеличения гибкости реализуемых решений. Добавлена функциональность отложенного 
+заполнения кешей.
+ 
+### Добавлено
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлена функциональность отложенного заполнения кешей.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлен интерфейс кешей для унификации их структуры.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлены точки расширения RunnableObject.
+ 
+### Изменено
+ 
+### Исправлено
+
+
 ## [0.4.0] - 2023-08-04
  
 Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
  
 ### Добавлено
 - [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
   MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
```

### Comparing `function-tools-0.4.0/README.md` & `function-tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/apps.py` & `function-tools-0.5.0/function_tools/apps.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/caches.py` & `function-tools-0.5.0/function_tools/caches.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,57 @@
     date2str,
     deep_getattr,
 )
 
 
 class BaseCache:
     """
-    Кеш-заглушка
+    Кеш-заглушка.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__()
 
+        # Кеш подготовлен к работе
+        self.__is_prepared = False
+
+    @property
+    def is_prepared(self) -> bool:
+        """Кеш уже подготовлен."""
+        return self.__is_prepared
+
+    @is_prepared.setter
+    def is_prepared(self, value: bool):
+        """Отметка кеша о готовности."""
+        self.__is_prepared = value
+
+    def _before_prepare(self, *args, **kwargs):
+        """Действия перед подготовкой кеша."""
+
+    def _prepare(self, *args, **kwargs):
+        """Заполнение кеша данными."""
+
+    def _after_prepare(self, *args, **kwargs):
+        """Действия после подготовки кеша."""
+
+    def _check_cache_prepared(self):
+        """Проверка, был ли подготовлен кеш ранее или нет."""
+        if self.is_prepared:
+            raise RuntimeError('Cache can not be prepared twice. Please check using method "prepare".')
+
+    def prepare(self, *args, **kwargs):
+        """"""
+        self._check_cache_prepared()
+
+        self._before_prepare(*args, **kwargs)
+        self._prepare(*args, **kwargs)
+        self._after_prepare(*args, **kwargs)
+
+        self.is_prepared = True
+
 
 class EntityCache(BaseCache):
     """
     Базовый класс кеша объектов сущности
     """
 
     def __init__(
@@ -84,18 +121,14 @@
         )
 
         self._additional_filter_params = additional_filter_params or {}
 
         self._entities = None
         self._entities_hash_table = None
 
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
-
     def __repr__(self):
         return (
             f'<{self.__class__.__name__} @model="{self._model.__name__}" '
             f'@searching_key="{self._searching_key}">'
         )
 
     def __str__(self):
@@ -105,27 +138,27 @@
     def entities(self) -> Union[QueryType[Model], List[Model]]:
         """
         Возвращает список объектов либо QuerySet в зависимости от подхода к
         получению объектов
         """
         return self._entities
 
-    def _before_prepare(self):
+    def _before_prepare(self, *args, **kwargs):
         """
         Точка расширения перед подготовкой кеша
         """
         pass
 
-    def _after_prepare(self):
+    def _after_prepare(self, *args, **kwargs):
         """
         Точка расширения после подготовки кеша
         """
         pass
 
-    def _prepare(self):
+    def _prepare(self, *args, **kwargs):
         """
         Метод подготовки кеша
         """
         self._prepare_entities()
         self._prepare_entities_hash_table()
 
     def _prepare_entities(self):
@@ -414,18 +447,14 @@
 
         self._date_from = date_from
         self._date_to = date_to
 
         self._old_entities_cache: Optional[EntityCache] = None
         self._new_entities_cache: Optional[EntityCache] = None
 
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
-
     def __repr__(self):
         return (
             f'<{self.__class__.__name__} @model="{self._model.__name__}" '
             f'@date_from="{date2str(self._date_from)}" '
             f'@date_to="{date2str(self._date_to)}" '
             f'@searching_key="{self._searching_key}">'
         )
@@ -540,27 +569,27 @@
         Формирование кеша объектов модели на конечную дату
         """
         additional_filter_params = self._prepare_new_additional_filter_params()
         self._new_entities_cache = self._prepare_entities_cache(
             additional_filter_params=additional_filter_params,
         )
 
-    def _before_prepare(self):
+    def _before_prepare(self, *args, **kwargs):
         """
         Точка расширения перед формированием кеша
         """
 
-    def _prepare(self):
+    def _prepare(self, *args, **kwargs):
         """
         Формирование кешей на начальную и конечную даты
         """
         self._prepare_old_entities_cache()
         self._prepare_new_entities_cache()
 
-    def _after_prepare(self):
+    def _after_prepare(self, *args, **kwargs):
         """
         Точка расширения после формирования кеша
         """
 
 
 class CacheStorage(BaseCache):
     """
@@ -571,14 +600,26 @@
     Для их объединения и применения в функции создаются хранилища, содержащие кеши в виде публичных свойств, с
     которыми в дальнейшем удобно работать
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+    def prepare(self, *args, **kwargs):
+        """
+        Подготовка хранилища кешей.
+
+        При подготовке хранилища должна быть произведена подготовка всех кешей для работы с ними.
+        """
+        super().prepare(*args, **kwargs)
+
+        for attr_value in self.__dict__.values():
+            if isinstance(attr_value, BaseCache):
+                attr_value.prepare(*args, **kwargs)
+
 
 class PatchedGlobalCacheStorage(CacheStorage):
     """
     Хранилище кешей с функциональностью патчинга кеша или хранилища кешей с использованием глобального (внешнего)
     кеша или хранилища кешей. Пригождается в случае использования глобального хелпера, когда есть необходимость
     создания кеша функции на основе кеша ранера.
     """
```

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/caches.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/results.py-tpl`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from {{ strategy.function_cache_storage_class_module }} import (
-    {{ strategy.function_cache_storage_class_name }},
+from {{ strategy.runner_result_class_module }} import (
+    {{ strategy.runner_result_class_name }},
 )
-from {{ strategy.runner_cache_storage_class_module }} import (
-    {{ strategy.runner_cache_storage_class_name }},
+from {{ strategy.function_result_class_module }} import (
+    {{ strategy.function_result_class_name }},
 )
 
 
-class {{ camel_case_function_name }}RunnerCacheStorage({{ strategy.runner_cache_storage_class_name }}):
+class {{ camel_case_function_name }}RunnerResult({{ strategy.runner_result_class_name }}):
     """
-    Кеш помощника ранера функции "{{ function_verbose_name }}".
+    Результат работы ранера функции "{{ function_verbose_name }}".
     """
 
 
-class {{ camel_case_function_name }}FunctionCacheStorage({{ strategy.function_cache_storage_class_name }}):
+class {{ camel_case_function_name }}FunctionResult({{ strategy.function_result_class_name }}):
     """
-    Кеш помощника функции "{{ function_verbose_name }}".
+    Результат работы функции "{{ function_verbose_name }}".
     """
```

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/functions.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/functions.py-tpl`

 * *Files 5% similar despite different names*

```diff
@@ -73,13 +73,13 @@
 
     def _prepare_result_class(self) -> Type[{{ camel_case_function_name }}FunctionResult]:
         """
         Возвращает класс результата функции.
         """
         return {{ camel_case_function_name }}FunctionResult
 
-    def _prepare(self):
+    def _prepare(self, *args, **kwargs):
         """
         Выполнение действий функции.
         """
         if self.result.has_not_errors:
             pass
```

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/helpers.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/helpers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/managers.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/managers.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/runners.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/runners.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/function_templates/function_sync_template/validators.py-tpl` & `function-tools-0.5.0/function_tools/function_templates/function_sync_template/validators.py-tpl`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/functions.py` & `function-tools-0.5.0/function_tools/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,37 +38,48 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._helper: Union[BaseHelper, BaseFunctionHelper] = self._prepare_helper(*args, **kwargs)
 
-    def _before_prepare(self):
+    def _before_prepare(self, *args, **kwargs):
         """
         Точка расширения функциональности перед фактическим началом работы функции
         """
 
     @abstractmethod
-    def _prepare(self):
+    def _prepare(self, *args, **kwargs):
         """
         Метод содержащий все действия работы функции
         """
 
-    def _after_prepare(self):
+    def _after_prepare(self, *args, **kwargs):
         """
         Точка расширения функциональности после окончания работы функции
         """
 
-    def run(self):
+    def before_run(self, *args, is_force_fill_cache: bool = True, **kwargs):
+        """
+        Действия перед запуском.
+
+        Осуществляется заполнение кеша хелпера, если требовалось заполнить перед запуском. Можно использовать как
+        оптимизацию работы при запуске цепочки из большого количества записей."""
+        super().before_run(*args, **kwargs)
+
+        if not is_force_fill_cache:
+            self.helper.fill_cache(*args, **kwargs)
+
+    def run(self, *args, **kwargs):
         """
         Контрактный метод служащий для запуска функции
         """
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
+        self._before_prepare(*args, **kwargs)
+        self._prepare(*args, **kwargs)
+        self._after_prepare(*args, **kwargs)
 
 
 class BaseGlobalHelperFunction(
     GlobalHelperMixin,
     BaseFunction,
     metaclass=ABCMeta,
 ):
@@ -109,22 +120,22 @@
         """
         if isinstance(object_, (Iterable, Sequence)):
             for act in object_:
                 self.do_on_save(act)
         else:
             self._queue_to_save.append(object_)
 
-    def run(self):
+    def run(self, *args, **kwargs):
         """
         Выполнение действий функции с дальнейшим сохранением объектов в базу
         при отсутствии ошибок или явном указании игнорирования ошибок при сохранении
         """
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
+        self._before_prepare(*args, **kwargs)
+        self._prepare(*args, **kwargs)
+        self._after_prepare(*args, **kwargs)
 
         if self._ignore_errors_on_saving or self.result.has_not_errors:
             self.do_save()
 
 
 class LazySavingPredefinedQueueFunction(
     LazySavingFunction,
@@ -173,22 +184,22 @@
     def do_save(self):
         """
         Выполнение сохранения объектов в зависимости от признака глобального
         сохранения создаваемых объектов функции.
         """
         self._do_save_objects_queue()
 
-    def run(self):
+    def run(self, *args, **kwargs):
         """
         Выполнение действий функции с дальнейшим сохранением объектов в базу
         при отсутствии ошибок и локальном сохранении
         """
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
+        self._before_prepare(*args, **kwargs)
+        self._prepare(*args, **kwargs)
+        self._after_prepare(*args, **kwargs)
 
 
 class LazyDelegateSavingPredefinedQueueGlobalHelperFunction(
     GlobalHelperMixin,
     LazyDelegateSavingPredefinedQueueFunction,
     metaclass=ABCMeta,
 ):
@@ -262,21 +273,21 @@
     """
 
     def do_save(self):
         """
         Сохранение делегировано на уровень ранера.
         """
 
-    def run(self):
+    def run(self, *args, **kwargs):
         """
         Выполнение действий функции с дальнейшим сохранением объектов
         """
-        self._before_prepare()
-        self._prepare()
-        self._after_prepare()
+        self._before_prepare(*args, **kwargs)
+        self._prepare(*args, **kwargs)
+        self._after_prepare(*args, **kwargs)
 
 
 class LazyDelegateSavingSettableQueueGlobalHelperFunction(
     GlobalHelperMixin,
     LazyDelegateSavingSettableQueueFunction,
     metaclass=ABCMeta,
 ):
```

### Comparing `function-tools-0.4.0/function_tools/general.py` & `function-tools-0.5.0/function_tools/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,19 +68,23 @@
 
         return result
 
     def adopt_prev_runnable_result(self, prev_runnable_result):
         """Метод перенимания результата предыдущего ранера."""
         pass
 
+    def before_run(self, *args, **kwargs):
+        """Действия перед запуском."""
+
     @abstractmethod
     def run(self, *args, **kwargs):
-        """
-        Метод запуска выполняемого объекта
-        """
+        """Метод запуска выполняемого объекта."""
+
+    def after_run(self, *args, **kwargs):
+        """Действия выполняемые после запуска."""
 
 
 class LazySavingRunnableObject(
     RunnableObject,
     metaclass=ABCMeta,
 ):
     """
```

### Comparing `function-tools-0.4.0/function_tools/helpers.py` & `function-tools-0.5.0/function_tools/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,31 @@
 )
 
 
 class BaseHelper:
     """
     Базовый класс помощника. Предполагается, что у наследников будут
     создаваться кеши и собираться прочая вспомогательная информация, которая
-    требуется для исполнения действий
+    требуется для исполнения действий.
+
+    is_force_fill_cache указывает, что необходимо наполнить кеш при его инициализации.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, is_force_fill_cache: bool = True, **kwargs):
         super().__init__()
 
         self._cache_class = self._prepare_cache_class()
 
-        self._cache: Union[Optional[BaseCache], Optional[CacheStorage]] = None
+        self._cache: Optional[Union[BaseCache, CacheStorage]] = None
 
         self._prepare_cache(*args, **kwargs)
 
+        if is_force_fill_cache:
+            self.fill_cache()
+
     @property
     def cache(self):
         """
         Возвращает кеш помощника
         """
         return self._cache
 
@@ -47,14 +52,20 @@
         заглушка.
         """
         if issubclass(self._cache_class, (BaseCache, CacheStorage)):
             self._cache = self._cache_class(*args, **kwargs)
         else:
             self._cache = BaseCache(*args, **kwargs)
 
+    def fill_cache(self, *args, **kwargs):
+        """
+        Насыщение кеша данными.
+        """
+        self._cache.prepare(*args, **kwargs)
+
 
 class BaseRunnerHelper(BaseHelper):
     """
     Базовый класс помощника ранера выполнения функций
     """
```

### Comparing `function-tools-0.4.0/function_tools/management/commands/register_entities.py` & `function-tools-0.5.0/function_tools/management/commands/register_entities.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/management/commands/startfunction.py` & `function-tools-0.5.0/function_tools/management/commands/startfunction.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/management/strategies.py` & `function-tools-0.5.0/function_tools/management/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/managers.py` & `function-tools-0.5.0/function_tools/managers.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/migrations/0001_initial.py` & `function-tools-0.5.0/function_tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/migrations/0002_registeredfunction_tags.py` & `function-tools-0.5.0/function_tools/migrations/0002_registeredfunction_tags.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/migrations/0003_implementationstrategy.py` & `function-tools-0.5.0/function_tools/migrations/0003_implementationstrategy.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/migrations/0005_auto_20220724_0050.py` & `function-tools-0.5.0/function_tools/migrations/0005_auto_20220724_0050.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/mixins.py` & `function-tools-0.5.0/function_tools/mixins.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/models.py` & `function-tools-0.5.0/function_tools/models.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/presenters.py` & `function-tools-0.5.0/function_tools/presenters.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/results.py` & `function-tools-0.5.0/function_tools/results.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/runners.py` & `function-tools-0.5.0/function_tools/runners.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,14 +105,26 @@
             self._queue.append(r)
 
     def _update_queue(self):
         """
         Метод позволяет обновлять очередь ранеров на ходу.
         """
 
+    def before_run(self, *args, is_force_fill_cache: bool = True, **kwargs):
+        """
+        Действия перед запуском.
+
+        Осуществляется заполнение кеша хелпера, если требовалось заполнить перед запуском. Можно использовать как
+        оптимизацию работы при запуске цепочки из большого количества записей.
+        """
+        super().before_run(*args, **kwargs)
+
+        if not is_force_fill_cache:
+            self.helper.fill_cache(*args, **kwargs)
+
     def run(self, *args, **kwargs):
         """
         Выполнение всех задач стоящих в очереди.
         """
         self.before_validate()
         self.validate()
         self.after_validate()
@@ -130,15 +142,17 @@
 
                 runnable.adopt_prev_runnable_result(prev_runnable_result=prev_runnable_result)
 
                 runnable.before_validate()
                 runnable.validate()
                 runnable.after_validate()
 
-                runnable.run()
+                runnable.before_run(*args, **kwargs)
+                runnable.run(*args, **kwargs)
+                runnable.after_run(*args, **kwargs)
 
                 prev_runnable_result = runnable.result
 
                 self.result.append_entity(runnable.result)
 
 
 class LazySavingRunner(
@@ -180,15 +194,17 @@
 
                 runnable.adopt_prev_runnable_result(prev_runnable_result=prev_runnable_result)
 
                 runnable.before_validate()
                 runnable.validate()
                 runnable.after_validate()
 
-                runnable.run()
+                runnable.before_run(*args, **kwargs)
+                runnable.run(*args, **kwargs)
+                runnable.after_run(*args, **kwargs)
 
                 prev_runnable_result = runnable.result
 
                 self.result.append_entity(runnable.result)
 
                 if runnable.result.has_not_errors:
                     self._queue_to_save.append(runnable)
@@ -231,15 +247,17 @@
 
                 runnable.adopt_prev_runnable_result(prev_runnable_result=prev_runnable_result)
 
                 runnable.before_validate()
                 runnable.validate()
                 runnable.after_validate()
 
-                runnable.run()
+                runnable.before_run(*args, **kwargs)
+                runnable.run(*args, **kwargs)
+                runnable.after_run(*args, **kwargs)
 
                 prev_runnable_result = runnable.result
 
                 self.result.append_entity(runnable.result)
 
                 if runnable.result.has_not_errors:
                     self._queue_to_save.append(runnable)
```

### Comparing `function-tools-0.4.0/function_tools/storages.py` & `function-tools-0.5.0/function_tools/storages.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/strategies.py` & `function-tools-0.5.0/function_tools/strategies.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/strings.py` & `function-tools-0.5.0/function_tools/strings.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/types.py` & `function-tools-0.5.0/function_tools/types.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools/utils.py` & `function-tools-0.5.0/function_tools/utils.py`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/function_tools.egg-info/PKG-INFO` & `function-tools-0.5.0/function_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-tools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools for creating functions
 Home-page: https://github.com/sandanilenko/function-tools
 Author: Alexander Danilenko
 Author-email: a.danilenko@bars.group
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -122,14 +122,35 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.5.0] - 2023-08-06
+ 
+Добавление точек расширения для увеличения гибкости реализуемых решений. Добавлена функциональность отложенного 
+заполнения кешей.
+ 
+### Добавлено
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлена функциональность отложенного заполнения кешей.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлен интерфейс кешей для унификации их структуры.
+
+- [EDUSCHL-20235](https://jira.bars.group/browse/EDUSCHL-20235)
+  MINOR Добавлены точки расширения RunnableObject.
+ 
+### Изменено
+ 
+### Исправлено
+
+
 ## [0.4.0] - 2023-08-04
  
 Исправление ошибки поиска сущностей function-tools в пакетах, которые не являются django-приложениями.
  
 ### Добавлено
 - [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
   MINOR Добавление параметра FUNCTION_TOOLS_EXCLUDED_APPS для возможности исключения приложений из поиска сущностей.
```

### Comparing `function-tools-0.4.0/function_tools.egg-info/SOURCES.txt` & `function-tools-0.5.0/function_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `function-tools-0.4.0/setup.py` & `function-tools-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import (
     find_packages,
     setup,
 )
 
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

