# Comparing `tmp/datazen-3.1.2.tar.gz` & `tmp/datazen-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazen-3.1.2.tar", last modified: Mon Apr  3 07:07:45 2023, max compression
+gzip compressed data, was "datazen-3.1.3.tar", last modified: Sun Aug  6 07:12:51 2023, max compression
```

## Comparing `datazen-3.1.2.tar` & `datazen-3.1.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.506120 datazen-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-03 07:06:06.000000 datazen-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-03 07:07:45.506120 datazen-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-03 07:06:06.000000 datazen-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.498120 datazen-3.1.2/datazen/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.502120 datazen-3.1.2/datazen/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/file_info_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/target_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/task_data_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/classes/valid_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.502120 datazen-3.1.2/datazen/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/commands/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/commands/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.494120 datazen-3.1.2/datazen/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.502120 datazen-3.1.2/datazen/data/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/data/schema_types/deps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/data/schema_types/paths.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.502120 datazen-3.1.2/datazen/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/data/schemas/manifest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.502120 datazen-3.1.2/datazen/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.506120 datazen-3.1.2/datazen/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/integrated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/manifest_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/environment/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-03 07:06:06.000000 datazen-3.1.2/datazen/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.498120 datazen-3.1.2/datazen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 07:07:45.000000 datazen-3.1.2/datazen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-03 07:06:06.000000 datazen-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 07:07:45.506120 datazen-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-03 07:06:06.000000 datazen-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:07:45.506120 datazen-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-03 07:06:06.000000 datazen-3.1.2/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.724740 datazen-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:11:04.000000 datazen-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-06 07:12:51.724740 datazen-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-08-06 07:11:04.000000 datazen-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/file_info_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/target_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/task_data_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/classes/valid_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/commands/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/commands/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.716740 datazen-3.1.3/datazen/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/data/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/data/schema_types/deps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/data/schema_types/paths.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/data/schemas/manifest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.724740 datazen-3.1.3/datazen/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/integrated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/manifest_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/environment/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-06 07:11:04.000000 datazen-3.1.3/datazen/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.720740 datazen-3.1.3/datazen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 07:12:51.000000 datazen-3.1.3/datazen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-06 07:11:04.000000 datazen-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:12:51.724740 datazen-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-06 07:11:04.000000 datazen-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:51.724740 datazen-3.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-06 07:11:04.000000 datazen-3.1.3/tests/test_variables.py
```

### Comparing `datazen-3.1.2/LICENSE` & `datazen-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/PKG-INFO` & `datazen-3.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: datazen
-Version: 3.1.2
+Version: 3.1.3
 Summary: Compile and render schema-validated configuration data.
 Home-page: https://github.com/vkottler/datazen
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.1
-    hash=4b9615d388d51665e51354af2b12d253
+    version=3.1.2
+    hash=b75e2ba0093fa4965f164f9b41bc7c80
     =====================================
 -->
 
-# datazen ([3.1.2](https://pypi.org/project/datazen/))
+# datazen ([3.1.3](https://pypi.org/project/datazen/))
 
 [![python](https://img.shields.io/pypi/pyversions/datazen.svg)](https://pypi.org/project/datazen/)
 ![Build Status](https://github.com/vkottler/datazen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/datazen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/datazen)
 ![PyPI - Status](https://img.shields.io/pypi/status/datazen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/datazen)
 
 *Compile and render schema-validated configuration data.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/datazen.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/datazen)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/datazen.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
@@ -82,26 +86,26 @@
 * [Commands](#commands)
 * [Renders](#renders)
 * [Groups](#groups)
 
 # Usage
 
 ```
-$ ./venv3.8/bin/dz -h
+$ ./venv3.11/bin/dz -h
 
 usage: dz [-h] [--version] [-v] [-C DIR] [--line-ending {unix,dos,unix}]
           [-m MANIFEST] [-c] [--sync] [-d]
-          [targets [targets ...]]
+          [targets ...]
 
 Compile and render schema-validated configuration data.
 
 positional arguments:
   targets               target(s) to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   --line-ending {unix,dos,unix}
                         line-ending option to use by default (default: 'unix')
   -m MANIFEST, --manifest MANIFEST
@@ -160,19 +164,19 @@
   type: string
 ```
 ## Global Loads
 
 For each of these keys, add paths that should be loaded globally.
 
 ```
-configs:      paths
-schemas:      paths
+configs: paths
+schemas: paths
 schema_types: paths
-templates:    paths
-variables:    paths
+templates: paths
+variables: paths
 ```
 ## Manifest Parameters
 
 Manifests themselves are
 [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) templates that are
 rendered with the data contained in this key.
```

### Comparing `datazen-3.1.2/README.md` & `datazen-3.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 <!--
     =====================================
     generator=datazen
-    version=3.1.1
-    hash=4b9615d388d51665e51354af2b12d253
+    version=3.1.2
+    hash=b75e2ba0093fa4965f164f9b41bc7c80
     =====================================
 -->
 
-# datazen ([3.1.2](https://pypi.org/project/datazen/))
+# datazen ([3.1.3](https://pypi.org/project/datazen/))
 
 [![python](https://img.shields.io/pypi/pyversions/datazen.svg)](https://pypi.org/project/datazen/)
 ![Build Status](https://github.com/vkottler/datazen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/datazen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/datazen)
 ![PyPI - Status](https://img.shields.io/pypi/status/datazen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/datazen)
 
 *Compile and render schema-validated configuration data.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/datazen.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/datazen)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/datazen.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
@@ -58,26 +63,26 @@
 * [Commands](#commands)
 * [Renders](#renders)
 * [Groups](#groups)
 
 # Usage
 
 ```
-$ ./venv3.8/bin/dz -h
+$ ./venv3.11/bin/dz -h
 
 usage: dz [-h] [--version] [-v] [-C DIR] [--line-ending {unix,dos,unix}]
           [-m MANIFEST] [-c] [--sync] [-d]
-          [targets [targets ...]]
+          [targets ...]
 
 Compile and render schema-validated configuration data.
 
 positional arguments:
   targets               target(s) to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   --line-ending {unix,dos,unix}
                         line-ending option to use by default (default: 'unix')
   -m MANIFEST, --manifest MANIFEST
@@ -136,19 +141,19 @@
   type: string
 ```
 ## Global Loads
 
 For each of these keys, add paths that should be loaded globally.
 
 ```
-configs:      paths
-schemas:      paths
+configs: paths
+schemas: paths
 schema_types: paths
-templates:    paths
-variables:    paths
+templates: paths
+variables: paths
 ```
 ## Manifest Parameters
 
 Manifests themselves are
 [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) templates that are
 rendered with the data contained in this key.
```

### Comparing `datazen-3.1.2/datazen/__init__.py` & `datazen-3.1.3/datazen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # =====================================
 # generator=datazen
-# version=3.1.1
-# hash=58d450b1b8ac664ad4c76e5b568cf91f
+# version=3.1.2
+# hash=5556a9ea5670697996e29999640f7636
 # =====================================
 
 """
 Useful defaults and other package metadata.
 """
 
 DESCRIPTION = "Compile and render schema-validated configuration data."
 PKG_NAME = "datazen"
-VERSION = "3.1.2"
+VERSION = "3.1.3"
 
 # datazen-specific content.
 DEFAULT_TYPE = "yaml"
 DEFAULT_MANIFEST = f"manifest.{DEFAULT_TYPE}"
 DEFAULT_DIR = f"{PKG_NAME}-out"
 DEFAULT_INDENT = 2
 CACHE_SUFFIX = "_cache"
```

### Comparing `datazen-3.1.2/datazen/app.py` & `datazen-3.1.3/datazen/app.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/classes/data_repository.py` & `datazen-3.1.3/datazen/classes/data_repository.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/classes/file_info_cache.py` & `datazen-3.1.3/datazen/classes/file_info_cache.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/classes/target_resolver.py` & `datazen-3.1.3/datazen/classes/target_resolver.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/classes/task_data_cache.py` & `datazen-3.1.3/datazen/classes/task_data_cache.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/classes/valid_dict.py` & `datazen-3.1.3/datazen/classes/valid_dict.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/commands/compile.py` & `datazen-3.1.3/datazen/commands/compile.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/commands/render.py` & `datazen-3.1.3/datazen/commands/render.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/compile.py` & `datazen-3.1.3/datazen/compile.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/configs.py` & `datazen-3.1.3/datazen/configs.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/data/schemas/manifest.yaml` & `datazen-3.1.3/datazen/data/schemas/manifest.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # =====================================
 # generator=datazen
-# version=3.1.1
-# hash=4c1dc7e8f5a0bbd708767f446abe2744
+# version=3.1.2
+# hash=96b5e887b1d934d78879c6fedf46154a
 # =====================================
+---
 default_dirs:
   type: boolean
   default: true
 
 includes: paths
 
 output_dir:
   type: string
 
 cache_dir:
   type: string
 
-configs:      paths
-schemas:      paths
+configs: paths
+schemas: paths
 schema_types: paths
-templates:    paths
-variables:    paths
+templates: paths
+variables: paths
 
 params:
   type: dict
 
 default_target:
   type: string
```

### Comparing `datazen-3.1.2/datazen/entry.py` & `datazen-3.1.3/datazen/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # =====================================
 # generator=datazen
-# version=3.1.1
+# version=3.1.2
 # hash=a64ea72f1554bacbcd05e398fef4ba89
 # =====================================
 
 """
 This package's command-line entry-point (boilerplate).
 """
```

### Comparing `datazen-3.1.2/datazen/environment/__init__.py` & `datazen-3.1.3/datazen/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/base.py` & `datazen-3.1.3/datazen/environment/base.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/command.py` & `datazen-3.1.3/datazen/environment/command.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/compile.py` & `datazen-3.1.3/datazen/environment/compile.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/config.py` & `datazen-3.1.3/datazen/environment/config.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/group.py` & `datazen-3.1.3/datazen/environment/group.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/integrated.py` & `datazen-3.1.3/datazen/environment/integrated.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/manifest.py` & `datazen-3.1.3/datazen/environment/manifest.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/manifest_cache.py` & `datazen-3.1.3/datazen/environment/manifest_cache.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/render.py` & `datazen-3.1.3/datazen/environment/render.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/schema.py` & `datazen-3.1.3/datazen/environment/schema.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/task.py` & `datazen-3.1.3/datazen/environment/task.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/template.py` & `datazen-3.1.3/datazen/environment/template.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/environment/variable.py` & `datazen-3.1.3/datazen/environment/variable.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/fingerprinting.py` & `datazen-3.1.3/datazen/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/load.py` & `datazen-3.1.3/datazen/load.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/parsing.py` & `datazen-3.1.3/datazen/parsing.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/paths.py` & `datazen-3.1.3/datazen/paths.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/schemas.py` & `datazen-3.1.3/datazen/schemas.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/targets.py` & `datazen-3.1.3/datazen/targets.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/templates.py` & `datazen-3.1.3/datazen/templates.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen/variables.py` & `datazen-3.1.3/datazen/variables.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/datazen.egg-info/PKG-INFO` & `datazen-3.1.3/datazen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: datazen
-Version: 3.1.2
+Version: 3.1.3
 Summary: Compile and render schema-validated configuration data.
 Home-page: https://github.com/vkottler/datazen
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
-    version=3.1.1
-    hash=4b9615d388d51665e51354af2b12d253
+    version=3.1.2
+    hash=b75e2ba0093fa4965f164f9b41bc7c80
     =====================================
 -->
 
-# datazen ([3.1.2](https://pypi.org/project/datazen/))
+# datazen ([3.1.3](https://pypi.org/project/datazen/))
 
 [![python](https://img.shields.io/pypi/pyversions/datazen.svg)](https://pypi.org/project/datazen/)
 ![Build Status](https://github.com/vkottler/datazen/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/datazen/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/datazen)
 ![PyPI - Status](https://img.shields.io/pypi/status/datazen)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/datazen)
 
 *Compile and render schema-validated configuration data.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/datazen.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/datazen)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/datazen.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
@@ -82,26 +86,26 @@
 * [Commands](#commands)
 * [Renders](#renders)
 * [Groups](#groups)
 
 # Usage
 
 ```
-$ ./venv3.8/bin/dz -h
+$ ./venv3.11/bin/dz -h
 
 usage: dz [-h] [--version] [-v] [-C DIR] [--line-ending {unix,dos,unix}]
           [-m MANIFEST] [-c] [--sync] [-d]
-          [targets [targets ...]]
+          [targets ...]
 
 Compile and render schema-validated configuration data.
 
 positional arguments:
   targets               target(s) to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   --line-ending {unix,dos,unix}
                         line-ending option to use by default (default: 'unix')
   -m MANIFEST, --manifest MANIFEST
@@ -160,19 +164,19 @@
   type: string
 ```
 ## Global Loads
 
 For each of these keys, add paths that should be loaded globally.
 
 ```
-configs:      paths
-schemas:      paths
+configs: paths
+schemas: paths
 schema_types: paths
-templates:    paths
-variables:    paths
+templates: paths
+variables: paths
 ```
 ## Manifest Parameters
 
 Manifests themselves are
 [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) templates that are
 rendered with the data contained in this key.
```

### Comparing `datazen-3.1.2/datazen.egg-info/SOURCES.txt` & `datazen-3.1.3/datazen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/pyproject.toml` & `datazen-3.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "datazen"
-version = "3.1.2"
+version = "3.1.3"
 description = "Compile and render schema-validated configuration data."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
@@ -29,17 +28,20 @@
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
   "pylint",
   "flake8",
-  "pytest",
-  "pytest-cov",
-  "mypy",
   "black",
+  "ruff",
+  "mypy",
   "isort",
-  "setuptools-wrapper"
+  "yamllint",
+  "yambs",
+  "vmklib",
+  "setuptools-wrapper",
+  "pytest"
 ]
 
 [project.scripts]
 dz = "datazen.entry:main"
```

### Comparing `datazen-3.1.2/setup.py` & `datazen-3.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
-# version=3.1.1
-# hash=49f76c2255e92ca83ccc273491bf620b
+# version=3.1.2
+# hash=34b76b9026053b3954ee61e055c724d6
 # =====================================
 
 """
 datazen - Package definition for distribution.
 """
 
 # third-party
@@ -24,15 +24,14 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.7",
         "3.8",
         "3.9",
         "3.10",
         "3.11",
     ],
 }
 setup(
```

### Comparing `datazen-3.1.2/tests/test_configs.py` & `datazen-3.1.3/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/tests/test_entry.py` & `datazen-3.1.3/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/tests/test_parsing.py` & `datazen-3.1.3/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/tests/test_paths.py` & `datazen-3.1.3/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/tests/test_schemas.py` & `datazen-3.1.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `datazen-3.1.2/tests/test_targets.py` & `datazen-3.1.3/tests/test_targets.py`

 * *Files identical despite different names*

