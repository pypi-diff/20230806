# Comparing `tmp/yambs-2.3.3.tar.gz` & `tmp/yambs-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.3.3.tar", last modified: Sun Aug  6 08:15:23 2023, max compression
+gzip compressed data, was "yambs-2.4.0.tar", last modified: Sun Aug  6 18:53:11 2023, max compression
```

## Comparing `yambs-2.3.3.tar` & `yambs-2.4.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.934909 yambs-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 08:13:08.000000 yambs-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-08-06 08:15:23.934909 yambs-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-08-06 08:13:08.000000 yambs-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 08:13:08.000000 yambs-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 08:15:23.934909 yambs-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-06 08:13:08.000000 yambs-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.914909 yambs-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-06 08:13:08.000000 yambs-2.3.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 08:13:08.000000 yambs-2.3.3/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.918909 yambs-2.3.3/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.918909 yambs-2.3.3/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.918909 yambs-2.3.3/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.922909 yambs-2.3.3/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.922909 yambs-2.3.3/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.922909 yambs-2.3.3/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.926909 yambs-2.3.3/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.926909 yambs-2.3.3/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/handlers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/dependency/handlers/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/handlers/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/handlers/yambs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/handlers/yambs/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.930909 yambs-2.3.3/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-08-06 08:13:08.000000 yambs-2.3.3/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:15:23.918909 yambs-2.3.3/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 08:15:23.000000 yambs-2.3.3/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 18:51:24.000000 yambs-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-08-06 18:53:11.743539 yambs-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-08-06 18:51:24.000000 yambs-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-06 18:51:24.000000 yambs-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:53:11.743539 yambs-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-06 18:51:24.000000 yambs-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.731539 yambs-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-06 18:51:24.000000 yambs-2.4.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 18:51:24.000000 yambs-2.4.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.731539 yambs-2.4.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/handlers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/dependency/handlers/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/handlers/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/handlers/yambs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/handlers/yambs/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.739539 yambs-2.4.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.743539 yambs-2.4.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-08-06 18:51:24.000000 yambs-2.4.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:53:11.735539 yambs-2.4.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 18:53:11.000000 yambs-2.4.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.3.3/LICENSE` & `yambs-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/PKG-INFO` & `yambs-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.3.3
+Version: 2.4.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.3
-    hash=605f8c7be702e2c1acaa6ff990953e10
+    hash=56e5498dfc3e0d2dbd23a5dfbfe11761
     =====================================
 -->
 
-# yambs ([2.3.3](https://pypi.org/project/yambs/))
+# yambs ([2.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.3/README.md` & `yambs-2.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.3
-    hash=605f8c7be702e2c1acaa6ff990953e10
+    hash=56e5498dfc3e0d2dbd23a5dfbfe11761
     =====================================
 -->
 
-# yambs ([2.3.3](https://pypi.org/project/yambs/))
+# yambs ([2.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.3/pyproject.toml` & `yambs-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.3.3"
+version = "2.4.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-2.3.3/setup.py` & `yambs-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/tests/test_entry.py` & `yambs-2.4.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/aggregation/__init__.py` & `yambs-2.4.0/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/app.py` & `yambs-2.4.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/all.py` & `yambs-2.4.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/common.py` & `yambs-2.4.0/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/dist.py` & `yambs-2.4.0/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/gen.py` & `yambs-2.4.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/native.py` & `yambs-2.4.0/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/commands/uf2conv.py` & `yambs-2.4.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/config/__init__.py` & `yambs-2.4.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/config/board.py` & `yambs-2.4.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/config/common.py` & `yambs-2.4.0/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/includes/chips.yaml` & `yambs-2.4.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/includes/infineon.yaml` & `yambs-2.4.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/includes/microchip.yaml` & `yambs-2.4.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/native.yaml` & `yambs-2.4.0/yambs/data/native.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 
 cflag_groups:
   # Compile position-independent to build shared objects.
   pic: [-fPIC]
 
   # Instrument builds for coverage and other analysis.
   debug: [-Og, -g, --coverage]
-  opt: [-O2, -s]
+  opt: [-O2]
   asan: [-fsanitize=address]
   msan: [-fsanitize=memory]
 
+ldflag_groups:
+  opt: [-s]
+
 variants:
 
   debug:
     cflag_groups: [asan]
 
   opt: {}
 
@@ -23,10 +26,11 @@
     cflag_groups: [debug, msan]
     cc: clang
     cxx: clang++
     ld: clang++
 
   clang-opt:
     cflag_groups: [opt]
+    ldflag_groups: [opt]
     cc: clang
     cxx: clang++
     ld: clang++
```

### Comparing `yambs-2.3.3/yambs/data/schemas/Chip.yaml` & `yambs-2.4.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/schemas/Config.yaml` & `yambs-2.4.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/schemas/Native.yaml` & `yambs-2.4.0/yambs/data/schemas/Native.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 
   common_cflags:
     type: array
     default: [-Wall, -Werror, -Wextra, -Wpedantic, -ffunction-sections]
     items:
       type: string
 
-  cflag_groups:
+  cflag_groups: &flag_groups
     type: object
     additionalProperties: false
     patternProperties:
       "^[a-zA-Z0-9-_.]+$":
         type: array
         items:
           type: string
 
+  ldflag_groups: *flag_groups
+
   variants:
     type: object
     additionalProperties: false
     patternProperties:
       "^[a-zA-Z0-9-_.]+$":
         $ref: package://yambs/schemas/Variant.yaml
```

### Comparing `yambs-2.3.3/yambs/data/schemas/config_common.yaml` & `yambs-2.4.0/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.4.0/yambs/data/templates/native_rules.ninja.j2`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 rule cxx
   depfile = $out.d
   deps = gcc
   command = $cxx -MD -MF $out.d $cflags -std=$cxx_standard -c $in -o $out
 {% if common_ldflags %}
 
-ldflags ={% for flag in common_ldflags %} {{flag}}{% endfor %}
+common_ldflags ={% for flag in common_ldflags %} {{flag}}{% endfor %}
 
 {% endif %}
+ldflags = $common_ldflags $variant_ldflags
 
 rule link
   command = $ld $cflags -Wl,-Map=$out.map $in $ldflags -o $out
 
 rule ar
   command = ar rcs $out $in
```

### Comparing `yambs-2.3.3/yambs/data/templates/rules.ninja.j2` & `yambs-2.4.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/data/uf2families.json` & `yambs-2.4.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/config.py` & `yambs-2.4.0/yambs/dependency/config.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/github.py` & `yambs-2.4.0/yambs/dependency/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/handlers/types.py` & `yambs-2.4.0/yambs/dependency/handlers/types.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/handlers/yambs/__init__.py` & `yambs-2.4.0/yambs/dependency/handlers/yambs/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/handlers/yambs/config.py` & `yambs-2.4.0/yambs/dependency/handlers/yambs/config.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/handlers/yambs/github.py` & `yambs-2.4.0/yambs/dependency/handlers/yambs/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dependency/manager.py` & `yambs-2.4.0/yambs/dependency/manager.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/dist/__init__.py` & `yambs-2.4.0/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/entry.py` & `yambs-2.4.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/environment/__init__.py` & `yambs-2.4.0/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/environment/native.py` & `yambs-2.4.0/yambs/environment/native.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,15 +198,18 @@
             )
             self.config.data["common_ldflags"].extend(
                 self.dependency_manager.link_flags
             )
 
             # Render templates.
             generate_variants(
-                self.jinja, self.config, self.config.data["cflag_groups"]
+                self.jinja,
+                self.config,
+                self.config.data["cflag_groups"],
+                self.config.data["ldflag_groups"],
             )
             self.render(self.config.root, "build.ninja")
             for template in ["all", "rules"]:
                 self.render(self.config.ninja_root, f"{template}.ninja")
 
         # Render sources file.
         path = self.config.ninja_root.joinpath("sources.ninja")
```

### Comparing `yambs-2.3.3/yambs/generate/__init__.py` & `yambs-2.4.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/architectures.py` & `yambs-2.4.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/boards.py` & `yambs-2.4.0/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/chips.py` & `yambs-2.4.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/common.py` & `yambs-2.4.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/ninja/__init__.py` & `yambs-2.4.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/ninja/format.py` & `yambs-2.4.0/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/toolchains.py` & `yambs-2.4.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/generate/variants.py` & `yambs-2.4.0/yambs/generate/variants.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,54 +9,66 @@
 # third-party
 from jinja2 import Environment
 
 # internal
 from yambs.config.common import CommonConfig
 from yambs.generate.common import render_template
 
+FlagGroups = Dict[str, List[str]]
+
 
 @contextmanager
 def modified_variant_data(
-    name: str, data: Dict[str, Any], cflag_groups: Dict[str, List[str]]
+    name: str,
+    data: Dict[str, Any],
+    cflag_groups: FlagGroups,
+    ldflag_groups: FlagGroups,
 ) -> Iterator[None]:
     """
     Ensure that cflag groups are processed, and that the variant has access to
     its name while rendering.
     """
 
-    orig = []
-    if "extra_cflags" in data:
-        orig = data["extra_cflags"]
-
-        # Process cflag groups.
-        flags = set(orig + cflag_groups.get(name, []))
-        for group in data["cflag_groups"]:
-            flags |= set(cflag_groups[group])
+    orig_c = data["extra_cflags"]
+    orig_ld = data["extra_ldflags"]
 
-        data["extra_cflags"] = flags
+    # Process cflag groups.
+    flags = set(orig_c + cflag_groups.get(name, []))
+    for group in data["cflag_groups"]:
+        flags |= set(cflag_groups[group])
+    data["extra_cflags"] = flags
+
+    # Process ldflag groups.
+    flags = set(orig_ld + ldflag_groups.get(name, []))
+    for group in data["ldflag_groups"]:
+        flags |= set(ldflag_groups[group])
+    data["extra_ldflags"] = flags
 
+    # Add other useful data.
     data["name"] = name
 
     yield
 
+    # Restore original data.
     del data["name"]
-    if "extra_cflags" in data:
-        data["extra_cflags"] = orig
+    data["extra_cflags"] = orig_c
+    data["extra_ldflags"] = orig_ld
 
 
 def generate(
     jinja: Environment,
     config: CommonConfig,
-    cflag_groups: Dict[str, List[str]],
+    cflag_groups: FlagGroups,
+    ldflag_groups: FlagGroups,
 ) -> None:
     """Generate variant-related ninja files."""
 
     for name, data in config.data["variants"].items():
         variants_root = config.ninja_root.joinpath("variants", name)
         variants_root.mkdir(parents=True, exist_ok=True)
-        with modified_variant_data(name, data, cflag_groups):
+        with modified_variant_data(name, data, cflag_groups, ldflag_groups):
             render_template(
                 jinja,
                 variants_root,
                 "variant.ninja",
                 data,
             )
```

### Comparing `yambs-2.3.3/yambs/github/__init__.py` & `yambs-2.4.0/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/schemas.py` & `yambs-2.4.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/translation/__init__.py` & `yambs-2.4.0/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs/uf2/__init__.py` & `yambs-2.4.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.3.3/yambs.egg-info/PKG-INFO` & `yambs-2.4.0/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.3.3
+Version: 2.4.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.3
-    hash=605f8c7be702e2c1acaa6ff990953e10
+    hash=56e5498dfc3e0d2dbd23a5dfbfe11761
     =====================================
 -->
 
-# yambs ([2.3.3](https://pypi.org/project/yambs/))
+# yambs ([2.4.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.3.3/yambs.egg-info/SOURCES.txt` & `yambs-2.4.0/yambs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

