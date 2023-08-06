# Comparing `tmp/heatmap_cli-0.2.2.tar.gz` & `tmp/heatmap_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatmap_cli-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "heatmap_cli-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `heatmap_cli-0.2.2.tar` & `heatmap_cli-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      198 2023-07-29 11:03:01.033125 heatmap_cli-0.2.2/.coveragerc
--rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.gitignore
--rw-r--r--   0        0        0     2589 2023-07-19 03:34:58.303707 heatmap_cli-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.prettierignore
--rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/.python-version
--rw-r--r--   0        0        0     1872 2023-07-30 05:28:45.121770 heatmap_cli-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/LICENSE.md
--rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.2.2/Pipfile
--rw-r--r--   0        0        0   126618 2023-07-24 03:36:11.870630 heatmap_cli-0.2.2/Pipfile.lock
--rw-r--r--   0        0        0     2214 2023-07-29 11:33:39.226367 heatmap_cli-0.2.2/README.md
--rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/Makefile
--rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/LICENSE.md -> ../../LICENSE.md
-lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/_static/logo.jpg
--rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/conf.py
--rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.2.2/docs/source/index.rst
--rw-r--r--   0        0        0      779 2023-07-30 05:28:28.369639 heatmap_cli-0.2.2/heatmap_cli/__init__.py
--rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/heatmap_cli/__main__.py
--rw-r--r--   0        0        0     8735 2023-07-29 12:52:57.238708 heatmap_cli-0.2.2/heatmap_cli/cli.py
--rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.2.2/tests/test_debug_flag.py
--rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_help_flag.py
--rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_verbose_flag.py
--rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.2.2/tests/test_version_flag.py
--rw-r--r--   0        0        0      306 2023-07-19 23:00:14.071564 heatmap_cli-0.2.2/tests/test_week_flag.py
--rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.2.2/tests/test_year_flag.py
--rw-r--r--   0        0        0      678 2023-07-29 11:34:24.338632 heatmap_cli-0.2.2/tox.ini
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 heatmap_cli-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-07-31 02:49:13.458964 heatmap_cli-0.3.0/.coveragerc
+-rw-r--r--   0        0        0     3101 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2620 2023-08-02 02:25:44.140087 heatmap_cli-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       29 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/.python-version
+-rw-r--r--   0        0        0     2283 2023-08-06 07:18:25.958407 heatmap_cli-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1967 2023-07-22 05:51:16.547471 heatmap_cli-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    31956 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0      509 2023-07-21 00:25:50.551442 heatmap_cli-0.3.0/Pipfile
+-rw-r--r--   0        0        0   126619 2023-08-04 03:55:27.463120 heatmap_cli-0.3.0/Pipfile.lock
+-rw-r--r--   0        0        0     4069 2023-08-05 06:49:47.464035 heatmap_cli-0.3.0/README.md
+-rw-r--r--   0        0        0      638 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/LICENSE.md -> ../../LICENSE.md
+lrwxr-xr-x   0        0        0        0 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0    14202 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/_static/logo.jpg
+-rw-r--r--   0        0        0     1555 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      172 2023-07-10 15:24:28.645268 heatmap_cli-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0      779 2023-08-06 07:18:08.062311 heatmap_cli-0.3.0/heatmap_cli/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/heatmap_cli/__main__.py
+-rw-r--r--   0        0        0     9334 2023-08-05 06:52:52.967504 heatmap_cli-0.3.0/heatmap_cli/cli.py
+-rw-r--r--   0        0        0     1077 2023-07-17 23:52:03.000872 heatmap_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     5810 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      473 2023-08-05 06:52:37.286874 heatmap_cli-0.3.0/tests/test_cmap_option.py
+-rw-r--r--   0        0        0      358 2023-07-19 03:58:00.025209 heatmap_cli-0.3.0/tests/test_debug_flag.py
+-rw-r--r--   0        0        0      326 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/test_help_flag.py
+-rw-r--r--   0        0        0      545 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/test_verbose_flag.py
+-rw-r--r--   0        0        0      306 2023-07-10 15:24:28.649268 heatmap_cli-0.3.0/tests/test_version_flag.py
+-rw-r--r--   0        0        0      603 2023-08-05 10:01:18.155732 heatmap_cli-0.3.0/tests/test_week_option.py
+-rw-r--r--   0        0        0      516 2023-07-19 03:33:39.924975 heatmap_cli-0.3.0/tests/test_year_option.py
+-rw-r--r--   0        0        0      661 2023-08-05 04:54:08.045967 heatmap_cli-0.3.0/tox.ini
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 heatmap_cli-0.3.0/PKG-INFO
```

### Comparing `heatmap_cli-0.2.2/.gitignore` & `heatmap_cli-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/.pre-commit-config.yaml` & `heatmap_cli-0.3.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     rev: v4.4.0
     hooks:
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
+      - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.13
     hooks:
@@ -67,15 +68,15 @@
           - --remove-unused-variables
           - --remove-all-unused-imports
         language: python
         files: \.py$
         language_version: python3.11
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
       - id: flake8
         language_version: python3.11
         additional_dependencies:
           - flake8-docstrings
           - flake8-pytest-style
         args:
```

### Comparing `heatmap_cli-0.2.2/CHANGELOG.md` & `heatmap_cli-0.3.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,55 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [0-based versioning](https://0ver.org/).
 
 ## [Unreleased]
 
+## v0.3.0 (2023-08-06)
+
+### Added
+
+- Add additional default hook for `pre-commit`
+- Add `-cm` or `--cmap` option to set a default colormap
+
+### Changed
+
+- Rename test files based on the right term
+- Add missing tests for `-wk` option
+
+### Fixed
+
+- Fix incorrect coverage configs
+- Fix incorrect changelog URL
+
 ## v0.2.2 (2023-07-30)
 
 ### Added
 
-- Add changelog url to help message
+- Add changelog URL to help message
 - Add missing documentation for functions
 
 ### Changed
 
-- Set title and png filename to year only when week is set to 52
+- Set title and PNG filename to year only when week is set to 52
+- Reset DataFrame index after the last filtering step
+- Move some coverage configs to `tox.ini` file
 
 ### Fixed
 
 - Fix incorrect header level in changelog
 - Fix incorrect source module in coverage config file
 
 ## v0.2.1 (2023-07-28)
 
 ### Changed
 
 - Move `coverage` config from `tox` to its own file
-- Reset Dataframe index after filtering
+- Reset DataFrame index after filtering
 
 ### Fixed
 
 - Show verbose log of last date of current week
 - Fix incorrect header level in changelog
 
 ## v0.2.0 (2023-07-23)
```

### Comparing `heatmap_cli-0.2.2/CONTRIBUTING.md` & `heatmap_cli-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/LICENSE.md` & `heatmap_cli-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/Pipfile.lock` & `heatmap_cli-0.3.0/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964344384707287%*

 * *Differences: {"'default'": "{'fonttools': {'hashes': "*

 * *              "['sha256:01cfe02416b6d416c5c8d15e30315cbcd3e97d1b50d3b34b0ce59f742ef55258', "*

 * *              "'sha256:0a1466713e54bdbf5521f2f73eebfe727a528905ff5ec63cda40961b4b1eea95', "*

 * *              "'sha256:0df8ef75ba5791e873c9eac2262196497525e3f07699a2576d3ab9ddf41cb619', "*

 * *              "'sha256:10dac980f2b975ef74532e2a94bb00e97a95b4595fb7f98db493c474d5f54d0e', "*

 * *              "'sha256:150122ed93127a26bc3670ebab7e2add1e0983d30927733aec327ebf4255b072', "*

 * *          […]*

```diff
@@ -67,51 +67,51 @@
                 "sha256:9c87405839a19696e837b3b818fed3f5f69f16f1eec1a1ad77e043dcea9c772f"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.11.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:1df1b6f4c7c4bc8201eb47f3b268adbf2539943aa43c400f84556557e3e109c0",
-                "sha256:2a22b2c425c698dcd5d6b0ff0b566e8e9663172118db6fd5f1941f9b8063da9b",
-                "sha256:33191f062549e6bb1a4782c22a04ebd37009c09360e2d6686ac5083774d06d95",
-                "sha256:38cdecd8f1fd4bf4daae7fed1b3170dfc1b523388d6664b2204b351820aa78a7",
-                "sha256:3ae64303ba670f8959fdaaa30ba0c2dabe75364fdec1caeee596c45d51ca3425",
-                "sha256:3d1f9471134affc1e3b1b806db6e3e2ad3fa99439e332f1881a474c825101096",
-                "sha256:4e3334d51f0e37e2c6056e67141b2adabc92613a968797e2571ca8a03bd64773",
-                "sha256:4edc795533421e98f60acee7d28fc8d941ff5ac10f44668c9c3635ad72ae9045",
-                "sha256:547ab36a799dded58a46fa647266c24d0ed43a66028cd1cd4370b246ad426cac",
-                "sha256:59eba8b2e749a1de85760da22333f3d17c42b66e03758855a12a2a542723c6e7",
-                "sha256:704bccd69b0abb6fab9f5e4d2b75896afa48b427caa2c7988792a2ffce35b441",
-                "sha256:73ef0bb5d60eb02ba4d3a7d23ada32184bd86007cb2de3657cfcb1175325fc83",
-                "sha256:7763316111df7b5165529f4183a334aa24c13cdb5375ffa1dc8ce309c8bf4e5c",
-                "sha256:849ec722bbf7d3501a0e879e57dec1fc54919d31bff3f690af30bb87970f9784",
-                "sha256:891cfc5a83b0307688f78b9bb446f03a7a1ad981690ac8362f50518bc6153975",
-                "sha256:952cb405f78734cf6466252fec42e206450d1a6715746013f64df9cbd4f896fa",
-                "sha256:a7bbb290d13c6dd718ec2c3db46fe6c5f6811e7ea1e07f145fd8468176398224",
-                "sha256:a9b3cc10dc9e0834b6665fd63ae0c6964c6bc3d7166e9bc84772e0edd09f9fa2",
-                "sha256:aaaef294d8e411f0ecb778a0aefd11bb5884c9b8333cc1011bdaf3b58ca4bd75",
-                "sha256:afce2aeb80be72b4da7dd114f10f04873ff512793d13ce0b19d12b2a4c44c0f0",
-                "sha256:b0938ebbeccf7c80bb9a15e31645cf831572c3a33d5cc69abe436e7000c61b14",
-                "sha256:b2d1ee95be42b80d1f002d1ee0a51d7a435ea90d36f1a5ae331be9962ee5a3f1",
-                "sha256:b927e5f466d99c03e6e20961946314b81d6e3490d95865ef88061144d9f62e38",
-                "sha256:bdd729744ae7ecd7f7311ad25d99da4999003dcfe43b436cf3c333d4e68de73d",
-                "sha256:c2071267deaa6d93cb16288613419679c77220543551cbe61da02c93d92df72f",
-                "sha256:cac73bbef7734e78c60949da11c4903ee5837168e58772371bd42a75872f4f82",
-                "sha256:da2c2964bdc827ba6b8a91dc6de792620be4da3922c4cf0599f36a488c07e2b2",
-                "sha256:e16a9449f21a93909c5be2f5ed5246420f2316e94195dbfccb5238aaa38f9751",
-                "sha256:e5c2b0a95a221838991e2f0e455dec1ca3a8cc9cd54febd68cc64d40fdb83669",
-                "sha256:ec453a45778524f925a8f20fd26a3326f398bfc55d534e37bab470c5e415caa1",
-                "sha256:edee0900cf0eedb29d17c7876102d6e5a91ee333882b1f5abc83e85b934cadb5",
-                "sha256:f14f3ccea4cc7dd1b277385adf3c3bf18f9860f87eab9c2fb650b0af16800f55",
-                "sha256:f240d9adf0583ac8fc1646afe7f4ac039022b6f8fa4f1575a2cfa53675360b69",
-                "sha256:f48602c0b3fd79cd83a34c40af565fe6db7ac9085c8823b552e6e751e3a5b8be"
+                "sha256:01cfe02416b6d416c5c8d15e30315cbcd3e97d1b50d3b34b0ce59f742ef55258",
+                "sha256:0a1466713e54bdbf5521f2f73eebfe727a528905ff5ec63cda40961b4b1eea95",
+                "sha256:0df8ef75ba5791e873c9eac2262196497525e3f07699a2576d3ab9ddf41cb619",
+                "sha256:10dac980f2b975ef74532e2a94bb00e97a95b4595fb7f98db493c474d5f54d0e",
+                "sha256:150122ed93127a26bc3670ebab7e2add1e0983d30927733aec327ebf4255b072",
+                "sha256:1f81ed9065b4bd3f4f3ce8e4873cd6a6b3f4e92b1eddefde35d332c6f414acc3",
+                "sha256:27ec3246a088555629f9f0902f7412220c67340553ca91eb540cf247aacb1983",
+                "sha256:2d6dc3fa91414ff4daa195c05f946e6a575bd214821e26d17ca50f74b35b0fe4",
+                "sha256:329341ba3d86a36e482610db56b30705384cb23bd595eac8cbb045f627778e9d",
+                "sha256:3fb2a69870bfe143ec20b039a1c8009e149dd7780dd89554cc8a11f79e5de86b",
+                "sha256:4655c480a1a4d706152ff54f20e20cf7609084016f1df3851cce67cef768f40a",
+                "sha256:48e82d776d2e93f88ca56567509d102266e7ab2fb707a0326f032fe657335238",
+                "sha256:57b68eab183fafac7cd7d464a7bfa0fcd4edf6c67837d14fb09c1c20516cf20b",
+                "sha256:58c1165f9b2662645de9b19a8c8bdd636b36294ccc07e1b0163856b74f10bafc",
+                "sha256:614b1283dca88effd20ee48160518e6de275ce9b5456a3134d5f235523fc5065",
+                "sha256:685a4dd6cf31593b50d6d441feb7781a4a7ef61e19551463e14ed7c527b86f9f",
+                "sha256:6bd7e4777bff1dcb7c4eff4786998422770f3bfbef8be401c5332895517ba3fa",
+                "sha256:703101eb0490fae32baf385385d47787b73d9ea55253df43b487c89ec767e0d7",
+                "sha256:83b98be5d291e08501bd4fc0c4e0f8e6e05b99f3924068b17c5c9972af6fff84",
+                "sha256:8ece1886d12bb36c48c00b2031518877f41abae317e3a55620d38e307d799b7e",
+                "sha256:9c456d1f23deff64ffc8b5b098718e149279abdea4d8692dba69172fb6a0d597",
+                "sha256:9cd2363ea7728496827658682d049ffb2e98525e2247ca64554864a8cc945568",
+                "sha256:a9b55d2a3b360e0c7fc5bd8badf1503ca1c11dd3a1cd20f2c26787ffa145a9c7",
+                "sha256:ae7df0ae9ee2f3f7676b0ff6f4ebe48ad0acaeeeaa0b6839d15dbf0709f2c5ef",
+                "sha256:ae881e484702efdb6cf756462622de81d4414c454edfd950b137e9a7352b3cb9",
+                "sha256:b8600ae7dce6ec3ddfb201abb98c9d53abbf8064d7ac0c8a0d8925e722ccf2a0",
+                "sha256:c36c904ce0322df01e590ba814d5d69e084e985d7e4c2869378671d79662a7d4",
+                "sha256:c8bf88f9e3ce347c716921804ef3a8330cb128284eb6c0b6c4b3574f3c580023",
+                "sha256:d40673b2e927f7cd0819c6f04489dfbeb337b4a7b10fc633c89bf4f34ecb9620",
+                "sha256:d54e600a2bcfa5cdaa860237765c01804a03b08404d6affcd92942fa7315ffba",
+                "sha256:dfe7fa7e607f7e8b58d0c32501a3a7cac148538300626d1b930082c90ae7f6bd",
+                "sha256:e35bed436726194c5e6e094fdfb423fb7afaa0211199f9d245e59e11118c576c",
+                "sha256:f0290ea7f9945174bd4dfd66e96149037441eb2008f3649094f056201d99e293",
+                "sha256:fae4e801b774cc62cecf4a57b1eae4097903fced00c608d9e2bc8f84cd87b54a"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.41.1"
+            "version": "==4.42.0"
         },
         "heatmap-cli": {
             "editable": true,
             "path": "."
         },
         "importlib-resources": {
             "hashes": [
@@ -722,51 +722,51 @@
                 "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.9.0"
         },
         "fonttools": {
             "hashes": [
-                "sha256:1df1b6f4c7c4bc8201eb47f3b268adbf2539943aa43c400f84556557e3e109c0",
-                "sha256:2a22b2c425c698dcd5d6b0ff0b566e8e9663172118db6fd5f1941f9b8063da9b",
-                "sha256:33191f062549e6bb1a4782c22a04ebd37009c09360e2d6686ac5083774d06d95",
-                "sha256:38cdecd8f1fd4bf4daae7fed1b3170dfc1b523388d6664b2204b351820aa78a7",
-                "sha256:3ae64303ba670f8959fdaaa30ba0c2dabe75364fdec1caeee596c45d51ca3425",
-                "sha256:3d1f9471134affc1e3b1b806db6e3e2ad3fa99439e332f1881a474c825101096",
-                "sha256:4e3334d51f0e37e2c6056e67141b2adabc92613a968797e2571ca8a03bd64773",
-                "sha256:4edc795533421e98f60acee7d28fc8d941ff5ac10f44668c9c3635ad72ae9045",
-                "sha256:547ab36a799dded58a46fa647266c24d0ed43a66028cd1cd4370b246ad426cac",
-                "sha256:59eba8b2e749a1de85760da22333f3d17c42b66e03758855a12a2a542723c6e7",
-                "sha256:704bccd69b0abb6fab9f5e4d2b75896afa48b427caa2c7988792a2ffce35b441",
-                "sha256:73ef0bb5d60eb02ba4d3a7d23ada32184bd86007cb2de3657cfcb1175325fc83",
-                "sha256:7763316111df7b5165529f4183a334aa24c13cdb5375ffa1dc8ce309c8bf4e5c",
-                "sha256:849ec722bbf7d3501a0e879e57dec1fc54919d31bff3f690af30bb87970f9784",
-                "sha256:891cfc5a83b0307688f78b9bb446f03a7a1ad981690ac8362f50518bc6153975",
-                "sha256:952cb405f78734cf6466252fec42e206450d1a6715746013f64df9cbd4f896fa",
-                "sha256:a7bbb290d13c6dd718ec2c3db46fe6c5f6811e7ea1e07f145fd8468176398224",
-                "sha256:a9b3cc10dc9e0834b6665fd63ae0c6964c6bc3d7166e9bc84772e0edd09f9fa2",
-                "sha256:aaaef294d8e411f0ecb778a0aefd11bb5884c9b8333cc1011bdaf3b58ca4bd75",
-                "sha256:afce2aeb80be72b4da7dd114f10f04873ff512793d13ce0b19d12b2a4c44c0f0",
-                "sha256:b0938ebbeccf7c80bb9a15e31645cf831572c3a33d5cc69abe436e7000c61b14",
-                "sha256:b2d1ee95be42b80d1f002d1ee0a51d7a435ea90d36f1a5ae331be9962ee5a3f1",
-                "sha256:b927e5f466d99c03e6e20961946314b81d6e3490d95865ef88061144d9f62e38",
-                "sha256:bdd729744ae7ecd7f7311ad25d99da4999003dcfe43b436cf3c333d4e68de73d",
-                "sha256:c2071267deaa6d93cb16288613419679c77220543551cbe61da02c93d92df72f",
-                "sha256:cac73bbef7734e78c60949da11c4903ee5837168e58772371bd42a75872f4f82",
-                "sha256:da2c2964bdc827ba6b8a91dc6de792620be4da3922c4cf0599f36a488c07e2b2",
-                "sha256:e16a9449f21a93909c5be2f5ed5246420f2316e94195dbfccb5238aaa38f9751",
-                "sha256:e5c2b0a95a221838991e2f0e455dec1ca3a8cc9cd54febd68cc64d40fdb83669",
-                "sha256:ec453a45778524f925a8f20fd26a3326f398bfc55d534e37bab470c5e415caa1",
-                "sha256:edee0900cf0eedb29d17c7876102d6e5a91ee333882b1f5abc83e85b934cadb5",
-                "sha256:f14f3ccea4cc7dd1b277385adf3c3bf18f9860f87eab9c2fb650b0af16800f55",
-                "sha256:f240d9adf0583ac8fc1646afe7f4ac039022b6f8fa4f1575a2cfa53675360b69",
-                "sha256:f48602c0b3fd79cd83a34c40af565fe6db7ac9085c8823b552e6e751e3a5b8be"
+                "sha256:01cfe02416b6d416c5c8d15e30315cbcd3e97d1b50d3b34b0ce59f742ef55258",
+                "sha256:0a1466713e54bdbf5521f2f73eebfe727a528905ff5ec63cda40961b4b1eea95",
+                "sha256:0df8ef75ba5791e873c9eac2262196497525e3f07699a2576d3ab9ddf41cb619",
+                "sha256:10dac980f2b975ef74532e2a94bb00e97a95b4595fb7f98db493c474d5f54d0e",
+                "sha256:150122ed93127a26bc3670ebab7e2add1e0983d30927733aec327ebf4255b072",
+                "sha256:1f81ed9065b4bd3f4f3ce8e4873cd6a6b3f4e92b1eddefde35d332c6f414acc3",
+                "sha256:27ec3246a088555629f9f0902f7412220c67340553ca91eb540cf247aacb1983",
+                "sha256:2d6dc3fa91414ff4daa195c05f946e6a575bd214821e26d17ca50f74b35b0fe4",
+                "sha256:329341ba3d86a36e482610db56b30705384cb23bd595eac8cbb045f627778e9d",
+                "sha256:3fb2a69870bfe143ec20b039a1c8009e149dd7780dd89554cc8a11f79e5de86b",
+                "sha256:4655c480a1a4d706152ff54f20e20cf7609084016f1df3851cce67cef768f40a",
+                "sha256:48e82d776d2e93f88ca56567509d102266e7ab2fb707a0326f032fe657335238",
+                "sha256:57b68eab183fafac7cd7d464a7bfa0fcd4edf6c67837d14fb09c1c20516cf20b",
+                "sha256:58c1165f9b2662645de9b19a8c8bdd636b36294ccc07e1b0163856b74f10bafc",
+                "sha256:614b1283dca88effd20ee48160518e6de275ce9b5456a3134d5f235523fc5065",
+                "sha256:685a4dd6cf31593b50d6d441feb7781a4a7ef61e19551463e14ed7c527b86f9f",
+                "sha256:6bd7e4777bff1dcb7c4eff4786998422770f3bfbef8be401c5332895517ba3fa",
+                "sha256:703101eb0490fae32baf385385d47787b73d9ea55253df43b487c89ec767e0d7",
+                "sha256:83b98be5d291e08501bd4fc0c4e0f8e6e05b99f3924068b17c5c9972af6fff84",
+                "sha256:8ece1886d12bb36c48c00b2031518877f41abae317e3a55620d38e307d799b7e",
+                "sha256:9c456d1f23deff64ffc8b5b098718e149279abdea4d8692dba69172fb6a0d597",
+                "sha256:9cd2363ea7728496827658682d049ffb2e98525e2247ca64554864a8cc945568",
+                "sha256:a9b55d2a3b360e0c7fc5bd8badf1503ca1c11dd3a1cd20f2c26787ffa145a9c7",
+                "sha256:ae7df0ae9ee2f3f7676b0ff6f4ebe48ad0acaeeeaa0b6839d15dbf0709f2c5ef",
+                "sha256:ae881e484702efdb6cf756462622de81d4414c454edfd950b137e9a7352b3cb9",
+                "sha256:b8600ae7dce6ec3ddfb201abb98c9d53abbf8064d7ac0c8a0d8925e722ccf2a0",
+                "sha256:c36c904ce0322df01e590ba814d5d69e084e985d7e4c2869378671d79662a7d4",
+                "sha256:c8bf88f9e3ce347c716921804ef3a8330cb128284eb6c0b6c4b3574f3c580023",
+                "sha256:d40673b2e927f7cd0819c6f04489dfbeb337b4a7b10fc633c89bf4f34ecb9620",
+                "sha256:d54e600a2bcfa5cdaa860237765c01804a03b08404d6affcd92942fa7315ffba",
+                "sha256:dfe7fa7e607f7e8b58d0c32501a3a7cac148538300626d1b930082c90ae7f6bd",
+                "sha256:e35bed436726194c5e6e094fdfb423fb7afaa0211199f9d245e59e11118c576c",
+                "sha256:f0290ea7f9945174bd4dfd66e96149037441eb2008f3649094f056201d99e293",
+                "sha256:fae4e801b774cc62cecf4a57b1eae4097903fced00c608d9e2bc8f84cd87b54a"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==4.41.1"
+            "version": "==4.42.0"
         },
         "heatmap-cli": {
             "editable": true,
             "path": "."
         },
         "identify": {
             "hashes": [
@@ -1128,19 +1128,19 @@
                 "sha256:faaf07ea35355b01a35cb442dd950d8f1bb5b040a7787791a535de13db15ed90"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==10.0.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421",
-                "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"
+                "sha256:b45696dab2d7cc691a3226759c0d3b00c47c8b6e293d96f6436f733303f77f6d",
+                "sha256:d7c24979f292f916dc9cbf8648319032f551ea8c49a4c9bf2fb556a02070ec1d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.1"
+            "version": "==3.10.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
                 "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.7'",
@@ -1160,19 +1160,19 @@
                 "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==1.11.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
-                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
+                "sha256:73995fb8216d3bed149c8d51bba25b2c52a8251a2c8ac846ec668ce38fab5413",
+                "sha256:f7b601cbc06fef7e62a754e2b41294c2aa31f1cb659624b9a85bcba29eaf8252"
             ],
             "index": "pypi",
-            "version": "==2.17.4"
+            "version": "==2.17.5"
         },
         "pyparsing": {
             "hashes": [
                 "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb",
                 "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
             "markers": "python_full_version >= '3.6.8'",
@@ -1317,19 +1317,19 @@
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
-                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
+                "sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86",
+                "sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.8"
+            "version": "==0.12.1"
         },
         "tox": {
             "hashes": [
                 "sha256:57b5ab7e8bb3074edc3c0c0b4b192a4f3799d3723b2c5b76f1fa9f2d40316eea",
                 "sha256:d0d28f3fe6d6d7195c27f8b054c3e99d5451952b54abdae673b71609a581f640"
             ],
             "index": "pypi",
@@ -1365,19 +1365,19 @@
                 "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.4"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:01aacf8decd346cf9a865ae85c0cdc7f64c8caa07ff0d8b1dfc1733d10677442",
-                "sha256:2ef6a237c31629da6442b0bcaa3999748108c7166318d1f55cc9f8d7294e97bd"
+                "sha256:43a3052be36080548bdee0b42919c88072037d50d56c28bd3f853cbe92b953ff",
+                "sha256:fd8a78f46f6b99a67b7ec5cf73f92357891a7b3a40fd97637c27f854aae3b9e0"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.24.1"
+            "version": "==20.24.2"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
@@ -1781,19 +1781,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616",
-                "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"
+                "sha256:780f4d32f1d7d1126576e0e5ecc19dc32ab76cd24e950228dcf7b1f6d3d9e22f",
+                "sha256:d170a81825b2fcacb6dfd5a0d7f578a053e45d3f2b153fecc948c37344eb4cbe"
             ],
             "index": "pypi",
-            "version": "==7.0.1"
+            "version": "==7.1.2"
         },
         "sphinx-autodoc-typehints": {
             "hashes": [
                 "sha256:6a73c0c61a9144ce2ed5ef2bed99d615254e5005c1cc32002017d72d69fb70e6",
                 "sha256:94e440066941bb237704bb880785e2d05e8ae5406c88674feefbb938ad0dc6af"
             ],
             "index": "pypi",
```

### Comparing `heatmap_cli-0.2.2/docs/Makefile` & `heatmap_cli-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/docs/make.bat` & `heatmap_cli-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/docs/source/_static/logo.jpg` & `heatmap_cli-0.3.0/docs/source/_static/logo.jpg`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/docs/source/conf.py` & `heatmap_cli-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/heatmap_cli/__init__.py` & `heatmap_cli-0.3.0/heatmap_cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap."""
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
```

### Comparing `heatmap_cli-0.2.2/heatmap_cli/__main__.py` & `heatmap_cli-0.3.0/heatmap_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/heatmap_cli/cli.py` & `heatmap_cli-0.3.0/heatmap_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """A console program that generates yearly calendar heatmap.
 
   website: https://github.com/kianmeng/heatmap_cli
   issues: https://github.com/kianmeng/heatmap_cli/issues
-  changelog: https://github.com/kianmeng/heatmap_cli/issues
+  changelog: https://github.com/kianmeng/heatmap_cli/blog/master/CHANGELOG.md
 """
 
 import argparse
 import datetime
 import logging
 import sys
+from itertools import zip_longest
 from typing import Dict, Optional, Sequence
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 
@@ -50,15 +51,15 @@
         parser (argparse.ArgumentParser)
     """
     parser = argparse.ArgumentParser(
         add_help=False,
         description=__doc__,
         formatter_class=lambda prog: argparse.RawTextHelpFormatter(
             prog,
-            max_help_position=25,
+            max_help_position=6,
         ),
     )
 
     parser.add_argument(
         "input_filename",
         help="csv filename",
         type=argparse.FileType("rb"),
@@ -84,14 +85,34 @@
         help=(
             "filter until week of the year from the CSV file "
             "(default: '%(default)s')"
         ),
         metavar="WEEK",
     )
 
+    # sort in insensitive case
+    cmaps = sorted(plt.colormaps, key=str.casefold)
+    cmap_choices = ""
+    cmap_bygroups = zip_longest(*(iter(cmaps),) * 6)
+    for cmap_bygroup in cmap_bygroups:
+        cmap_choices += ", ".join(filter(None, cmap_bygroup)) + "\n"
+
+    parser.add_argument(
+        "-cm",
+        "--cmap",
+        default="RdYlGn_r",
+        choices=plt.colormaps,
+        dest="cmap",
+        help=(
+            "set default color map (default: '%(default)s')\n"
+            f"{cmap_choices}"
+        ),
+        metavar="COLORMAP",
+    )
+
     parser.add_argument(
         "-d",
         "--debug",
         default=False,
         action="store_true",
         dest="debug",
         help="show debugging log and stacktrace",
@@ -215,60 +236,59 @@
     Returns:
         None
     """
     # generating matplotlib graphs without a x-server
     # see http://stackoverflow.com/a/4935945
     mpl.use("Agg")
 
-    cmap = "RdYlGn_r"
     _fig, axis = plt.subplots(figsize=(8, 5))
     axis.tick_params(axis="both", which="major", labelsize=9)
     axis.tick_params(axis="both", which="minor", labelsize=9)
     sns.heatmap(
         dataframe,
         ax=axis,
         annot=True,
         annot_kws={"fontsize": 9},
         fmt="d",
         linewidth=0.0,
         square=True,
-        cmap=cmap,
+        cmap=config.cmap,
         cbar_kws={
             "orientation": "horizontal",
-            "label": f"colourmap: {cmap}, count: by hundred",
+            "label": f"colourmap: {config.cmap}, count: by hundred",
             "pad": 0.15,
         },
     )
 
-    png_filename = _generate_filename(config, cmap)
+    png_filename = _generate_filename(config)
     plt.title(_generate_title(config), fontsize=10)
     plt.tight_layout()
     plt.savefig(
         png_filename,
         bbox_inches="tight",
         transparent=False,
         dpi=76,
     )
     _logger.info("generate heatmap png file: %s", png_filename)
 
 
-def _generate_filename(config: argparse.Namespace, cmap: str) -> str:
+def _generate_filename(config: argparse.Namespace) -> str:
     """Generate a PNG filename.
 
     Args:
         config (argparse.Namespace): Config from command line arguments
 
     Returns:
         str: A generated file name for the PNG image
     """
     filename = "_annotated_heatmap_of_total_daily_walked_steps_count.png"
     if config.week == 52:
-        return f"{config.year}_{cmap}_" + filename
+        return f"{config.year}_{config.cmap}_" + filename
 
-    return f"{config.year}_week_{config.week}_{cmap}_" + filename
+    return f"{config.year}_week_{config.week}_{config.cmap}_" + filename
 
 
 def _generate_title(config: argparse.Namespace) -> str:
     """Run the main flow.
 
     Args:
         config (argparse.Namespace): Config from command line arguments
```

### Comparing `heatmap_cli-0.2.2/pyproject.toml` & `heatmap_cli-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/tests/conftest.py` & `heatmap_cli-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/tests/fixtures/sample.csv` & `heatmap_cli-0.3.0/tests/fixtures/sample.csv`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/tests/test_verbose_flag.py` & `heatmap_cli-0.3.0/tests/test_verbose_flag.py`

 * *Files identical despite different names*

### Comparing `heatmap_cli-0.2.2/tests/test_year_flag.py` & `heatmap_cli-0.3.0/tests/test_year_option.py`

 * *Files identical despite different names*

